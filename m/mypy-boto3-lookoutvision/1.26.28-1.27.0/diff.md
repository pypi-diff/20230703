# Comparing `tmp/mypy-boto3-lookoutvision-1.26.28.tar.gz` & `tmp/mypy-boto3-lookoutvision-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lookoutvision-1.26.28.tar", last modified: Mon Dec 12 20:27:27 2022, max compression
+gzip compressed data, was "mypy-boto3-lookoutvision-1.27.0.tar", last modified: Mon Jul  3 19:51:03 2023, max compression
```

## Comparing `mypy-boto3-lookoutvision-1.26.28.tar` & `mypy-boto3-lookoutvision-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:27:27.843752 mypy-boto3-lookoutvision-1.26.28/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-12 20:26:49.000000 mypy-boto3-lookoutvision-1.26.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16253 2022-12-12 20:27:27.843752 mypy-boto3-lookoutvision-1.26.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14739 2022-12-12 20:26:49.000000 mypy-boto3-lookoutvision-1.26.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:27:27.843752 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2022-12-12 20:26:49.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2022-12-12 20:26:49.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2022-12-12 20:26:49.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19001 2022-12-12 20:26:49.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18968 2022-12-12 20:26:49.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9019 2022-12-12 20:26:49.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2022-12-12 20:26:49.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2022-12-12 20:26:49.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2022-12-12 20:26:49.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 20:26:49.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26154 2022-12-12 20:26:51.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26113 2022-12-12 20:26:51.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-12 20:26:49.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 20:27:27.843752 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16253 2022-12-12 20:27:27.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2022-12-12 20:27:27.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 20:27:27.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 20:27:27.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-12 20:27:27.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-12 20:27:27.000000 mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 20:27:27.843752 mypy-boto3-lookoutvision-1.26.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2022-12-12 20:26:49.000000 mypy-boto3-lookoutvision-1.26.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.759598 mypy-boto3-lookoutvision-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:23.000000 mypy-boto3-lookoutvision-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16235 2023-07-03 19:51:03.755598 mypy-boto3-lookoutvision-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-07-03 19:41:23.000000 mypy-boto3-lookoutvision-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.747598 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-03 19:41:23.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-03 19:41:23.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 19:41:23.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-07-03 19:41:23.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-07-03 19:41:23.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-03 19:41:23.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-07-03 19:41:23.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-03 19:41:23.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-03 19:41:23.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:23.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26200 2023-07-03 19:41:24.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26159 2023-07-03 19:41:23.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:23.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.755598 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16235 2023-07-03 19:51:03.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 19:51:03.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:03.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 19:51:03.000000 mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:03.759598 mypy-boto3-lookoutvision-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-03 19:41:23.000000 mypy-boto3-lookoutvision-1.27.0/setup.py
```

### Comparing `mypy-boto3-lookoutvision-1.26.28/LICENSE` & `mypy-boto3-lookoutvision-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-lookoutvision-1.26.28/PKG-INFO` & `mypy-boto3-lookoutvision-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutvision
-Version: 1.26.28
-Summary: Type annotations for boto3.LookoutforVision 1.26.28 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.LookoutforVision 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-lookoutvision"></a>
 
 # mypy-boto3-lookoutvision
 
 [![PyPI - mypy-boto3-lookoutvision](https://img.shields.io/pypi/v/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutvision?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutvision)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutforVision 1.26.28](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
+[boto3.LookoutforVision 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lookoutvision docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,68 +345,68 @@
 `mypy_boto3_lookoutvision.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lookoutvision.type_defs import (
     PixelAnomalyTypeDef,
     DatasetMetadataTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectMetadataTypeDef,
     DatasetImageStatsTypeDef,
     InputS3ObjectTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
+    DeleteModelResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
+    DeleteProjectResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeModelPackagingJobRequestRequestTypeDef,
     DescribeModelRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DetectAnomaliesRequestRequestTypeDef,
     ImageSourceTypeDef,
     S3LocationTypeDef,
     TargetPlatformTypeDef,
     GreengrassOutputDetailsTypeDef,
-    PaginatorConfigTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
+    ListDatasetEntriesResponseTypeDef,
+    ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
     ListModelPackagingJobsRequestRequestTypeDef,
     ModelPackagingJobMetadataTypeDef,
+    ListModelsRequestListModelsPaginateTypeDef,
     ListModelsRequestRequestTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModelPerformanceTypeDef,
     OutputS3ObjectTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    StartModelPackagingJobResponseTypeDef,
     StartModelRequestRequestTypeDef,
+    StartModelResponseTypeDef,
     StopModelRequestRequestTypeDef,
+    StopModelResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetEntriesRequestRequestTypeDef,
+    UpdateDatasetEntriesResponseTypeDef,
     AnomalyTypeDef,
-    ProjectDescriptionTypeDef,
     CreateDatasetResponseTypeDef,
-    DeleteModelResponseTypeDef,
-    DeleteProjectResponseTypeDef,
-    ListDatasetEntriesResponseTypeDef,
-    StartModelPackagingJobResponseTypeDef,
-    StartModelResponseTypeDef,
-    StopModelResponseTypeDef,
-    UpdateDatasetEntriesResponseTypeDef,
+    ProjectDescriptionTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateProjectResponseTypeDef,
     ListProjectsResponseTypeDef,
     DatasetDescriptionTypeDef,
     DatasetGroundTruthManifestTypeDef,
     OutputConfigTypeDef,
     GreengrassConfigurationTypeDef,
     ModelPackagingOutputDetailsTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
-    ListModelsRequestListModelsPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ModelMetadataTypeDef,
     DetectAnomalyResultTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DatasetSourceTypeDef,
     CreateModelRequestRequestTypeDef,
@@ -430,42 +430,42 @@
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

### Comparing `mypy-boto3-lookoutvision-1.26.28/README.md` & `mypy-boto3-lookoutvision-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lookoutvision"></a>
 
 # mypy-boto3-lookoutvision
 
 [![PyPI - mypy-boto3-lookoutvision](https://img.shields.io/pypi/v/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutvision?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutvision)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutforVision 1.26.28](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
+[boto3.LookoutforVision 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lookoutvision docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,68 +313,68 @@
 `mypy_boto3_lookoutvision.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lookoutvision.type_defs import (
     PixelAnomalyTypeDef,
     DatasetMetadataTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectMetadataTypeDef,
     DatasetImageStatsTypeDef,
     InputS3ObjectTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
+    DeleteModelResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
+    DeleteProjectResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeModelPackagingJobRequestRequestTypeDef,
     DescribeModelRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DetectAnomaliesRequestRequestTypeDef,
     ImageSourceTypeDef,
     S3LocationTypeDef,
     TargetPlatformTypeDef,
     GreengrassOutputDetailsTypeDef,
-    PaginatorConfigTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
+    ListDatasetEntriesResponseTypeDef,
+    ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
     ListModelPackagingJobsRequestRequestTypeDef,
     ModelPackagingJobMetadataTypeDef,
+    ListModelsRequestListModelsPaginateTypeDef,
     ListModelsRequestRequestTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModelPerformanceTypeDef,
     OutputS3ObjectTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    StartModelPackagingJobResponseTypeDef,
     StartModelRequestRequestTypeDef,
+    StartModelResponseTypeDef,
     StopModelRequestRequestTypeDef,
+    StopModelResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetEntriesRequestRequestTypeDef,
+    UpdateDatasetEntriesResponseTypeDef,
     AnomalyTypeDef,
-    ProjectDescriptionTypeDef,
     CreateDatasetResponseTypeDef,
-    DeleteModelResponseTypeDef,
-    DeleteProjectResponseTypeDef,
-    ListDatasetEntriesResponseTypeDef,
-    StartModelPackagingJobResponseTypeDef,
-    StartModelResponseTypeDef,
-    StopModelResponseTypeDef,
-    UpdateDatasetEntriesResponseTypeDef,
+    ProjectDescriptionTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateProjectResponseTypeDef,
     ListProjectsResponseTypeDef,
     DatasetDescriptionTypeDef,
     DatasetGroundTruthManifestTypeDef,
     OutputConfigTypeDef,
     GreengrassConfigurationTypeDef,
     ModelPackagingOutputDetailsTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
-    ListModelsRequestListModelsPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ModelMetadataTypeDef,
     DetectAnomalyResultTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DatasetSourceTypeDef,
     CreateModelRequestRequestTypeDef,
@@ -398,42 +398,42 @@
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

### Comparing `mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/__init__.py` & `mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/__init__.pyi` & `mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/__main__.py` & `mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LookoutforVision 1.26.28\nVersion:         1.26.28\nBuilder"
-        " version: 7.12.0\nDocs:           "
+        "Type annotations for boto3.LookoutforVision 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.28")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/client.py` & `mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#create_project)
         """
 
     def delete_dataset(
         self, *, ProjectName: str, DatasetType: str, ClientToken: str = ...
     ) -> Dict[str, Any]:
         """
-        Deletes an existing Amazon Lookout for Vision `dataset` .
+        Deletes an existing Amazon Lookout for Vision `dataset`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.delete_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#delete_dataset)
         """
 
     def delete_model(
         self, *, ProjectName: str, ModelVersion: str, ClientToken: str = ...
@@ -293,15 +293,15 @@
         """
 
     def list_projects(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListProjectsResponseTypeDef:
         """
         Lists the Amazon Lookout for Vision projects in your AWS account that are in the
-        AWS Region in which you call `ListProjects` .
+        AWS Region in which you call `ListProjects`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.list_projects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#list_projects)
         """
 
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
```

### Comparing `mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/client.pyi` & `mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#create_project)
         """
     def delete_dataset(
         self, *, ProjectName: str, DatasetType: str, ClientToken: str = ...
     ) -> Dict[str, Any]:
         """
-        Deletes an existing Amazon Lookout for Vision `dataset` .
+        Deletes an existing Amazon Lookout for Vision `dataset`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.delete_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#delete_dataset)
         """
     def delete_model(
         self, *, ProjectName: str, ModelVersion: str, ClientToken: str = ...
     ) -> DeleteModelResponseTypeDef:
@@ -271,15 +271,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#list_models)
         """
     def list_projects(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListProjectsResponseTypeDef:
         """
         Lists the Amazon Lookout for Vision projects in your AWS account that are in the
-        AWS Region in which you call `ListProjects` .
+        AWS Region in which you call `ListProjects`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.list_projects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#list_projects)
         """
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of tags attached to the specified Amazon Lookout for Vision
```

### Comparing `mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/literals.py` & `mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DatasetStatusType",
     "ListDatasetEntriesPaginatorName",
     "ListModelPackagingJobsPaginatorName",
     "ListModelsPaginatorName",
     "ListProjectsPaginatorName",
     "ModelHostingStatusType",
@@ -35,15 +34,14 @@
     "LookoutforVisionServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DatasetStatusType = Literal[
     "CREATE_COMPLETE",
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
     "DELETE_COMPLETE",
     "DELETE_FAILED",
     "DELETE_IN_PROGRESS",
@@ -87,14 +85,15 @@
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
@@ -115,31 +114,34 @@
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
@@ -218,14 +220,15 @@
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
@@ -236,34 +239,38 @@
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
@@ -276,14 +283,15 @@
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
@@ -302,16 +310,19 @@
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
@@ -391,18 +402,21 @@
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

### Comparing `mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/literals.pyi` & `mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DatasetStatusType",
     "ListDatasetEntriesPaginatorName",
     "ListModelPackagingJobsPaginatorName",
     "ListModelsPaginatorName",
     "ListProjectsPaginatorName",
     "ModelHostingStatusType",
@@ -34,14 +35,15 @@
     "LookoutforVisionServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DatasetStatusType = Literal[
     "CREATE_COMPLETE",
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
     "DELETE_COMPLETE",
     "DELETE_FAILED",
     "DELETE_IN_PROGRESS",
@@ -85,14 +87,15 @@
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
@@ -113,31 +116,34 @@
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
@@ -216,14 +222,15 @@
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
@@ -234,34 +241,38 @@
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
@@ -274,14 +285,15 @@
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
@@ -300,16 +312,19 @@
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
@@ -389,18 +404,21 @@
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

### Comparing `mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/paginator.py` & `mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,58 +68,58 @@
         ProjectName: str,
         DatasetType: str,
         Labeled: bool = ...,
         AnomalyClass: str = ...,
         BeforeCreationDate: Union[datetime, str] = ...,
         AfterCreationDate: Union[datetime, str] = ...,
         SourceRefContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListDatasetEntries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listdatasetentriespaginator)
         """
 
 
 class ListModelPackagingJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModelPackagingJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelpackagingjobspaginator)
     """
 
     def paginate(
-        self, *, ProjectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ProjectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListModelPackagingJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModelPackagingJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelpackagingjobspaginator)
         """
 
 
 class ListModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelspaginator)
     """
 
     def paginate(
-        self, *, ProjectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ProjectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelspaginator)
         """
 
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listprojectspaginator)
         """
```

### Comparing `mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/paginator.pyi` & `mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -65,55 +65,55 @@
         ProjectName: str,
         DatasetType: str,
         Labeled: bool = ...,
         AnomalyClass: str = ...,
         BeforeCreationDate: Union[datetime, str] = ...,
         AfterCreationDate: Union[datetime, str] = ...,
         SourceRefContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListDatasetEntries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listdatasetentriespaginator)
         """
 
 class ListModelPackagingJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModelPackagingJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelpackagingjobspaginator)
     """
 
     def paginate(
-        self, *, ProjectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ProjectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListModelPackagingJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModelPackagingJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelpackagingjobspaginator)
         """
 
 class ListModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelspaginator)
     """
 
     def paginate(
-        self, *, ProjectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ProjectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listmodelspaginator)
         """
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/paginators/#listprojectspaginator)
         """
```

### Comparing `mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/type_defs.py` & `mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,68 +34,68 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "PixelAnomalyTypeDef",
     "DatasetMetadataTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectMetadataTypeDef",
     "DatasetImageStatsTypeDef",
     "InputS3ObjectTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
+    "DeleteModelResponseTypeDef",
     "DeleteProjectRequestRequestTypeDef",
+    "DeleteProjectResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeModelPackagingJobRequestRequestTypeDef",
     "DescribeModelRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DetectAnomaliesRequestRequestTypeDef",
     "ImageSourceTypeDef",
     "S3LocationTypeDef",
     "TargetPlatformTypeDef",
     "GreengrassOutputDetailsTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
+    "ListDatasetEntriesResponseTypeDef",
+    "ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
     "ListModelPackagingJobsRequestRequestTypeDef",
     "ModelPackagingJobMetadataTypeDef",
+    "ListModelsRequestListModelsPaginateTypeDef",
     "ListModelsRequestRequestTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModelPerformanceTypeDef",
     "OutputS3ObjectTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartModelPackagingJobResponseTypeDef",
     "StartModelRequestRequestTypeDef",
+    "StartModelResponseTypeDef",
     "StopModelRequestRequestTypeDef",
+    "StopModelResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetEntriesRequestRequestTypeDef",
+    "UpdateDatasetEntriesResponseTypeDef",
     "AnomalyTypeDef",
-    "ProjectDescriptionTypeDef",
     "CreateDatasetResponseTypeDef",
-    "DeleteModelResponseTypeDef",
-    "DeleteProjectResponseTypeDef",
-    "ListDatasetEntriesResponseTypeDef",
-    "StartModelPackagingJobResponseTypeDef",
-    "StartModelResponseTypeDef",
-    "StopModelResponseTypeDef",
-    "UpdateDatasetEntriesResponseTypeDef",
+    "ProjectDescriptionTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateProjectResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetGroundTruthManifestTypeDef",
     "OutputConfigTypeDef",
     "GreengrassConfigurationTypeDef",
     "ModelPackagingOutputDetailsTypeDef",
-    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    "ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
-    "ListModelsRequestListModelsPaginateTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListModelPackagingJobsResponseTypeDef",
     "ModelMetadataTypeDef",
     "DetectAnomalyResultTypeDef",
     "DescribeProjectResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DatasetSourceTypeDef",
     "CreateModelRequestRequestTypeDef",
@@ -127,25 +127,14 @@
         "CreationTimestamp": datetime,
         "Status": DatasetStatusType,
         "StatusMessage": str,
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -252,14 +241,22 @@
 
 class DeleteModelRequestRequestTypeDef(
     _RequiredDeleteModelRequestRequestTypeDef, _OptionalDeleteModelRequestRequestTypeDef
 ):
     pass
 
 
+DeleteModelResponseTypeDef = TypedDict(
+    "DeleteModelResponseTypeDef",
+    {
+        "ModelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteProjectRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalDeleteProjectRequestRequestTypeDef = TypedDict(
@@ -273,14 +270,22 @@
 
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
 
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "ProjectArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -371,24 +376,42 @@
         "ComponentVersionArn": str,
         "ComponentName": str,
         "ComponentVersion": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ProjectName": str,
+        "DatasetType": str,
+    },
+)
+_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "Labeled": bool,
+        "AnomalyClass": str,
+        "BeforeCreationDate": Union[datetime, str],
+        "AfterCreationDate": Union[datetime, str],
+        "SourceRefContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
+    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetEntriesRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -410,14 +433,45 @@
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
 
+ListDatasetEntriesResponseTypeDef = TypedDict(
+    "ListDatasetEntriesResponseTypeDef",
+    {
+        "DatasetEntries": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
+    "_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
+    {
+        "ProjectName": str,
+    },
+)
+_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
+    "_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef(
+    _RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
+    _OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListModelPackagingJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListModelPackagingJobsRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelPackagingJobsRequestRequestTypeDef = TypedDict(
@@ -449,14 +503,36 @@
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+_RequiredListModelsRequestListModelsPaginateTypeDef = TypedDict(
+    "_RequiredListModelsRequestListModelsPaginateTypeDef",
+    {
+        "ProjectName": str,
+    },
+)
+_OptionalListModelsRequestListModelsPaginateTypeDef = TypedDict(
+    "_OptionalListModelsRequestListModelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListModelsRequestListModelsPaginateTypeDef(
+    _RequiredListModelsRequestListModelsPaginateTypeDef,
+    _OptionalListModelsRequestListModelsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListModelsRequestRequestTypeDef = TypedDict(
     "_RequiredListModelsRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelsRequestRequestTypeDef = TypedDict(
@@ -471,14 +547,22 @@
 
 class ListModelsRequestRequestTypeDef(
     _RequiredListModelsRequestRequestTypeDef, _OptionalListModelsRequestRequestTypeDef
 ):
     pass
 
 
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -505,14 +589,43 @@
     "OutputS3ObjectTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
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
+StartModelPackagingJobResponseTypeDef = TypedDict(
+    "StartModelPackagingJobResponseTypeDef",
+    {
+        "JobName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartModelRequestRequestTypeDef = TypedDict(
     "_RequiredStartModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
         "MinInferenceUnits": int,
     },
@@ -529,14 +642,22 @@
 
 class StartModelRequestRequestTypeDef(
     _RequiredStartModelRequestRequestTypeDef, _OptionalStartModelRequestRequestTypeDef
 ):
     pass
 
 
+StartModelResponseTypeDef = TypedDict(
+    "StartModelResponseTypeDef",
+    {
+        "Status": ModelHostingStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStopModelRequestRequestTypeDef = TypedDict(
     "_RequiredStopModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
     },
 )
@@ -551,14 +672,22 @@
 
 class StopModelRequestRequestTypeDef(
     _RequiredStopModelRequestRequestTypeDef, _OptionalStopModelRequestRequestTypeDef
 ):
     pass
 
 
+StopModelResponseTypeDef = TypedDict(
+    "StopModelResponseTypeDef",
+    {
+        "Status": ModelHostingStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -583,104 +712,55 @@
 class UpdateDatasetEntriesRequestRequestTypeDef(
     _RequiredUpdateDatasetEntriesRequestRequestTypeDef,
     _OptionalUpdateDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
 
-AnomalyTypeDef = TypedDict(
-    "AnomalyTypeDef",
+UpdateDatasetEntriesResponseTypeDef = TypedDict(
+    "UpdateDatasetEntriesResponseTypeDef",
     {
-        "Name": str,
-        "PixelAnomaly": PixelAnomalyTypeDef,
+        "Status": DatasetStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ProjectDescriptionTypeDef = TypedDict(
-    "ProjectDescriptionTypeDef",
+AnomalyTypeDef = TypedDict(
+    "AnomalyTypeDef",
     {
-        "ProjectArn": str,
-        "ProjectName": str,
-        "CreationTimestamp": datetime,
-        "Datasets": List[DatasetMetadataTypeDef],
+        "Name": str,
+        "PixelAnomaly": PixelAnomalyTypeDef,
     },
     total=False,
 )
 
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "DatasetMetadata": DatasetMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteModelResponseTypeDef = TypedDict(
-    "DeleteModelResponseTypeDef",
-    {
-        "ModelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
+ProjectDescriptionTypeDef = TypedDict(
+    "ProjectDescriptionTypeDef",
     {
         "ProjectArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDatasetEntriesResponseTypeDef = TypedDict(
-    "ListDatasetEntriesResponseTypeDef",
-    {
-        "DatasetEntries": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartModelPackagingJobResponseTypeDef = TypedDict(
-    "StartModelPackagingJobResponseTypeDef",
-    {
-        "JobName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartModelResponseTypeDef = TypedDict(
-    "StartModelResponseTypeDef",
-    {
-        "Status": ModelHostingStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopModelResponseTypeDef = TypedDict(
-    "StopModelResponseTypeDef",
-    {
-        "Status": ModelHostingStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDatasetEntriesResponseTypeDef = TypedDict(
-    "UpdateDatasetEntriesResponseTypeDef",
-    {
-        "Status": DatasetStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProjectName": str,
+        "CreationTimestamp": datetime,
+        "Datasets": List[DatasetMetadataTypeDef],
     },
+    total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -688,24 +768,24 @@
     },
 )
 
 CreateProjectResponseTypeDef = TypedDict(
     "CreateProjectResponseTypeDef",
     {
         "ProjectMetadata": ProjectMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "Projects": List[ProjectMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatasetDescriptionTypeDef = TypedDict(
     "DatasetDescriptionTypeDef",
     {
         "ProjectName": str,
@@ -765,100 +845,20 @@
     "ModelPackagingOutputDetailsTypeDef",
     {
         "Greengrass": GreengrassOutputDetailsTypeDef,
     },
     total=False,
 )
 
-_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "ProjectName": str,
-        "DatasetType": str,
-    },
-)
-_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "Labeled": bool,
-        "AnomalyClass": str,
-        "BeforeCreationDate": Union[datetime, str],
-        "AfterCreationDate": Union[datetime, str],
-        "SourceRefContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
-    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
-    "_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
-    {
-        "ProjectName": str,
-    },
-)
-_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
-    "_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef(
-    _RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
-    _OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListModelsRequestListModelsPaginateTypeDef = TypedDict(
-    "_RequiredListModelsRequestListModelsPaginateTypeDef",
-    {
-        "ProjectName": str,
-    },
-)
-_OptionalListModelsRequestListModelsPaginateTypeDef = TypedDict(
-    "_OptionalListModelsRequestListModelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListModelsRequestListModelsPaginateTypeDef(
-    _RequiredListModelsRequestListModelsPaginateTypeDef,
-    _OptionalListModelsRequestListModelsPaginateTypeDef,
-):
-    pass
-
-
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListModelPackagingJobsResponseTypeDef = TypedDict(
     "ListModelPackagingJobsResponseTypeDef",
     {
         "ModelPackagingJobs": List[ModelPackagingJobMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModelMetadataTypeDef = TypedDict(
     "ModelMetadataTypeDef",
     {
         "CreationTimestamp": datetime,
@@ -884,23 +884,23 @@
     total=False,
 )
 
 DescribeProjectResponseTypeDef = TypedDict(
     "DescribeProjectResponseTypeDef",
     {
         "ProjectDescription": ProjectDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetDescription": DatasetDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatasetSourceTypeDef = TypedDict(
     "DatasetSourceTypeDef",
     {
         "GroundTruthManifest": DatasetGroundTruthManifestTypeDef,
@@ -961,32 +961,32 @@
     },
 )
 
 CreateModelResponseTypeDef = TypedDict(
     "CreateModelResponseTypeDef",
     {
         "ModelMetadata": ModelMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListModelsResponseTypeDef = TypedDict(
     "ListModelsResponseTypeDef",
     {
         "Models": List[ModelMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectAnomaliesResponseTypeDef = TypedDict(
     "DetectAnomaliesResponseTypeDef",
     {
         "DetectAnomalyResult": DetectAnomalyResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
@@ -1009,15 +1009,15 @@
     pass
 
 
 DescribeModelResponseTypeDef = TypedDict(
     "DescribeModelResponseTypeDef",
     {
         "ModelDescription": ModelDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModelPackagingDescriptionTypeDef = TypedDict(
     "ModelPackagingDescriptionTypeDef",
     {
         "JobName": str,
@@ -1061,10 +1061,10 @@
     pass
 
 
 DescribeModelPackagingJobResponseTypeDef = TypedDict(
     "DescribeModelPackagingJobResponseTypeDef",
     {
         "ModelPackagingDescription": ModelPackagingDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision/type_defs.pyi` & `mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -33,68 +33,68 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "PixelAnomalyTypeDef",
     "DatasetMetadataTypeDef",
-    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectMetadataTypeDef",
     "DatasetImageStatsTypeDef",
     "InputS3ObjectTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
+    "DeleteModelResponseTypeDef",
     "DeleteProjectRequestRequestTypeDef",
+    "DeleteProjectResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeModelPackagingJobRequestRequestTypeDef",
     "DescribeModelRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DetectAnomaliesRequestRequestTypeDef",
     "ImageSourceTypeDef",
     "S3LocationTypeDef",
     "TargetPlatformTypeDef",
     "GreengrassOutputDetailsTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
+    "ListDatasetEntriesResponseTypeDef",
+    "ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
     "ListModelPackagingJobsRequestRequestTypeDef",
     "ModelPackagingJobMetadataTypeDef",
+    "ListModelsRequestListModelsPaginateTypeDef",
     "ListModelsRequestRequestTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModelPerformanceTypeDef",
     "OutputS3ObjectTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartModelPackagingJobResponseTypeDef",
     "StartModelRequestRequestTypeDef",
+    "StartModelResponseTypeDef",
     "StopModelRequestRequestTypeDef",
+    "StopModelResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetEntriesRequestRequestTypeDef",
+    "UpdateDatasetEntriesResponseTypeDef",
     "AnomalyTypeDef",
-    "ProjectDescriptionTypeDef",
     "CreateDatasetResponseTypeDef",
-    "DeleteModelResponseTypeDef",
-    "DeleteProjectResponseTypeDef",
-    "ListDatasetEntriesResponseTypeDef",
-    "StartModelPackagingJobResponseTypeDef",
-    "StartModelResponseTypeDef",
-    "StopModelResponseTypeDef",
-    "UpdateDatasetEntriesResponseTypeDef",
+    "ProjectDescriptionTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateProjectResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetGroundTruthManifestTypeDef",
     "OutputConfigTypeDef",
     "GreengrassConfigurationTypeDef",
     "ModelPackagingOutputDetailsTypeDef",
-    "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    "ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
-    "ListModelsRequestListModelsPaginateTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListModelPackagingJobsResponseTypeDef",
     "ModelMetadataTypeDef",
     "DetectAnomalyResultTypeDef",
     "DescribeProjectResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DatasetSourceTypeDef",
     "CreateModelRequestRequestTypeDef",
@@ -126,25 +126,14 @@
         "CreationTimestamp": datetime,
         "Status": DatasetStatusType,
         "StatusMessage": str,
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -243,14 +232,22 @@
 )
 
 class DeleteModelRequestRequestTypeDef(
     _RequiredDeleteModelRequestRequestTypeDef, _OptionalDeleteModelRequestRequestTypeDef
 ):
     pass
 
+DeleteModelResponseTypeDef = TypedDict(
+    "DeleteModelResponseTypeDef",
+    {
+        "ModelArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteProjectRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalDeleteProjectRequestRequestTypeDef = TypedDict(
@@ -262,14 +259,22 @@
 )
 
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "ProjectArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -356,24 +361,40 @@
         "ComponentVersionArn": str,
         "ComponentName": str,
         "ComponentVersion": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ProjectName": str,
+        "DatasetType": str,
+    },
+)
+_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
+    {
+        "Labeled": bool,
+        "AnomalyClass": str,
+        "BeforeCreationDate": Union[datetime, str],
+        "AfterCreationDate": Union[datetime, str],
+        "SourceRefContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
+    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
+):
+    pass
+
 _RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetEntriesRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -393,14 +414,43 @@
 
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
+ListDatasetEntriesResponseTypeDef = TypedDict(
+    "ListDatasetEntriesResponseTypeDef",
+    {
+        "DatasetEntries": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
+    "_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
+    {
+        "ProjectName": str,
+    },
+)
+_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
+    "_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef(
+    _RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
+    _OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
+):
+    pass
+
 _RequiredListModelPackagingJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListModelPackagingJobsRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelPackagingJobsRequestRequestTypeDef = TypedDict(
@@ -430,14 +480,34 @@
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+_RequiredListModelsRequestListModelsPaginateTypeDef = TypedDict(
+    "_RequiredListModelsRequestListModelsPaginateTypeDef",
+    {
+        "ProjectName": str,
+    },
+)
+_OptionalListModelsRequestListModelsPaginateTypeDef = TypedDict(
+    "_OptionalListModelsRequestListModelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListModelsRequestListModelsPaginateTypeDef(
+    _RequiredListModelsRequestListModelsPaginateTypeDef,
+    _OptionalListModelsRequestListModelsPaginateTypeDef,
+):
+    pass
+
 _RequiredListModelsRequestRequestTypeDef = TypedDict(
     "_RequiredListModelsRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelsRequestRequestTypeDef = TypedDict(
@@ -450,14 +520,22 @@
 )
 
 class ListModelsRequestRequestTypeDef(
     _RequiredListModelsRequestRequestTypeDef, _OptionalListModelsRequestRequestTypeDef
 ):
     pass
 
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -484,14 +562,43 @@
     "OutputS3ObjectTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
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
+StartModelPackagingJobResponseTypeDef = TypedDict(
+    "StartModelPackagingJobResponseTypeDef",
+    {
+        "JobName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartModelRequestRequestTypeDef = TypedDict(
     "_RequiredStartModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
         "MinInferenceUnits": int,
     },
@@ -506,14 +613,22 @@
 )
 
 class StartModelRequestRequestTypeDef(
     _RequiredStartModelRequestRequestTypeDef, _OptionalStartModelRequestRequestTypeDef
 ):
     pass
 
+StartModelResponseTypeDef = TypedDict(
+    "StartModelResponseTypeDef",
+    {
+        "Status": ModelHostingStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStopModelRequestRequestTypeDef = TypedDict(
     "_RequiredStopModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
     },
 )
@@ -526,14 +641,22 @@
 )
 
 class StopModelRequestRequestTypeDef(
     _RequiredStopModelRequestRequestTypeDef, _OptionalStopModelRequestRequestTypeDef
 ):
     pass
 
+StopModelResponseTypeDef = TypedDict(
+    "StopModelResponseTypeDef",
+    {
+        "Status": ModelHostingStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -556,104 +679,55 @@
 
 class UpdateDatasetEntriesRequestRequestTypeDef(
     _RequiredUpdateDatasetEntriesRequestRequestTypeDef,
     _OptionalUpdateDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
-AnomalyTypeDef = TypedDict(
-    "AnomalyTypeDef",
+UpdateDatasetEntriesResponseTypeDef = TypedDict(
+    "UpdateDatasetEntriesResponseTypeDef",
     {
-        "Name": str,
-        "PixelAnomaly": PixelAnomalyTypeDef,
+        "Status": DatasetStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ProjectDescriptionTypeDef = TypedDict(
-    "ProjectDescriptionTypeDef",
+AnomalyTypeDef = TypedDict(
+    "AnomalyTypeDef",
     {
-        "ProjectArn": str,
-        "ProjectName": str,
-        "CreationTimestamp": datetime,
-        "Datasets": List[DatasetMetadataTypeDef],
+        "Name": str,
+        "PixelAnomaly": PixelAnomalyTypeDef,
     },
     total=False,
 )
 
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "DatasetMetadata": DatasetMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteModelResponseTypeDef = TypedDict(
-    "DeleteModelResponseTypeDef",
-    {
-        "ModelArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
+ProjectDescriptionTypeDef = TypedDict(
+    "ProjectDescriptionTypeDef",
     {
         "ProjectArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDatasetEntriesResponseTypeDef = TypedDict(
-    "ListDatasetEntriesResponseTypeDef",
-    {
-        "DatasetEntries": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartModelPackagingJobResponseTypeDef = TypedDict(
-    "StartModelPackagingJobResponseTypeDef",
-    {
-        "JobName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartModelResponseTypeDef = TypedDict(
-    "StartModelResponseTypeDef",
-    {
-        "Status": ModelHostingStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopModelResponseTypeDef = TypedDict(
-    "StopModelResponseTypeDef",
-    {
-        "Status": ModelHostingStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDatasetEntriesResponseTypeDef = TypedDict(
-    "UpdateDatasetEntriesResponseTypeDef",
-    {
-        "Status": DatasetStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ProjectName": str,
+        "CreationTimestamp": datetime,
+        "Datasets": List[DatasetMetadataTypeDef],
     },
+    total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -661,24 +735,24 @@
     },
 )
 
 CreateProjectResponseTypeDef = TypedDict(
     "CreateProjectResponseTypeDef",
     {
         "ProjectMetadata": ProjectMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "Projects": List[ProjectMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatasetDescriptionTypeDef = TypedDict(
     "DatasetDescriptionTypeDef",
     {
         "ProjectName": str,
@@ -736,94 +810,20 @@
     "ModelPackagingOutputDetailsTypeDef",
     {
         "Greengrass": GreengrassOutputDetailsTypeDef,
     },
     total=False,
 )
 
-_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "ProjectName": str,
-        "DatasetType": str,
-    },
-)
-_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
-    {
-        "Labeled": bool,
-        "AnomalyClass": str,
-        "BeforeCreationDate": Union[datetime, str],
-        "AfterCreationDate": Union[datetime, str],
-        "SourceRefContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
-    _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-):
-    pass
-
-_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
-    "_RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
-    {
-        "ProjectName": str,
-    },
-)
-_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef = TypedDict(
-    "_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef(
-    _RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
-    _OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
-):
-    pass
-
-_RequiredListModelsRequestListModelsPaginateTypeDef = TypedDict(
-    "_RequiredListModelsRequestListModelsPaginateTypeDef",
-    {
-        "ProjectName": str,
-    },
-)
-_OptionalListModelsRequestListModelsPaginateTypeDef = TypedDict(
-    "_OptionalListModelsRequestListModelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListModelsRequestListModelsPaginateTypeDef(
-    _RequiredListModelsRequestListModelsPaginateTypeDef,
-    _OptionalListModelsRequestListModelsPaginateTypeDef,
-):
-    pass
-
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListModelPackagingJobsResponseTypeDef = TypedDict(
     "ListModelPackagingJobsResponseTypeDef",
     {
         "ModelPackagingJobs": List[ModelPackagingJobMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModelMetadataTypeDef = TypedDict(
     "ModelMetadataTypeDef",
     {
         "CreationTimestamp": datetime,
@@ -849,23 +849,23 @@
     total=False,
 )
 
 DescribeProjectResponseTypeDef = TypedDict(
     "DescribeProjectResponseTypeDef",
     {
         "ProjectDescription": ProjectDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "DatasetDescription": DatasetDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatasetSourceTypeDef = TypedDict(
     "DatasetSourceTypeDef",
     {
         "GroundTruthManifest": DatasetGroundTruthManifestTypeDef,
@@ -924,32 +924,32 @@
     },
 )
 
 CreateModelResponseTypeDef = TypedDict(
     "CreateModelResponseTypeDef",
     {
         "ModelMetadata": ModelMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListModelsResponseTypeDef = TypedDict(
     "ListModelsResponseTypeDef",
     {
         "Models": List[ModelMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectAnomaliesResponseTypeDef = TypedDict(
     "DetectAnomaliesResponseTypeDef",
     {
         "DetectAnomalyResult": DetectAnomalyResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
@@ -970,15 +970,15 @@
 ):
     pass
 
 DescribeModelResponseTypeDef = TypedDict(
     "DescribeModelResponseTypeDef",
     {
         "ModelDescription": ModelDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModelPackagingDescriptionTypeDef = TypedDict(
     "ModelPackagingDescriptionTypeDef",
     {
         "JobName": str,
@@ -1020,10 +1020,10 @@
 ):
     pass
 
 DescribeModelPackagingJobResponseTypeDef = TypedDict(
     "DescribeModelPackagingJobResponseTypeDef",
     {
         "ModelPackagingDescription": ModelPackagingDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision.egg-info/PKG-INFO` & `mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutvision
-Version: 1.26.28
-Summary: Type annotations for boto3.LookoutforVision 1.26.28 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.LookoutforVision 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-lookoutvision"></a>
 
 # mypy-boto3-lookoutvision
 
 [![PyPI - mypy-boto3-lookoutvision](https://img.shields.io/pypi/v/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutvision?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutvision)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutforVision 1.26.28](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
+[boto3.LookoutforVision 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lookoutvision docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,68 +345,68 @@
 `mypy_boto3_lookoutvision.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lookoutvision.type_defs import (
     PixelAnomalyTypeDef,
     DatasetMetadataTypeDef,
-    ResponseMetadataTypeDef,
     TagTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectMetadataTypeDef,
     DatasetImageStatsTypeDef,
     InputS3ObjectTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
+    DeleteModelResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
+    DeleteProjectResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeModelPackagingJobRequestRequestTypeDef,
     DescribeModelRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DetectAnomaliesRequestRequestTypeDef,
     ImageSourceTypeDef,
     S3LocationTypeDef,
     TargetPlatformTypeDef,
     GreengrassOutputDetailsTypeDef,
-    PaginatorConfigTypeDef,
+    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
+    ListDatasetEntriesResponseTypeDef,
+    ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
     ListModelPackagingJobsRequestRequestTypeDef,
     ModelPackagingJobMetadataTypeDef,
+    ListModelsRequestListModelsPaginateTypeDef,
     ListModelsRequestRequestTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModelPerformanceTypeDef,
     OutputS3ObjectTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
+    StartModelPackagingJobResponseTypeDef,
     StartModelRequestRequestTypeDef,
+    StartModelResponseTypeDef,
     StopModelRequestRequestTypeDef,
+    StopModelResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetEntriesRequestRequestTypeDef,
+    UpdateDatasetEntriesResponseTypeDef,
     AnomalyTypeDef,
-    ProjectDescriptionTypeDef,
     CreateDatasetResponseTypeDef,
-    DeleteModelResponseTypeDef,
-    DeleteProjectResponseTypeDef,
-    ListDatasetEntriesResponseTypeDef,
-    StartModelPackagingJobResponseTypeDef,
-    StartModelResponseTypeDef,
-    StopModelResponseTypeDef,
-    UpdateDatasetEntriesResponseTypeDef,
+    ProjectDescriptionTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateProjectResponseTypeDef,
     ListProjectsResponseTypeDef,
     DatasetDescriptionTypeDef,
     DatasetGroundTruthManifestTypeDef,
     OutputConfigTypeDef,
     GreengrassConfigurationTypeDef,
     ModelPackagingOutputDetailsTypeDef,
-    ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
-    ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
-    ListModelsRequestListModelsPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ModelMetadataTypeDef,
     DetectAnomalyResultTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DatasetSourceTypeDef,
     CreateModelRequestRequestTypeDef,
@@ -430,42 +430,42 @@
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

### Comparing `mypy-boto3-lookoutvision-1.26.28/mypy_boto3_lookoutvision.egg-info/SOURCES.txt` & `mypy-boto3-lookoutvision-1.27.0/mypy_boto3_lookoutvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.26.28/setup.py` & `mypy-boto3-lookoutvision-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-lookoutvision.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lookoutvision",
-    version="1.26.28",
+    version="1.27.0",
     packages=["mypy_boto3_lookoutvision"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LookoutforVision 1.26.28 service generated with"
-        " mypy-boto3-builder 7.12.0"
+        "Type annotations for boto3.LookoutforVision 1.27.0 service generated with"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/",
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


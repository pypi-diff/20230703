# Comparing `tmp/mypy-boto3-sagemaker-geospatial-1.26.20.tar.gz` & `tmp/mypy-boto3-sagemaker-geospatial-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-geospatial-1.26.20.tar", last modified: Wed Nov 30 20:28:44 2022, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-geospatial-1.27.0.tar", last modified: Mon Jul  3 19:51:24 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-geospatial-1.26.20.tar` & `mypy-boto3-sagemaker-geospatial-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 20:28:44.611351 mypy-boto3-sagemaker-geospatial-1.26.20/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-30 20:28:14.000000 mypy-boto3-sagemaker-geospatial-1.26.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    18220 2022-11-30 20:28:44.599351 mypy-boto3-sagemaker-geospatial-1.26.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    16720 2022-11-30 20:28:14.000000 mypy-boto3-sagemaker-geospatial-1.26.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 20:28:44.599351 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/
--rw-r--r--   0 runner    (1001) docker     (122)     1339 2022-11-30 20:28:14.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1338 2022-11-30 20:28:14.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      993 2022-11-30 20:28:14.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18463 2022-11-30 20:28:14.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    18434 2022-11-30 20:28:14.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    10705 2022-11-30 20:28:14.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)    10703 2022-11-30 20:28:14.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     4965 2022-11-30 20:28:14.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4960 2022-11-30 20:28:14.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 20:28:14.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    34428 2022-11-30 20:28:14.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    34385 2022-11-30 20:28:14.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-30 20:28:14.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 20:28:44.599351 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    18220 2022-11-30 20:28:44.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      927 2022-11-30 20:28:44.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 20:28:44.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 20:28:44.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-30 20:28:44.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2022-11-30 20:28:44.000000 mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-30 20:28:44.611351 mypy-boto3-sagemaker-geospatial-1.26.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2090 2022-11-30 20:28:13.000000 mypy-boto3-sagemaker-geospatial-1.26.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:24.135940 mypy-boto3-sagemaker-geospatial-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:47:26.000000 mypy-boto3-sagemaker-geospatial-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18205 2023-07-03 19:51:24.131940 mypy-boto3-sagemaker-geospatial-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16657 2023-07-03 19:47:26.000000 mypy-boto3-sagemaker-geospatial-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:24.127940 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-03 19:47:26.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-03 19:47:26.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-03 19:47:26.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18580 2023-07-03 19:47:26.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18551 2023-07-03 19:47:26.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-03 19:47:26.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-07-03 19:47:26.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-03 19:47:26.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-03 19:47:26.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:47:26.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34431 2023-07-03 19:47:27.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34388 2023-07-03 19:47:26.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:47:26.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:24.127940 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18205 2023-07-03 19:51:23.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 19:51:23.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:23.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:23.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:23.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 19:51:23.000000 mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:24.135940 mypy-boto3-sagemaker-geospatial-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-03 19:47:26.000000 mypy-boto3-sagemaker-geospatial-1.27.0/setup.py
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/LICENSE` & `mypy-boto3-sagemaker-geospatial-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/PKG-INFO` & `mypy-boto3-sagemaker-geospatial-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-geospatial
-Version: 1.26.20
-Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.26.20 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/
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
 
 <a id="mypy-boto3-sagemaker-geospatial"></a>
 
 # mypy-boto3-sagemaker-geospatial
 
 [![PyPI - mypy-boto3-sagemaker-geospatial](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-geospatial?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakergeospatialcapabilities 1.26.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[boto3.SageMakergeospatialcapabilities 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sagemaker-geospatial docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,15 +324,14 @@
     EarthObservationJobStatusType,
     ExportErrorTypeType,
     GroupByType,
     ListEarthObservationJobsPaginatorName,
     ListRasterDataCollectionsPaginatorName,
     ListVectorEnrichmentJobsPaginatorName,
     LogicalOperatorType,
-    MetadataProviderType,
     OutputTypeType,
     PredefinedResolutionType,
     SortOrderType,
     TargetOptionsType,
     TemporalStatisticsType,
     UnitType,
     VectorEnrichmentJobDocumentTypeType,
@@ -367,67 +367,66 @@
     AssetValueTypeDef,
     CloudRemovalConfigInputTypeDef,
     OperationTypeDef,
     DeleteEarthObservationJobInputRequestTypeDef,
     DeleteVectorEnrichmentJobInputRequestTypeDef,
     EarthObservationJobErrorDetailsTypeDef,
     EoCloudCoverInputTypeDef,
-    S3DataInputTypeDef,
-    ResponseMetadataTypeDef,
     ExportErrorDetailsOutputTypeDef,
     ExportS3DataInputTypeDef,
     VectorEnrichmentJobS3DataTypeDef,
     FilterTypeDef,
     GeoMosaicConfigInputTypeDef,
     GeometryTypeDef,
     GetEarthObservationJobInputRequestTypeDef,
     OutputBandTypeDef,
     GetRasterDataCollectionInputRequestTypeDef,
     GetTileInputRequestTypeDef,
+    GetTileOutputTypeDef,
     GetVectorEnrichmentJobInputRequestTypeDef,
     VectorEnrichmentJobErrorDetailsTypeDef,
     VectorEnrichmentJobExportErrorDetailsTypeDef,
     PropertiesTypeDef,
     TemporalStatisticsConfigInputTypeDef,
     ZonalStatisticsConfigInputTypeDef,
     LandsatCloudCoverLandInputTypeDef,
-    PaginatorConfigTypeDef,
+    ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef,
     ListEarthObservationJobInputRequestTypeDef,
     ListEarthObservationJobOutputConfigTypeDef,
+    ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef,
     ListRasterDataCollectionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListVectorEnrichmentJobInputRequestTypeDef,
     ListVectorEnrichmentJobOutputConfigTypeDef,
     MapMatchingConfigTypeDef,
     UserDefinedTypeDef,
+    PaginatorConfigTypeDef,
     PlatformInputTypeDef,
     ViewOffNadirInputTypeDef,
     ViewSunAzimuthInputTypeDef,
     ViewSunElevationInputTypeDef,
     TimeRangeFilterInputTypeDef,
+    TimeRangeFilterOutputTypeDef,
+    ResponseMetadataTypeDef,
     ReverseGeocodingConfigTypeDef,
     StopEarthObservationJobInputRequestTypeDef,
     StopVectorEnrichmentJobInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AreaOfInterestGeometryTypeDef,
     CustomIndicesInputTypeDef,
-    EojDataSourceConfigInputTypeDef,
-    GetTileOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ExportErrorDetailsTypeDef,
     OutputConfigInputTypeDef,
     ExportVectorEnrichmentJobOutputConfigTypeDef,
     VectorEnrichmentJobDataSourceConfigInputTypeDef,
     GetRasterDataCollectionOutputTypeDef,
     RasterDataCollectionMetadataTypeDef,
     ItemSourceTypeDef,
-    ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef,
-    ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef,
-    ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
     OutputResolutionResamplingInputTypeDef,
     OutputResolutionStackInputTypeDef,
     PropertyTypeDef,
     VectorEnrichmentJobConfigTypeDef,
     AreaOfInterestTypeDef,
@@ -466,42 +465,42 @@
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

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/README.md` & `mypy-boto3-sagemaker-geospatial-1.27.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sagemaker-geospatial"></a>
 
 # mypy-boto3-sagemaker-geospatial
 
 [![PyPI - mypy-boto3-sagemaker-geospatial](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-geospatial?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakergeospatialcapabilities 1.26.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[boto3.SageMakergeospatialcapabilities 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sagemaker-geospatial docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/).
 
 See how it helps to find and fix potential bugs:
 
@@ -292,15 +292,14 @@
     EarthObservationJobStatusType,
     ExportErrorTypeType,
     GroupByType,
     ListEarthObservationJobsPaginatorName,
     ListRasterDataCollectionsPaginatorName,
     ListVectorEnrichmentJobsPaginatorName,
     LogicalOperatorType,
-    MetadataProviderType,
     OutputTypeType,
     PredefinedResolutionType,
     SortOrderType,
     TargetOptionsType,
     TemporalStatisticsType,
     UnitType,
     VectorEnrichmentJobDocumentTypeType,
@@ -336,67 +335,66 @@
     AssetValueTypeDef,
     CloudRemovalConfigInputTypeDef,
     OperationTypeDef,
     DeleteEarthObservationJobInputRequestTypeDef,
     DeleteVectorEnrichmentJobInputRequestTypeDef,
     EarthObservationJobErrorDetailsTypeDef,
     EoCloudCoverInputTypeDef,
-    S3DataInputTypeDef,
-    ResponseMetadataTypeDef,
     ExportErrorDetailsOutputTypeDef,
     ExportS3DataInputTypeDef,
     VectorEnrichmentJobS3DataTypeDef,
     FilterTypeDef,
     GeoMosaicConfigInputTypeDef,
     GeometryTypeDef,
     GetEarthObservationJobInputRequestTypeDef,
     OutputBandTypeDef,
     GetRasterDataCollectionInputRequestTypeDef,
     GetTileInputRequestTypeDef,
+    GetTileOutputTypeDef,
     GetVectorEnrichmentJobInputRequestTypeDef,
     VectorEnrichmentJobErrorDetailsTypeDef,
     VectorEnrichmentJobExportErrorDetailsTypeDef,
     PropertiesTypeDef,
     TemporalStatisticsConfigInputTypeDef,
     ZonalStatisticsConfigInputTypeDef,
     LandsatCloudCoverLandInputTypeDef,
-    PaginatorConfigTypeDef,
+    ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef,
     ListEarthObservationJobInputRequestTypeDef,
     ListEarthObservationJobOutputConfigTypeDef,
+    ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef,
     ListRasterDataCollectionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListVectorEnrichmentJobInputRequestTypeDef,
     ListVectorEnrichmentJobOutputConfigTypeDef,
     MapMatchingConfigTypeDef,
     UserDefinedTypeDef,
+    PaginatorConfigTypeDef,
     PlatformInputTypeDef,
     ViewOffNadirInputTypeDef,
     ViewSunAzimuthInputTypeDef,
     ViewSunElevationInputTypeDef,
     TimeRangeFilterInputTypeDef,
+    TimeRangeFilterOutputTypeDef,
+    ResponseMetadataTypeDef,
     ReverseGeocodingConfigTypeDef,
     StopEarthObservationJobInputRequestTypeDef,
     StopVectorEnrichmentJobInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AreaOfInterestGeometryTypeDef,
     CustomIndicesInputTypeDef,
-    EojDataSourceConfigInputTypeDef,
-    GetTileOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ExportErrorDetailsTypeDef,
     OutputConfigInputTypeDef,
     ExportVectorEnrichmentJobOutputConfigTypeDef,
     VectorEnrichmentJobDataSourceConfigInputTypeDef,
     GetRasterDataCollectionOutputTypeDef,
     RasterDataCollectionMetadataTypeDef,
     ItemSourceTypeDef,
-    ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef,
-    ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef,
-    ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
     OutputResolutionResamplingInputTypeDef,
     OutputResolutionStackInputTypeDef,
     PropertyTypeDef,
     VectorEnrichmentJobConfigTypeDef,
     AreaOfInterestTypeDef,
@@ -435,42 +433,42 @@
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

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/__init__.py` & `mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/__init__.pyi` & `mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/__main__.py` & `mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMakergeospatialcapabilities 1.26.20\nVersion:        "
-        " 1.26.20\nBuilder version: 7.11.11\nDocs:           "
+        "Type annotations for boto3.SageMakergeospatialcapabilities 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.20")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/client.py` & `mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,33 +131,36 @@
 
     def export_earth_observation_job(
         self,
         *,
         Arn: str,
         ExecutionRoleArn: str,
         OutputConfig: OutputConfigInputTypeDef,
+        ClientToken: str = ...,
         ExportSourceImages: bool = ...
     ) -> ExportEarthObservationJobOutputTypeDef:
         """
         Use this operation to export results of an Earth Observation job and optionally
-        source images used as input to the EOJ to an S3 location.
+        source images used as input to the EOJ to an Amazon S3 location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.export_earth_observation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/client/#export_earth_observation_job)
         """
 
     def export_vector_enrichment_job(
         self,
         *,
         Arn: str,
         ExecutionRoleArn: str,
-        OutputConfig: ExportVectorEnrichmentJobOutputConfigTypeDef
+        OutputConfig: ExportVectorEnrichmentJobOutputConfigTypeDef,
+        ClientToken: str = ...
     ) -> ExportVectorEnrichmentJobOutputTypeDef:
         """
-        Use this operation to copy results of a Vector Enrichment job to an S3 location.
+        Use this operation to copy results of a Vector Enrichment job to an Amazon S3
+        location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.export_vector_enrichment_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/client/#export_vector_enrichment_job)
         """
 
     def generate_presigned_url(
         self,
@@ -194,14 +197,15 @@
         *,
         Arn: str,
         ImageAssets: Sequence[str],
         Target: TargetOptionsType,
         x: int,
         y: int,
         z: int,
+        ExecutionRoleArn: str = ...,
         ImageMask: bool = ...,
         OutputDataType: OutputTypeType = ...,
         OutputFormat: str = ...,
         PropertyFilters: str = ...,
         TimeRangeFilter: str = ...
     ) -> GetTileOutputTypeDef:
         """
@@ -285,19 +289,19 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.search_raster_data_collection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/client/#search_raster_data_collection)
         """
 
     def start_earth_observation_job(
         self,
         *,
+        ExecutionRoleArn: str,
         InputConfig: InputConfigInputTypeDef,
         JobConfig: JobConfigInputTypeDef,
         Name: str,
         ClientToken: str = ...,
-        ExecutionRoleArn: str = ...,
         KmsKeyId: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> StartEarthObservationJobOutputTypeDef:
         """
         Use this operation to create an Earth observation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.start_earth_observation_job)
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/client.pyi` & `mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -122,32 +122,35 @@
         """
     def export_earth_observation_job(
         self,
         *,
         Arn: str,
         ExecutionRoleArn: str,
         OutputConfig: OutputConfigInputTypeDef,
+        ClientToken: str = ...,
         ExportSourceImages: bool = ...
     ) -> ExportEarthObservationJobOutputTypeDef:
         """
         Use this operation to export results of an Earth Observation job and optionally
-        source images used as input to the EOJ to an S3 location.
+        source images used as input to the EOJ to an Amazon S3 location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.export_earth_observation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/client/#export_earth_observation_job)
         """
     def export_vector_enrichment_job(
         self,
         *,
         Arn: str,
         ExecutionRoleArn: str,
-        OutputConfig: ExportVectorEnrichmentJobOutputConfigTypeDef
+        OutputConfig: ExportVectorEnrichmentJobOutputConfigTypeDef,
+        ClientToken: str = ...
     ) -> ExportVectorEnrichmentJobOutputTypeDef:
         """
-        Use this operation to copy results of a Vector Enrichment job to an S3 location.
+        Use this operation to copy results of a Vector Enrichment job to an Amazon S3
+        location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.export_vector_enrichment_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/client/#export_vector_enrichment_job)
         """
     def generate_presigned_url(
         self,
         ClientMethod: str,
@@ -180,14 +183,15 @@
         *,
         Arn: str,
         ImageAssets: Sequence[str],
         Target: TargetOptionsType,
         x: int,
         y: int,
         z: int,
+        ExecutionRoleArn: str = ...,
         ImageMask: bool = ...,
         OutputDataType: OutputTypeType = ...,
         OutputFormat: str = ...,
         PropertyFilters: str = ...,
         TimeRangeFilter: str = ...
     ) -> GetTileOutputTypeDef:
         """
@@ -264,19 +268,19 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.search_raster_data_collection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/client/#search_raster_data_collection)
         """
     def start_earth_observation_job(
         self,
         *,
+        ExecutionRoleArn: str,
         InputConfig: InputConfigInputTypeDef,
         JobConfig: JobConfigInputTypeDef,
         Name: str,
         ClientToken: str = ...,
-        ExecutionRoleArn: str = ...,
         KmsKeyId: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> StartEarthObservationJobOutputTypeDef:
         """
         Use this operation to create an Earth observation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.start_earth_observation_job)
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/literals.py` & `mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/literals.pyi`

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
     "AlgorithmNameCloudRemovalType",
     "AlgorithmNameGeoMosaicType",
     "AlgorithmNameResamplingType",
     "ComparisonOperatorType",
     "DataCollectionTypeType",
     "EarthObservationJobErrorTypeType",
@@ -30,15 +29,14 @@
     "EarthObservationJobStatusType",
     "ExportErrorTypeType",
     "GroupByType",
     "ListEarthObservationJobsPaginatorName",
     "ListRasterDataCollectionsPaginatorName",
     "ListVectorEnrichmentJobsPaginatorName",
     "LogicalOperatorType",
-    "MetadataProviderType",
     "OutputTypeType",
     "PredefinedResolutionType",
     "SortOrderType",
     "TargetOptionsType",
     "TemporalStatisticsType",
     "UnitType",
     "VectorEnrichmentJobDocumentTypeType",
@@ -51,15 +49,14 @@
     "SageMakergeospatialcapabilitiesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AlgorithmNameCloudRemovalType = Literal["INTERPOLATION"]
 AlgorithmNameGeoMosaicType = Literal[
     "AVERAGE",
     "BILINEAR",
     "CUBIC",
     "CUBICSPLINE",
     "LANCZOS",
@@ -105,15 +102,14 @@
 ]
 ExportErrorTypeType = Literal["CLIENT_ERROR", "SERVER_ERROR"]
 GroupByType = Literal["ALL", "YEARLY"]
 ListEarthObservationJobsPaginatorName = Literal["list_earth_observation_jobs"]
 ListRasterDataCollectionsPaginatorName = Literal["list_raster_data_collections"]
 ListVectorEnrichmentJobsPaginatorName = Literal["list_vector_enrichment_jobs"]
 LogicalOperatorType = Literal["AND"]
-MetadataProviderType = Literal["PLANET_ORDER"]
 OutputTypeType = Literal["FLOAT32", "FLOAT64", "INT16", "INT32", "UINT16"]
 PredefinedResolutionType = Literal["AVERAGE", "HIGHEST", "LOWEST"]
 SortOrderType = Literal["ASCENDING", "DESCENDING"]
 TargetOptionsType = Literal["INPUT", "OUTPUT"]
 TemporalStatisticsType = Literal["MEAN", "MEDIAN", "STANDARD_DEVIATION"]
 UnitType = Literal["METERS"]
 VectorEnrichmentJobDocumentTypeType = Literal["CSV"]
@@ -144,14 +140,15 @@
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
@@ -172,30 +169,34 @@
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
@@ -274,14 +275,15 @@
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
@@ -292,34 +294,38 @@
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
@@ -332,14 +338,15 @@
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
@@ -358,24 +365,28 @@
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
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -404,14 +415,15 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -445,18 +457,21 @@
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

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/literals.pyi` & `mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/literals.py`

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
     "AlgorithmNameCloudRemovalType",
     "AlgorithmNameGeoMosaicType",
     "AlgorithmNameResamplingType",
     "ComparisonOperatorType",
     "DataCollectionTypeType",
     "EarthObservationJobErrorTypeType",
@@ -29,15 +30,14 @@
     "EarthObservationJobStatusType",
     "ExportErrorTypeType",
     "GroupByType",
     "ListEarthObservationJobsPaginatorName",
     "ListRasterDataCollectionsPaginatorName",
     "ListVectorEnrichmentJobsPaginatorName",
     "LogicalOperatorType",
-    "MetadataProviderType",
     "OutputTypeType",
     "PredefinedResolutionType",
     "SortOrderType",
     "TargetOptionsType",
     "TemporalStatisticsType",
     "UnitType",
     "VectorEnrichmentJobDocumentTypeType",
@@ -50,14 +50,15 @@
     "SageMakergeospatialcapabilitiesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AlgorithmNameCloudRemovalType = Literal["INTERPOLATION"]
 AlgorithmNameGeoMosaicType = Literal[
     "AVERAGE",
     "BILINEAR",
     "CUBIC",
     "CUBICSPLINE",
     "LANCZOS",
@@ -103,15 +104,14 @@
 ]
 ExportErrorTypeType = Literal["CLIENT_ERROR", "SERVER_ERROR"]
 GroupByType = Literal["ALL", "YEARLY"]
 ListEarthObservationJobsPaginatorName = Literal["list_earth_observation_jobs"]
 ListRasterDataCollectionsPaginatorName = Literal["list_raster_data_collections"]
 ListVectorEnrichmentJobsPaginatorName = Literal["list_vector_enrichment_jobs"]
 LogicalOperatorType = Literal["AND"]
-MetadataProviderType = Literal["PLANET_ORDER"]
 OutputTypeType = Literal["FLOAT32", "FLOAT64", "INT16", "INT32", "UINT16"]
 PredefinedResolutionType = Literal["AVERAGE", "HIGHEST", "LOWEST"]
 SortOrderType = Literal["ASCENDING", "DESCENDING"]
 TargetOptionsType = Literal["INPUT", "OUTPUT"]
 TemporalStatisticsType = Literal["MEAN", "MEDIAN", "STANDARD_DEVIATION"]
 UnitType = Literal["METERS"]
 VectorEnrichmentJobDocumentTypeType = Literal["CSV"]
@@ -142,14 +142,15 @@
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
@@ -170,30 +171,34 @@
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
@@ -272,14 +277,15 @@
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
@@ -290,34 +296,38 @@
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
@@ -330,14 +340,15 @@
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
@@ -356,24 +367,28 @@
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
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -402,14 +417,15 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -443,18 +459,21 @@
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

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/paginator.py` & `mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/paginator.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -37,71 +37,66 @@
 
 __all__ = (
     "ListEarthObservationJobsPaginator",
     "ListRasterDataCollectionsPaginator",
     "ListVectorEnrichmentJobsPaginator",
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
 class ListEarthObservationJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListEarthObservationJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listearthobservationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: EarthObservationJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEarthObservationJobOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListEarthObservationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listearthobservationjobspaginator)
         """
 
-
 class ListRasterDataCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListRasterDataCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listrasterdatacollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRasterDataCollectionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListRasterDataCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listrasterdatacollectionspaginator)
         """
 
-
 class ListVectorEnrichmentJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListVectorEnrichmentJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listvectorenrichmentjobspaginator)
     """
 
     def paginate(
         self,
         *,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVectorEnrichmentJobOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListVectorEnrichmentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listvectorenrichmentjobspaginator)
         """
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/paginator.pyi` & `mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/paginator.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,66 +37,71 @@
 
 __all__ = (
     "ListEarthObservationJobsPaginator",
     "ListRasterDataCollectionsPaginator",
     "ListVectorEnrichmentJobsPaginator",
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
 class ListEarthObservationJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListEarthObservationJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listearthobservationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: EarthObservationJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEarthObservationJobOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListEarthObservationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listearthobservationjobspaginator)
         """
 
+
 class ListRasterDataCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListRasterDataCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listrasterdatacollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRasterDataCollectionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListRasterDataCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listrasterdatacollectionspaginator)
         """
 
+
 class ListVectorEnrichmentJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListVectorEnrichmentJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listvectorenrichmentjobspaginator)
     """
 
     def paginate(
         self,
         *,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVectorEnrichmentJobOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListVectorEnrichmentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listvectorenrichmentjobspaginator)
         """
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/type_defs.py` & `mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_sagemaker_geospatial.type_defs import MultiPolygonGeometryInputTypeDef
 
     data: MultiPolygonGeometryInputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AlgorithmNameGeoMosaicType,
     AlgorithmNameResamplingType,
     ComparisonOperatorType,
@@ -56,67 +56,66 @@
     "AssetValueTypeDef",
     "CloudRemovalConfigInputTypeDef",
     "OperationTypeDef",
     "DeleteEarthObservationJobInputRequestTypeDef",
     "DeleteVectorEnrichmentJobInputRequestTypeDef",
     "EarthObservationJobErrorDetailsTypeDef",
     "EoCloudCoverInputTypeDef",
-    "S3DataInputTypeDef",
-    "ResponseMetadataTypeDef",
     "ExportErrorDetailsOutputTypeDef",
     "ExportS3DataInputTypeDef",
     "VectorEnrichmentJobS3DataTypeDef",
     "FilterTypeDef",
     "GeoMosaicConfigInputTypeDef",
     "GeometryTypeDef",
     "GetEarthObservationJobInputRequestTypeDef",
     "OutputBandTypeDef",
     "GetRasterDataCollectionInputRequestTypeDef",
     "GetTileInputRequestTypeDef",
+    "GetTileOutputTypeDef",
     "GetVectorEnrichmentJobInputRequestTypeDef",
     "VectorEnrichmentJobErrorDetailsTypeDef",
     "VectorEnrichmentJobExportErrorDetailsTypeDef",
     "PropertiesTypeDef",
     "TemporalStatisticsConfigInputTypeDef",
     "ZonalStatisticsConfigInputTypeDef",
     "LandsatCloudCoverLandInputTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
     "ListEarthObservationJobInputRequestTypeDef",
     "ListEarthObservationJobOutputConfigTypeDef",
+    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
     "ListRasterDataCollectionsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
     "ListVectorEnrichmentJobInputRequestTypeDef",
     "ListVectorEnrichmentJobOutputConfigTypeDef",
     "MapMatchingConfigTypeDef",
     "UserDefinedTypeDef",
+    "PaginatorConfigTypeDef",
     "PlatformInputTypeDef",
     "ViewOffNadirInputTypeDef",
     "ViewSunAzimuthInputTypeDef",
     "ViewSunElevationInputTypeDef",
     "TimeRangeFilterInputTypeDef",
+    "TimeRangeFilterOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "ReverseGeocodingConfigTypeDef",
     "StopEarthObservationJobInputRequestTypeDef",
     "StopVectorEnrichmentJobInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AreaOfInterestGeometryTypeDef",
     "CustomIndicesInputTypeDef",
-    "EojDataSourceConfigInputTypeDef",
-    "GetTileOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ExportErrorDetailsTypeDef",
     "OutputConfigInputTypeDef",
     "ExportVectorEnrichmentJobOutputConfigTypeDef",
     "VectorEnrichmentJobDataSourceConfigInputTypeDef",
     "GetRasterDataCollectionOutputTypeDef",
     "RasterDataCollectionMetadataTypeDef",
     "ItemSourceTypeDef",
-    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
-    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
-    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
     "ListEarthObservationJobOutputTypeDef",
     "ListVectorEnrichmentJobOutputTypeDef",
     "OutputResolutionResamplingInputTypeDef",
     "OutputResolutionStackInputTypeDef",
     "PropertyTypeDef",
     "VectorEnrichmentJobConfigTypeDef",
     "AreaOfInterestTypeDef",
@@ -226,45 +225,14 @@
     "EoCloudCoverInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
 
-_RequiredS3DataInputTypeDef = TypedDict(
-    "_RequiredS3DataInputTypeDef",
-    {
-        "MetadataProvider": Literal["PLANET_ORDER"],
-        "S3Uri": str,
-    },
-)
-_OptionalS3DataInputTypeDef = TypedDict(
-    "_OptionalS3DataInputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class S3DataInputTypeDef(_RequiredS3DataInputTypeDef, _OptionalS3DataInputTypeDef):
-    pass
-
-
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
 ExportErrorDetailsOutputTypeDef = TypedDict(
     "ExportErrorDetailsOutputTypeDef",
     {
         "Message": str,
         "Type": ExportErrorTypeType,
     },
     total=False,
@@ -382,14 +350,15 @@
         "y": int,
         "z": int,
     },
 )
 _OptionalGetTileInputRequestTypeDef = TypedDict(
     "_OptionalGetTileInputRequestTypeDef",
     {
+        "ExecutionRoleArn": str,
         "ImageMask": bool,
         "OutputDataType": OutputTypeType,
         "OutputFormat": str,
         "PropertyFilters": str,
         "TimeRangeFilter": str,
     },
     total=False,
@@ -398,14 +367,22 @@
 
 class GetTileInputRequestTypeDef(
     _RequiredGetTileInputRequestTypeDef, _OptionalGetTileInputRequestTypeDef
 ):
     pass
 
 
+GetTileOutputTypeDef = TypedDict(
+    "GetTileOutputTypeDef",
+    {
+        "BinaryFile": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "GetVectorEnrichmentJobInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -469,14 +446,15 @@
         "ZoneS3Path": str,
     },
 )
 _OptionalZonalStatisticsConfigInputTypeDef = TypedDict(
     "_OptionalZonalStatisticsConfigInputTypeDef",
     {
         "TargetBands": List[str],
+        "ZoneS3PathKmsKeyId": str,
     },
     total=False,
 )
 
 
 class ZonalStatisticsConfigInputTypeDef(
     _RequiredZonalStatisticsConfigInputTypeDef, _OptionalZonalStatisticsConfigInputTypeDef
@@ -488,20 +466,21 @@
     "LandsatCloudCoverLandInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef = TypedDict(
+    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "StatusEquals": EarthObservationJobStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListEarthObservationJobInputRequestTypeDef = TypedDict(
     "ListEarthObservationJobInputRequestTypeDef",
     {
@@ -537,14 +516,22 @@
 class ListEarthObservationJobOutputConfigTypeDef(
     _RequiredListEarthObservationJobOutputConfigTypeDef,
     _OptionalListEarthObservationJobOutputConfigTypeDef,
 ):
     pass
 
 
+ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef = TypedDict(
+    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRasterDataCollectionsInputRequestTypeDef = TypedDict(
     "ListRasterDataCollectionsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -553,14 +540,33 @@
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
+ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef = TypedDict(
+    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
+    {
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "StatusEquals": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "ListVectorEnrichmentJobInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "SortBy": str,
         "SortOrder": SortOrderType,
@@ -610,14 +616,24 @@
     "UserDefinedTypeDef",
     {
         "Unit": Literal["METERS"],
         "Value": float,
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
 _RequiredPlatformInputTypeDef = TypedDict(
     "_RequiredPlatformInputTypeDef",
     {
         "Value": str,
     },
 )
 _OptionalPlatformInputTypeDef = TypedDict(
@@ -656,19 +672,38 @@
         "UpperBound": float,
     },
 )
 
 TimeRangeFilterInputTypeDef = TypedDict(
     "TimeRangeFilterInputTypeDef",
     {
+        "EndTime": Union[datetime, str],
+        "StartTime": Union[datetime, str],
+    },
+)
+
+TimeRangeFilterOutputTypeDef = TypedDict(
+    "TimeRangeFilterOutputTypeDef",
+    {
         "EndTime": datetime,
         "StartTime": datetime,
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
 ReverseGeocodingConfigTypeDef = TypedDict(
     "ReverseGeocodingConfigTypeDef",
     {
         "XAttributeName": str,
         "YAttributeName": str,
     },
 )
@@ -716,38 +751,14 @@
     "CustomIndicesInputTypeDef",
     {
         "Operations": List[OperationTypeDef],
     },
     total=False,
 )
 
-EojDataSourceConfigInputTypeDef = TypedDict(
-    "EojDataSourceConfigInputTypeDef",
-    {
-        "S3Data": S3DataInputTypeDef,
-    },
-    total=False,
-)
-
-GetTileOutputTypeDef = TypedDict(
-    "GetTileOutputTypeDef",
-    {
-        "BinaryFile": StreamingBody,
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
 ExportErrorDetailsTypeDef = TypedDict(
     "ExportErrorDetailsTypeDef",
     {
         "ExportResults": ExportErrorDetailsOutputTypeDef,
         "ExportSourceImages": ExportErrorDetailsOutputTypeDef,
     },
     total=False,
@@ -782,15 +793,15 @@
         "Description": str,
         "DescriptionPageUrl": str,
         "ImageSourceBands": List[str],
         "Name": str,
         "SupportedFilters": List[FilterTypeDef],
         "Tags": Dict[str, str],
         "Type": DataCollectionTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRasterDataCollectionMetadataTypeDef = TypedDict(
     "_RequiredRasterDataCollectionMetadataTypeDef",
     {
         "Arn": str,
@@ -834,59 +845,29 @@
 )
 
 
 class ItemSourceTypeDef(_RequiredItemSourceTypeDef, _OptionalItemSourceTypeDef):
     pass
 
 
-ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef = TypedDict(
-    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
-    {
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "StatusEquals": EarthObservationJobStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef = TypedDict(
-    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef = TypedDict(
-    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
-    {
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "StatusEquals": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListEarthObservationJobOutputTypeDef = TypedDict(
     "ListEarthObservationJobOutputTypeDef",
     {
         "EarthObservationJobSummaries": List[ListEarthObservationJobOutputConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVectorEnrichmentJobOutputTypeDef = TypedDict(
     "ListVectorEnrichmentJobOutputTypeDef",
     {
         "NextToken": str,
         "VectorEnrichmentJobSummaries": List[ListVectorEnrichmentJobOutputConfigTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OutputResolutionResamplingInputTypeDef = TypedDict(
     "OutputResolutionResamplingInputTypeDef",
     {
         "UserDefined": UserDefinedTypeDef,
@@ -948,14 +929,15 @@
         "ExecutionRoleArn": str,
         "OutputConfig": OutputConfigInputTypeDef,
     },
 )
 _OptionalExportEarthObservationJobInputRequestTypeDef = TypedDict(
     "_OptionalExportEarthObservationJobInputRequestTypeDef",
     {
+        "ClientToken": str,
         "ExportSourceImages": bool,
     },
     total=False,
 )
 
 
 class ExportEarthObservationJobInputRequestTypeDef(
@@ -970,36 +952,51 @@
     {
         "Arn": str,
         "CreationTime": datetime,
         "ExecutionRoleArn": str,
         "ExportSourceImages": bool,
         "ExportStatus": EarthObservationJobExportStatusType,
         "OutputConfig": OutputConfigInputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ExportVectorEnrichmentJobInputRequestTypeDef = TypedDict(
-    "ExportVectorEnrichmentJobInputRequestTypeDef",
+_RequiredExportVectorEnrichmentJobInputRequestTypeDef = TypedDict(
+    "_RequiredExportVectorEnrichmentJobInputRequestTypeDef",
     {
         "Arn": str,
         "ExecutionRoleArn": str,
         "OutputConfig": ExportVectorEnrichmentJobOutputConfigTypeDef,
     },
 )
+_OptionalExportVectorEnrichmentJobInputRequestTypeDef = TypedDict(
+    "_OptionalExportVectorEnrichmentJobInputRequestTypeDef",
+    {
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class ExportVectorEnrichmentJobInputRequestTypeDef(
+    _RequiredExportVectorEnrichmentJobInputRequestTypeDef,
+    _OptionalExportVectorEnrichmentJobInputRequestTypeDef,
+):
+    pass
+
 
 ExportVectorEnrichmentJobOutputTypeDef = TypedDict(
     "ExportVectorEnrichmentJobOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "ExecutionRoleArn": str,
         "ExportStatus": VectorEnrichmentJobExportStatusType,
         "OutputConfig": ExportVectorEnrichmentJobOutputConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VectorEnrichmentJobInputConfigTypeDef = TypedDict(
     "VectorEnrichmentJobInputConfigTypeDef",
     {
         "DataSourceConfig": VectorEnrichmentJobDataSourceConfigInputTypeDef,
@@ -1008,25 +1005,25 @@
 )
 
 ListRasterDataCollectionsOutputTypeDef = TypedDict(
     "ListRasterDataCollectionsOutputTypeDef",
     {
         "NextToken": str,
         "RasterDataCollectionSummaries": List[RasterDataCollectionMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchRasterDataCollectionOutputTypeDef = TypedDict(
     "SearchRasterDataCollectionOutputTypeDef",
     {
         "ApproximateResultCount": int,
         "Items": List[ItemSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredResamplingConfigInputTypeDef = TypedDict(
     "_RequiredResamplingConfigInputTypeDef",
     {
         "OutputResolution": OutputResolutionResamplingInputTypeDef,
@@ -1077,15 +1074,15 @@
         "InputConfig": VectorEnrichmentJobInputConfigTypeDef,
         "JobConfig": VectorEnrichmentJobConfigTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "Status": VectorEnrichmentJobStatusType,
         "Tags": Dict[str, str],
         "Type": VectorEnrichmentJobTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "_RequiredStartVectorEnrichmentJobInputRequestTypeDef",
     {
         "ExecutionRoleArn": str,
@@ -1122,15 +1119,15 @@
         "InputConfig": VectorEnrichmentJobInputConfigTypeDef,
         "JobConfig": VectorEnrichmentJobConfigTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "Status": VectorEnrichmentJobStatusType,
         "Tags": Dict[str, str],
         "Type": VectorEnrichmentJobTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JobConfigInputTypeDef = TypedDict(
     "JobConfigInputTypeDef",
     {
         "BandMathConfig": BandMathConfigInputTypeDef,
@@ -1179,15 +1176,15 @@
 
 
 _RequiredRasterDataCollectionQueryOutputTypeDef = TypedDict(
     "_RequiredRasterDataCollectionQueryOutputTypeDef",
     {
         "RasterDataCollectionArn": str,
         "RasterDataCollectionName": str,
-        "TimeRangeFilter": TimeRangeFilterInputTypeDef,
+        "TimeRangeFilter": TimeRangeFilterOutputTypeDef,
     },
 )
 _OptionalRasterDataCollectionQueryOutputTypeDef = TypedDict(
     "_OptionalRasterDataCollectionQueryOutputTypeDef",
     {
         "AreaOfInterest": AreaOfInterestTypeDef,
         "PropertyFilters": PropertyFiltersTypeDef,
@@ -1225,25 +1222,23 @@
 ):
     pass
 
 
 InputConfigInputTypeDef = TypedDict(
     "InputConfigInputTypeDef",
     {
-        "DataSourceConfig": EojDataSourceConfigInputTypeDef,
         "PreviousEarthObservationJobArn": str,
         "RasterDataCollectionQuery": RasterDataCollectionQueryInputTypeDef,
     },
     total=False,
 )
 
 InputConfigOutputTypeDef = TypedDict(
     "InputConfigOutputTypeDef",
     {
-        "DataSourceConfig": EojDataSourceConfigInputTypeDef,
         "PreviousEarthObservationJobArn": str,
         "RasterDataCollectionQuery": RasterDataCollectionQueryOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredSearchRasterDataCollectionInputRequestTypeDef = TypedDict(
@@ -1268,24 +1263,24 @@
 ):
     pass
 
 
 _RequiredStartEarthObservationJobInputRequestTypeDef = TypedDict(
     "_RequiredStartEarthObservationJobInputRequestTypeDef",
     {
+        "ExecutionRoleArn": str,
         "InputConfig": InputConfigInputTypeDef,
         "JobConfig": JobConfigInputTypeDef,
         "Name": str,
     },
 )
 _OptionalStartEarthObservationJobInputRequestTypeDef = TypedDict(
     "_OptionalStartEarthObservationJobInputRequestTypeDef",
     {
         "ClientToken": str,
-        "ExecutionRoleArn": str,
         "KmsKeyId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
@@ -1309,15 +1304,15 @@
         "InputConfig": InputConfigOutputTypeDef,
         "JobConfig": JobConfigInputTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "OutputBands": List[OutputBandTypeDef],
         "Status": EarthObservationJobStatusType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartEarthObservationJobOutputTypeDef = TypedDict(
     "StartEarthObservationJobOutputTypeDef",
     {
         "Arn": str,
@@ -1326,10 +1321,10 @@
         "ExecutionRoleArn": str,
         "InputConfig": InputConfigOutputTypeDef,
         "JobConfig": JobConfigInputTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "Status": EarthObservationJobStatusType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial/type_defs.pyi` & `mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_sagemaker_geospatial.type_defs import MultiPolygonGeometryInputTypeDef
 
     data: MultiPolygonGeometryInputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AlgorithmNameGeoMosaicType,
     AlgorithmNameResamplingType,
     ComparisonOperatorType,
@@ -55,67 +55,66 @@
     "AssetValueTypeDef",
     "CloudRemovalConfigInputTypeDef",
     "OperationTypeDef",
     "DeleteEarthObservationJobInputRequestTypeDef",
     "DeleteVectorEnrichmentJobInputRequestTypeDef",
     "EarthObservationJobErrorDetailsTypeDef",
     "EoCloudCoverInputTypeDef",
-    "S3DataInputTypeDef",
-    "ResponseMetadataTypeDef",
     "ExportErrorDetailsOutputTypeDef",
     "ExportS3DataInputTypeDef",
     "VectorEnrichmentJobS3DataTypeDef",
     "FilterTypeDef",
     "GeoMosaicConfigInputTypeDef",
     "GeometryTypeDef",
     "GetEarthObservationJobInputRequestTypeDef",
     "OutputBandTypeDef",
     "GetRasterDataCollectionInputRequestTypeDef",
     "GetTileInputRequestTypeDef",
+    "GetTileOutputTypeDef",
     "GetVectorEnrichmentJobInputRequestTypeDef",
     "VectorEnrichmentJobErrorDetailsTypeDef",
     "VectorEnrichmentJobExportErrorDetailsTypeDef",
     "PropertiesTypeDef",
     "TemporalStatisticsConfigInputTypeDef",
     "ZonalStatisticsConfigInputTypeDef",
     "LandsatCloudCoverLandInputTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
     "ListEarthObservationJobInputRequestTypeDef",
     "ListEarthObservationJobOutputConfigTypeDef",
+    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
     "ListRasterDataCollectionsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
     "ListVectorEnrichmentJobInputRequestTypeDef",
     "ListVectorEnrichmentJobOutputConfigTypeDef",
     "MapMatchingConfigTypeDef",
     "UserDefinedTypeDef",
+    "PaginatorConfigTypeDef",
     "PlatformInputTypeDef",
     "ViewOffNadirInputTypeDef",
     "ViewSunAzimuthInputTypeDef",
     "ViewSunElevationInputTypeDef",
     "TimeRangeFilterInputTypeDef",
+    "TimeRangeFilterOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "ReverseGeocodingConfigTypeDef",
     "StopEarthObservationJobInputRequestTypeDef",
     "StopVectorEnrichmentJobInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AreaOfInterestGeometryTypeDef",
     "CustomIndicesInputTypeDef",
-    "EojDataSourceConfigInputTypeDef",
-    "GetTileOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ExportErrorDetailsTypeDef",
     "OutputConfigInputTypeDef",
     "ExportVectorEnrichmentJobOutputConfigTypeDef",
     "VectorEnrichmentJobDataSourceConfigInputTypeDef",
     "GetRasterDataCollectionOutputTypeDef",
     "RasterDataCollectionMetadataTypeDef",
     "ItemSourceTypeDef",
-    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
-    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
-    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
     "ListEarthObservationJobOutputTypeDef",
     "ListVectorEnrichmentJobOutputTypeDef",
     "OutputResolutionResamplingInputTypeDef",
     "OutputResolutionStackInputTypeDef",
     "PropertyTypeDef",
     "VectorEnrichmentJobConfigTypeDef",
     "AreaOfInterestTypeDef",
@@ -223,43 +222,14 @@
     "EoCloudCoverInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
 
-_RequiredS3DataInputTypeDef = TypedDict(
-    "_RequiredS3DataInputTypeDef",
-    {
-        "MetadataProvider": Literal["PLANET_ORDER"],
-        "S3Uri": str,
-    },
-)
-_OptionalS3DataInputTypeDef = TypedDict(
-    "_OptionalS3DataInputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class S3DataInputTypeDef(_RequiredS3DataInputTypeDef, _OptionalS3DataInputTypeDef):
-    pass
-
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
 ExportErrorDetailsOutputTypeDef = TypedDict(
     "ExportErrorDetailsOutputTypeDef",
     {
         "Message": str,
         "Type": ExportErrorTypeType,
     },
     total=False,
@@ -371,28 +341,37 @@
         "y": int,
         "z": int,
     },
 )
 _OptionalGetTileInputRequestTypeDef = TypedDict(
     "_OptionalGetTileInputRequestTypeDef",
     {
+        "ExecutionRoleArn": str,
         "ImageMask": bool,
         "OutputDataType": OutputTypeType,
         "OutputFormat": str,
         "PropertyFilters": str,
         "TimeRangeFilter": str,
     },
     total=False,
 )
 
 class GetTileInputRequestTypeDef(
     _RequiredGetTileInputRequestTypeDef, _OptionalGetTileInputRequestTypeDef
 ):
     pass
 
+GetTileOutputTypeDef = TypedDict(
+    "GetTileOutputTypeDef",
+    {
+        "BinaryFile": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "GetVectorEnrichmentJobInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -454,14 +433,15 @@
         "ZoneS3Path": str,
     },
 )
 _OptionalZonalStatisticsConfigInputTypeDef = TypedDict(
     "_OptionalZonalStatisticsConfigInputTypeDef",
     {
         "TargetBands": List[str],
+        "ZoneS3PathKmsKeyId": str,
     },
     total=False,
 )
 
 class ZonalStatisticsConfigInputTypeDef(
     _RequiredZonalStatisticsConfigInputTypeDef, _OptionalZonalStatisticsConfigInputTypeDef
 ):
@@ -471,20 +451,21 @@
     "LandsatCloudCoverLandInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef = TypedDict(
+    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "StatusEquals": EarthObservationJobStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListEarthObservationJobInputRequestTypeDef = TypedDict(
     "ListEarthObservationJobInputRequestTypeDef",
     {
@@ -518,14 +499,22 @@
 
 class ListEarthObservationJobOutputConfigTypeDef(
     _RequiredListEarthObservationJobOutputConfigTypeDef,
     _OptionalListEarthObservationJobOutputConfigTypeDef,
 ):
     pass
 
+ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef = TypedDict(
+    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRasterDataCollectionsInputRequestTypeDef = TypedDict(
     "ListRasterDataCollectionsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -534,14 +523,33 @@
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
+ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef = TypedDict(
+    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
+    {
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "StatusEquals": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "ListVectorEnrichmentJobInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "SortBy": str,
         "SortOrder": SortOrderType,
@@ -589,14 +597,24 @@
     "UserDefinedTypeDef",
     {
         "Unit": Literal["METERS"],
         "Value": float,
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
 _RequiredPlatformInputTypeDef = TypedDict(
     "_RequiredPlatformInputTypeDef",
     {
         "Value": str,
     },
 )
 _OptionalPlatformInputTypeDef = TypedDict(
@@ -633,19 +651,38 @@
         "UpperBound": float,
     },
 )
 
 TimeRangeFilterInputTypeDef = TypedDict(
     "TimeRangeFilterInputTypeDef",
     {
+        "EndTime": Union[datetime, str],
+        "StartTime": Union[datetime, str],
+    },
+)
+
+TimeRangeFilterOutputTypeDef = TypedDict(
+    "TimeRangeFilterOutputTypeDef",
+    {
         "EndTime": datetime,
         "StartTime": datetime,
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
 ReverseGeocodingConfigTypeDef = TypedDict(
     "ReverseGeocodingConfigTypeDef",
     {
         "XAttributeName": str,
         "YAttributeName": str,
     },
 )
@@ -693,38 +730,14 @@
     "CustomIndicesInputTypeDef",
     {
         "Operations": List[OperationTypeDef],
     },
     total=False,
 )
 
-EojDataSourceConfigInputTypeDef = TypedDict(
-    "EojDataSourceConfigInputTypeDef",
-    {
-        "S3Data": S3DataInputTypeDef,
-    },
-    total=False,
-)
-
-GetTileOutputTypeDef = TypedDict(
-    "GetTileOutputTypeDef",
-    {
-        "BinaryFile": StreamingBody,
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
 ExportErrorDetailsTypeDef = TypedDict(
     "ExportErrorDetailsTypeDef",
     {
         "ExportResults": ExportErrorDetailsOutputTypeDef,
         "ExportSourceImages": ExportErrorDetailsOutputTypeDef,
     },
     total=False,
@@ -759,15 +772,15 @@
         "Description": str,
         "DescriptionPageUrl": str,
         "ImageSourceBands": List[str],
         "Name": str,
         "SupportedFilters": List[FilterTypeDef],
         "Tags": Dict[str, str],
         "Type": DataCollectionTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRasterDataCollectionMetadataTypeDef = TypedDict(
     "_RequiredRasterDataCollectionMetadataTypeDef",
     {
         "Arn": str,
@@ -807,59 +820,29 @@
     },
     total=False,
 )
 
 class ItemSourceTypeDef(_RequiredItemSourceTypeDef, _OptionalItemSourceTypeDef):
     pass
 
-ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef = TypedDict(
-    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
-    {
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "StatusEquals": EarthObservationJobStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef = TypedDict(
-    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef = TypedDict(
-    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
-    {
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "StatusEquals": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListEarthObservationJobOutputTypeDef = TypedDict(
     "ListEarthObservationJobOutputTypeDef",
     {
         "EarthObservationJobSummaries": List[ListEarthObservationJobOutputConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVectorEnrichmentJobOutputTypeDef = TypedDict(
     "ListVectorEnrichmentJobOutputTypeDef",
     {
         "NextToken": str,
         "VectorEnrichmentJobSummaries": List[ListVectorEnrichmentJobOutputConfigTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OutputResolutionResamplingInputTypeDef = TypedDict(
     "OutputResolutionResamplingInputTypeDef",
     {
         "UserDefined": UserDefinedTypeDef,
@@ -921,14 +904,15 @@
         "ExecutionRoleArn": str,
         "OutputConfig": OutputConfigInputTypeDef,
     },
 )
 _OptionalExportEarthObservationJobInputRequestTypeDef = TypedDict(
     "_OptionalExportEarthObservationJobInputRequestTypeDef",
     {
+        "ClientToken": str,
         "ExportSourceImages": bool,
     },
     total=False,
 )
 
 class ExportEarthObservationJobInputRequestTypeDef(
     _RequiredExportEarthObservationJobInputRequestTypeDef,
@@ -941,36 +925,49 @@
     {
         "Arn": str,
         "CreationTime": datetime,
         "ExecutionRoleArn": str,
         "ExportSourceImages": bool,
         "ExportStatus": EarthObservationJobExportStatusType,
         "OutputConfig": OutputConfigInputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ExportVectorEnrichmentJobInputRequestTypeDef = TypedDict(
-    "ExportVectorEnrichmentJobInputRequestTypeDef",
+_RequiredExportVectorEnrichmentJobInputRequestTypeDef = TypedDict(
+    "_RequiredExportVectorEnrichmentJobInputRequestTypeDef",
     {
         "Arn": str,
         "ExecutionRoleArn": str,
         "OutputConfig": ExportVectorEnrichmentJobOutputConfigTypeDef,
     },
 )
+_OptionalExportVectorEnrichmentJobInputRequestTypeDef = TypedDict(
+    "_OptionalExportVectorEnrichmentJobInputRequestTypeDef",
+    {
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class ExportVectorEnrichmentJobInputRequestTypeDef(
+    _RequiredExportVectorEnrichmentJobInputRequestTypeDef,
+    _OptionalExportVectorEnrichmentJobInputRequestTypeDef,
+):
+    pass
 
 ExportVectorEnrichmentJobOutputTypeDef = TypedDict(
     "ExportVectorEnrichmentJobOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "ExecutionRoleArn": str,
         "ExportStatus": VectorEnrichmentJobExportStatusType,
         "OutputConfig": ExportVectorEnrichmentJobOutputConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VectorEnrichmentJobInputConfigTypeDef = TypedDict(
     "VectorEnrichmentJobInputConfigTypeDef",
     {
         "DataSourceConfig": VectorEnrichmentJobDataSourceConfigInputTypeDef,
@@ -979,25 +976,25 @@
 )
 
 ListRasterDataCollectionsOutputTypeDef = TypedDict(
     "ListRasterDataCollectionsOutputTypeDef",
     {
         "NextToken": str,
         "RasterDataCollectionSummaries": List[RasterDataCollectionMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchRasterDataCollectionOutputTypeDef = TypedDict(
     "SearchRasterDataCollectionOutputTypeDef",
     {
         "ApproximateResultCount": int,
         "Items": List[ItemSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredResamplingConfigInputTypeDef = TypedDict(
     "_RequiredResamplingConfigInputTypeDef",
     {
         "OutputResolution": OutputResolutionResamplingInputTypeDef,
@@ -1046,15 +1043,15 @@
         "InputConfig": VectorEnrichmentJobInputConfigTypeDef,
         "JobConfig": VectorEnrichmentJobConfigTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "Status": VectorEnrichmentJobStatusType,
         "Tags": Dict[str, str],
         "Type": VectorEnrichmentJobTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "_RequiredStartVectorEnrichmentJobInputRequestTypeDef",
     {
         "ExecutionRoleArn": str,
@@ -1089,15 +1086,15 @@
         "InputConfig": VectorEnrichmentJobInputConfigTypeDef,
         "JobConfig": VectorEnrichmentJobConfigTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "Status": VectorEnrichmentJobStatusType,
         "Tags": Dict[str, str],
         "Type": VectorEnrichmentJobTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JobConfigInputTypeDef = TypedDict(
     "JobConfigInputTypeDef",
     {
         "BandMathConfig": BandMathConfigInputTypeDef,
@@ -1144,15 +1141,15 @@
     pass
 
 _RequiredRasterDataCollectionQueryOutputTypeDef = TypedDict(
     "_RequiredRasterDataCollectionQueryOutputTypeDef",
     {
         "RasterDataCollectionArn": str,
         "RasterDataCollectionName": str,
-        "TimeRangeFilter": TimeRangeFilterInputTypeDef,
+        "TimeRangeFilter": TimeRangeFilterOutputTypeDef,
     },
 )
 _OptionalRasterDataCollectionQueryOutputTypeDef = TypedDict(
     "_OptionalRasterDataCollectionQueryOutputTypeDef",
     {
         "AreaOfInterest": AreaOfInterestTypeDef,
         "PropertyFilters": PropertyFiltersTypeDef,
@@ -1186,25 +1183,23 @@
     _OptionalRasterDataCollectionQueryWithBandFilterInputTypeDef,
 ):
     pass
 
 InputConfigInputTypeDef = TypedDict(
     "InputConfigInputTypeDef",
     {
-        "DataSourceConfig": EojDataSourceConfigInputTypeDef,
         "PreviousEarthObservationJobArn": str,
         "RasterDataCollectionQuery": RasterDataCollectionQueryInputTypeDef,
     },
     total=False,
 )
 
 InputConfigOutputTypeDef = TypedDict(
     "InputConfigOutputTypeDef",
     {
-        "DataSourceConfig": EojDataSourceConfigInputTypeDef,
         "PreviousEarthObservationJobArn": str,
         "RasterDataCollectionQuery": RasterDataCollectionQueryOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredSearchRasterDataCollectionInputRequestTypeDef = TypedDict(
@@ -1227,24 +1222,24 @@
     _OptionalSearchRasterDataCollectionInputRequestTypeDef,
 ):
     pass
 
 _RequiredStartEarthObservationJobInputRequestTypeDef = TypedDict(
     "_RequiredStartEarthObservationJobInputRequestTypeDef",
     {
+        "ExecutionRoleArn": str,
         "InputConfig": InputConfigInputTypeDef,
         "JobConfig": JobConfigInputTypeDef,
         "Name": str,
     },
 )
 _OptionalStartEarthObservationJobInputRequestTypeDef = TypedDict(
     "_OptionalStartEarthObservationJobInputRequestTypeDef",
     {
         "ClientToken": str,
-        "ExecutionRoleArn": str,
         "KmsKeyId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 class StartEarthObservationJobInputRequestTypeDef(
@@ -1266,15 +1261,15 @@
         "InputConfig": InputConfigOutputTypeDef,
         "JobConfig": JobConfigInputTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "OutputBands": List[OutputBandTypeDef],
         "Status": EarthObservationJobStatusType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartEarthObservationJobOutputTypeDef = TypedDict(
     "StartEarthObservationJobOutputTypeDef",
     {
         "Arn": str,
@@ -1283,10 +1278,10 @@
         "ExecutionRoleArn": str,
         "InputConfig": InputConfigOutputTypeDef,
         "JobConfig": JobConfigInputTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "Status": EarthObservationJobStatusType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-geospatial
-Version: 1.26.20
-Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.26.20 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/
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
 
 <a id="mypy-boto3-sagemaker-geospatial"></a>
 
 # mypy-boto3-sagemaker-geospatial
 
 [![PyPI - mypy-boto3-sagemaker-geospatial](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-geospatial?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakergeospatialcapabilities 1.26.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[boto3.SageMakergeospatialcapabilities 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sagemaker-geospatial docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,15 +324,14 @@
     EarthObservationJobStatusType,
     ExportErrorTypeType,
     GroupByType,
     ListEarthObservationJobsPaginatorName,
     ListRasterDataCollectionsPaginatorName,
     ListVectorEnrichmentJobsPaginatorName,
     LogicalOperatorType,
-    MetadataProviderType,
     OutputTypeType,
     PredefinedResolutionType,
     SortOrderType,
     TargetOptionsType,
     TemporalStatisticsType,
     UnitType,
     VectorEnrichmentJobDocumentTypeType,
@@ -367,67 +367,66 @@
     AssetValueTypeDef,
     CloudRemovalConfigInputTypeDef,
     OperationTypeDef,
     DeleteEarthObservationJobInputRequestTypeDef,
     DeleteVectorEnrichmentJobInputRequestTypeDef,
     EarthObservationJobErrorDetailsTypeDef,
     EoCloudCoverInputTypeDef,
-    S3DataInputTypeDef,
-    ResponseMetadataTypeDef,
     ExportErrorDetailsOutputTypeDef,
     ExportS3DataInputTypeDef,
     VectorEnrichmentJobS3DataTypeDef,
     FilterTypeDef,
     GeoMosaicConfigInputTypeDef,
     GeometryTypeDef,
     GetEarthObservationJobInputRequestTypeDef,
     OutputBandTypeDef,
     GetRasterDataCollectionInputRequestTypeDef,
     GetTileInputRequestTypeDef,
+    GetTileOutputTypeDef,
     GetVectorEnrichmentJobInputRequestTypeDef,
     VectorEnrichmentJobErrorDetailsTypeDef,
     VectorEnrichmentJobExportErrorDetailsTypeDef,
     PropertiesTypeDef,
     TemporalStatisticsConfigInputTypeDef,
     ZonalStatisticsConfigInputTypeDef,
     LandsatCloudCoverLandInputTypeDef,
-    PaginatorConfigTypeDef,
+    ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef,
     ListEarthObservationJobInputRequestTypeDef,
     ListEarthObservationJobOutputConfigTypeDef,
+    ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef,
     ListRasterDataCollectionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListVectorEnrichmentJobInputRequestTypeDef,
     ListVectorEnrichmentJobOutputConfigTypeDef,
     MapMatchingConfigTypeDef,
     UserDefinedTypeDef,
+    PaginatorConfigTypeDef,
     PlatformInputTypeDef,
     ViewOffNadirInputTypeDef,
     ViewSunAzimuthInputTypeDef,
     ViewSunElevationInputTypeDef,
     TimeRangeFilterInputTypeDef,
+    TimeRangeFilterOutputTypeDef,
+    ResponseMetadataTypeDef,
     ReverseGeocodingConfigTypeDef,
     StopEarthObservationJobInputRequestTypeDef,
     StopVectorEnrichmentJobInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AreaOfInterestGeometryTypeDef,
     CustomIndicesInputTypeDef,
-    EojDataSourceConfigInputTypeDef,
-    GetTileOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ExportErrorDetailsTypeDef,
     OutputConfigInputTypeDef,
     ExportVectorEnrichmentJobOutputConfigTypeDef,
     VectorEnrichmentJobDataSourceConfigInputTypeDef,
     GetRasterDataCollectionOutputTypeDef,
     RasterDataCollectionMetadataTypeDef,
     ItemSourceTypeDef,
-    ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef,
-    ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef,
-    ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
     OutputResolutionResamplingInputTypeDef,
     OutputResolutionStackInputTypeDef,
     PropertyTypeDef,
     VectorEnrichmentJobConfigTypeDef,
     AreaOfInterestTypeDef,
@@ -466,42 +465,42 @@
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

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-geospatial-1.27.0/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.26.20/setup.py` & `mypy-boto3-sagemaker-geospatial-1.27.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 """
 Setup script for mypy-boto3-sagemaker-geospatial.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-geospatial",
-    version="1.26.20",
+    version="1.27.0",
     packages=["mypy_boto3_sagemaker_geospatial"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMakergeospatialcapabilities 1.26.20 service generated with"
-        " mypy-boto3-builder 7.11.11"
+        "Type annotations for boto3.SageMakergeospatialcapabilities 1.27.0 service generated with"
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
     keywords="boto3 sagemaker-geospatial type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_sagemaker_geospatial": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_sagemaker_geospatial": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/"
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


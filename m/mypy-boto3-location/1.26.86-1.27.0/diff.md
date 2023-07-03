# Comparing `tmp/mypy-boto3-location-1.26.86.tar.gz` & `tmp/mypy-boto3-location-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-location-1.26.86.tar", last modified: Tue Mar  7 20:27:21 2023, max compression
+gzip compressed data, was "mypy-boto3-location-1.27.0.tar", last modified: Mon Jul  3 19:51:03 2023, max compression
```

## Comparing `mypy-boto3-location-1.26.86.tar` & `mypy-boto3-location-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:27:21.143664 mypy-boto3-location-1.26.86/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-03-07 20:27:21.143664 mypy-boto3-location-1.26.86/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19543 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:27:21.135664 mypy-boto3-location-1.26.86/mypy_boto3_location/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45004 2023-03-07 20:27:09.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    44929 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-03-07 20:27:09.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-03-07 20:27:09.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-03-07 20:27:09.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-03-07 20:27:09.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62800 2023-03-07 20:27:11.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62697 2023-03-07 20:27:10.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/mypy_boto3_location/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 20:27:21.143664 mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-03-07 20:27:21.000000 mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-07 20:27:21.000000 mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 20:27:21.000000 mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 20:27:21.000000 mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-07 20:27:21.000000 mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-07 20:27:21.000000 mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 20:27:21.143664 mypy-boto3-location-1.26.86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-07 20:27:08.000000 mypy-boto3-location-1.26.86/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.267589 mypy-boto3-location-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21053 2023-07-03 19:51:03.267589 mypy-boto3-location-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.267589 mypy-boto3-location-1.27.0/mypy_boto3_location/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45353 2023-07-03 19:41:13.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45278 2023-07-03 19:41:13.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-07-03 19:41:13.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-07-03 19:41:13.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-07-03 19:41:13.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-07-03 19:41:13.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64854 2023-07-03 19:41:16.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64743 2023-07-03 19:41:14.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/mypy_boto3_location/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.267589 mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21053 2023-07-03 19:51:03.000000 mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 19:51:03.000000 mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:03.000000 mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:03.000000 mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:03.267589 mypy-boto3-location-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:41:12.000000 mypy-boto3-location-1.27.0/setup.py
```

### Comparing `mypy-boto3-location-1.26.86/LICENSE` & `mypy-boto3-location-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-location-1.26.86/PKG-INFO` & `mypy-boto3-location-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-location
-Version: 1.26.86
-Summary: Type annotations for boto3.LocationService 1.26.86 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.LocationService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-location"></a>
 
 # mypy-boto3-location
 
 [![PyPI - mypy-boto3-location](https://img.shields.io/pypi/v/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-location?color=blue)](https://pypistats.org/packages/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.26.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
 See how it helps to find and fix potential bugs:
 
@@ -372,144 +372,145 @@
 ```python
 from mypy_boto3_location.type_defs import (
     ApiKeyFilterTypeDef,
     ApiKeyRestrictionsTypeDef,
     AssociateTrackerConsumerRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDeleteDevicePositionHistoryRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     BatchDeleteGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionRequestRequestTypeDef,
     BatchPutGeofenceSuccessTypeDef,
     CalculateRouteCarModeOptionsTypeDef,
     CalculateRouteMatrixSummaryTypeDef,
     CalculateRouteSummaryTypeDef,
     TruckDimensionsTypeDef,
     TruckWeightTypeDef,
     CircleTypeDef,
     CreateGeofenceCollectionRequestRequestTypeDef,
+    CreateGeofenceCollectionResponseTypeDef,
+    CreateKeyResponseTypeDef,
     MapConfigurationTypeDef,
+    CreateMapResponseTypeDef,
     DataSourceConfigurationTypeDef,
+    CreatePlaceIndexResponseTypeDef,
     CreateRouteCalculatorRequestRequestTypeDef,
+    CreateRouteCalculatorResponseTypeDef,
     CreateTrackerRequestRequestTypeDef,
+    CreateTrackerResponseTypeDef,
     DeleteGeofenceCollectionRequestRequestTypeDef,
     DeleteKeyRequestRequestTypeDef,
     DeleteMapRequestRequestTypeDef,
     DeletePlaceIndexRequestRequestTypeDef,
     DeleteRouteCalculatorRequestRequestTypeDef,
     DeleteTrackerRequestRequestTypeDef,
     DescribeGeofenceCollectionRequestRequestTypeDef,
+    DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DescribeMapRequestRequestTypeDef,
     DescribePlaceIndexRequestRequestTypeDef,
     DescribeRouteCalculatorRequestRequestTypeDef,
+    DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerRequestRequestTypeDef,
+    DescribeTrackerResponseTypeDef,
     PositionalAccuracyTypeDef,
     DisassociateTrackerConsumerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
     GetDevicePositionHistoryRequestRequestTypeDef,
     GetDevicePositionRequestRequestTypeDef,
     GetGeofenceRequestRequestTypeDef,
     GetMapGlyphsRequestRequestTypeDef,
+    GetMapGlyphsResponseTypeDef,
     GetMapSpritesRequestRequestTypeDef,
+    GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorRequestRequestTypeDef,
+    GetMapStyleDescriptorResponseTypeDef,
     GetMapTileRequestRequestTypeDef,
+    GetMapTileResponseTypeDef,
     GetPlaceRequestRequestTypeDef,
     LegGeometryTypeDef,
     StepTypeDef,
+    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
     ListDevicePositionsRequestRequestTypeDef,
+    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
     ListGeofenceCollectionsRequestRequestTypeDef,
     ListGeofenceCollectionsResponseEntryTypeDef,
+    ListGeofencesRequestListGeofencesPaginateTypeDef,
     ListGeofencesRequestRequestTypeDef,
+    ListMapsRequestListMapsPaginateTypeDef,
     ListMapsRequestRequestTypeDef,
     ListMapsResponseEntryTypeDef,
+    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
     ListPlaceIndexesRequestRequestTypeDef,
     ListPlaceIndexesResponseEntryTypeDef,
+    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
     ListRouteCalculatorsRequestRequestTypeDef,
     ListRouteCalculatorsResponseEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
     ListTrackerConsumersRequestRequestTypeDef,
+    ListTrackerConsumersResponseTypeDef,
+    ListTrackersRequestListTrackersPaginateTypeDef,
     ListTrackersRequestRequestTypeDef,
     ListTrackersResponseEntryTypeDef,
+    MapConfigurationUpdateTypeDef,
+    PaginatorConfigTypeDef,
     PlaceGeometryTypeDef,
     TimeZoneTypeDef,
+    PutGeofenceResponseTypeDef,
+    ResponseMetadataTypeDef,
     RouteMatrixEntryErrorTypeDef,
     SearchForSuggestionsResultTypeDef,
     SearchPlaceIndexForPositionRequestRequestTypeDef,
     SearchPlaceIndexForPositionSummaryTypeDef,
     SearchPlaceIndexForSuggestionsRequestRequestTypeDef,
     SearchPlaceIndexForSuggestionsSummaryTypeDef,
     SearchPlaceIndexForTextRequestRequestTypeDef,
     SearchPlaceIndexForTextSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGeofenceCollectionRequestRequestTypeDef,
-    UpdateMapRequestRequestTypeDef,
+    UpdateGeofenceCollectionResponseTypeDef,
+    UpdateKeyResponseTypeDef,
+    UpdateMapResponseTypeDef,
+    UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorRequestRequestTypeDef,
+    UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerRequestRequestTypeDef,
+    UpdateTrackerResponseTypeDef,
+    ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
     CreateKeyRequestRequestTypeDef,
+    DescribeKeyResponseTypeDef,
     ListKeysResponseEntryTypeDef,
     UpdateKeyRequestRequestTypeDef,
     BatchDeleteDevicePositionHistoryErrorTypeDef,
     BatchDeleteGeofenceErrorTypeDef,
     BatchEvaluateGeofencesErrorTypeDef,
     BatchGetDevicePositionErrorTypeDef,
     BatchPutGeofenceErrorTypeDef,
     BatchUpdateDevicePositionErrorTypeDef,
-    CreateGeofenceCollectionResponseTypeDef,
-    CreateKeyResponseTypeDef,
-    CreateMapResponseTypeDef,
-    CreatePlaceIndexResponseTypeDef,
-    CreateRouteCalculatorResponseTypeDef,
-    CreateTrackerResponseTypeDef,
-    DescribeGeofenceCollectionResponseTypeDef,
-    DescribeKeyResponseTypeDef,
-    DescribeRouteCalculatorResponseTypeDef,
-    DescribeTrackerResponseTypeDef,
-    GetMapGlyphsResponseTypeDef,
-    GetMapSpritesResponseTypeDef,
-    GetMapStyleDescriptorResponseTypeDef,
-    GetMapTileResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTrackerConsumersResponseTypeDef,
-    PutGeofenceResponseTypeDef,
-    UpdateGeofenceCollectionResponseTypeDef,
-    UpdateKeyResponseTypeDef,
-    UpdateMapResponseTypeDef,
-    UpdatePlaceIndexResponseTypeDef,
-    UpdateRouteCalculatorResponseTypeDef,
-    UpdateTrackerResponseTypeDef,
     CalculateRouteTruckModeOptionsTypeDef,
     GeofenceGeometryTypeDef,
     CreateMapRequestRequestTypeDef,
     DescribeMapResponseTypeDef,
     CreatePlaceIndexRequestRequestTypeDef,
     DescribePlaceIndexResponseTypeDef,
     UpdatePlaceIndexRequestRequestTypeDef,
     DevicePositionTypeDef,
     DevicePositionUpdateTypeDef,
     GetDevicePositionResponseTypeDef,
     ListDevicePositionsResponseEntryTypeDef,
-    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
-    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
-    ListGeofencesRequestListGeofencesPaginateTypeDef,
-    ListKeysRequestListKeysPaginateTypeDef,
-    ListMapsRequestListMapsPaginateTypeDef,
-    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
-    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
-    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
-    ListTrackersRequestListTrackersPaginateTypeDef,
     LegTypeDef,
     ListGeofenceCollectionsResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackersResponseTypeDef,
+    UpdateMapRequestRequestTypeDef,
     PlaceTypeDef,
     RouteMatrixEntryTypeDef,
     SearchPlaceIndexForSuggestionsResponseTypeDef,
     ListKeysResponseTypeDef,
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
@@ -545,42 +546,42 @@
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

### Comparing `mypy-boto3-location-1.26.86/README.md` & `mypy-boto3-location-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-location"></a>
 
 # mypy-boto3-location
 
 [![PyPI - mypy-boto3-location](https://img.shields.io/pypi/v/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-location?color=blue)](https://pypistats.org/packages/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.26.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,144 +340,145 @@
 ```python
 from mypy_boto3_location.type_defs import (
     ApiKeyFilterTypeDef,
     ApiKeyRestrictionsTypeDef,
     AssociateTrackerConsumerRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDeleteDevicePositionHistoryRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     BatchDeleteGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionRequestRequestTypeDef,
     BatchPutGeofenceSuccessTypeDef,
     CalculateRouteCarModeOptionsTypeDef,
     CalculateRouteMatrixSummaryTypeDef,
     CalculateRouteSummaryTypeDef,
     TruckDimensionsTypeDef,
     TruckWeightTypeDef,
     CircleTypeDef,
     CreateGeofenceCollectionRequestRequestTypeDef,
+    CreateGeofenceCollectionResponseTypeDef,
+    CreateKeyResponseTypeDef,
     MapConfigurationTypeDef,
+    CreateMapResponseTypeDef,
     DataSourceConfigurationTypeDef,
+    CreatePlaceIndexResponseTypeDef,
     CreateRouteCalculatorRequestRequestTypeDef,
+    CreateRouteCalculatorResponseTypeDef,
     CreateTrackerRequestRequestTypeDef,
+    CreateTrackerResponseTypeDef,
     DeleteGeofenceCollectionRequestRequestTypeDef,
     DeleteKeyRequestRequestTypeDef,
     DeleteMapRequestRequestTypeDef,
     DeletePlaceIndexRequestRequestTypeDef,
     DeleteRouteCalculatorRequestRequestTypeDef,
     DeleteTrackerRequestRequestTypeDef,
     DescribeGeofenceCollectionRequestRequestTypeDef,
+    DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DescribeMapRequestRequestTypeDef,
     DescribePlaceIndexRequestRequestTypeDef,
     DescribeRouteCalculatorRequestRequestTypeDef,
+    DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerRequestRequestTypeDef,
+    DescribeTrackerResponseTypeDef,
     PositionalAccuracyTypeDef,
     DisassociateTrackerConsumerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
     GetDevicePositionHistoryRequestRequestTypeDef,
     GetDevicePositionRequestRequestTypeDef,
     GetGeofenceRequestRequestTypeDef,
     GetMapGlyphsRequestRequestTypeDef,
+    GetMapGlyphsResponseTypeDef,
     GetMapSpritesRequestRequestTypeDef,
+    GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorRequestRequestTypeDef,
+    GetMapStyleDescriptorResponseTypeDef,
     GetMapTileRequestRequestTypeDef,
+    GetMapTileResponseTypeDef,
     GetPlaceRequestRequestTypeDef,
     LegGeometryTypeDef,
     StepTypeDef,
+    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
     ListDevicePositionsRequestRequestTypeDef,
+    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
     ListGeofenceCollectionsRequestRequestTypeDef,
     ListGeofenceCollectionsResponseEntryTypeDef,
+    ListGeofencesRequestListGeofencesPaginateTypeDef,
     ListGeofencesRequestRequestTypeDef,
+    ListMapsRequestListMapsPaginateTypeDef,
     ListMapsRequestRequestTypeDef,
     ListMapsResponseEntryTypeDef,
+    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
     ListPlaceIndexesRequestRequestTypeDef,
     ListPlaceIndexesResponseEntryTypeDef,
+    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
     ListRouteCalculatorsRequestRequestTypeDef,
     ListRouteCalculatorsResponseEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
     ListTrackerConsumersRequestRequestTypeDef,
+    ListTrackerConsumersResponseTypeDef,
+    ListTrackersRequestListTrackersPaginateTypeDef,
     ListTrackersRequestRequestTypeDef,
     ListTrackersResponseEntryTypeDef,
+    MapConfigurationUpdateTypeDef,
+    PaginatorConfigTypeDef,
     PlaceGeometryTypeDef,
     TimeZoneTypeDef,
+    PutGeofenceResponseTypeDef,
+    ResponseMetadataTypeDef,
     RouteMatrixEntryErrorTypeDef,
     SearchForSuggestionsResultTypeDef,
     SearchPlaceIndexForPositionRequestRequestTypeDef,
     SearchPlaceIndexForPositionSummaryTypeDef,
     SearchPlaceIndexForSuggestionsRequestRequestTypeDef,
     SearchPlaceIndexForSuggestionsSummaryTypeDef,
     SearchPlaceIndexForTextRequestRequestTypeDef,
     SearchPlaceIndexForTextSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGeofenceCollectionRequestRequestTypeDef,
-    UpdateMapRequestRequestTypeDef,
+    UpdateGeofenceCollectionResponseTypeDef,
+    UpdateKeyResponseTypeDef,
+    UpdateMapResponseTypeDef,
+    UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorRequestRequestTypeDef,
+    UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerRequestRequestTypeDef,
+    UpdateTrackerResponseTypeDef,
+    ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
     CreateKeyRequestRequestTypeDef,
+    DescribeKeyResponseTypeDef,
     ListKeysResponseEntryTypeDef,
     UpdateKeyRequestRequestTypeDef,
     BatchDeleteDevicePositionHistoryErrorTypeDef,
     BatchDeleteGeofenceErrorTypeDef,
     BatchEvaluateGeofencesErrorTypeDef,
     BatchGetDevicePositionErrorTypeDef,
     BatchPutGeofenceErrorTypeDef,
     BatchUpdateDevicePositionErrorTypeDef,
-    CreateGeofenceCollectionResponseTypeDef,
-    CreateKeyResponseTypeDef,
-    CreateMapResponseTypeDef,
-    CreatePlaceIndexResponseTypeDef,
-    CreateRouteCalculatorResponseTypeDef,
-    CreateTrackerResponseTypeDef,
-    DescribeGeofenceCollectionResponseTypeDef,
-    DescribeKeyResponseTypeDef,
-    DescribeRouteCalculatorResponseTypeDef,
-    DescribeTrackerResponseTypeDef,
-    GetMapGlyphsResponseTypeDef,
-    GetMapSpritesResponseTypeDef,
-    GetMapStyleDescriptorResponseTypeDef,
-    GetMapTileResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTrackerConsumersResponseTypeDef,
-    PutGeofenceResponseTypeDef,
-    UpdateGeofenceCollectionResponseTypeDef,
-    UpdateKeyResponseTypeDef,
-    UpdateMapResponseTypeDef,
-    UpdatePlaceIndexResponseTypeDef,
-    UpdateRouteCalculatorResponseTypeDef,
-    UpdateTrackerResponseTypeDef,
     CalculateRouteTruckModeOptionsTypeDef,
     GeofenceGeometryTypeDef,
     CreateMapRequestRequestTypeDef,
     DescribeMapResponseTypeDef,
     CreatePlaceIndexRequestRequestTypeDef,
     DescribePlaceIndexResponseTypeDef,
     UpdatePlaceIndexRequestRequestTypeDef,
     DevicePositionTypeDef,
     DevicePositionUpdateTypeDef,
     GetDevicePositionResponseTypeDef,
     ListDevicePositionsResponseEntryTypeDef,
-    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
-    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
-    ListGeofencesRequestListGeofencesPaginateTypeDef,
-    ListKeysRequestListKeysPaginateTypeDef,
-    ListMapsRequestListMapsPaginateTypeDef,
-    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
-    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
-    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
-    ListTrackersRequestListTrackersPaginateTypeDef,
     LegTypeDef,
     ListGeofenceCollectionsResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackersResponseTypeDef,
+    UpdateMapRequestRequestTypeDef,
     PlaceTypeDef,
     RouteMatrixEntryTypeDef,
     SearchPlaceIndexForSuggestionsResponseTypeDef,
     ListKeysResponseTypeDef,
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
@@ -513,42 +514,42 @@
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

### Comparing `mypy-boto3-location-1.26.86/mypy_boto3_location/__init__.py` & `mypy-boto3-location-1.27.0/mypy_boto3_location/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.26.86/mypy_boto3_location/__init__.pyi` & `mypy-boto3-location-1.27.0/mypy_boto3_location/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.26.86/mypy_boto3_location/__main__.py` & `mypy-boto3-location-1.27.0/mypy_boto3_location/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LocationService 1.26.86\nVersion:         1.26.86\nBuilder"
-        " version: 7.12.5\nDocs:           "
+        "Type annotations for boto3.LocationService 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.86")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-location-1.26.86/mypy_boto3_location/client.py` & `mypy-boto3-location-1.27.0/mypy_boto3_location/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTrackerConsumersResponseTypeDef,
     ListTrackersResponseTypeDef,
     MapConfigurationTypeDef,
+    MapConfigurationUpdateTypeDef,
     PutGeofenceResponseTypeDef,
     SearchPlaceIndexForPositionResponseTypeDef,
     SearchPlaceIndexForSuggestionsResponseTypeDef,
     SearchPlaceIndexForTextResponseTypeDef,
     UpdateGeofenceCollectionResponseTypeDef,
     UpdateKeyResponseTypeDef,
     UpdateMapResponseTypeDef,
@@ -198,15 +199,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#batch_put_geofence)
         """
 
     def batch_update_device_position(
         self, *, TrackerName: str, Updates: Sequence[DevicePositionUpdateTypeDef]
     ) -> BatchUpdateDevicePositionResponseTypeDef:
         """
-        Uploads position update data for one or more devices to a tracker resource.
+        Uploads position update data for one or more devices to a tracker resource (up
+        to 10 devices per batch).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.batch_update_device_position)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#batch_update_device_position)
         """
 
     def calculate_route(
         self,
@@ -681,15 +683,20 @@
         Lists tracker resources in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.list_trackers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#list_trackers)
         """
 
     def put_geofence(
-        self, *, CollectionName: str, GeofenceId: str, Geometry: GeofenceGeometryTypeDef
+        self,
+        *,
+        CollectionName: str,
+        GeofenceId: str,
+        Geometry: GeofenceGeometryTypeDef,
+        GeofenceProperties: Mapping[str, str] = ...
     ) -> PutGeofenceResponseTypeDef:
         """
         Stores a geofence geometry in a given geofence collection, or updates the
         geometry of an existing geofence if a geofence ID is included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.put_geofence)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#put_geofence)
@@ -713,14 +720,15 @@
     def search_place_index_for_suggestions(
         self,
         *,
         IndexName: str,
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
+        FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForSuggestionsResponseTypeDef:
         """
         Generates suggestions for addresses and points of interest based on partial or
         misspelled free-form text.
@@ -732,14 +740,15 @@
     def search_place_index_for_text(
         self,
         *,
         IndexName: str,
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
+        FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForTextResponseTypeDef:
         """
         Geocodes free-form text, such as an address, name, city, or region to allow you
         to search for Places or points of interest.
@@ -794,15 +803,20 @@
         Updates the specified properties of a given API key resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#update_key)
         """
 
     def update_map(
-        self, *, MapName: str, Description: str = ..., PricingPlan: PricingPlanType = ...
+        self,
+        *,
+        MapName: str,
+        ConfigurationUpdate: MapConfigurationUpdateTypeDef = ...,
+        Description: str = ...,
+        PricingPlan: PricingPlanType = ...
     ) -> UpdateMapResponseTypeDef:
         """
         Updates the specified properties of a given map resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_map)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#update_map)
         """
```

### Comparing `mypy-boto3-location-1.26.86/mypy_boto3_location/client.pyi` & `mypy-boto3-location-1.27.0/mypy_boto3_location/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTrackerConsumersResponseTypeDef,
     ListTrackersResponseTypeDef,
     MapConfigurationTypeDef,
+    MapConfigurationUpdateTypeDef,
     PutGeofenceResponseTypeDef,
     SearchPlaceIndexForPositionResponseTypeDef,
     SearchPlaceIndexForSuggestionsResponseTypeDef,
     SearchPlaceIndexForTextResponseTypeDef,
     UpdateGeofenceCollectionResponseTypeDef,
     UpdateKeyResponseTypeDef,
     UpdateMapResponseTypeDef,
@@ -187,15 +188,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.batch_put_geofence)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#batch_put_geofence)
         """
     def batch_update_device_position(
         self, *, TrackerName: str, Updates: Sequence[DevicePositionUpdateTypeDef]
     ) -> BatchUpdateDevicePositionResponseTypeDef:
         """
-        Uploads position update data for one or more devices to a tracker resource.
+        Uploads position update data for one or more devices to a tracker resource (up
+        to 10 devices per batch).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.batch_update_device_position)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#batch_update_device_position)
         """
     def calculate_route(
         self,
         *,
@@ -627,15 +629,20 @@
         """
         Lists tracker resources in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.list_trackers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#list_trackers)
         """
     def put_geofence(
-        self, *, CollectionName: str, GeofenceId: str, Geometry: GeofenceGeometryTypeDef
+        self,
+        *,
+        CollectionName: str,
+        GeofenceId: str,
+        Geometry: GeofenceGeometryTypeDef,
+        GeofenceProperties: Mapping[str, str] = ...
     ) -> PutGeofenceResponseTypeDef:
         """
         Stores a geofence geometry in a given geofence collection, or updates the
         geometry of an existing geofence if a geofence ID is included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.put_geofence)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#put_geofence)
@@ -657,14 +664,15 @@
     def search_place_index_for_suggestions(
         self,
         *,
         IndexName: str,
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
+        FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForSuggestionsResponseTypeDef:
         """
         Generates suggestions for addresses and points of interest based on partial or
         misspelled free-form text.
@@ -675,14 +683,15 @@
     def search_place_index_for_text(
         self,
         *,
         IndexName: str,
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
+        FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForTextResponseTypeDef:
         """
         Geocodes free-form text, such as an address, name, city, or region to allow you
         to search for Places or points of interest.
@@ -732,15 +741,20 @@
         """
         Updates the specified properties of a given API key resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#update_key)
         """
     def update_map(
-        self, *, MapName: str, Description: str = ..., PricingPlan: PricingPlanType = ...
+        self,
+        *,
+        MapName: str,
+        ConfigurationUpdate: MapConfigurationUpdateTypeDef = ...,
+        Description: str = ...,
+        PricingPlan: PricingPlanType = ...
     ) -> UpdateMapResponseTypeDef:
         """
         Updates the specified properties of a given map resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_map)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#update_map)
         """
```

### Comparing `mypy-boto3-location-1.26.86/mypy_boto3_location/literals.py` & `mypy-boto3-location-1.27.0/mypy_boto3_location/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
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
@@ -141,14 +142,15 @@
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
@@ -246,14 +248,15 @@
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
@@ -289,14 +292,15 @@
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
@@ -315,16 +319,19 @@
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
@@ -408,15 +415,17 @@
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

### Comparing `mypy-boto3-location-1.26.86/mypy_boto3_location/literals.pyi` & `mypy-boto3-location-1.27.0/mypy_boto3_location/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
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
@@ -139,14 +140,15 @@
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
@@ -244,14 +246,15 @@
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
@@ -287,14 +290,15 @@
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
@@ -313,16 +317,19 @@
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
@@ -406,15 +413,17 @@
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

### Comparing `mypy-boto3-location-1.26.86/mypy_boto3_location/paginator.py` & `mypy-boto3-location-1.27.0/mypy_boto3_location/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -66,172 +66,160 @@
     "ListMapsPaginator",
     "ListPlaceIndexesPaginator",
     "ListRouteCalculatorsPaginator",
     "ListTrackerConsumersPaginator",
     "ListTrackersPaginator",
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
 class GetDevicePositionHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#getdevicepositionhistorypaginator)
     """
 
     def paginate(
         self,
         *,
         DeviceId: str,
         TrackerName: str,
         EndTimeExclusive: Union[datetime, str] = ...,
         StartTimeInclusive: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDevicePositionHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#getdevicepositionhistorypaginator)
         """
 
-
 class ListDevicePositionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listdevicepositionspaginator)
     """
 
     def paginate(
-        self, *, TrackerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TrackerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDevicePositionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listdevicepositionspaginator)
         """
 
-
 class ListGeofenceCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofenceCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencecollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGeofenceCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofenceCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencecollectionspaginator)
         """
 
-
 class ListGeofencesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofences)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencespaginator)
     """
 
     def paginate(
-        self, *, CollectionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CollectionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGeofencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencespaginator)
         """
 
-
 class ListKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listkeyspaginator)
     """
 
     def paginate(
-        self, *, Filter: ApiKeyFilterTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Filter: ApiKeyFilterTypeDef = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listkeyspaginator)
         """
 
-
 class ListMapsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListMaps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listmapspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMapsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListMaps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listmapspaginator)
         """
 
-
 class ListPlaceIndexesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListPlaceIndexes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listplaceindexespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPlaceIndexesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListPlaceIndexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listplaceindexespaginator)
         """
 
-
 class ListRouteCalculatorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListRouteCalculators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listroutecalculatorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRouteCalculatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListRouteCalculators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listroutecalculatorspaginator)
         """
 
-
 class ListTrackerConsumersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackerConsumers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerconsumerspaginator)
     """
 
     def paginate(
-        self, *, TrackerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TrackerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTrackerConsumersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackerConsumers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerconsumerspaginator)
         """
 
-
 class ListTrackersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTrackersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerspaginator)
         """
```

### Comparing `mypy-boto3-location-1.26.86/mypy_boto3_location/paginator.pyi` & `mypy-boto3-location-1.27.0/mypy_boto3_location/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,160 +66,172 @@
     "ListMapsPaginator",
     "ListPlaceIndexesPaginator",
     "ListRouteCalculatorsPaginator",
     "ListTrackerConsumersPaginator",
     "ListTrackersPaginator",
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
 class GetDevicePositionHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#getdevicepositionhistorypaginator)
     """
 
     def paginate(
         self,
         *,
         DeviceId: str,
         TrackerName: str,
         EndTimeExclusive: Union[datetime, str] = ...,
         StartTimeInclusive: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDevicePositionHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#getdevicepositionhistorypaginator)
         """
 
+
 class ListDevicePositionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listdevicepositionspaginator)
     """
 
     def paginate(
-        self, *, TrackerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TrackerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDevicePositionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listdevicepositionspaginator)
         """
 
+
 class ListGeofenceCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofenceCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencecollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGeofenceCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofenceCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencecollectionspaginator)
         """
 
+
 class ListGeofencesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofences)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencespaginator)
     """
 
     def paginate(
-        self, *, CollectionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CollectionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGeofencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listgeofencespaginator)
         """
 
+
 class ListKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listkeyspaginator)
     """
 
     def paginate(
-        self, *, Filter: ApiKeyFilterTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Filter: ApiKeyFilterTypeDef = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listkeyspaginator)
         """
 
+
 class ListMapsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListMaps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listmapspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMapsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListMaps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listmapspaginator)
         """
 
+
 class ListPlaceIndexesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListPlaceIndexes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listplaceindexespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPlaceIndexesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListPlaceIndexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listplaceindexespaginator)
         """
 
+
 class ListRouteCalculatorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListRouteCalculators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listroutecalculatorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRouteCalculatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListRouteCalculators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listroutecalculatorspaginator)
         """
 
+
 class ListTrackerConsumersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackerConsumers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerconsumerspaginator)
     """
 
     def paginate(
-        self, *, TrackerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TrackerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTrackerConsumersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackerConsumers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerconsumerspaginator)
         """
 
+
 class ListTrackersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTrackersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#listtrackerspaginator)
         """
```

### Comparing `mypy-boto3-location-1.26.86/mypy_boto3_location/type_defs.py` & `mypy-boto3-location-1.27.0/mypy_boto3_location/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,144 +38,145 @@
 
 __all__ = (
     "ApiKeyFilterTypeDef",
     "ApiKeyRestrictionsTypeDef",
     "AssociateTrackerConsumerRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchDeleteGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionRequestRequestTypeDef",
     "BatchPutGeofenceSuccessTypeDef",
     "CalculateRouteCarModeOptionsTypeDef",
     "CalculateRouteMatrixSummaryTypeDef",
     "CalculateRouteSummaryTypeDef",
     "TruckDimensionsTypeDef",
     "TruckWeightTypeDef",
     "CircleTypeDef",
     "CreateGeofenceCollectionRequestRequestTypeDef",
+    "CreateGeofenceCollectionResponseTypeDef",
+    "CreateKeyResponseTypeDef",
     "MapConfigurationTypeDef",
+    "CreateMapResponseTypeDef",
     "DataSourceConfigurationTypeDef",
+    "CreatePlaceIndexResponseTypeDef",
     "CreateRouteCalculatorRequestRequestTypeDef",
+    "CreateRouteCalculatorResponseTypeDef",
     "CreateTrackerRequestRequestTypeDef",
+    "CreateTrackerResponseTypeDef",
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     "DeleteKeyRequestRequestTypeDef",
     "DeleteMapRequestRequestTypeDef",
     "DeletePlaceIndexRequestRequestTypeDef",
     "DeleteRouteCalculatorRequestRequestTypeDef",
     "DeleteTrackerRequestRequestTypeDef",
     "DescribeGeofenceCollectionRequestRequestTypeDef",
+    "DescribeGeofenceCollectionResponseTypeDef",
     "DescribeKeyRequestRequestTypeDef",
     "DescribeMapRequestRequestTypeDef",
     "DescribePlaceIndexRequestRequestTypeDef",
     "DescribeRouteCalculatorRequestRequestTypeDef",
+    "DescribeRouteCalculatorResponseTypeDef",
     "DescribeTrackerRequestRequestTypeDef",
+    "DescribeTrackerResponseTypeDef",
     "PositionalAccuracyTypeDef",
     "DisassociateTrackerConsumerRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
     "GetDevicePositionHistoryRequestRequestTypeDef",
     "GetDevicePositionRequestRequestTypeDef",
     "GetGeofenceRequestRequestTypeDef",
     "GetMapGlyphsRequestRequestTypeDef",
+    "GetMapGlyphsResponseTypeDef",
     "GetMapSpritesRequestRequestTypeDef",
+    "GetMapSpritesResponseTypeDef",
     "GetMapStyleDescriptorRequestRequestTypeDef",
+    "GetMapStyleDescriptorResponseTypeDef",
     "GetMapTileRequestRequestTypeDef",
+    "GetMapTileResponseTypeDef",
     "GetPlaceRequestRequestTypeDef",
     "LegGeometryTypeDef",
     "StepTypeDef",
+    "ListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
     "ListDevicePositionsRequestRequestTypeDef",
+    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
     "ListGeofenceCollectionsRequestRequestTypeDef",
     "ListGeofenceCollectionsResponseEntryTypeDef",
+    "ListGeofencesRequestListGeofencesPaginateTypeDef",
     "ListGeofencesRequestRequestTypeDef",
+    "ListMapsRequestListMapsPaginateTypeDef",
     "ListMapsRequestRequestTypeDef",
     "ListMapsResponseEntryTypeDef",
+    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
     "ListPlaceIndexesRequestRequestTypeDef",
     "ListPlaceIndexesResponseEntryTypeDef",
+    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
     "ListRouteCalculatorsRequestRequestTypeDef",
     "ListRouteCalculatorsResponseEntryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
     "ListTrackerConsumersRequestRequestTypeDef",
+    "ListTrackerConsumersResponseTypeDef",
+    "ListTrackersRequestListTrackersPaginateTypeDef",
     "ListTrackersRequestRequestTypeDef",
     "ListTrackersResponseEntryTypeDef",
+    "MapConfigurationUpdateTypeDef",
+    "PaginatorConfigTypeDef",
     "PlaceGeometryTypeDef",
     "TimeZoneTypeDef",
+    "PutGeofenceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "RouteMatrixEntryErrorTypeDef",
     "SearchForSuggestionsResultTypeDef",
     "SearchPlaceIndexForPositionRequestRequestTypeDef",
     "SearchPlaceIndexForPositionSummaryTypeDef",
     "SearchPlaceIndexForSuggestionsRequestRequestTypeDef",
     "SearchPlaceIndexForSuggestionsSummaryTypeDef",
     "SearchPlaceIndexForTextRequestRequestTypeDef",
     "SearchPlaceIndexForTextSummaryTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGeofenceCollectionRequestRequestTypeDef",
-    "UpdateMapRequestRequestTypeDef",
+    "UpdateGeofenceCollectionResponseTypeDef",
+    "UpdateKeyResponseTypeDef",
+    "UpdateMapResponseTypeDef",
+    "UpdatePlaceIndexResponseTypeDef",
     "UpdateRouteCalculatorRequestRequestTypeDef",
+    "UpdateRouteCalculatorResponseTypeDef",
     "UpdateTrackerRequestRequestTypeDef",
+    "UpdateTrackerResponseTypeDef",
+    "ListKeysRequestListKeysPaginateTypeDef",
     "ListKeysRequestRequestTypeDef",
     "CreateKeyRequestRequestTypeDef",
+    "DescribeKeyResponseTypeDef",
     "ListKeysResponseEntryTypeDef",
     "UpdateKeyRequestRequestTypeDef",
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     "BatchDeleteGeofenceErrorTypeDef",
     "BatchEvaluateGeofencesErrorTypeDef",
     "BatchGetDevicePositionErrorTypeDef",
     "BatchPutGeofenceErrorTypeDef",
     "BatchUpdateDevicePositionErrorTypeDef",
-    "CreateGeofenceCollectionResponseTypeDef",
-    "CreateKeyResponseTypeDef",
-    "CreateMapResponseTypeDef",
-    "CreatePlaceIndexResponseTypeDef",
-    "CreateRouteCalculatorResponseTypeDef",
-    "CreateTrackerResponseTypeDef",
-    "DescribeGeofenceCollectionResponseTypeDef",
-    "DescribeKeyResponseTypeDef",
-    "DescribeRouteCalculatorResponseTypeDef",
-    "DescribeTrackerResponseTypeDef",
-    "GetMapGlyphsResponseTypeDef",
-    "GetMapSpritesResponseTypeDef",
-    "GetMapStyleDescriptorResponseTypeDef",
-    "GetMapTileResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTrackerConsumersResponseTypeDef",
-    "PutGeofenceResponseTypeDef",
-    "UpdateGeofenceCollectionResponseTypeDef",
-    "UpdateKeyResponseTypeDef",
-    "UpdateMapResponseTypeDef",
-    "UpdatePlaceIndexResponseTypeDef",
-    "UpdateRouteCalculatorResponseTypeDef",
-    "UpdateTrackerResponseTypeDef",
     "CalculateRouteTruckModeOptionsTypeDef",
     "GeofenceGeometryTypeDef",
     "CreateMapRequestRequestTypeDef",
     "DescribeMapResponseTypeDef",
     "CreatePlaceIndexRequestRequestTypeDef",
     "DescribePlaceIndexResponseTypeDef",
     "UpdatePlaceIndexRequestRequestTypeDef",
     "DevicePositionTypeDef",
     "DevicePositionUpdateTypeDef",
     "GetDevicePositionResponseTypeDef",
     "ListDevicePositionsResponseEntryTypeDef",
-    "GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
-    "ListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
-    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
-    "ListGeofencesRequestListGeofencesPaginateTypeDef",
-    "ListKeysRequestListKeysPaginateTypeDef",
-    "ListMapsRequestListMapsPaginateTypeDef",
-    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
-    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
-    "ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
-    "ListTrackersRequestListTrackersPaginateTypeDef",
     "LegTypeDef",
     "ListGeofenceCollectionsResponseTypeDef",
     "ListMapsResponseTypeDef",
     "ListPlaceIndexesResponseTypeDef",
     "ListRouteCalculatorsResponseTypeDef",
     "ListTrackersResponseTypeDef",
+    "UpdateMapRequestRequestTypeDef",
     "PlaceTypeDef",
     "RouteMatrixEntryTypeDef",
     "SearchPlaceIndexForSuggestionsResponseTypeDef",
     "ListKeysResponseTypeDef",
     "BatchDeleteDevicePositionHistoryResponseTypeDef",
     "BatchDeleteGeofenceResponseTypeDef",
     "BatchEvaluateGeofencesResponseTypeDef",
@@ -254,25 +255,14 @@
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
     {
         "DeviceIds": Sequence[str],
         "TrackerName": str,
     },
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
 BatchDeleteGeofenceRequestRequestTypeDef = TypedDict(
     "BatchDeleteGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceIds": Sequence[str],
     },
 )
@@ -374,29 +364,82 @@
 class CreateGeofenceCollectionRequestRequestTypeDef(
     _RequiredCreateGeofenceCollectionRequestRequestTypeDef,
     _OptionalCreateGeofenceCollectionRequestRequestTypeDef,
 ):
     pass
 
 
-MapConfigurationTypeDef = TypedDict(
-    "MapConfigurationTypeDef",
+CreateGeofenceCollectionResponseTypeDef = TypedDict(
+    "CreateGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "CreateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateKeyResponseTypeDef = TypedDict(
+    "CreateKeyResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Key": str,
+        "KeyArn": str,
+        "KeyName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredMapConfigurationTypeDef = TypedDict(
+    "_RequiredMapConfigurationTypeDef",
     {
         "Style": str,
     },
 )
+_OptionalMapConfigurationTypeDef = TypedDict(
+    "_OptionalMapConfigurationTypeDef",
+    {
+        "PoliticalView": str,
+    },
+    total=False,
+)
+
+
+class MapConfigurationTypeDef(_RequiredMapConfigurationTypeDef, _OptionalMapConfigurationTypeDef):
+    pass
+
+
+CreateMapResponseTypeDef = TypedDict(
+    "CreateMapResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "MapArn": str,
+        "MapName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 DataSourceConfigurationTypeDef = TypedDict(
     "DataSourceConfigurationTypeDef",
     {
         "IntendedUse": IntendedUseType,
     },
     total=False,
 )
 
+CreatePlaceIndexResponseTypeDef = TypedDict(
+    "CreatePlaceIndexResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "IndexArn": str,
+        "IndexName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateRouteCalculatorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
         "DataSource": str,
     },
 )
@@ -414,14 +457,24 @@
 class CreateRouteCalculatorRequestRequestTypeDef(
     _RequiredCreateRouteCalculatorRequestRequestTypeDef,
     _OptionalCreateRouteCalculatorRequestRequestTypeDef,
 ):
     pass
 
 
+CreateRouteCalculatorResponseTypeDef = TypedDict(
+    "CreateRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "CreateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateTrackerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalCreateTrackerRequestRequestTypeDef = TypedDict(
@@ -440,14 +493,24 @@
 
 class CreateTrackerRequestRequestTypeDef(
     _RequiredCreateTrackerRequestRequestTypeDef, _OptionalCreateTrackerRequestRequestTypeDef
 ):
     pass
 
 
+CreateTrackerResponseTypeDef = TypedDict(
+    "CreateTrackerResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "TrackerArn": str,
+        "TrackerName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteGeofenceCollectionRequestRequestTypeDef = TypedDict(
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 
@@ -489,14 +552,30 @@
 DescribeGeofenceCollectionRequestRequestTypeDef = TypedDict(
     "DescribeGeofenceCollectionRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 
+DescribeGeofenceCollectionResponseTypeDef = TypedDict(
+    "DescribeGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "CreateTime": datetime,
+        "Description": str,
+        "KmsKeyId": str,
+        "PricingPlan": PricingPlanType,
+        "PricingPlanDataSource": str,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeKeyRequestRequestTypeDef = TypedDict(
     "DescribeKeyRequestRequestTypeDef",
     {
         "KeyName": str,
     },
 )
 
@@ -517,21 +596,53 @@
 DescribeRouteCalculatorRequestRequestTypeDef = TypedDict(
     "DescribeRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
     },
 )
 
+DescribeRouteCalculatorResponseTypeDef = TypedDict(
+    "DescribeRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "CreateTime": datetime,
+        "DataSource": str,
+        "Description": str,
+        "PricingPlan": PricingPlanType,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeTrackerRequestRequestTypeDef = TypedDict(
     "DescribeTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 
+DescribeTrackerResponseTypeDef = TypedDict(
+    "DescribeTrackerResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Description": str,
+        "KmsKeyId": str,
+        "PositionFiltering": PositionFilteringType,
+        "PricingPlan": PricingPlanType,
+        "PricingPlanDataSource": str,
+        "Tags": Dict[str, str],
+        "TrackerArn": str,
+        "TrackerName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PositionalAccuracyTypeDef = TypedDict(
     "PositionalAccuracyTypeDef",
     {
         "Horizontal": float,
     },
 )
 
@@ -539,24 +650,39 @@
     "DisassociateTrackerConsumerRequestRequestTypeDef",
     {
         "ConsumerArn": str,
         "TrackerName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DeviceId": str,
+        "TrackerName": str,
+    },
+)
+_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
+    {
+        "EndTimeExclusive": Union[datetime, str],
+        "StartTimeInclusive": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(
+    _RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+    _OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetDevicePositionHistoryRequestRequestTypeDef",
     {
         "DeviceId": str,
         "TrackerName": str,
     },
 )
@@ -614,14 +740,24 @@
 
 class GetMapGlyphsRequestRequestTypeDef(
     _RequiredGetMapGlyphsRequestRequestTypeDef, _OptionalGetMapGlyphsRequestRequestTypeDef
 ):
     pass
 
 
+GetMapGlyphsResponseTypeDef = TypedDict(
+    "GetMapGlyphsResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetMapSpritesRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapSpritesRequestRequestTypeDef",
     {
         "FileName": str,
         "MapName": str,
     },
 )
@@ -636,14 +772,24 @@
 
 class GetMapSpritesRequestRequestTypeDef(
     _RequiredGetMapSpritesRequestRequestTypeDef, _OptionalGetMapSpritesRequestRequestTypeDef
 ):
     pass
 
 
+GetMapSpritesResponseTypeDef = TypedDict(
+    "GetMapSpritesResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetMapStyleDescriptorRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapStyleDescriptorRequestRequestTypeDef",
     {
         "MapName": str,
     },
 )
 _OptionalGetMapStyleDescriptorRequestRequestTypeDef = TypedDict(
@@ -658,14 +804,24 @@
 class GetMapStyleDescriptorRequestRequestTypeDef(
     _RequiredGetMapStyleDescriptorRequestRequestTypeDef,
     _OptionalGetMapStyleDescriptorRequestRequestTypeDef,
 ):
     pass
 
 
+GetMapStyleDescriptorResponseTypeDef = TypedDict(
+    "GetMapStyleDescriptorResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetMapTileRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapTileRequestRequestTypeDef",
     {
         "MapName": str,
         "X": str,
         "Y": str,
         "Z": str,
@@ -682,14 +838,24 @@
 
 class GetMapTileRequestRequestTypeDef(
     _RequiredGetMapTileRequestRequestTypeDef, _OptionalGetMapTileRequestRequestTypeDef
 ):
     pass
 
 
+GetMapTileResponseTypeDef = TypedDict(
+    "GetMapTileResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetPlaceRequestRequestTypeDef = TypedDict(
     "_RequiredGetPlaceRequestRequestTypeDef",
     {
         "IndexName": str,
         "PlaceId": str,
     },
 )
@@ -734,14 +900,36 @@
 )
 
 
 class StepTypeDef(_RequiredStepTypeDef, _OptionalStepTypeDef):
     pass
 
 
+_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
+    "_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    {
+        "TrackerName": str,
+    },
+)
+_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
+    "_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDevicePositionsRequestListDevicePositionsPaginateTypeDef(
+    _RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+    _OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDevicePositionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevicePositionsRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalListDevicePositionsRequestRequestTypeDef = TypedDict(
@@ -757,14 +945,22 @@
 class ListDevicePositionsRequestRequestTypeDef(
     _RequiredListDevicePositionsRequestRequestTypeDef,
     _OptionalListDevicePositionsRequestRequestTypeDef,
 ):
     pass
 
 
+ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef = TypedDict(
+    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGeofenceCollectionsRequestRequestTypeDef = TypedDict(
     "ListGeofenceCollectionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -792,14 +988,36 @@
 class ListGeofenceCollectionsResponseEntryTypeDef(
     _RequiredListGeofenceCollectionsResponseEntryTypeDef,
     _OptionalListGeofenceCollectionsResponseEntryTypeDef,
 ):
     pass
 
 
+_RequiredListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
+    "_RequiredListGeofencesRequestListGeofencesPaginateTypeDef",
+    {
+        "CollectionName": str,
+    },
+)
+_OptionalListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
+    "_OptionalListGeofencesRequestListGeofencesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListGeofencesRequestListGeofencesPaginateTypeDef(
+    _RequiredListGeofencesRequestListGeofencesPaginateTypeDef,
+    _OptionalListGeofencesRequestListGeofencesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListGeofencesRequestRequestTypeDef = TypedDict(
     "_RequiredListGeofencesRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 _OptionalListGeofencesRequestRequestTypeDef = TypedDict(
@@ -814,14 +1032,22 @@
 
 class ListGeofencesRequestRequestTypeDef(
     _RequiredListGeofencesRequestRequestTypeDef, _OptionalListGeofencesRequestRequestTypeDef
 ):
     pass
 
 
+ListMapsRequestListMapsPaginateTypeDef = TypedDict(
+    "ListMapsRequestListMapsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMapsRequestRequestTypeDef = TypedDict(
     "ListMapsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -848,14 +1074,22 @@
 
 class ListMapsResponseEntryTypeDef(
     _RequiredListMapsResponseEntryTypeDef, _OptionalListMapsResponseEntryTypeDef
 ):
     pass
 
 
+ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef = TypedDict(
+    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPlaceIndexesRequestRequestTypeDef = TypedDict(
     "ListPlaceIndexesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -882,14 +1116,22 @@
 
 class ListPlaceIndexesResponseEntryTypeDef(
     _RequiredListPlaceIndexesResponseEntryTypeDef, _OptionalListPlaceIndexesResponseEntryTypeDef
 ):
     pass
 
 
+ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef = TypedDict(
+    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRouteCalculatorsRequestRequestTypeDef = TypedDict(
     "ListRouteCalculatorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -924,14 +1166,44 @@
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
+_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
+    "_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    {
+        "TrackerName": str,
+    },
+)
+_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
+    "_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef(
+    _RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+    _OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTrackerConsumersRequestRequestTypeDef = TypedDict(
     "_RequiredListTrackerConsumersRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalListTrackerConsumersRequestRequestTypeDef = TypedDict(
@@ -947,14 +1219,31 @@
 class ListTrackerConsumersRequestRequestTypeDef(
     _RequiredListTrackerConsumersRequestRequestTypeDef,
     _OptionalListTrackerConsumersRequestRequestTypeDef,
 ):
     pass
 
 
+ListTrackerConsumersResponseTypeDef = TypedDict(
+    "ListTrackerConsumersResponseTypeDef",
+    {
+        "ConsumerArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTrackersRequestListTrackersPaginateTypeDef = TypedDict(
+    "ListTrackersRequestListTrackersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTrackersRequestRequestTypeDef = TypedDict(
     "ListTrackersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -981,14 +1270,32 @@
 
 class ListTrackersResponseEntryTypeDef(
     _RequiredListTrackersResponseEntryTypeDef, _OptionalListTrackersResponseEntryTypeDef
 ):
     pass
 
 
+MapConfigurationUpdateTypeDef = TypedDict(
+    "MapConfigurationUpdateTypeDef",
+    {
+        "PoliticalView": str,
+    },
+    total=False,
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
 PlaceGeometryTypeDef = TypedDict(
     "PlaceGeometryTypeDef",
     {
         "Point": List[float],
     },
     total=False,
 )
@@ -1008,14 +1315,35 @@
 )
 
 
 class TimeZoneTypeDef(_RequiredTimeZoneTypeDef, _OptionalTimeZoneTypeDef):
     pass
 
 
+PutGeofenceResponseTypeDef = TypedDict(
+    "PutGeofenceResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "GeofenceId": str,
+        "UpdateTime": datetime,
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
 _RequiredRouteMatrixEntryErrorTypeDef = TypedDict(
     "_RequiredRouteMatrixEntryErrorTypeDef",
     {
         "Code": RouteMatrixErrorCodeType,
     },
 )
 _OptionalRouteMatrixEntryErrorTypeDef = TypedDict(
@@ -1038,15 +1366,17 @@
     {
         "Text": str,
     },
 )
 _OptionalSearchForSuggestionsResultTypeDef = TypedDict(
     "_OptionalSearchForSuggestionsResultTypeDef",
     {
+        "Categories": List[str],
         "PlaceId": str,
+        "SupplementalCategories": List[str],
     },
     total=False,
 )
 
 
 class SearchForSuggestionsResultTypeDef(
     _RequiredSearchForSuggestionsResultTypeDef, _OptionalSearchForSuggestionsResultTypeDef
@@ -1110,14 +1440,15 @@
     },
 )
 _OptionalSearchPlaceIndexForSuggestionsRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForSuggestionsRequestRequestTypeDef",
     {
         "BiasPosition": Sequence[float],
         "FilterBBox": Sequence[float],
+        "FilterCategories": Sequence[str],
         "FilterCountries": Sequence[str],
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
@@ -1137,14 +1468,15 @@
     },
 )
 _OptionalSearchPlaceIndexForSuggestionsSummaryTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForSuggestionsSummaryTypeDef",
     {
         "BiasPosition": List[float],
         "FilterBBox": List[float],
+        "FilterCategories": List[str],
         "FilterCountries": List[str],
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
@@ -1164,14 +1496,15 @@
     },
 )
 _OptionalSearchPlaceIndexForTextRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForTextRequestRequestTypeDef",
     {
         "BiasPosition": Sequence[float],
         "FilterBBox": Sequence[float],
+        "FilterCategories": Sequence[str],
         "FilterCountries": Sequence[str],
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
@@ -1191,14 +1524,15 @@
     },
 )
 _OptionalSearchPlaceIndexForTextSummaryTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForTextSummaryTypeDef",
     {
         "BiasPosition": List[float],
         "FilterBBox": List[float],
+        "FilterCategories": List[str],
         "FilterCountries": List[str],
         "Language": str,
         "MaxResults": int,
         "ResultBBox": List[float],
     },
     total=False,
 )
@@ -1246,35 +1580,53 @@
 class UpdateGeofenceCollectionRequestRequestTypeDef(
     _RequiredUpdateGeofenceCollectionRequestRequestTypeDef,
     _OptionalUpdateGeofenceCollectionRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredUpdateMapRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMapRequestRequestTypeDef",
+UpdateGeofenceCollectionResponseTypeDef = TypedDict(
+    "UpdateGeofenceCollectionResponseTypeDef",
     {
-        "MapName": str,
+        "CollectionArn": str,
+        "CollectionName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalUpdateMapRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMapRequestRequestTypeDef",
+
+UpdateKeyResponseTypeDef = TypedDict(
+    "UpdateKeyResponseTypeDef",
     {
-        "Description": str,
-        "PricingPlan": PricingPlanType,
+        "KeyArn": str,
+        "KeyName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
+UpdateMapResponseTypeDef = TypedDict(
+    "UpdateMapResponseTypeDef",
+    {
+        "MapArn": str,
+        "MapName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-class UpdateMapRequestRequestTypeDef(
-    _RequiredUpdateMapRequestRequestTypeDef, _OptionalUpdateMapRequestRequestTypeDef
-):
-    pass
-
+UpdatePlaceIndexResponseTypeDef = TypedDict(
+    "UpdatePlaceIndexResponseTypeDef",
+    {
+        "IndexArn": str,
+        "IndexName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredUpdateRouteCalculatorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
     },
 )
@@ -1291,14 +1643,24 @@
 class UpdateRouteCalculatorRequestRequestTypeDef(
     _RequiredUpdateRouteCalculatorRequestRequestTypeDef,
     _OptionalUpdateRouteCalculatorRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateRouteCalculatorResponseTypeDef = TypedDict(
+    "UpdateRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateTrackerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalUpdateTrackerRequestRequestTypeDef = TypedDict(
@@ -1315,14 +1677,33 @@
 
 class UpdateTrackerRequestRequestTypeDef(
     _RequiredUpdateTrackerRequestRequestTypeDef, _OptionalUpdateTrackerRequestRequestTypeDef
 ):
     pass
 
 
+UpdateTrackerResponseTypeDef = TypedDict(
+    "UpdateTrackerResponseTypeDef",
+    {
+        "TrackerArn": str,
+        "TrackerName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListKeysRequestListKeysPaginateTypeDef = TypedDict(
+    "ListKeysRequestListKeysPaginateTypeDef",
+    {
+        "Filter": ApiKeyFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListKeysRequestRequestTypeDef = TypedDict(
     "ListKeysRequestRequestTypeDef",
     {
         "Filter": ApiKeyFilterTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -1350,14 +1731,30 @@
 
 class CreateKeyRequestRequestTypeDef(
     _RequiredCreateKeyRequestRequestTypeDef, _OptionalCreateKeyRequestRequestTypeDef
 ):
     pass
 
 
+DescribeKeyResponseTypeDef = TypedDict(
+    "DescribeKeyResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Description": str,
+        "ExpireTime": datetime,
+        "Key": str,
+        "KeyArn": str,
+        "KeyName": str,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListKeysResponseEntryTypeDef = TypedDict(
     "_RequiredListKeysResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "ExpireTime": datetime,
         "KeyName": str,
         "Restrictions": ApiKeyRestrictionsTypeDef,
@@ -1450,266 +1847,14 @@
     {
         "DeviceId": str,
         "Error": BatchItemErrorTypeDef,
         "SampleTime": datetime,
     },
 )
 
-CreateGeofenceCollectionResponseTypeDef = TypedDict(
-    "CreateGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "CreateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateKeyResponseTypeDef = TypedDict(
-    "CreateKeyResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Key": str,
-        "KeyArn": str,
-        "KeyName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMapResponseTypeDef = TypedDict(
-    "CreateMapResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "MapArn": str,
-        "MapName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePlaceIndexResponseTypeDef = TypedDict(
-    "CreatePlaceIndexResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "IndexArn": str,
-        "IndexName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRouteCalculatorResponseTypeDef = TypedDict(
-    "CreateRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "CreateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTrackerResponseTypeDef = TypedDict(
-    "CreateTrackerResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "TrackerArn": str,
-        "TrackerName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeGeofenceCollectionResponseTypeDef = TypedDict(
-    "DescribeGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "CreateTime": datetime,
-        "Description": str,
-        "KmsKeyId": str,
-        "PricingPlan": PricingPlanType,
-        "PricingPlanDataSource": str,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeKeyResponseTypeDef = TypedDict(
-    "DescribeKeyResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Description": str,
-        "ExpireTime": datetime,
-        "Key": str,
-        "KeyArn": str,
-        "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRouteCalculatorResponseTypeDef = TypedDict(
-    "DescribeRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "CreateTime": datetime,
-        "DataSource": str,
-        "Description": str,
-        "PricingPlan": PricingPlanType,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeTrackerResponseTypeDef = TypedDict(
-    "DescribeTrackerResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Description": str,
-        "KmsKeyId": str,
-        "PositionFiltering": PositionFilteringType,
-        "PricingPlan": PricingPlanType,
-        "PricingPlanDataSource": str,
-        "Tags": Dict[str, str],
-        "TrackerArn": str,
-        "TrackerName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMapGlyphsResponseTypeDef = TypedDict(
-    "GetMapGlyphsResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMapSpritesResponseTypeDef = TypedDict(
-    "GetMapSpritesResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMapStyleDescriptorResponseTypeDef = TypedDict(
-    "GetMapStyleDescriptorResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMapTileResponseTypeDef = TypedDict(
-    "GetMapTileResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
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
-ListTrackerConsumersResponseTypeDef = TypedDict(
-    "ListTrackerConsumersResponseTypeDef",
-    {
-        "ConsumerArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutGeofenceResponseTypeDef = TypedDict(
-    "PutGeofenceResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "GeofenceId": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGeofenceCollectionResponseTypeDef = TypedDict(
-    "UpdateGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateKeyResponseTypeDef = TypedDict(
-    "UpdateKeyResponseTypeDef",
-    {
-        "KeyArn": str,
-        "KeyName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMapResponseTypeDef = TypedDict(
-    "UpdateMapResponseTypeDef",
-    {
-        "MapArn": str,
-        "MapName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePlaceIndexResponseTypeDef = TypedDict(
-    "UpdatePlaceIndexResponseTypeDef",
-    {
-        "IndexArn": str,
-        "IndexName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateRouteCalculatorResponseTypeDef = TypedDict(
-    "UpdateRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTrackerResponseTypeDef = TypedDict(
-    "UpdateTrackerResponseTypeDef",
-    {
-        "TrackerArn": str,
-        "TrackerName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CalculateRouteTruckModeOptionsTypeDef = TypedDict(
     "CalculateRouteTruckModeOptionsTypeDef",
     {
         "AvoidFerries": bool,
         "AvoidTolls": bool,
         "Dimensions": TruckDimensionsTypeDef,
         "Weight": TruckWeightTypeDef,
@@ -1758,15 +1903,15 @@
         "DataSource": str,
         "Description": str,
         "MapArn": str,
         "MapName": str,
         "PricingPlan": PricingPlanType,
         "Tags": Dict[str, str],
         "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePlaceIndexRequestRequestTypeDef",
     {
         "DataSource": str,
@@ -1799,15 +1944,15 @@
         "DataSourceConfiguration": DataSourceConfigurationTypeDef,
         "Description": str,
         "IndexArn": str,
         "IndexName": str,
         "PricingPlan": PricingPlanType,
         "Tags": Dict[str, str],
         "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePlaceIndexRequestRequestTypeDef",
     {
         "IndexName": str,
@@ -1882,15 +2027,15 @@
     {
         "Accuracy": PositionalAccuracyTypeDef,
         "DeviceId": str,
         "Position": List[float],
         "PositionProperties": Dict[str, str],
         "ReceivedTime": datetime,
         "SampleTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListDevicePositionsResponseEntryTypeDef = TypedDict(
     "_RequiredListDevicePositionsResponseEntryTypeDef",
     {
         "DeviceId": str,
@@ -1911,154 +2056,14 @@
 class ListDevicePositionsResponseEntryTypeDef(
     _RequiredListDevicePositionsResponseEntryTypeDef,
     _OptionalListDevicePositionsResponseEntryTypeDef,
 ):
     pass
 
 
-_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
-    {
-        "DeviceId": str,
-        "TrackerName": str,
-    },
-)
-_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
-    {
-        "EndTimeExclusive": Union[datetime, str],
-        "StartTimeInclusive": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(
-    _RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-    _OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
-    "_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
-    {
-        "TrackerName": str,
-    },
-)
-_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
-    "_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDevicePositionsRequestListDevicePositionsPaginateTypeDef(
-    _RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
-    _OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
-):
-    pass
-
-
-ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef = TypedDict(
-    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
-    "_RequiredListGeofencesRequestListGeofencesPaginateTypeDef",
-    {
-        "CollectionName": str,
-    },
-)
-_OptionalListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
-    "_OptionalListGeofencesRequestListGeofencesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListGeofencesRequestListGeofencesPaginateTypeDef(
-    _RequiredListGeofencesRequestListGeofencesPaginateTypeDef,
-    _OptionalListGeofencesRequestListGeofencesPaginateTypeDef,
-):
-    pass
-
-
-ListKeysRequestListKeysPaginateTypeDef = TypedDict(
-    "ListKeysRequestListKeysPaginateTypeDef",
-    {
-        "Filter": ApiKeyFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListMapsRequestListMapsPaginateTypeDef = TypedDict(
-    "ListMapsRequestListMapsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef = TypedDict(
-    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef = TypedDict(
-    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
-    "_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
-    {
-        "TrackerName": str,
-    },
-)
-_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
-    "_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef(
-    _RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
-    _OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
-):
-    pass
-
-
-ListTrackersRequestListTrackersPaginateTypeDef = TypedDict(
-    "ListTrackersRequestListTrackersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredLegTypeDef = TypedDict(
     "_RequiredLegTypeDef",
     {
         "Distance": float,
         "DurationSeconds": float,
         "EndPosition": List[float],
         "StartPosition": List[float],
@@ -2079,73 +2084,98 @@
 
 
 ListGeofenceCollectionsResponseTypeDef = TypedDict(
     "ListGeofenceCollectionsResponseTypeDef",
     {
         "Entries": List[ListGeofenceCollectionsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMapsResponseTypeDef = TypedDict(
     "ListMapsResponseTypeDef",
     {
         "Entries": List[ListMapsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPlaceIndexesResponseTypeDef = TypedDict(
     "ListPlaceIndexesResponseTypeDef",
     {
         "Entries": List[ListPlaceIndexesResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRouteCalculatorsResponseTypeDef = TypedDict(
     "ListRouteCalculatorsResponseTypeDef",
     {
         "Entries": List[ListRouteCalculatorsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrackersResponseTypeDef = TypedDict(
     "ListTrackersResponseTypeDef",
     {
         "Entries": List[ListTrackersResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredUpdateMapRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMapRequestRequestTypeDef",
+    {
+        "MapName": str,
+    },
+)
+_OptionalUpdateMapRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMapRequestRequestTypeDef",
+    {
+        "ConfigurationUpdate": MapConfigurationUpdateTypeDef,
+        "Description": str,
+        "PricingPlan": PricingPlanType,
     },
+    total=False,
 )
 
+
+class UpdateMapRequestRequestTypeDef(
+    _RequiredUpdateMapRequestRequestTypeDef, _OptionalUpdateMapRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredPlaceTypeDef = TypedDict(
     "_RequiredPlaceTypeDef",
     {
         "Geometry": PlaceGeometryTypeDef,
     },
 )
 _OptionalPlaceTypeDef = TypedDict(
     "_OptionalPlaceTypeDef",
     {
         "AddressNumber": str,
+        "Categories": List[str],
         "Country": str,
         "Interpolated": bool,
         "Label": str,
         "Municipality": str,
         "Neighborhood": str,
         "PostalCode": str,
         "Region": str,
         "Street": str,
         "SubRegion": str,
+        "SupplementalCategories": List[str],
         "TimeZone": TimeZoneTypeDef,
         "UnitNumber": str,
         "UnitType": str,
     },
     total=False,
 )
 
@@ -2165,65 +2195,65 @@
 )
 
 SearchPlaceIndexForSuggestionsResponseTypeDef = TypedDict(
     "SearchPlaceIndexForSuggestionsResponseTypeDef",
     {
         "Results": List[SearchForSuggestionsResultTypeDef],
         "Summary": SearchPlaceIndexForSuggestionsSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKeysResponseTypeDef = TypedDict(
     "ListKeysResponseTypeDef",
     {
         "Entries": List[ListKeysResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteDevicePositionHistoryResponseTypeDef = TypedDict(
     "BatchDeleteDevicePositionHistoryResponseTypeDef",
     {
         "Errors": List[BatchDeleteDevicePositionHistoryErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteGeofenceResponseTypeDef = TypedDict(
     "BatchDeleteGeofenceResponseTypeDef",
     {
         "Errors": List[BatchDeleteGeofenceErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchEvaluateGeofencesResponseTypeDef = TypedDict(
     "BatchEvaluateGeofencesResponseTypeDef",
     {
         "Errors": List[BatchEvaluateGeofencesErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutGeofenceResponseTypeDef = TypedDict(
     "BatchPutGeofenceResponseTypeDef",
     {
         "Errors": List[BatchPutGeofenceErrorTypeDef],
         "Successes": List[BatchPutGeofenceSuccessTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateDevicePositionResponseTypeDef = TypedDict(
     "BatchUpdateDevicePositionResponseTypeDef",
     {
         "Errors": List[BatchUpdateDevicePositionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCalculateRouteMatrixRequestRequestTypeDef = TypedDict(
     "_RequiredCalculateRouteMatrixRequestRequestTypeDef",
     {
         "CalculatorName": str,
@@ -2278,69 +2308,112 @@
 
 class CalculateRouteRequestRequestTypeDef(
     _RequiredCalculateRouteRequestRequestTypeDef, _OptionalCalculateRouteRequestRequestTypeDef
 ):
     pass
 
 
-BatchPutGeofenceRequestEntryTypeDef = TypedDict(
-    "BatchPutGeofenceRequestEntryTypeDef",
+_RequiredBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_RequiredBatchPutGeofenceRequestEntryTypeDef",
     {
         "GeofenceId": str,
         "Geometry": GeofenceGeometryTypeDef,
     },
 )
+_OptionalBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_OptionalBatchPutGeofenceRequestEntryTypeDef",
+    {
+        "GeofenceProperties": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class BatchPutGeofenceRequestEntryTypeDef(
+    _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
+):
+    pass
+
 
 GetGeofenceResponseTypeDef = TypedDict(
     "GetGeofenceResponseTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
+        "GeofenceProperties": Dict[str, str],
         "Geometry": GeofenceGeometryTypeDef,
         "Status": str,
         "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListGeofenceResponseEntryTypeDef = TypedDict(
-    "ListGeofenceResponseEntryTypeDef",
+_RequiredListGeofenceResponseEntryTypeDef = TypedDict(
+    "_RequiredListGeofenceResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
         "Geometry": GeofenceGeometryTypeDef,
         "Status": str,
         "UpdateTime": datetime,
     },
 )
+_OptionalListGeofenceResponseEntryTypeDef = TypedDict(
+    "_OptionalListGeofenceResponseEntryTypeDef",
+    {
+        "GeofenceProperties": Dict[str, str],
+    },
+    total=False,
+)
 
-PutGeofenceRequestRequestTypeDef = TypedDict(
-    "PutGeofenceRequestRequestTypeDef",
+
+class ListGeofenceResponseEntryTypeDef(
+    _RequiredListGeofenceResponseEntryTypeDef, _OptionalListGeofenceResponseEntryTypeDef
+):
+    pass
+
+
+_RequiredPutGeofenceRequestRequestTypeDef = TypedDict(
+    "_RequiredPutGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceId": str,
         "Geometry": GeofenceGeometryTypeDef,
     },
 )
+_OptionalPutGeofenceRequestRequestTypeDef = TypedDict(
+    "_OptionalPutGeofenceRequestRequestTypeDef",
+    {
+        "GeofenceProperties": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class PutGeofenceRequestRequestTypeDef(
+    _RequiredPutGeofenceRequestRequestTypeDef, _OptionalPutGeofenceRequestRequestTypeDef
+):
+    pass
+
 
 BatchGetDevicePositionResponseTypeDef = TypedDict(
     "BatchGetDevicePositionResponseTypeDef",
     {
         "DevicePositions": List[DevicePositionTypeDef],
         "Errors": List[BatchGetDevicePositionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDevicePositionHistoryResponseTypeDef = TypedDict(
     "GetDevicePositionHistoryResponseTypeDef",
     {
         "DevicePositions": List[DevicePositionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchEvaluateGeofencesRequestRequestTypeDef = TypedDict(
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     {
         "CollectionName": str,
@@ -2357,32 +2430,32 @@
 )
 
 ListDevicePositionsResponseTypeDef = TypedDict(
     "ListDevicePositionsResponseTypeDef",
     {
         "Entries": List[ListDevicePositionsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CalculateRouteResponseTypeDef = TypedDict(
     "CalculateRouteResponseTypeDef",
     {
         "Legs": List[LegTypeDef],
         "Summary": CalculateRouteSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPlaceResponseTypeDef = TypedDict(
     "GetPlaceResponseTypeDef",
     {
         "Place": PlaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchForPositionResultTypeDef = TypedDict(
     "_RequiredSearchForPositionResultTypeDef",
     {
         "Distance": float,
@@ -2430,15 +2503,15 @@
 CalculateRouteMatrixResponseTypeDef = TypedDict(
     "CalculateRouteMatrixResponseTypeDef",
     {
         "RouteMatrix": List[List[RouteMatrixEntryTypeDef]],
         "SnappedDeparturePositions": List[List[float]],
         "SnappedDestinationPositions": List[List[float]],
         "Summary": CalculateRouteMatrixSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutGeofenceRequestRequestTypeDef = TypedDict(
     "BatchPutGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
@@ -2447,28 +2520,28 @@
 )
 
 ListGeofencesResponseTypeDef = TypedDict(
     "ListGeofencesResponseTypeDef",
     {
         "Entries": List[ListGeofenceResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchPlaceIndexForPositionResponseTypeDef = TypedDict(
     "SearchPlaceIndexForPositionResponseTypeDef",
     {
         "Results": List[SearchForPositionResultTypeDef],
         "Summary": SearchPlaceIndexForPositionSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchPlaceIndexForTextResponseTypeDef = TypedDict(
     "SearchPlaceIndexForTextResponseTypeDef",
     {
         "Results": List[SearchForTextResultTypeDef],
         "Summary": SearchPlaceIndexForTextSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-location-1.26.86/mypy_boto3_location/type_defs.pyi` & `mypy-boto3-location-1.27.0/mypy_boto3_location/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -37,144 +37,145 @@
 
 __all__ = (
     "ApiKeyFilterTypeDef",
     "ApiKeyRestrictionsTypeDef",
     "AssociateTrackerConsumerRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchDeleteGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionRequestRequestTypeDef",
     "BatchPutGeofenceSuccessTypeDef",
     "CalculateRouteCarModeOptionsTypeDef",
     "CalculateRouteMatrixSummaryTypeDef",
     "CalculateRouteSummaryTypeDef",
     "TruckDimensionsTypeDef",
     "TruckWeightTypeDef",
     "CircleTypeDef",
     "CreateGeofenceCollectionRequestRequestTypeDef",
+    "CreateGeofenceCollectionResponseTypeDef",
+    "CreateKeyResponseTypeDef",
     "MapConfigurationTypeDef",
+    "CreateMapResponseTypeDef",
     "DataSourceConfigurationTypeDef",
+    "CreatePlaceIndexResponseTypeDef",
     "CreateRouteCalculatorRequestRequestTypeDef",
+    "CreateRouteCalculatorResponseTypeDef",
     "CreateTrackerRequestRequestTypeDef",
+    "CreateTrackerResponseTypeDef",
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     "DeleteKeyRequestRequestTypeDef",
     "DeleteMapRequestRequestTypeDef",
     "DeletePlaceIndexRequestRequestTypeDef",
     "DeleteRouteCalculatorRequestRequestTypeDef",
     "DeleteTrackerRequestRequestTypeDef",
     "DescribeGeofenceCollectionRequestRequestTypeDef",
+    "DescribeGeofenceCollectionResponseTypeDef",
     "DescribeKeyRequestRequestTypeDef",
     "DescribeMapRequestRequestTypeDef",
     "DescribePlaceIndexRequestRequestTypeDef",
     "DescribeRouteCalculatorRequestRequestTypeDef",
+    "DescribeRouteCalculatorResponseTypeDef",
     "DescribeTrackerRequestRequestTypeDef",
+    "DescribeTrackerResponseTypeDef",
     "PositionalAccuracyTypeDef",
     "DisassociateTrackerConsumerRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
     "GetDevicePositionHistoryRequestRequestTypeDef",
     "GetDevicePositionRequestRequestTypeDef",
     "GetGeofenceRequestRequestTypeDef",
     "GetMapGlyphsRequestRequestTypeDef",
+    "GetMapGlyphsResponseTypeDef",
     "GetMapSpritesRequestRequestTypeDef",
+    "GetMapSpritesResponseTypeDef",
     "GetMapStyleDescriptorRequestRequestTypeDef",
+    "GetMapStyleDescriptorResponseTypeDef",
     "GetMapTileRequestRequestTypeDef",
+    "GetMapTileResponseTypeDef",
     "GetPlaceRequestRequestTypeDef",
     "LegGeometryTypeDef",
     "StepTypeDef",
+    "ListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
     "ListDevicePositionsRequestRequestTypeDef",
+    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
     "ListGeofenceCollectionsRequestRequestTypeDef",
     "ListGeofenceCollectionsResponseEntryTypeDef",
+    "ListGeofencesRequestListGeofencesPaginateTypeDef",
     "ListGeofencesRequestRequestTypeDef",
+    "ListMapsRequestListMapsPaginateTypeDef",
     "ListMapsRequestRequestTypeDef",
     "ListMapsResponseEntryTypeDef",
+    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
     "ListPlaceIndexesRequestRequestTypeDef",
     "ListPlaceIndexesResponseEntryTypeDef",
+    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
     "ListRouteCalculatorsRequestRequestTypeDef",
     "ListRouteCalculatorsResponseEntryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
     "ListTrackerConsumersRequestRequestTypeDef",
+    "ListTrackerConsumersResponseTypeDef",
+    "ListTrackersRequestListTrackersPaginateTypeDef",
     "ListTrackersRequestRequestTypeDef",
     "ListTrackersResponseEntryTypeDef",
+    "MapConfigurationUpdateTypeDef",
+    "PaginatorConfigTypeDef",
     "PlaceGeometryTypeDef",
     "TimeZoneTypeDef",
+    "PutGeofenceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "RouteMatrixEntryErrorTypeDef",
     "SearchForSuggestionsResultTypeDef",
     "SearchPlaceIndexForPositionRequestRequestTypeDef",
     "SearchPlaceIndexForPositionSummaryTypeDef",
     "SearchPlaceIndexForSuggestionsRequestRequestTypeDef",
     "SearchPlaceIndexForSuggestionsSummaryTypeDef",
     "SearchPlaceIndexForTextRequestRequestTypeDef",
     "SearchPlaceIndexForTextSummaryTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGeofenceCollectionRequestRequestTypeDef",
-    "UpdateMapRequestRequestTypeDef",
+    "UpdateGeofenceCollectionResponseTypeDef",
+    "UpdateKeyResponseTypeDef",
+    "UpdateMapResponseTypeDef",
+    "UpdatePlaceIndexResponseTypeDef",
     "UpdateRouteCalculatorRequestRequestTypeDef",
+    "UpdateRouteCalculatorResponseTypeDef",
     "UpdateTrackerRequestRequestTypeDef",
+    "UpdateTrackerResponseTypeDef",
+    "ListKeysRequestListKeysPaginateTypeDef",
     "ListKeysRequestRequestTypeDef",
     "CreateKeyRequestRequestTypeDef",
+    "DescribeKeyResponseTypeDef",
     "ListKeysResponseEntryTypeDef",
     "UpdateKeyRequestRequestTypeDef",
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     "BatchDeleteGeofenceErrorTypeDef",
     "BatchEvaluateGeofencesErrorTypeDef",
     "BatchGetDevicePositionErrorTypeDef",
     "BatchPutGeofenceErrorTypeDef",
     "BatchUpdateDevicePositionErrorTypeDef",
-    "CreateGeofenceCollectionResponseTypeDef",
-    "CreateKeyResponseTypeDef",
-    "CreateMapResponseTypeDef",
-    "CreatePlaceIndexResponseTypeDef",
-    "CreateRouteCalculatorResponseTypeDef",
-    "CreateTrackerResponseTypeDef",
-    "DescribeGeofenceCollectionResponseTypeDef",
-    "DescribeKeyResponseTypeDef",
-    "DescribeRouteCalculatorResponseTypeDef",
-    "DescribeTrackerResponseTypeDef",
-    "GetMapGlyphsResponseTypeDef",
-    "GetMapSpritesResponseTypeDef",
-    "GetMapStyleDescriptorResponseTypeDef",
-    "GetMapTileResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTrackerConsumersResponseTypeDef",
-    "PutGeofenceResponseTypeDef",
-    "UpdateGeofenceCollectionResponseTypeDef",
-    "UpdateKeyResponseTypeDef",
-    "UpdateMapResponseTypeDef",
-    "UpdatePlaceIndexResponseTypeDef",
-    "UpdateRouteCalculatorResponseTypeDef",
-    "UpdateTrackerResponseTypeDef",
     "CalculateRouteTruckModeOptionsTypeDef",
     "GeofenceGeometryTypeDef",
     "CreateMapRequestRequestTypeDef",
     "DescribeMapResponseTypeDef",
     "CreatePlaceIndexRequestRequestTypeDef",
     "DescribePlaceIndexResponseTypeDef",
     "UpdatePlaceIndexRequestRequestTypeDef",
     "DevicePositionTypeDef",
     "DevicePositionUpdateTypeDef",
     "GetDevicePositionResponseTypeDef",
     "ListDevicePositionsResponseEntryTypeDef",
-    "GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
-    "ListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
-    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
-    "ListGeofencesRequestListGeofencesPaginateTypeDef",
-    "ListKeysRequestListKeysPaginateTypeDef",
-    "ListMapsRequestListMapsPaginateTypeDef",
-    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
-    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
-    "ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
-    "ListTrackersRequestListTrackersPaginateTypeDef",
     "LegTypeDef",
     "ListGeofenceCollectionsResponseTypeDef",
     "ListMapsResponseTypeDef",
     "ListPlaceIndexesResponseTypeDef",
     "ListRouteCalculatorsResponseTypeDef",
     "ListTrackersResponseTypeDef",
+    "UpdateMapRequestRequestTypeDef",
     "PlaceTypeDef",
     "RouteMatrixEntryTypeDef",
     "SearchPlaceIndexForSuggestionsResponseTypeDef",
     "ListKeysResponseTypeDef",
     "BatchDeleteDevicePositionHistoryResponseTypeDef",
     "BatchDeleteGeofenceResponseTypeDef",
     "BatchEvaluateGeofencesResponseTypeDef",
@@ -251,25 +252,14 @@
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
     {
         "DeviceIds": Sequence[str],
         "TrackerName": str,
     },
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
 BatchDeleteGeofenceRequestRequestTypeDef = TypedDict(
     "BatchDeleteGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceIds": Sequence[str],
     },
 )
@@ -369,29 +359,80 @@
 
 class CreateGeofenceCollectionRequestRequestTypeDef(
     _RequiredCreateGeofenceCollectionRequestRequestTypeDef,
     _OptionalCreateGeofenceCollectionRequestRequestTypeDef,
 ):
     pass
 
-MapConfigurationTypeDef = TypedDict(
-    "MapConfigurationTypeDef",
+CreateGeofenceCollectionResponseTypeDef = TypedDict(
+    "CreateGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "CreateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateKeyResponseTypeDef = TypedDict(
+    "CreateKeyResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Key": str,
+        "KeyArn": str,
+        "KeyName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredMapConfigurationTypeDef = TypedDict(
+    "_RequiredMapConfigurationTypeDef",
     {
         "Style": str,
     },
 )
+_OptionalMapConfigurationTypeDef = TypedDict(
+    "_OptionalMapConfigurationTypeDef",
+    {
+        "PoliticalView": str,
+    },
+    total=False,
+)
+
+class MapConfigurationTypeDef(_RequiredMapConfigurationTypeDef, _OptionalMapConfigurationTypeDef):
+    pass
+
+CreateMapResponseTypeDef = TypedDict(
+    "CreateMapResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "MapArn": str,
+        "MapName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 DataSourceConfigurationTypeDef = TypedDict(
     "DataSourceConfigurationTypeDef",
     {
         "IntendedUse": IntendedUseType,
     },
     total=False,
 )
 
+CreatePlaceIndexResponseTypeDef = TypedDict(
+    "CreatePlaceIndexResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "IndexArn": str,
+        "IndexName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateRouteCalculatorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
         "DataSource": str,
     },
 )
@@ -407,14 +448,24 @@
 
 class CreateRouteCalculatorRequestRequestTypeDef(
     _RequiredCreateRouteCalculatorRequestRequestTypeDef,
     _OptionalCreateRouteCalculatorRequestRequestTypeDef,
 ):
     pass
 
+CreateRouteCalculatorResponseTypeDef = TypedDict(
+    "CreateRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "CreateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateTrackerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalCreateTrackerRequestRequestTypeDef = TypedDict(
@@ -431,14 +482,24 @@
 )
 
 class CreateTrackerRequestRequestTypeDef(
     _RequiredCreateTrackerRequestRequestTypeDef, _OptionalCreateTrackerRequestRequestTypeDef
 ):
     pass
 
+CreateTrackerResponseTypeDef = TypedDict(
+    "CreateTrackerResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "TrackerArn": str,
+        "TrackerName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteGeofenceCollectionRequestRequestTypeDef = TypedDict(
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 
@@ -480,14 +541,30 @@
 DescribeGeofenceCollectionRequestRequestTypeDef = TypedDict(
     "DescribeGeofenceCollectionRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 
+DescribeGeofenceCollectionResponseTypeDef = TypedDict(
+    "DescribeGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "CreateTime": datetime,
+        "Description": str,
+        "KmsKeyId": str,
+        "PricingPlan": PricingPlanType,
+        "PricingPlanDataSource": str,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeKeyRequestRequestTypeDef = TypedDict(
     "DescribeKeyRequestRequestTypeDef",
     {
         "KeyName": str,
     },
 )
 
@@ -508,21 +585,53 @@
 DescribeRouteCalculatorRequestRequestTypeDef = TypedDict(
     "DescribeRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
     },
 )
 
+DescribeRouteCalculatorResponseTypeDef = TypedDict(
+    "DescribeRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "CreateTime": datetime,
+        "DataSource": str,
+        "Description": str,
+        "PricingPlan": PricingPlanType,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeTrackerRequestRequestTypeDef = TypedDict(
     "DescribeTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 
+DescribeTrackerResponseTypeDef = TypedDict(
+    "DescribeTrackerResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Description": str,
+        "KmsKeyId": str,
+        "PositionFiltering": PositionFilteringType,
+        "PricingPlan": PricingPlanType,
+        "PricingPlanDataSource": str,
+        "Tags": Dict[str, str],
+        "TrackerArn": str,
+        "TrackerName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PositionalAccuracyTypeDef = TypedDict(
     "PositionalAccuracyTypeDef",
     {
         "Horizontal": float,
     },
 )
 
@@ -530,24 +639,37 @@
     "DisassociateTrackerConsumerRequestRequestTypeDef",
     {
         "ConsumerArn": str,
         "TrackerName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DeviceId": str,
+        "TrackerName": str,
+    },
+)
+_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
+    {
+        "EndTimeExclusive": Union[datetime, str],
+        "StartTimeInclusive": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(
+    _RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+    _OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+):
+    pass
+
 _RequiredGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetDevicePositionHistoryRequestRequestTypeDef",
     {
         "DeviceId": str,
         "TrackerName": str,
     },
 )
@@ -601,14 +723,24 @@
 )
 
 class GetMapGlyphsRequestRequestTypeDef(
     _RequiredGetMapGlyphsRequestRequestTypeDef, _OptionalGetMapGlyphsRequestRequestTypeDef
 ):
     pass
 
+GetMapGlyphsResponseTypeDef = TypedDict(
+    "GetMapGlyphsResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetMapSpritesRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapSpritesRequestRequestTypeDef",
     {
         "FileName": str,
         "MapName": str,
     },
 )
@@ -621,14 +753,24 @@
 )
 
 class GetMapSpritesRequestRequestTypeDef(
     _RequiredGetMapSpritesRequestRequestTypeDef, _OptionalGetMapSpritesRequestRequestTypeDef
 ):
     pass
 
+GetMapSpritesResponseTypeDef = TypedDict(
+    "GetMapSpritesResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetMapStyleDescriptorRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapStyleDescriptorRequestRequestTypeDef",
     {
         "MapName": str,
     },
 )
 _OptionalGetMapStyleDescriptorRequestRequestTypeDef = TypedDict(
@@ -641,14 +783,24 @@
 
 class GetMapStyleDescriptorRequestRequestTypeDef(
     _RequiredGetMapStyleDescriptorRequestRequestTypeDef,
     _OptionalGetMapStyleDescriptorRequestRequestTypeDef,
 ):
     pass
 
+GetMapStyleDescriptorResponseTypeDef = TypedDict(
+    "GetMapStyleDescriptorResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetMapTileRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapTileRequestRequestTypeDef",
     {
         "MapName": str,
         "X": str,
         "Y": str,
         "Z": str,
@@ -663,14 +815,24 @@
 )
 
 class GetMapTileRequestRequestTypeDef(
     _RequiredGetMapTileRequestRequestTypeDef, _OptionalGetMapTileRequestRequestTypeDef
 ):
     pass
 
+GetMapTileResponseTypeDef = TypedDict(
+    "GetMapTileResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetPlaceRequestRequestTypeDef = TypedDict(
     "_RequiredGetPlaceRequestRequestTypeDef",
     {
         "IndexName": str,
         "PlaceId": str,
     },
 )
@@ -711,14 +873,34 @@
     },
     total=False,
 )
 
 class StepTypeDef(_RequiredStepTypeDef, _OptionalStepTypeDef):
     pass
 
+_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
+    "_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    {
+        "TrackerName": str,
+    },
+)
+_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
+    "_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDevicePositionsRequestListDevicePositionsPaginateTypeDef(
+    _RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+    _OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDevicePositionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevicePositionsRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalListDevicePositionsRequestRequestTypeDef = TypedDict(
@@ -732,14 +914,22 @@
 
 class ListDevicePositionsRequestRequestTypeDef(
     _RequiredListDevicePositionsRequestRequestTypeDef,
     _OptionalListDevicePositionsRequestRequestTypeDef,
 ):
     pass
 
+ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef = TypedDict(
+    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGeofenceCollectionsRequestRequestTypeDef = TypedDict(
     "ListGeofenceCollectionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -765,14 +955,34 @@
 
 class ListGeofenceCollectionsResponseEntryTypeDef(
     _RequiredListGeofenceCollectionsResponseEntryTypeDef,
     _OptionalListGeofenceCollectionsResponseEntryTypeDef,
 ):
     pass
 
+_RequiredListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
+    "_RequiredListGeofencesRequestListGeofencesPaginateTypeDef",
+    {
+        "CollectionName": str,
+    },
+)
+_OptionalListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
+    "_OptionalListGeofencesRequestListGeofencesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListGeofencesRequestListGeofencesPaginateTypeDef(
+    _RequiredListGeofencesRequestListGeofencesPaginateTypeDef,
+    _OptionalListGeofencesRequestListGeofencesPaginateTypeDef,
+):
+    pass
+
 _RequiredListGeofencesRequestRequestTypeDef = TypedDict(
     "_RequiredListGeofencesRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 _OptionalListGeofencesRequestRequestTypeDef = TypedDict(
@@ -785,14 +995,22 @@
 )
 
 class ListGeofencesRequestRequestTypeDef(
     _RequiredListGeofencesRequestRequestTypeDef, _OptionalListGeofencesRequestRequestTypeDef
 ):
     pass
 
+ListMapsRequestListMapsPaginateTypeDef = TypedDict(
+    "ListMapsRequestListMapsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMapsRequestRequestTypeDef = TypedDict(
     "ListMapsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -817,14 +1035,22 @@
 )
 
 class ListMapsResponseEntryTypeDef(
     _RequiredListMapsResponseEntryTypeDef, _OptionalListMapsResponseEntryTypeDef
 ):
     pass
 
+ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef = TypedDict(
+    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPlaceIndexesRequestRequestTypeDef = TypedDict(
     "ListPlaceIndexesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -849,14 +1075,22 @@
 )
 
 class ListPlaceIndexesResponseEntryTypeDef(
     _RequiredListPlaceIndexesResponseEntryTypeDef, _OptionalListPlaceIndexesResponseEntryTypeDef
 ):
     pass
 
+ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef = TypedDict(
+    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRouteCalculatorsRequestRequestTypeDef = TypedDict(
     "ListRouteCalculatorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -889,14 +1123,42 @@
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
+_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
+    "_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    {
+        "TrackerName": str,
+    },
+)
+_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
+    "_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef(
+    _RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+    _OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+):
+    pass
+
 _RequiredListTrackerConsumersRequestRequestTypeDef = TypedDict(
     "_RequiredListTrackerConsumersRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalListTrackerConsumersRequestRequestTypeDef = TypedDict(
@@ -910,14 +1172,31 @@
 
 class ListTrackerConsumersRequestRequestTypeDef(
     _RequiredListTrackerConsumersRequestRequestTypeDef,
     _OptionalListTrackerConsumersRequestRequestTypeDef,
 ):
     pass
 
+ListTrackerConsumersResponseTypeDef = TypedDict(
+    "ListTrackerConsumersResponseTypeDef",
+    {
+        "ConsumerArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTrackersRequestListTrackersPaginateTypeDef = TypedDict(
+    "ListTrackersRequestListTrackersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTrackersRequestRequestTypeDef = TypedDict(
     "ListTrackersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -942,14 +1221,32 @@
 )
 
 class ListTrackersResponseEntryTypeDef(
     _RequiredListTrackersResponseEntryTypeDef, _OptionalListTrackersResponseEntryTypeDef
 ):
     pass
 
+MapConfigurationUpdateTypeDef = TypedDict(
+    "MapConfigurationUpdateTypeDef",
+    {
+        "PoliticalView": str,
+    },
+    total=False,
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
 PlaceGeometryTypeDef = TypedDict(
     "PlaceGeometryTypeDef",
     {
         "Point": List[float],
     },
     total=False,
 )
@@ -967,14 +1264,35 @@
     },
     total=False,
 )
 
 class TimeZoneTypeDef(_RequiredTimeZoneTypeDef, _OptionalTimeZoneTypeDef):
     pass
 
+PutGeofenceResponseTypeDef = TypedDict(
+    "PutGeofenceResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "GeofenceId": str,
+        "UpdateTime": datetime,
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
 _RequiredRouteMatrixEntryErrorTypeDef = TypedDict(
     "_RequiredRouteMatrixEntryErrorTypeDef",
     {
         "Code": RouteMatrixErrorCodeType,
     },
 )
 _OptionalRouteMatrixEntryErrorTypeDef = TypedDict(
@@ -995,15 +1313,17 @@
     {
         "Text": str,
     },
 )
 _OptionalSearchForSuggestionsResultTypeDef = TypedDict(
     "_OptionalSearchForSuggestionsResultTypeDef",
     {
+        "Categories": List[str],
         "PlaceId": str,
+        "SupplementalCategories": List[str],
     },
     total=False,
 )
 
 class SearchForSuggestionsResultTypeDef(
     _RequiredSearchForSuggestionsResultTypeDef, _OptionalSearchForSuggestionsResultTypeDef
 ):
@@ -1061,14 +1381,15 @@
     },
 )
 _OptionalSearchPlaceIndexForSuggestionsRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForSuggestionsRequestRequestTypeDef",
     {
         "BiasPosition": Sequence[float],
         "FilterBBox": Sequence[float],
+        "FilterCategories": Sequence[str],
         "FilterCountries": Sequence[str],
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
@@ -1086,14 +1407,15 @@
     },
 )
 _OptionalSearchPlaceIndexForSuggestionsSummaryTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForSuggestionsSummaryTypeDef",
     {
         "BiasPosition": List[float],
         "FilterBBox": List[float],
+        "FilterCategories": List[str],
         "FilterCountries": List[str],
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
@@ -1111,14 +1433,15 @@
     },
 )
 _OptionalSearchPlaceIndexForTextRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForTextRequestRequestTypeDef",
     {
         "BiasPosition": Sequence[float],
         "FilterBBox": Sequence[float],
+        "FilterCategories": Sequence[str],
         "FilterCountries": Sequence[str],
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
@@ -1136,14 +1459,15 @@
     },
 )
 _OptionalSearchPlaceIndexForTextSummaryTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForTextSummaryTypeDef",
     {
         "BiasPosition": List[float],
         "FilterBBox": List[float],
+        "FilterCategories": List[str],
         "FilterCountries": List[str],
         "Language": str,
         "MaxResults": int,
         "ResultBBox": List[float],
     },
     total=False,
 )
@@ -1187,33 +1511,53 @@
 
 class UpdateGeofenceCollectionRequestRequestTypeDef(
     _RequiredUpdateGeofenceCollectionRequestRequestTypeDef,
     _OptionalUpdateGeofenceCollectionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredUpdateMapRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMapRequestRequestTypeDef",
+UpdateGeofenceCollectionResponseTypeDef = TypedDict(
+    "UpdateGeofenceCollectionResponseTypeDef",
     {
-        "MapName": str,
+        "CollectionArn": str,
+        "CollectionName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalUpdateMapRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMapRequestRequestTypeDef",
+
+UpdateKeyResponseTypeDef = TypedDict(
+    "UpdateKeyResponseTypeDef",
     {
-        "Description": str,
-        "PricingPlan": PricingPlanType,
+        "KeyArn": str,
+        "KeyName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class UpdateMapRequestRequestTypeDef(
-    _RequiredUpdateMapRequestRequestTypeDef, _OptionalUpdateMapRequestRequestTypeDef
-):
-    pass
+UpdateMapResponseTypeDef = TypedDict(
+    "UpdateMapResponseTypeDef",
+    {
+        "MapArn": str,
+        "MapName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdatePlaceIndexResponseTypeDef = TypedDict(
+    "UpdatePlaceIndexResponseTypeDef",
+    {
+        "IndexArn": str,
+        "IndexName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredUpdateRouteCalculatorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
     },
 )
@@ -1228,14 +1572,24 @@
 
 class UpdateRouteCalculatorRequestRequestTypeDef(
     _RequiredUpdateRouteCalculatorRequestRequestTypeDef,
     _OptionalUpdateRouteCalculatorRequestRequestTypeDef,
 ):
     pass
 
+UpdateRouteCalculatorResponseTypeDef = TypedDict(
+    "UpdateRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateTrackerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalUpdateTrackerRequestRequestTypeDef = TypedDict(
@@ -1250,14 +1604,33 @@
 )
 
 class UpdateTrackerRequestRequestTypeDef(
     _RequiredUpdateTrackerRequestRequestTypeDef, _OptionalUpdateTrackerRequestRequestTypeDef
 ):
     pass
 
+UpdateTrackerResponseTypeDef = TypedDict(
+    "UpdateTrackerResponseTypeDef",
+    {
+        "TrackerArn": str,
+        "TrackerName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListKeysRequestListKeysPaginateTypeDef = TypedDict(
+    "ListKeysRequestListKeysPaginateTypeDef",
+    {
+        "Filter": ApiKeyFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListKeysRequestRequestTypeDef = TypedDict(
     "ListKeysRequestRequestTypeDef",
     {
         "Filter": ApiKeyFilterTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -1283,14 +1656,30 @@
 )
 
 class CreateKeyRequestRequestTypeDef(
     _RequiredCreateKeyRequestRequestTypeDef, _OptionalCreateKeyRequestRequestTypeDef
 ):
     pass
 
+DescribeKeyResponseTypeDef = TypedDict(
+    "DescribeKeyResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Description": str,
+        "ExpireTime": datetime,
+        "Key": str,
+        "KeyArn": str,
+        "KeyName": str,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListKeysResponseEntryTypeDef = TypedDict(
     "_RequiredListKeysResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "ExpireTime": datetime,
         "KeyName": str,
         "Restrictions": ApiKeyRestrictionsTypeDef,
@@ -1379,266 +1768,14 @@
     {
         "DeviceId": str,
         "Error": BatchItemErrorTypeDef,
         "SampleTime": datetime,
     },
 )
 
-CreateGeofenceCollectionResponseTypeDef = TypedDict(
-    "CreateGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "CreateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateKeyResponseTypeDef = TypedDict(
-    "CreateKeyResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Key": str,
-        "KeyArn": str,
-        "KeyName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMapResponseTypeDef = TypedDict(
-    "CreateMapResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "MapArn": str,
-        "MapName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePlaceIndexResponseTypeDef = TypedDict(
-    "CreatePlaceIndexResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "IndexArn": str,
-        "IndexName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRouteCalculatorResponseTypeDef = TypedDict(
-    "CreateRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "CreateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTrackerResponseTypeDef = TypedDict(
-    "CreateTrackerResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "TrackerArn": str,
-        "TrackerName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeGeofenceCollectionResponseTypeDef = TypedDict(
-    "DescribeGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "CreateTime": datetime,
-        "Description": str,
-        "KmsKeyId": str,
-        "PricingPlan": PricingPlanType,
-        "PricingPlanDataSource": str,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeKeyResponseTypeDef = TypedDict(
-    "DescribeKeyResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Description": str,
-        "ExpireTime": datetime,
-        "Key": str,
-        "KeyArn": str,
-        "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRouteCalculatorResponseTypeDef = TypedDict(
-    "DescribeRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "CreateTime": datetime,
-        "DataSource": str,
-        "Description": str,
-        "PricingPlan": PricingPlanType,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeTrackerResponseTypeDef = TypedDict(
-    "DescribeTrackerResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Description": str,
-        "KmsKeyId": str,
-        "PositionFiltering": PositionFilteringType,
-        "PricingPlan": PricingPlanType,
-        "PricingPlanDataSource": str,
-        "Tags": Dict[str, str],
-        "TrackerArn": str,
-        "TrackerName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMapGlyphsResponseTypeDef = TypedDict(
-    "GetMapGlyphsResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMapSpritesResponseTypeDef = TypedDict(
-    "GetMapSpritesResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMapStyleDescriptorResponseTypeDef = TypedDict(
-    "GetMapStyleDescriptorResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMapTileResponseTypeDef = TypedDict(
-    "GetMapTileResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
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
-ListTrackerConsumersResponseTypeDef = TypedDict(
-    "ListTrackerConsumersResponseTypeDef",
-    {
-        "ConsumerArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutGeofenceResponseTypeDef = TypedDict(
-    "PutGeofenceResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "GeofenceId": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGeofenceCollectionResponseTypeDef = TypedDict(
-    "UpdateGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateKeyResponseTypeDef = TypedDict(
-    "UpdateKeyResponseTypeDef",
-    {
-        "KeyArn": str,
-        "KeyName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMapResponseTypeDef = TypedDict(
-    "UpdateMapResponseTypeDef",
-    {
-        "MapArn": str,
-        "MapName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePlaceIndexResponseTypeDef = TypedDict(
-    "UpdatePlaceIndexResponseTypeDef",
-    {
-        "IndexArn": str,
-        "IndexName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateRouteCalculatorResponseTypeDef = TypedDict(
-    "UpdateRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTrackerResponseTypeDef = TypedDict(
-    "UpdateTrackerResponseTypeDef",
-    {
-        "TrackerArn": str,
-        "TrackerName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CalculateRouteTruckModeOptionsTypeDef = TypedDict(
     "CalculateRouteTruckModeOptionsTypeDef",
     {
         "AvoidFerries": bool,
         "AvoidTolls": bool,
         "Dimensions": TruckDimensionsTypeDef,
         "Weight": TruckWeightTypeDef,
@@ -1685,15 +1822,15 @@
         "DataSource": str,
         "Description": str,
         "MapArn": str,
         "MapName": str,
         "PricingPlan": PricingPlanType,
         "Tags": Dict[str, str],
         "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePlaceIndexRequestRequestTypeDef",
     {
         "DataSource": str,
@@ -1724,15 +1861,15 @@
         "DataSourceConfiguration": DataSourceConfigurationTypeDef,
         "Description": str,
         "IndexArn": str,
         "IndexName": str,
         "PricingPlan": PricingPlanType,
         "Tags": Dict[str, str],
         "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePlaceIndexRequestRequestTypeDef",
     {
         "IndexName": str,
@@ -1801,15 +1938,15 @@
     {
         "Accuracy": PositionalAccuracyTypeDef,
         "DeviceId": str,
         "Position": List[float],
         "PositionProperties": Dict[str, str],
         "ReceivedTime": datetime,
         "SampleTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListDevicePositionsResponseEntryTypeDef = TypedDict(
     "_RequiredListDevicePositionsResponseEntryTypeDef",
     {
         "DeviceId": str,
@@ -1828,146 +1965,14 @@
 
 class ListDevicePositionsResponseEntryTypeDef(
     _RequiredListDevicePositionsResponseEntryTypeDef,
     _OptionalListDevicePositionsResponseEntryTypeDef,
 ):
     pass
 
-_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
-    {
-        "DeviceId": str,
-        "TrackerName": str,
-    },
-)
-_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
-    {
-        "EndTimeExclusive": Union[datetime, str],
-        "StartTimeInclusive": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(
-    _RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-    _OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-):
-    pass
-
-_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
-    "_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
-    {
-        "TrackerName": str,
-    },
-)
-_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
-    "_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDevicePositionsRequestListDevicePositionsPaginateTypeDef(
-    _RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
-    _OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
-):
-    pass
-
-ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef = TypedDict(
-    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
-    "_RequiredListGeofencesRequestListGeofencesPaginateTypeDef",
-    {
-        "CollectionName": str,
-    },
-)
-_OptionalListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
-    "_OptionalListGeofencesRequestListGeofencesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListGeofencesRequestListGeofencesPaginateTypeDef(
-    _RequiredListGeofencesRequestListGeofencesPaginateTypeDef,
-    _OptionalListGeofencesRequestListGeofencesPaginateTypeDef,
-):
-    pass
-
-ListKeysRequestListKeysPaginateTypeDef = TypedDict(
-    "ListKeysRequestListKeysPaginateTypeDef",
-    {
-        "Filter": ApiKeyFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListMapsRequestListMapsPaginateTypeDef = TypedDict(
-    "ListMapsRequestListMapsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef = TypedDict(
-    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef = TypedDict(
-    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
-    "_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
-    {
-        "TrackerName": str,
-    },
-)
-_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
-    "_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef(
-    _RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
-    _OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
-):
-    pass
-
-ListTrackersRequestListTrackersPaginateTypeDef = TypedDict(
-    "ListTrackersRequestListTrackersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredLegTypeDef = TypedDict(
     "_RequiredLegTypeDef",
     {
         "Distance": float,
         "DurationSeconds": float,
         "EndPosition": List[float],
         "StartPosition": List[float],
@@ -1986,73 +1991,96 @@
     pass
 
 ListGeofenceCollectionsResponseTypeDef = TypedDict(
     "ListGeofenceCollectionsResponseTypeDef",
     {
         "Entries": List[ListGeofenceCollectionsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMapsResponseTypeDef = TypedDict(
     "ListMapsResponseTypeDef",
     {
         "Entries": List[ListMapsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPlaceIndexesResponseTypeDef = TypedDict(
     "ListPlaceIndexesResponseTypeDef",
     {
         "Entries": List[ListPlaceIndexesResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRouteCalculatorsResponseTypeDef = TypedDict(
     "ListRouteCalculatorsResponseTypeDef",
     {
         "Entries": List[ListRouteCalculatorsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrackersResponseTypeDef = TypedDict(
     "ListTrackersResponseTypeDef",
     {
         "Entries": List[ListTrackersResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredUpdateMapRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMapRequestRequestTypeDef",
+    {
+        "MapName": str,
+    },
+)
+_OptionalUpdateMapRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMapRequestRequestTypeDef",
+    {
+        "ConfigurationUpdate": MapConfigurationUpdateTypeDef,
+        "Description": str,
+        "PricingPlan": PricingPlanType,
+    },
+    total=False,
+)
+
+class UpdateMapRequestRequestTypeDef(
+    _RequiredUpdateMapRequestRequestTypeDef, _OptionalUpdateMapRequestRequestTypeDef
+):
+    pass
+
 _RequiredPlaceTypeDef = TypedDict(
     "_RequiredPlaceTypeDef",
     {
         "Geometry": PlaceGeometryTypeDef,
     },
 )
 _OptionalPlaceTypeDef = TypedDict(
     "_OptionalPlaceTypeDef",
     {
         "AddressNumber": str,
+        "Categories": List[str],
         "Country": str,
         "Interpolated": bool,
         "Label": str,
         "Municipality": str,
         "Neighborhood": str,
         "PostalCode": str,
         "Region": str,
         "Street": str,
         "SubRegion": str,
+        "SupplementalCategories": List[str],
         "TimeZone": TimeZoneTypeDef,
         "UnitNumber": str,
         "UnitType": str,
     },
     total=False,
 )
 
@@ -2070,65 +2098,65 @@
 )
 
 SearchPlaceIndexForSuggestionsResponseTypeDef = TypedDict(
     "SearchPlaceIndexForSuggestionsResponseTypeDef",
     {
         "Results": List[SearchForSuggestionsResultTypeDef],
         "Summary": SearchPlaceIndexForSuggestionsSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKeysResponseTypeDef = TypedDict(
     "ListKeysResponseTypeDef",
     {
         "Entries": List[ListKeysResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteDevicePositionHistoryResponseTypeDef = TypedDict(
     "BatchDeleteDevicePositionHistoryResponseTypeDef",
     {
         "Errors": List[BatchDeleteDevicePositionHistoryErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteGeofenceResponseTypeDef = TypedDict(
     "BatchDeleteGeofenceResponseTypeDef",
     {
         "Errors": List[BatchDeleteGeofenceErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchEvaluateGeofencesResponseTypeDef = TypedDict(
     "BatchEvaluateGeofencesResponseTypeDef",
     {
         "Errors": List[BatchEvaluateGeofencesErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutGeofenceResponseTypeDef = TypedDict(
     "BatchPutGeofenceResponseTypeDef",
     {
         "Errors": List[BatchPutGeofenceErrorTypeDef],
         "Successes": List[BatchPutGeofenceSuccessTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdateDevicePositionResponseTypeDef = TypedDict(
     "BatchUpdateDevicePositionResponseTypeDef",
     {
         "Errors": List[BatchUpdateDevicePositionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCalculateRouteMatrixRequestRequestTypeDef = TypedDict(
     "_RequiredCalculateRouteMatrixRequestRequestTypeDef",
     {
         "CalculatorName": str,
@@ -2179,69 +2207,106 @@
 )
 
 class CalculateRouteRequestRequestTypeDef(
     _RequiredCalculateRouteRequestRequestTypeDef, _OptionalCalculateRouteRequestRequestTypeDef
 ):
     pass
 
-BatchPutGeofenceRequestEntryTypeDef = TypedDict(
-    "BatchPutGeofenceRequestEntryTypeDef",
+_RequiredBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_RequiredBatchPutGeofenceRequestEntryTypeDef",
     {
         "GeofenceId": str,
         "Geometry": GeofenceGeometryTypeDef,
     },
 )
+_OptionalBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_OptionalBatchPutGeofenceRequestEntryTypeDef",
+    {
+        "GeofenceProperties": Mapping[str, str],
+    },
+    total=False,
+)
+
+class BatchPutGeofenceRequestEntryTypeDef(
+    _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
+):
+    pass
 
 GetGeofenceResponseTypeDef = TypedDict(
     "GetGeofenceResponseTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
+        "GeofenceProperties": Dict[str, str],
         "Geometry": GeofenceGeometryTypeDef,
         "Status": str,
         "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListGeofenceResponseEntryTypeDef = TypedDict(
-    "ListGeofenceResponseEntryTypeDef",
+_RequiredListGeofenceResponseEntryTypeDef = TypedDict(
+    "_RequiredListGeofenceResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
         "Geometry": GeofenceGeometryTypeDef,
         "Status": str,
         "UpdateTime": datetime,
     },
 )
+_OptionalListGeofenceResponseEntryTypeDef = TypedDict(
+    "_OptionalListGeofenceResponseEntryTypeDef",
+    {
+        "GeofenceProperties": Dict[str, str],
+    },
+    total=False,
+)
 
-PutGeofenceRequestRequestTypeDef = TypedDict(
-    "PutGeofenceRequestRequestTypeDef",
+class ListGeofenceResponseEntryTypeDef(
+    _RequiredListGeofenceResponseEntryTypeDef, _OptionalListGeofenceResponseEntryTypeDef
+):
+    pass
+
+_RequiredPutGeofenceRequestRequestTypeDef = TypedDict(
+    "_RequiredPutGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceId": str,
         "Geometry": GeofenceGeometryTypeDef,
     },
 )
+_OptionalPutGeofenceRequestRequestTypeDef = TypedDict(
+    "_OptionalPutGeofenceRequestRequestTypeDef",
+    {
+        "GeofenceProperties": Mapping[str, str],
+    },
+    total=False,
+)
+
+class PutGeofenceRequestRequestTypeDef(
+    _RequiredPutGeofenceRequestRequestTypeDef, _OptionalPutGeofenceRequestRequestTypeDef
+):
+    pass
 
 BatchGetDevicePositionResponseTypeDef = TypedDict(
     "BatchGetDevicePositionResponseTypeDef",
     {
         "DevicePositions": List[DevicePositionTypeDef],
         "Errors": List[BatchGetDevicePositionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDevicePositionHistoryResponseTypeDef = TypedDict(
     "GetDevicePositionHistoryResponseTypeDef",
     {
         "DevicePositions": List[DevicePositionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchEvaluateGeofencesRequestRequestTypeDef = TypedDict(
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     {
         "CollectionName": str,
@@ -2258,32 +2323,32 @@
 )
 
 ListDevicePositionsResponseTypeDef = TypedDict(
     "ListDevicePositionsResponseTypeDef",
     {
         "Entries": List[ListDevicePositionsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CalculateRouteResponseTypeDef = TypedDict(
     "CalculateRouteResponseTypeDef",
     {
         "Legs": List[LegTypeDef],
         "Summary": CalculateRouteSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPlaceResponseTypeDef = TypedDict(
     "GetPlaceResponseTypeDef",
     {
         "Place": PlaceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchForPositionResultTypeDef = TypedDict(
     "_RequiredSearchForPositionResultTypeDef",
     {
         "Distance": float,
@@ -2327,15 +2392,15 @@
 CalculateRouteMatrixResponseTypeDef = TypedDict(
     "CalculateRouteMatrixResponseTypeDef",
     {
         "RouteMatrix": List[List[RouteMatrixEntryTypeDef]],
         "SnappedDeparturePositions": List[List[float]],
         "SnappedDestinationPositions": List[List[float]],
         "Summary": CalculateRouteMatrixSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutGeofenceRequestRequestTypeDef = TypedDict(
     "BatchPutGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
@@ -2344,28 +2409,28 @@
 )
 
 ListGeofencesResponseTypeDef = TypedDict(
     "ListGeofencesResponseTypeDef",
     {
         "Entries": List[ListGeofenceResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchPlaceIndexForPositionResponseTypeDef = TypedDict(
     "SearchPlaceIndexForPositionResponseTypeDef",
     {
         "Results": List[SearchForPositionResultTypeDef],
         "Summary": SearchPlaceIndexForPositionSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchPlaceIndexForTextResponseTypeDef = TypedDict(
     "SearchPlaceIndexForTextResponseTypeDef",
     {
         "Results": List[SearchForTextResultTypeDef],
         "Summary": SearchPlaceIndexForTextSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/PKG-INFO` & `mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-location
-Version: 1.26.86
-Summary: Type annotations for boto3.LocationService 1.26.86 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.LocationService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-location"></a>
 
 # mypy-boto3-location
 
 [![PyPI - mypy-boto3-location](https://img.shields.io/pypi/v/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-location?color=blue)](https://pypistats.org/packages/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.26.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
 See how it helps to find and fix potential bugs:
 
@@ -372,144 +372,145 @@
 ```python
 from mypy_boto3_location.type_defs import (
     ApiKeyFilterTypeDef,
     ApiKeyRestrictionsTypeDef,
     AssociateTrackerConsumerRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDeleteDevicePositionHistoryRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     BatchDeleteGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionRequestRequestTypeDef,
     BatchPutGeofenceSuccessTypeDef,
     CalculateRouteCarModeOptionsTypeDef,
     CalculateRouteMatrixSummaryTypeDef,
     CalculateRouteSummaryTypeDef,
     TruckDimensionsTypeDef,
     TruckWeightTypeDef,
     CircleTypeDef,
     CreateGeofenceCollectionRequestRequestTypeDef,
+    CreateGeofenceCollectionResponseTypeDef,
+    CreateKeyResponseTypeDef,
     MapConfigurationTypeDef,
+    CreateMapResponseTypeDef,
     DataSourceConfigurationTypeDef,
+    CreatePlaceIndexResponseTypeDef,
     CreateRouteCalculatorRequestRequestTypeDef,
+    CreateRouteCalculatorResponseTypeDef,
     CreateTrackerRequestRequestTypeDef,
+    CreateTrackerResponseTypeDef,
     DeleteGeofenceCollectionRequestRequestTypeDef,
     DeleteKeyRequestRequestTypeDef,
     DeleteMapRequestRequestTypeDef,
     DeletePlaceIndexRequestRequestTypeDef,
     DeleteRouteCalculatorRequestRequestTypeDef,
     DeleteTrackerRequestRequestTypeDef,
     DescribeGeofenceCollectionRequestRequestTypeDef,
+    DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DescribeMapRequestRequestTypeDef,
     DescribePlaceIndexRequestRequestTypeDef,
     DescribeRouteCalculatorRequestRequestTypeDef,
+    DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerRequestRequestTypeDef,
+    DescribeTrackerResponseTypeDef,
     PositionalAccuracyTypeDef,
     DisassociateTrackerConsumerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
     GetDevicePositionHistoryRequestRequestTypeDef,
     GetDevicePositionRequestRequestTypeDef,
     GetGeofenceRequestRequestTypeDef,
     GetMapGlyphsRequestRequestTypeDef,
+    GetMapGlyphsResponseTypeDef,
     GetMapSpritesRequestRequestTypeDef,
+    GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorRequestRequestTypeDef,
+    GetMapStyleDescriptorResponseTypeDef,
     GetMapTileRequestRequestTypeDef,
+    GetMapTileResponseTypeDef,
     GetPlaceRequestRequestTypeDef,
     LegGeometryTypeDef,
     StepTypeDef,
+    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
     ListDevicePositionsRequestRequestTypeDef,
+    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
     ListGeofenceCollectionsRequestRequestTypeDef,
     ListGeofenceCollectionsResponseEntryTypeDef,
+    ListGeofencesRequestListGeofencesPaginateTypeDef,
     ListGeofencesRequestRequestTypeDef,
+    ListMapsRequestListMapsPaginateTypeDef,
     ListMapsRequestRequestTypeDef,
     ListMapsResponseEntryTypeDef,
+    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
     ListPlaceIndexesRequestRequestTypeDef,
     ListPlaceIndexesResponseEntryTypeDef,
+    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
     ListRouteCalculatorsRequestRequestTypeDef,
     ListRouteCalculatorsResponseEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
     ListTrackerConsumersRequestRequestTypeDef,
+    ListTrackerConsumersResponseTypeDef,
+    ListTrackersRequestListTrackersPaginateTypeDef,
     ListTrackersRequestRequestTypeDef,
     ListTrackersResponseEntryTypeDef,
+    MapConfigurationUpdateTypeDef,
+    PaginatorConfigTypeDef,
     PlaceGeometryTypeDef,
     TimeZoneTypeDef,
+    PutGeofenceResponseTypeDef,
+    ResponseMetadataTypeDef,
     RouteMatrixEntryErrorTypeDef,
     SearchForSuggestionsResultTypeDef,
     SearchPlaceIndexForPositionRequestRequestTypeDef,
     SearchPlaceIndexForPositionSummaryTypeDef,
     SearchPlaceIndexForSuggestionsRequestRequestTypeDef,
     SearchPlaceIndexForSuggestionsSummaryTypeDef,
     SearchPlaceIndexForTextRequestRequestTypeDef,
     SearchPlaceIndexForTextSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGeofenceCollectionRequestRequestTypeDef,
-    UpdateMapRequestRequestTypeDef,
+    UpdateGeofenceCollectionResponseTypeDef,
+    UpdateKeyResponseTypeDef,
+    UpdateMapResponseTypeDef,
+    UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorRequestRequestTypeDef,
+    UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerRequestRequestTypeDef,
+    UpdateTrackerResponseTypeDef,
+    ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
     CreateKeyRequestRequestTypeDef,
+    DescribeKeyResponseTypeDef,
     ListKeysResponseEntryTypeDef,
     UpdateKeyRequestRequestTypeDef,
     BatchDeleteDevicePositionHistoryErrorTypeDef,
     BatchDeleteGeofenceErrorTypeDef,
     BatchEvaluateGeofencesErrorTypeDef,
     BatchGetDevicePositionErrorTypeDef,
     BatchPutGeofenceErrorTypeDef,
     BatchUpdateDevicePositionErrorTypeDef,
-    CreateGeofenceCollectionResponseTypeDef,
-    CreateKeyResponseTypeDef,
-    CreateMapResponseTypeDef,
-    CreatePlaceIndexResponseTypeDef,
-    CreateRouteCalculatorResponseTypeDef,
-    CreateTrackerResponseTypeDef,
-    DescribeGeofenceCollectionResponseTypeDef,
-    DescribeKeyResponseTypeDef,
-    DescribeRouteCalculatorResponseTypeDef,
-    DescribeTrackerResponseTypeDef,
-    GetMapGlyphsResponseTypeDef,
-    GetMapSpritesResponseTypeDef,
-    GetMapStyleDescriptorResponseTypeDef,
-    GetMapTileResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTrackerConsumersResponseTypeDef,
-    PutGeofenceResponseTypeDef,
-    UpdateGeofenceCollectionResponseTypeDef,
-    UpdateKeyResponseTypeDef,
-    UpdateMapResponseTypeDef,
-    UpdatePlaceIndexResponseTypeDef,
-    UpdateRouteCalculatorResponseTypeDef,
-    UpdateTrackerResponseTypeDef,
     CalculateRouteTruckModeOptionsTypeDef,
     GeofenceGeometryTypeDef,
     CreateMapRequestRequestTypeDef,
     DescribeMapResponseTypeDef,
     CreatePlaceIndexRequestRequestTypeDef,
     DescribePlaceIndexResponseTypeDef,
     UpdatePlaceIndexRequestRequestTypeDef,
     DevicePositionTypeDef,
     DevicePositionUpdateTypeDef,
     GetDevicePositionResponseTypeDef,
     ListDevicePositionsResponseEntryTypeDef,
-    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
-    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
-    ListGeofencesRequestListGeofencesPaginateTypeDef,
-    ListKeysRequestListKeysPaginateTypeDef,
-    ListMapsRequestListMapsPaginateTypeDef,
-    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
-    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
-    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
-    ListTrackersRequestListTrackersPaginateTypeDef,
     LegTypeDef,
     ListGeofenceCollectionsResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackersResponseTypeDef,
+    UpdateMapRequestRequestTypeDef,
     PlaceTypeDef,
     RouteMatrixEntryTypeDef,
     SearchPlaceIndexForSuggestionsResponseTypeDef,
     ListKeysResponseTypeDef,
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
@@ -545,42 +546,42 @@
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

### Comparing `mypy-boto3-location-1.26.86/mypy_boto3_location.egg-info/SOURCES.txt` & `mypy-boto3-location-1.27.0/mypy_boto3_location.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.26.86/setup.py` & `mypy-boto3-location-1.27.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-location.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-location",
-    version="1.26.86",
+    version="1.27.0",
     packages=["mypy_boto3_location"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LocationService 1.26.86 service generated with"
-        " mypy-boto3-builder 7.12.5"
+        "Type annotations for boto3.LocationService 1.27.0 service generated with"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/",
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


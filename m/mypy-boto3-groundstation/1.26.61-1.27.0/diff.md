# Comparing `tmp/mypy-boto3-groundstation-1.26.61.tar.gz` & `tmp/mypy-boto3-groundstation-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-groundstation-1.26.61.tar", last modified: Tue Jan 31 20:49:56 2023, max compression
+gzip compressed data, was "mypy-boto3-groundstation-1.27.0.tar", last modified: Mon Jul  3 19:50:50 2023, max compression
```

## Comparing `mypy-boto3-groundstation-1.26.61.tar` & `mypy-boto3-groundstation-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:56.862166 mypy-boto3-groundstation-1.26.61/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-01-31 20:49:56.858166 mypy-boto3-groundstation-1.26.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:56.850166 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26979 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26931 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39742 2023-01-31 20:48:31.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39695 2023-01-31 20:48:31.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-01-31 20:48:30.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:56.858166 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-01-31 20:49:56.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-01-31 20:49:56.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:56.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:56.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 20:49:56.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 20:49:56.000000 mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 20:49:56.862166 mypy-boto3-groundstation-1.26.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-01-31 20:48:28.000000 mypy-boto3-groundstation-1.26.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.171351 mypy-boto3-groundstation-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:38:42.000000 mypy-boto3-groundstation-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19266 2023-07-03 19:50:50.163350 mypy-boto3-groundstation-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-07-03 19:38:42.000000 mypy-boto3-groundstation-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.163350 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-03 19:38:43.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-03 19:38:42.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 19:38:43.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26848 2023-07-03 19:38:43.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26800 2023-07-03 19:38:43.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-03 19:38:43.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-07-03 19:38:43.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-03 19:38:43.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-07-03 19:38:43.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:38:43.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40185 2023-07-03 19:38:44.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40136 2023-07-03 19:38:43.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:38:42.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-03 19:38:43.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-03 19:38:43.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.163350 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19266 2023-07-03 19:50:50.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-03 19:50:50.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:50.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:50.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:50.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 19:50:50.000000 mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:50.171351 mypy-boto3-groundstation-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-03 19:38:42.000000 mypy-boto3-groundstation-1.27.0/setup.py
```

### Comparing `mypy-boto3-groundstation-1.26.61/LICENSE` & `mypy-boto3-groundstation-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-groundstation-1.26.61/PKG-INFO` & `mypy-boto3-groundstation-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-groundstation
-Version: 1.26.61
-Summary: Type annotations for boto3.GroundStation 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.GroundStation 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-groundstation"></a>
 
 # mypy-boto3-groundstation
 
 [![PyPI - mypy-boto3-groundstation](https://img.shields.io/pypi/v/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-groundstation?color=blue)](https://pypistats.org/packages/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
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
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,15 +342,16 @@
 
 ```python
 from mypy_boto3_groundstation.literals import (
     AgentStatusType,
     AngleUnitsType,
     AuditResultsType,
     BandwidthUnitsType,
-    ComponentTypeType,
+    CapabilityHealthReasonType,
+    CapabilityHealthType,
     ConfigCapabilityTypeType,
     ContactScheduledWaiterName,
     ContactStatusType,
     CriticalityType,
     EirpUnitsType,
     EndpointStatusType,
     EphemerisInvalidReasonType,
@@ -392,72 +393,79 @@
     AntennaDemodDecodeDetailsTypeDef,
     DecodeConfigTypeDef,
     DemodulationConfigTypeDef,
     EirpTypeDef,
     CancelContactRequestRequestTypeDef,
     ComponentStatusDataTypeDef,
     S3RecordingDetailsTypeDef,
-    ResponseMetadataTypeDef,
+    ConfigIdResponseTypeDef,
     ConfigListItemTypeDef,
     DataflowEndpointConfigTypeDef,
     S3RecordingConfigTypeDef,
     TrackingConfigTypeDef,
     UplinkEchoConfigTypeDef,
     SocketAddressTypeDef,
     ElevationTypeDef,
+    ContactIdResponseTypeDef,
     KmsKeyTypeDef,
+    DataflowEndpointGroupIdResponseTypeDef,
     DataflowEndpointListItemTypeDef,
     DeleteConfigRequestRequestTypeDef,
     DeleteDataflowEndpointGroupRequestRequestTypeDef,
     DeleteEphemerisRequestRequestTypeDef,
     DeleteMissionProfileRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeContactRequestRequestTypeDef,
     DescribeEphemerisRequestRequestTypeDef,
     DiscoveryDataTypeDef,
     SecurityDetailsTypeDef,
     S3ObjectTypeDef,
+    EphemerisIdResponseTypeDef,
     EphemerisMetaDataTypeDef,
     FrequencyBandwidthTypeDef,
     FrequencyTypeDef,
     GetAgentConfigurationRequestRequestTypeDef,
+    GetAgentConfigurationResponseTypeDef,
     GetConfigRequestRequestTypeDef,
     GetDataflowEndpointGroupRequestRequestTypeDef,
     GetMinuteUsageRequestRequestTypeDef,
+    GetMinuteUsageResponseTypeDef,
     GetMissionProfileRequestRequestTypeDef,
     GetSatelliteRequestRequestTypeDef,
     GroundStationDataTypeDef,
     IntegerRangeTypeDef,
-    PaginatorConfigTypeDef,
+    ListConfigsRequestListConfigsPaginateTypeDef,
     ListConfigsRequestRequestTypeDef,
+    ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
+    ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
     ListDataflowEndpointGroupsRequestRequestTypeDef,
+    ListEphemeridesRequestListEphemeridesPaginateTypeDef,
     ListEphemeridesRequestRequestTypeDef,
+    ListGroundStationsRequestListGroundStationsPaginateTypeDef,
     ListGroundStationsRequestRequestTypeDef,
+    ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
     ListMissionProfilesRequestRequestTypeDef,
     MissionProfileListItemTypeDef,
+    ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListSatellitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MissionProfileIdResponseTypeDef,
+    PaginatorConfigTypeDef,
+    RegisterAgentResponseTypeDef,
     ReserveContactRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TimeRangeTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateAgentStatusResponseTypeDef,
     UpdateEphemerisRequestRequestTypeDef,
     AgentDetailsTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
-    ConfigIdResponseTypeDef,
-    ContactIdResponseTypeDef,
-    DataflowEndpointGroupIdResponseTypeDef,
-    EphemerisIdResponseTypeDef,
-    GetAgentConfigurationResponseTypeDef,
-    GetMinuteUsageResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MissionProfileIdResponseTypeDef,
-    RegisterAgentResponseTypeDef,
-    UpdateAgentStatusResponseTypeDef,
     ListConfigsResponseTypeDef,
     ConnectionDetailsTypeDef,
     DataflowEndpointTypeDef,
     ContactDataTypeDef,
     CreateMissionProfileRequestRequestTypeDef,
     GetMissionProfileResponseTypeDef,
     UpdateMissionProfileRequestRequestTypeDef,
@@ -468,21 +476,14 @@
     OEMEphemerisTypeDef,
     GetSatelliteResponseTypeDef,
     SatelliteListItemTypeDef,
     SpectrumConfigTypeDef,
     UplinkSpectrumConfigTypeDef,
     ListGroundStationsResponseTypeDef,
     RangedSocketAddressTypeDef,
-    ListConfigsRequestListConfigsPaginateTypeDef,
-    ListContactsRequestListContactsPaginateTypeDef,
-    ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
-    ListEphemeridesRequestListEphemeridesPaginateTypeDef,
-    ListGroundStationsRequestListGroundStationsPaginateTypeDef,
-    ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
-    ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListMissionProfilesResponseTypeDef,
     TLEDataTypeDef,
     RegisterAgentRequestRequestTypeDef,
     ListContactsResponseTypeDef,
     EphemerisTypeDescriptionTypeDef,
     ListEphemeridesResponseTypeDef,
     ListSatellitesResponseTypeDef,
@@ -517,42 +518,42 @@
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

### Comparing `mypy-boto3-groundstation-1.26.61/README.md` & `mypy-boto3-groundstation-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-groundstation"></a>
 
 # mypy-boto3-groundstation
 
 [![PyPI - mypy-boto3-groundstation](https://img.shields.io/pypi/v/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-groundstation?color=blue)](https://pypistats.org/packages/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
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
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,15 +310,16 @@
 
 ```python
 from mypy_boto3_groundstation.literals import (
     AgentStatusType,
     AngleUnitsType,
     AuditResultsType,
     BandwidthUnitsType,
-    ComponentTypeType,
+    CapabilityHealthReasonType,
+    CapabilityHealthType,
     ConfigCapabilityTypeType,
     ContactScheduledWaiterName,
     ContactStatusType,
     CriticalityType,
     EirpUnitsType,
     EndpointStatusType,
     EphemerisInvalidReasonType,
@@ -360,72 +361,79 @@
     AntennaDemodDecodeDetailsTypeDef,
     DecodeConfigTypeDef,
     DemodulationConfigTypeDef,
     EirpTypeDef,
     CancelContactRequestRequestTypeDef,
     ComponentStatusDataTypeDef,
     S3RecordingDetailsTypeDef,
-    ResponseMetadataTypeDef,
+    ConfigIdResponseTypeDef,
     ConfigListItemTypeDef,
     DataflowEndpointConfigTypeDef,
     S3RecordingConfigTypeDef,
     TrackingConfigTypeDef,
     UplinkEchoConfigTypeDef,
     SocketAddressTypeDef,
     ElevationTypeDef,
+    ContactIdResponseTypeDef,
     KmsKeyTypeDef,
+    DataflowEndpointGroupIdResponseTypeDef,
     DataflowEndpointListItemTypeDef,
     DeleteConfigRequestRequestTypeDef,
     DeleteDataflowEndpointGroupRequestRequestTypeDef,
     DeleteEphemerisRequestRequestTypeDef,
     DeleteMissionProfileRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeContactRequestRequestTypeDef,
     DescribeEphemerisRequestRequestTypeDef,
     DiscoveryDataTypeDef,
     SecurityDetailsTypeDef,
     S3ObjectTypeDef,
+    EphemerisIdResponseTypeDef,
     EphemerisMetaDataTypeDef,
     FrequencyBandwidthTypeDef,
     FrequencyTypeDef,
     GetAgentConfigurationRequestRequestTypeDef,
+    GetAgentConfigurationResponseTypeDef,
     GetConfigRequestRequestTypeDef,
     GetDataflowEndpointGroupRequestRequestTypeDef,
     GetMinuteUsageRequestRequestTypeDef,
+    GetMinuteUsageResponseTypeDef,
     GetMissionProfileRequestRequestTypeDef,
     GetSatelliteRequestRequestTypeDef,
     GroundStationDataTypeDef,
     IntegerRangeTypeDef,
-    PaginatorConfigTypeDef,
+    ListConfigsRequestListConfigsPaginateTypeDef,
     ListConfigsRequestRequestTypeDef,
+    ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
+    ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
     ListDataflowEndpointGroupsRequestRequestTypeDef,
+    ListEphemeridesRequestListEphemeridesPaginateTypeDef,
     ListEphemeridesRequestRequestTypeDef,
+    ListGroundStationsRequestListGroundStationsPaginateTypeDef,
     ListGroundStationsRequestRequestTypeDef,
+    ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
     ListMissionProfilesRequestRequestTypeDef,
     MissionProfileListItemTypeDef,
+    ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListSatellitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MissionProfileIdResponseTypeDef,
+    PaginatorConfigTypeDef,
+    RegisterAgentResponseTypeDef,
     ReserveContactRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TimeRangeTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateAgentStatusResponseTypeDef,
     UpdateEphemerisRequestRequestTypeDef,
     AgentDetailsTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
-    ConfigIdResponseTypeDef,
-    ContactIdResponseTypeDef,
-    DataflowEndpointGroupIdResponseTypeDef,
-    EphemerisIdResponseTypeDef,
-    GetAgentConfigurationResponseTypeDef,
-    GetMinuteUsageResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MissionProfileIdResponseTypeDef,
-    RegisterAgentResponseTypeDef,
-    UpdateAgentStatusResponseTypeDef,
     ListConfigsResponseTypeDef,
     ConnectionDetailsTypeDef,
     DataflowEndpointTypeDef,
     ContactDataTypeDef,
     CreateMissionProfileRequestRequestTypeDef,
     GetMissionProfileResponseTypeDef,
     UpdateMissionProfileRequestRequestTypeDef,
@@ -436,21 +444,14 @@
     OEMEphemerisTypeDef,
     GetSatelliteResponseTypeDef,
     SatelliteListItemTypeDef,
     SpectrumConfigTypeDef,
     UplinkSpectrumConfigTypeDef,
     ListGroundStationsResponseTypeDef,
     RangedSocketAddressTypeDef,
-    ListConfigsRequestListConfigsPaginateTypeDef,
-    ListContactsRequestListContactsPaginateTypeDef,
-    ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
-    ListEphemeridesRequestListEphemeridesPaginateTypeDef,
-    ListGroundStationsRequestListGroundStationsPaginateTypeDef,
-    ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
-    ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListMissionProfilesResponseTypeDef,
     TLEDataTypeDef,
     RegisterAgentRequestRequestTypeDef,
     ListContactsResponseTypeDef,
     EphemerisTypeDescriptionTypeDef,
     ListEphemeridesResponseTypeDef,
     ListSatellitesResponseTypeDef,
@@ -485,42 +486,42 @@
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

### Comparing `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/__init__.py` & `mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/__init__.pyi` & `mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/__main__.py` & `mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GroundStation 1.26.61\nVersion:         1.26.61\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.GroundStation 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation\nOther"
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

### Comparing `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/client.py` & `mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         ephemeris: EphemerisDataTypeDef = ...,
         expirationTime: Union[datetime, str] = ...,
         kmsKeyArn: str = ...,
         priority: int = ...,
         tags: Mapping[str, str] = ...
     ) -> EphemerisIdResponseTypeDef:
         """
-        Creates an Ephemeris with the specified `EphemerisData` .
+        Creates an Ephemeris with the specified `EphemerisData`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_ephemeris)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#create_ephemeris)
         """
 
     def create_mission_profile(
         self,
@@ -195,15 +195,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#create_mission_profile)
         """
 
     def delete_config(
         self, *, configId: str, configType: ConfigCapabilityTypeType
     ) -> ConfigIdResponseTypeDef:
         """
-        Deletes a `Config` .
+        Deletes a `Config`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.delete_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#delete_config)
         """
 
     def delete_dataflow_endpoint_group(
         self, *, dataflowEndpointGroupId: str
@@ -260,15 +260,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#generate_presigned_url)
         """
 
     def get_agent_configuration(self, *, agentId: str) -> GetAgentConfigurationResponseTypeDef:
         """
-        Gets the latest configuration information for a registered agent.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_agent_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#get_agent_configuration)
         """
 
     def get_config(
         self, *, configId: str, configType: ConfigCapabilityTypeType
@@ -288,15 +288,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_dataflow_endpoint_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#get_dataflow_endpoint_group)
         """
 
     def get_minute_usage(self, *, month: int, year: int) -> GetMinuteUsageResponseTypeDef:
         """
-        Returns the number of minutes used by account.
+        Returns the number of reserved minutes used by account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_minute_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#get_minute_usage)
         """
 
     def get_mission_profile(self, *, missionProfileId: str) -> GetMissionProfileResponseTypeDef:
         """
@@ -408,15 +408,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#list_tags_for_resource)
         """
 
     def register_agent(
         self, *, agentDetails: AgentDetailsTypeDef, discoveryData: DiscoveryDataTypeDef
     ) -> RegisterAgentResponseTypeDef:
         """
-        Registers a new agent with AWS Groundstation.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.register_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#register_agent)
         """
 
     def reserve_contact(
         self,
@@ -456,15 +456,15 @@
         *,
         agentId: str,
         aggregateStatus: AggregateStatusTypeDef,
         componentStatuses: Sequence[ComponentStatusDataTypeDef],
         taskId: str
     ) -> UpdateAgentStatusResponseTypeDef:
         """
-        Update the status of the agent.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_agent_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#update_agent_status)
         """
 
     def update_config(
         self,
```

### Comparing `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/client.pyi` & `mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         ephemeris: EphemerisDataTypeDef = ...,
         expirationTime: Union[datetime, str] = ...,
         kmsKeyArn: str = ...,
         priority: int = ...,
         tags: Mapping[str, str] = ...
     ) -> EphemerisIdResponseTypeDef:
         """
-        Creates an Ephemeris with the specified `EphemerisData` .
+        Creates an Ephemeris with the specified `EphemerisData`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_ephemeris)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#create_ephemeris)
         """
     def create_mission_profile(
         self,
         *,
@@ -183,15 +183,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_mission_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#create_mission_profile)
         """
     def delete_config(
         self, *, configId: str, configType: ConfigCapabilityTypeType
     ) -> ConfigIdResponseTypeDef:
         """
-        Deletes a `Config` .
+        Deletes a `Config`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.delete_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#delete_config)
         """
     def delete_dataflow_endpoint_group(
         self, *, dataflowEndpointGroupId: str
     ) -> DataflowEndpointGroupIdResponseTypeDef:
@@ -241,15 +241,15 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#generate_presigned_url)
         """
     def get_agent_configuration(self, *, agentId: str) -> GetAgentConfigurationResponseTypeDef:
         """
-        Gets the latest configuration information for a registered agent.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_agent_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#get_agent_configuration)
         """
     def get_config(
         self, *, configId: str, configType: ConfigCapabilityTypeType
     ) -> GetConfigResponseTypeDef:
@@ -266,15 +266,15 @@
         Returns the dataflow endpoint group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_dataflow_endpoint_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#get_dataflow_endpoint_group)
         """
     def get_minute_usage(self, *, month: int, year: int) -> GetMinuteUsageResponseTypeDef:
         """
-        Returns the number of minutes used by account.
+        Returns the number of reserved minutes used by account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_minute_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#get_minute_usage)
         """
     def get_mission_profile(self, *, missionProfileId: str) -> GetMissionProfileResponseTypeDef:
         """
         Returns a mission profile.
@@ -375,15 +375,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#list_tags_for_resource)
         """
     def register_agent(
         self, *, agentDetails: AgentDetailsTypeDef, discoveryData: DiscoveryDataTypeDef
     ) -> RegisterAgentResponseTypeDef:
         """
-        Registers a new agent with AWS Groundstation.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.register_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#register_agent)
         """
     def reserve_contact(
         self,
         *,
@@ -419,15 +419,15 @@
         *,
         agentId: str,
         aggregateStatus: AggregateStatusTypeDef,
         componentStatuses: Sequence[ComponentStatusDataTypeDef],
         taskId: str
     ) -> UpdateAgentStatusResponseTypeDef:
         """
-        Update the status of the agent.
+        .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_agent_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/client/#update_agent_status)
         """
     def update_config(
         self,
         *,
```

### Comparing `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/literals.py` & `mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
 
 __all__ = (
     "AgentStatusType",
     "AngleUnitsType",
     "AuditResultsType",
     "BandwidthUnitsType",
-    "ComponentTypeType",
+    "CapabilityHealthReasonType",
+    "CapabilityHealthType",
     "ConfigCapabilityTypeType",
     "ContactScheduledWaiterName",
     "ContactStatusType",
     "CriticalityType",
     "EirpUnitsType",
     "EndpointStatusType",
     "EphemerisInvalidReasonType",
@@ -52,15 +53,24 @@
 )
 
 
 AgentStatusType = Literal["ACTIVE", "FAILED", "INACTIVE", "SUCCESS"]
 AngleUnitsType = Literal["DEGREE_ANGLE", "RADIAN"]
 AuditResultsType = Literal["HEALTHY", "UNHEALTHY"]
 BandwidthUnitsType = Literal["GHz", "MHz", "kHz"]
-ComponentTypeType = Literal["DIGITIZER", "LAMINAR_FLOW", "PRISM"]
+CapabilityHealthReasonType = Literal[
+    "DATAPLANE_FAILURE",
+    "HEALTHY",
+    "INITIALIZING_DATAPLANE",
+    "INVALID_IP_OWNERSHIP",
+    "NOT_AUTHORIZED_TO_CREATE_SLR",
+    "NO_REGISTERED_AGENT",
+    "UNVERIFIED_IP_OWNERSHIP",
+]
+CapabilityHealthType = Literal["HEALTHY", "UNHEALTHY"]
 ConfigCapabilityTypeType = Literal[
     "antenna-downlink",
     "antenna-downlink-demod-decode",
     "antenna-uplink",
     "dataflow-endpoint",
     "s3-recording",
     "tracking",
@@ -115,14 +125,15 @@
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
@@ -162,14 +173,15 @@
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
@@ -248,14 +260,15 @@
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
@@ -266,14 +279,15 @@
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
@@ -309,14 +323,15 @@
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
@@ -335,16 +350,19 @@
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
@@ -424,18 +442,21 @@
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

### Comparing `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/literals.pyi` & `mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     from typing_extensions import Literal
 
 __all__ = (
     "AgentStatusType",
     "AngleUnitsType",
     "AuditResultsType",
     "BandwidthUnitsType",
-    "ComponentTypeType",
+    "CapabilityHealthReasonType",
+    "CapabilityHealthType",
     "ConfigCapabilityTypeType",
     "ContactScheduledWaiterName",
     "ContactStatusType",
     "CriticalityType",
     "EirpUnitsType",
     "EndpointStatusType",
     "EphemerisInvalidReasonType",
@@ -50,15 +51,24 @@
     "RegionName",
 )
 
 AgentStatusType = Literal["ACTIVE", "FAILED", "INACTIVE", "SUCCESS"]
 AngleUnitsType = Literal["DEGREE_ANGLE", "RADIAN"]
 AuditResultsType = Literal["HEALTHY", "UNHEALTHY"]
 BandwidthUnitsType = Literal["GHz", "MHz", "kHz"]
-ComponentTypeType = Literal["DIGITIZER", "LAMINAR_FLOW", "PRISM"]
+CapabilityHealthReasonType = Literal[
+    "DATAPLANE_FAILURE",
+    "HEALTHY",
+    "INITIALIZING_DATAPLANE",
+    "INVALID_IP_OWNERSHIP",
+    "NOT_AUTHORIZED_TO_CREATE_SLR",
+    "NO_REGISTERED_AGENT",
+    "UNVERIFIED_IP_OWNERSHIP",
+]
+CapabilityHealthType = Literal["HEALTHY", "UNHEALTHY"]
 ConfigCapabilityTypeType = Literal[
     "antenna-downlink",
     "antenna-downlink-demod-decode",
     "antenna-uplink",
     "dataflow-endpoint",
     "s3-recording",
     "tracking",
@@ -113,14 +123,15 @@
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
@@ -160,14 +171,15 @@
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
@@ -246,14 +258,15 @@
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
@@ -264,14 +277,15 @@
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
@@ -307,14 +321,15 @@
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
@@ -333,16 +348,19 @@
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
@@ -422,18 +440,21 @@
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

### Comparing `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/paginator.py` & `mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/paginator.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 class ListConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listconfigspaginator)
         """
 
 
@@ -95,30 +95,30 @@
         *,
         endTime: Union[datetime, str],
         startTime: Union[datetime, str],
         statusList: Sequence[ContactStatusType],
         groundStation: str = ...,
         missionProfileArn: str = ...,
         satelliteArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListContactsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListContacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listcontactspaginator)
         """
 
 
 class ListDataflowEndpointGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListDataflowEndpointGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listdataflowendpointgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataflowEndpointGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListDataflowEndpointGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listdataflowendpointgroupspaginator)
         """
 
 
@@ -131,58 +131,58 @@
     def paginate(
         self,
         *,
         endTime: Union[datetime, str],
         satelliteId: str,
         startTime: Union[datetime, str],
         statusList: Sequence[EphemerisStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEphemeridesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListEphemerides.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listephemeridespaginator)
         """
 
 
 class ListGroundStationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListGroundStations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listgroundstationspaginator)
     """
 
     def paginate(
-        self, *, satelliteId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, satelliteId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroundStationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListGroundStations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listgroundstationspaginator)
         """
 
 
 class ListMissionProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListMissionProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listmissionprofilespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMissionProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListMissionProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listmissionprofilespaginator)
         """
 
 
 class ListSatellitesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListSatellites)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listsatellitespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSatellitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListSatellites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listsatellitespaginator)
         """
```

### Comparing `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/paginator.pyi` & `mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/paginator.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 class ListConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listconfigspaginator)
         """
 
 class ListContactsPaginator(Paginator):
@@ -91,29 +91,29 @@
         *,
         endTime: Union[datetime, str],
         startTime: Union[datetime, str],
         statusList: Sequence[ContactStatusType],
         groundStation: str = ...,
         missionProfileArn: str = ...,
         satelliteArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListContactsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListContacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listcontactspaginator)
         """
 
 class ListDataflowEndpointGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListDataflowEndpointGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listdataflowendpointgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataflowEndpointGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListDataflowEndpointGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listdataflowendpointgroupspaginator)
         """
 
 class ListEphemeridesPaginator(Paginator):
@@ -125,55 +125,55 @@
     def paginate(
         self,
         *,
         endTime: Union[datetime, str],
         satelliteId: str,
         startTime: Union[datetime, str],
         statusList: Sequence[EphemerisStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEphemeridesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListEphemerides.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listephemeridespaginator)
         """
 
 class ListGroundStationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListGroundStations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listgroundstationspaginator)
     """
 
     def paginate(
-        self, *, satelliteId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, satelliteId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGroundStationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListGroundStations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listgroundstationspaginator)
         """
 
 class ListMissionProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListMissionProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listmissionprofilespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMissionProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListMissionProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listmissionprofilespaginator)
         """
 
 class ListSatellitesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListSatellites)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listsatellitespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSatellitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListSatellites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listsatellitespaginator)
         """
```

### Comparing `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/type_defs.py` & `mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AgentStatusType,
     AngleUnitsType,
     AuditResultsType,
     BandwidthUnitsType,
-    ComponentTypeType,
+    CapabilityHealthReasonType,
+    CapabilityHealthType,
     ConfigCapabilityTypeType,
     ContactStatusType,
     CriticalityType,
     EndpointStatusType,
     EphemerisInvalidReasonType,
     EphemerisSourceType,
     EphemerisStatusType,
@@ -48,72 +49,79 @@
     "AntennaDemodDecodeDetailsTypeDef",
     "DecodeConfigTypeDef",
     "DemodulationConfigTypeDef",
     "EirpTypeDef",
     "CancelContactRequestRequestTypeDef",
     "ComponentStatusDataTypeDef",
     "S3RecordingDetailsTypeDef",
-    "ResponseMetadataTypeDef",
+    "ConfigIdResponseTypeDef",
     "ConfigListItemTypeDef",
     "DataflowEndpointConfigTypeDef",
     "S3RecordingConfigTypeDef",
     "TrackingConfigTypeDef",
     "UplinkEchoConfigTypeDef",
     "SocketAddressTypeDef",
     "ElevationTypeDef",
+    "ContactIdResponseTypeDef",
     "KmsKeyTypeDef",
+    "DataflowEndpointGroupIdResponseTypeDef",
     "DataflowEndpointListItemTypeDef",
     "DeleteConfigRequestRequestTypeDef",
     "DeleteDataflowEndpointGroupRequestRequestTypeDef",
     "DeleteEphemerisRequestRequestTypeDef",
     "DeleteMissionProfileRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeContactRequestRequestTypeDef",
     "DescribeEphemerisRequestRequestTypeDef",
     "DiscoveryDataTypeDef",
     "SecurityDetailsTypeDef",
     "S3ObjectTypeDef",
+    "EphemerisIdResponseTypeDef",
     "EphemerisMetaDataTypeDef",
     "FrequencyBandwidthTypeDef",
     "FrequencyTypeDef",
     "GetAgentConfigurationRequestRequestTypeDef",
+    "GetAgentConfigurationResponseTypeDef",
     "GetConfigRequestRequestTypeDef",
     "GetDataflowEndpointGroupRequestRequestTypeDef",
     "GetMinuteUsageRequestRequestTypeDef",
+    "GetMinuteUsageResponseTypeDef",
     "GetMissionProfileRequestRequestTypeDef",
     "GetSatelliteRequestRequestTypeDef",
     "GroundStationDataTypeDef",
     "IntegerRangeTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListConfigsRequestListConfigsPaginateTypeDef",
     "ListConfigsRequestRequestTypeDef",
+    "ListContactsRequestListContactsPaginateTypeDef",
     "ListContactsRequestRequestTypeDef",
+    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
+    "ListEphemeridesRequestListEphemeridesPaginateTypeDef",
     "ListEphemeridesRequestRequestTypeDef",
+    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
     "ListGroundStationsRequestRequestTypeDef",
+    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
     "ListMissionProfilesRequestRequestTypeDef",
     "MissionProfileListItemTypeDef",
+    "ListSatellitesRequestListSatellitesPaginateTypeDef",
     "ListSatellitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "MissionProfileIdResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "RegisterAgentResponseTypeDef",
     "ReserveContactRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TimeRangeTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateAgentStatusResponseTypeDef",
     "UpdateEphemerisRequestRequestTypeDef",
     "AgentDetailsTypeDef",
     "UpdateAgentStatusRequestRequestTypeDef",
-    "ConfigIdResponseTypeDef",
-    "ContactIdResponseTypeDef",
-    "DataflowEndpointGroupIdResponseTypeDef",
-    "EphemerisIdResponseTypeDef",
-    "GetAgentConfigurationResponseTypeDef",
-    "GetMinuteUsageResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "MissionProfileIdResponseTypeDef",
-    "RegisterAgentResponseTypeDef",
-    "UpdateAgentStatusResponseTypeDef",
     "ListConfigsResponseTypeDef",
     "ConnectionDetailsTypeDef",
     "DataflowEndpointTypeDef",
     "ContactDataTypeDef",
     "CreateMissionProfileRequestRequestTypeDef",
     "GetMissionProfileResponseTypeDef",
     "UpdateMissionProfileRequestRequestTypeDef",
@@ -124,21 +132,14 @@
     "OEMEphemerisTypeDef",
     "GetSatelliteResponseTypeDef",
     "SatelliteListItemTypeDef",
     "SpectrumConfigTypeDef",
     "UplinkSpectrumConfigTypeDef",
     "ListGroundStationsResponseTypeDef",
     "RangedSocketAddressTypeDef",
-    "ListConfigsRequestListConfigsPaginateTypeDef",
-    "ListContactsRequestListContactsPaginateTypeDef",
-    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
-    "ListEphemeridesRequestListEphemeridesPaginateTypeDef",
-    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
-    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
-    "ListSatellitesRequestListSatellitesPaginateTypeDef",
     "ListMissionProfilesResponseTypeDef",
     "TLEDataTypeDef",
     "RegisterAgentRequestRequestTypeDef",
     "ListContactsResponseTypeDef",
     "EphemerisTypeDescriptionTypeDef",
     "ListEphemeridesResponseTypeDef",
     "ListSatellitesResponseTypeDef",
@@ -164,15 +165,15 @@
     "DataflowDetailTypeDef",
     "DescribeContactResponseTypeDef",
 )
 
 ComponentVersionTypeDef = TypedDict(
     "ComponentVersionTypeDef",
     {
-        "componentType": ComponentTypeType,
+        "componentType": str,
         "versions": Sequence[str],
     },
 )
 
 _RequiredAggregateStatusTypeDef = TypedDict(
     "_RequiredAggregateStatusTypeDef",
     {
@@ -229,15 +230,15 @@
     },
 )
 
 _RequiredComponentStatusDataTypeDef = TypedDict(
     "_RequiredComponentStatusDataTypeDef",
     {
         "capabilityArn": str,
-        "componentType": ComponentTypeType,
+        "componentType": str,
         "dataflowId": str,
         "status": AgentStatusType,
     },
 )
 _OptionalComponentStatusDataTypeDef = TypedDict(
     "_OptionalComponentStatusDataTypeDef",
     {
@@ -260,22 +261,21 @@
     {
         "bucketArn": str,
         "keyTemplate": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ConfigIdResponseTypeDef = TypedDict(
+    "ConfigIdResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "configArn": str,
+        "configId": str,
+        "configType": ConfigCapabilityTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigListItemTypeDef = TypedDict(
     "ConfigListItemTypeDef",
     {
         "configArn": str,
@@ -356,23 +356,39 @@
     "ElevationTypeDef",
     {
         "unit": AngleUnitsType,
         "value": float,
     },
 )
 
+ContactIdResponseTypeDef = TypedDict(
+    "ContactIdResponseTypeDef",
+    {
+        "contactId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 KmsKeyTypeDef = TypedDict(
     "KmsKeyTypeDef",
     {
         "kmsAliasArn": str,
         "kmsKeyArn": str,
     },
     total=False,
 )
 
+DataflowEndpointGroupIdResponseTypeDef = TypedDict(
+    "DataflowEndpointGroupIdResponseTypeDef",
+    {
+        "dataflowEndpointGroupId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataflowEndpointListItemTypeDef = TypedDict(
     "DataflowEndpointListItemTypeDef",
     {
         "dataflowEndpointGroupArn": str,
         "dataflowEndpointGroupId": str,
     },
     total=False,
@@ -454,14 +470,22 @@
         "bucket": str,
         "key": str,
         "version": str,
     },
     total=False,
 )
 
+EphemerisIdResponseTypeDef = TypedDict(
+    "EphemerisIdResponseTypeDef",
+    {
+        "ephemerisId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEphemerisMetaDataTypeDef = TypedDict(
     "_RequiredEphemerisMetaDataTypeDef",
     {
         "source": EphemerisSourceType,
     },
 )
 _OptionalEphemerisMetaDataTypeDef = TypedDict(
@@ -500,14 +524,23 @@
 GetAgentConfigurationRequestRequestTypeDef = TypedDict(
     "GetAgentConfigurationRequestRequestTypeDef",
     {
         "agentId": str,
     },
 )
 
+GetAgentConfigurationResponseTypeDef = TypedDict(
+    "GetAgentConfigurationResponseTypeDef",
+    {
+        "agentId": str,
+        "taskingDocument": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetConfigRequestRequestTypeDef = TypedDict(
     "GetConfigRequestRequestTypeDef",
     {
         "configId": str,
         "configType": ConfigCapabilityTypeType,
     },
 )
@@ -523,14 +556,26 @@
     "GetMinuteUsageRequestRequestTypeDef",
     {
         "month": int,
         "year": int,
     },
 )
 
+GetMinuteUsageResponseTypeDef = TypedDict(
+    "GetMinuteUsageResponseTypeDef",
+    {
+        "estimatedMinutesRemaining": int,
+        "isReservedMinutesCustomer": bool,
+        "totalReservedMinuteAllocation": int,
+        "totalScheduledMinutes": int,
+        "upcomingMinutesScheduled": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetMissionProfileRequestRequestTypeDef = TypedDict(
     "GetMissionProfileRequestRequestTypeDef",
     {
         "missionProfileId": str,
     },
 )
 
@@ -555,33 +600,58 @@
     "IntegerRangeTypeDef",
     {
         "maximum": int,
         "minimum": int,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListConfigsRequestListConfigsPaginateTypeDef = TypedDict(
+    "ListConfigsRequestListConfigsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListConfigsRequestRequestTypeDef = TypedDict(
     "ListConfigsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListContactsRequestListContactsPaginateTypeDef = TypedDict(
+    "_RequiredListContactsRequestListContactsPaginateTypeDef",
+    {
+        "endTime": Union[datetime, str],
+        "startTime": Union[datetime, str],
+        "statusList": Sequence[ContactStatusType],
+    },
+)
+_OptionalListContactsRequestListContactsPaginateTypeDef = TypedDict(
+    "_OptionalListContactsRequestListContactsPaginateTypeDef",
+    {
+        "groundStation": str,
+        "missionProfileArn": str,
+        "satelliteArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListContactsRequestListContactsPaginateTypeDef(
+    _RequiredListContactsRequestListContactsPaginateTypeDef,
+    _OptionalListContactsRequestListContactsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListContactsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "startTime": Union[datetime, str],
         "statusList": Sequence[ContactStatusType],
     },
@@ -601,23 +671,56 @@
 
 class ListContactsRequestRequestTypeDef(
     _RequiredListContactsRequestRequestTypeDef, _OptionalListContactsRequestRequestTypeDef
 ):
     pass
 
 
+ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef = TypedDict(
+    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDataflowEndpointGroupsRequestRequestTypeDef = TypedDict(
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
+    "_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef",
+    {
+        "endTime": Union[datetime, str],
+        "satelliteId": str,
+        "startTime": Union[datetime, str],
+    },
+)
+_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
+    "_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef",
+    {
+        "statusList": Sequence[EphemerisStatusType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListEphemeridesRequestListEphemeridesPaginateTypeDef(
+    _RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef,
+    _OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListEphemeridesRequestRequestTypeDef = TypedDict(
     "_RequiredListEphemeridesRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "satelliteId": str,
         "startTime": Union[datetime, str],
     },
@@ -635,24 +738,41 @@
 
 class ListEphemeridesRequestRequestTypeDef(
     _RequiredListEphemeridesRequestRequestTypeDef, _OptionalListEphemeridesRequestRequestTypeDef
 ):
     pass
 
 
+ListGroundStationsRequestListGroundStationsPaginateTypeDef = TypedDict(
+    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
+    {
+        "satelliteId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGroundStationsRequestRequestTypeDef = TypedDict(
     "ListGroundStationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "satelliteId": str,
     },
     total=False,
 )
 
+ListMissionProfilesRequestListMissionProfilesPaginateTypeDef = TypedDict(
+    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMissionProfilesRequestRequestTypeDef = TypedDict(
     "ListMissionProfilesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -665,14 +785,22 @@
         "missionProfileId": str,
         "name": str,
         "region": str,
     },
     total=False,
 )
 
+ListSatellitesRequestListSatellitesPaginateTypeDef = TypedDict(
+    "ListSatellitesRequestListSatellitesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSatellitesRequestRequestTypeDef = TypedDict(
     "ListSatellitesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -681,14 +809,48 @@
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
+MissionProfileIdResponseTypeDef = TypedDict(
+    "MissionProfileIdResponseTypeDef",
+    {
+        "missionProfileId": str,
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
+RegisterAgentResponseTypeDef = TypedDict(
+    "RegisterAgentResponseTypeDef",
+    {
+        "agentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredReserveContactRequestRequestTypeDef = TypedDict(
     "_RequiredReserveContactRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "groundStation": str,
         "missionProfileArn": str,
         "satelliteArn": str,
@@ -706,14 +868,25 @@
 
 class ReserveContactRequestRequestTypeDef(
     _RequiredReserveContactRequestRequestTypeDef, _OptionalReserveContactRequestRequestTypeDef
 ):
     pass
 
 
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
 TimeRangeTypeDef = TypedDict(
     "TimeRangeTypeDef",
     {
         "endTime": Union[datetime, str],
         "startTime": Union[datetime, str],
     },
 )
@@ -730,14 +903,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateAgentStatusResponseTypeDef = TypedDict(
+    "UpdateAgentStatusResponseTypeDef",
+    {
+        "agentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateEphemerisRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEphemerisRequestRequestTypeDef",
     {
         "enabled": bool,
         "ephemerisId": str,
     },
 )
@@ -753,128 +934,53 @@
 
 class UpdateEphemerisRequestRequestTypeDef(
     _RequiredUpdateEphemerisRequestRequestTypeDef, _OptionalUpdateEphemerisRequestRequestTypeDef
 ):
     pass
 
 
-AgentDetailsTypeDef = TypedDict(
-    "AgentDetailsTypeDef",
+_RequiredAgentDetailsTypeDef = TypedDict(
+    "_RequiredAgentDetailsTypeDef",
     {
         "agentVersion": str,
         "componentVersions": Sequence[ComponentVersionTypeDef],
         "instanceId": str,
         "instanceType": str,
-        "reservedCpuCores": Sequence[int],
-    },
-)
-
-UpdateAgentStatusRequestRequestTypeDef = TypedDict(
-    "UpdateAgentStatusRequestRequestTypeDef",
-    {
-        "agentId": str,
-        "aggregateStatus": AggregateStatusTypeDef,
-        "componentStatuses": Sequence[ComponentStatusDataTypeDef],
-        "taskId": str,
     },
 )
-
-ConfigIdResponseTypeDef = TypedDict(
-    "ConfigIdResponseTypeDef",
-    {
-        "configArn": str,
-        "configId": str,
-        "configType": ConfigCapabilityTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ContactIdResponseTypeDef = TypedDict(
-    "ContactIdResponseTypeDef",
+_OptionalAgentDetailsTypeDef = TypedDict(
+    "_OptionalAgentDetailsTypeDef",
     {
-        "contactId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DataflowEndpointGroupIdResponseTypeDef = TypedDict(
-    "DataflowEndpointGroupIdResponseTypeDef",
-    {
-        "dataflowEndpointGroupId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EphemerisIdResponseTypeDef = TypedDict(
-    "EphemerisIdResponseTypeDef",
-    {
-        "ephemerisId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAgentConfigurationResponseTypeDef = TypedDict(
-    "GetAgentConfigurationResponseTypeDef",
-    {
-        "agentId": str,
-        "taskingDocument": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMinuteUsageResponseTypeDef = TypedDict(
-    "GetMinuteUsageResponseTypeDef",
-    {
-        "estimatedMinutesRemaining": int,
-        "isReservedMinutesCustomer": bool,
-        "totalReservedMinuteAllocation": int,
-        "totalScheduledMinutes": int,
-        "upcomingMinutesScheduled": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "agentCpuCores": Sequence[int],
+        "reservedCpuCores": Sequence[int],
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-MissionProfileIdResponseTypeDef = TypedDict(
-    "MissionProfileIdResponseTypeDef",
-    {
-        "missionProfileId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class AgentDetailsTypeDef(_RequiredAgentDetailsTypeDef, _OptionalAgentDetailsTypeDef):
+    pass
 
-RegisterAgentResponseTypeDef = TypedDict(
-    "RegisterAgentResponseTypeDef",
-    {
-        "agentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpdateAgentStatusResponseTypeDef = TypedDict(
-    "UpdateAgentStatusResponseTypeDef",
+UpdateAgentStatusRequestRequestTypeDef = TypedDict(
+    "UpdateAgentStatusRequestRequestTypeDef",
     {
         "agentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "aggregateStatus": AggregateStatusTypeDef,
+        "componentStatuses": Sequence[ComponentStatusDataTypeDef],
+        "taskId": str,
     },
 )
 
 ListConfigsResponseTypeDef = TypedDict(
     "ListConfigsResponseTypeDef",
     {
         "configList": List[ConfigListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredConnectionDetailsTypeDef = TypedDict(
     "_RequiredConnectionDetailsTypeDef",
     {
         "socketAddress": SocketAddressTypeDef,
@@ -966,15 +1072,15 @@
         "missionProfileId": str,
         "name": str,
         "region": str,
         "streamsKmsKey": KmsKeyTypeDef,
         "streamsKmsRole": str,
         "tags": Dict[str, str],
         "trackingConfigArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateMissionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMissionProfileRequestRequestTypeDef",
     {
         "missionProfileId": str,
@@ -1004,15 +1110,15 @@
 
 
 ListDataflowEndpointGroupsResponseTypeDef = TypedDict(
     "ListDataflowEndpointGroupsResponseTypeDef",
     {
         "dataflowEndpointGroupList": List[DataflowEndpointListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeContactRequestContactScheduledWaitTypeDef = TypedDict(
     "_RequiredDescribeContactRequestContactScheduledWaitTypeDef",
     {
         "contactId": str,
@@ -1070,15 +1176,15 @@
     "GetSatelliteResponseTypeDef",
     {
         "currentEphemeris": EphemerisMetaDataTypeDef,
         "groundStations": List[str],
         "noradSatelliteID": int,
         "satelliteArn": str,
         "satelliteId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SatelliteListItemTypeDef = TypedDict(
     "SatelliteListItemTypeDef",
     {
         "currentEphemeris": EphemerisMetaDataTypeDef,
@@ -1132,125 +1238,32 @@
 
 
 ListGroundStationsResponseTypeDef = TypedDict(
     "ListGroundStationsResponseTypeDef",
     {
         "groundStationList": List[GroundStationDataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RangedSocketAddressTypeDef = TypedDict(
     "RangedSocketAddressTypeDef",
     {
         "name": str,
         "portRange": IntegerRangeTypeDef,
     },
 )
 
-ListConfigsRequestListConfigsPaginateTypeDef = TypedDict(
-    "ListConfigsRequestListConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListContactsRequestListContactsPaginateTypeDef = TypedDict(
-    "_RequiredListContactsRequestListContactsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "startTime": Union[datetime, str],
-        "statusList": Sequence[ContactStatusType],
-    },
-)
-_OptionalListContactsRequestListContactsPaginateTypeDef = TypedDict(
-    "_OptionalListContactsRequestListContactsPaginateTypeDef",
-    {
-        "groundStation": str,
-        "missionProfileArn": str,
-        "satelliteArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListContactsRequestListContactsPaginateTypeDef(
-    _RequiredListContactsRequestListContactsPaginateTypeDef,
-    _OptionalListContactsRequestListContactsPaginateTypeDef,
-):
-    pass
-
-
-ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef = TypedDict(
-    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
-    "_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "satelliteId": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
-    "_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef",
-    {
-        "statusList": Sequence[EphemerisStatusType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListEphemeridesRequestListEphemeridesPaginateTypeDef(
-    _RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef,
-    _OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef,
-):
-    pass
-
-
-ListGroundStationsRequestListGroundStationsPaginateTypeDef = TypedDict(
-    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
-    {
-        "satelliteId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListMissionProfilesRequestListMissionProfilesPaginateTypeDef = TypedDict(
-    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSatellitesRequestListSatellitesPaginateTypeDef = TypedDict(
-    "ListSatellitesRequestListSatellitesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListMissionProfilesResponseTypeDef = TypedDict(
     "ListMissionProfilesResponseTypeDef",
     {
         "missionProfileList": List[MissionProfileListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TLEDataTypeDef = TypedDict(
     "TLEDataTypeDef",
     {
         "tleLine1": str,
@@ -1268,15 +1281,15 @@
 )
 
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "contactList": List[ContactDataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EphemerisTypeDescriptionTypeDef = TypedDict(
     "EphemerisTypeDescriptionTypeDef",
     {
         "oem": EphemerisDescriptionTypeDef,
@@ -1286,24 +1299,24 @@
 )
 
 ListEphemeridesResponseTypeDef = TypedDict(
     "ListEphemeridesResponseTypeDef",
     {
         "ephemerides": List[EphemerisItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSatellitesResponseTypeDef = TypedDict(
     "ListSatellitesResponseTypeDef",
     {
         "nextToken": str,
         "satellites": List[SatelliteListItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AntennaDownlinkConfigTypeDef = TypedDict(
     "AntennaDownlinkConfigTypeDef",
     {
         "spectrumConfig": SpectrumConfigTypeDef,
@@ -1380,15 +1393,15 @@
         "invalidReason": EphemerisInvalidReasonType,
         "name": str,
         "priority": int,
         "satelliteId": str,
         "status": EphemerisStatusType,
         "suppliedData": EphemerisTypeDescriptionTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigTypeDataTypeDef = TypedDict(
     "ConfigTypeDataTypeDef",
     {
         "antennaDownlinkConfig": AntennaDownlinkConfigTypeDef,
@@ -1462,15 +1475,15 @@
     {
         "configArn": str,
         "configData": ConfigTypeDataTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "name": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConfigRequestRequestTypeDef = TypedDict(
     "UpdateConfigRequestRequestTypeDef",
     {
         "configData": ConfigTypeDataTypeDef,
@@ -1481,14 +1494,16 @@
 )
 
 EndpointDetailsTypeDef = TypedDict(
     "EndpointDetailsTypeDef",
     {
         "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointTypeDef,
         "endpoint": DataflowEndpointTypeDef,
+        "healthReasons": Sequence[CapabilityHealthReasonType],
+        "healthStatus": CapabilityHealthType,
         "securityDetails": SecurityDetailsTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateEphemerisRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEphemerisRequestRequestTypeDef",
@@ -1556,15 +1571,15 @@
     {
         "contactPostPassDurationSeconds": int,
         "contactPrePassDurationSeconds": int,
         "dataflowEndpointGroupArn": str,
         "dataflowEndpointGroupId": str,
         "endpointsDetails": List[EndpointDetailsTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "configDetails": ConfigDetailsTypeDef,
@@ -1609,10 +1624,10 @@
         "missionProfileArn": str,
         "postPassEndTime": datetime,
         "prePassStartTime": datetime,
         "region": str,
         "satelliteArn": str,
         "startTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/type_defs.pyi` & `mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AgentStatusType,
     AngleUnitsType,
     AuditResultsType,
     BandwidthUnitsType,
-    ComponentTypeType,
+    CapabilityHealthReasonType,
+    CapabilityHealthType,
     ConfigCapabilityTypeType,
     ContactStatusType,
     CriticalityType,
     EndpointStatusType,
     EphemerisInvalidReasonType,
     EphemerisSourceType,
     EphemerisStatusType,
@@ -47,72 +48,79 @@
     "AntennaDemodDecodeDetailsTypeDef",
     "DecodeConfigTypeDef",
     "DemodulationConfigTypeDef",
     "EirpTypeDef",
     "CancelContactRequestRequestTypeDef",
     "ComponentStatusDataTypeDef",
     "S3RecordingDetailsTypeDef",
-    "ResponseMetadataTypeDef",
+    "ConfigIdResponseTypeDef",
     "ConfigListItemTypeDef",
     "DataflowEndpointConfigTypeDef",
     "S3RecordingConfigTypeDef",
     "TrackingConfigTypeDef",
     "UplinkEchoConfigTypeDef",
     "SocketAddressTypeDef",
     "ElevationTypeDef",
+    "ContactIdResponseTypeDef",
     "KmsKeyTypeDef",
+    "DataflowEndpointGroupIdResponseTypeDef",
     "DataflowEndpointListItemTypeDef",
     "DeleteConfigRequestRequestTypeDef",
     "DeleteDataflowEndpointGroupRequestRequestTypeDef",
     "DeleteEphemerisRequestRequestTypeDef",
     "DeleteMissionProfileRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeContactRequestRequestTypeDef",
     "DescribeEphemerisRequestRequestTypeDef",
     "DiscoveryDataTypeDef",
     "SecurityDetailsTypeDef",
     "S3ObjectTypeDef",
+    "EphemerisIdResponseTypeDef",
     "EphemerisMetaDataTypeDef",
     "FrequencyBandwidthTypeDef",
     "FrequencyTypeDef",
     "GetAgentConfigurationRequestRequestTypeDef",
+    "GetAgentConfigurationResponseTypeDef",
     "GetConfigRequestRequestTypeDef",
     "GetDataflowEndpointGroupRequestRequestTypeDef",
     "GetMinuteUsageRequestRequestTypeDef",
+    "GetMinuteUsageResponseTypeDef",
     "GetMissionProfileRequestRequestTypeDef",
     "GetSatelliteRequestRequestTypeDef",
     "GroundStationDataTypeDef",
     "IntegerRangeTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListConfigsRequestListConfigsPaginateTypeDef",
     "ListConfigsRequestRequestTypeDef",
+    "ListContactsRequestListContactsPaginateTypeDef",
     "ListContactsRequestRequestTypeDef",
+    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
+    "ListEphemeridesRequestListEphemeridesPaginateTypeDef",
     "ListEphemeridesRequestRequestTypeDef",
+    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
     "ListGroundStationsRequestRequestTypeDef",
+    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
     "ListMissionProfilesRequestRequestTypeDef",
     "MissionProfileListItemTypeDef",
+    "ListSatellitesRequestListSatellitesPaginateTypeDef",
     "ListSatellitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "MissionProfileIdResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "RegisterAgentResponseTypeDef",
     "ReserveContactRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TimeRangeTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateAgentStatusResponseTypeDef",
     "UpdateEphemerisRequestRequestTypeDef",
     "AgentDetailsTypeDef",
     "UpdateAgentStatusRequestRequestTypeDef",
-    "ConfigIdResponseTypeDef",
-    "ContactIdResponseTypeDef",
-    "DataflowEndpointGroupIdResponseTypeDef",
-    "EphemerisIdResponseTypeDef",
-    "GetAgentConfigurationResponseTypeDef",
-    "GetMinuteUsageResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "MissionProfileIdResponseTypeDef",
-    "RegisterAgentResponseTypeDef",
-    "UpdateAgentStatusResponseTypeDef",
     "ListConfigsResponseTypeDef",
     "ConnectionDetailsTypeDef",
     "DataflowEndpointTypeDef",
     "ContactDataTypeDef",
     "CreateMissionProfileRequestRequestTypeDef",
     "GetMissionProfileResponseTypeDef",
     "UpdateMissionProfileRequestRequestTypeDef",
@@ -123,21 +131,14 @@
     "OEMEphemerisTypeDef",
     "GetSatelliteResponseTypeDef",
     "SatelliteListItemTypeDef",
     "SpectrumConfigTypeDef",
     "UplinkSpectrumConfigTypeDef",
     "ListGroundStationsResponseTypeDef",
     "RangedSocketAddressTypeDef",
-    "ListConfigsRequestListConfigsPaginateTypeDef",
-    "ListContactsRequestListContactsPaginateTypeDef",
-    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
-    "ListEphemeridesRequestListEphemeridesPaginateTypeDef",
-    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
-    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
-    "ListSatellitesRequestListSatellitesPaginateTypeDef",
     "ListMissionProfilesResponseTypeDef",
     "TLEDataTypeDef",
     "RegisterAgentRequestRequestTypeDef",
     "ListContactsResponseTypeDef",
     "EphemerisTypeDescriptionTypeDef",
     "ListEphemeridesResponseTypeDef",
     "ListSatellitesResponseTypeDef",
@@ -163,15 +164,15 @@
     "DataflowDetailTypeDef",
     "DescribeContactResponseTypeDef",
 )
 
 ComponentVersionTypeDef = TypedDict(
     "ComponentVersionTypeDef",
     {
-        "componentType": ComponentTypeType,
+        "componentType": str,
         "versions": Sequence[str],
     },
 )
 
 _RequiredAggregateStatusTypeDef = TypedDict(
     "_RequiredAggregateStatusTypeDef",
     {
@@ -226,15 +227,15 @@
     },
 )
 
 _RequiredComponentStatusDataTypeDef = TypedDict(
     "_RequiredComponentStatusDataTypeDef",
     {
         "capabilityArn": str,
-        "componentType": ComponentTypeType,
+        "componentType": str,
         "dataflowId": str,
         "status": AgentStatusType,
     },
 )
 _OptionalComponentStatusDataTypeDef = TypedDict(
     "_OptionalComponentStatusDataTypeDef",
     {
@@ -255,22 +256,21 @@
     {
         "bucketArn": str,
         "keyTemplate": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ConfigIdResponseTypeDef = TypedDict(
+    "ConfigIdResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "configArn": str,
+        "configId": str,
+        "configType": ConfigCapabilityTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigListItemTypeDef = TypedDict(
     "ConfigListItemTypeDef",
     {
         "configArn": str,
@@ -347,23 +347,39 @@
     "ElevationTypeDef",
     {
         "unit": AngleUnitsType,
         "value": float,
     },
 )
 
+ContactIdResponseTypeDef = TypedDict(
+    "ContactIdResponseTypeDef",
+    {
+        "contactId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 KmsKeyTypeDef = TypedDict(
     "KmsKeyTypeDef",
     {
         "kmsAliasArn": str,
         "kmsKeyArn": str,
     },
     total=False,
 )
 
+DataflowEndpointGroupIdResponseTypeDef = TypedDict(
+    "DataflowEndpointGroupIdResponseTypeDef",
+    {
+        "dataflowEndpointGroupId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataflowEndpointListItemTypeDef = TypedDict(
     "DataflowEndpointListItemTypeDef",
     {
         "dataflowEndpointGroupArn": str,
         "dataflowEndpointGroupId": str,
     },
     total=False,
@@ -445,14 +461,22 @@
         "bucket": str,
         "key": str,
         "version": str,
     },
     total=False,
 )
 
+EphemerisIdResponseTypeDef = TypedDict(
+    "EphemerisIdResponseTypeDef",
+    {
+        "ephemerisId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEphemerisMetaDataTypeDef = TypedDict(
     "_RequiredEphemerisMetaDataTypeDef",
     {
         "source": EphemerisSourceType,
     },
 )
 _OptionalEphemerisMetaDataTypeDef = TypedDict(
@@ -489,14 +513,23 @@
 GetAgentConfigurationRequestRequestTypeDef = TypedDict(
     "GetAgentConfigurationRequestRequestTypeDef",
     {
         "agentId": str,
     },
 )
 
+GetAgentConfigurationResponseTypeDef = TypedDict(
+    "GetAgentConfigurationResponseTypeDef",
+    {
+        "agentId": str,
+        "taskingDocument": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetConfigRequestRequestTypeDef = TypedDict(
     "GetConfigRequestRequestTypeDef",
     {
         "configId": str,
         "configType": ConfigCapabilityTypeType,
     },
 )
@@ -512,14 +545,26 @@
     "GetMinuteUsageRequestRequestTypeDef",
     {
         "month": int,
         "year": int,
     },
 )
 
+GetMinuteUsageResponseTypeDef = TypedDict(
+    "GetMinuteUsageResponseTypeDef",
+    {
+        "estimatedMinutesRemaining": int,
+        "isReservedMinutesCustomer": bool,
+        "totalReservedMinuteAllocation": int,
+        "totalScheduledMinutes": int,
+        "upcomingMinutesScheduled": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetMissionProfileRequestRequestTypeDef = TypedDict(
     "GetMissionProfileRequestRequestTypeDef",
     {
         "missionProfileId": str,
     },
 )
 
@@ -544,33 +589,56 @@
     "IntegerRangeTypeDef",
     {
         "maximum": int,
         "minimum": int,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListConfigsRequestListConfigsPaginateTypeDef = TypedDict(
+    "ListConfigsRequestListConfigsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListConfigsRequestRequestTypeDef = TypedDict(
     "ListConfigsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListContactsRequestListContactsPaginateTypeDef = TypedDict(
+    "_RequiredListContactsRequestListContactsPaginateTypeDef",
+    {
+        "endTime": Union[datetime, str],
+        "startTime": Union[datetime, str],
+        "statusList": Sequence[ContactStatusType],
+    },
+)
+_OptionalListContactsRequestListContactsPaginateTypeDef = TypedDict(
+    "_OptionalListContactsRequestListContactsPaginateTypeDef",
+    {
+        "groundStation": str,
+        "missionProfileArn": str,
+        "satelliteArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListContactsRequestListContactsPaginateTypeDef(
+    _RequiredListContactsRequestListContactsPaginateTypeDef,
+    _OptionalListContactsRequestListContactsPaginateTypeDef,
+):
+    pass
+
 _RequiredListContactsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "startTime": Union[datetime, str],
         "statusList": Sequence[ContactStatusType],
     },
@@ -588,23 +656,54 @@
 )
 
 class ListContactsRequestRequestTypeDef(
     _RequiredListContactsRequestRequestTypeDef, _OptionalListContactsRequestRequestTypeDef
 ):
     pass
 
+ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef = TypedDict(
+    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDataflowEndpointGroupsRequestRequestTypeDef = TypedDict(
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
+    "_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef",
+    {
+        "endTime": Union[datetime, str],
+        "satelliteId": str,
+        "startTime": Union[datetime, str],
+    },
+)
+_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
+    "_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef",
+    {
+        "statusList": Sequence[EphemerisStatusType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListEphemeridesRequestListEphemeridesPaginateTypeDef(
+    _RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef,
+    _OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef,
+):
+    pass
+
 _RequiredListEphemeridesRequestRequestTypeDef = TypedDict(
     "_RequiredListEphemeridesRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "satelliteId": str,
         "startTime": Union[datetime, str],
     },
@@ -620,24 +719,41 @@
 )
 
 class ListEphemeridesRequestRequestTypeDef(
     _RequiredListEphemeridesRequestRequestTypeDef, _OptionalListEphemeridesRequestRequestTypeDef
 ):
     pass
 
+ListGroundStationsRequestListGroundStationsPaginateTypeDef = TypedDict(
+    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
+    {
+        "satelliteId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGroundStationsRequestRequestTypeDef = TypedDict(
     "ListGroundStationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "satelliteId": str,
     },
     total=False,
 )
 
+ListMissionProfilesRequestListMissionProfilesPaginateTypeDef = TypedDict(
+    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMissionProfilesRequestRequestTypeDef = TypedDict(
     "ListMissionProfilesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -650,14 +766,22 @@
         "missionProfileId": str,
         "name": str,
         "region": str,
     },
     total=False,
 )
 
+ListSatellitesRequestListSatellitesPaginateTypeDef = TypedDict(
+    "ListSatellitesRequestListSatellitesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSatellitesRequestRequestTypeDef = TypedDict(
     "ListSatellitesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -666,14 +790,48 @@
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
+MissionProfileIdResponseTypeDef = TypedDict(
+    "MissionProfileIdResponseTypeDef",
+    {
+        "missionProfileId": str,
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
+RegisterAgentResponseTypeDef = TypedDict(
+    "RegisterAgentResponseTypeDef",
+    {
+        "agentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredReserveContactRequestRequestTypeDef = TypedDict(
     "_RequiredReserveContactRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "groundStation": str,
         "missionProfileArn": str,
         "satelliteArn": str,
@@ -689,14 +847,25 @@
 )
 
 class ReserveContactRequestRequestTypeDef(
     _RequiredReserveContactRequestRequestTypeDef, _OptionalReserveContactRequestRequestTypeDef
 ):
     pass
 
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
 TimeRangeTypeDef = TypedDict(
     "TimeRangeTypeDef",
     {
         "endTime": Union[datetime, str],
         "startTime": Union[datetime, str],
     },
 )
@@ -713,14 +882,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateAgentStatusResponseTypeDef = TypedDict(
+    "UpdateAgentStatusResponseTypeDef",
+    {
+        "agentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateEphemerisRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEphemerisRequestRequestTypeDef",
     {
         "enabled": bool,
         "ephemerisId": str,
     },
 )
@@ -734,128 +911,51 @@
 )
 
 class UpdateEphemerisRequestRequestTypeDef(
     _RequiredUpdateEphemerisRequestRequestTypeDef, _OptionalUpdateEphemerisRequestRequestTypeDef
 ):
     pass
 
-AgentDetailsTypeDef = TypedDict(
-    "AgentDetailsTypeDef",
+_RequiredAgentDetailsTypeDef = TypedDict(
+    "_RequiredAgentDetailsTypeDef",
     {
         "agentVersion": str,
         "componentVersions": Sequence[ComponentVersionTypeDef],
         "instanceId": str,
         "instanceType": str,
+    },
+)
+_OptionalAgentDetailsTypeDef = TypedDict(
+    "_OptionalAgentDetailsTypeDef",
+    {
+        "agentCpuCores": Sequence[int],
         "reservedCpuCores": Sequence[int],
     },
+    total=False,
 )
 
+class AgentDetailsTypeDef(_RequiredAgentDetailsTypeDef, _OptionalAgentDetailsTypeDef):
+    pass
+
 UpdateAgentStatusRequestRequestTypeDef = TypedDict(
     "UpdateAgentStatusRequestRequestTypeDef",
     {
         "agentId": str,
         "aggregateStatus": AggregateStatusTypeDef,
         "componentStatuses": Sequence[ComponentStatusDataTypeDef],
         "taskId": str,
     },
 )
 
-ConfigIdResponseTypeDef = TypedDict(
-    "ConfigIdResponseTypeDef",
-    {
-        "configArn": str,
-        "configId": str,
-        "configType": ConfigCapabilityTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ContactIdResponseTypeDef = TypedDict(
-    "ContactIdResponseTypeDef",
-    {
-        "contactId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DataflowEndpointGroupIdResponseTypeDef = TypedDict(
-    "DataflowEndpointGroupIdResponseTypeDef",
-    {
-        "dataflowEndpointGroupId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EphemerisIdResponseTypeDef = TypedDict(
-    "EphemerisIdResponseTypeDef",
-    {
-        "ephemerisId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAgentConfigurationResponseTypeDef = TypedDict(
-    "GetAgentConfigurationResponseTypeDef",
-    {
-        "agentId": str,
-        "taskingDocument": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetMinuteUsageResponseTypeDef = TypedDict(
-    "GetMinuteUsageResponseTypeDef",
-    {
-        "estimatedMinutesRemaining": int,
-        "isReservedMinutesCustomer": bool,
-        "totalReservedMinuteAllocation": int,
-        "totalScheduledMinutes": int,
-        "upcomingMinutesScheduled": int,
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
-MissionProfileIdResponseTypeDef = TypedDict(
-    "MissionProfileIdResponseTypeDef",
-    {
-        "missionProfileId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterAgentResponseTypeDef = TypedDict(
-    "RegisterAgentResponseTypeDef",
-    {
-        "agentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAgentStatusResponseTypeDef = TypedDict(
-    "UpdateAgentStatusResponseTypeDef",
-    {
-        "agentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListConfigsResponseTypeDef = TypedDict(
     "ListConfigsResponseTypeDef",
     {
         "configList": List[ConfigListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredConnectionDetailsTypeDef = TypedDict(
     "_RequiredConnectionDetailsTypeDef",
     {
         "socketAddress": SocketAddressTypeDef,
@@ -943,15 +1043,15 @@
         "missionProfileId": str,
         "name": str,
         "region": str,
         "streamsKmsKey": KmsKeyTypeDef,
         "streamsKmsRole": str,
         "tags": Dict[str, str],
         "trackingConfigArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateMissionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMissionProfileRequestRequestTypeDef",
     {
         "missionProfileId": str,
@@ -979,15 +1079,15 @@
     pass
 
 ListDataflowEndpointGroupsResponseTypeDef = TypedDict(
     "ListDataflowEndpointGroupsResponseTypeDef",
     {
         "dataflowEndpointGroupList": List[DataflowEndpointListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeContactRequestContactScheduledWaitTypeDef = TypedDict(
     "_RequiredDescribeContactRequestContactScheduledWaitTypeDef",
     {
         "contactId": str,
@@ -1043,15 +1143,15 @@
     "GetSatelliteResponseTypeDef",
     {
         "currentEphemeris": EphemerisMetaDataTypeDef,
         "groundStations": List[str],
         "noradSatelliteID": int,
         "satelliteArn": str,
         "satelliteId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SatelliteListItemTypeDef = TypedDict(
     "SatelliteListItemTypeDef",
     {
         "currentEphemeris": EphemerisMetaDataTypeDef,
@@ -1101,121 +1201,32 @@
     pass
 
 ListGroundStationsResponseTypeDef = TypedDict(
     "ListGroundStationsResponseTypeDef",
     {
         "groundStationList": List[GroundStationDataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RangedSocketAddressTypeDef = TypedDict(
     "RangedSocketAddressTypeDef",
     {
         "name": str,
         "portRange": IntegerRangeTypeDef,
     },
 )
 
-ListConfigsRequestListConfigsPaginateTypeDef = TypedDict(
-    "ListConfigsRequestListConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListContactsRequestListContactsPaginateTypeDef = TypedDict(
-    "_RequiredListContactsRequestListContactsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "startTime": Union[datetime, str],
-        "statusList": Sequence[ContactStatusType],
-    },
-)
-_OptionalListContactsRequestListContactsPaginateTypeDef = TypedDict(
-    "_OptionalListContactsRequestListContactsPaginateTypeDef",
-    {
-        "groundStation": str,
-        "missionProfileArn": str,
-        "satelliteArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListContactsRequestListContactsPaginateTypeDef(
-    _RequiredListContactsRequestListContactsPaginateTypeDef,
-    _OptionalListContactsRequestListContactsPaginateTypeDef,
-):
-    pass
-
-ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef = TypedDict(
-    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
-    "_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "satelliteId": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
-    "_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef",
-    {
-        "statusList": Sequence[EphemerisStatusType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListEphemeridesRequestListEphemeridesPaginateTypeDef(
-    _RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef,
-    _OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef,
-):
-    pass
-
-ListGroundStationsRequestListGroundStationsPaginateTypeDef = TypedDict(
-    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
-    {
-        "satelliteId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListMissionProfilesRequestListMissionProfilesPaginateTypeDef = TypedDict(
-    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSatellitesRequestListSatellitesPaginateTypeDef = TypedDict(
-    "ListSatellitesRequestListSatellitesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListMissionProfilesResponseTypeDef = TypedDict(
     "ListMissionProfilesResponseTypeDef",
     {
         "missionProfileList": List[MissionProfileListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TLEDataTypeDef = TypedDict(
     "TLEDataTypeDef",
     {
         "tleLine1": str,
@@ -1233,15 +1244,15 @@
 )
 
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "contactList": List[ContactDataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EphemerisTypeDescriptionTypeDef = TypedDict(
     "EphemerisTypeDescriptionTypeDef",
     {
         "oem": EphemerisDescriptionTypeDef,
@@ -1251,24 +1262,24 @@
 )
 
 ListEphemeridesResponseTypeDef = TypedDict(
     "ListEphemeridesResponseTypeDef",
     {
         "ephemerides": List[EphemerisItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSatellitesResponseTypeDef = TypedDict(
     "ListSatellitesResponseTypeDef",
     {
         "nextToken": str,
         "satellites": List[SatelliteListItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AntennaDownlinkConfigTypeDef = TypedDict(
     "AntennaDownlinkConfigTypeDef",
     {
         "spectrumConfig": SpectrumConfigTypeDef,
@@ -1341,15 +1352,15 @@
         "invalidReason": EphemerisInvalidReasonType,
         "name": str,
         "priority": int,
         "satelliteId": str,
         "status": EphemerisStatusType,
         "suppliedData": EphemerisTypeDescriptionTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigTypeDataTypeDef = TypedDict(
     "ConfigTypeDataTypeDef",
     {
         "antennaDownlinkConfig": AntennaDownlinkConfigTypeDef,
@@ -1419,15 +1430,15 @@
     {
         "configArn": str,
         "configData": ConfigTypeDataTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "name": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConfigRequestRequestTypeDef = TypedDict(
     "UpdateConfigRequestRequestTypeDef",
     {
         "configData": ConfigTypeDataTypeDef,
@@ -1438,14 +1449,16 @@
 )
 
 EndpointDetailsTypeDef = TypedDict(
     "EndpointDetailsTypeDef",
     {
         "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointTypeDef,
         "endpoint": DataflowEndpointTypeDef,
+        "healthReasons": Sequence[CapabilityHealthReasonType],
+        "healthStatus": CapabilityHealthType,
         "securityDetails": SecurityDetailsTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateEphemerisRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEphemerisRequestRequestTypeDef",
@@ -1509,15 +1522,15 @@
     {
         "contactPostPassDurationSeconds": int,
         "contactPrePassDurationSeconds": int,
         "dataflowEndpointGroupArn": str,
         "dataflowEndpointGroupId": str,
         "endpointsDetails": List[EndpointDetailsTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "configDetails": ConfigDetailsTypeDef,
@@ -1562,10 +1575,10 @@
         "missionProfileArn": str,
         "postPassEndTime": datetime,
         "prePassStartTime": datetime,
         "region": str,
         "satelliteArn": str,
         "startTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/waiter.py` & `mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation/waiter.pyi` & `mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/PKG-INFO` & `mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-groundstation
-Version: 1.26.61
-Summary: Type annotations for boto3.GroundStation 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.GroundStation 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-groundstation"></a>
 
 # mypy-boto3-groundstation
 
 [![PyPI - mypy-boto3-groundstation](https://img.shields.io/pypi/v/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-groundstation?color=blue)](https://pypistats.org/packages/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
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
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,15 +342,16 @@
 
 ```python
 from mypy_boto3_groundstation.literals import (
     AgentStatusType,
     AngleUnitsType,
     AuditResultsType,
     BandwidthUnitsType,
-    ComponentTypeType,
+    CapabilityHealthReasonType,
+    CapabilityHealthType,
     ConfigCapabilityTypeType,
     ContactScheduledWaiterName,
     ContactStatusType,
     CriticalityType,
     EirpUnitsType,
     EndpointStatusType,
     EphemerisInvalidReasonType,
@@ -392,72 +393,79 @@
     AntennaDemodDecodeDetailsTypeDef,
     DecodeConfigTypeDef,
     DemodulationConfigTypeDef,
     EirpTypeDef,
     CancelContactRequestRequestTypeDef,
     ComponentStatusDataTypeDef,
     S3RecordingDetailsTypeDef,
-    ResponseMetadataTypeDef,
+    ConfigIdResponseTypeDef,
     ConfigListItemTypeDef,
     DataflowEndpointConfigTypeDef,
     S3RecordingConfigTypeDef,
     TrackingConfigTypeDef,
     UplinkEchoConfigTypeDef,
     SocketAddressTypeDef,
     ElevationTypeDef,
+    ContactIdResponseTypeDef,
     KmsKeyTypeDef,
+    DataflowEndpointGroupIdResponseTypeDef,
     DataflowEndpointListItemTypeDef,
     DeleteConfigRequestRequestTypeDef,
     DeleteDataflowEndpointGroupRequestRequestTypeDef,
     DeleteEphemerisRequestRequestTypeDef,
     DeleteMissionProfileRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeContactRequestRequestTypeDef,
     DescribeEphemerisRequestRequestTypeDef,
     DiscoveryDataTypeDef,
     SecurityDetailsTypeDef,
     S3ObjectTypeDef,
+    EphemerisIdResponseTypeDef,
     EphemerisMetaDataTypeDef,
     FrequencyBandwidthTypeDef,
     FrequencyTypeDef,
     GetAgentConfigurationRequestRequestTypeDef,
+    GetAgentConfigurationResponseTypeDef,
     GetConfigRequestRequestTypeDef,
     GetDataflowEndpointGroupRequestRequestTypeDef,
     GetMinuteUsageRequestRequestTypeDef,
+    GetMinuteUsageResponseTypeDef,
     GetMissionProfileRequestRequestTypeDef,
     GetSatelliteRequestRequestTypeDef,
     GroundStationDataTypeDef,
     IntegerRangeTypeDef,
-    PaginatorConfigTypeDef,
+    ListConfigsRequestListConfigsPaginateTypeDef,
     ListConfigsRequestRequestTypeDef,
+    ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
+    ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
     ListDataflowEndpointGroupsRequestRequestTypeDef,
+    ListEphemeridesRequestListEphemeridesPaginateTypeDef,
     ListEphemeridesRequestRequestTypeDef,
+    ListGroundStationsRequestListGroundStationsPaginateTypeDef,
     ListGroundStationsRequestRequestTypeDef,
+    ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
     ListMissionProfilesRequestRequestTypeDef,
     MissionProfileListItemTypeDef,
+    ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListSatellitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MissionProfileIdResponseTypeDef,
+    PaginatorConfigTypeDef,
+    RegisterAgentResponseTypeDef,
     ReserveContactRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TimeRangeTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateAgentStatusResponseTypeDef,
     UpdateEphemerisRequestRequestTypeDef,
     AgentDetailsTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
-    ConfigIdResponseTypeDef,
-    ContactIdResponseTypeDef,
-    DataflowEndpointGroupIdResponseTypeDef,
-    EphemerisIdResponseTypeDef,
-    GetAgentConfigurationResponseTypeDef,
-    GetMinuteUsageResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MissionProfileIdResponseTypeDef,
-    RegisterAgentResponseTypeDef,
-    UpdateAgentStatusResponseTypeDef,
     ListConfigsResponseTypeDef,
     ConnectionDetailsTypeDef,
     DataflowEndpointTypeDef,
     ContactDataTypeDef,
     CreateMissionProfileRequestRequestTypeDef,
     GetMissionProfileResponseTypeDef,
     UpdateMissionProfileRequestRequestTypeDef,
@@ -468,21 +476,14 @@
     OEMEphemerisTypeDef,
     GetSatelliteResponseTypeDef,
     SatelliteListItemTypeDef,
     SpectrumConfigTypeDef,
     UplinkSpectrumConfigTypeDef,
     ListGroundStationsResponseTypeDef,
     RangedSocketAddressTypeDef,
-    ListConfigsRequestListConfigsPaginateTypeDef,
-    ListContactsRequestListContactsPaginateTypeDef,
-    ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
-    ListEphemeridesRequestListEphemeridesPaginateTypeDef,
-    ListGroundStationsRequestListGroundStationsPaginateTypeDef,
-    ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
-    ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListMissionProfilesResponseTypeDef,
     TLEDataTypeDef,
     RegisterAgentRequestRequestTypeDef,
     ListContactsResponseTypeDef,
     EphemerisTypeDescriptionTypeDef,
     ListEphemeridesResponseTypeDef,
     ListSatellitesResponseTypeDef,
@@ -517,42 +518,42 @@
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

### Comparing `mypy-boto3-groundstation-1.26.61/mypy_boto3_groundstation.egg-info/SOURCES.txt` & `mypy-boto3-groundstation-1.27.0/mypy_boto3_groundstation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.26.61/setup.py` & `mypy-boto3-groundstation-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-groundstation.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-groundstation",
-    version="1.26.61",
+    version="1.27.0",
     packages=["mypy_boto3_groundstation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GroundStation 1.26.61 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.GroundStation 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/",
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


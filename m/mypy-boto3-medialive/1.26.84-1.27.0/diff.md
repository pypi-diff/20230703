# Comparing `tmp/mypy-boto3-medialive-1.26.84.tar.gz` & `tmp/mypy-boto3-medialive-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-medialive-1.26.84.tar", last modified: Fri Mar  3 20:27:52 2023, max compression
+gzip compressed data, was "mypy-boto3-medialive-1.27.0.tar", last modified: Mon Jul  3 19:51:06 2023, max compression
```

## Comparing `mypy-boto3-medialive-1.26.84.tar` & `mypy-boto3-medialive-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:52.686264 mypy-boto3-medialive-1.26.84/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-03 20:27:36.000000 mypy-boto3-medialive-1.26.84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37135 2023-03-03 20:27:52.686264 mypy-boto3-medialive-1.26.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35640 2023-03-03 20:27:36.000000 mypy-boto3-medialive-1.26.84/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:52.686264 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-03-03 20:27:36.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-03-03 20:27:36.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-03 20:27:36.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50981 2023-03-03 20:27:37.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    50894 2023-03-03 20:27:36.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    39142 2023-03-03 20:27:38.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    39140 2023-03-03 20:27:37.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-03-03 20:27:37.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-03-03 20:27:37.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:36.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   146844 2023-03-03 20:27:41.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   146695 2023-03-03 20:27:39.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-03 20:27:36.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-03-03 20:27:37.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-03-03 20:27:37.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:27:52.686264 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37135 2023-03-03 20:27:52.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-03 20:27:52.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 20:27:52.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 20:27:52.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-03 20:27:52.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-03 20:27:52.000000 mypy-boto3-medialive-1.26.84/mypy_boto3_medialive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 20:27:52.686264 mypy-boto3-medialive-1.26.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-03 20:27:36.000000 mypy-boto3-medialive-1.26.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.259644 mypy-boto3-medialive-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:58.000000 mypy-boto3-medialive-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37113 2023-07-03 19:51:06.251644 mypy-boto3-medialive-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35620 2023-07-03 19:41:58.000000 mypy-boto3-medialive-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.251644 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-03 19:41:58.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-03 19:41:58.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:41:58.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50981 2023-07-03 19:41:58.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50894 2023-07-03 19:41:58.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    39345 2023-07-03 19:41:59.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39343 2023-07-03 19:41:59.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-07-03 19:41:58.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-03 19:41:58.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:58.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   147093 2023-07-03 19:42:03.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146944 2023-07-03 19:42:00.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:58.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-07-03 19:41:58.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-07-03 19:41:58.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.251644 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37113 2023-07-03 19:51:06.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-03 19:51:06.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:06.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:06.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:06.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:51:06.000000 mypy-boto3-medialive-1.27.0/mypy_boto3_medialive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:06.259644 mypy-boto3-medialive-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:41:58.000000 mypy-boto3-medialive-1.27.0/setup.py
```

### Comparing `mypy-boto3-medialive-1.26.84/LICENSE` & `mypy-boto3-medialive-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-medialive-1.26.84/PKG-INFO` & `mypy-boto3-medialive-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.26.84
-Summary: Type annotations for boto3.MediaLive 1.26.84 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.MediaLive 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-medialive"></a>
 
 # mypy-boto3-medialive
 
 [![PyPI - mypy-boto3-medialive](https://img.shields.io/pypi/v/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-medialive?color=blue)](https://pypistats.org/packages/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.26.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
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
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
 See how it helps to find and fix potential bugs:
 
@@ -697,15 +697,14 @@
     AudioTrackTypeDef,
     EsamTypeDef,
     Scte35SpliceInsertTypeDef,
     Scte35TimeSignalAposTypeDef,
     BatchDeleteRequestRequestTypeDef,
     BatchFailedResultModelTypeDef,
     BatchSuccessfulResultModelTypeDef,
-    ResponseMetadataTypeDef,
     BatchScheduleActionDeleteRequestTypeDef,
     BatchStartRequestRequestTypeDef,
     BatchStopRequestRequestTypeDef,
     CancelInputDeviceTransferRequestRequestTypeDef,
     EbuTtDDestinationSettingsTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
@@ -748,28 +747,30 @@
     WaiterConfigTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeInputDeviceRequestRequestTypeDef,
     InputDeviceHdSettingsTypeDef,
     InputDeviceNetworkSettingsTypeDef,
     InputDeviceUhdSettingsTypeDef,
     DescribeInputDeviceThumbnailRequestRequestTypeDef,
+    DescribeInputDeviceThumbnailResponseTypeDef,
     DescribeInputRequestRequestTypeDef,
     InputSourceTypeDef,
     MediaConnectFlowTypeDef,
     DescribeInputSecurityGroupRequestRequestTypeDef,
     InputWhitelistRuleTypeDef,
     DescribeMultiplexProgramRequestRequestTypeDef,
     DescribeMultiplexRequestRequestTypeDef,
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
     DescribeScheduleRequestRequestTypeDef,
     DvbNitSettingsTypeDef,
     DvbSdtSettingsTypeDef,
     DvbTdtSettingsTypeDef,
+    EmptyResponseMetadataTypeDef,
     FeatureActivationsTypeDef,
     NielsenConfigurationTypeDef,
     TimecodeConfigTypeDef,
     InputLossFailoverSettingsTypeDef,
     VideoBlackFailoverSettingsTypeDef,
     FecOutputSettingsTypeDef,
     FixedModeScheduleActionStartSettingsTypeDef,
@@ -790,26 +791,36 @@
     HlsInputSettingsTypeDef,
     HlsTimedMetadataScheduleActionSettingsTypeDef,
     StartTimecodeTypeDef,
     StopTimecodeTypeDef,
     InputDestinationVpcTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
     ListInputDeviceTransfersRequestRequestTypeDef,
     TransferringInputDeviceSummaryTypeDef,
+    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
     ListInputDevicesRequestRequestTypeDef,
+    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
     ListInputSecurityGroupsRequestRequestTypeDef,
+    ListInputsRequestListInputsPaginateTypeDef,
     ListInputsRequestRequestTypeDef,
+    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
     ListMultiplexProgramsRequestRequestTypeDef,
     MultiplexProgramSummaryTypeDef,
+    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
     ListMultiplexesRequestRequestTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
+    ListReservationsRequestListReservationsPaginateTypeDef,
     ListReservationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     M3u8SettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
     MediaPackageOutputDestinationSettingsTypeDef,
     MotionGraphicsActivateScheduleActionSettingsTypeDef,
     MotionGraphicsSettingsTypeDef,
     MsSmoothOutputSettingsTypeDef,
     MultiplexMediaConnectOutputDestinationSettingsTypeDef,
@@ -818,17 +829,19 @@
     MultiplexSettingsSummaryTypeDef,
     MultiplexStatmuxVideoSettingsTypeDef,
     NielsenCBETTypeDef,
     NielsenNaesIiNwTypeDef,
     OutputDestinationSettingsTypeDef,
     RtmpGroupSettingsTypeDef,
     UdpGroupSettingsTypeDef,
+    PaginatorConfigTypeDef,
     PipelinePauseStateSettingsTypeDef,
     RebootInputDeviceRequestRequestTypeDef,
     RejectInputDeviceTransferRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     Scte35InputScheduleActionSettingsTypeDef,
     Scte35ReturnToNetworkScheduleActionSettingsTypeDef,
     Scte35SpliceInsertScheduleActionSettingsTypeDef,
     StaticImageDeactivateScheduleActionSettingsTypeDef,
     Scte35DeliveryRestrictionsTypeDef,
     StartChannelRequestRequestTypeDef,
     StartInputDeviceMaintenanceWindowRequestRequestTypeDef,
@@ -854,17 +867,14 @@
     StaticImageActivateScheduleActionSettingsTypeDef,
     StaticKeySettingsTypeDef,
     AudioTrackSelectionTypeDef,
     AvailSettingsTypeDef,
     BatchDeleteResponseTypeDef,
     BatchStartResponseTypeDef,
     BatchStopResponseTypeDef,
-    DescribeInputDeviceThumbnailResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TeletextSourceSettingsTypeDef,
     CreateInputRequestRequestTypeDef,
     CreateInputSecurityGroupRequestRequestTypeDef,
     UpdateInputSecurityGroupRequestRequestTypeDef,
     CreateMultiplexRequestRequestTypeDef,
     UpdateMultiplexRequestRequestTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
@@ -886,24 +896,14 @@
     DescribeMultiplexRequestMultiplexRunningWaitTypeDef,
     DescribeMultiplexRequestMultiplexStoppedWaitTypeDef,
     DescribeInputDeviceResponseTypeDef,
     InputDeviceSummaryTypeDef,
     UpdateInputDeviceResponseTypeDef,
     DescribeInputSecurityGroupResponseTypeDef,
     InputSecurityGroupTypeDef,
-    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
-    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
-    ListInputsRequestListInputsPaginateTypeDef,
-    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
-    ListReservationsRequestListReservationsPaginateTypeDef,
     M2tsSettingsTypeDef,
     FailoverConditionSettingsTypeDef,
     ScheduleActionStartSettingsTypeDef,
     FrameCaptureCdnSettingsTypeDef,
     FrameCaptureSettingsTypeDef,
     H264FilterSettingsTypeDef,
     H265FilterSettingsTypeDef,
@@ -1030,42 +1030,42 @@
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

### Comparing `mypy-boto3-medialive-1.26.84/README.md` & `mypy-boto3-medialive-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-medialive"></a>
 
 # mypy-boto3-medialive
 
 [![PyPI - mypy-boto3-medialive](https://img.shields.io/pypi/v/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-medialive?color=blue)](https://pypistats.org/packages/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.26.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
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
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
 See how it helps to find and fix potential bugs:
 
@@ -665,15 +665,14 @@
     AudioTrackTypeDef,
     EsamTypeDef,
     Scte35SpliceInsertTypeDef,
     Scte35TimeSignalAposTypeDef,
     BatchDeleteRequestRequestTypeDef,
     BatchFailedResultModelTypeDef,
     BatchSuccessfulResultModelTypeDef,
-    ResponseMetadataTypeDef,
     BatchScheduleActionDeleteRequestTypeDef,
     BatchStartRequestRequestTypeDef,
     BatchStopRequestRequestTypeDef,
     CancelInputDeviceTransferRequestRequestTypeDef,
     EbuTtDDestinationSettingsTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
@@ -716,28 +715,30 @@
     WaiterConfigTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeInputDeviceRequestRequestTypeDef,
     InputDeviceHdSettingsTypeDef,
     InputDeviceNetworkSettingsTypeDef,
     InputDeviceUhdSettingsTypeDef,
     DescribeInputDeviceThumbnailRequestRequestTypeDef,
+    DescribeInputDeviceThumbnailResponseTypeDef,
     DescribeInputRequestRequestTypeDef,
     InputSourceTypeDef,
     MediaConnectFlowTypeDef,
     DescribeInputSecurityGroupRequestRequestTypeDef,
     InputWhitelistRuleTypeDef,
     DescribeMultiplexProgramRequestRequestTypeDef,
     DescribeMultiplexRequestRequestTypeDef,
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
     DescribeScheduleRequestRequestTypeDef,
     DvbNitSettingsTypeDef,
     DvbSdtSettingsTypeDef,
     DvbTdtSettingsTypeDef,
+    EmptyResponseMetadataTypeDef,
     FeatureActivationsTypeDef,
     NielsenConfigurationTypeDef,
     TimecodeConfigTypeDef,
     InputLossFailoverSettingsTypeDef,
     VideoBlackFailoverSettingsTypeDef,
     FecOutputSettingsTypeDef,
     FixedModeScheduleActionStartSettingsTypeDef,
@@ -758,26 +759,36 @@
     HlsInputSettingsTypeDef,
     HlsTimedMetadataScheduleActionSettingsTypeDef,
     StartTimecodeTypeDef,
     StopTimecodeTypeDef,
     InputDestinationVpcTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
     ListInputDeviceTransfersRequestRequestTypeDef,
     TransferringInputDeviceSummaryTypeDef,
+    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
     ListInputDevicesRequestRequestTypeDef,
+    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
     ListInputSecurityGroupsRequestRequestTypeDef,
+    ListInputsRequestListInputsPaginateTypeDef,
     ListInputsRequestRequestTypeDef,
+    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
     ListMultiplexProgramsRequestRequestTypeDef,
     MultiplexProgramSummaryTypeDef,
+    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
     ListMultiplexesRequestRequestTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
+    ListReservationsRequestListReservationsPaginateTypeDef,
     ListReservationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     M3u8SettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
     MediaPackageOutputDestinationSettingsTypeDef,
     MotionGraphicsActivateScheduleActionSettingsTypeDef,
     MotionGraphicsSettingsTypeDef,
     MsSmoothOutputSettingsTypeDef,
     MultiplexMediaConnectOutputDestinationSettingsTypeDef,
@@ -786,17 +797,19 @@
     MultiplexSettingsSummaryTypeDef,
     MultiplexStatmuxVideoSettingsTypeDef,
     NielsenCBETTypeDef,
     NielsenNaesIiNwTypeDef,
     OutputDestinationSettingsTypeDef,
     RtmpGroupSettingsTypeDef,
     UdpGroupSettingsTypeDef,
+    PaginatorConfigTypeDef,
     PipelinePauseStateSettingsTypeDef,
     RebootInputDeviceRequestRequestTypeDef,
     RejectInputDeviceTransferRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     Scte35InputScheduleActionSettingsTypeDef,
     Scte35ReturnToNetworkScheduleActionSettingsTypeDef,
     Scte35SpliceInsertScheduleActionSettingsTypeDef,
     StaticImageDeactivateScheduleActionSettingsTypeDef,
     Scte35DeliveryRestrictionsTypeDef,
     StartChannelRequestRequestTypeDef,
     StartInputDeviceMaintenanceWindowRequestRequestTypeDef,
@@ -822,17 +835,14 @@
     StaticImageActivateScheduleActionSettingsTypeDef,
     StaticKeySettingsTypeDef,
     AudioTrackSelectionTypeDef,
     AvailSettingsTypeDef,
     BatchDeleteResponseTypeDef,
     BatchStartResponseTypeDef,
     BatchStopResponseTypeDef,
-    DescribeInputDeviceThumbnailResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TeletextSourceSettingsTypeDef,
     CreateInputRequestRequestTypeDef,
     CreateInputSecurityGroupRequestRequestTypeDef,
     UpdateInputSecurityGroupRequestRequestTypeDef,
     CreateMultiplexRequestRequestTypeDef,
     UpdateMultiplexRequestRequestTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
@@ -854,24 +864,14 @@
     DescribeMultiplexRequestMultiplexRunningWaitTypeDef,
     DescribeMultiplexRequestMultiplexStoppedWaitTypeDef,
     DescribeInputDeviceResponseTypeDef,
     InputDeviceSummaryTypeDef,
     UpdateInputDeviceResponseTypeDef,
     DescribeInputSecurityGroupResponseTypeDef,
     InputSecurityGroupTypeDef,
-    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
-    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
-    ListInputsRequestListInputsPaginateTypeDef,
-    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
-    ListReservationsRequestListReservationsPaginateTypeDef,
     M2tsSettingsTypeDef,
     FailoverConditionSettingsTypeDef,
     ScheduleActionStartSettingsTypeDef,
     FrameCaptureCdnSettingsTypeDef,
     FrameCaptureSettingsTypeDef,
     H264FilterSettingsTypeDef,
     H265FilterSettingsTypeDef,
@@ -998,42 +998,42 @@
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

### Comparing `mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/__init__.py` & `mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/__init__.pyi` & `mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/__main__.py` & `mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaLive 1.26.84\nVersion:         1.26.84\nBuilder version:"
-        " 7.12.5\nDocs:           "
+        "Type annotations for boto3.MediaLive 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.84")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/client.py` & `mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/client.pyi` & `mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/literals.py` & `mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -788,14 +788,15 @@
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
@@ -835,14 +836,15 @@
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
@@ -940,14 +942,15 @@
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
@@ -983,14 +986,15 @@
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
@@ -1009,16 +1013,19 @@
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
@@ -1102,15 +1109,17 @@
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

### Comparing `mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/literals.pyi` & `mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -786,14 +786,15 @@
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
@@ -833,14 +834,15 @@
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
@@ -938,14 +940,15 @@
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
@@ -981,14 +984,15 @@
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
@@ -1007,16 +1011,19 @@
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
@@ -1100,15 +1107,17 @@
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

### Comparing `mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/paginator.py` & `mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,120 +82,120 @@
 class DescribeSchedulePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
     """
 
     def paginate(
-        self, *, ChannelId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ChannelId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScheduleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
         """
 
 
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
         """
 
 
 class ListInputDeviceTransfersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
     """
 
     def paginate(
-        self, *, TransferType: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TransferType: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputDeviceTransfersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
         """
 
 
 class ListInputDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
         """
 
 
 class ListInputSecurityGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputSecurityGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
         """
 
 
 class ListInputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
         """
 
 
 class ListMultiplexProgramsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
     """
 
     def paginate(
-        self, *, MultiplexId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, MultiplexId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMultiplexProgramsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
         """
 
 
 class ListMultiplexesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMultiplexesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
         """
 
 
@@ -214,15 +214,15 @@
         Duration: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listofferingspaginator)
         """
 
 
@@ -239,13 +239,13 @@
         Codec: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReservationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListReservations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listreservationspaginator)
         """
```

### Comparing `mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/paginator.pyi` & `mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -79,113 +79,113 @@
 class DescribeSchedulePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
     """
 
     def paginate(
-        self, *, ChannelId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ChannelId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScheduleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
         """
 
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
         """
 
 class ListInputDeviceTransfersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
     """
 
     def paginate(
-        self, *, TransferType: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TransferType: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputDeviceTransfersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicetransferspaginator)
         """
 
 class ListInputDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputdevicespaginator)
         """
 
 class ListInputSecurityGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputSecurityGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputsecuritygroupspaginator)
         """
 
 class ListInputsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInputsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listinputspaginator)
         """
 
 class ListMultiplexProgramsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
     """
 
     def paginate(
-        self, *, MultiplexId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, MultiplexId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMultiplexProgramsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexprogramspaginator)
         """
 
 class ListMultiplexesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMultiplexesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listmultiplexespaginator)
         """
 
 class ListOfferingsPaginator(Paginator):
@@ -203,15 +203,15 @@
         Duration: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listofferingspaginator)
         """
 
 class ListReservationsPaginator(Paginator):
@@ -227,13 +227,13 @@
         Codec: str = ...,
         MaximumBitrate: str = ...,
         MaximumFramerate: str = ...,
         Resolution: str = ...,
         ResourceType: str = ...,
         SpecialFeature: str = ...,
         VideoQuality: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReservationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListReservations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listreservationspaginator)
         """
```

### Comparing `mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/type_defs.py` & `mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,14 @@
     "AudioTrackTypeDef",
     "EsamTypeDef",
     "Scte35SpliceInsertTypeDef",
     "Scte35TimeSignalAposTypeDef",
     "BatchDeleteRequestRequestTypeDef",
     "BatchFailedResultModelTypeDef",
     "BatchSuccessfulResultModelTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchScheduleActionDeleteRequestTypeDef",
     "BatchStartRequestRequestTypeDef",
     "BatchStopRequestRequestTypeDef",
     "CancelInputDeviceTransferRequestRequestTypeDef",
     "EbuTtDDestinationSettingsTypeDef",
     "TtmlDestinationSettingsTypeDef",
     "WebvttDestinationSettingsTypeDef",
@@ -361,28 +360,30 @@
     "WaiterConfigTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeInputDeviceRequestRequestTypeDef",
     "InputDeviceHdSettingsTypeDef",
     "InputDeviceNetworkSettingsTypeDef",
     "InputDeviceUhdSettingsTypeDef",
     "DescribeInputDeviceThumbnailRequestRequestTypeDef",
+    "DescribeInputDeviceThumbnailResponseTypeDef",
     "DescribeInputRequestRequestTypeDef",
     "InputSourceTypeDef",
     "MediaConnectFlowTypeDef",
     "DescribeInputSecurityGroupRequestRequestTypeDef",
     "InputWhitelistRuleTypeDef",
     "DescribeMultiplexProgramRequestRequestTypeDef",
     "DescribeMultiplexRequestRequestTypeDef",
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeScheduleRequestDescribeSchedulePaginateTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
     "DvbNitSettingsTypeDef",
     "DvbSdtSettingsTypeDef",
     "DvbTdtSettingsTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "FeatureActivationsTypeDef",
     "NielsenConfigurationTypeDef",
     "TimecodeConfigTypeDef",
     "InputLossFailoverSettingsTypeDef",
     "VideoBlackFailoverSettingsTypeDef",
     "FecOutputSettingsTypeDef",
     "FixedModeScheduleActionStartSettingsTypeDef",
@@ -403,26 +404,36 @@
     "HlsInputSettingsTypeDef",
     "HlsTimedMetadataScheduleActionSettingsTypeDef",
     "StartTimecodeTypeDef",
     "StopTimecodeTypeDef",
     "InputDestinationVpcTypeDef",
     "InputDeviceConfigurableSettingsTypeDef",
     "InputDeviceRequestTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
     "ListInputDeviceTransfersRequestRequestTypeDef",
     "TransferringInputDeviceSummaryTypeDef",
+    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
     "ListInputDevicesRequestRequestTypeDef",
+    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
     "ListInputSecurityGroupsRequestRequestTypeDef",
+    "ListInputsRequestListInputsPaginateTypeDef",
     "ListInputsRequestRequestTypeDef",
+    "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
     "ListMultiplexProgramsRequestRequestTypeDef",
     "MultiplexProgramSummaryTypeDef",
+    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
     "ListMultiplexesRequestRequestTypeDef",
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListOfferingsRequestRequestTypeDef",
+    "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListReservationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "M3u8SettingsTypeDef",
     "MaintenanceUpdateSettingsTypeDef",
     "MediaPackageOutputDestinationSettingsTypeDef",
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
     "MotionGraphicsSettingsTypeDef",
     "MsSmoothOutputSettingsTypeDef",
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
@@ -431,17 +442,19 @@
     "MultiplexSettingsSummaryTypeDef",
     "MultiplexStatmuxVideoSettingsTypeDef",
     "NielsenCBETTypeDef",
     "NielsenNaesIiNwTypeDef",
     "OutputDestinationSettingsTypeDef",
     "RtmpGroupSettingsTypeDef",
     "UdpGroupSettingsTypeDef",
+    "PaginatorConfigTypeDef",
     "PipelinePauseStateSettingsTypeDef",
     "RebootInputDeviceRequestRequestTypeDef",
     "RejectInputDeviceTransferRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "Scte35InputScheduleActionSettingsTypeDef",
     "Scte35ReturnToNetworkScheduleActionSettingsTypeDef",
     "Scte35SpliceInsertScheduleActionSettingsTypeDef",
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
     "Scte35DeliveryRestrictionsTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StartInputDeviceMaintenanceWindowRequestRequestTypeDef",
@@ -467,17 +480,14 @@
     "StaticImageActivateScheduleActionSettingsTypeDef",
     "StaticKeySettingsTypeDef",
     "AudioTrackSelectionTypeDef",
     "AvailSettingsTypeDef",
     "BatchDeleteResponseTypeDef",
     "BatchStartResponseTypeDef",
     "BatchStopResponseTypeDef",
-    "DescribeInputDeviceThumbnailResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TeletextSourceSettingsTypeDef",
     "CreateInputRequestRequestTypeDef",
     "CreateInputSecurityGroupRequestRequestTypeDef",
     "UpdateInputSecurityGroupRequestRequestTypeDef",
     "CreateMultiplexRequestRequestTypeDef",
     "UpdateMultiplexRequestRequestTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
@@ -499,24 +509,14 @@
     "DescribeMultiplexRequestMultiplexRunningWaitTypeDef",
     "DescribeMultiplexRequestMultiplexStoppedWaitTypeDef",
     "DescribeInputDeviceResponseTypeDef",
     "InputDeviceSummaryTypeDef",
     "UpdateInputDeviceResponseTypeDef",
     "DescribeInputSecurityGroupResponseTypeDef",
     "InputSecurityGroupTypeDef",
-    "DescribeScheduleRequestDescribeSchedulePaginateTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
-    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
-    "ListInputsRequestListInputsPaginateTypeDef",
-    "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    "ListReservationsRequestListReservationsPaginateTypeDef",
     "M2tsSettingsTypeDef",
     "FailoverConditionSettingsTypeDef",
     "ScheduleActionStartSettingsTypeDef",
     "FrameCaptureCdnSettingsTypeDef",
     "FrameCaptureSettingsTypeDef",
     "H264FilterSettingsTypeDef",
     "H265FilterSettingsTypeDef",
@@ -937,25 +937,14 @@
         "Arn": str,
         "Id": str,
         "State": str,
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
 BatchScheduleActionDeleteRequestTypeDef = TypedDict(
     "BatchScheduleActionDeleteRequestTypeDef",
     {
         "ActionNames": Sequence[str],
     },
 )
 
@@ -1477,14 +1466,26 @@
     "DescribeInputDeviceThumbnailRequestRequestTypeDef",
     {
         "InputDeviceId": str,
         "Accept": Literal["image/jpeg"],
     },
 )
 
+DescribeInputDeviceThumbnailResponseTypeDef = TypedDict(
+    "DescribeInputDeviceThumbnailResponseTypeDef",
+    {
+        "Body": StreamingBody,
+        "ContentType": Literal["image/jpeg"],
+        "ContentLength": int,
+        "ETag": str,
+        "LastModified": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeInputRequestRequestTypeDef = TypedDict(
     "DescribeInputRequestRequestTypeDef",
     {
         "InputId": str,
     },
 )
 
@@ -1546,24 +1547,36 @@
 DescribeReservationRequestRequestTypeDef = TypedDict(
     "DescribeReservationRequestRequestTypeDef",
     {
         "ReservationId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
+    "_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ChannelId": str,
+    },
+)
+_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
+    "_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class DescribeScheduleRequestDescribeSchedulePaginateTypeDef(
+    _RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+    _OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduleRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalDescribeScheduleRequestRequestTypeDef = TypedDict(
@@ -1617,14 +1630,21 @@
     "DvbTdtSettingsTypeDef",
     {
         "RepInterval": int,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FeatureActivationsTypeDef = TypedDict(
     "FeatureActivationsTypeDef",
     {
         "InputPrepareScheduleActions": FeatureActivationsInputPrepareScheduleActionsType,
     },
     total=False,
 )
@@ -1832,15 +1852,17 @@
     total=False,
 )
 
 HlsId3SegmentTaggingScheduleActionSettingsTypeDef = TypedDict(
     "HlsId3SegmentTaggingScheduleActionSettingsTypeDef",
     {
         "Tag": str,
+        "Id3": str,
     },
+    total=False,
 )
 
 HlsInputSettingsTypeDef = TypedDict(
     "HlsInputSettingsTypeDef",
     {
         "Bandwidth": int,
         "BufferSegments": int,
@@ -1898,23 +1920,53 @@
     "InputDeviceRequestTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
+    "_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
+    {
+        "TransferType": str,
+    },
+)
+_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
+    "_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef(
+    _RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
+    _OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListInputDeviceTransfersRequestRequestTypeDef = TypedDict(
     "_RequiredListInputDeviceTransfersRequestRequestTypeDef",
     {
         "TransferType": str,
     },
 )
 _OptionalListInputDeviceTransfersRequestRequestTypeDef = TypedDict(
@@ -1941,41 +1993,87 @@
         "Message": str,
         "TargetCustomerId": str,
         "TransferType": InputDeviceTransferTypeType,
     },
     total=False,
 )
 
+ListInputDevicesRequestListInputDevicesPaginateTypeDef = TypedDict(
+    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInputDevicesRequestRequestTypeDef = TypedDict(
     "ListInputDevicesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef = TypedDict(
+    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInputSecurityGroupsRequestRequestTypeDef = TypedDict(
     "ListInputSecurityGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListInputsRequestListInputsPaginateTypeDef = TypedDict(
+    "ListInputsRequestListInputsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInputsRequestRequestTypeDef = TypedDict(
     "ListInputsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
+    "_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
+    {
+        "MultiplexId": str,
+    },
+)
+_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
+    "_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef(
+    _RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
+    _OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListMultiplexProgramsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultiplexProgramsRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalListMultiplexProgramsRequestRequestTypeDef = TypedDict(
@@ -2000,23 +2098,49 @@
     {
         "ChannelId": str,
         "ProgramName": str,
     },
     total=False,
 )
 
+ListMultiplexesRequestListMultiplexesPaginateTypeDef = TypedDict(
+    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMultiplexesRequestRequestTypeDef = TypedDict(
     "ListMultiplexesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    {
+        "ChannelClass": str,
+        "ChannelConfiguration": str,
+        "Codec": str,
+        "Duration": str,
+        "MaximumBitrate": str,
+        "MaximumFramerate": str,
+        "Resolution": str,
+        "ResourceType": str,
+        "SpecialFeature": str,
+        "VideoQuality": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "ChannelClass": str,
         "ChannelConfiguration": str,
         "Codec": str,
         "Duration": str,
@@ -2028,14 +2152,30 @@
         "ResourceType": str,
         "SpecialFeature": str,
         "VideoQuality": str,
     },
     total=False,
 )
 
+ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
+    "ListReservationsRequestListReservationsPaginateTypeDef",
+    {
+        "ChannelClass": str,
+        "Codec": str,
+        "MaximumBitrate": str,
+        "MaximumFramerate": str,
+        "Resolution": str,
+        "ResourceType": str,
+        "SpecialFeature": str,
+        "VideoQuality": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReservationsRequestRequestTypeDef = TypedDict(
     "ListReservationsRequestRequestTypeDef",
     {
         "ChannelClass": str,
         "Codec": str,
         "MaxResults": int,
         "MaximumBitrate": str,
@@ -2052,14 +2192,22 @@
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
 M3u8SettingsTypeDef = TypedDict(
     "M3u8SettingsTypeDef",
     {
         "AudioFramesPerPes": int,
         "AudioPids": str,
         "EcmPid": str,
         "NielsenId3Behavior": M3u8NielsenId3BehaviorType,
@@ -2229,14 +2377,24 @@
         "InputLossAction": InputLossActionForUdpOutType,
         "TimedMetadataId3Frame": UdpTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
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
 PipelinePauseStateSettingsTypeDef = TypedDict(
     "PipelinePauseStateSettingsTypeDef",
     {
         "PipelineId": PipelineIdType,
     },
 )
 
@@ -2264,14 +2422,25 @@
 RejectInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "RejectInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
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
 _RequiredScte35InputScheduleActionSettingsTypeDef = TypedDict(
     "_RequiredScte35InputScheduleActionSettingsTypeDef",
     {
         "Mode": Scte35InputModeType,
     },
 )
 _OptionalScte35InputScheduleActionSettingsTypeDef = TypedDict(
@@ -2693,60 +2862,33 @@
 )
 
 BatchDeleteResponseTypeDef = TypedDict(
     "BatchDeleteResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchStartResponseTypeDef = TypedDict(
     "BatchStartResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchStopResponseTypeDef = TypedDict(
     "BatchStopResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeInputDeviceThumbnailResponseTypeDef = TypedDict(
-    "DescribeInputDeviceThumbnailResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "ContentType": Literal["image/jpeg"],
-        "ContentLength": int,
-        "ETag": str,
-        "LastModified": datetime,
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
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TeletextSourceSettingsTypeDef = TypedDict(
     "TeletextSourceSettingsTypeDef",
     {
         "OutputRectangle": CaptionRectangleTypeDef,
@@ -2917,15 +3059,15 @@
         "RenewalSettings": RenewalSettingsTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOfferingResponseTypeDef = TypedDict(
     "DescribeOfferingResponseTypeDef",
     {
         "Arn": str,
@@ -2935,15 +3077,15 @@
         "FixedPrice": float,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "UsagePrice": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReservationResponseTypeDef = TypedDict(
     "DescribeReservationResponseTypeDef",
     {
         "Arn": str,
@@ -2961,15 +3103,15 @@
         "RenewalSettings": RenewalSettingsTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "Arn": str,
@@ -3266,15 +3408,16 @@
         "Id": str,
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputDeviceSummaryTypeDef = TypedDict(
     "InputDeviceSummaryTypeDef",
     {
         "Arn": str,
@@ -3285,14 +3428,15 @@
         "Id": str,
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
+        "Tags": Dict[str, str],
     },
     total=False,
 )
 
 UpdateInputDeviceResponseTypeDef = TypedDict(
     "UpdateInputDeviceResponseTypeDef",
     {
@@ -3304,28 +3448,29 @@
         "Id": str,
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInputSecurityGroupResponseTypeDef = TypedDict(
     "DescribeInputSecurityGroupResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Inputs": List[str],
         "State": InputSecurityGroupStateType,
         "Tags": Dict[str, str],
         "WhitelistRules": List[InputWhitelistRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputSecurityGroupTypeDef = TypedDict(
     "InputSecurityGroupTypeDef",
     {
         "Arn": str,
@@ -3334,154 +3479,14 @@
         "State": InputSecurityGroupStateType,
         "Tags": Dict[str, str],
         "WhitelistRules": List[InputWhitelistRuleTypeDef],
     },
     total=False,
 )
 
-_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
-    "_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
-    {
-        "ChannelId": str,
-    },
-)
-_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
-    "_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeScheduleRequestDescribeSchedulePaginateTypeDef(
-    _RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-    _OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-):
-    pass
-
-
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
-    "_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    {
-        "TransferType": str,
-    },
-)
-_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
-    "_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef(
-    _RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-    _OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-):
-    pass
-
-
-ListInputDevicesRequestListInputDevicesPaginateTypeDef = TypedDict(
-    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef = TypedDict(
-    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListInputsRequestListInputsPaginateTypeDef = TypedDict(
-    "ListInputsRequestListInputsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
-    "_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    {
-        "MultiplexId": str,
-    },
-)
-_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
-    "_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef(
-    _RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-    _OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-):
-    pass
-
-
-ListMultiplexesRequestListMultiplexesPaginateTypeDef = TypedDict(
-    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    {
-        "ChannelClass": str,
-        "ChannelConfiguration": str,
-        "Codec": str,
-        "Duration": str,
-        "MaximumBitrate": str,
-        "MaximumFramerate": str,
-        "Resolution": str,
-        "ResourceType": str,
-        "SpecialFeature": str,
-        "VideoQuality": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
-    "ListReservationsRequestListReservationsPaginateTypeDef",
-    {
-        "ChannelClass": str,
-        "Codec": str,
-        "MaximumBitrate": str,
-        "MaximumFramerate": str,
-        "Resolution": str,
-        "ResourceType": str,
-        "SpecialFeature": str,
-        "VideoQuality": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AbsentInputAudioBehavior": M2tsAbsentInputAudioBehaviorType,
         "Arib": M2tsAribType,
         "AribCaptionsPid": str,
         "AribCaptionsPidControl": M2tsAribCaptionsPidControlType,
@@ -3720,24 +3725,24 @@
 
 
 ListInputDeviceTransfersResponseTypeDef = TypedDict(
     "ListInputDeviceTransfersResponseTypeDef",
     {
         "InputDeviceTransfers": List[TransferringInputDeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMultiplexProgramsResponseTypeDef = TypedDict(
     "ListMultiplexProgramsResponseTypeDef",
     {
         "MultiplexPrograms": List[MultiplexProgramSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStandardHlsSettingsTypeDef = TypedDict(
     "_RequiredStandardHlsSettingsTypeDef",
     {
         "M3u8Settings": M3u8SettingsTypeDef,
@@ -3997,74 +4002,74 @@
 )
 
 ListOfferingsResponseTypeDef = TypedDict(
     "ListOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "Offerings": List[OfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReservationsResponseTypeDef = TypedDict(
     "ListReservationsResponseTypeDef",
     {
         "NextToken": str,
         "Reservations": List[ReservationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PurchaseOfferingResponseTypeDef = TypedDict(
     "PurchaseOfferingResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateReservationResponseTypeDef = TypedDict(
     "UpdateReservationResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInputDevicesResponseTypeDef = TypedDict(
     "ListInputDevicesResponseTypeDef",
     {
         "InputDevices": List[InputDeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInputSecurityGroupResponseTypeDef = TypedDict(
     "CreateInputSecurityGroupResponseTypeDef",
     {
         "SecurityGroup": InputSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInputSecurityGroupsResponseTypeDef = TypedDict(
     "ListInputSecurityGroupsResponseTypeDef",
     {
         "InputSecurityGroups": List[InputSecurityGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInputSecurityGroupResponseTypeDef = TypedDict(
     "UpdateInputSecurityGroupResponseTypeDef",
     {
         "SecurityGroup": InputSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ArchiveContainerSettingsTypeDef = TypedDict(
     "ArchiveContainerSettingsTypeDef",
     {
         "M2tsSettings": M2tsSettingsTypeDef,
@@ -4288,15 +4293,15 @@
         "Name": str,
         "RoleArn": str,
         "SecurityGroups": List[str],
         "Sources": List[InputSourceTypeDef],
         "State": InputStateType,
         "Tags": Dict[str, str],
         "Type": InputTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputTypeDef = TypedDict(
     "InputTypeDef",
     {
         "Arn": str,
@@ -4339,15 +4344,15 @@
         "Id": str,
         "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMultiplexResponseTypeDef = TypedDict(
     "DescribeMultiplexResponseTypeDef",
     {
         "Arn": str,
@@ -4356,15 +4361,15 @@
         "Id": str,
         "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MultiplexTypeDef = TypedDict(
     "MultiplexTypeDef",
     {
         "Arn": str,
@@ -4390,15 +4395,15 @@
         "Id": str,
         "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopMultiplexResponseTypeDef = TypedDict(
     "StopMultiplexResponseTypeDef",
     {
         "Arn": str,
@@ -4407,24 +4412,24 @@
         "Id": str,
         "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMultiplexesResponseTypeDef = TypedDict(
     "ListMultiplexesResponseTypeDef",
     {
         "Multiplexes": List[MultiplexSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMultiplexProgramSettingsTypeDef = TypedDict(
     "_RequiredMultiplexProgramSettingsTypeDef",
     {
         "ProgramNumber": int,
@@ -4699,40 +4704,40 @@
     total=False,
 )
 
 CreateInputResponseTypeDef = TypedDict(
     "CreateInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePartnerInputResponseTypeDef = TypedDict(
     "CreatePartnerInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "Inputs": List[InputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInputResponseTypeDef = TypedDict(
     "UpdateInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredHlsOutputSettingsTypeDef = TypedDict(
     "_RequiredHlsOutputSettingsTypeDef",
     {
         "HlsSettings": HlsSettingsTypeDef,
@@ -4755,23 +4760,23 @@
     pass
 
 
 CreateMultiplexResponseTypeDef = TypedDict(
     "CreateMultiplexResponseTypeDef",
     {
         "Multiplex": MultiplexTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMultiplexResponseTypeDef = TypedDict(
     "UpdateMultiplexResponseTypeDef",
     {
         "Multiplex": MultiplexTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMultiplexProgramRequestRequestTypeDef = TypedDict(
     "CreateMultiplexProgramRequestRequestTypeDef",
     {
         "MultiplexId": str,
@@ -4785,27 +4790,27 @@
     "DeleteMultiplexProgramResponseTypeDef",
     {
         "ChannelId": str,
         "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMultiplexProgramResponseTypeDef = TypedDict(
     "DescribeMultiplexProgramResponseTypeDef",
     {
         "ChannelId": str,
         "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MultiplexProgramTypeDef = TypedDict(
     "MultiplexProgramTypeDef",
     {
         "ChannelId": str,
@@ -4947,23 +4952,23 @@
     total=False,
 )
 
 CreateMultiplexProgramResponseTypeDef = TypedDict(
     "CreateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMultiplexProgramResponseTypeDef = TypedDict(
     "UpdateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 Scte35TimeSignalScheduleActionSettingsTypeDef = TypedDict(
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
     {
         "Scte35Descriptors": Sequence[Scte35DescriptorTypeDef],
@@ -5076,15 +5081,15 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEncoderSettingsTypeDef = TypedDict(
     "_RequiredEncoderSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
@@ -5135,15 +5140,15 @@
 )
 
 DescribeScheduleResponseTypeDef = TypedDict(
     "DescribeScheduleResponseTypeDef",
     {
         "NextToken": str,
         "ScheduleActions": List[ScheduleActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Arn": str,
@@ -5206,15 +5211,15 @@
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
@@ -5231,15 +5236,15 @@
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartChannelResponseTypeDef = TypedDict(
     "StartChannelResponseTypeDef",
     {
         "Arn": str,
@@ -5256,15 +5261,15 @@
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopChannelResponseTypeDef = TypedDict(
     "StopChannelResponseTypeDef",
     {
         "Arn": str,
@@ -5281,15 +5286,15 @@
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
@@ -5342,34 +5347,34 @@
 
 
 BatchUpdateScheduleResponseTypeDef = TypedDict(
     "BatchUpdateScheduleResponseTypeDef",
     {
         "Creates": BatchScheduleActionCreateResultTypeDef,
         "Deletes": BatchScheduleActionDeleteResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelClassResponseTypeDef = TypedDict(
     "UpdateChannelClassResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/type_defs.pyi` & `mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -309,15 +309,14 @@
     "AudioTrackTypeDef",
     "EsamTypeDef",
     "Scte35SpliceInsertTypeDef",
     "Scte35TimeSignalAposTypeDef",
     "BatchDeleteRequestRequestTypeDef",
     "BatchFailedResultModelTypeDef",
     "BatchSuccessfulResultModelTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchScheduleActionDeleteRequestTypeDef",
     "BatchStartRequestRequestTypeDef",
     "BatchStopRequestRequestTypeDef",
     "CancelInputDeviceTransferRequestRequestTypeDef",
     "EbuTtDDestinationSettingsTypeDef",
     "TtmlDestinationSettingsTypeDef",
     "WebvttDestinationSettingsTypeDef",
@@ -360,28 +359,30 @@
     "WaiterConfigTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeInputDeviceRequestRequestTypeDef",
     "InputDeviceHdSettingsTypeDef",
     "InputDeviceNetworkSettingsTypeDef",
     "InputDeviceUhdSettingsTypeDef",
     "DescribeInputDeviceThumbnailRequestRequestTypeDef",
+    "DescribeInputDeviceThumbnailResponseTypeDef",
     "DescribeInputRequestRequestTypeDef",
     "InputSourceTypeDef",
     "MediaConnectFlowTypeDef",
     "DescribeInputSecurityGroupRequestRequestTypeDef",
     "InputWhitelistRuleTypeDef",
     "DescribeMultiplexProgramRequestRequestTypeDef",
     "DescribeMultiplexRequestRequestTypeDef",
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeScheduleRequestDescribeSchedulePaginateTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
     "DvbNitSettingsTypeDef",
     "DvbSdtSettingsTypeDef",
     "DvbTdtSettingsTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "FeatureActivationsTypeDef",
     "NielsenConfigurationTypeDef",
     "TimecodeConfigTypeDef",
     "InputLossFailoverSettingsTypeDef",
     "VideoBlackFailoverSettingsTypeDef",
     "FecOutputSettingsTypeDef",
     "FixedModeScheduleActionStartSettingsTypeDef",
@@ -402,26 +403,36 @@
     "HlsInputSettingsTypeDef",
     "HlsTimedMetadataScheduleActionSettingsTypeDef",
     "StartTimecodeTypeDef",
     "StopTimecodeTypeDef",
     "InputDestinationVpcTypeDef",
     "InputDeviceConfigurableSettingsTypeDef",
     "InputDeviceRequestTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
+    "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
     "ListInputDeviceTransfersRequestRequestTypeDef",
     "TransferringInputDeviceSummaryTypeDef",
+    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
     "ListInputDevicesRequestRequestTypeDef",
+    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
     "ListInputSecurityGroupsRequestRequestTypeDef",
+    "ListInputsRequestListInputsPaginateTypeDef",
     "ListInputsRequestRequestTypeDef",
+    "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
     "ListMultiplexProgramsRequestRequestTypeDef",
     "MultiplexProgramSummaryTypeDef",
+    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
     "ListMultiplexesRequestRequestTypeDef",
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListOfferingsRequestRequestTypeDef",
+    "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListReservationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "M3u8SettingsTypeDef",
     "MaintenanceUpdateSettingsTypeDef",
     "MediaPackageOutputDestinationSettingsTypeDef",
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
     "MotionGraphicsSettingsTypeDef",
     "MsSmoothOutputSettingsTypeDef",
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
@@ -430,17 +441,19 @@
     "MultiplexSettingsSummaryTypeDef",
     "MultiplexStatmuxVideoSettingsTypeDef",
     "NielsenCBETTypeDef",
     "NielsenNaesIiNwTypeDef",
     "OutputDestinationSettingsTypeDef",
     "RtmpGroupSettingsTypeDef",
     "UdpGroupSettingsTypeDef",
+    "PaginatorConfigTypeDef",
     "PipelinePauseStateSettingsTypeDef",
     "RebootInputDeviceRequestRequestTypeDef",
     "RejectInputDeviceTransferRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "Scte35InputScheduleActionSettingsTypeDef",
     "Scte35ReturnToNetworkScheduleActionSettingsTypeDef",
     "Scte35SpliceInsertScheduleActionSettingsTypeDef",
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
     "Scte35DeliveryRestrictionsTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StartInputDeviceMaintenanceWindowRequestRequestTypeDef",
@@ -466,17 +479,14 @@
     "StaticImageActivateScheduleActionSettingsTypeDef",
     "StaticKeySettingsTypeDef",
     "AudioTrackSelectionTypeDef",
     "AvailSettingsTypeDef",
     "BatchDeleteResponseTypeDef",
     "BatchStartResponseTypeDef",
     "BatchStopResponseTypeDef",
-    "DescribeInputDeviceThumbnailResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TeletextSourceSettingsTypeDef",
     "CreateInputRequestRequestTypeDef",
     "CreateInputSecurityGroupRequestRequestTypeDef",
     "UpdateInputSecurityGroupRequestRequestTypeDef",
     "CreateMultiplexRequestRequestTypeDef",
     "UpdateMultiplexRequestRequestTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
@@ -498,24 +508,14 @@
     "DescribeMultiplexRequestMultiplexRunningWaitTypeDef",
     "DescribeMultiplexRequestMultiplexStoppedWaitTypeDef",
     "DescribeInputDeviceResponseTypeDef",
     "InputDeviceSummaryTypeDef",
     "UpdateInputDeviceResponseTypeDef",
     "DescribeInputSecurityGroupResponseTypeDef",
     "InputSecurityGroupTypeDef",
-    "DescribeScheduleRequestDescribeSchedulePaginateTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    "ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
-    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
-    "ListInputsRequestListInputsPaginateTypeDef",
-    "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    "ListReservationsRequestListReservationsPaginateTypeDef",
     "M2tsSettingsTypeDef",
     "FailoverConditionSettingsTypeDef",
     "ScheduleActionStartSettingsTypeDef",
     "FrameCaptureCdnSettingsTypeDef",
     "FrameCaptureSettingsTypeDef",
     "H264FilterSettingsTypeDef",
     "H265FilterSettingsTypeDef",
@@ -928,25 +928,14 @@
         "Arn": str,
         "Id": str,
         "State": str,
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
 BatchScheduleActionDeleteRequestTypeDef = TypedDict(
     "BatchScheduleActionDeleteRequestTypeDef",
     {
         "ActionNames": Sequence[str],
     },
 )
 
@@ -1458,14 +1447,26 @@
     "DescribeInputDeviceThumbnailRequestRequestTypeDef",
     {
         "InputDeviceId": str,
         "Accept": Literal["image/jpeg"],
     },
 )
 
+DescribeInputDeviceThumbnailResponseTypeDef = TypedDict(
+    "DescribeInputDeviceThumbnailResponseTypeDef",
+    {
+        "Body": StreamingBody,
+        "ContentType": Literal["image/jpeg"],
+        "ContentLength": int,
+        "ETag": str,
+        "LastModified": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeInputRequestRequestTypeDef = TypedDict(
     "DescribeInputRequestRequestTypeDef",
     {
         "InputId": str,
     },
 )
 
@@ -1527,24 +1528,34 @@
 DescribeReservationRequestRequestTypeDef = TypedDict(
     "DescribeReservationRequestRequestTypeDef",
     {
         "ReservationId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
+    "_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ChannelId": str,
+    },
+)
+_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
+    "_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class DescribeScheduleRequestDescribeSchedulePaginateTypeDef(
+    _RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+    _OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduleRequestRequestTypeDef",
     {
         "ChannelId": str,
     },
 )
 _OptionalDescribeScheduleRequestRequestTypeDef = TypedDict(
@@ -1594,14 +1605,21 @@
     "DvbTdtSettingsTypeDef",
     {
         "RepInterval": int,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FeatureActivationsTypeDef = TypedDict(
     "FeatureActivationsTypeDef",
     {
         "InputPrepareScheduleActions": FeatureActivationsInputPrepareScheduleActionsType,
     },
     total=False,
 )
@@ -1805,15 +1823,17 @@
     total=False,
 )
 
 HlsId3SegmentTaggingScheduleActionSettingsTypeDef = TypedDict(
     "HlsId3SegmentTaggingScheduleActionSettingsTypeDef",
     {
         "Tag": str,
+        "Id3": str,
     },
+    total=False,
 )
 
 HlsInputSettingsTypeDef = TypedDict(
     "HlsInputSettingsTypeDef",
     {
         "Bandwidth": int,
         "BufferSegments": int,
@@ -1871,23 +1891,51 @@
     "InputDeviceRequestTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
+    "_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
+    {
+        "TransferType": str,
+    },
+)
+_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
+    "_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef(
+    _RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
+    _OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
+):
+    pass
+
 _RequiredListInputDeviceTransfersRequestRequestTypeDef = TypedDict(
     "_RequiredListInputDeviceTransfersRequestRequestTypeDef",
     {
         "TransferType": str,
     },
 )
 _OptionalListInputDeviceTransfersRequestRequestTypeDef = TypedDict(
@@ -1912,41 +1960,85 @@
         "Message": str,
         "TargetCustomerId": str,
         "TransferType": InputDeviceTransferTypeType,
     },
     total=False,
 )
 
+ListInputDevicesRequestListInputDevicesPaginateTypeDef = TypedDict(
+    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInputDevicesRequestRequestTypeDef = TypedDict(
     "ListInputDevicesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef = TypedDict(
+    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInputSecurityGroupsRequestRequestTypeDef = TypedDict(
     "ListInputSecurityGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListInputsRequestListInputsPaginateTypeDef = TypedDict(
+    "ListInputsRequestListInputsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListInputsRequestRequestTypeDef = TypedDict(
     "ListInputsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
+    "_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
+    {
+        "MultiplexId": str,
+    },
+)
+_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
+    "_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef(
+    _RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
+    _OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
+):
+    pass
+
 _RequiredListMultiplexProgramsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultiplexProgramsRequestRequestTypeDef",
     {
         "MultiplexId": str,
     },
 )
 _OptionalListMultiplexProgramsRequestRequestTypeDef = TypedDict(
@@ -1969,23 +2061,49 @@
     {
         "ChannelId": str,
         "ProgramName": str,
     },
     total=False,
 )
 
+ListMultiplexesRequestListMultiplexesPaginateTypeDef = TypedDict(
+    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMultiplexesRequestRequestTypeDef = TypedDict(
     "ListMultiplexesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    {
+        "ChannelClass": str,
+        "ChannelConfiguration": str,
+        "Codec": str,
+        "Duration": str,
+        "MaximumBitrate": str,
+        "MaximumFramerate": str,
+        "Resolution": str,
+        "ResourceType": str,
+        "SpecialFeature": str,
+        "VideoQuality": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "ChannelClass": str,
         "ChannelConfiguration": str,
         "Codec": str,
         "Duration": str,
@@ -1997,14 +2115,30 @@
         "ResourceType": str,
         "SpecialFeature": str,
         "VideoQuality": str,
     },
     total=False,
 )
 
+ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
+    "ListReservationsRequestListReservationsPaginateTypeDef",
+    {
+        "ChannelClass": str,
+        "Codec": str,
+        "MaximumBitrate": str,
+        "MaximumFramerate": str,
+        "Resolution": str,
+        "ResourceType": str,
+        "SpecialFeature": str,
+        "VideoQuality": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReservationsRequestRequestTypeDef = TypedDict(
     "ListReservationsRequestRequestTypeDef",
     {
         "ChannelClass": str,
         "Codec": str,
         "MaxResults": int,
         "MaximumBitrate": str,
@@ -2021,14 +2155,22 @@
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
 M3u8SettingsTypeDef = TypedDict(
     "M3u8SettingsTypeDef",
     {
         "AudioFramesPerPes": int,
         "AudioPids": str,
         "EcmPid": str,
         "NielsenId3Behavior": M3u8NielsenId3BehaviorType,
@@ -2196,14 +2338,24 @@
         "InputLossAction": InputLossActionForUdpOutType,
         "TimedMetadataId3Frame": UdpTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
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
 PipelinePauseStateSettingsTypeDef = TypedDict(
     "PipelinePauseStateSettingsTypeDef",
     {
         "PipelineId": PipelineIdType,
     },
 )
 
@@ -2229,14 +2381,25 @@
 RejectInputDeviceTransferRequestRequestTypeDef = TypedDict(
     "RejectInputDeviceTransferRequestRequestTypeDef",
     {
         "InputDeviceId": str,
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
 _RequiredScte35InputScheduleActionSettingsTypeDef = TypedDict(
     "_RequiredScte35InputScheduleActionSettingsTypeDef",
     {
         "Mode": Scte35InputModeType,
     },
 )
 _OptionalScte35InputScheduleActionSettingsTypeDef = TypedDict(
@@ -2642,60 +2805,33 @@
 )
 
 BatchDeleteResponseTypeDef = TypedDict(
     "BatchDeleteResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchStartResponseTypeDef = TypedDict(
     "BatchStartResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchStopResponseTypeDef = TypedDict(
     "BatchStopResponseTypeDef",
     {
         "Failed": List[BatchFailedResultModelTypeDef],
         "Successful": List[BatchSuccessfulResultModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeInputDeviceThumbnailResponseTypeDef = TypedDict(
-    "DescribeInputDeviceThumbnailResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "ContentType": Literal["image/jpeg"],
-        "ContentLength": int,
-        "ETag": str,
-        "LastModified": datetime,
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
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TeletextSourceSettingsTypeDef = TypedDict(
     "TeletextSourceSettingsTypeDef",
     {
         "OutputRectangle": CaptionRectangleTypeDef,
@@ -2856,15 +2992,15 @@
         "RenewalSettings": RenewalSettingsTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOfferingResponseTypeDef = TypedDict(
     "DescribeOfferingResponseTypeDef",
     {
         "Arn": str,
@@ -2874,15 +3010,15 @@
         "FixedPrice": float,
         "OfferingDescription": str,
         "OfferingId": str,
         "OfferingType": Literal["NO_UPFRONT"],
         "Region": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "UsagePrice": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReservationResponseTypeDef = TypedDict(
     "DescribeReservationResponseTypeDef",
     {
         "Arn": str,
@@ -2900,15 +3036,15 @@
         "RenewalSettings": RenewalSettingsTypeDef,
         "ReservationId": str,
         "ResourceSpecification": ReservationResourceSpecificationTypeDef,
         "Start": str,
         "State": ReservationStateType,
         "Tags": Dict[str, str],
         "UsagePrice": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "Arn": str,
@@ -3183,15 +3319,16 @@
         "Id": str,
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputDeviceSummaryTypeDef = TypedDict(
     "InputDeviceSummaryTypeDef",
     {
         "Arn": str,
@@ -3202,14 +3339,15 @@
         "Id": str,
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
+        "Tags": Dict[str, str],
     },
     total=False,
 )
 
 UpdateInputDeviceResponseTypeDef = TypedDict(
     "UpdateInputDeviceResponseTypeDef",
     {
@@ -3221,28 +3359,29 @@
         "Id": str,
         "MacAddress": str,
         "Name": str,
         "NetworkSettings": InputDeviceNetworkSettingsTypeDef,
         "SerialNumber": str,
         "Type": InputDeviceTypeType,
         "UhdDeviceSettings": InputDeviceUhdSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeInputSecurityGroupResponseTypeDef = TypedDict(
     "DescribeInputSecurityGroupResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Inputs": List[str],
         "State": InputSecurityGroupStateType,
         "Tags": Dict[str, str],
         "WhitelistRules": List[InputWhitelistRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputSecurityGroupTypeDef = TypedDict(
     "InputSecurityGroupTypeDef",
     {
         "Arn": str,
@@ -3251,148 +3390,14 @@
         "State": InputSecurityGroupStateType,
         "Tags": Dict[str, str],
         "WhitelistRules": List[InputWhitelistRuleTypeDef],
     },
     total=False,
 )
 
-_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
-    "_RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
-    {
-        "ChannelId": str,
-    },
-)
-_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef = TypedDict(
-    "_OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeScheduleRequestDescribeSchedulePaginateTypeDef(
-    _RequiredDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-    _OptionalDescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-):
-    pass
-
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
-    "_RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    {
-        "TransferType": str,
-    },
-)
-_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = TypedDict(
-    "_OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef(
-    _RequiredListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-    _OptionalListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-):
-    pass
-
-ListInputDevicesRequestListInputDevicesPaginateTypeDef = TypedDict(
-    "ListInputDevicesRequestListInputDevicesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef = TypedDict(
-    "ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListInputsRequestListInputsPaginateTypeDef = TypedDict(
-    "ListInputsRequestListInputsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
-    "_RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    {
-        "MultiplexId": str,
-    },
-)
-_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = TypedDict(
-    "_OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef(
-    _RequiredListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-    _OptionalListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-):
-    pass
-
-ListMultiplexesRequestListMultiplexesPaginateTypeDef = TypedDict(
-    "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    {
-        "ChannelClass": str,
-        "ChannelConfiguration": str,
-        "Codec": str,
-        "Duration": str,
-        "MaximumBitrate": str,
-        "MaximumFramerate": str,
-        "Resolution": str,
-        "ResourceType": str,
-        "SpecialFeature": str,
-        "VideoQuality": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
-    "ListReservationsRequestListReservationsPaginateTypeDef",
-    {
-        "ChannelClass": str,
-        "Codec": str,
-        "MaximumBitrate": str,
-        "MaximumFramerate": str,
-        "Resolution": str,
-        "ResourceType": str,
-        "SpecialFeature": str,
-        "VideoQuality": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AbsentInputAudioBehavior": M2tsAbsentInputAudioBehaviorType,
         "Arib": M2tsAribType,
         "AribCaptionsPid": str,
         "AribCaptionsPidControl": M2tsAribCaptionsPidControlType,
@@ -3625,24 +3630,24 @@
     pass
 
 ListInputDeviceTransfersResponseTypeDef = TypedDict(
     "ListInputDeviceTransfersResponseTypeDef",
     {
         "InputDeviceTransfers": List[TransferringInputDeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMultiplexProgramsResponseTypeDef = TypedDict(
     "ListMultiplexProgramsResponseTypeDef",
     {
         "MultiplexPrograms": List[MultiplexProgramSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStandardHlsSettingsTypeDef = TypedDict(
     "_RequiredStandardHlsSettingsTypeDef",
     {
         "M3u8Settings": M3u8SettingsTypeDef,
@@ -3892,74 +3897,74 @@
 )
 
 ListOfferingsResponseTypeDef = TypedDict(
     "ListOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "Offerings": List[OfferingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReservationsResponseTypeDef = TypedDict(
     "ListReservationsResponseTypeDef",
     {
         "NextToken": str,
         "Reservations": List[ReservationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PurchaseOfferingResponseTypeDef = TypedDict(
     "PurchaseOfferingResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateReservationResponseTypeDef = TypedDict(
     "UpdateReservationResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInputDevicesResponseTypeDef = TypedDict(
     "ListInputDevicesResponseTypeDef",
     {
         "InputDevices": List[InputDeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInputSecurityGroupResponseTypeDef = TypedDict(
     "CreateInputSecurityGroupResponseTypeDef",
     {
         "SecurityGroup": InputSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInputSecurityGroupsResponseTypeDef = TypedDict(
     "ListInputSecurityGroupsResponseTypeDef",
     {
         "InputSecurityGroups": List[InputSecurityGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInputSecurityGroupResponseTypeDef = TypedDict(
     "UpdateInputSecurityGroupResponseTypeDef",
     {
         "SecurityGroup": InputSecurityGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ArchiveContainerSettingsTypeDef = TypedDict(
     "ArchiveContainerSettingsTypeDef",
     {
         "M2tsSettings": M2tsSettingsTypeDef,
@@ -4175,15 +4180,15 @@
         "Name": str,
         "RoleArn": str,
         "SecurityGroups": List[str],
         "Sources": List[InputSourceTypeDef],
         "State": InputStateType,
         "Tags": Dict[str, str],
         "Type": InputTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputTypeDef = TypedDict(
     "InputTypeDef",
     {
         "Arn": str,
@@ -4226,15 +4231,15 @@
         "Id": str,
         "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMultiplexResponseTypeDef = TypedDict(
     "DescribeMultiplexResponseTypeDef",
     {
         "Arn": str,
@@ -4243,15 +4248,15 @@
         "Id": str,
         "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MultiplexTypeDef = TypedDict(
     "MultiplexTypeDef",
     {
         "Arn": str,
@@ -4277,15 +4282,15 @@
         "Id": str,
         "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopMultiplexResponseTypeDef = TypedDict(
     "StopMultiplexResponseTypeDef",
     {
         "Arn": str,
@@ -4294,24 +4299,24 @@
         "Id": str,
         "MultiplexSettings": MultiplexSettingsTypeDef,
         "Name": str,
         "PipelinesRunningCount": int,
         "ProgramCount": int,
         "State": MultiplexStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMultiplexesResponseTypeDef = TypedDict(
     "ListMultiplexesResponseTypeDef",
     {
         "Multiplexes": List[MultiplexSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMultiplexProgramSettingsTypeDef = TypedDict(
     "_RequiredMultiplexProgramSettingsTypeDef",
     {
         "ProgramNumber": int,
@@ -4568,40 +4573,40 @@
     total=False,
 )
 
 CreateInputResponseTypeDef = TypedDict(
     "CreateInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePartnerInputResponseTypeDef = TypedDict(
     "CreatePartnerInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "Inputs": List[InputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInputResponseTypeDef = TypedDict(
     "UpdateInputResponseTypeDef",
     {
         "Input": InputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredHlsOutputSettingsTypeDef = TypedDict(
     "_RequiredHlsOutputSettingsTypeDef",
     {
         "HlsSettings": HlsSettingsTypeDef,
@@ -4622,23 +4627,23 @@
 ):
     pass
 
 CreateMultiplexResponseTypeDef = TypedDict(
     "CreateMultiplexResponseTypeDef",
     {
         "Multiplex": MultiplexTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMultiplexResponseTypeDef = TypedDict(
     "UpdateMultiplexResponseTypeDef",
     {
         "Multiplex": MultiplexTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMultiplexProgramRequestRequestTypeDef = TypedDict(
     "CreateMultiplexProgramRequestRequestTypeDef",
     {
         "MultiplexId": str,
@@ -4652,27 +4657,27 @@
     "DeleteMultiplexProgramResponseTypeDef",
     {
         "ChannelId": str,
         "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMultiplexProgramResponseTypeDef = TypedDict(
     "DescribeMultiplexProgramResponseTypeDef",
     {
         "ChannelId": str,
         "MultiplexProgramSettings": MultiplexProgramSettingsTypeDef,
         "PacketIdentifiersMap": MultiplexProgramPacketIdentifiersMapTypeDef,
         "PipelineDetails": List[MultiplexProgramPipelineDetailTypeDef],
         "ProgramName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MultiplexProgramTypeDef = TypedDict(
     "MultiplexProgramTypeDef",
     {
         "ChannelId": str,
@@ -4808,23 +4813,23 @@
     total=False,
 )
 
 CreateMultiplexProgramResponseTypeDef = TypedDict(
     "CreateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMultiplexProgramResponseTypeDef = TypedDict(
     "UpdateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 Scte35TimeSignalScheduleActionSettingsTypeDef = TypedDict(
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
     {
         "Scte35Descriptors": Sequence[Scte35DescriptorTypeDef],
@@ -4933,15 +4938,15 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEncoderSettingsTypeDef = TypedDict(
     "_RequiredEncoderSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
@@ -4990,15 +4995,15 @@
 )
 
 DescribeScheduleResponseTypeDef = TypedDict(
     "DescribeScheduleResponseTypeDef",
     {
         "NextToken": str,
         "ScheduleActions": List[ScheduleActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Arn": str,
@@ -5061,15 +5066,15 @@
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
@@ -5086,15 +5091,15 @@
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartChannelResponseTypeDef = TypedDict(
     "StartChannelResponseTypeDef",
     {
         "Arn": str,
@@ -5111,15 +5116,15 @@
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopChannelResponseTypeDef = TypedDict(
     "StopChannelResponseTypeDef",
     {
         "Arn": str,
@@ -5136,15 +5141,15 @@
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
@@ -5193,34 +5198,34 @@
     pass
 
 BatchUpdateScheduleResponseTypeDef = TypedDict(
     "BatchUpdateScheduleResponseTypeDef",
     {
         "Creates": BatchScheduleActionCreateResultTypeDef,
         "Deletes": BatchScheduleActionDeleteResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelClassResponseTypeDef = TypedDict(
     "UpdateChannelClassResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/waiter.py` & `mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.26.84/mypy_boto3_medialive/waiter.pyi` & `mypy-boto3-medialive-1.27.0/mypy_boto3_medialive/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.26.84/mypy_boto3_medialive.egg-info/PKG-INFO` & `mypy-boto3-medialive-1.27.0/mypy_boto3_medialive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.26.84
-Summary: Type annotations for boto3.MediaLive 1.26.84 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.MediaLive 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-medialive"></a>
 
 # mypy-boto3-medialive
 
 [![PyPI - mypy-boto3-medialive](https://img.shields.io/pypi/v/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-medialive?color=blue)](https://pypistats.org/packages/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.26.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
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
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
 See how it helps to find and fix potential bugs:
 
@@ -697,15 +697,14 @@
     AudioTrackTypeDef,
     EsamTypeDef,
     Scte35SpliceInsertTypeDef,
     Scte35TimeSignalAposTypeDef,
     BatchDeleteRequestRequestTypeDef,
     BatchFailedResultModelTypeDef,
     BatchSuccessfulResultModelTypeDef,
-    ResponseMetadataTypeDef,
     BatchScheduleActionDeleteRequestTypeDef,
     BatchStartRequestRequestTypeDef,
     BatchStopRequestRequestTypeDef,
     CancelInputDeviceTransferRequestRequestTypeDef,
     EbuTtDDestinationSettingsTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
@@ -748,28 +747,30 @@
     WaiterConfigTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeInputDeviceRequestRequestTypeDef,
     InputDeviceHdSettingsTypeDef,
     InputDeviceNetworkSettingsTypeDef,
     InputDeviceUhdSettingsTypeDef,
     DescribeInputDeviceThumbnailRequestRequestTypeDef,
+    DescribeInputDeviceThumbnailResponseTypeDef,
     DescribeInputRequestRequestTypeDef,
     InputSourceTypeDef,
     MediaConnectFlowTypeDef,
     DescribeInputSecurityGroupRequestRequestTypeDef,
     InputWhitelistRuleTypeDef,
     DescribeMultiplexProgramRequestRequestTypeDef,
     DescribeMultiplexRequestRequestTypeDef,
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
     DescribeScheduleRequestRequestTypeDef,
     DvbNitSettingsTypeDef,
     DvbSdtSettingsTypeDef,
     DvbTdtSettingsTypeDef,
+    EmptyResponseMetadataTypeDef,
     FeatureActivationsTypeDef,
     NielsenConfigurationTypeDef,
     TimecodeConfigTypeDef,
     InputLossFailoverSettingsTypeDef,
     VideoBlackFailoverSettingsTypeDef,
     FecOutputSettingsTypeDef,
     FixedModeScheduleActionStartSettingsTypeDef,
@@ -790,26 +791,36 @@
     HlsInputSettingsTypeDef,
     HlsTimedMetadataScheduleActionSettingsTypeDef,
     StartTimecodeTypeDef,
     StopTimecodeTypeDef,
     InputDestinationVpcTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
+    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
     ListInputDeviceTransfersRequestRequestTypeDef,
     TransferringInputDeviceSummaryTypeDef,
+    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
     ListInputDevicesRequestRequestTypeDef,
+    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
     ListInputSecurityGroupsRequestRequestTypeDef,
+    ListInputsRequestListInputsPaginateTypeDef,
     ListInputsRequestRequestTypeDef,
+    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
     ListMultiplexProgramsRequestRequestTypeDef,
     MultiplexProgramSummaryTypeDef,
+    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
     ListMultiplexesRequestRequestTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
+    ListReservationsRequestListReservationsPaginateTypeDef,
     ListReservationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     M3u8SettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
     MediaPackageOutputDestinationSettingsTypeDef,
     MotionGraphicsActivateScheduleActionSettingsTypeDef,
     MotionGraphicsSettingsTypeDef,
     MsSmoothOutputSettingsTypeDef,
     MultiplexMediaConnectOutputDestinationSettingsTypeDef,
@@ -818,17 +829,19 @@
     MultiplexSettingsSummaryTypeDef,
     MultiplexStatmuxVideoSettingsTypeDef,
     NielsenCBETTypeDef,
     NielsenNaesIiNwTypeDef,
     OutputDestinationSettingsTypeDef,
     RtmpGroupSettingsTypeDef,
     UdpGroupSettingsTypeDef,
+    PaginatorConfigTypeDef,
     PipelinePauseStateSettingsTypeDef,
     RebootInputDeviceRequestRequestTypeDef,
     RejectInputDeviceTransferRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     Scte35InputScheduleActionSettingsTypeDef,
     Scte35ReturnToNetworkScheduleActionSettingsTypeDef,
     Scte35SpliceInsertScheduleActionSettingsTypeDef,
     StaticImageDeactivateScheduleActionSettingsTypeDef,
     Scte35DeliveryRestrictionsTypeDef,
     StartChannelRequestRequestTypeDef,
     StartInputDeviceMaintenanceWindowRequestRequestTypeDef,
@@ -854,17 +867,14 @@
     StaticImageActivateScheduleActionSettingsTypeDef,
     StaticKeySettingsTypeDef,
     AudioTrackSelectionTypeDef,
     AvailSettingsTypeDef,
     BatchDeleteResponseTypeDef,
     BatchStartResponseTypeDef,
     BatchStopResponseTypeDef,
-    DescribeInputDeviceThumbnailResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TeletextSourceSettingsTypeDef,
     CreateInputRequestRequestTypeDef,
     CreateInputSecurityGroupRequestRequestTypeDef,
     UpdateInputSecurityGroupRequestRequestTypeDef,
     CreateMultiplexRequestRequestTypeDef,
     UpdateMultiplexRequestRequestTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
@@ -886,24 +896,14 @@
     DescribeMultiplexRequestMultiplexRunningWaitTypeDef,
     DescribeMultiplexRequestMultiplexStoppedWaitTypeDef,
     DescribeInputDeviceResponseTypeDef,
     InputDeviceSummaryTypeDef,
     UpdateInputDeviceResponseTypeDef,
     DescribeInputSecurityGroupResponseTypeDef,
     InputSecurityGroupTypeDef,
-    DescribeScheduleRequestDescribeSchedulePaginateTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
-    ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef,
-    ListInputDevicesRequestListInputDevicesPaginateTypeDef,
-    ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef,
-    ListInputsRequestListInputsPaginateTypeDef,
-    ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef,
-    ListMultiplexesRequestListMultiplexesPaginateTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
-    ListReservationsRequestListReservationsPaginateTypeDef,
     M2tsSettingsTypeDef,
     FailoverConditionSettingsTypeDef,
     ScheduleActionStartSettingsTypeDef,
     FrameCaptureCdnSettingsTypeDef,
     FrameCaptureSettingsTypeDef,
     H264FilterSettingsTypeDef,
     H265FilterSettingsTypeDef,
@@ -1030,42 +1030,42 @@
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

### Comparing `mypy-boto3-medialive-1.26.84/mypy_boto3_medialive.egg-info/SOURCES.txt` & `mypy-boto3-medialive-1.27.0/mypy_boto3_medialive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.26.84/setup.py` & `mypy-boto3-medialive-1.27.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-medialive.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-medialive",
-    version="1.26.84",
+    version="1.27.0",
     packages=["mypy_boto3_medialive"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaLive 1.26.84 service generated with mypy-boto3-builder"
-        " 7.12.5"
+        "Type annotations for boto3.MediaLive 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/",
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


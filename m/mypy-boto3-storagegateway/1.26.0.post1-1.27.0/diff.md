# Comparing `tmp/mypy-boto3-storagegateway-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-storagegateway-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-storagegateway-1.26.0.post1.tar", last modified: Tue Nov  1 21:44:03 2022, max compression
+gzip compressed data, was "mypy-boto3-storagegateway-1.27.0.tar", last modified: Mon Jul  3 19:51:32 2023, max compression
```

## Comparing `mypy-boto3-storagegateway-1.26.0.post1.tar` & `mypy-boto3-storagegateway-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:03.788853 mypy-boto3-storagegateway-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:41:55.000000 mypy-boto3-storagegateway-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    23996 2022-11-01 21:44:03.784852 mypy-boto3-storagegateway-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    22527 2022-11-01 21:41:55.000000 mypy-boto3-storagegateway-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:03.784852 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/
--rw-r--r--   0 runner    (1001) docker     (121)     2740 2022-11-01 21:41:55.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2739 2022-11-01 21:41:55.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-11-01 21:41:55.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    68221 2022-11-01 21:41:56.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    68113 2022-11-01 21:41:56.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10006 2022-11-01 21:41:58.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    10004 2022-11-01 21:41:58.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13146 2022-11-01 21:41:56.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    13133 2022-11-01 21:41:56.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:41:55.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    76726 2022-11-01 21:42:00.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    76649 2022-11-01 21:41:59.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:41:55.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:03.784852 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    23996 2022-11-01 21:44:03.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-11-01 21:44:03.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:03.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:03.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:44:03.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-01 21:44:03.000000 mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:44:03.788853 mypy-boto3-storagegateway-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-11-01 21:41:55.000000 mypy-boto3-storagegateway-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:32.076074 mypy-boto3-storagegateway-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:51.000000 mypy-boto3-storagegateway-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24025 2023-07-03 19:51:32.072074 mypy-boto3-storagegateway-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22512 2023-07-03 19:48:51.000000 mypy-boto3-storagegateway-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:32.072074 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-03 19:48:51.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-03 19:48:51.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 19:48:51.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68220 2023-07-03 19:48:52.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68112 2023-07-03 19:48:51.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-07-03 19:48:52.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-07-03 19:48:52.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-07-03 19:48:52.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-07-03 19:48:52.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:51.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    76928 2023-07-03 19:48:53.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76851 2023-07-03 19:48:53.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:51.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:32.072074 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24025 2023-07-03 19:51:31.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 19:51:31.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:31.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:31.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:31.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:51:31.000000 mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:32.076074 mypy-boto3-storagegateway-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-03 19:48:51.000000 mypy-boto3-storagegateway-1.27.0/setup.py
```

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/LICENSE` & `mypy-boto3-storagegateway-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/PKG-INFO` & `mypy-boto3-storagegateway-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-storagegateway
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.StorageGateway 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.StorageGateway 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/
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
 
 <a id="mypy-boto3-storagegateway"></a>
 
 # mypy-boto3-storagegateway
 
 [![PyPI - mypy-boto3-storagegateway](https://img.shields.io/pypi/v/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-storagegateway?color=blue)](https://pypistats.org/packages/mypy-boto3-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.StorageGateway 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[boto3.StorageGateway 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -373,187 +374,198 @@
 
 `mypy_boto3_storagegateway.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_storagegateway.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    ActivateGatewayOutputTypeDef,
     AddCacheInputRequestTypeDef,
+    AddCacheOutputTypeDef,
+    AddTagsToResourceOutputTypeDef,
     AddUploadBufferInputRequestTypeDef,
+    AddUploadBufferOutputTypeDef,
     AddWorkingStorageInputRequestTypeDef,
+    AddWorkingStorageOutputTypeDef,
     AssignTapePoolInputRequestTypeDef,
+    AssignTapePoolOutputTypeDef,
     CacheAttributesTypeDef,
     EndpointNetworkConfigurationTypeDef,
+    AssociateFileSystemOutputTypeDef,
     AttachVolumeInputRequestTypeDef,
+    AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     VolumeiSCSIAttributesTypeDef,
     CancelArchivalInputRequestTypeDef,
+    CancelArchivalOutputTypeDef,
     CancelRetrievalInputRequestTypeDef,
+    CancelRetrievalOutputTypeDef,
     ChapInfoTypeDef,
+    CreateCachediSCSIVolumeOutputTypeDef,
     NFSFileShareDefaultsTypeDef,
+    CreateNFSFileShareOutputTypeDef,
+    CreateSMBFileShareOutputTypeDef,
+    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
+    CreateSnapshotOutputTypeDef,
+    CreateStorediSCSIVolumeOutputTypeDef,
+    CreateTapePoolOutputTypeDef,
+    CreateTapeWithBarcodeOutputTypeDef,
+    CreateTapesOutputTypeDef,
     DeleteAutomaticTapeCreationPolicyInputRequestTypeDef,
+    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
     DeleteBandwidthRateLimitInputRequestTypeDef,
+    DeleteBandwidthRateLimitOutputTypeDef,
     DeleteChapCredentialsInputRequestTypeDef,
+    DeleteChapCredentialsOutputTypeDef,
     DeleteFileShareInputRequestTypeDef,
+    DeleteFileShareOutputTypeDef,
     DeleteGatewayInputRequestTypeDef,
+    DeleteGatewayOutputTypeDef,
     DeleteSnapshotScheduleInputRequestTypeDef,
+    DeleteSnapshotScheduleOutputTypeDef,
     DeleteTapeArchiveInputRequestTypeDef,
+    DeleteTapeArchiveOutputTypeDef,
     DeleteTapeInputRequestTypeDef,
+    DeleteTapeOutputTypeDef,
     DeleteTapePoolInputRequestTypeDef,
+    DeleteTapePoolOutputTypeDef,
     DeleteVolumeInputRequestTypeDef,
+    DeleteVolumeOutputTypeDef,
     DescribeAvailabilityMonitorTestInputRequestTypeDef,
+    DescribeAvailabilityMonitorTestOutputTypeDef,
     DescribeBandwidthRateLimitInputRequestTypeDef,
+    DescribeBandwidthRateLimitOutputTypeDef,
     DescribeBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCacheInputRequestTypeDef,
+    DescribeCacheOutputTypeDef,
     DescribeCachediSCSIVolumesInputRequestTypeDef,
     DescribeChapCredentialsInputRequestTypeDef,
     DescribeFileSystemAssociationsInputRequestTypeDef,
     DescribeGatewayInformationInputRequestTypeDef,
     NetworkInterfaceTypeDef,
     DescribeMaintenanceStartTimeInputRequestTypeDef,
+    DescribeMaintenanceStartTimeOutputTypeDef,
     DescribeNFSFileSharesInputRequestTypeDef,
     DescribeSMBFileSharesInputRequestTypeDef,
     DescribeSMBSettingsInputRequestTypeDef,
     SMBLocalGroupsTypeDef,
     DescribeSnapshotScheduleInputRequestTypeDef,
     DescribeStorediSCSIVolumesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
     DescribeTapeArchivesInputRequestTypeDef,
     TapeArchiveTypeDef,
+    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
     DescribeTapeRecoveryPointsInputRequestTypeDef,
     TapeRecoveryPointInfoTypeDef,
+    DescribeTapesInputDescribeTapesPaginateTypeDef,
     DescribeTapesInputRequestTypeDef,
     TapeTypeDef,
     DescribeUploadBufferInputRequestTypeDef,
+    DescribeUploadBufferOutputTypeDef,
+    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
     DescribeVTLDevicesInputRequestTypeDef,
     DescribeWorkingStorageInputRequestTypeDef,
+    DescribeWorkingStorageOutputTypeDef,
     DetachVolumeInputRequestTypeDef,
+    DetachVolumeOutputTypeDef,
     DeviceiSCSIAttributesTypeDef,
     DisableGatewayInputRequestTypeDef,
+    DisableGatewayOutputTypeDef,
     DisassociateFileSystemInputRequestTypeDef,
+    DisassociateFileSystemOutputTypeDef,
     DiskTypeDef,
     FileShareInfoTypeDef,
     FileSystemAssociationStatusDetailTypeDef,
     FileSystemAssociationSummaryTypeDef,
     GatewayInfoTypeDef,
     JoinDomainInputRequestTypeDef,
+    JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesInputRequestTypeDef,
+    ListFileSharesInputListFileSharesPaginateTypeDef,
     ListFileSharesInputRequestTypeDef,
+    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
     ListFileSystemAssociationsInputRequestTypeDef,
+    ListGatewaysInputListGatewaysPaginateTypeDef,
     ListGatewaysInputRequestTypeDef,
     ListLocalDisksInputRequestTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTapePoolsInputListTapePoolsPaginateTypeDef,
     ListTapePoolsInputRequestTypeDef,
     PoolInfoTypeDef,
+    ListTapesInputListTapesPaginateTypeDef,
     ListTapesInputRequestTypeDef,
     TapeInfoTypeDef,
     ListVolumeInitiatorsInputRequestTypeDef,
+    ListVolumeInitiatorsOutputTypeDef,
     ListVolumeRecoveryPointsInputRequestTypeDef,
     VolumeRecoveryPointInfoTypeDef,
+    ListVolumesInputListVolumesPaginateTypeDef,
     ListVolumesInputRequestTypeDef,
     VolumeInfoTypeDef,
     NotifyWhenUploadedInputRequestTypeDef,
+    NotifyWhenUploadedOutputTypeDef,
+    PaginatorConfigTypeDef,
     RefreshCacheInputRequestTypeDef,
+    RefreshCacheOutputTypeDef,
     RemoveTagsFromResourceInputRequestTypeDef,
+    RemoveTagsFromResourceOutputTypeDef,
     ResetCacheInputRequestTypeDef,
+    ResetCacheOutputTypeDef,
+    ResponseMetadataTypeDef,
     RetrieveTapeArchiveInputRequestTypeDef,
+    RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointInputRequestTypeDef,
+    RetrieveTapeRecoveryPointOutputTypeDef,
     SetLocalConsolePasswordInputRequestTypeDef,
+    SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordInputRequestTypeDef,
+    SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayInputRequestTypeDef,
+    ShutdownGatewayOutputTypeDef,
     StartAvailabilityMonitorTestInputRequestTypeDef,
+    StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayInputRequestTypeDef,
+    StartGatewayOutputTypeDef,
+    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitInputRequestTypeDef,
+    UpdateBandwidthRateLimitOutputTypeDef,
+    UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsInputRequestTypeDef,
+    UpdateChapCredentialsOutputTypeDef,
+    UpdateFileSystemAssociationOutputTypeDef,
     UpdateGatewayInformationInputRequestTypeDef,
+    UpdateGatewayInformationOutputTypeDef,
     UpdateGatewaySoftwareNowInputRequestTypeDef,
+    UpdateGatewaySoftwareNowOutputTypeDef,
     UpdateMaintenanceStartTimeInputRequestTypeDef,
+    UpdateMaintenanceStartTimeOutputTypeDef,
+    UpdateNFSFileShareOutputTypeDef,
+    UpdateSMBFileShareOutputTypeDef,
     UpdateSMBFileShareVisibilityInputRequestTypeDef,
+    UpdateSMBFileShareVisibilityOutputTypeDef,
+    UpdateSMBLocalGroupsOutputTypeDef,
     UpdateSMBSecurityStrategyInputRequestTypeDef,
+    UpdateSMBSecurityStrategyOutputTypeDef,
+    UpdateSnapshotScheduleOutputTypeDef,
     UpdateVTLDeviceTypeInputRequestTypeDef,
+    UpdateVTLDeviceTypeOutputTypeDef,
     ActivateGatewayInputRequestTypeDef,
     AddTagsToResourceInputRequestTypeDef,
     CreateCachediSCSIVolumeInputRequestTypeDef,
     CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef,
     CreateSnapshotInputRequestTypeDef,
     CreateStorediSCSIVolumeInputRequestTypeDef,
     CreateTapePoolInputRequestTypeDef,
     CreateTapeWithBarcodeInputRequestTypeDef,
     CreateTapesInputRequestTypeDef,
-    UpdateSnapshotScheduleInputRequestTypeDef,
-    ActivateGatewayOutputTypeDef,
-    AddCacheOutputTypeDef,
-    AddTagsToResourceOutputTypeDef,
-    AddUploadBufferOutputTypeDef,
-    AddWorkingStorageOutputTypeDef,
-    AssignTapePoolOutputTypeDef,
-    AssociateFileSystemOutputTypeDef,
-    AttachVolumeOutputTypeDef,
-    CancelArchivalOutputTypeDef,
-    CancelRetrievalOutputTypeDef,
-    CreateCachediSCSIVolumeOutputTypeDef,
-    CreateNFSFileShareOutputTypeDef,
-    CreateSMBFileShareOutputTypeDef,
-    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
-    CreateSnapshotOutputTypeDef,
-    CreateStorediSCSIVolumeOutputTypeDef,
-    CreateTapePoolOutputTypeDef,
-    CreateTapeWithBarcodeOutputTypeDef,
-    CreateTapesOutputTypeDef,
-    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
-    DeleteBandwidthRateLimitOutputTypeDef,
-    DeleteChapCredentialsOutputTypeDef,
-    DeleteFileShareOutputTypeDef,
-    DeleteGatewayOutputTypeDef,
-    DeleteSnapshotScheduleOutputTypeDef,
-    DeleteTapeArchiveOutputTypeDef,
-    DeleteTapeOutputTypeDef,
-    DeleteTapePoolOutputTypeDef,
-    DeleteVolumeOutputTypeDef,
-    DescribeAvailabilityMonitorTestOutputTypeDef,
-    DescribeBandwidthRateLimitOutputTypeDef,
-    DescribeCacheOutputTypeDef,
-    DescribeMaintenanceStartTimeOutputTypeDef,
     DescribeSnapshotScheduleOutputTypeDef,
-    DescribeUploadBufferOutputTypeDef,
-    DescribeWorkingStorageOutputTypeDef,
-    DetachVolumeOutputTypeDef,
-    DisableGatewayOutputTypeDef,
-    DisassociateFileSystemOutputTypeDef,
-    JoinDomainOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    ListVolumeInitiatorsOutputTypeDef,
-    NotifyWhenUploadedOutputTypeDef,
-    RefreshCacheOutputTypeDef,
-    RemoveTagsFromResourceOutputTypeDef,
-    ResetCacheOutputTypeDef,
-    RetrieveTapeArchiveOutputTypeDef,
-    RetrieveTapeRecoveryPointOutputTypeDef,
-    SetLocalConsolePasswordOutputTypeDef,
-    SetSMBGuestPasswordOutputTypeDef,
-    ShutdownGatewayOutputTypeDef,
-    StartAvailabilityMonitorTestOutputTypeDef,
-    StartGatewayOutputTypeDef,
-    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
-    UpdateBandwidthRateLimitOutputTypeDef,
-    UpdateBandwidthRateLimitScheduleOutputTypeDef,
-    UpdateChapCredentialsOutputTypeDef,
-    UpdateFileSystemAssociationOutputTypeDef,
-    UpdateGatewayInformationOutputTypeDef,
-    UpdateGatewaySoftwareNowOutputTypeDef,
-    UpdateMaintenanceStartTimeOutputTypeDef,
-    UpdateNFSFileShareOutputTypeDef,
-    UpdateSMBFileShareOutputTypeDef,
-    UpdateSMBFileShareVisibilityOutputTypeDef,
-    UpdateSMBLocalGroupsOutputTypeDef,
-    UpdateSMBSecurityStrategyOutputTypeDef,
-    UpdateSnapshotScheduleOutputTypeDef,
-    UpdateVTLDeviceTypeOutputTypeDef,
+    UpdateSnapshotScheduleInputRequestTypeDef,
     CreateSMBFileShareInputRequestTypeDef,
     SMBFileShareInfoTypeDef,
     UpdateFileSystemAssociationInputRequestTypeDef,
     UpdateSMBFileShareInputRequestTypeDef,
     AssociateFileSystemInputRequestTypeDef,
     AutomaticTapeCreationPolicyInfoTypeDef,
     UpdateAutomaticTapeCreationPolicyInputRequestTypeDef,
@@ -564,25 +576,14 @@
     DescribeChapCredentialsOutputTypeDef,
     CreateNFSFileShareInputRequestTypeDef,
     NFSFileShareInfoTypeDef,
     UpdateNFSFileShareInputRequestTypeDef,
     DescribeGatewayInformationOutputTypeDef,
     DescribeSMBSettingsOutputTypeDef,
     UpdateSMBLocalGroupsInputRequestTypeDef,
-    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
-    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
-    DescribeTapesInputDescribeTapesPaginateTypeDef,
-    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
-    ListFileSharesInputListFileSharesPaginateTypeDef,
-    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ListTapePoolsInputListTapePoolsPaginateTypeDef,
-    ListTapesInputListTapesPaginateTypeDef,
-    ListVolumesInputListVolumesPaginateTypeDef,
     DescribeTapeArchivesOutputTypeDef,
     DescribeTapeRecoveryPointsOutputTypeDef,
     DescribeTapesOutputTypeDef,
     VTLDeviceTypeDef,
     ListLocalDisksOutputTypeDef,
     ListFileSharesOutputTypeDef,
     FileSystemAssociationInfoTypeDef,
@@ -609,42 +610,42 @@
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

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/README.md` & `mypy-boto3-storagegateway-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-storagegateway"></a>
 
 # mypy-boto3-storagegateway
 
 [![PyPI - mypy-boto3-storagegateway](https://img.shields.io/pypi/v/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-storagegateway?color=blue)](https://pypistats.org/packages/mypy-boto3-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.StorageGateway 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[boto3.StorageGateway 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,187 +342,198 @@
 
 `mypy_boto3_storagegateway.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_storagegateway.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    ActivateGatewayOutputTypeDef,
     AddCacheInputRequestTypeDef,
+    AddCacheOutputTypeDef,
+    AddTagsToResourceOutputTypeDef,
     AddUploadBufferInputRequestTypeDef,
+    AddUploadBufferOutputTypeDef,
     AddWorkingStorageInputRequestTypeDef,
+    AddWorkingStorageOutputTypeDef,
     AssignTapePoolInputRequestTypeDef,
+    AssignTapePoolOutputTypeDef,
     CacheAttributesTypeDef,
     EndpointNetworkConfigurationTypeDef,
+    AssociateFileSystemOutputTypeDef,
     AttachVolumeInputRequestTypeDef,
+    AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     VolumeiSCSIAttributesTypeDef,
     CancelArchivalInputRequestTypeDef,
+    CancelArchivalOutputTypeDef,
     CancelRetrievalInputRequestTypeDef,
+    CancelRetrievalOutputTypeDef,
     ChapInfoTypeDef,
+    CreateCachediSCSIVolumeOutputTypeDef,
     NFSFileShareDefaultsTypeDef,
+    CreateNFSFileShareOutputTypeDef,
+    CreateSMBFileShareOutputTypeDef,
+    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
+    CreateSnapshotOutputTypeDef,
+    CreateStorediSCSIVolumeOutputTypeDef,
+    CreateTapePoolOutputTypeDef,
+    CreateTapeWithBarcodeOutputTypeDef,
+    CreateTapesOutputTypeDef,
     DeleteAutomaticTapeCreationPolicyInputRequestTypeDef,
+    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
     DeleteBandwidthRateLimitInputRequestTypeDef,
+    DeleteBandwidthRateLimitOutputTypeDef,
     DeleteChapCredentialsInputRequestTypeDef,
+    DeleteChapCredentialsOutputTypeDef,
     DeleteFileShareInputRequestTypeDef,
+    DeleteFileShareOutputTypeDef,
     DeleteGatewayInputRequestTypeDef,
+    DeleteGatewayOutputTypeDef,
     DeleteSnapshotScheduleInputRequestTypeDef,
+    DeleteSnapshotScheduleOutputTypeDef,
     DeleteTapeArchiveInputRequestTypeDef,
+    DeleteTapeArchiveOutputTypeDef,
     DeleteTapeInputRequestTypeDef,
+    DeleteTapeOutputTypeDef,
     DeleteTapePoolInputRequestTypeDef,
+    DeleteTapePoolOutputTypeDef,
     DeleteVolumeInputRequestTypeDef,
+    DeleteVolumeOutputTypeDef,
     DescribeAvailabilityMonitorTestInputRequestTypeDef,
+    DescribeAvailabilityMonitorTestOutputTypeDef,
     DescribeBandwidthRateLimitInputRequestTypeDef,
+    DescribeBandwidthRateLimitOutputTypeDef,
     DescribeBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCacheInputRequestTypeDef,
+    DescribeCacheOutputTypeDef,
     DescribeCachediSCSIVolumesInputRequestTypeDef,
     DescribeChapCredentialsInputRequestTypeDef,
     DescribeFileSystemAssociationsInputRequestTypeDef,
     DescribeGatewayInformationInputRequestTypeDef,
     NetworkInterfaceTypeDef,
     DescribeMaintenanceStartTimeInputRequestTypeDef,
+    DescribeMaintenanceStartTimeOutputTypeDef,
     DescribeNFSFileSharesInputRequestTypeDef,
     DescribeSMBFileSharesInputRequestTypeDef,
     DescribeSMBSettingsInputRequestTypeDef,
     SMBLocalGroupsTypeDef,
     DescribeSnapshotScheduleInputRequestTypeDef,
     DescribeStorediSCSIVolumesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
     DescribeTapeArchivesInputRequestTypeDef,
     TapeArchiveTypeDef,
+    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
     DescribeTapeRecoveryPointsInputRequestTypeDef,
     TapeRecoveryPointInfoTypeDef,
+    DescribeTapesInputDescribeTapesPaginateTypeDef,
     DescribeTapesInputRequestTypeDef,
     TapeTypeDef,
     DescribeUploadBufferInputRequestTypeDef,
+    DescribeUploadBufferOutputTypeDef,
+    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
     DescribeVTLDevicesInputRequestTypeDef,
     DescribeWorkingStorageInputRequestTypeDef,
+    DescribeWorkingStorageOutputTypeDef,
     DetachVolumeInputRequestTypeDef,
+    DetachVolumeOutputTypeDef,
     DeviceiSCSIAttributesTypeDef,
     DisableGatewayInputRequestTypeDef,
+    DisableGatewayOutputTypeDef,
     DisassociateFileSystemInputRequestTypeDef,
+    DisassociateFileSystemOutputTypeDef,
     DiskTypeDef,
     FileShareInfoTypeDef,
     FileSystemAssociationStatusDetailTypeDef,
     FileSystemAssociationSummaryTypeDef,
     GatewayInfoTypeDef,
     JoinDomainInputRequestTypeDef,
+    JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesInputRequestTypeDef,
+    ListFileSharesInputListFileSharesPaginateTypeDef,
     ListFileSharesInputRequestTypeDef,
+    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
     ListFileSystemAssociationsInputRequestTypeDef,
+    ListGatewaysInputListGatewaysPaginateTypeDef,
     ListGatewaysInputRequestTypeDef,
     ListLocalDisksInputRequestTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTapePoolsInputListTapePoolsPaginateTypeDef,
     ListTapePoolsInputRequestTypeDef,
     PoolInfoTypeDef,
+    ListTapesInputListTapesPaginateTypeDef,
     ListTapesInputRequestTypeDef,
     TapeInfoTypeDef,
     ListVolumeInitiatorsInputRequestTypeDef,
+    ListVolumeInitiatorsOutputTypeDef,
     ListVolumeRecoveryPointsInputRequestTypeDef,
     VolumeRecoveryPointInfoTypeDef,
+    ListVolumesInputListVolumesPaginateTypeDef,
     ListVolumesInputRequestTypeDef,
     VolumeInfoTypeDef,
     NotifyWhenUploadedInputRequestTypeDef,
+    NotifyWhenUploadedOutputTypeDef,
+    PaginatorConfigTypeDef,
     RefreshCacheInputRequestTypeDef,
+    RefreshCacheOutputTypeDef,
     RemoveTagsFromResourceInputRequestTypeDef,
+    RemoveTagsFromResourceOutputTypeDef,
     ResetCacheInputRequestTypeDef,
+    ResetCacheOutputTypeDef,
+    ResponseMetadataTypeDef,
     RetrieveTapeArchiveInputRequestTypeDef,
+    RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointInputRequestTypeDef,
+    RetrieveTapeRecoveryPointOutputTypeDef,
     SetLocalConsolePasswordInputRequestTypeDef,
+    SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordInputRequestTypeDef,
+    SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayInputRequestTypeDef,
+    ShutdownGatewayOutputTypeDef,
     StartAvailabilityMonitorTestInputRequestTypeDef,
+    StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayInputRequestTypeDef,
+    StartGatewayOutputTypeDef,
+    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitInputRequestTypeDef,
+    UpdateBandwidthRateLimitOutputTypeDef,
+    UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsInputRequestTypeDef,
+    UpdateChapCredentialsOutputTypeDef,
+    UpdateFileSystemAssociationOutputTypeDef,
     UpdateGatewayInformationInputRequestTypeDef,
+    UpdateGatewayInformationOutputTypeDef,
     UpdateGatewaySoftwareNowInputRequestTypeDef,
+    UpdateGatewaySoftwareNowOutputTypeDef,
     UpdateMaintenanceStartTimeInputRequestTypeDef,
+    UpdateMaintenanceStartTimeOutputTypeDef,
+    UpdateNFSFileShareOutputTypeDef,
+    UpdateSMBFileShareOutputTypeDef,
     UpdateSMBFileShareVisibilityInputRequestTypeDef,
+    UpdateSMBFileShareVisibilityOutputTypeDef,
+    UpdateSMBLocalGroupsOutputTypeDef,
     UpdateSMBSecurityStrategyInputRequestTypeDef,
+    UpdateSMBSecurityStrategyOutputTypeDef,
+    UpdateSnapshotScheduleOutputTypeDef,
     UpdateVTLDeviceTypeInputRequestTypeDef,
+    UpdateVTLDeviceTypeOutputTypeDef,
     ActivateGatewayInputRequestTypeDef,
     AddTagsToResourceInputRequestTypeDef,
     CreateCachediSCSIVolumeInputRequestTypeDef,
     CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef,
     CreateSnapshotInputRequestTypeDef,
     CreateStorediSCSIVolumeInputRequestTypeDef,
     CreateTapePoolInputRequestTypeDef,
     CreateTapeWithBarcodeInputRequestTypeDef,
     CreateTapesInputRequestTypeDef,
-    UpdateSnapshotScheduleInputRequestTypeDef,
-    ActivateGatewayOutputTypeDef,
-    AddCacheOutputTypeDef,
-    AddTagsToResourceOutputTypeDef,
-    AddUploadBufferOutputTypeDef,
-    AddWorkingStorageOutputTypeDef,
-    AssignTapePoolOutputTypeDef,
-    AssociateFileSystemOutputTypeDef,
-    AttachVolumeOutputTypeDef,
-    CancelArchivalOutputTypeDef,
-    CancelRetrievalOutputTypeDef,
-    CreateCachediSCSIVolumeOutputTypeDef,
-    CreateNFSFileShareOutputTypeDef,
-    CreateSMBFileShareOutputTypeDef,
-    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
-    CreateSnapshotOutputTypeDef,
-    CreateStorediSCSIVolumeOutputTypeDef,
-    CreateTapePoolOutputTypeDef,
-    CreateTapeWithBarcodeOutputTypeDef,
-    CreateTapesOutputTypeDef,
-    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
-    DeleteBandwidthRateLimitOutputTypeDef,
-    DeleteChapCredentialsOutputTypeDef,
-    DeleteFileShareOutputTypeDef,
-    DeleteGatewayOutputTypeDef,
-    DeleteSnapshotScheduleOutputTypeDef,
-    DeleteTapeArchiveOutputTypeDef,
-    DeleteTapeOutputTypeDef,
-    DeleteTapePoolOutputTypeDef,
-    DeleteVolumeOutputTypeDef,
-    DescribeAvailabilityMonitorTestOutputTypeDef,
-    DescribeBandwidthRateLimitOutputTypeDef,
-    DescribeCacheOutputTypeDef,
-    DescribeMaintenanceStartTimeOutputTypeDef,
     DescribeSnapshotScheduleOutputTypeDef,
-    DescribeUploadBufferOutputTypeDef,
-    DescribeWorkingStorageOutputTypeDef,
-    DetachVolumeOutputTypeDef,
-    DisableGatewayOutputTypeDef,
-    DisassociateFileSystemOutputTypeDef,
-    JoinDomainOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    ListVolumeInitiatorsOutputTypeDef,
-    NotifyWhenUploadedOutputTypeDef,
-    RefreshCacheOutputTypeDef,
-    RemoveTagsFromResourceOutputTypeDef,
-    ResetCacheOutputTypeDef,
-    RetrieveTapeArchiveOutputTypeDef,
-    RetrieveTapeRecoveryPointOutputTypeDef,
-    SetLocalConsolePasswordOutputTypeDef,
-    SetSMBGuestPasswordOutputTypeDef,
-    ShutdownGatewayOutputTypeDef,
-    StartAvailabilityMonitorTestOutputTypeDef,
-    StartGatewayOutputTypeDef,
-    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
-    UpdateBandwidthRateLimitOutputTypeDef,
-    UpdateBandwidthRateLimitScheduleOutputTypeDef,
-    UpdateChapCredentialsOutputTypeDef,
-    UpdateFileSystemAssociationOutputTypeDef,
-    UpdateGatewayInformationOutputTypeDef,
-    UpdateGatewaySoftwareNowOutputTypeDef,
-    UpdateMaintenanceStartTimeOutputTypeDef,
-    UpdateNFSFileShareOutputTypeDef,
-    UpdateSMBFileShareOutputTypeDef,
-    UpdateSMBFileShareVisibilityOutputTypeDef,
-    UpdateSMBLocalGroupsOutputTypeDef,
-    UpdateSMBSecurityStrategyOutputTypeDef,
-    UpdateSnapshotScheduleOutputTypeDef,
-    UpdateVTLDeviceTypeOutputTypeDef,
+    UpdateSnapshotScheduleInputRequestTypeDef,
     CreateSMBFileShareInputRequestTypeDef,
     SMBFileShareInfoTypeDef,
     UpdateFileSystemAssociationInputRequestTypeDef,
     UpdateSMBFileShareInputRequestTypeDef,
     AssociateFileSystemInputRequestTypeDef,
     AutomaticTapeCreationPolicyInfoTypeDef,
     UpdateAutomaticTapeCreationPolicyInputRequestTypeDef,
@@ -533,25 +544,14 @@
     DescribeChapCredentialsOutputTypeDef,
     CreateNFSFileShareInputRequestTypeDef,
     NFSFileShareInfoTypeDef,
     UpdateNFSFileShareInputRequestTypeDef,
     DescribeGatewayInformationOutputTypeDef,
     DescribeSMBSettingsOutputTypeDef,
     UpdateSMBLocalGroupsInputRequestTypeDef,
-    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
-    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
-    DescribeTapesInputDescribeTapesPaginateTypeDef,
-    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
-    ListFileSharesInputListFileSharesPaginateTypeDef,
-    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ListTapePoolsInputListTapePoolsPaginateTypeDef,
-    ListTapesInputListTapesPaginateTypeDef,
-    ListVolumesInputListVolumesPaginateTypeDef,
     DescribeTapeArchivesOutputTypeDef,
     DescribeTapeRecoveryPointsOutputTypeDef,
     DescribeTapesOutputTypeDef,
     VTLDeviceTypeDef,
     ListLocalDisksOutputTypeDef,
     ListFileSharesOutputTypeDef,
     FileSystemAssociationInfoTypeDef,
@@ -578,42 +578,42 @@
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

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/__init__.py` & `mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/__init__.pyi` & `mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/__main__.py` & `mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.StorageGateway 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.StorageGateway 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway\nOther"
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

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/client.py` & `mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1070,15 +1070,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.start_availability_monitor_test)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#start_availability_monitor_test)
         """
 
     def start_gateway(self, *, GatewayARN: str) -> StartGatewayOutputTypeDef:
         """
-        Starts a gateway that you previously shut down (see  ShutdownGateway ).
+        Starts a gateway that you previously shut down (see  ShutdownGateway).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.start_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#start_gateway)
         """
 
     def update_automatic_tape_creation_policy(
         self,
```

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/client.pyi` & `mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -988,15 +988,15 @@
         Availability monitoring in your host environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.start_availability_monitor_test)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#start_availability_monitor_test)
         """
     def start_gateway(self, *, GatewayARN: str) -> StartGatewayOutputTypeDef:
         """
-        Starts a gateway that you previously shut down (see  ShutdownGateway ).
+        Starts a gateway that you previously shut down (see  ShutdownGateway).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.start_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/client/#start_gateway)
         """
     def update_automatic_tape_creation_policy(
         self,
         *,
```

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/literals.py` & `mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/literals.pyi`

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
     "ActiveDirectoryStatusType",
     "AvailabilityMonitorTestStatusType",
     "CaseSensitivityType",
     "DescribeTapeArchivesPaginatorName",
     "DescribeTapeRecoveryPointsPaginatorName",
     "DescribeTapesPaginatorName",
@@ -45,15 +44,14 @@
     "StorageGatewayServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActiveDirectoryStatusType = Literal[
     "ACCESS_DENIED", "DETACHED", "JOINED", "JOINING", "NETWORK_ERROR", "TIMEOUT", "UNKNOWN_ERROR"
 ]
 AvailabilityMonitorTestStatusType = Literal["COMPLETE", "FAILED", "PENDING"]
 CaseSensitivityType = Literal["CaseSensitive", "ClientSpecified"]
 DescribeTapeArchivesPaginatorName = Literal["describe_tape_archives"]
 DescribeTapeRecoveryPointsPaginatorName = Literal["describe_tape_recovery_points"]
@@ -94,23 +92,25 @@
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
@@ -120,30 +120,35 @@
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
@@ -169,14 +174,15 @@
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
@@ -221,51 +227,57 @@
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
@@ -278,14 +290,15 @@
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
@@ -297,28 +310,35 @@
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
@@ -327,14 +347,15 @@
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
@@ -345,55 +366,64 @@
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
@@ -431,24 +461,29 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/literals.pyi` & `mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ActiveDirectoryStatusType",
     "AvailabilityMonitorTestStatusType",
     "CaseSensitivityType",
     "DescribeTapeArchivesPaginatorName",
     "DescribeTapeRecoveryPointsPaginatorName",
     "DescribeTapesPaginatorName",
@@ -44,14 +45,15 @@
     "StorageGatewayServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ActiveDirectoryStatusType = Literal[
     "ACCESS_DENIED", "DETACHED", "JOINED", "JOINING", "NETWORK_ERROR", "TIMEOUT", "UNKNOWN_ERROR"
 ]
 AvailabilityMonitorTestStatusType = Literal["COMPLETE", "FAILED", "PENDING"]
 CaseSensitivityType = Literal["CaseSensitive", "ClientSpecified"]
 DescribeTapeArchivesPaginatorName = Literal["describe_tape_archives"]
 DescribeTapeRecoveryPointsPaginatorName = Literal["describe_tape_recovery_points"]
@@ -92,23 +94,25 @@
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
@@ -118,30 +122,35 @@
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
@@ -167,14 +176,15 @@
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
@@ -219,51 +229,57 @@
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
@@ -276,14 +292,15 @@
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
@@ -295,28 +312,35 @@
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
@@ -325,14 +349,15 @@
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
@@ -343,55 +368,64 @@
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
@@ -429,24 +463,29 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/paginator.py` & `mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,30 +86,30 @@
 class DescribeTapeArchivesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeArchives)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetapearchivespaginator)
     """
 
     def paginate(
-        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTapeArchivesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeArchives.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetapearchivespaginator)
         """
 
 
 class DescribeTapeRecoveryPointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeRecoveryPoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetaperecoverypointspaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GatewayARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTapeRecoveryPointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeRecoveryPoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetaperecoverypointspaginator)
         """
 
 
@@ -120,15 +120,15 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         TapeARNs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTapesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetapespaginator)
         """
 
 
@@ -139,118 +139,118 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         VTLDeviceARNs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeVTLDevicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeVTLDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describevtldevicespaginator)
         """
 
 
 class ListFileSharesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileShares)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesharespaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFileSharesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesharespaginator)
         """
 
 
 class ListFileSystemAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileSystemAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesystemassociationspaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFileSystemAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileSystemAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesystemassociationspaginator)
         """
 
 
 class ListGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listgatewayspaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtagsforresourcepaginator)
         """
 
 
 class ListTapePoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapePools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapepoolspaginator)
     """
 
     def paginate(
-        self, *, PoolARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PoolARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTapePoolsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapePools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapepoolspaginator)
         """
 
 
 class ListTapesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapespaginator)
     """
 
     def paginate(
-        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTapesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapespaginator)
         """
 
 
 class ListVolumesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListVolumes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listvolumespaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVolumesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListVolumes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listvolumespaginator)
         """
```

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/paginator.pyi` & `mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -83,29 +83,29 @@
 class DescribeTapeArchivesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeArchives)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetapearchivespaginator)
     """
 
     def paginate(
-        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTapeArchivesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeArchives.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetapearchivespaginator)
         """
 
 class DescribeTapeRecoveryPointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeRecoveryPoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetaperecoverypointspaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GatewayARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTapeRecoveryPointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeRecoveryPoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetaperecoverypointspaginator)
         """
 
 class DescribeTapesPaginator(Paginator):
@@ -115,15 +115,15 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         TapeARNs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTapesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describetapespaginator)
         """
 
 class DescribeVTLDevicesPaginator(Paginator):
@@ -133,111 +133,111 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         VTLDeviceARNs: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeVTLDevicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeVTLDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#describevtldevicespaginator)
         """
 
 class ListFileSharesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileShares)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesharespaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFileSharesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesharespaginator)
         """
 
 class ListFileSystemAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileSystemAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesystemassociationspaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFileSystemAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileSystemAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listfilesystemassociationspaginator)
         """
 
 class ListGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listgatewayspaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtagsforresourcepaginator)
         """
 
 class ListTapePoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapePools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapepoolspaginator)
     """
 
     def paginate(
-        self, *, PoolARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PoolARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTapePoolsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapePools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapepoolspaginator)
         """
 
 class ListTapesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapespaginator)
     """
 
     def paginate(
-        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTapesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listtapespaginator)
         """
 
 class ListVolumesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListVolumes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listvolumespaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVolumesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListVolumes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/paginators/#listvolumespaginator)
         """
```

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/type_defs.py` & `mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,187 +33,198 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "ActivateGatewayOutputTypeDef",
     "AddCacheInputRequestTypeDef",
+    "AddCacheOutputTypeDef",
+    "AddTagsToResourceOutputTypeDef",
     "AddUploadBufferInputRequestTypeDef",
+    "AddUploadBufferOutputTypeDef",
     "AddWorkingStorageInputRequestTypeDef",
+    "AddWorkingStorageOutputTypeDef",
     "AssignTapePoolInputRequestTypeDef",
+    "AssignTapePoolOutputTypeDef",
     "CacheAttributesTypeDef",
     "EndpointNetworkConfigurationTypeDef",
+    "AssociateFileSystemOutputTypeDef",
     "AttachVolumeInputRequestTypeDef",
+    "AttachVolumeOutputTypeDef",
     "AutomaticTapeCreationRuleTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
     "VolumeiSCSIAttributesTypeDef",
     "CancelArchivalInputRequestTypeDef",
+    "CancelArchivalOutputTypeDef",
     "CancelRetrievalInputRequestTypeDef",
+    "CancelRetrievalOutputTypeDef",
     "ChapInfoTypeDef",
+    "CreateCachediSCSIVolumeOutputTypeDef",
     "NFSFileShareDefaultsTypeDef",
+    "CreateNFSFileShareOutputTypeDef",
+    "CreateSMBFileShareOutputTypeDef",
+    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
+    "CreateSnapshotOutputTypeDef",
+    "CreateStorediSCSIVolumeOutputTypeDef",
+    "CreateTapePoolOutputTypeDef",
+    "CreateTapeWithBarcodeOutputTypeDef",
+    "CreateTapesOutputTypeDef",
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
+    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
     "DeleteBandwidthRateLimitInputRequestTypeDef",
+    "DeleteBandwidthRateLimitOutputTypeDef",
     "DeleteChapCredentialsInputRequestTypeDef",
+    "DeleteChapCredentialsOutputTypeDef",
     "DeleteFileShareInputRequestTypeDef",
+    "DeleteFileShareOutputTypeDef",
     "DeleteGatewayInputRequestTypeDef",
+    "DeleteGatewayOutputTypeDef",
     "DeleteSnapshotScheduleInputRequestTypeDef",
+    "DeleteSnapshotScheduleOutputTypeDef",
     "DeleteTapeArchiveInputRequestTypeDef",
+    "DeleteTapeArchiveOutputTypeDef",
     "DeleteTapeInputRequestTypeDef",
+    "DeleteTapeOutputTypeDef",
     "DeleteTapePoolInputRequestTypeDef",
+    "DeleteTapePoolOutputTypeDef",
     "DeleteVolumeInputRequestTypeDef",
+    "DeleteVolumeOutputTypeDef",
     "DescribeAvailabilityMonitorTestInputRequestTypeDef",
+    "DescribeAvailabilityMonitorTestOutputTypeDef",
     "DescribeBandwidthRateLimitInputRequestTypeDef",
+    "DescribeBandwidthRateLimitOutputTypeDef",
     "DescribeBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCacheInputRequestTypeDef",
+    "DescribeCacheOutputTypeDef",
     "DescribeCachediSCSIVolumesInputRequestTypeDef",
     "DescribeChapCredentialsInputRequestTypeDef",
     "DescribeFileSystemAssociationsInputRequestTypeDef",
     "DescribeGatewayInformationInputRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
+    "DescribeMaintenanceStartTimeOutputTypeDef",
     "DescribeNFSFileSharesInputRequestTypeDef",
     "DescribeSMBFileSharesInputRequestTypeDef",
     "DescribeSMBSettingsInputRequestTypeDef",
     "SMBLocalGroupsTypeDef",
     "DescribeSnapshotScheduleInputRequestTypeDef",
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
     "DescribeTapeArchivesInputRequestTypeDef",
     "TapeArchiveTypeDef",
+    "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
     "DescribeTapeRecoveryPointsInputRequestTypeDef",
     "TapeRecoveryPointInfoTypeDef",
+    "DescribeTapesInputDescribeTapesPaginateTypeDef",
     "DescribeTapesInputRequestTypeDef",
     "TapeTypeDef",
     "DescribeUploadBufferInputRequestTypeDef",
+    "DescribeUploadBufferOutputTypeDef",
+    "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
     "DescribeVTLDevicesInputRequestTypeDef",
     "DescribeWorkingStorageInputRequestTypeDef",
+    "DescribeWorkingStorageOutputTypeDef",
     "DetachVolumeInputRequestTypeDef",
+    "DetachVolumeOutputTypeDef",
     "DeviceiSCSIAttributesTypeDef",
     "DisableGatewayInputRequestTypeDef",
+    "DisableGatewayOutputTypeDef",
     "DisassociateFileSystemInputRequestTypeDef",
+    "DisassociateFileSystemOutputTypeDef",
     "DiskTypeDef",
     "FileShareInfoTypeDef",
     "FileSystemAssociationStatusDetailTypeDef",
     "FileSystemAssociationSummaryTypeDef",
     "GatewayInfoTypeDef",
     "JoinDomainInputRequestTypeDef",
+    "JoinDomainOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
+    "ListFileSharesInputListFileSharesPaginateTypeDef",
     "ListFileSharesInputRequestTypeDef",
+    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
     "ListFileSystemAssociationsInputRequestTypeDef",
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
     "ListGatewaysInputRequestTypeDef",
     "ListLocalDisksInputRequestTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
     "ListTapePoolsInputRequestTypeDef",
     "PoolInfoTypeDef",
+    "ListTapesInputListTapesPaginateTypeDef",
     "ListTapesInputRequestTypeDef",
     "TapeInfoTypeDef",
     "ListVolumeInitiatorsInputRequestTypeDef",
+    "ListVolumeInitiatorsOutputTypeDef",
     "ListVolumeRecoveryPointsInputRequestTypeDef",
     "VolumeRecoveryPointInfoTypeDef",
+    "ListVolumesInputListVolumesPaginateTypeDef",
     "ListVolumesInputRequestTypeDef",
     "VolumeInfoTypeDef",
     "NotifyWhenUploadedInputRequestTypeDef",
+    "NotifyWhenUploadedOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "RefreshCacheInputRequestTypeDef",
+    "RefreshCacheOutputTypeDef",
     "RemoveTagsFromResourceInputRequestTypeDef",
+    "RemoveTagsFromResourceOutputTypeDef",
     "ResetCacheInputRequestTypeDef",
+    "ResetCacheOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "RetrieveTapeArchiveInputRequestTypeDef",
+    "RetrieveTapeArchiveOutputTypeDef",
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
+    "RetrieveTapeRecoveryPointOutputTypeDef",
     "SetLocalConsolePasswordInputRequestTypeDef",
+    "SetLocalConsolePasswordOutputTypeDef",
     "SetSMBGuestPasswordInputRequestTypeDef",
+    "SetSMBGuestPasswordOutputTypeDef",
     "ShutdownGatewayInputRequestTypeDef",
+    "ShutdownGatewayOutputTypeDef",
     "StartAvailabilityMonitorTestInputRequestTypeDef",
+    "StartAvailabilityMonitorTestOutputTypeDef",
     "StartGatewayInputRequestTypeDef",
+    "StartGatewayOutputTypeDef",
+    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
     "UpdateBandwidthRateLimitInputRequestTypeDef",
+    "UpdateBandwidthRateLimitOutputTypeDef",
+    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
     "UpdateChapCredentialsInputRequestTypeDef",
+    "UpdateChapCredentialsOutputTypeDef",
+    "UpdateFileSystemAssociationOutputTypeDef",
     "UpdateGatewayInformationInputRequestTypeDef",
+    "UpdateGatewayInformationOutputTypeDef",
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
+    "UpdateGatewaySoftwareNowOutputTypeDef",
     "UpdateMaintenanceStartTimeInputRequestTypeDef",
+    "UpdateMaintenanceStartTimeOutputTypeDef",
+    "UpdateNFSFileShareOutputTypeDef",
+    "UpdateSMBFileShareOutputTypeDef",
     "UpdateSMBFileShareVisibilityInputRequestTypeDef",
+    "UpdateSMBFileShareVisibilityOutputTypeDef",
+    "UpdateSMBLocalGroupsOutputTypeDef",
     "UpdateSMBSecurityStrategyInputRequestTypeDef",
+    "UpdateSMBSecurityStrategyOutputTypeDef",
+    "UpdateSnapshotScheduleOutputTypeDef",
     "UpdateVTLDeviceTypeInputRequestTypeDef",
+    "UpdateVTLDeviceTypeOutputTypeDef",
     "ActivateGatewayInputRequestTypeDef",
     "AddTagsToResourceInputRequestTypeDef",
     "CreateCachediSCSIVolumeInputRequestTypeDef",
     "CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef",
     "CreateSnapshotInputRequestTypeDef",
     "CreateStorediSCSIVolumeInputRequestTypeDef",
     "CreateTapePoolInputRequestTypeDef",
     "CreateTapeWithBarcodeInputRequestTypeDef",
     "CreateTapesInputRequestTypeDef",
-    "UpdateSnapshotScheduleInputRequestTypeDef",
-    "ActivateGatewayOutputTypeDef",
-    "AddCacheOutputTypeDef",
-    "AddTagsToResourceOutputTypeDef",
-    "AddUploadBufferOutputTypeDef",
-    "AddWorkingStorageOutputTypeDef",
-    "AssignTapePoolOutputTypeDef",
-    "AssociateFileSystemOutputTypeDef",
-    "AttachVolumeOutputTypeDef",
-    "CancelArchivalOutputTypeDef",
-    "CancelRetrievalOutputTypeDef",
-    "CreateCachediSCSIVolumeOutputTypeDef",
-    "CreateNFSFileShareOutputTypeDef",
-    "CreateSMBFileShareOutputTypeDef",
-    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
-    "CreateSnapshotOutputTypeDef",
-    "CreateStorediSCSIVolumeOutputTypeDef",
-    "CreateTapePoolOutputTypeDef",
-    "CreateTapeWithBarcodeOutputTypeDef",
-    "CreateTapesOutputTypeDef",
-    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
-    "DeleteBandwidthRateLimitOutputTypeDef",
-    "DeleteChapCredentialsOutputTypeDef",
-    "DeleteFileShareOutputTypeDef",
-    "DeleteGatewayOutputTypeDef",
-    "DeleteSnapshotScheduleOutputTypeDef",
-    "DeleteTapeArchiveOutputTypeDef",
-    "DeleteTapeOutputTypeDef",
-    "DeleteTapePoolOutputTypeDef",
-    "DeleteVolumeOutputTypeDef",
-    "DescribeAvailabilityMonitorTestOutputTypeDef",
-    "DescribeBandwidthRateLimitOutputTypeDef",
-    "DescribeCacheOutputTypeDef",
-    "DescribeMaintenanceStartTimeOutputTypeDef",
     "DescribeSnapshotScheduleOutputTypeDef",
-    "DescribeUploadBufferOutputTypeDef",
-    "DescribeWorkingStorageOutputTypeDef",
-    "DetachVolumeOutputTypeDef",
-    "DisableGatewayOutputTypeDef",
-    "DisassociateFileSystemOutputTypeDef",
-    "JoinDomainOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "ListVolumeInitiatorsOutputTypeDef",
-    "NotifyWhenUploadedOutputTypeDef",
-    "RefreshCacheOutputTypeDef",
-    "RemoveTagsFromResourceOutputTypeDef",
-    "ResetCacheOutputTypeDef",
-    "RetrieveTapeArchiveOutputTypeDef",
-    "RetrieveTapeRecoveryPointOutputTypeDef",
-    "SetLocalConsolePasswordOutputTypeDef",
-    "SetSMBGuestPasswordOutputTypeDef",
-    "ShutdownGatewayOutputTypeDef",
-    "StartAvailabilityMonitorTestOutputTypeDef",
-    "StartGatewayOutputTypeDef",
-    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
-    "UpdateBandwidthRateLimitOutputTypeDef",
-    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
-    "UpdateChapCredentialsOutputTypeDef",
-    "UpdateFileSystemAssociationOutputTypeDef",
-    "UpdateGatewayInformationOutputTypeDef",
-    "UpdateGatewaySoftwareNowOutputTypeDef",
-    "UpdateMaintenanceStartTimeOutputTypeDef",
-    "UpdateNFSFileShareOutputTypeDef",
-    "UpdateSMBFileShareOutputTypeDef",
-    "UpdateSMBFileShareVisibilityOutputTypeDef",
-    "UpdateSMBLocalGroupsOutputTypeDef",
-    "UpdateSMBSecurityStrategyOutputTypeDef",
-    "UpdateSnapshotScheduleOutputTypeDef",
-    "UpdateVTLDeviceTypeOutputTypeDef",
+    "UpdateSnapshotScheduleInputRequestTypeDef",
     "CreateSMBFileShareInputRequestTypeDef",
     "SMBFileShareInfoTypeDef",
     "UpdateFileSystemAssociationInputRequestTypeDef",
     "UpdateSMBFileShareInputRequestTypeDef",
     "AssociateFileSystemInputRequestTypeDef",
     "AutomaticTapeCreationPolicyInfoTypeDef",
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
@@ -224,25 +235,14 @@
     "DescribeChapCredentialsOutputTypeDef",
     "CreateNFSFileShareInputRequestTypeDef",
     "NFSFileShareInfoTypeDef",
     "UpdateNFSFileShareInputRequestTypeDef",
     "DescribeGatewayInformationOutputTypeDef",
     "DescribeSMBSettingsOutputTypeDef",
     "UpdateSMBLocalGroupsInputRequestTypeDef",
-    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
-    "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
-    "DescribeTapesInputDescribeTapesPaginateTypeDef",
-    "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
-    "ListFileSharesInputListFileSharesPaginateTypeDef",
-    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
-    "ListTapesInputListTapesPaginateTypeDef",
-    "ListVolumesInputListVolumesPaginateTypeDef",
     "DescribeTapeArchivesOutputTypeDef",
     "DescribeTapeRecoveryPointsOutputTypeDef",
     "DescribeTapesOutputTypeDef",
     "VTLDeviceTypeDef",
     "ListLocalDisksOutputTypeDef",
     "ListFileSharesOutputTypeDef",
     "FileSystemAssociationInfoTypeDef",
@@ -265,49 +265,78 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ActivateGatewayOutputTypeDef = TypedDict(
+    "ActivateGatewayOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddCacheInputRequestTypeDef = TypedDict(
     "AddCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
+AddCacheOutputTypeDef = TypedDict(
+    "AddCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AddTagsToResourceOutputTypeDef = TypedDict(
+    "AddTagsToResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AddUploadBufferInputRequestTypeDef = TypedDict(
     "AddUploadBufferInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
+AddUploadBufferOutputTypeDef = TypedDict(
+    "AddUploadBufferOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AddWorkingStorageInputRequestTypeDef = TypedDict(
     "AddWorkingStorageInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
+AddWorkingStorageOutputTypeDef = TypedDict(
+    "AddWorkingStorageOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAssignTapePoolInputRequestTypeDef = TypedDict(
     "_RequiredAssignTapePoolInputRequestTypeDef",
     {
         "TapeARN": str,
         "PoolId": str,
     },
 )
@@ -322,14 +351,22 @@
 
 class AssignTapePoolInputRequestTypeDef(
     _RequiredAssignTapePoolInputRequestTypeDef, _OptionalAssignTapePoolInputRequestTypeDef
 ):
     pass
 
 
+AssignTapePoolOutputTypeDef = TypedDict(
+    "AssignTapePoolOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CacheAttributesTypeDef = TypedDict(
     "CacheAttributesTypeDef",
     {
         "CacheStaleTimeoutInSeconds": int,
     },
     total=False,
 )
@@ -338,14 +375,22 @@
     "EndpointNetworkConfigurationTypeDef",
     {
         "IpAddresses": Sequence[str],
     },
     total=False,
 )
 
+AssociateFileSystemOutputTypeDef = TypedDict(
+    "AssociateFileSystemOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAttachVolumeInputRequestTypeDef = TypedDict(
     "_RequiredAttachVolumeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "VolumeARN": str,
         "NetworkInterfaceId": str,
     },
@@ -362,14 +407,23 @@
 
 class AttachVolumeInputRequestTypeDef(
     _RequiredAttachVolumeInputRequestTypeDef, _OptionalAttachVolumeInputRequestTypeDef
 ):
     pass
 
 
+AttachVolumeOutputTypeDef = TypedDict(
+    "AttachVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "TargetARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAutomaticTapeCreationRuleTypeDef = TypedDict(
     "_RequiredAutomaticTapeCreationRuleTypeDef",
     {
         "TapeBarcodePrefix": str,
         "PoolId": str,
         "TapeSizeInBytes": int,
         "MinimumNumTapes": int,
@@ -432,67 +486,186 @@
     "CancelArchivalInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
 
+CancelArchivalOutputTypeDef = TypedDict(
+    "CancelArchivalOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CancelRetrievalInputRequestTypeDef = TypedDict(
     "CancelRetrievalInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
 
+CancelRetrievalOutputTypeDef = TypedDict(
+    "CancelRetrievalOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ChapInfoTypeDef = TypedDict(
     "ChapInfoTypeDef",
     {
         "TargetARN": str,
         "SecretToAuthenticateInitiator": str,
         "InitiatorName": str,
         "SecretToAuthenticateTarget": str,
     },
     total=False,
 )
 
+CreateCachediSCSIVolumeOutputTypeDef = TypedDict(
+    "CreateCachediSCSIVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "TargetARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 NFSFileShareDefaultsTypeDef = TypedDict(
     "NFSFileShareDefaultsTypeDef",
     {
         "FileMode": str,
         "DirectoryMode": str,
         "GroupId": int,
         "OwnerId": int,
     },
     total=False,
 )
 
+CreateNFSFileShareOutputTypeDef = TypedDict(
+    "CreateNFSFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSMBFileShareOutputTypeDef = TypedDict(
+    "CreateSMBFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSnapshotFromVolumeRecoveryPointOutputTypeDef = TypedDict(
+    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
+    {
+        "SnapshotId": str,
+        "VolumeARN": str,
+        "VolumeRecoveryPointTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSnapshotOutputTypeDef = TypedDict(
+    "CreateSnapshotOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "SnapshotId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateStorediSCSIVolumeOutputTypeDef = TypedDict(
+    "CreateStorediSCSIVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "VolumeSizeInBytes": int,
+        "TargetARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateTapePoolOutputTypeDef = TypedDict(
+    "CreateTapePoolOutputTypeDef",
+    {
+        "PoolARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateTapeWithBarcodeOutputTypeDef = TypedDict(
+    "CreateTapeWithBarcodeOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateTapesOutputTypeDef = TypedDict(
+    "CreateTapesOutputTypeDef",
+    {
+        "TapeARNs": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteAutomaticTapeCreationPolicyInputRequestTypeDef = TypedDict(
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DeleteAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
+    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "DeleteBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
         "BandwidthType": str,
     },
 )
 
+DeleteBandwidthRateLimitOutputTypeDef = TypedDict(
+    "DeleteBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteChapCredentialsInputRequestTypeDef = TypedDict(
     "DeleteChapCredentialsInputRequestTypeDef",
     {
         "TargetARN": str,
         "InitiatorName": str,
     },
 )
 
+DeleteChapCredentialsOutputTypeDef = TypedDict(
+    "DeleteChapCredentialsOutputTypeDef",
+    {
+        "TargetARN": str,
+        "InitiatorName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteFileShareInputRequestTypeDef = TypedDict(
     "_RequiredDeleteFileShareInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalDeleteFileShareInputRequestTypeDef = TypedDict(
@@ -506,28 +679,52 @@
 
 class DeleteFileShareInputRequestTypeDef(
     _RequiredDeleteFileShareInputRequestTypeDef, _OptionalDeleteFileShareInputRequestTypeDef
 ):
     pass
 
 
+DeleteFileShareOutputTypeDef = TypedDict(
+    "DeleteFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteGatewayInputRequestTypeDef = TypedDict(
     "DeleteGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DeleteGatewayOutputTypeDef = TypedDict(
+    "DeleteGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSnapshotScheduleInputRequestTypeDef = TypedDict(
     "DeleteSnapshotScheduleInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
+DeleteSnapshotScheduleOutputTypeDef = TypedDict(
+    "DeleteSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteTapeArchiveInputRequestTypeDef = TypedDict(
     "_RequiredDeleteTapeArchiveInputRequestTypeDef",
     {
         "TapeARN": str,
     },
 )
 _OptionalDeleteTapeArchiveInputRequestTypeDef = TypedDict(
@@ -541,14 +738,22 @@
 
 class DeleteTapeArchiveInputRequestTypeDef(
     _RequiredDeleteTapeArchiveInputRequestTypeDef, _OptionalDeleteTapeArchiveInputRequestTypeDef
 ):
     pass
 
 
+DeleteTapeArchiveOutputTypeDef = TypedDict(
+    "DeleteTapeArchiveOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteTapeInputRequestTypeDef = TypedDict(
     "_RequiredDeleteTapeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
@@ -563,56 +768,114 @@
 
 class DeleteTapeInputRequestTypeDef(
     _RequiredDeleteTapeInputRequestTypeDef, _OptionalDeleteTapeInputRequestTypeDef
 ):
     pass
 
 
+DeleteTapeOutputTypeDef = TypedDict(
+    "DeleteTapeOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTapePoolInputRequestTypeDef = TypedDict(
     "DeleteTapePoolInputRequestTypeDef",
     {
         "PoolARN": str,
     },
 )
 
+DeleteTapePoolOutputTypeDef = TypedDict(
+    "DeleteTapePoolOutputTypeDef",
+    {
+        "PoolARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteVolumeInputRequestTypeDef = TypedDict(
     "DeleteVolumeInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
+DeleteVolumeOutputTypeDef = TypedDict(
+    "DeleteVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeAvailabilityMonitorTestInputRequestTypeDef = TypedDict(
     "DescribeAvailabilityMonitorTestInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DescribeAvailabilityMonitorTestOutputTypeDef = TypedDict(
+    "DescribeAvailabilityMonitorTestOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "Status": AvailabilityMonitorTestStatusType,
+        "StartTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "DescribeBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DescribeBandwidthRateLimitOutputTypeDef = TypedDict(
+    "DescribeBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "AverageUploadRateLimitInBitsPerSec": int,
+        "AverageDownloadRateLimitInBitsPerSec": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
 DescribeCacheInputRequestTypeDef = TypedDict(
     "DescribeCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DescribeCacheOutputTypeDef = TypedDict(
+    "DescribeCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "CacheAllocatedInBytes": int,
+        "CacheUsedPercentage": float,
+        "CacheDirtyPercentage": float,
+        "CacheHitPercentage": float,
+        "CacheMissPercentage": float,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeCachediSCSIVolumesInputRequestTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesInputRequestTypeDef",
     {
         "VolumeARNs": Sequence[str],
     },
 )
 
@@ -650,14 +913,27 @@
 DescribeMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DescribeMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "DescribeMaintenanceStartTimeOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "HourOfDay": int,
+        "MinuteOfHour": int,
+        "DayOfWeek": int,
+        "DayOfMonth": int,
+        "Timezone": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeNFSFileSharesInputRequestTypeDef = TypedDict(
     "DescribeNFSFileSharesInputRequestTypeDef",
     {
         "FileShareARNList": Sequence[str],
     },
 )
 
@@ -693,20 +969,19 @@
 DescribeStorediSCSIVolumesInputRequestTypeDef = TypedDict(
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
     {
         "VolumeARNs": Sequence[str],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
+    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeTapeArchivesInputRequestTypeDef = TypedDict(
     "DescribeTapeArchivesInputRequestTypeDef",
     {
@@ -733,14 +1008,36 @@
         "Worm": bool,
         "RetentionStartDate": datetime,
         "PoolEntryDate": datetime,
     },
     total=False,
 )
 
+_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
+    {
+        "GatewayARN": str,
+    },
+)
+_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef(
+    _RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+    _OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeTapeRecoveryPointsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTapeRecoveryPointsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeTapeRecoveryPointsInputRequestTypeDef = TypedDict(
@@ -767,14 +1064,37 @@
         "TapeRecoveryPointTime": datetime,
         "TapeSizeInBytes": int,
         "TapeStatus": str,
     },
     total=False,
 )
 
+_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+    },
+)
+_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeTapesInputDescribeTapesPaginateTypeDef(
+    _RequiredDescribeTapesInputDescribeTapesPaginateTypeDef,
+    _OptionalDescribeTapesInputDescribeTapesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeTapesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTapesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeTapesInputRequestTypeDef = TypedDict(
@@ -817,14 +1137,48 @@
 DescribeUploadBufferInputRequestTypeDef = TypedDict(
     "DescribeUploadBufferInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DescribeUploadBufferOutputTypeDef = TypedDict(
+    "DescribeUploadBufferOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "UploadBufferUsedInBytes": int,
+        "UploadBufferAllocatedInBytes": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+    },
+)
+_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
+    {
+        "VTLDeviceARNs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef(
+    _RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+    _OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeVTLDevicesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVTLDevicesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeVTLDevicesInputRequestTypeDef = TypedDict(
@@ -847,14 +1201,25 @@
 DescribeWorkingStorageInputRequestTypeDef = TypedDict(
     "DescribeWorkingStorageInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DescribeWorkingStorageOutputTypeDef = TypedDict(
+    "DescribeWorkingStorageOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "WorkingStorageUsedInBytes": int,
+        "WorkingStorageAllocatedInBytes": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDetachVolumeInputRequestTypeDef = TypedDict(
     "_RequiredDetachVolumeInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 _OptionalDetachVolumeInputRequestTypeDef = TypedDict(
@@ -868,14 +1233,22 @@
 
 class DetachVolumeInputRequestTypeDef(
     _RequiredDetachVolumeInputRequestTypeDef, _OptionalDetachVolumeInputRequestTypeDef
 ):
     pass
 
 
+DetachVolumeOutputTypeDef = TypedDict(
+    "DetachVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeviceiSCSIAttributesTypeDef = TypedDict(
     "DeviceiSCSIAttributesTypeDef",
     {
         "TargetARN": str,
         "NetworkInterfaceId": str,
         "NetworkInterfacePort": int,
         "ChapEnabled": bool,
@@ -886,14 +1259,22 @@
 DisableGatewayInputRequestTypeDef = TypedDict(
     "DisableGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DisableGatewayOutputTypeDef = TypedDict(
+    "DisableGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDisassociateFileSystemInputRequestTypeDef = TypedDict(
     "_RequiredDisassociateFileSystemInputRequestTypeDef",
     {
         "FileSystemAssociationARN": str,
     },
 )
 _OptionalDisassociateFileSystemInputRequestTypeDef = TypedDict(
@@ -908,14 +1289,22 @@
 class DisassociateFileSystemInputRequestTypeDef(
     _RequiredDisassociateFileSystemInputRequestTypeDef,
     _OptionalDisassociateFileSystemInputRequestTypeDef,
 ):
     pass
 
 
+DisassociateFileSystemOutputTypeDef = TypedDict(
+    "DisassociateFileSystemOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DiskTypeDef = TypedDict(
     "DiskTypeDef",
     {
         "DiskId": str,
         "DiskPath": str,
         "DiskNode": str,
         "DiskStatus": str,
@@ -996,42 +1385,77 @@
 
 class JoinDomainInputRequestTypeDef(
     _RequiredJoinDomainInputRequestTypeDef, _OptionalJoinDomainInputRequestTypeDef
 ):
     pass
 
 
+JoinDomainOutputTypeDef = TypedDict(
+    "JoinDomainOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ActiveDirectoryStatus": ActiveDirectoryStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListAutomaticTapeCreationPoliciesInputRequestTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
     total=False,
 )
 
+ListFileSharesInputListFileSharesPaginateTypeDef = TypedDict(
+    "ListFileSharesInputListFileSharesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFileSharesInputRequestTypeDef = TypedDict(
     "ListFileSharesInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef = TypedDict(
+    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFileSystemAssociationsInputRequestTypeDef = TypedDict(
     "ListFileSystemAssociationsInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGatewaysInputRequestTypeDef = TypedDict(
     "ListGatewaysInputRequestTypeDef",
     {
         "Marker": str,
         "Limit": int,
     },
     total=False,
@@ -1040,14 +1464,36 @@
 ListLocalDisksInputRequestTypeDef = TypedDict(
     "ListLocalDisksInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -1062,14 +1508,23 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
+ListTapePoolsInputListTapePoolsPaginateTypeDef = TypedDict(
+    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
+    {
+        "PoolARNs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTapePoolsInputRequestTypeDef = TypedDict(
     "ListTapePoolsInputRequestTypeDef",
     {
         "PoolARNs": Sequence[str],
         "Marker": str,
         "Limit": int,
     },
@@ -1085,14 +1540,23 @@
         "RetentionLockType": RetentionLockTypeType,
         "RetentionLockTimeInDays": int,
         "PoolStatus": PoolStatusType,
     },
     total=False,
 )
 
+ListTapesInputListTapesPaginateTypeDef = TypedDict(
+    "ListTapesInputListTapesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTapesInputRequestTypeDef = TypedDict(
     "ListTapesInputRequestTypeDef",
     {
         "TapeARNs": Sequence[str],
         "Marker": str,
         "Limit": int,
     },
@@ -1117,14 +1581,22 @@
 ListVolumeInitiatorsInputRequestTypeDef = TypedDict(
     "ListVolumeInitiatorsInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
+ListVolumeInitiatorsOutputTypeDef = TypedDict(
+    "ListVolumeInitiatorsOutputTypeDef",
+    {
+        "Initiators": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListVolumeRecoveryPointsInputRequestTypeDef = TypedDict(
     "ListVolumeRecoveryPointsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
@@ -1135,14 +1607,23 @@
         "VolumeSizeInBytes": int,
         "VolumeUsageInBytes": int,
         "VolumeRecoveryPointTime": str,
     },
     total=False,
 )
 
+ListVolumesInputListVolumesPaginateTypeDef = TypedDict(
+    "ListVolumesInputListVolumesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListVolumesInputRequestTypeDef = TypedDict(
     "ListVolumesInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Marker": str,
         "Limit": int,
     },
@@ -1166,14 +1647,33 @@
 NotifyWhenUploadedInputRequestTypeDef = TypedDict(
     "NotifyWhenUploadedInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 
+NotifyWhenUploadedOutputTypeDef = TypedDict(
+    "NotifyWhenUploadedOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "NotificationId": str,
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
 _RequiredRefreshCacheInputRequestTypeDef = TypedDict(
     "_RequiredRefreshCacheInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalRefreshCacheInputRequestTypeDef = TypedDict(
@@ -1188,82 +1688,182 @@
 
 class RefreshCacheInputRequestTypeDef(
     _RequiredRefreshCacheInputRequestTypeDef, _OptionalRefreshCacheInputRequestTypeDef
 ):
     pass
 
 
+RefreshCacheOutputTypeDef = TypedDict(
+    "RefreshCacheOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "NotificationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveTagsFromResourceInputRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+RemoveTagsFromResourceOutputTypeDef = TypedDict(
+    "RemoveTagsFromResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ResetCacheInputRequestTypeDef = TypedDict(
     "ResetCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+ResetCacheOutputTypeDef = TypedDict(
+    "ResetCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
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
 RetrieveTapeArchiveInputRequestTypeDef = TypedDict(
     "RetrieveTapeArchiveInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
 
+RetrieveTapeArchiveOutputTypeDef = TypedDict(
+    "RetrieveTapeArchiveOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RetrieveTapeRecoveryPointInputRequestTypeDef = TypedDict(
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
 
+RetrieveTapeRecoveryPointOutputTypeDef = TypedDict(
+    "RetrieveTapeRecoveryPointOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetLocalConsolePasswordInputRequestTypeDef = TypedDict(
     "SetLocalConsolePasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "LocalConsolePassword": str,
     },
 )
 
+SetLocalConsolePasswordOutputTypeDef = TypedDict(
+    "SetLocalConsolePasswordOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetSMBGuestPasswordInputRequestTypeDef = TypedDict(
     "SetSMBGuestPasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Password": str,
     },
 )
 
+SetSMBGuestPasswordOutputTypeDef = TypedDict(
+    "SetSMBGuestPasswordOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ShutdownGatewayInputRequestTypeDef = TypedDict(
     "ShutdownGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+ShutdownGatewayOutputTypeDef = TypedDict(
+    "ShutdownGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartAvailabilityMonitorTestInputRequestTypeDef = TypedDict(
     "StartAvailabilityMonitorTestInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+StartAvailabilityMonitorTestOutputTypeDef = TypedDict(
+    "StartAvailabilityMonitorTestOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartGatewayInputRequestTypeDef = TypedDict(
     "StartGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+StartGatewayOutputTypeDef = TypedDict(
+    "StartGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
+    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "_RequiredUpdateBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalUpdateBandwidthRateLimitInputRequestTypeDef = TypedDict(
@@ -1279,14 +1879,30 @@
 class UpdateBandwidthRateLimitInputRequestTypeDef(
     _RequiredUpdateBandwidthRateLimitInputRequestTypeDef,
     _OptionalUpdateBandwidthRateLimitInputRequestTypeDef,
 ):
     pass
 
 
+UpdateBandwidthRateLimitOutputTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateChapCredentialsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateChapCredentialsInputRequestTypeDef",
     {
         "TargetARN": str,
         "SecretToAuthenticateInitiator": str,
         "InitiatorName": str,
     },
@@ -1303,14 +1919,31 @@
 class UpdateChapCredentialsInputRequestTypeDef(
     _RequiredUpdateChapCredentialsInputRequestTypeDef,
     _OptionalUpdateChapCredentialsInputRequestTypeDef,
 ):
     pass
 
 
+UpdateChapCredentialsOutputTypeDef = TypedDict(
+    "UpdateChapCredentialsOutputTypeDef",
+    {
+        "TargetARN": str,
+        "InitiatorName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateFileSystemAssociationOutputTypeDef = TypedDict(
+    "UpdateFileSystemAssociationOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateGatewayInformationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayInformationInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalUpdateGatewayInformationInputRequestTypeDef = TypedDict(
@@ -1328,21 +1961,38 @@
 class UpdateGatewayInformationInputRequestTypeDef(
     _RequiredUpdateGatewayInformationInputRequestTypeDef,
     _OptionalUpdateGatewayInformationInputRequestTypeDef,
 ):
     pass
 
 
+UpdateGatewayInformationOutputTypeDef = TypedDict(
+    "UpdateGatewayInformationOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "GatewayName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateGatewaySoftwareNowInputRequestTypeDef = TypedDict(
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
+    "UpdateGatewaySoftwareNowOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
@@ -1360,38 +2010,102 @@
 class UpdateMaintenanceStartTimeInputRequestTypeDef(
     _RequiredUpdateMaintenanceStartTimeInputRequestTypeDef,
     _OptionalUpdateMaintenanceStartTimeInputRequestTypeDef,
 ):
     pass
 
 
+UpdateMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "UpdateMaintenanceStartTimeOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateNFSFileShareOutputTypeDef = TypedDict(
+    "UpdateNFSFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSMBFileShareOutputTypeDef = TypedDict(
+    "UpdateSMBFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateSMBFileShareVisibilityInputRequestTypeDef = TypedDict(
     "UpdateSMBFileShareVisibilityInputRequestTypeDef",
     {
         "GatewayARN": str,
         "FileSharesVisible": bool,
     },
 )
 
+UpdateSMBFileShareVisibilityOutputTypeDef = TypedDict(
+    "UpdateSMBFileShareVisibilityOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSMBLocalGroupsOutputTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateSMBSecurityStrategyInputRequestTypeDef = TypedDict(
     "UpdateSMBSecurityStrategyInputRequestTypeDef",
     {
         "GatewayARN": str,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
     },
 )
 
+UpdateSMBSecurityStrategyOutputTypeDef = TypedDict(
+    "UpdateSMBSecurityStrategyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSnapshotScheduleOutputTypeDef = TypedDict(
+    "UpdateSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateVTLDeviceTypeInputRequestTypeDef = TypedDict(
     "UpdateVTLDeviceTypeInputRequestTypeDef",
     {
         "VTLDeviceARN": str,
         "DeviceType": str,
     },
 )
 
+UpdateVTLDeviceTypeOutputTypeDef = TypedDict(
+    "UpdateVTLDeviceTypeOutputTypeDef",
+    {
+        "VTLDeviceARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredActivateGatewayInputRequestTypeDef = TypedDict(
     "_RequiredActivateGatewayInputRequestTypeDef",
     {
         "ActivationKey": str,
         "GatewayName": str,
         "GatewayTimezone": str,
         "GatewayRegion": str,
@@ -1604,623 +2318,61 @@
 
 class CreateTapesInputRequestTypeDef(
     _RequiredCreateTapesInputRequestTypeDef, _OptionalCreateTapesInputRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateSnapshotScheduleInputRequestTypeDef",
-    {
-        "VolumeARN": str,
-        "StartAt": int,
-        "RecurrenceInHours": int,
-    },
-)
-_OptionalUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateSnapshotScheduleInputRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class UpdateSnapshotScheduleInputRequestTypeDef(
-    _RequiredUpdateSnapshotScheduleInputRequestTypeDef,
-    _OptionalUpdateSnapshotScheduleInputRequestTypeDef,
-):
-    pass
-
-
-ActivateGatewayOutputTypeDef = TypedDict(
-    "ActivateGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddCacheOutputTypeDef = TypedDict(
-    "AddCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddTagsToResourceOutputTypeDef = TypedDict(
-    "AddTagsToResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddUploadBufferOutputTypeDef = TypedDict(
-    "AddUploadBufferOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddWorkingStorageOutputTypeDef = TypedDict(
-    "AddWorkingStorageOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssignTapePoolOutputTypeDef = TypedDict(
-    "AssignTapePoolOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateFileSystemOutputTypeDef = TypedDict(
-    "AssociateFileSystemOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AttachVolumeOutputTypeDef = TypedDict(
-    "AttachVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "TargetARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelArchivalOutputTypeDef = TypedDict(
-    "CancelArchivalOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelRetrievalOutputTypeDef = TypedDict(
-    "CancelRetrievalOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCachediSCSIVolumeOutputTypeDef = TypedDict(
-    "CreateCachediSCSIVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "TargetARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateNFSFileShareOutputTypeDef = TypedDict(
-    "CreateNFSFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSMBFileShareOutputTypeDef = TypedDict(
-    "CreateSMBFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSnapshotFromVolumeRecoveryPointOutputTypeDef = TypedDict(
-    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
-    {
-        "SnapshotId": str,
-        "VolumeARN": str,
-        "VolumeRecoveryPointTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSnapshotOutputTypeDef = TypedDict(
-    "CreateSnapshotOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "SnapshotId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStorediSCSIVolumeOutputTypeDef = TypedDict(
-    "CreateStorediSCSIVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "VolumeSizeInBytes": int,
-        "TargetARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTapePoolOutputTypeDef = TypedDict(
-    "CreateTapePoolOutputTypeDef",
-    {
-        "PoolARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTapeWithBarcodeOutputTypeDef = TypedDict(
-    "CreateTapeWithBarcodeOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTapesOutputTypeDef = TypedDict(
-    "CreateTapesOutputTypeDef",
-    {
-        "TapeARNs": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
-    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBandwidthRateLimitOutputTypeDef = TypedDict(
-    "DeleteBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteChapCredentialsOutputTypeDef = TypedDict(
-    "DeleteChapCredentialsOutputTypeDef",
-    {
-        "TargetARN": str,
-        "InitiatorName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFileShareOutputTypeDef = TypedDict(
-    "DeleteFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteGatewayOutputTypeDef = TypedDict(
-    "DeleteGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSnapshotScheduleOutputTypeDef = TypedDict(
-    "DeleteSnapshotScheduleOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteTapeArchiveOutputTypeDef = TypedDict(
-    "DeleteTapeArchiveOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteTapeOutputTypeDef = TypedDict(
-    "DeleteTapeOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteTapePoolOutputTypeDef = TypedDict(
-    "DeleteTapePoolOutputTypeDef",
-    {
-        "PoolARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteVolumeOutputTypeDef = TypedDict(
-    "DeleteVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAvailabilityMonitorTestOutputTypeDef = TypedDict(
-    "DescribeAvailabilityMonitorTestOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "Status": AvailabilityMonitorTestStatusType,
-        "StartTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBandwidthRateLimitOutputTypeDef = TypedDict(
-    "DescribeBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "AverageUploadRateLimitInBitsPerSec": int,
-        "AverageDownloadRateLimitInBitsPerSec": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeCacheOutputTypeDef = TypedDict(
-    "DescribeCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "CacheAllocatedInBytes": int,
-        "CacheUsedPercentage": float,
-        "CacheDirtyPercentage": float,
-        "CacheHitPercentage": float,
-        "CacheMissPercentage": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "DescribeMaintenanceStartTimeOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "HourOfDay": int,
-        "MinuteOfHour": int,
-        "DayOfWeek": int,
-        "DayOfMonth": int,
-        "Timezone": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeSnapshotScheduleOutputTypeDef = TypedDict(
     "DescribeSnapshotScheduleOutputTypeDef",
     {
         "VolumeARN": str,
         "StartAt": int,
         "RecurrenceInHours": int,
         "Description": str,
         "Timezone": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeUploadBufferOutputTypeDef = TypedDict(
-    "DescribeUploadBufferOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "UploadBufferUsedInBytes": int,
-        "UploadBufferAllocatedInBytes": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeWorkingStorageOutputTypeDef = TypedDict(
-    "DescribeWorkingStorageOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "WorkingStorageUsedInBytes": int,
-        "WorkingStorageAllocatedInBytes": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetachVolumeOutputTypeDef = TypedDict(
-    "DetachVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisableGatewayOutputTypeDef = TypedDict(
-    "DisableGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateFileSystemOutputTypeDef = TypedDict(
-    "DisassociateFileSystemOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-JoinDomainOutputTypeDef = TypedDict(
-    "JoinDomainOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ActiveDirectoryStatus": ActiveDirectoryStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "ResourceARN": str,
         "Marker": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListVolumeInitiatorsOutputTypeDef = TypedDict(
-    "ListVolumeInitiatorsOutputTypeDef",
-    {
-        "Initiators": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-NotifyWhenUploadedOutputTypeDef = TypedDict(
-    "NotifyWhenUploadedOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "NotificationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RefreshCacheOutputTypeDef = TypedDict(
-    "RefreshCacheOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "NotificationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveTagsFromResourceOutputTypeDef = TypedDict(
-    "RemoveTagsFromResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ResetCacheOutputTypeDef = TypedDict(
-    "ResetCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RetrieveTapeArchiveOutputTypeDef = TypedDict(
-    "RetrieveTapeArchiveOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RetrieveTapeRecoveryPointOutputTypeDef = TypedDict(
-    "RetrieveTapeRecoveryPointOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetLocalConsolePasswordOutputTypeDef = TypedDict(
-    "SetLocalConsolePasswordOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetSMBGuestPasswordOutputTypeDef = TypedDict(
-    "SetSMBGuestPasswordOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ShutdownGatewayOutputTypeDef = TypedDict(
-    "ShutdownGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartAvailabilityMonitorTestOutputTypeDef = TypedDict(
-    "StartAvailabilityMonitorTestOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartGatewayOutputTypeDef = TypedDict(
-    "StartGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
-    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateBandwidthRateLimitOutputTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateChapCredentialsOutputTypeDef = TypedDict(
-    "UpdateChapCredentialsOutputTypeDef",
-    {
-        "TargetARN": str,
-        "InitiatorName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFileSystemAssociationOutputTypeDef = TypedDict(
-    "UpdateFileSystemAssociationOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGatewayInformationOutputTypeDef = TypedDict(
-    "UpdateGatewayInformationOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "GatewayName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
-    "UpdateGatewaySoftwareNowOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "UpdateMaintenanceStartTimeOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateNFSFileShareOutputTypeDef = TypedDict(
-    "UpdateNFSFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSMBFileShareOutputTypeDef = TypedDict(
-    "UpdateSMBFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateSMBFileShareVisibilityOutputTypeDef = TypedDict(
-    "UpdateSMBFileShareVisibilityOutputTypeDef",
+_RequiredUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateSnapshotScheduleInputRequestTypeDef",
     {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "VolumeARN": str,
+        "StartAt": int,
+        "RecurrenceInHours": int,
     },
 )
-
-UpdateSMBLocalGroupsOutputTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsOutputTypeDef",
+_OptionalUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateSnapshotScheduleInputRequestTypeDef",
     {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
-UpdateSMBSecurityStrategyOutputTypeDef = TypedDict(
-    "UpdateSMBSecurityStrategyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpdateSnapshotScheduleOutputTypeDef = TypedDict(
-    "UpdateSnapshotScheduleOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UpdateSnapshotScheduleInputRequestTypeDef(
+    _RequiredUpdateSnapshotScheduleInputRequestTypeDef,
+    _OptionalUpdateSnapshotScheduleInputRequestTypeDef,
+):
+    pass
 
-UpdateVTLDeviceTypeOutputTypeDef = TypedDict(
-    "UpdateVTLDeviceTypeOutputTypeDef",
-    {
-        "VTLDeviceARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 _RequiredCreateSMBFileShareInputRequestTypeDef = TypedDict(
     "_RequiredCreateSMBFileShareInputRequestTypeDef",
     {
         "ClientToken": str,
         "GatewayARN": str,
         "Role": str,
@@ -2408,15 +2560,15 @@
 )
 
 DescribeBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
     {
         "GatewayARN": str,
         "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     {
         "GatewayARN": str,
@@ -2466,15 +2618,15 @@
     total=False,
 )
 
 DescribeChapCredentialsOutputTypeDef = TypedDict(
     "DescribeChapCredentialsOutputTypeDef",
     {
         "ChapCredentials": List[ChapInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateNFSFileShareInputRequestTypeDef = TypedDict(
     "_RequiredCreateNFSFileShareInputRequestTypeDef",
     {
         "ClientToken": str,
@@ -2599,217 +2751,65 @@
         "HostEnvironment": HostEnvironmentType,
         "EndpointType": str,
         "SoftwareUpdatesEndDate": str,
         "DeprecationDate": str,
         "GatewayCapacity": GatewayCapacityType,
         "SupportedGatewayCapacities": List[GatewayCapacityType],
         "HostEnvironmentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSMBSettingsOutputTypeDef = TypedDict(
     "DescribeSMBSettingsOutputTypeDef",
     {
         "GatewayARN": str,
         "DomainName": str,
         "ActiveDirectoryStatus": ActiveDirectoryStatusType,
         "SMBGuestPasswordSet": bool,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
         "FileSharesVisible": bool,
         "SMBLocalGroups": SMBLocalGroupsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
     "UpdateSMBLocalGroupsInputRequestTypeDef",
     {
         "GatewayARN": str,
         "SMBLocalGroups": SMBLocalGroupsTypeDef,
     },
 )
 
-DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
-    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
-    {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef(
-    _RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
-    _OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef",
-    {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeTapesInputDescribeTapesPaginateTypeDef(
-    _RequiredDescribeTapesInputDescribeTapesPaginateTypeDef,
-    _OptionalDescribeTapesInputDescribeTapesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
-    {
-        "VTLDeviceARNs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef(
-    _RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
-    _OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
-):
-    pass
-
-
-ListFileSharesInputListFileSharesPaginateTypeDef = TypedDict(
-    "ListFileSharesInputListFileSharesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef = TypedDict(
-    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
-ListTapePoolsInputListTapePoolsPaginateTypeDef = TypedDict(
-    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
-    {
-        "PoolARNs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTapesInputListTapesPaginateTypeDef = TypedDict(
-    "ListTapesInputListTapesPaginateTypeDef",
-    {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListVolumesInputListVolumesPaginateTypeDef = TypedDict(
-    "ListVolumesInputListVolumesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeTapeArchivesOutputTypeDef = TypedDict(
     "DescribeTapeArchivesOutputTypeDef",
     {
         "TapeArchives": List[TapeArchiveTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTapeRecoveryPointsOutputTypeDef = TypedDict(
     "DescribeTapeRecoveryPointsOutputTypeDef",
     {
         "GatewayARN": str,
         "TapeRecoveryPointInfos": List[TapeRecoveryPointInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTapesOutputTypeDef = TypedDict(
     "DescribeTapesOutputTypeDef",
     {
         "Tapes": List[TapeTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VTLDeviceTypeDef = TypedDict(
     "VTLDeviceTypeDef",
     {
         "VTLDeviceARN": str,
@@ -2822,25 +2822,25 @@
 )
 
 ListLocalDisksOutputTypeDef = TypedDict(
     "ListLocalDisksOutputTypeDef",
     {
         "GatewayARN": str,
         "Disks": List[DiskTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFileSharesOutputTypeDef = TypedDict(
     "ListFileSharesOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileShareInfoList": List[FileShareInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FileSystemAssociationInfoTypeDef = TypedDict(
     "FileSystemAssociationInfoTypeDef",
     {
         "FileSystemAssociationARN": str,
@@ -2858,114 +2858,114 @@
 
 ListFileSystemAssociationsOutputTypeDef = TypedDict(
     "ListFileSystemAssociationsOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileSystemAssociationSummaryList": List[FileSystemAssociationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGatewaysOutputTypeDef = TypedDict(
     "ListGatewaysOutputTypeDef",
     {
         "Gateways": List[GatewayInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTapePoolsOutputTypeDef = TypedDict(
     "ListTapePoolsOutputTypeDef",
     {
         "PoolInfos": List[PoolInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTapesOutputTypeDef = TypedDict(
     "ListTapesOutputTypeDef",
     {
         "TapeInfos": List[TapeInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVolumeRecoveryPointsOutputTypeDef = TypedDict(
     "ListVolumeRecoveryPointsOutputTypeDef",
     {
         "GatewayARN": str,
         "VolumeRecoveryPointInfos": List[VolumeRecoveryPointInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVolumesOutputTypeDef = TypedDict(
     "ListVolumesOutputTypeDef",
     {
         "GatewayARN": str,
         "Marker": str,
         "VolumeInfos": List[VolumeInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSMBFileSharesOutputTypeDef = TypedDict(
     "DescribeSMBFileSharesOutputTypeDef",
     {
         "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAutomaticTapeCreationPoliciesOutputTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     {
         "AutomaticTapeCreationPolicyInfos": List[AutomaticTapeCreationPolicyInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCachediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesOutputTypeDef",
     {
         "CachediSCSIVolumes": List[CachediSCSIVolumeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStorediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeStorediSCSIVolumesOutputTypeDef",
     {
         "StorediSCSIVolumes": List[StorediSCSIVolumeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeNFSFileSharesOutputTypeDef = TypedDict(
     "DescribeNFSFileSharesOutputTypeDef",
     {
         "NFSFileShareInfoList": List[NFSFileShareInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVTLDevicesOutputTypeDef = TypedDict(
     "DescribeVTLDevicesOutputTypeDef",
     {
         "GatewayARN": str,
         "VTLDevices": List[VTLDeviceTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFileSystemAssociationsOutputTypeDef = TypedDict(
     "DescribeFileSystemAssociationsOutputTypeDef",
     {
         "FileSystemAssociationInfoList": List[FileSystemAssociationInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway/type_defs.pyi` & `mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -32,187 +32,198 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "ActivateGatewayOutputTypeDef",
     "AddCacheInputRequestTypeDef",
+    "AddCacheOutputTypeDef",
+    "AddTagsToResourceOutputTypeDef",
     "AddUploadBufferInputRequestTypeDef",
+    "AddUploadBufferOutputTypeDef",
     "AddWorkingStorageInputRequestTypeDef",
+    "AddWorkingStorageOutputTypeDef",
     "AssignTapePoolInputRequestTypeDef",
+    "AssignTapePoolOutputTypeDef",
     "CacheAttributesTypeDef",
     "EndpointNetworkConfigurationTypeDef",
+    "AssociateFileSystemOutputTypeDef",
     "AttachVolumeInputRequestTypeDef",
+    "AttachVolumeOutputTypeDef",
     "AutomaticTapeCreationRuleTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
     "VolumeiSCSIAttributesTypeDef",
     "CancelArchivalInputRequestTypeDef",
+    "CancelArchivalOutputTypeDef",
     "CancelRetrievalInputRequestTypeDef",
+    "CancelRetrievalOutputTypeDef",
     "ChapInfoTypeDef",
+    "CreateCachediSCSIVolumeOutputTypeDef",
     "NFSFileShareDefaultsTypeDef",
+    "CreateNFSFileShareOutputTypeDef",
+    "CreateSMBFileShareOutputTypeDef",
+    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
+    "CreateSnapshotOutputTypeDef",
+    "CreateStorediSCSIVolumeOutputTypeDef",
+    "CreateTapePoolOutputTypeDef",
+    "CreateTapeWithBarcodeOutputTypeDef",
+    "CreateTapesOutputTypeDef",
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
+    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
     "DeleteBandwidthRateLimitInputRequestTypeDef",
+    "DeleteBandwidthRateLimitOutputTypeDef",
     "DeleteChapCredentialsInputRequestTypeDef",
+    "DeleteChapCredentialsOutputTypeDef",
     "DeleteFileShareInputRequestTypeDef",
+    "DeleteFileShareOutputTypeDef",
     "DeleteGatewayInputRequestTypeDef",
+    "DeleteGatewayOutputTypeDef",
     "DeleteSnapshotScheduleInputRequestTypeDef",
+    "DeleteSnapshotScheduleOutputTypeDef",
     "DeleteTapeArchiveInputRequestTypeDef",
+    "DeleteTapeArchiveOutputTypeDef",
     "DeleteTapeInputRequestTypeDef",
+    "DeleteTapeOutputTypeDef",
     "DeleteTapePoolInputRequestTypeDef",
+    "DeleteTapePoolOutputTypeDef",
     "DeleteVolumeInputRequestTypeDef",
+    "DeleteVolumeOutputTypeDef",
     "DescribeAvailabilityMonitorTestInputRequestTypeDef",
+    "DescribeAvailabilityMonitorTestOutputTypeDef",
     "DescribeBandwidthRateLimitInputRequestTypeDef",
+    "DescribeBandwidthRateLimitOutputTypeDef",
     "DescribeBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCacheInputRequestTypeDef",
+    "DescribeCacheOutputTypeDef",
     "DescribeCachediSCSIVolumesInputRequestTypeDef",
     "DescribeChapCredentialsInputRequestTypeDef",
     "DescribeFileSystemAssociationsInputRequestTypeDef",
     "DescribeGatewayInformationInputRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
+    "DescribeMaintenanceStartTimeOutputTypeDef",
     "DescribeNFSFileSharesInputRequestTypeDef",
     "DescribeSMBFileSharesInputRequestTypeDef",
     "DescribeSMBSettingsInputRequestTypeDef",
     "SMBLocalGroupsTypeDef",
     "DescribeSnapshotScheduleInputRequestTypeDef",
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
     "DescribeTapeArchivesInputRequestTypeDef",
     "TapeArchiveTypeDef",
+    "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
     "DescribeTapeRecoveryPointsInputRequestTypeDef",
     "TapeRecoveryPointInfoTypeDef",
+    "DescribeTapesInputDescribeTapesPaginateTypeDef",
     "DescribeTapesInputRequestTypeDef",
     "TapeTypeDef",
     "DescribeUploadBufferInputRequestTypeDef",
+    "DescribeUploadBufferOutputTypeDef",
+    "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
     "DescribeVTLDevicesInputRequestTypeDef",
     "DescribeWorkingStorageInputRequestTypeDef",
+    "DescribeWorkingStorageOutputTypeDef",
     "DetachVolumeInputRequestTypeDef",
+    "DetachVolumeOutputTypeDef",
     "DeviceiSCSIAttributesTypeDef",
     "DisableGatewayInputRequestTypeDef",
+    "DisableGatewayOutputTypeDef",
     "DisassociateFileSystemInputRequestTypeDef",
+    "DisassociateFileSystemOutputTypeDef",
     "DiskTypeDef",
     "FileShareInfoTypeDef",
     "FileSystemAssociationStatusDetailTypeDef",
     "FileSystemAssociationSummaryTypeDef",
     "GatewayInfoTypeDef",
     "JoinDomainInputRequestTypeDef",
+    "JoinDomainOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
+    "ListFileSharesInputListFileSharesPaginateTypeDef",
     "ListFileSharesInputRequestTypeDef",
+    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
     "ListFileSystemAssociationsInputRequestTypeDef",
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
     "ListGatewaysInputRequestTypeDef",
     "ListLocalDisksInputRequestTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
     "ListTapePoolsInputRequestTypeDef",
     "PoolInfoTypeDef",
+    "ListTapesInputListTapesPaginateTypeDef",
     "ListTapesInputRequestTypeDef",
     "TapeInfoTypeDef",
     "ListVolumeInitiatorsInputRequestTypeDef",
+    "ListVolumeInitiatorsOutputTypeDef",
     "ListVolumeRecoveryPointsInputRequestTypeDef",
     "VolumeRecoveryPointInfoTypeDef",
+    "ListVolumesInputListVolumesPaginateTypeDef",
     "ListVolumesInputRequestTypeDef",
     "VolumeInfoTypeDef",
     "NotifyWhenUploadedInputRequestTypeDef",
+    "NotifyWhenUploadedOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "RefreshCacheInputRequestTypeDef",
+    "RefreshCacheOutputTypeDef",
     "RemoveTagsFromResourceInputRequestTypeDef",
+    "RemoveTagsFromResourceOutputTypeDef",
     "ResetCacheInputRequestTypeDef",
+    "ResetCacheOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "RetrieveTapeArchiveInputRequestTypeDef",
+    "RetrieveTapeArchiveOutputTypeDef",
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
+    "RetrieveTapeRecoveryPointOutputTypeDef",
     "SetLocalConsolePasswordInputRequestTypeDef",
+    "SetLocalConsolePasswordOutputTypeDef",
     "SetSMBGuestPasswordInputRequestTypeDef",
+    "SetSMBGuestPasswordOutputTypeDef",
     "ShutdownGatewayInputRequestTypeDef",
+    "ShutdownGatewayOutputTypeDef",
     "StartAvailabilityMonitorTestInputRequestTypeDef",
+    "StartAvailabilityMonitorTestOutputTypeDef",
     "StartGatewayInputRequestTypeDef",
+    "StartGatewayOutputTypeDef",
+    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
     "UpdateBandwidthRateLimitInputRequestTypeDef",
+    "UpdateBandwidthRateLimitOutputTypeDef",
+    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
     "UpdateChapCredentialsInputRequestTypeDef",
+    "UpdateChapCredentialsOutputTypeDef",
+    "UpdateFileSystemAssociationOutputTypeDef",
     "UpdateGatewayInformationInputRequestTypeDef",
+    "UpdateGatewayInformationOutputTypeDef",
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
+    "UpdateGatewaySoftwareNowOutputTypeDef",
     "UpdateMaintenanceStartTimeInputRequestTypeDef",
+    "UpdateMaintenanceStartTimeOutputTypeDef",
+    "UpdateNFSFileShareOutputTypeDef",
+    "UpdateSMBFileShareOutputTypeDef",
     "UpdateSMBFileShareVisibilityInputRequestTypeDef",
+    "UpdateSMBFileShareVisibilityOutputTypeDef",
+    "UpdateSMBLocalGroupsOutputTypeDef",
     "UpdateSMBSecurityStrategyInputRequestTypeDef",
+    "UpdateSMBSecurityStrategyOutputTypeDef",
+    "UpdateSnapshotScheduleOutputTypeDef",
     "UpdateVTLDeviceTypeInputRequestTypeDef",
+    "UpdateVTLDeviceTypeOutputTypeDef",
     "ActivateGatewayInputRequestTypeDef",
     "AddTagsToResourceInputRequestTypeDef",
     "CreateCachediSCSIVolumeInputRequestTypeDef",
     "CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef",
     "CreateSnapshotInputRequestTypeDef",
     "CreateStorediSCSIVolumeInputRequestTypeDef",
     "CreateTapePoolInputRequestTypeDef",
     "CreateTapeWithBarcodeInputRequestTypeDef",
     "CreateTapesInputRequestTypeDef",
-    "UpdateSnapshotScheduleInputRequestTypeDef",
-    "ActivateGatewayOutputTypeDef",
-    "AddCacheOutputTypeDef",
-    "AddTagsToResourceOutputTypeDef",
-    "AddUploadBufferOutputTypeDef",
-    "AddWorkingStorageOutputTypeDef",
-    "AssignTapePoolOutputTypeDef",
-    "AssociateFileSystemOutputTypeDef",
-    "AttachVolumeOutputTypeDef",
-    "CancelArchivalOutputTypeDef",
-    "CancelRetrievalOutputTypeDef",
-    "CreateCachediSCSIVolumeOutputTypeDef",
-    "CreateNFSFileShareOutputTypeDef",
-    "CreateSMBFileShareOutputTypeDef",
-    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
-    "CreateSnapshotOutputTypeDef",
-    "CreateStorediSCSIVolumeOutputTypeDef",
-    "CreateTapePoolOutputTypeDef",
-    "CreateTapeWithBarcodeOutputTypeDef",
-    "CreateTapesOutputTypeDef",
-    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
-    "DeleteBandwidthRateLimitOutputTypeDef",
-    "DeleteChapCredentialsOutputTypeDef",
-    "DeleteFileShareOutputTypeDef",
-    "DeleteGatewayOutputTypeDef",
-    "DeleteSnapshotScheduleOutputTypeDef",
-    "DeleteTapeArchiveOutputTypeDef",
-    "DeleteTapeOutputTypeDef",
-    "DeleteTapePoolOutputTypeDef",
-    "DeleteVolumeOutputTypeDef",
-    "DescribeAvailabilityMonitorTestOutputTypeDef",
-    "DescribeBandwidthRateLimitOutputTypeDef",
-    "DescribeCacheOutputTypeDef",
-    "DescribeMaintenanceStartTimeOutputTypeDef",
     "DescribeSnapshotScheduleOutputTypeDef",
-    "DescribeUploadBufferOutputTypeDef",
-    "DescribeWorkingStorageOutputTypeDef",
-    "DetachVolumeOutputTypeDef",
-    "DisableGatewayOutputTypeDef",
-    "DisassociateFileSystemOutputTypeDef",
-    "JoinDomainOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "ListVolumeInitiatorsOutputTypeDef",
-    "NotifyWhenUploadedOutputTypeDef",
-    "RefreshCacheOutputTypeDef",
-    "RemoveTagsFromResourceOutputTypeDef",
-    "ResetCacheOutputTypeDef",
-    "RetrieveTapeArchiveOutputTypeDef",
-    "RetrieveTapeRecoveryPointOutputTypeDef",
-    "SetLocalConsolePasswordOutputTypeDef",
-    "SetSMBGuestPasswordOutputTypeDef",
-    "ShutdownGatewayOutputTypeDef",
-    "StartAvailabilityMonitorTestOutputTypeDef",
-    "StartGatewayOutputTypeDef",
-    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
-    "UpdateBandwidthRateLimitOutputTypeDef",
-    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
-    "UpdateChapCredentialsOutputTypeDef",
-    "UpdateFileSystemAssociationOutputTypeDef",
-    "UpdateGatewayInformationOutputTypeDef",
-    "UpdateGatewaySoftwareNowOutputTypeDef",
-    "UpdateMaintenanceStartTimeOutputTypeDef",
-    "UpdateNFSFileShareOutputTypeDef",
-    "UpdateSMBFileShareOutputTypeDef",
-    "UpdateSMBFileShareVisibilityOutputTypeDef",
-    "UpdateSMBLocalGroupsOutputTypeDef",
-    "UpdateSMBSecurityStrategyOutputTypeDef",
-    "UpdateSnapshotScheduleOutputTypeDef",
-    "UpdateVTLDeviceTypeOutputTypeDef",
+    "UpdateSnapshotScheduleInputRequestTypeDef",
     "CreateSMBFileShareInputRequestTypeDef",
     "SMBFileShareInfoTypeDef",
     "UpdateFileSystemAssociationInputRequestTypeDef",
     "UpdateSMBFileShareInputRequestTypeDef",
     "AssociateFileSystemInputRequestTypeDef",
     "AutomaticTapeCreationPolicyInfoTypeDef",
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
@@ -223,25 +234,14 @@
     "DescribeChapCredentialsOutputTypeDef",
     "CreateNFSFileShareInputRequestTypeDef",
     "NFSFileShareInfoTypeDef",
     "UpdateNFSFileShareInputRequestTypeDef",
     "DescribeGatewayInformationOutputTypeDef",
     "DescribeSMBSettingsOutputTypeDef",
     "UpdateSMBLocalGroupsInputRequestTypeDef",
-    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
-    "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
-    "DescribeTapesInputDescribeTapesPaginateTypeDef",
-    "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
-    "ListFileSharesInputListFileSharesPaginateTypeDef",
-    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
-    "ListTapesInputListTapesPaginateTypeDef",
-    "ListVolumesInputListVolumesPaginateTypeDef",
     "DescribeTapeArchivesOutputTypeDef",
     "DescribeTapeRecoveryPointsOutputTypeDef",
     "DescribeTapesOutputTypeDef",
     "VTLDeviceTypeDef",
     "ListLocalDisksOutputTypeDef",
     "ListFileSharesOutputTypeDef",
     "FileSystemAssociationInfoTypeDef",
@@ -264,49 +264,78 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ActivateGatewayOutputTypeDef = TypedDict(
+    "ActivateGatewayOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddCacheInputRequestTypeDef = TypedDict(
     "AddCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
+AddCacheOutputTypeDef = TypedDict(
+    "AddCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AddTagsToResourceOutputTypeDef = TypedDict(
+    "AddTagsToResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AddUploadBufferInputRequestTypeDef = TypedDict(
     "AddUploadBufferInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
+AddUploadBufferOutputTypeDef = TypedDict(
+    "AddUploadBufferOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AddWorkingStorageInputRequestTypeDef = TypedDict(
     "AddWorkingStorageInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
+AddWorkingStorageOutputTypeDef = TypedDict(
+    "AddWorkingStorageOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAssignTapePoolInputRequestTypeDef = TypedDict(
     "_RequiredAssignTapePoolInputRequestTypeDef",
     {
         "TapeARN": str,
         "PoolId": str,
     },
 )
@@ -319,14 +348,22 @@
 )
 
 class AssignTapePoolInputRequestTypeDef(
     _RequiredAssignTapePoolInputRequestTypeDef, _OptionalAssignTapePoolInputRequestTypeDef
 ):
     pass
 
+AssignTapePoolOutputTypeDef = TypedDict(
+    "AssignTapePoolOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CacheAttributesTypeDef = TypedDict(
     "CacheAttributesTypeDef",
     {
         "CacheStaleTimeoutInSeconds": int,
     },
     total=False,
 )
@@ -335,14 +372,22 @@
     "EndpointNetworkConfigurationTypeDef",
     {
         "IpAddresses": Sequence[str],
     },
     total=False,
 )
 
+AssociateFileSystemOutputTypeDef = TypedDict(
+    "AssociateFileSystemOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAttachVolumeInputRequestTypeDef = TypedDict(
     "_RequiredAttachVolumeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "VolumeARN": str,
         "NetworkInterfaceId": str,
     },
@@ -357,14 +402,23 @@
 )
 
 class AttachVolumeInputRequestTypeDef(
     _RequiredAttachVolumeInputRequestTypeDef, _OptionalAttachVolumeInputRequestTypeDef
 ):
     pass
 
+AttachVolumeOutputTypeDef = TypedDict(
+    "AttachVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "TargetARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAutomaticTapeCreationRuleTypeDef = TypedDict(
     "_RequiredAutomaticTapeCreationRuleTypeDef",
     {
         "TapeBarcodePrefix": str,
         "PoolId": str,
         "TapeSizeInBytes": int,
         "MinimumNumTapes": int,
@@ -423,67 +477,186 @@
     "CancelArchivalInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
 
+CancelArchivalOutputTypeDef = TypedDict(
+    "CancelArchivalOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CancelRetrievalInputRequestTypeDef = TypedDict(
     "CancelRetrievalInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
 
+CancelRetrievalOutputTypeDef = TypedDict(
+    "CancelRetrievalOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ChapInfoTypeDef = TypedDict(
     "ChapInfoTypeDef",
     {
         "TargetARN": str,
         "SecretToAuthenticateInitiator": str,
         "InitiatorName": str,
         "SecretToAuthenticateTarget": str,
     },
     total=False,
 )
 
+CreateCachediSCSIVolumeOutputTypeDef = TypedDict(
+    "CreateCachediSCSIVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "TargetARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 NFSFileShareDefaultsTypeDef = TypedDict(
     "NFSFileShareDefaultsTypeDef",
     {
         "FileMode": str,
         "DirectoryMode": str,
         "GroupId": int,
         "OwnerId": int,
     },
     total=False,
 )
 
+CreateNFSFileShareOutputTypeDef = TypedDict(
+    "CreateNFSFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSMBFileShareOutputTypeDef = TypedDict(
+    "CreateSMBFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSnapshotFromVolumeRecoveryPointOutputTypeDef = TypedDict(
+    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
+    {
+        "SnapshotId": str,
+        "VolumeARN": str,
+        "VolumeRecoveryPointTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSnapshotOutputTypeDef = TypedDict(
+    "CreateSnapshotOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "SnapshotId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateStorediSCSIVolumeOutputTypeDef = TypedDict(
+    "CreateStorediSCSIVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "VolumeSizeInBytes": int,
+        "TargetARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateTapePoolOutputTypeDef = TypedDict(
+    "CreateTapePoolOutputTypeDef",
+    {
+        "PoolARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateTapeWithBarcodeOutputTypeDef = TypedDict(
+    "CreateTapeWithBarcodeOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateTapesOutputTypeDef = TypedDict(
+    "CreateTapesOutputTypeDef",
+    {
+        "TapeARNs": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteAutomaticTapeCreationPolicyInputRequestTypeDef = TypedDict(
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DeleteAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
+    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "DeleteBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
         "BandwidthType": str,
     },
 )
 
+DeleteBandwidthRateLimitOutputTypeDef = TypedDict(
+    "DeleteBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteChapCredentialsInputRequestTypeDef = TypedDict(
     "DeleteChapCredentialsInputRequestTypeDef",
     {
         "TargetARN": str,
         "InitiatorName": str,
     },
 )
 
+DeleteChapCredentialsOutputTypeDef = TypedDict(
+    "DeleteChapCredentialsOutputTypeDef",
+    {
+        "TargetARN": str,
+        "InitiatorName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteFileShareInputRequestTypeDef = TypedDict(
     "_RequiredDeleteFileShareInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalDeleteFileShareInputRequestTypeDef = TypedDict(
@@ -495,28 +668,52 @@
 )
 
 class DeleteFileShareInputRequestTypeDef(
     _RequiredDeleteFileShareInputRequestTypeDef, _OptionalDeleteFileShareInputRequestTypeDef
 ):
     pass
 
+DeleteFileShareOutputTypeDef = TypedDict(
+    "DeleteFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteGatewayInputRequestTypeDef = TypedDict(
     "DeleteGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DeleteGatewayOutputTypeDef = TypedDict(
+    "DeleteGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSnapshotScheduleInputRequestTypeDef = TypedDict(
     "DeleteSnapshotScheduleInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
+DeleteSnapshotScheduleOutputTypeDef = TypedDict(
+    "DeleteSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteTapeArchiveInputRequestTypeDef = TypedDict(
     "_RequiredDeleteTapeArchiveInputRequestTypeDef",
     {
         "TapeARN": str,
     },
 )
 _OptionalDeleteTapeArchiveInputRequestTypeDef = TypedDict(
@@ -528,14 +725,22 @@
 )
 
 class DeleteTapeArchiveInputRequestTypeDef(
     _RequiredDeleteTapeArchiveInputRequestTypeDef, _OptionalDeleteTapeArchiveInputRequestTypeDef
 ):
     pass
 
+DeleteTapeArchiveOutputTypeDef = TypedDict(
+    "DeleteTapeArchiveOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteTapeInputRequestTypeDef = TypedDict(
     "_RequiredDeleteTapeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
@@ -548,56 +753,114 @@
 )
 
 class DeleteTapeInputRequestTypeDef(
     _RequiredDeleteTapeInputRequestTypeDef, _OptionalDeleteTapeInputRequestTypeDef
 ):
     pass
 
+DeleteTapeOutputTypeDef = TypedDict(
+    "DeleteTapeOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteTapePoolInputRequestTypeDef = TypedDict(
     "DeleteTapePoolInputRequestTypeDef",
     {
         "PoolARN": str,
     },
 )
 
+DeleteTapePoolOutputTypeDef = TypedDict(
+    "DeleteTapePoolOutputTypeDef",
+    {
+        "PoolARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteVolumeInputRequestTypeDef = TypedDict(
     "DeleteVolumeInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
+DeleteVolumeOutputTypeDef = TypedDict(
+    "DeleteVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeAvailabilityMonitorTestInputRequestTypeDef = TypedDict(
     "DescribeAvailabilityMonitorTestInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DescribeAvailabilityMonitorTestOutputTypeDef = TypedDict(
+    "DescribeAvailabilityMonitorTestOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "Status": AvailabilityMonitorTestStatusType,
+        "StartTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "DescribeBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DescribeBandwidthRateLimitOutputTypeDef = TypedDict(
+    "DescribeBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "AverageUploadRateLimitInBitsPerSec": int,
+        "AverageDownloadRateLimitInBitsPerSec": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
 DescribeCacheInputRequestTypeDef = TypedDict(
     "DescribeCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DescribeCacheOutputTypeDef = TypedDict(
+    "DescribeCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "CacheAllocatedInBytes": int,
+        "CacheUsedPercentage": float,
+        "CacheDirtyPercentage": float,
+        "CacheHitPercentage": float,
+        "CacheMissPercentage": float,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeCachediSCSIVolumesInputRequestTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesInputRequestTypeDef",
     {
         "VolumeARNs": Sequence[str],
     },
 )
 
@@ -635,14 +898,27 @@
 DescribeMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DescribeMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "DescribeMaintenanceStartTimeOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "HourOfDay": int,
+        "MinuteOfHour": int,
+        "DayOfWeek": int,
+        "DayOfMonth": int,
+        "Timezone": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeNFSFileSharesInputRequestTypeDef = TypedDict(
     "DescribeNFSFileSharesInputRequestTypeDef",
     {
         "FileShareARNList": Sequence[str],
     },
 )
 
@@ -678,20 +954,19 @@
 DescribeStorediSCSIVolumesInputRequestTypeDef = TypedDict(
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
     {
         "VolumeARNs": Sequence[str],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
+    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeTapeArchivesInputRequestTypeDef = TypedDict(
     "DescribeTapeArchivesInputRequestTypeDef",
     {
@@ -718,14 +993,34 @@
         "Worm": bool,
         "RetentionStartDate": datetime,
         "PoolEntryDate": datetime,
     },
     total=False,
 )
 
+_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
+    {
+        "GatewayARN": str,
+    },
+)
+_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef(
+    _RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+    _OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeTapeRecoveryPointsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTapeRecoveryPointsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeTapeRecoveryPointsInputRequestTypeDef = TypedDict(
@@ -750,14 +1045,35 @@
         "TapeRecoveryPointTime": datetime,
         "TapeSizeInBytes": int,
         "TapeStatus": str,
     },
     total=False,
 )
 
+_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+    },
+)
+_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeTapesInputDescribeTapesPaginateTypeDef(
+    _RequiredDescribeTapesInputDescribeTapesPaginateTypeDef,
+    _OptionalDescribeTapesInputDescribeTapesPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeTapesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTapesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeTapesInputRequestTypeDef = TypedDict(
@@ -798,14 +1114,46 @@
 DescribeUploadBufferInputRequestTypeDef = TypedDict(
     "DescribeUploadBufferInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DescribeUploadBufferOutputTypeDef = TypedDict(
+    "DescribeUploadBufferOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "UploadBufferUsedInBytes": int,
+        "UploadBufferAllocatedInBytes": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+    },
+)
+_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
+    {
+        "VTLDeviceARNs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef(
+    _RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+    _OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeVTLDevicesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVTLDevicesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeVTLDevicesInputRequestTypeDef = TypedDict(
@@ -826,14 +1174,25 @@
 DescribeWorkingStorageInputRequestTypeDef = TypedDict(
     "DescribeWorkingStorageInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DescribeWorkingStorageOutputTypeDef = TypedDict(
+    "DescribeWorkingStorageOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "WorkingStorageUsedInBytes": int,
+        "WorkingStorageAllocatedInBytes": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDetachVolumeInputRequestTypeDef = TypedDict(
     "_RequiredDetachVolumeInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 _OptionalDetachVolumeInputRequestTypeDef = TypedDict(
@@ -845,14 +1204,22 @@
 )
 
 class DetachVolumeInputRequestTypeDef(
     _RequiredDetachVolumeInputRequestTypeDef, _OptionalDetachVolumeInputRequestTypeDef
 ):
     pass
 
+DetachVolumeOutputTypeDef = TypedDict(
+    "DetachVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeviceiSCSIAttributesTypeDef = TypedDict(
     "DeviceiSCSIAttributesTypeDef",
     {
         "TargetARN": str,
         "NetworkInterfaceId": str,
         "NetworkInterfacePort": int,
         "ChapEnabled": bool,
@@ -863,14 +1230,22 @@
 DisableGatewayInputRequestTypeDef = TypedDict(
     "DisableGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+DisableGatewayOutputTypeDef = TypedDict(
+    "DisableGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDisassociateFileSystemInputRequestTypeDef = TypedDict(
     "_RequiredDisassociateFileSystemInputRequestTypeDef",
     {
         "FileSystemAssociationARN": str,
     },
 )
 _OptionalDisassociateFileSystemInputRequestTypeDef = TypedDict(
@@ -883,14 +1258,22 @@
 
 class DisassociateFileSystemInputRequestTypeDef(
     _RequiredDisassociateFileSystemInputRequestTypeDef,
     _OptionalDisassociateFileSystemInputRequestTypeDef,
 ):
     pass
 
+DisassociateFileSystemOutputTypeDef = TypedDict(
+    "DisassociateFileSystemOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DiskTypeDef = TypedDict(
     "DiskTypeDef",
     {
         "DiskId": str,
         "DiskPath": str,
         "DiskNode": str,
         "DiskStatus": str,
@@ -969,42 +1352,77 @@
 )
 
 class JoinDomainInputRequestTypeDef(
     _RequiredJoinDomainInputRequestTypeDef, _OptionalJoinDomainInputRequestTypeDef
 ):
     pass
 
+JoinDomainOutputTypeDef = TypedDict(
+    "JoinDomainOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ActiveDirectoryStatus": ActiveDirectoryStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListAutomaticTapeCreationPoliciesInputRequestTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
     total=False,
 )
 
+ListFileSharesInputListFileSharesPaginateTypeDef = TypedDict(
+    "ListFileSharesInputListFileSharesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFileSharesInputRequestTypeDef = TypedDict(
     "ListFileSharesInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef = TypedDict(
+    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFileSystemAssociationsInputRequestTypeDef = TypedDict(
     "ListFileSystemAssociationsInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGatewaysInputRequestTypeDef = TypedDict(
     "ListGatewaysInputRequestTypeDef",
     {
         "Marker": str,
         "Limit": int,
     },
     total=False,
@@ -1013,14 +1431,34 @@
 ListLocalDisksInputRequestTypeDef = TypedDict(
     "ListLocalDisksInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -1033,14 +1471,23 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
+ListTapePoolsInputListTapePoolsPaginateTypeDef = TypedDict(
+    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
+    {
+        "PoolARNs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTapePoolsInputRequestTypeDef = TypedDict(
     "ListTapePoolsInputRequestTypeDef",
     {
         "PoolARNs": Sequence[str],
         "Marker": str,
         "Limit": int,
     },
@@ -1056,14 +1503,23 @@
         "RetentionLockType": RetentionLockTypeType,
         "RetentionLockTimeInDays": int,
         "PoolStatus": PoolStatusType,
     },
     total=False,
 )
 
+ListTapesInputListTapesPaginateTypeDef = TypedDict(
+    "ListTapesInputListTapesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTapesInputRequestTypeDef = TypedDict(
     "ListTapesInputRequestTypeDef",
     {
         "TapeARNs": Sequence[str],
         "Marker": str,
         "Limit": int,
     },
@@ -1088,14 +1544,22 @@
 ListVolumeInitiatorsInputRequestTypeDef = TypedDict(
     "ListVolumeInitiatorsInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
+ListVolumeInitiatorsOutputTypeDef = TypedDict(
+    "ListVolumeInitiatorsOutputTypeDef",
+    {
+        "Initiators": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListVolumeRecoveryPointsInputRequestTypeDef = TypedDict(
     "ListVolumeRecoveryPointsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
@@ -1106,14 +1570,23 @@
         "VolumeSizeInBytes": int,
         "VolumeUsageInBytes": int,
         "VolumeRecoveryPointTime": str,
     },
     total=False,
 )
 
+ListVolumesInputListVolumesPaginateTypeDef = TypedDict(
+    "ListVolumesInputListVolumesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListVolumesInputRequestTypeDef = TypedDict(
     "ListVolumesInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Marker": str,
         "Limit": int,
     },
@@ -1137,14 +1610,33 @@
 NotifyWhenUploadedInputRequestTypeDef = TypedDict(
     "NotifyWhenUploadedInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 
+NotifyWhenUploadedOutputTypeDef = TypedDict(
+    "NotifyWhenUploadedOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "NotificationId": str,
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
 _RequiredRefreshCacheInputRequestTypeDef = TypedDict(
     "_RequiredRefreshCacheInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalRefreshCacheInputRequestTypeDef = TypedDict(
@@ -1157,82 +1649,182 @@
 )
 
 class RefreshCacheInputRequestTypeDef(
     _RequiredRefreshCacheInputRequestTypeDef, _OptionalRefreshCacheInputRequestTypeDef
 ):
     pass
 
+RefreshCacheOutputTypeDef = TypedDict(
+    "RefreshCacheOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "NotificationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveTagsFromResourceInputRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+RemoveTagsFromResourceOutputTypeDef = TypedDict(
+    "RemoveTagsFromResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ResetCacheInputRequestTypeDef = TypedDict(
     "ResetCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+ResetCacheOutputTypeDef = TypedDict(
+    "ResetCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
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
 RetrieveTapeArchiveInputRequestTypeDef = TypedDict(
     "RetrieveTapeArchiveInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
 
+RetrieveTapeArchiveOutputTypeDef = TypedDict(
+    "RetrieveTapeArchiveOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RetrieveTapeRecoveryPointInputRequestTypeDef = TypedDict(
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
 
+RetrieveTapeRecoveryPointOutputTypeDef = TypedDict(
+    "RetrieveTapeRecoveryPointOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetLocalConsolePasswordInputRequestTypeDef = TypedDict(
     "SetLocalConsolePasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "LocalConsolePassword": str,
     },
 )
 
+SetLocalConsolePasswordOutputTypeDef = TypedDict(
+    "SetLocalConsolePasswordOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetSMBGuestPasswordInputRequestTypeDef = TypedDict(
     "SetSMBGuestPasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Password": str,
     },
 )
 
+SetSMBGuestPasswordOutputTypeDef = TypedDict(
+    "SetSMBGuestPasswordOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ShutdownGatewayInputRequestTypeDef = TypedDict(
     "ShutdownGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+ShutdownGatewayOutputTypeDef = TypedDict(
+    "ShutdownGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartAvailabilityMonitorTestInputRequestTypeDef = TypedDict(
     "StartAvailabilityMonitorTestInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+StartAvailabilityMonitorTestOutputTypeDef = TypedDict(
+    "StartAvailabilityMonitorTestOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartGatewayInputRequestTypeDef = TypedDict(
     "StartGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+StartGatewayOutputTypeDef = TypedDict(
+    "StartGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
+    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "_RequiredUpdateBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalUpdateBandwidthRateLimitInputRequestTypeDef = TypedDict(
@@ -1246,14 +1838,30 @@
 
 class UpdateBandwidthRateLimitInputRequestTypeDef(
     _RequiredUpdateBandwidthRateLimitInputRequestTypeDef,
     _OptionalUpdateBandwidthRateLimitInputRequestTypeDef,
 ):
     pass
 
+UpdateBandwidthRateLimitOutputTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateChapCredentialsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateChapCredentialsInputRequestTypeDef",
     {
         "TargetARN": str,
         "SecretToAuthenticateInitiator": str,
         "InitiatorName": str,
     },
@@ -1268,14 +1876,31 @@
 
 class UpdateChapCredentialsInputRequestTypeDef(
     _RequiredUpdateChapCredentialsInputRequestTypeDef,
     _OptionalUpdateChapCredentialsInputRequestTypeDef,
 ):
     pass
 
+UpdateChapCredentialsOutputTypeDef = TypedDict(
+    "UpdateChapCredentialsOutputTypeDef",
+    {
+        "TargetARN": str,
+        "InitiatorName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateFileSystemAssociationOutputTypeDef = TypedDict(
+    "UpdateFileSystemAssociationOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateGatewayInformationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayInformationInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalUpdateGatewayInformationInputRequestTypeDef = TypedDict(
@@ -1291,21 +1916,38 @@
 
 class UpdateGatewayInformationInputRequestTypeDef(
     _RequiredUpdateGatewayInformationInputRequestTypeDef,
     _OptionalUpdateGatewayInformationInputRequestTypeDef,
 ):
     pass
 
+UpdateGatewayInformationOutputTypeDef = TypedDict(
+    "UpdateGatewayInformationOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "GatewayName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateGatewaySoftwareNowInputRequestTypeDef = TypedDict(
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
+UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
+    "UpdateGatewaySoftwareNowOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
@@ -1321,38 +1963,102 @@
 
 class UpdateMaintenanceStartTimeInputRequestTypeDef(
     _RequiredUpdateMaintenanceStartTimeInputRequestTypeDef,
     _OptionalUpdateMaintenanceStartTimeInputRequestTypeDef,
 ):
     pass
 
+UpdateMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "UpdateMaintenanceStartTimeOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateNFSFileShareOutputTypeDef = TypedDict(
+    "UpdateNFSFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSMBFileShareOutputTypeDef = TypedDict(
+    "UpdateSMBFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateSMBFileShareVisibilityInputRequestTypeDef = TypedDict(
     "UpdateSMBFileShareVisibilityInputRequestTypeDef",
     {
         "GatewayARN": str,
         "FileSharesVisible": bool,
     },
 )
 
+UpdateSMBFileShareVisibilityOutputTypeDef = TypedDict(
+    "UpdateSMBFileShareVisibilityOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSMBLocalGroupsOutputTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateSMBSecurityStrategyInputRequestTypeDef = TypedDict(
     "UpdateSMBSecurityStrategyInputRequestTypeDef",
     {
         "GatewayARN": str,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
     },
 )
 
+UpdateSMBSecurityStrategyOutputTypeDef = TypedDict(
+    "UpdateSMBSecurityStrategyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSnapshotScheduleOutputTypeDef = TypedDict(
+    "UpdateSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateVTLDeviceTypeInputRequestTypeDef = TypedDict(
     "UpdateVTLDeviceTypeInputRequestTypeDef",
     {
         "VTLDeviceARN": str,
         "DeviceType": str,
     },
 )
 
+UpdateVTLDeviceTypeOutputTypeDef = TypedDict(
+    "UpdateVTLDeviceTypeOutputTypeDef",
+    {
+        "VTLDeviceARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredActivateGatewayInputRequestTypeDef = TypedDict(
     "_RequiredActivateGatewayInputRequestTypeDef",
     {
         "ActivationKey": str,
         "GatewayName": str,
         "GatewayTimezone": str,
         "GatewayRegion": str,
@@ -1549,622 +2255,60 @@
 )
 
 class CreateTapesInputRequestTypeDef(
     _RequiredCreateTapesInputRequestTypeDef, _OptionalCreateTapesInputRequestTypeDef
 ):
     pass
 
-_RequiredUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateSnapshotScheduleInputRequestTypeDef",
-    {
-        "VolumeARN": str,
-        "StartAt": int,
-        "RecurrenceInHours": int,
-    },
-)
-_OptionalUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateSnapshotScheduleInputRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class UpdateSnapshotScheduleInputRequestTypeDef(
-    _RequiredUpdateSnapshotScheduleInputRequestTypeDef,
-    _OptionalUpdateSnapshotScheduleInputRequestTypeDef,
-):
-    pass
-
-ActivateGatewayOutputTypeDef = TypedDict(
-    "ActivateGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddCacheOutputTypeDef = TypedDict(
-    "AddCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddTagsToResourceOutputTypeDef = TypedDict(
-    "AddTagsToResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddUploadBufferOutputTypeDef = TypedDict(
-    "AddUploadBufferOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddWorkingStorageOutputTypeDef = TypedDict(
-    "AddWorkingStorageOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssignTapePoolOutputTypeDef = TypedDict(
-    "AssignTapePoolOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateFileSystemOutputTypeDef = TypedDict(
-    "AssociateFileSystemOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AttachVolumeOutputTypeDef = TypedDict(
-    "AttachVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "TargetARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelArchivalOutputTypeDef = TypedDict(
-    "CancelArchivalOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelRetrievalOutputTypeDef = TypedDict(
-    "CancelRetrievalOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCachediSCSIVolumeOutputTypeDef = TypedDict(
-    "CreateCachediSCSIVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "TargetARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateNFSFileShareOutputTypeDef = TypedDict(
-    "CreateNFSFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSMBFileShareOutputTypeDef = TypedDict(
-    "CreateSMBFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSnapshotFromVolumeRecoveryPointOutputTypeDef = TypedDict(
-    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
-    {
-        "SnapshotId": str,
-        "VolumeARN": str,
-        "VolumeRecoveryPointTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSnapshotOutputTypeDef = TypedDict(
-    "CreateSnapshotOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "SnapshotId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateStorediSCSIVolumeOutputTypeDef = TypedDict(
-    "CreateStorediSCSIVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "VolumeSizeInBytes": int,
-        "TargetARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTapePoolOutputTypeDef = TypedDict(
-    "CreateTapePoolOutputTypeDef",
-    {
-        "PoolARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTapeWithBarcodeOutputTypeDef = TypedDict(
-    "CreateTapeWithBarcodeOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTapesOutputTypeDef = TypedDict(
-    "CreateTapesOutputTypeDef",
-    {
-        "TapeARNs": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
-    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBandwidthRateLimitOutputTypeDef = TypedDict(
-    "DeleteBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteChapCredentialsOutputTypeDef = TypedDict(
-    "DeleteChapCredentialsOutputTypeDef",
-    {
-        "TargetARN": str,
-        "InitiatorName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFileShareOutputTypeDef = TypedDict(
-    "DeleteFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteGatewayOutputTypeDef = TypedDict(
-    "DeleteGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSnapshotScheduleOutputTypeDef = TypedDict(
-    "DeleteSnapshotScheduleOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteTapeArchiveOutputTypeDef = TypedDict(
-    "DeleteTapeArchiveOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteTapeOutputTypeDef = TypedDict(
-    "DeleteTapeOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteTapePoolOutputTypeDef = TypedDict(
-    "DeleteTapePoolOutputTypeDef",
-    {
-        "PoolARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteVolumeOutputTypeDef = TypedDict(
-    "DeleteVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAvailabilityMonitorTestOutputTypeDef = TypedDict(
-    "DescribeAvailabilityMonitorTestOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "Status": AvailabilityMonitorTestStatusType,
-        "StartTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBandwidthRateLimitOutputTypeDef = TypedDict(
-    "DescribeBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "AverageUploadRateLimitInBitsPerSec": int,
-        "AverageDownloadRateLimitInBitsPerSec": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeCacheOutputTypeDef = TypedDict(
-    "DescribeCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "CacheAllocatedInBytes": int,
-        "CacheUsedPercentage": float,
-        "CacheDirtyPercentage": float,
-        "CacheHitPercentage": float,
-        "CacheMissPercentage": float,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "DescribeMaintenanceStartTimeOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "HourOfDay": int,
-        "MinuteOfHour": int,
-        "DayOfWeek": int,
-        "DayOfMonth": int,
-        "Timezone": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeSnapshotScheduleOutputTypeDef = TypedDict(
     "DescribeSnapshotScheduleOutputTypeDef",
     {
         "VolumeARN": str,
         "StartAt": int,
         "RecurrenceInHours": int,
         "Description": str,
         "Timezone": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeUploadBufferOutputTypeDef = TypedDict(
-    "DescribeUploadBufferOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "UploadBufferUsedInBytes": int,
-        "UploadBufferAllocatedInBytes": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeWorkingStorageOutputTypeDef = TypedDict(
-    "DescribeWorkingStorageOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "WorkingStorageUsedInBytes": int,
-        "WorkingStorageAllocatedInBytes": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetachVolumeOutputTypeDef = TypedDict(
-    "DetachVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisableGatewayOutputTypeDef = TypedDict(
-    "DisableGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateFileSystemOutputTypeDef = TypedDict(
-    "DisassociateFileSystemOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-JoinDomainOutputTypeDef = TypedDict(
-    "JoinDomainOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ActiveDirectoryStatus": ActiveDirectoryStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "ResourceARN": str,
         "Marker": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListVolumeInitiatorsOutputTypeDef = TypedDict(
-    "ListVolumeInitiatorsOutputTypeDef",
-    {
-        "Initiators": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-NotifyWhenUploadedOutputTypeDef = TypedDict(
-    "NotifyWhenUploadedOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "NotificationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RefreshCacheOutputTypeDef = TypedDict(
-    "RefreshCacheOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "NotificationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveTagsFromResourceOutputTypeDef = TypedDict(
-    "RemoveTagsFromResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ResetCacheOutputTypeDef = TypedDict(
-    "ResetCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RetrieveTapeArchiveOutputTypeDef = TypedDict(
-    "RetrieveTapeArchiveOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RetrieveTapeRecoveryPointOutputTypeDef = TypedDict(
-    "RetrieveTapeRecoveryPointOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetLocalConsolePasswordOutputTypeDef = TypedDict(
-    "SetLocalConsolePasswordOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetSMBGuestPasswordOutputTypeDef = TypedDict(
-    "SetSMBGuestPasswordOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ShutdownGatewayOutputTypeDef = TypedDict(
-    "ShutdownGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartAvailabilityMonitorTestOutputTypeDef = TypedDict(
-    "StartAvailabilityMonitorTestOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartGatewayOutputTypeDef = TypedDict(
-    "StartGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
-    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateBandwidthRateLimitOutputTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateChapCredentialsOutputTypeDef = TypedDict(
-    "UpdateChapCredentialsOutputTypeDef",
-    {
-        "TargetARN": str,
-        "InitiatorName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFileSystemAssociationOutputTypeDef = TypedDict(
-    "UpdateFileSystemAssociationOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGatewayInformationOutputTypeDef = TypedDict(
-    "UpdateGatewayInformationOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "GatewayName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
-    "UpdateGatewaySoftwareNowOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "UpdateMaintenanceStartTimeOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateNFSFileShareOutputTypeDef = TypedDict(
-    "UpdateNFSFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSMBFileShareOutputTypeDef = TypedDict(
-    "UpdateSMBFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSMBFileShareVisibilityOutputTypeDef = TypedDict(
-    "UpdateSMBFileShareVisibilityOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSMBLocalGroupsOutputTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateSMBSecurityStrategyOutputTypeDef = TypedDict(
-    "UpdateSMBSecurityStrategyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSnapshotScheduleOutputTypeDef = TypedDict(
-    "UpdateSnapshotScheduleOutputTypeDef",
+_RequiredUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateSnapshotScheduleInputRequestTypeDef",
     {
         "VolumeARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "StartAt": int,
+        "RecurrenceInHours": int,
     },
 )
-
-UpdateVTLDeviceTypeOutputTypeDef = TypedDict(
-    "UpdateVTLDeviceTypeOutputTypeDef",
+_OptionalUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateSnapshotScheduleInputRequestTypeDef",
     {
-        "VTLDeviceARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
+class UpdateSnapshotScheduleInputRequestTypeDef(
+    _RequiredUpdateSnapshotScheduleInputRequestTypeDef,
+    _OptionalUpdateSnapshotScheduleInputRequestTypeDef,
+):
+    pass
+
 _RequiredCreateSMBFileShareInputRequestTypeDef = TypedDict(
     "_RequiredCreateSMBFileShareInputRequestTypeDef",
     {
         "ClientToken": str,
         "GatewayARN": str,
         "Role": str,
         "LocationARN": str,
@@ -2343,15 +2487,15 @@
 )
 
 DescribeBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
     {
         "GatewayARN": str,
         "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     {
         "GatewayARN": str,
@@ -2401,15 +2545,15 @@
     total=False,
 )
 
 DescribeChapCredentialsOutputTypeDef = TypedDict(
     "DescribeChapCredentialsOutputTypeDef",
     {
         "ChapCredentials": List[ChapInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateNFSFileShareInputRequestTypeDef = TypedDict(
     "_RequiredCreateNFSFileShareInputRequestTypeDef",
     {
         "ClientToken": str,
@@ -2530,209 +2674,65 @@
         "HostEnvironment": HostEnvironmentType,
         "EndpointType": str,
         "SoftwareUpdatesEndDate": str,
         "DeprecationDate": str,
         "GatewayCapacity": GatewayCapacityType,
         "SupportedGatewayCapacities": List[GatewayCapacityType],
         "HostEnvironmentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSMBSettingsOutputTypeDef = TypedDict(
     "DescribeSMBSettingsOutputTypeDef",
     {
         "GatewayARN": str,
         "DomainName": str,
         "ActiveDirectoryStatus": ActiveDirectoryStatusType,
         "SMBGuestPasswordSet": bool,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
         "FileSharesVisible": bool,
         "SMBLocalGroups": SMBLocalGroupsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
     "UpdateSMBLocalGroupsInputRequestTypeDef",
     {
         "GatewayARN": str,
         "SMBLocalGroups": SMBLocalGroupsTypeDef,
     },
 )
 
-DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
-    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
-    {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef(
-    _RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
-    _OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef",
-    {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeTapesInputDescribeTapesPaginateTypeDef(
-    _RequiredDescribeTapesInputDescribeTapesPaginateTypeDef,
-    _OptionalDescribeTapesInputDescribeTapesPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
-    {
-        "VTLDeviceARNs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef(
-    _RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
-    _OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
-):
-    pass
-
-ListFileSharesInputListFileSharesPaginateTypeDef = TypedDict(
-    "ListFileSharesInputListFileSharesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef = TypedDict(
-    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-ListTapePoolsInputListTapePoolsPaginateTypeDef = TypedDict(
-    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
-    {
-        "PoolARNs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTapesInputListTapesPaginateTypeDef = TypedDict(
-    "ListTapesInputListTapesPaginateTypeDef",
-    {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListVolumesInputListVolumesPaginateTypeDef = TypedDict(
-    "ListVolumesInputListVolumesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeTapeArchivesOutputTypeDef = TypedDict(
     "DescribeTapeArchivesOutputTypeDef",
     {
         "TapeArchives": List[TapeArchiveTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTapeRecoveryPointsOutputTypeDef = TypedDict(
     "DescribeTapeRecoveryPointsOutputTypeDef",
     {
         "GatewayARN": str,
         "TapeRecoveryPointInfos": List[TapeRecoveryPointInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTapesOutputTypeDef = TypedDict(
     "DescribeTapesOutputTypeDef",
     {
         "Tapes": List[TapeTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VTLDeviceTypeDef = TypedDict(
     "VTLDeviceTypeDef",
     {
         "VTLDeviceARN": str,
@@ -2745,25 +2745,25 @@
 )
 
 ListLocalDisksOutputTypeDef = TypedDict(
     "ListLocalDisksOutputTypeDef",
     {
         "GatewayARN": str,
         "Disks": List[DiskTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFileSharesOutputTypeDef = TypedDict(
     "ListFileSharesOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileShareInfoList": List[FileShareInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FileSystemAssociationInfoTypeDef = TypedDict(
     "FileSystemAssociationInfoTypeDef",
     {
         "FileSystemAssociationARN": str,
@@ -2781,114 +2781,114 @@
 
 ListFileSystemAssociationsOutputTypeDef = TypedDict(
     "ListFileSystemAssociationsOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileSystemAssociationSummaryList": List[FileSystemAssociationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGatewaysOutputTypeDef = TypedDict(
     "ListGatewaysOutputTypeDef",
     {
         "Gateways": List[GatewayInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTapePoolsOutputTypeDef = TypedDict(
     "ListTapePoolsOutputTypeDef",
     {
         "PoolInfos": List[PoolInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTapesOutputTypeDef = TypedDict(
     "ListTapesOutputTypeDef",
     {
         "TapeInfos": List[TapeInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVolumeRecoveryPointsOutputTypeDef = TypedDict(
     "ListVolumeRecoveryPointsOutputTypeDef",
     {
         "GatewayARN": str,
         "VolumeRecoveryPointInfos": List[VolumeRecoveryPointInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVolumesOutputTypeDef = TypedDict(
     "ListVolumesOutputTypeDef",
     {
         "GatewayARN": str,
         "Marker": str,
         "VolumeInfos": List[VolumeInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSMBFileSharesOutputTypeDef = TypedDict(
     "DescribeSMBFileSharesOutputTypeDef",
     {
         "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAutomaticTapeCreationPoliciesOutputTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     {
         "AutomaticTapeCreationPolicyInfos": List[AutomaticTapeCreationPolicyInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCachediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesOutputTypeDef",
     {
         "CachediSCSIVolumes": List[CachediSCSIVolumeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStorediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeStorediSCSIVolumesOutputTypeDef",
     {
         "StorediSCSIVolumes": List[StorediSCSIVolumeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeNFSFileSharesOutputTypeDef = TypedDict(
     "DescribeNFSFileSharesOutputTypeDef",
     {
         "NFSFileShareInfoList": List[NFSFileShareInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVTLDevicesOutputTypeDef = TypedDict(
     "DescribeVTLDevicesOutputTypeDef",
     {
         "GatewayARN": str,
         "VTLDevices": List[VTLDeviceTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFileSystemAssociationsOutputTypeDef = TypedDict(
     "DescribeFileSystemAssociationsOutputTypeDef",
     {
         "FileSystemAssociationInfoList": List[FileSystemAssociationInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway.egg-info/PKG-INFO` & `mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-storagegateway
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.StorageGateway 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.StorageGateway 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/
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
 
 <a id="mypy-boto3-storagegateway"></a>
 
 # mypy-boto3-storagegateway
 
 [![PyPI - mypy-boto3-storagegateway](https://img.shields.io/pypi/v/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-storagegateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-storagegateway)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-storagegateway?color=blue)](https://pypistats.org/packages/mypy-boto3-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.StorageGateway 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
+[boto3.StorageGateway 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [mypy-boto3-storagegateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -373,187 +374,198 @@
 
 `mypy_boto3_storagegateway.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_storagegateway.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    ActivateGatewayOutputTypeDef,
     AddCacheInputRequestTypeDef,
+    AddCacheOutputTypeDef,
+    AddTagsToResourceOutputTypeDef,
     AddUploadBufferInputRequestTypeDef,
+    AddUploadBufferOutputTypeDef,
     AddWorkingStorageInputRequestTypeDef,
+    AddWorkingStorageOutputTypeDef,
     AssignTapePoolInputRequestTypeDef,
+    AssignTapePoolOutputTypeDef,
     CacheAttributesTypeDef,
     EndpointNetworkConfigurationTypeDef,
+    AssociateFileSystemOutputTypeDef,
     AttachVolumeInputRequestTypeDef,
+    AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     VolumeiSCSIAttributesTypeDef,
     CancelArchivalInputRequestTypeDef,
+    CancelArchivalOutputTypeDef,
     CancelRetrievalInputRequestTypeDef,
+    CancelRetrievalOutputTypeDef,
     ChapInfoTypeDef,
+    CreateCachediSCSIVolumeOutputTypeDef,
     NFSFileShareDefaultsTypeDef,
+    CreateNFSFileShareOutputTypeDef,
+    CreateSMBFileShareOutputTypeDef,
+    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
+    CreateSnapshotOutputTypeDef,
+    CreateStorediSCSIVolumeOutputTypeDef,
+    CreateTapePoolOutputTypeDef,
+    CreateTapeWithBarcodeOutputTypeDef,
+    CreateTapesOutputTypeDef,
     DeleteAutomaticTapeCreationPolicyInputRequestTypeDef,
+    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
     DeleteBandwidthRateLimitInputRequestTypeDef,
+    DeleteBandwidthRateLimitOutputTypeDef,
     DeleteChapCredentialsInputRequestTypeDef,
+    DeleteChapCredentialsOutputTypeDef,
     DeleteFileShareInputRequestTypeDef,
+    DeleteFileShareOutputTypeDef,
     DeleteGatewayInputRequestTypeDef,
+    DeleteGatewayOutputTypeDef,
     DeleteSnapshotScheduleInputRequestTypeDef,
+    DeleteSnapshotScheduleOutputTypeDef,
     DeleteTapeArchiveInputRequestTypeDef,
+    DeleteTapeArchiveOutputTypeDef,
     DeleteTapeInputRequestTypeDef,
+    DeleteTapeOutputTypeDef,
     DeleteTapePoolInputRequestTypeDef,
+    DeleteTapePoolOutputTypeDef,
     DeleteVolumeInputRequestTypeDef,
+    DeleteVolumeOutputTypeDef,
     DescribeAvailabilityMonitorTestInputRequestTypeDef,
+    DescribeAvailabilityMonitorTestOutputTypeDef,
     DescribeBandwidthRateLimitInputRequestTypeDef,
+    DescribeBandwidthRateLimitOutputTypeDef,
     DescribeBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCacheInputRequestTypeDef,
+    DescribeCacheOutputTypeDef,
     DescribeCachediSCSIVolumesInputRequestTypeDef,
     DescribeChapCredentialsInputRequestTypeDef,
     DescribeFileSystemAssociationsInputRequestTypeDef,
     DescribeGatewayInformationInputRequestTypeDef,
     NetworkInterfaceTypeDef,
     DescribeMaintenanceStartTimeInputRequestTypeDef,
+    DescribeMaintenanceStartTimeOutputTypeDef,
     DescribeNFSFileSharesInputRequestTypeDef,
     DescribeSMBFileSharesInputRequestTypeDef,
     DescribeSMBSettingsInputRequestTypeDef,
     SMBLocalGroupsTypeDef,
     DescribeSnapshotScheduleInputRequestTypeDef,
     DescribeStorediSCSIVolumesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
     DescribeTapeArchivesInputRequestTypeDef,
     TapeArchiveTypeDef,
+    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
     DescribeTapeRecoveryPointsInputRequestTypeDef,
     TapeRecoveryPointInfoTypeDef,
+    DescribeTapesInputDescribeTapesPaginateTypeDef,
     DescribeTapesInputRequestTypeDef,
     TapeTypeDef,
     DescribeUploadBufferInputRequestTypeDef,
+    DescribeUploadBufferOutputTypeDef,
+    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
     DescribeVTLDevicesInputRequestTypeDef,
     DescribeWorkingStorageInputRequestTypeDef,
+    DescribeWorkingStorageOutputTypeDef,
     DetachVolumeInputRequestTypeDef,
+    DetachVolumeOutputTypeDef,
     DeviceiSCSIAttributesTypeDef,
     DisableGatewayInputRequestTypeDef,
+    DisableGatewayOutputTypeDef,
     DisassociateFileSystemInputRequestTypeDef,
+    DisassociateFileSystemOutputTypeDef,
     DiskTypeDef,
     FileShareInfoTypeDef,
     FileSystemAssociationStatusDetailTypeDef,
     FileSystemAssociationSummaryTypeDef,
     GatewayInfoTypeDef,
     JoinDomainInputRequestTypeDef,
+    JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesInputRequestTypeDef,
+    ListFileSharesInputListFileSharesPaginateTypeDef,
     ListFileSharesInputRequestTypeDef,
+    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
     ListFileSystemAssociationsInputRequestTypeDef,
+    ListGatewaysInputListGatewaysPaginateTypeDef,
     ListGatewaysInputRequestTypeDef,
     ListLocalDisksInputRequestTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTapePoolsInputListTapePoolsPaginateTypeDef,
     ListTapePoolsInputRequestTypeDef,
     PoolInfoTypeDef,
+    ListTapesInputListTapesPaginateTypeDef,
     ListTapesInputRequestTypeDef,
     TapeInfoTypeDef,
     ListVolumeInitiatorsInputRequestTypeDef,
+    ListVolumeInitiatorsOutputTypeDef,
     ListVolumeRecoveryPointsInputRequestTypeDef,
     VolumeRecoveryPointInfoTypeDef,
+    ListVolumesInputListVolumesPaginateTypeDef,
     ListVolumesInputRequestTypeDef,
     VolumeInfoTypeDef,
     NotifyWhenUploadedInputRequestTypeDef,
+    NotifyWhenUploadedOutputTypeDef,
+    PaginatorConfigTypeDef,
     RefreshCacheInputRequestTypeDef,
+    RefreshCacheOutputTypeDef,
     RemoveTagsFromResourceInputRequestTypeDef,
+    RemoveTagsFromResourceOutputTypeDef,
     ResetCacheInputRequestTypeDef,
+    ResetCacheOutputTypeDef,
+    ResponseMetadataTypeDef,
     RetrieveTapeArchiveInputRequestTypeDef,
+    RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointInputRequestTypeDef,
+    RetrieveTapeRecoveryPointOutputTypeDef,
     SetLocalConsolePasswordInputRequestTypeDef,
+    SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordInputRequestTypeDef,
+    SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayInputRequestTypeDef,
+    ShutdownGatewayOutputTypeDef,
     StartAvailabilityMonitorTestInputRequestTypeDef,
+    StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayInputRequestTypeDef,
+    StartGatewayOutputTypeDef,
+    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitInputRequestTypeDef,
+    UpdateBandwidthRateLimitOutputTypeDef,
+    UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsInputRequestTypeDef,
+    UpdateChapCredentialsOutputTypeDef,
+    UpdateFileSystemAssociationOutputTypeDef,
     UpdateGatewayInformationInputRequestTypeDef,
+    UpdateGatewayInformationOutputTypeDef,
     UpdateGatewaySoftwareNowInputRequestTypeDef,
+    UpdateGatewaySoftwareNowOutputTypeDef,
     UpdateMaintenanceStartTimeInputRequestTypeDef,
+    UpdateMaintenanceStartTimeOutputTypeDef,
+    UpdateNFSFileShareOutputTypeDef,
+    UpdateSMBFileShareOutputTypeDef,
     UpdateSMBFileShareVisibilityInputRequestTypeDef,
+    UpdateSMBFileShareVisibilityOutputTypeDef,
+    UpdateSMBLocalGroupsOutputTypeDef,
     UpdateSMBSecurityStrategyInputRequestTypeDef,
+    UpdateSMBSecurityStrategyOutputTypeDef,
+    UpdateSnapshotScheduleOutputTypeDef,
     UpdateVTLDeviceTypeInputRequestTypeDef,
+    UpdateVTLDeviceTypeOutputTypeDef,
     ActivateGatewayInputRequestTypeDef,
     AddTagsToResourceInputRequestTypeDef,
     CreateCachediSCSIVolumeInputRequestTypeDef,
     CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef,
     CreateSnapshotInputRequestTypeDef,
     CreateStorediSCSIVolumeInputRequestTypeDef,
     CreateTapePoolInputRequestTypeDef,
     CreateTapeWithBarcodeInputRequestTypeDef,
     CreateTapesInputRequestTypeDef,
-    UpdateSnapshotScheduleInputRequestTypeDef,
-    ActivateGatewayOutputTypeDef,
-    AddCacheOutputTypeDef,
-    AddTagsToResourceOutputTypeDef,
-    AddUploadBufferOutputTypeDef,
-    AddWorkingStorageOutputTypeDef,
-    AssignTapePoolOutputTypeDef,
-    AssociateFileSystemOutputTypeDef,
-    AttachVolumeOutputTypeDef,
-    CancelArchivalOutputTypeDef,
-    CancelRetrievalOutputTypeDef,
-    CreateCachediSCSIVolumeOutputTypeDef,
-    CreateNFSFileShareOutputTypeDef,
-    CreateSMBFileShareOutputTypeDef,
-    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
-    CreateSnapshotOutputTypeDef,
-    CreateStorediSCSIVolumeOutputTypeDef,
-    CreateTapePoolOutputTypeDef,
-    CreateTapeWithBarcodeOutputTypeDef,
-    CreateTapesOutputTypeDef,
-    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
-    DeleteBandwidthRateLimitOutputTypeDef,
-    DeleteChapCredentialsOutputTypeDef,
-    DeleteFileShareOutputTypeDef,
-    DeleteGatewayOutputTypeDef,
-    DeleteSnapshotScheduleOutputTypeDef,
-    DeleteTapeArchiveOutputTypeDef,
-    DeleteTapeOutputTypeDef,
-    DeleteTapePoolOutputTypeDef,
-    DeleteVolumeOutputTypeDef,
-    DescribeAvailabilityMonitorTestOutputTypeDef,
-    DescribeBandwidthRateLimitOutputTypeDef,
-    DescribeCacheOutputTypeDef,
-    DescribeMaintenanceStartTimeOutputTypeDef,
     DescribeSnapshotScheduleOutputTypeDef,
-    DescribeUploadBufferOutputTypeDef,
-    DescribeWorkingStorageOutputTypeDef,
-    DetachVolumeOutputTypeDef,
-    DisableGatewayOutputTypeDef,
-    DisassociateFileSystemOutputTypeDef,
-    JoinDomainOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    ListVolumeInitiatorsOutputTypeDef,
-    NotifyWhenUploadedOutputTypeDef,
-    RefreshCacheOutputTypeDef,
-    RemoveTagsFromResourceOutputTypeDef,
-    ResetCacheOutputTypeDef,
-    RetrieveTapeArchiveOutputTypeDef,
-    RetrieveTapeRecoveryPointOutputTypeDef,
-    SetLocalConsolePasswordOutputTypeDef,
-    SetSMBGuestPasswordOutputTypeDef,
-    ShutdownGatewayOutputTypeDef,
-    StartAvailabilityMonitorTestOutputTypeDef,
-    StartGatewayOutputTypeDef,
-    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
-    UpdateBandwidthRateLimitOutputTypeDef,
-    UpdateBandwidthRateLimitScheduleOutputTypeDef,
-    UpdateChapCredentialsOutputTypeDef,
-    UpdateFileSystemAssociationOutputTypeDef,
-    UpdateGatewayInformationOutputTypeDef,
-    UpdateGatewaySoftwareNowOutputTypeDef,
-    UpdateMaintenanceStartTimeOutputTypeDef,
-    UpdateNFSFileShareOutputTypeDef,
-    UpdateSMBFileShareOutputTypeDef,
-    UpdateSMBFileShareVisibilityOutputTypeDef,
-    UpdateSMBLocalGroupsOutputTypeDef,
-    UpdateSMBSecurityStrategyOutputTypeDef,
-    UpdateSnapshotScheduleOutputTypeDef,
-    UpdateVTLDeviceTypeOutputTypeDef,
+    UpdateSnapshotScheduleInputRequestTypeDef,
     CreateSMBFileShareInputRequestTypeDef,
     SMBFileShareInfoTypeDef,
     UpdateFileSystemAssociationInputRequestTypeDef,
     UpdateSMBFileShareInputRequestTypeDef,
     AssociateFileSystemInputRequestTypeDef,
     AutomaticTapeCreationPolicyInfoTypeDef,
     UpdateAutomaticTapeCreationPolicyInputRequestTypeDef,
@@ -564,25 +576,14 @@
     DescribeChapCredentialsOutputTypeDef,
     CreateNFSFileShareInputRequestTypeDef,
     NFSFileShareInfoTypeDef,
     UpdateNFSFileShareInputRequestTypeDef,
     DescribeGatewayInformationOutputTypeDef,
     DescribeSMBSettingsOutputTypeDef,
     UpdateSMBLocalGroupsInputRequestTypeDef,
-    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
-    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
-    DescribeTapesInputDescribeTapesPaginateTypeDef,
-    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
-    ListFileSharesInputListFileSharesPaginateTypeDef,
-    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ListTapePoolsInputListTapePoolsPaginateTypeDef,
-    ListTapesInputListTapesPaginateTypeDef,
-    ListVolumesInputListVolumesPaginateTypeDef,
     DescribeTapeArchivesOutputTypeDef,
     DescribeTapeRecoveryPointsOutputTypeDef,
     DescribeTapesOutputTypeDef,
     VTLDeviceTypeDef,
     ListLocalDisksOutputTypeDef,
     ListFileSharesOutputTypeDef,
     FileSystemAssociationInfoTypeDef,
@@ -609,42 +610,42 @@
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

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/mypy_boto3_storagegateway.egg-info/SOURCES.txt` & `mypy-boto3-storagegateway-1.27.0/mypy_boto3_storagegateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-storagegateway-1.26.0.post1/setup.py` & `mypy-boto3-storagegateway-1.27.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-storagegateway.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-storagegateway",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_storagegateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.StorageGateway 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.StorageGateway 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
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
     keywords="boto3 storagegateway type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_storagegateway": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_storagegateway": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_storagegateway/",
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


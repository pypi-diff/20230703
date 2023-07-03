# Comparing `tmp/mypy-boto3-fsx-1.26.37.tar.gz` & `tmp/mypy-boto3-fsx-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fsx-1.26.37.tar", last modified: Fri Dec 23 20:32:30 2022, max compression
+gzip compressed data, was "mypy-boto3-fsx-1.27.0.tar", last modified: Mon Jul  3 19:50:47 2023, max compression
```

## Comparing `mypy-boto3-fsx-1.26.37.tar` & `mypy-boto3-fsx-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:30.588941 mypy-boto3-fsx-1.26.37/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21998 2022-12-23 20:32:30.584941 mypy-boto3-fsx-1.26.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20527 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:30.580941 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38793 2022-12-23 20:32:17.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38740 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14469 2022-12-23 20:32:17.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14467 2022-12-23 20:32:17.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2022-12-23 20:32:17.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2022-12-23 20:32:17.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    79078 2022-12-23 20:32:18.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    78981 2022-12-23 20:32:17.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:30.584941 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21998 2022-12-23 20:32:30.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2022-12-23 20:32:30.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 20:32:30.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 20:32:30.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-23 20:32:30.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-23 20:32:30.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 20:32:30.588941 mypy-boto3-fsx-1.26.37/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.979278 mypy-boto3-fsx-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-07-03 19:50:47.979278 mypy-boto3-fsx-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.979278 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38786 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38733 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14867 2023-07-03 19:38:05.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79400 2023-07-03 19:38:07.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79303 2023-07-03 19:38:05.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.979278 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-07-03 19:50:47.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:50:47.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:47.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:47.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:47.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:47.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:47.979278 mypy-boto3-fsx-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/setup.py
```

### Comparing `mypy-boto3-fsx-1.26.37/LICENSE` & `mypy-boto3-fsx-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-fsx-1.26.37/PKG-INFO` & `mypy-boto3-fsx-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fsx
-Version: 1.26.37
-Summary: Type annotations for boto3.FSx 1.26.37 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.FSx 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-fsx"></a>
 
 # mypy-boto3-fsx
 
 [![PyPI - mypy-boto3-fsx](https://img.shields.io/pypi/v/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fsx?color=blue)](https://pypistats.org/packages/mypy-boto3-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FSx 1.26.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[boto3.FSx 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-fsx docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/).
 
 See how it helps to find and fix potential bugs:
 
@@ -393,82 +393,84 @@
 
 ```python
 from mypy_boto3_fsx.type_defs import (
     ActiveDirectoryBackupAttributesTypeDef,
     AdministrativeActionFailureDetailsTypeDef,
     AliasTypeDef,
     AssociateFileSystemAliasesRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AutoExportPolicyTypeDef,
     AutoImportPolicyTypeDef,
     BackupFailureDetailsTypeDef,
     TagTypeDef,
     CancelDataRepositoryTaskRequestRequestTypeDef,
+    CancelDataRepositoryTaskResponseTypeDef,
     CompletionReportTypeDef,
     FileCacheLustreMetadataConfigurationTypeDef,
+    CreateFileSystemFromBackupResponseTypeDef,
     LustreLogCreateConfigurationTypeDef,
     LustreRootSquashConfigurationTypeDef,
     DiskIopsConfigurationTypeDef,
+    CreateFileSystemResponseTypeDef,
     SelfManagedActiveDirectoryConfigurationTypeDef,
     WindowsAuditLogCreateConfigurationTypeDef,
     TieringPolicyTypeDef,
     CreateOpenZFSOriginSnapshotConfigurationTypeDef,
     OpenZFSUserOrGroupQuotaTypeDef,
     DataRepositoryFailureDetailsTypeDef,
     DataRepositoryTaskFailureDetailsTypeDef,
     DataRepositoryTaskFilterTypeDef,
     DataRepositoryTaskStatusTypeDef,
     DeleteBackupRequestRequestTypeDef,
+    DeleteBackupResponseTypeDef,
     DeleteDataRepositoryAssociationRequestRequestTypeDef,
+    DeleteDataRepositoryAssociationResponseTypeDef,
     DeleteFileCacheRequestRequestTypeDef,
+    DeleteFileCacheResponseTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
+    DeleteSnapshotResponseTypeDef,
     DeleteStorageVirtualMachineRequestRequestTypeDef,
+    DeleteStorageVirtualMachineResponseTypeDef,
     DeleteVolumeOpenZFSConfigurationTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
     DescribeFileCachesRequestRequestTypeDef,
     DescribeFileSystemAliasesRequestRequestTypeDef,
+    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
+    DescribeFileSystemsResponseTypeDef,
     SnapshotFilterTypeDef,
     StorageVirtualMachineFilterTypeDef,
     VolumeFilterTypeDef,
     DisassociateFileSystemAliasesRequestRequestTypeDef,
     FileCacheFailureDetailsTypeDef,
     FileCacheNFSConfigurationTypeDef,
     LustreLogConfigurationTypeDef,
     FileSystemEndpointTypeDef,
     FileSystemFailureDetailsTypeDef,
     LifecycleTransitionReasonTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     OpenZFSClientConfigurationTypeDef,
     OpenZFSOriginSnapshotConfigurationTypeDef,
+    PaginatorConfigTypeDef,
     ReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
+    ReleaseFileSystemNfsV3LocksResponseTypeDef,
+    ResponseMetadataTypeDef,
     RestoreVolumeFromSnapshotRequestRequestTypeDef,
+    RestoreVolumeFromSnapshotResponseTypeDef,
     SelfManagedActiveDirectoryAttributesTypeDef,
     SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
     SvmEndpointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
+    UpdateFileSystemResponseTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     WindowsAuditLogConfigurationTypeDef,
     AssociateFileSystemAliasesResponseTypeDef,
-    CancelDataRepositoryTaskResponseTypeDef,
-    CreateFileSystemFromBackupResponseTypeDef,
-    CreateFileSystemResponseTypeDef,
-    DeleteBackupResponseTypeDef,
-    DeleteDataRepositoryAssociationResponseTypeDef,
-    DeleteFileCacheResponseTypeDef,
-    DeleteSnapshotResponseTypeDef,
-    DeleteStorageVirtualMachineResponseTypeDef,
     DescribeFileSystemAliasesResponseTypeDef,
-    DescribeFileSystemsResponseTypeDef,
     DisassociateFileSystemAliasesResponseTypeDef,
-    ReleaseFileSystemNfsV3LocksResponseTypeDef,
-    RestoreVolumeFromSnapshotResponseTypeDef,
-    UpdateFileSystemResponseTypeDef,
     NFSDataRepositoryConfigurationTypeDef,
     S3DataRepositoryConfigurationTypeDef,
     CopyBackupRequestRequestTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     DeleteFileSystemLustreConfigurationTypeDef,
     DeleteFileSystemLustreResponseTypeDef,
@@ -492,19 +494,17 @@
     CreateFileSystemWindowsConfigurationTypeDef,
     CreateOntapVolumeConfigurationTypeDef,
     OntapVolumeConfigurationTypeDef,
     UpdateOntapVolumeConfigurationTypeDef,
     DataRepositoryConfigurationTypeDef,
     DescribeDataRepositoryTasksRequestRequestTypeDef,
     DataRepositoryTaskTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeBackupsRequestRequestTypeDef,
     DescribeDataRepositoryAssociationsRequestRequestTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
-    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef,
     DescribeStorageVirtualMachinesRequestRequestTypeDef,
     DescribeVolumesRequestDescribeVolumesPaginateTypeDef,
     DescribeVolumesRequestRequestTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
     FileCacheLustreConfigurationTypeDef,
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

### Comparing `mypy-boto3-fsx-1.26.37/README.md` & `mypy-boto3-fsx-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-fsx"></a>
 
 # mypy-boto3-fsx
 
 [![PyPI - mypy-boto3-fsx](https://img.shields.io/pypi/v/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fsx?color=blue)](https://pypistats.org/packages/mypy-boto3-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FSx 1.26.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[boto3.FSx 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-fsx docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,82 +361,84 @@
 
 ```python
 from mypy_boto3_fsx.type_defs import (
     ActiveDirectoryBackupAttributesTypeDef,
     AdministrativeActionFailureDetailsTypeDef,
     AliasTypeDef,
     AssociateFileSystemAliasesRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AutoExportPolicyTypeDef,
     AutoImportPolicyTypeDef,
     BackupFailureDetailsTypeDef,
     TagTypeDef,
     CancelDataRepositoryTaskRequestRequestTypeDef,
+    CancelDataRepositoryTaskResponseTypeDef,
     CompletionReportTypeDef,
     FileCacheLustreMetadataConfigurationTypeDef,
+    CreateFileSystemFromBackupResponseTypeDef,
     LustreLogCreateConfigurationTypeDef,
     LustreRootSquashConfigurationTypeDef,
     DiskIopsConfigurationTypeDef,
+    CreateFileSystemResponseTypeDef,
     SelfManagedActiveDirectoryConfigurationTypeDef,
     WindowsAuditLogCreateConfigurationTypeDef,
     TieringPolicyTypeDef,
     CreateOpenZFSOriginSnapshotConfigurationTypeDef,
     OpenZFSUserOrGroupQuotaTypeDef,
     DataRepositoryFailureDetailsTypeDef,
     DataRepositoryTaskFailureDetailsTypeDef,
     DataRepositoryTaskFilterTypeDef,
     DataRepositoryTaskStatusTypeDef,
     DeleteBackupRequestRequestTypeDef,
+    DeleteBackupResponseTypeDef,
     DeleteDataRepositoryAssociationRequestRequestTypeDef,
+    DeleteDataRepositoryAssociationResponseTypeDef,
     DeleteFileCacheRequestRequestTypeDef,
+    DeleteFileCacheResponseTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
+    DeleteSnapshotResponseTypeDef,
     DeleteStorageVirtualMachineRequestRequestTypeDef,
+    DeleteStorageVirtualMachineResponseTypeDef,
     DeleteVolumeOpenZFSConfigurationTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
     DescribeFileCachesRequestRequestTypeDef,
     DescribeFileSystemAliasesRequestRequestTypeDef,
+    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
+    DescribeFileSystemsResponseTypeDef,
     SnapshotFilterTypeDef,
     StorageVirtualMachineFilterTypeDef,
     VolumeFilterTypeDef,
     DisassociateFileSystemAliasesRequestRequestTypeDef,
     FileCacheFailureDetailsTypeDef,
     FileCacheNFSConfigurationTypeDef,
     LustreLogConfigurationTypeDef,
     FileSystemEndpointTypeDef,
     FileSystemFailureDetailsTypeDef,
     LifecycleTransitionReasonTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     OpenZFSClientConfigurationTypeDef,
     OpenZFSOriginSnapshotConfigurationTypeDef,
+    PaginatorConfigTypeDef,
     ReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
+    ReleaseFileSystemNfsV3LocksResponseTypeDef,
+    ResponseMetadataTypeDef,
     RestoreVolumeFromSnapshotRequestRequestTypeDef,
+    RestoreVolumeFromSnapshotResponseTypeDef,
     SelfManagedActiveDirectoryAttributesTypeDef,
     SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
     SvmEndpointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
+    UpdateFileSystemResponseTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     WindowsAuditLogConfigurationTypeDef,
     AssociateFileSystemAliasesResponseTypeDef,
-    CancelDataRepositoryTaskResponseTypeDef,
-    CreateFileSystemFromBackupResponseTypeDef,
-    CreateFileSystemResponseTypeDef,
-    DeleteBackupResponseTypeDef,
-    DeleteDataRepositoryAssociationResponseTypeDef,
-    DeleteFileCacheResponseTypeDef,
-    DeleteSnapshotResponseTypeDef,
-    DeleteStorageVirtualMachineResponseTypeDef,
     DescribeFileSystemAliasesResponseTypeDef,
-    DescribeFileSystemsResponseTypeDef,
     DisassociateFileSystemAliasesResponseTypeDef,
-    ReleaseFileSystemNfsV3LocksResponseTypeDef,
-    RestoreVolumeFromSnapshotResponseTypeDef,
-    UpdateFileSystemResponseTypeDef,
     NFSDataRepositoryConfigurationTypeDef,
     S3DataRepositoryConfigurationTypeDef,
     CopyBackupRequestRequestTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     DeleteFileSystemLustreConfigurationTypeDef,
     DeleteFileSystemLustreResponseTypeDef,
@@ -460,19 +462,17 @@
     CreateFileSystemWindowsConfigurationTypeDef,
     CreateOntapVolumeConfigurationTypeDef,
     OntapVolumeConfigurationTypeDef,
     UpdateOntapVolumeConfigurationTypeDef,
     DataRepositoryConfigurationTypeDef,
     DescribeDataRepositoryTasksRequestRequestTypeDef,
     DataRepositoryTaskTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeBackupsRequestRequestTypeDef,
     DescribeDataRepositoryAssociationsRequestRequestTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
-    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef,
     DescribeStorageVirtualMachinesRequestRequestTypeDef,
     DescribeVolumesRequestDescribeVolumesPaginateTypeDef,
     DescribeVolumesRequestRequestTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
     FileCacheLustreConfigurationTypeDef,
@@ -546,42 +546,42 @@
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

### Comparing `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/__init__.py` & `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/__init__.pyi` & `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/__main__.py` & `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FSx 1.26.37\nVersion:         1.26.37\nBuilder version:"
-        " 7.12.2\nDocs:           "
+        "Type annotations for boto3.FSx 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.37")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/client.py` & `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -788,15 +788,15 @@
         *,
         StorageVirtualMachineId: str,
         ActiveDirectoryConfiguration: UpdateSvmActiveDirectoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         SvmAdminPassword: str = ...
     ) -> UpdateStorageVirtualMachineResponseTypeDef:
         """
-        Updates an Amazon FSx for ONTAP storage virtual machine (SVM).
+        Updates an FSx for ONTAP storage virtual machine (SVM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_storage_virtual_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_storage_virtual_machine)
         """
 
     def update_volume(
         self,
```

### Comparing `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/client.pyi` & `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -741,15 +741,15 @@
         *,
         StorageVirtualMachineId: str,
         ActiveDirectoryConfiguration: UpdateSvmActiveDirectoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         SvmAdminPassword: str = ...
     ) -> UpdateStorageVirtualMachineResponseTypeDef:
         """
-        Updates an Amazon FSx for ONTAP storage virtual machine (SVM).
+        Updates an FSx for ONTAP storage virtual machine (SVM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_storage_virtual_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_storage_virtual_machine)
         """
     def update_volume(
         self,
         *,
```

### Comparing `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/literals.py` & `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/literals.pyi`

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
     "AdministrativeActionTypeType",
     "AliasLifecycleType",
     "AutoImportPolicyTypeType",
     "BackupLifecycleType",
     "BackupTypeType",
     "DataCompressionTypeType",
@@ -80,15 +79,14 @@
     "FSxServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdministrativeActionTypeType = Literal[
     "FILE_SYSTEM_ALIAS_ASSOCIATION",
     "FILE_SYSTEM_ALIAS_DISASSOCIATION",
     "FILE_SYSTEM_UPDATE",
     "RELEASE_NFS_V3_LOCKS",
     "SNAPSHOT_UPDATE",
     "STORAGE_OPTIMIZATION",
@@ -200,14 +198,15 @@
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
@@ -228,31 +227,34 @@
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
@@ -331,14 +333,15 @@
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
@@ -349,18 +352,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -391,14 +396,15 @@
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
@@ -417,16 +423,19 @@
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
@@ -506,18 +515,21 @@
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
@@ -549,24 +561,29 @@
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

### Comparing `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/literals.pyi` & `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/literals.py`

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
     "AdministrativeActionTypeType",
     "AliasLifecycleType",
     "AutoImportPolicyTypeType",
     "BackupLifecycleType",
     "BackupTypeType",
     "DataCompressionTypeType",
@@ -79,14 +80,15 @@
     "FSxServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AdministrativeActionTypeType = Literal[
     "FILE_SYSTEM_ALIAS_ASSOCIATION",
     "FILE_SYSTEM_ALIAS_DISASSOCIATION",
     "FILE_SYSTEM_UPDATE",
     "RELEASE_NFS_V3_LOCKS",
     "SNAPSHOT_UPDATE",
     "STORAGE_OPTIMIZATION",
@@ -198,14 +200,15 @@
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
@@ -226,31 +229,34 @@
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
@@ -329,14 +335,15 @@
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
@@ -347,18 +354,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -389,14 +398,15 @@
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
@@ -415,16 +425,19 @@
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
@@ -504,18 +517,21 @@
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
@@ -547,24 +563,29 @@
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

### Comparing `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/paginator.py` & `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,30 +69,33 @@
     """
 
     def paginate(
         self,
         *,
         BackupIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describebackupspaginator)
         """
 
 
 class DescribeFileSystemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeFileSystems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describefilesystemspaginator)
     """
 
     def paginate(
-        self, *, FileSystemIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        FileSystemIds: Sequence[str] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeFileSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeFileSystems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describefilesystemspaginator)
         """
 
 
@@ -103,15 +106,15 @@
     """
 
     def paginate(
         self,
         *,
         StorageVirtualMachineIds: Sequence[str] = ...,
         Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeStorageVirtualMachinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeStorageVirtualMachines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describestoragevirtualmachinespaginator)
         """
 
 
@@ -122,28 +125,28 @@
     """
 
     def paginate(
         self,
         *,
         VolumeIds: Sequence[str] = ...,
         Filters: Sequence[VolumeFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeVolumesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeVolumes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describevolumespaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/paginator.pyi` & `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/paginator.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -66,29 +66,32 @@
     """
 
     def paginate(
         self,
         *,
         BackupIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describebackupspaginator)
         """
 
 class DescribeFileSystemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeFileSystems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describefilesystemspaginator)
     """
 
     def paginate(
-        self, *, FileSystemIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        FileSystemIds: Sequence[str] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeFileSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeFileSystems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describefilesystemspaginator)
         """
 
 class DescribeStorageVirtualMachinesPaginator(Paginator):
@@ -98,15 +101,15 @@
     """
 
     def paginate(
         self,
         *,
         StorageVirtualMachineIds: Sequence[str] = ...,
         Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeStorageVirtualMachinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeStorageVirtualMachines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describestoragevirtualmachinespaginator)
         """
 
 class DescribeVolumesPaginator(Paginator):
@@ -116,27 +119,27 @@
     """
 
     def paginate(
         self,
         *,
         VolumeIds: Sequence[str] = ...,
         Filters: Sequence[VolumeFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeVolumesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeVolumes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describevolumespaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/type_defs.py` & `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,82 +73,84 @@
 
 
 __all__ = (
     "ActiveDirectoryBackupAttributesTypeDef",
     "AdministrativeActionFailureDetailsTypeDef",
     "AliasTypeDef",
     "AssociateFileSystemAliasesRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AutoExportPolicyTypeDef",
     "AutoImportPolicyTypeDef",
     "BackupFailureDetailsTypeDef",
     "TagTypeDef",
     "CancelDataRepositoryTaskRequestRequestTypeDef",
+    "CancelDataRepositoryTaskResponseTypeDef",
     "CompletionReportTypeDef",
     "FileCacheLustreMetadataConfigurationTypeDef",
+    "CreateFileSystemFromBackupResponseTypeDef",
     "LustreLogCreateConfigurationTypeDef",
     "LustreRootSquashConfigurationTypeDef",
     "DiskIopsConfigurationTypeDef",
+    "CreateFileSystemResponseTypeDef",
     "SelfManagedActiveDirectoryConfigurationTypeDef",
     "WindowsAuditLogCreateConfigurationTypeDef",
     "TieringPolicyTypeDef",
     "CreateOpenZFSOriginSnapshotConfigurationTypeDef",
     "OpenZFSUserOrGroupQuotaTypeDef",
     "DataRepositoryFailureDetailsTypeDef",
     "DataRepositoryTaskFailureDetailsTypeDef",
     "DataRepositoryTaskFilterTypeDef",
     "DataRepositoryTaskStatusTypeDef",
     "DeleteBackupRequestRequestTypeDef",
+    "DeleteBackupResponseTypeDef",
     "DeleteDataRepositoryAssociationRequestRequestTypeDef",
+    "DeleteDataRepositoryAssociationResponseTypeDef",
     "DeleteFileCacheRequestRequestTypeDef",
+    "DeleteFileCacheResponseTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
+    "DeleteSnapshotResponseTypeDef",
     "DeleteStorageVirtualMachineRequestRequestTypeDef",
+    "DeleteStorageVirtualMachineResponseTypeDef",
     "DeleteVolumeOpenZFSConfigurationTypeDef",
     "FilterTypeDef",
-    "PaginatorConfigTypeDef",
     "DescribeFileCachesRequestRequestTypeDef",
     "DescribeFileSystemAliasesRequestRequestTypeDef",
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
     "DescribeFileSystemsRequestRequestTypeDef",
+    "DescribeFileSystemsResponseTypeDef",
     "SnapshotFilterTypeDef",
     "StorageVirtualMachineFilterTypeDef",
     "VolumeFilterTypeDef",
     "DisassociateFileSystemAliasesRequestRequestTypeDef",
     "FileCacheFailureDetailsTypeDef",
     "FileCacheNFSConfigurationTypeDef",
     "LustreLogConfigurationTypeDef",
     "FileSystemEndpointTypeDef",
     "FileSystemFailureDetailsTypeDef",
     "LifecycleTransitionReasonTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "OpenZFSClientConfigurationTypeDef",
     "OpenZFSOriginSnapshotConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
     "ReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
+    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreVolumeFromSnapshotRequestRequestTypeDef",
+    "RestoreVolumeFromSnapshotResponseTypeDef",
     "SelfManagedActiveDirectoryAttributesTypeDef",
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
     "SvmEndpointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileCacheLustreConfigurationTypeDef",
+    "UpdateFileSystemResponseTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "WindowsAuditLogConfigurationTypeDef",
     "AssociateFileSystemAliasesResponseTypeDef",
-    "CancelDataRepositoryTaskResponseTypeDef",
-    "CreateFileSystemFromBackupResponseTypeDef",
-    "CreateFileSystemResponseTypeDef",
-    "DeleteBackupResponseTypeDef",
-    "DeleteDataRepositoryAssociationResponseTypeDef",
-    "DeleteFileCacheResponseTypeDef",
-    "DeleteSnapshotResponseTypeDef",
-    "DeleteStorageVirtualMachineResponseTypeDef",
     "DescribeFileSystemAliasesResponseTypeDef",
-    "DescribeFileSystemsResponseTypeDef",
     "DisassociateFileSystemAliasesResponseTypeDef",
-    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
-    "RestoreVolumeFromSnapshotResponseTypeDef",
-    "UpdateFileSystemResponseTypeDef",
     "NFSDataRepositoryConfigurationTypeDef",
     "S3DataRepositoryConfigurationTypeDef",
     "CopyBackupRequestRequestTypeDef",
     "CreateBackupRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "DeleteFileSystemLustreConfigurationTypeDef",
     "DeleteFileSystemLustreResponseTypeDef",
@@ -172,19 +174,17 @@
     "CreateFileSystemWindowsConfigurationTypeDef",
     "CreateOntapVolumeConfigurationTypeDef",
     "OntapVolumeConfigurationTypeDef",
     "UpdateOntapVolumeConfigurationTypeDef",
     "DataRepositoryConfigurationTypeDef",
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
     "DataRepositoryTaskTypeDef",
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
     "DescribeDataRepositoryAssociationsRequestRequestTypeDef",
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeSnapshotsRequestRequestTypeDef",
     "DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef",
     "DescribeStorageVirtualMachinesRequestRequestTypeDef",
     "DescribeVolumesRequestDescribeVolumesPaginateTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
     "FileCacheDataRepositoryAssociationTypeDef",
     "FileCacheLustreConfigurationTypeDef",
@@ -296,25 +296,14 @@
 class AssociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredAssociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalAssociateFileSystemAliasesRequestRequestTypeDef,
 ):
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
 AutoExportPolicyTypeDef = TypedDict(
     "AutoExportPolicyTypeDef",
     {
         "Events": Sequence[EventTypeType],
     },
     total=False,
 )
@@ -346,14 +335,23 @@
 CancelDataRepositoryTaskRequestRequestTypeDef = TypedDict(
     "CancelDataRepositoryTaskRequestRequestTypeDef",
     {
         "TaskId": str,
     },
 )
 
+CancelDataRepositoryTaskResponseTypeDef = TypedDict(
+    "CancelDataRepositoryTaskResponseTypeDef",
+    {
+        "Lifecycle": DataRepositoryTaskLifecycleType,
+        "TaskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCompletionReportTypeDef = TypedDict(
     "_RequiredCompletionReportTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalCompletionReportTypeDef = TypedDict(
@@ -374,14 +372,22 @@
 FileCacheLustreMetadataConfigurationTypeDef = TypedDict(
     "FileCacheLustreMetadataConfigurationTypeDef",
     {
         "StorageCapacity": int,
     },
 )
 
+CreateFileSystemFromBackupResponseTypeDef = TypedDict(
+    "CreateFileSystemFromBackupResponseTypeDef",
+    {
+        "FileSystem": "FileSystemTypeDef",
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredLustreLogCreateConfigurationTypeDef = TypedDict(
     "_RequiredLustreLogCreateConfigurationTypeDef",
     {
         "Level": LustreAccessAuditLogLevelType,
     },
 )
 _OptionalLustreLogCreateConfigurationTypeDef = TypedDict(
@@ -413,14 +419,22 @@
     {
         "Mode": DiskIopsConfigurationModeType,
         "Iops": int,
     },
     total=False,
 )
 
+CreateFileSystemResponseTypeDef = TypedDict(
+    "CreateFileSystemResponseTypeDef",
+    {
+        "FileSystem": "FileSystemTypeDef",
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSelfManagedActiveDirectoryConfigurationTypeDef = TypedDict(
     "_RequiredSelfManagedActiveDirectoryConfigurationTypeDef",
     {
         "DomainName": str,
         "UserName": str,
         "Password": str,
         "DnsIps": Sequence[str],
@@ -546,14 +560,23 @@
 
 class DeleteBackupRequestRequestTypeDef(
     _RequiredDeleteBackupRequestRequestTypeDef, _OptionalDeleteBackupRequestRequestTypeDef
 ):
     pass
 
 
+DeleteBackupResponseTypeDef = TypedDict(
+    "DeleteBackupResponseTypeDef",
+    {
+        "BackupId": str,
+        "Lifecycle": BackupLifecycleType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
@@ -569,14 +592,24 @@
 class DeleteDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
 
+DeleteDataRepositoryAssociationResponseTypeDef = TypedDict(
+    "DeleteDataRepositoryAssociationResponseTypeDef",
+    {
+        "AssociationId": str,
+        "Lifecycle": DataRepositoryLifecycleType,
+        "DeleteDataInFileSystem": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileCacheRequestRequestTypeDef",
     {
         "FileCacheId": str,
     },
 )
 _OptionalDeleteFileCacheRequestRequestTypeDef = TypedDict(
@@ -590,14 +623,23 @@
 
 class DeleteFileCacheRequestRequestTypeDef(
     _RequiredDeleteFileCacheRequestRequestTypeDef, _OptionalDeleteFileCacheRequestRequestTypeDef
 ):
     pass
 
 
+DeleteFileCacheResponseTypeDef = TypedDict(
+    "DeleteFileCacheResponseTypeDef",
+    {
+        "FileCacheId": str,
+        "Lifecycle": FileCacheLifecycleType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 _OptionalDeleteSnapshotRequestRequestTypeDef = TypedDict(
@@ -611,14 +653,23 @@
 
 class DeleteSnapshotRequestRequestTypeDef(
     _RequiredDeleteSnapshotRequestRequestTypeDef, _OptionalDeleteSnapshotRequestRequestTypeDef
 ):
     pass
 
 
+DeleteSnapshotResponseTypeDef = TypedDict(
+    "DeleteSnapshotResponseTypeDef",
+    {
+        "SnapshotId": str,
+        "Lifecycle": SnapshotLifecycleType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStorageVirtualMachineRequestRequestTypeDef",
     {
         "StorageVirtualMachineId": str,
     },
 )
 _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
@@ -633,14 +684,23 @@
 class DeleteStorageVirtualMachineRequestRequestTypeDef(
     _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef,
     _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
 
+DeleteStorageVirtualMachineResponseTypeDef = TypedDict(
+    "DeleteStorageVirtualMachineResponseTypeDef",
+    {
+        "StorageVirtualMachineId": str,
+        "Lifecycle": StorageVirtualMachineLifecycleType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteVolumeOpenZFSConfigurationTypeDef = TypedDict(
     "DeleteVolumeOpenZFSConfigurationTypeDef",
     {
         "Options": Sequence[Literal["DELETE_CHILD_VOLUMES_AND_SNAPSHOTS"]],
     },
     total=False,
 )
@@ -650,24 +710,14 @@
     {
         "Name": FilterNameType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 DescribeFileCachesRequestRequestTypeDef = TypedDict(
     "DescribeFileCachesRequestRequestTypeDef",
     {
         "FileCacheIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -694,24 +744,42 @@
 class DescribeFileSystemAliasesRequestRequestTypeDef(
     _RequiredDescribeFileSystemAliasesRequestRequestTypeDef,
     _OptionalDescribeFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
 
+DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+    {
+        "FileSystemIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeFileSystemsRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemsRequestRequestTypeDef",
     {
         "FileSystemIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeFileSystemsResponseTypeDef = TypedDict(
+    "DescribeFileSystemsResponseTypeDef",
+    {
+        "FileSystems": List["FileSystemTypeDef"],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SnapshotFilterTypeDef = TypedDict(
     "SnapshotFilterTypeDef",
     {
         "Name": SnapshotFilterNameType,
         "Values": Sequence[str],
     },
     total=False,
@@ -829,14 +897,36 @@
     "LifecycleTransitionReasonTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
 
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -869,14 +959,24 @@
     {
         "SnapshotARN": str,
         "CopyStrategy": OpenZFSCopyStrategyType,
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
 _RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef = TypedDict(
     "_RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef = TypedDict(
@@ -891,14 +991,33 @@
 class ReleaseFileSystemNfsV3LocksRequestRequestTypeDef(
     _RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
     _OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
 ):
     pass
 
 
+ReleaseFileSystemNfsV3LocksResponseTypeDef = TypedDict(
+    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
+    {
+        "FileSystem": "FileSystemTypeDef",
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
 _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef",
     {
         "VolumeId": str,
         "SnapshotId": str,
     },
 )
@@ -915,14 +1034,24 @@
 class RestoreVolumeFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreVolumeFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
 
+RestoreVolumeFromSnapshotResponseTypeDef = TypedDict(
+    "RestoreVolumeFromSnapshotResponseTypeDef",
+    {
+        "VolumeId": str,
+        "Lifecycle": VolumeLifecycleType,
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SelfManagedActiveDirectoryAttributesTypeDef = TypedDict(
     "SelfManagedActiveDirectoryAttributesTypeDef",
     {
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
         "UserName": str,
@@ -933,14 +1062,17 @@
 
 SelfManagedActiveDirectoryConfigurationUpdatesTypeDef = TypedDict(
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
     {
         "UserName": str,
         "Password": str,
         "DnsIps": Sequence[str],
+        "DomainName": str,
+        "OrganizationalUnitDistinguishedName": str,
+        "FileSystemAdministratorsGroup": str,
     },
     total=False,
 )
 
 SvmEndpointTypeDef = TypedDict(
     "SvmEndpointTypeDef",
     {
@@ -962,14 +1094,22 @@
     "UpdateFileCacheLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
+UpdateFileSystemResponseTypeDef = TypedDict(
+    "UpdateFileSystemResponseTypeDef",
+    {
+        "FileSystem": "FileSystemTypeDef",
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotRequestRequestTypeDef",
     {
         "Name": str,
         "SnapshotId": str,
     },
 )
@@ -1010,138 +1150,32 @@
     pass
 
 
 AssociateFileSystemAliasesResponseTypeDef = TypedDict(
     "AssociateFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelDataRepositoryTaskResponseTypeDef = TypedDict(
-    "CancelDataRepositoryTaskResponseTypeDef",
-    {
-        "Lifecycle": DataRepositoryTaskLifecycleType,
-        "TaskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFileSystemFromBackupResponseTypeDef = TypedDict(
-    "CreateFileSystemFromBackupResponseTypeDef",
-    {
-        "FileSystem": "FileSystemTypeDef",
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFileSystemResponseTypeDef = TypedDict(
-    "CreateFileSystemResponseTypeDef",
-    {
-        "FileSystem": "FileSystemTypeDef",
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBackupResponseTypeDef = TypedDict(
-    "DeleteBackupResponseTypeDef",
-    {
-        "BackupId": str,
-        "Lifecycle": BackupLifecycleType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDataRepositoryAssociationResponseTypeDef = TypedDict(
-    "DeleteDataRepositoryAssociationResponseTypeDef",
-    {
-        "AssociationId": str,
-        "Lifecycle": DataRepositoryLifecycleType,
-        "DeleteDataInFileSystem": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFileCacheResponseTypeDef = TypedDict(
-    "DeleteFileCacheResponseTypeDef",
-    {
-        "FileCacheId": str,
-        "Lifecycle": FileCacheLifecycleType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSnapshotResponseTypeDef = TypedDict(
-    "DeleteSnapshotResponseTypeDef",
-    {
-        "SnapshotId": str,
-        "Lifecycle": SnapshotLifecycleType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteStorageVirtualMachineResponseTypeDef = TypedDict(
-    "DeleteStorageVirtualMachineResponseTypeDef",
-    {
-        "StorageVirtualMachineId": str,
-        "Lifecycle": StorageVirtualMachineLifecycleType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFileSystemAliasesResponseTypeDef = TypedDict(
     "DescribeFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFileSystemsResponseTypeDef = TypedDict(
-    "DescribeFileSystemsResponseTypeDef",
-    {
-        "FileSystems": List["FileSystemTypeDef"],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateFileSystemAliasesResponseTypeDef = TypedDict(
     "DisassociateFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReleaseFileSystemNfsV3LocksResponseTypeDef = TypedDict(
-    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
-    {
-        "FileSystem": "FileSystemTypeDef",
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RestoreVolumeFromSnapshotResponseTypeDef = TypedDict(
-    "RestoreVolumeFromSnapshotResponseTypeDef",
-    {
-        "VolumeId": str,
-        "Lifecycle": VolumeLifecycleType,
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFileSystemResponseTypeDef = TypedDict(
-    "UpdateFileSystemResponseTypeDef",
-    {
-        "FileSystem": "FileSystemTypeDef",
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredNFSDataRepositoryConfigurationTypeDef = TypedDict(
     "_RequiredNFSDataRepositoryConfigurationTypeDef",
     {
         "Version": Literal["NFS3"],
@@ -1305,15 +1339,15 @@
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1650,14 +1684,24 @@
 
 class DataRepositoryTaskTypeDef(
     _RequiredDataRepositoryTaskTypeDef, _OptionalDataRepositoryTaskTypeDef
 ):
     pass
 
 
+DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    {
+        "BackupIds": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
         "BackupIds": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1672,55 +1716,14 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
-    {
-        "BackupIds": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
-    {
-        "FileSystemIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 DescribeSnapshotsRequestRequestTypeDef = TypedDict(
     "DescribeSnapshotsRequestRequestTypeDef",
     {
         "SnapshotIds": Sequence[str],
         "Filters": Sequence[SnapshotFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1729,15 +1732,15 @@
 )
 
 DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef = TypedDict(
     "DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef",
     {
         "StorageVirtualMachineIds": Sequence[str],
         "Filters": Sequence[StorageVirtualMachineFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeStorageVirtualMachinesRequestRequestTypeDef = TypedDict(
     "DescribeStorageVirtualMachinesRequestRequestTypeDef",
     {
@@ -1750,15 +1753,15 @@
 )
 
 DescribeVolumesRequestDescribeVolumesPaginateTypeDef = TypedDict(
     "DescribeVolumesRequestDescribeVolumesPaginateTypeDef",
     {
         "VolumeIds": Sequence[str],
         "Filters": Sequence[VolumeFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeVolumesRequestRequestTypeDef = TypedDict(
     "DescribeVolumesRequestRequestTypeDef",
     {
@@ -1823,15 +1826,15 @@
         "SnapshotId": str,
         "Name": str,
         "VolumeId": str,
         "CreationTime": datetime,
         "Lifecycle": SnapshotLifecycleType,
         "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "Tags": List[TagTypeDef],
-        "AdministrativeActions": List[Dict[str, Any]],
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
     },
     total=False,
 )
 
 OpenZFSNfsExportTypeDef = TypedDict(
     "OpenZFSNfsExportTypeDef",
     {
@@ -1851,24 +1854,29 @@
 UpdateFileSystemWindowsConfigurationTypeDef = TypedDict(
     "UpdateFileSystemWindowsConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "DailyAutomaticBackupStartTime": str,
         "AutomaticBackupRetentionDays": int,
         "ThroughputCapacity": int,
-        "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
+        "SelfManagedActiveDirectoryConfiguration": (
+            SelfManagedActiveDirectoryConfigurationUpdatesTypeDef
+        ),
         "AuditLogConfiguration": WindowsAuditLogCreateConfigurationTypeDef,
     },
     total=False,
 )
 
 UpdateSvmActiveDirectoryConfigurationTypeDef = TypedDict(
     "UpdateSvmActiveDirectoryConfigurationTypeDef",
     {
-        "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
+        "SelfManagedActiveDirectoryConfiguration": (
+            SelfManagedActiveDirectoryConfigurationUpdatesTypeDef
+        ),
+        "NetBiosName": str,
     },
     total=False,
 )
 
 SvmEndpointsTypeDef = TypedDict(
     "SvmEndpointsTypeDef",
     {
@@ -2026,15 +2034,15 @@
     "DeleteFileSystemResponseTypeDef",
     {
         "FileSystemId": str,
         "Lifecycle": FileSystemLifecycleType,
         "WindowsResponse": DeleteFileSystemWindowsResponseTypeDef,
         "LustreResponse": DeleteFileSystemLustreResponseTypeDef,
         "OpenZFSResponse": DeleteFileSystemOpenZFSResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteVolumeRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteVolumeRequestRequestTypeDef",
     {
         "VolumeId": str,
@@ -2059,15 +2067,15 @@
 
 DeleteVolumeResponseTypeDef = TypedDict(
     "DeleteVolumeResponseTypeDef",
     {
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
         "OntapResponse": DeleteVolumeOntapResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStorageVirtualMachineRequestRequestTypeDef",
     {
         "FileSystemId": str,
@@ -2138,24 +2146,24 @@
     total=False,
 )
 
 CreateDataRepositoryTaskResponseTypeDef = TypedDict(
     "CreateDataRepositoryTaskResponseTypeDef",
     {
         "DataRepositoryTask": DataRepositoryTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDataRepositoryTasksResponseTypeDef = TypedDict(
     "DescribeDataRepositoryTasksResponseTypeDef",
     {
         "DataRepositoryTasks": List[DataRepositoryTaskTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileCacheRequestRequestTypeDef",
     {
         "FileCacheType": Literal["LUSTRE"],
@@ -2242,40 +2250,41 @@
         "EndpointIpAddressRange": str,
         "Endpoints": FileSystemEndpointsTypeDef,
         "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
         "PreferredSubnetId": str,
         "RouteTableIds": List[str],
         "ThroughputCapacity": int,
         "WeeklyMaintenanceStartTime": str,
+        "FsxAdminPassword": str,
     },
     total=False,
 )
 
 CreateSnapshotResponseTypeDef = TypedDict(
     "CreateSnapshotResponseTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSnapshotsResponseTypeDef = TypedDict(
     "DescribeSnapshotsResponseTypeDef",
     {
         "Snapshots": List[SnapshotTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSnapshotResponseTypeDef = TypedDict(
     "UpdateSnapshotResponseTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateOpenZFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredCreateOpenZFSVolumeConfigurationTypeDef",
     {
         "ParentVolumeId": str,
@@ -2423,57 +2432,57 @@
     total=False,
 )
 
 CreateDataRepositoryAssociationResponseTypeDef = TypedDict(
     "CreateDataRepositoryAssociationResponseTypeDef",
     {
         "Association": DataRepositoryAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDataRepositoryAssociationsResponseTypeDef = TypedDict(
     "DescribeDataRepositoryAssociationsResponseTypeDef",
     {
         "Associations": List[DataRepositoryAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDataRepositoryAssociationResponseTypeDef = TypedDict(
     "UpdateDataRepositoryAssociationResponseTypeDef",
     {
         "Association": DataRepositoryAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFileCacheResponseTypeDef = TypedDict(
     "CreateFileCacheResponseTypeDef",
     {
         "FileCache": FileCacheCreatingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFileCachesResponseTypeDef = TypedDict(
     "DescribeFileCachesResponseTypeDef",
     {
         "FileCaches": List[FileCacheTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFileCacheResponseTypeDef = TypedDict(
     "UpdateFileCacheResponseTypeDef",
     {
         "FileCache": FileCacheTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FileSystemTypeDef = TypedDict(
     "FileSystemTypeDef",
     {
         "OwnerId": str,
@@ -2489,15 +2498,15 @@
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
         "WindowsConfiguration": WindowsFileSystemConfigurationTypeDef,
         "LustreConfiguration": LustreFileSystemConfigurationTypeDef,
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "AdministrativeActions": List[Dict[str, Any]],
         "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
     },
     total=False,
 )
 
@@ -2598,32 +2607,32 @@
     pass
 
 
 CreateStorageVirtualMachineResponseTypeDef = TypedDict(
     "CreateStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachine": StorageVirtualMachineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStorageVirtualMachinesResponseTypeDef = TypedDict(
     "DescribeStorageVirtualMachinesResponseTypeDef",
     {
         "StorageVirtualMachines": List[StorageVirtualMachineTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStorageVirtualMachineResponseTypeDef = TypedDict(
     "UpdateStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachine": StorageVirtualMachineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFileSystemFromBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemFromBackupRequestRequestTypeDef",
     {
         "BackupId": str,
@@ -2735,60 +2744,60 @@
     pass
 
 
 CreateVolumeFromBackupResponseTypeDef = TypedDict(
     "CreateVolumeFromBackupResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVolumeResponseTypeDef = TypedDict(
     "CreateVolumeResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVolumesResponseTypeDef = TypedDict(
     "DescribeVolumesResponseTypeDef",
     {
         "Volumes": List[VolumeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVolumeResponseTypeDef = TypedDict(
     "UpdateVolumeResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CopyBackupResponseTypeDef = TypedDict(
     "CopyBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateBackupResponseTypeDef = TypedDict(
     "CreateBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBackupsResponseTypeDef = TypedDict(
     "DescribeBackupsResponseTypeDef",
     {
         "Backups": List[BackupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/type_defs.pyi` & `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -72,82 +72,84 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActiveDirectoryBackupAttributesTypeDef",
     "AdministrativeActionFailureDetailsTypeDef",
     "AliasTypeDef",
     "AssociateFileSystemAliasesRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AutoExportPolicyTypeDef",
     "AutoImportPolicyTypeDef",
     "BackupFailureDetailsTypeDef",
     "TagTypeDef",
     "CancelDataRepositoryTaskRequestRequestTypeDef",
+    "CancelDataRepositoryTaskResponseTypeDef",
     "CompletionReportTypeDef",
     "FileCacheLustreMetadataConfigurationTypeDef",
+    "CreateFileSystemFromBackupResponseTypeDef",
     "LustreLogCreateConfigurationTypeDef",
     "LustreRootSquashConfigurationTypeDef",
     "DiskIopsConfigurationTypeDef",
+    "CreateFileSystemResponseTypeDef",
     "SelfManagedActiveDirectoryConfigurationTypeDef",
     "WindowsAuditLogCreateConfigurationTypeDef",
     "TieringPolicyTypeDef",
     "CreateOpenZFSOriginSnapshotConfigurationTypeDef",
     "OpenZFSUserOrGroupQuotaTypeDef",
     "DataRepositoryFailureDetailsTypeDef",
     "DataRepositoryTaskFailureDetailsTypeDef",
     "DataRepositoryTaskFilterTypeDef",
     "DataRepositoryTaskStatusTypeDef",
     "DeleteBackupRequestRequestTypeDef",
+    "DeleteBackupResponseTypeDef",
     "DeleteDataRepositoryAssociationRequestRequestTypeDef",
+    "DeleteDataRepositoryAssociationResponseTypeDef",
     "DeleteFileCacheRequestRequestTypeDef",
+    "DeleteFileCacheResponseTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
+    "DeleteSnapshotResponseTypeDef",
     "DeleteStorageVirtualMachineRequestRequestTypeDef",
+    "DeleteStorageVirtualMachineResponseTypeDef",
     "DeleteVolumeOpenZFSConfigurationTypeDef",
     "FilterTypeDef",
-    "PaginatorConfigTypeDef",
     "DescribeFileCachesRequestRequestTypeDef",
     "DescribeFileSystemAliasesRequestRequestTypeDef",
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
     "DescribeFileSystemsRequestRequestTypeDef",
+    "DescribeFileSystemsResponseTypeDef",
     "SnapshotFilterTypeDef",
     "StorageVirtualMachineFilterTypeDef",
     "VolumeFilterTypeDef",
     "DisassociateFileSystemAliasesRequestRequestTypeDef",
     "FileCacheFailureDetailsTypeDef",
     "FileCacheNFSConfigurationTypeDef",
     "LustreLogConfigurationTypeDef",
     "FileSystemEndpointTypeDef",
     "FileSystemFailureDetailsTypeDef",
     "LifecycleTransitionReasonTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "OpenZFSClientConfigurationTypeDef",
     "OpenZFSOriginSnapshotConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
     "ReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
+    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreVolumeFromSnapshotRequestRequestTypeDef",
+    "RestoreVolumeFromSnapshotResponseTypeDef",
     "SelfManagedActiveDirectoryAttributesTypeDef",
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
     "SvmEndpointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileCacheLustreConfigurationTypeDef",
+    "UpdateFileSystemResponseTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "WindowsAuditLogConfigurationTypeDef",
     "AssociateFileSystemAliasesResponseTypeDef",
-    "CancelDataRepositoryTaskResponseTypeDef",
-    "CreateFileSystemFromBackupResponseTypeDef",
-    "CreateFileSystemResponseTypeDef",
-    "DeleteBackupResponseTypeDef",
-    "DeleteDataRepositoryAssociationResponseTypeDef",
-    "DeleteFileCacheResponseTypeDef",
-    "DeleteSnapshotResponseTypeDef",
-    "DeleteStorageVirtualMachineResponseTypeDef",
     "DescribeFileSystemAliasesResponseTypeDef",
-    "DescribeFileSystemsResponseTypeDef",
     "DisassociateFileSystemAliasesResponseTypeDef",
-    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
-    "RestoreVolumeFromSnapshotResponseTypeDef",
-    "UpdateFileSystemResponseTypeDef",
     "NFSDataRepositoryConfigurationTypeDef",
     "S3DataRepositoryConfigurationTypeDef",
     "CopyBackupRequestRequestTypeDef",
     "CreateBackupRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "DeleteFileSystemLustreConfigurationTypeDef",
     "DeleteFileSystemLustreResponseTypeDef",
@@ -171,19 +173,17 @@
     "CreateFileSystemWindowsConfigurationTypeDef",
     "CreateOntapVolumeConfigurationTypeDef",
     "OntapVolumeConfigurationTypeDef",
     "UpdateOntapVolumeConfigurationTypeDef",
     "DataRepositoryConfigurationTypeDef",
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
     "DataRepositoryTaskTypeDef",
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
     "DescribeDataRepositoryAssociationsRequestRequestTypeDef",
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeSnapshotsRequestRequestTypeDef",
     "DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef",
     "DescribeStorageVirtualMachinesRequestRequestTypeDef",
     "DescribeVolumesRequestDescribeVolumesPaginateTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
     "FileCacheDataRepositoryAssociationTypeDef",
     "FileCacheLustreConfigurationTypeDef",
@@ -293,25 +293,14 @@
 
 class AssociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredAssociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalAssociateFileSystemAliasesRequestRequestTypeDef,
 ):
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
 AutoExportPolicyTypeDef = TypedDict(
     "AutoExportPolicyTypeDef",
     {
         "Events": Sequence[EventTypeType],
     },
     total=False,
 )
@@ -343,14 +332,23 @@
 CancelDataRepositoryTaskRequestRequestTypeDef = TypedDict(
     "CancelDataRepositoryTaskRequestRequestTypeDef",
     {
         "TaskId": str,
     },
 )
 
+CancelDataRepositoryTaskResponseTypeDef = TypedDict(
+    "CancelDataRepositoryTaskResponseTypeDef",
+    {
+        "Lifecycle": DataRepositoryTaskLifecycleType,
+        "TaskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCompletionReportTypeDef = TypedDict(
     "_RequiredCompletionReportTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalCompletionReportTypeDef = TypedDict(
@@ -369,14 +367,22 @@
 FileCacheLustreMetadataConfigurationTypeDef = TypedDict(
     "FileCacheLustreMetadataConfigurationTypeDef",
     {
         "StorageCapacity": int,
     },
 )
 
+CreateFileSystemFromBackupResponseTypeDef = TypedDict(
+    "CreateFileSystemFromBackupResponseTypeDef",
+    {
+        "FileSystem": "FileSystemTypeDef",
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredLustreLogCreateConfigurationTypeDef = TypedDict(
     "_RequiredLustreLogCreateConfigurationTypeDef",
     {
         "Level": LustreAccessAuditLogLevelType,
     },
 )
 _OptionalLustreLogCreateConfigurationTypeDef = TypedDict(
@@ -406,14 +412,22 @@
     {
         "Mode": DiskIopsConfigurationModeType,
         "Iops": int,
     },
     total=False,
 )
 
+CreateFileSystemResponseTypeDef = TypedDict(
+    "CreateFileSystemResponseTypeDef",
+    {
+        "FileSystem": "FileSystemTypeDef",
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSelfManagedActiveDirectoryConfigurationTypeDef = TypedDict(
     "_RequiredSelfManagedActiveDirectoryConfigurationTypeDef",
     {
         "DomainName": str,
         "UserName": str,
         "Password": str,
         "DnsIps": Sequence[str],
@@ -533,14 +547,23 @@
 )
 
 class DeleteBackupRequestRequestTypeDef(
     _RequiredDeleteBackupRequestRequestTypeDef, _OptionalDeleteBackupRequestRequestTypeDef
 ):
     pass
 
+DeleteBackupResponseTypeDef = TypedDict(
+    "DeleteBackupResponseTypeDef",
+    {
+        "BackupId": str,
+        "Lifecycle": BackupLifecycleType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
@@ -554,14 +577,24 @@
 
 class DeleteDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
+DeleteDataRepositoryAssociationResponseTypeDef = TypedDict(
+    "DeleteDataRepositoryAssociationResponseTypeDef",
+    {
+        "AssociationId": str,
+        "Lifecycle": DataRepositoryLifecycleType,
+        "DeleteDataInFileSystem": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileCacheRequestRequestTypeDef",
     {
         "FileCacheId": str,
     },
 )
 _OptionalDeleteFileCacheRequestRequestTypeDef = TypedDict(
@@ -573,14 +606,23 @@
 )
 
 class DeleteFileCacheRequestRequestTypeDef(
     _RequiredDeleteFileCacheRequestRequestTypeDef, _OptionalDeleteFileCacheRequestRequestTypeDef
 ):
     pass
 
+DeleteFileCacheResponseTypeDef = TypedDict(
+    "DeleteFileCacheResponseTypeDef",
+    {
+        "FileCacheId": str,
+        "Lifecycle": FileCacheLifecycleType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 _OptionalDeleteSnapshotRequestRequestTypeDef = TypedDict(
@@ -592,14 +634,23 @@
 )
 
 class DeleteSnapshotRequestRequestTypeDef(
     _RequiredDeleteSnapshotRequestRequestTypeDef, _OptionalDeleteSnapshotRequestRequestTypeDef
 ):
     pass
 
+DeleteSnapshotResponseTypeDef = TypedDict(
+    "DeleteSnapshotResponseTypeDef",
+    {
+        "SnapshotId": str,
+        "Lifecycle": SnapshotLifecycleType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStorageVirtualMachineRequestRequestTypeDef",
     {
         "StorageVirtualMachineId": str,
     },
 )
 _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
@@ -612,14 +663,23 @@
 
 class DeleteStorageVirtualMachineRequestRequestTypeDef(
     _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef,
     _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
+DeleteStorageVirtualMachineResponseTypeDef = TypedDict(
+    "DeleteStorageVirtualMachineResponseTypeDef",
+    {
+        "StorageVirtualMachineId": str,
+        "Lifecycle": StorageVirtualMachineLifecycleType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteVolumeOpenZFSConfigurationTypeDef = TypedDict(
     "DeleteVolumeOpenZFSConfigurationTypeDef",
     {
         "Options": Sequence[Literal["DELETE_CHILD_VOLUMES_AND_SNAPSHOTS"]],
     },
     total=False,
 )
@@ -629,24 +689,14 @@
     {
         "Name": FilterNameType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 DescribeFileCachesRequestRequestTypeDef = TypedDict(
     "DescribeFileCachesRequestRequestTypeDef",
     {
         "FileCacheIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -671,24 +721,42 @@
 
 class DescribeFileSystemAliasesRequestRequestTypeDef(
     _RequiredDescribeFileSystemAliasesRequestRequestTypeDef,
     _OptionalDescribeFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
+DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+    {
+        "FileSystemIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeFileSystemsRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemsRequestRequestTypeDef",
     {
         "FileSystemIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeFileSystemsResponseTypeDef = TypedDict(
+    "DescribeFileSystemsResponseTypeDef",
+    {
+        "FileSystems": List["FileSystemTypeDef"],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SnapshotFilterTypeDef = TypedDict(
     "SnapshotFilterTypeDef",
     {
         "Name": SnapshotFilterNameType,
         "Values": Sequence[str],
     },
     total=False,
@@ -800,14 +868,34 @@
     "LifecycleTransitionReasonTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
 
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -838,14 +926,24 @@
     {
         "SnapshotARN": str,
         "CopyStrategy": OpenZFSCopyStrategyType,
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
 _RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef = TypedDict(
     "_RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef = TypedDict(
@@ -858,14 +956,33 @@
 
 class ReleaseFileSystemNfsV3LocksRequestRequestTypeDef(
     _RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
     _OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
 ):
     pass
 
+ReleaseFileSystemNfsV3LocksResponseTypeDef = TypedDict(
+    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
+    {
+        "FileSystem": "FileSystemTypeDef",
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
 _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef",
     {
         "VolumeId": str,
         "SnapshotId": str,
     },
 )
@@ -880,14 +997,24 @@
 
 class RestoreVolumeFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreVolumeFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
+RestoreVolumeFromSnapshotResponseTypeDef = TypedDict(
+    "RestoreVolumeFromSnapshotResponseTypeDef",
+    {
+        "VolumeId": str,
+        "Lifecycle": VolumeLifecycleType,
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SelfManagedActiveDirectoryAttributesTypeDef = TypedDict(
     "SelfManagedActiveDirectoryAttributesTypeDef",
     {
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
         "UserName": str,
@@ -898,14 +1025,17 @@
 
 SelfManagedActiveDirectoryConfigurationUpdatesTypeDef = TypedDict(
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
     {
         "UserName": str,
         "Password": str,
         "DnsIps": Sequence[str],
+        "DomainName": str,
+        "OrganizationalUnitDistinguishedName": str,
+        "FileSystemAdministratorsGroup": str,
     },
     total=False,
 )
 
 SvmEndpointTypeDef = TypedDict(
     "SvmEndpointTypeDef",
     {
@@ -927,14 +1057,22 @@
     "UpdateFileCacheLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
+UpdateFileSystemResponseTypeDef = TypedDict(
+    "UpdateFileSystemResponseTypeDef",
+    {
+        "FileSystem": "FileSystemTypeDef",
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotRequestRequestTypeDef",
     {
         "Name": str,
         "SnapshotId": str,
     },
 )
@@ -971,138 +1109,32 @@
 ):
     pass
 
 AssociateFileSystemAliasesResponseTypeDef = TypedDict(
     "AssociateFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelDataRepositoryTaskResponseTypeDef = TypedDict(
-    "CancelDataRepositoryTaskResponseTypeDef",
-    {
-        "Lifecycle": DataRepositoryTaskLifecycleType,
-        "TaskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFileSystemFromBackupResponseTypeDef = TypedDict(
-    "CreateFileSystemFromBackupResponseTypeDef",
-    {
-        "FileSystem": "FileSystemTypeDef",
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFileSystemResponseTypeDef = TypedDict(
-    "CreateFileSystemResponseTypeDef",
-    {
-        "FileSystem": "FileSystemTypeDef",
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBackupResponseTypeDef = TypedDict(
-    "DeleteBackupResponseTypeDef",
-    {
-        "BackupId": str,
-        "Lifecycle": BackupLifecycleType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDataRepositoryAssociationResponseTypeDef = TypedDict(
-    "DeleteDataRepositoryAssociationResponseTypeDef",
-    {
-        "AssociationId": str,
-        "Lifecycle": DataRepositoryLifecycleType,
-        "DeleteDataInFileSystem": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFileCacheResponseTypeDef = TypedDict(
-    "DeleteFileCacheResponseTypeDef",
-    {
-        "FileCacheId": str,
-        "Lifecycle": FileCacheLifecycleType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSnapshotResponseTypeDef = TypedDict(
-    "DeleteSnapshotResponseTypeDef",
-    {
-        "SnapshotId": str,
-        "Lifecycle": SnapshotLifecycleType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteStorageVirtualMachineResponseTypeDef = TypedDict(
-    "DeleteStorageVirtualMachineResponseTypeDef",
-    {
-        "StorageVirtualMachineId": str,
-        "Lifecycle": StorageVirtualMachineLifecycleType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFileSystemAliasesResponseTypeDef = TypedDict(
     "DescribeFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFileSystemsResponseTypeDef = TypedDict(
-    "DescribeFileSystemsResponseTypeDef",
-    {
-        "FileSystems": List["FileSystemTypeDef"],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateFileSystemAliasesResponseTypeDef = TypedDict(
     "DisassociateFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReleaseFileSystemNfsV3LocksResponseTypeDef = TypedDict(
-    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
-    {
-        "FileSystem": "FileSystemTypeDef",
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RestoreVolumeFromSnapshotResponseTypeDef = TypedDict(
-    "RestoreVolumeFromSnapshotResponseTypeDef",
-    {
-        "VolumeId": str,
-        "Lifecycle": VolumeLifecycleType,
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateFileSystemResponseTypeDef = TypedDict(
-    "UpdateFileSystemResponseTypeDef",
-    {
-        "FileSystem": "FileSystemTypeDef",
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredNFSDataRepositoryConfigurationTypeDef = TypedDict(
     "_RequiredNFSDataRepositoryConfigurationTypeDef",
     {
         "Version": Literal["NFS3"],
@@ -1260,15 +1292,15 @@
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1591,14 +1623,24 @@
 )
 
 class DataRepositoryTaskTypeDef(
     _RequiredDataRepositoryTaskTypeDef, _OptionalDataRepositoryTaskTypeDef
 ):
     pass
 
+DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    {
+        "BackupIds": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
         "BackupIds": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1613,53 +1655,14 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
-    {
-        "BackupIds": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
-    {
-        "FileSystemIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 DescribeSnapshotsRequestRequestTypeDef = TypedDict(
     "DescribeSnapshotsRequestRequestTypeDef",
     {
         "SnapshotIds": Sequence[str],
         "Filters": Sequence[SnapshotFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1668,15 +1671,15 @@
 )
 
 DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef = TypedDict(
     "DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef",
     {
         "StorageVirtualMachineIds": Sequence[str],
         "Filters": Sequence[StorageVirtualMachineFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeStorageVirtualMachinesRequestRequestTypeDef = TypedDict(
     "DescribeStorageVirtualMachinesRequestRequestTypeDef",
     {
@@ -1689,15 +1692,15 @@
 )
 
 DescribeVolumesRequestDescribeVolumesPaginateTypeDef = TypedDict(
     "DescribeVolumesRequestDescribeVolumesPaginateTypeDef",
     {
         "VolumeIds": Sequence[str],
         "Filters": Sequence[VolumeFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeVolumesRequestRequestTypeDef = TypedDict(
     "DescribeVolumesRequestRequestTypeDef",
     {
@@ -1760,15 +1763,15 @@
         "SnapshotId": str,
         "Name": str,
         "VolumeId": str,
         "CreationTime": datetime,
         "Lifecycle": SnapshotLifecycleType,
         "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "Tags": List[TagTypeDef],
-        "AdministrativeActions": List[Dict[str, Any]],
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
     },
     total=False,
 )
 
 OpenZFSNfsExportTypeDef = TypedDict(
     "OpenZFSNfsExportTypeDef",
     {
@@ -1788,24 +1791,29 @@
 UpdateFileSystemWindowsConfigurationTypeDef = TypedDict(
     "UpdateFileSystemWindowsConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "DailyAutomaticBackupStartTime": str,
         "AutomaticBackupRetentionDays": int,
         "ThroughputCapacity": int,
-        "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
+        "SelfManagedActiveDirectoryConfiguration": (
+            SelfManagedActiveDirectoryConfigurationUpdatesTypeDef
+        ),
         "AuditLogConfiguration": WindowsAuditLogCreateConfigurationTypeDef,
     },
     total=False,
 )
 
 UpdateSvmActiveDirectoryConfigurationTypeDef = TypedDict(
     "UpdateSvmActiveDirectoryConfigurationTypeDef",
     {
-        "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
+        "SelfManagedActiveDirectoryConfiguration": (
+            SelfManagedActiveDirectoryConfigurationUpdatesTypeDef
+        ),
+        "NetBiosName": str,
     },
     total=False,
 )
 
 SvmEndpointsTypeDef = TypedDict(
     "SvmEndpointsTypeDef",
     {
@@ -1955,15 +1963,15 @@
     "DeleteFileSystemResponseTypeDef",
     {
         "FileSystemId": str,
         "Lifecycle": FileSystemLifecycleType,
         "WindowsResponse": DeleteFileSystemWindowsResponseTypeDef,
         "LustreResponse": DeleteFileSystemLustreResponseTypeDef,
         "OpenZFSResponse": DeleteFileSystemOpenZFSResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteVolumeRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteVolumeRequestRequestTypeDef",
     {
         "VolumeId": str,
@@ -1986,15 +1994,15 @@
 
 DeleteVolumeResponseTypeDef = TypedDict(
     "DeleteVolumeResponseTypeDef",
     {
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
         "OntapResponse": DeleteVolumeOntapResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStorageVirtualMachineRequestRequestTypeDef",
     {
         "FileSystemId": str,
@@ -2061,24 +2069,24 @@
     total=False,
 )
 
 CreateDataRepositoryTaskResponseTypeDef = TypedDict(
     "CreateDataRepositoryTaskResponseTypeDef",
     {
         "DataRepositoryTask": DataRepositoryTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDataRepositoryTasksResponseTypeDef = TypedDict(
     "DescribeDataRepositoryTasksResponseTypeDef",
     {
         "DataRepositoryTasks": List[DataRepositoryTaskTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileCacheRequestRequestTypeDef",
     {
         "FileCacheType": Literal["LUSTRE"],
@@ -2163,40 +2171,41 @@
         "EndpointIpAddressRange": str,
         "Endpoints": FileSystemEndpointsTypeDef,
         "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
         "PreferredSubnetId": str,
         "RouteTableIds": List[str],
         "ThroughputCapacity": int,
         "WeeklyMaintenanceStartTime": str,
+        "FsxAdminPassword": str,
     },
     total=False,
 )
 
 CreateSnapshotResponseTypeDef = TypedDict(
     "CreateSnapshotResponseTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSnapshotsResponseTypeDef = TypedDict(
     "DescribeSnapshotsResponseTypeDef",
     {
         "Snapshots": List[SnapshotTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSnapshotResponseTypeDef = TypedDict(
     "UpdateSnapshotResponseTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateOpenZFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredCreateOpenZFSVolumeConfigurationTypeDef",
     {
         "ParentVolumeId": str,
@@ -2338,57 +2347,57 @@
     total=False,
 )
 
 CreateDataRepositoryAssociationResponseTypeDef = TypedDict(
     "CreateDataRepositoryAssociationResponseTypeDef",
     {
         "Association": DataRepositoryAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDataRepositoryAssociationsResponseTypeDef = TypedDict(
     "DescribeDataRepositoryAssociationsResponseTypeDef",
     {
         "Associations": List[DataRepositoryAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDataRepositoryAssociationResponseTypeDef = TypedDict(
     "UpdateDataRepositoryAssociationResponseTypeDef",
     {
         "Association": DataRepositoryAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFileCacheResponseTypeDef = TypedDict(
     "CreateFileCacheResponseTypeDef",
     {
         "FileCache": FileCacheCreatingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFileCachesResponseTypeDef = TypedDict(
     "DescribeFileCachesResponseTypeDef",
     {
         "FileCaches": List[FileCacheTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFileCacheResponseTypeDef = TypedDict(
     "UpdateFileCacheResponseTypeDef",
     {
         "FileCache": FileCacheTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FileSystemTypeDef = TypedDict(
     "FileSystemTypeDef",
     {
         "OwnerId": str,
@@ -2404,15 +2413,15 @@
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
         "WindowsConfiguration": WindowsFileSystemConfigurationTypeDef,
         "LustreConfiguration": LustreFileSystemConfigurationTypeDef,
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "AdministrativeActions": List[Dict[str, Any]],
         "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
     },
     total=False,
 )
 
@@ -2507,32 +2516,32 @@
 ):
     pass
 
 CreateStorageVirtualMachineResponseTypeDef = TypedDict(
     "CreateStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachine": StorageVirtualMachineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeStorageVirtualMachinesResponseTypeDef = TypedDict(
     "DescribeStorageVirtualMachinesResponseTypeDef",
     {
         "StorageVirtualMachines": List[StorageVirtualMachineTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStorageVirtualMachineResponseTypeDef = TypedDict(
     "UpdateStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachine": StorageVirtualMachineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFileSystemFromBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemFromBackupRequestRequestTypeDef",
     {
         "BackupId": str,
@@ -2638,60 +2647,60 @@
 class BackupTypeDef(_RequiredBackupTypeDef, _OptionalBackupTypeDef):
     pass
 
 CreateVolumeFromBackupResponseTypeDef = TypedDict(
     "CreateVolumeFromBackupResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVolumeResponseTypeDef = TypedDict(
     "CreateVolumeResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVolumesResponseTypeDef = TypedDict(
     "DescribeVolumesResponseTypeDef",
     {
         "Volumes": List[VolumeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVolumeResponseTypeDef = TypedDict(
     "UpdateVolumeResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CopyBackupResponseTypeDef = TypedDict(
     "CopyBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateBackupResponseTypeDef = TypedDict(
     "CreateBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBackupsResponseTypeDef = TypedDict(
     "DescribeBackupsResponseTypeDef",
     {
         "Backups": List[BackupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/PKG-INFO` & `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fsx
-Version: 1.26.37
-Summary: Type annotations for boto3.FSx 1.26.37 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.FSx 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-fsx"></a>
 
 # mypy-boto3-fsx
 
 [![PyPI - mypy-boto3-fsx](https://img.shields.io/pypi/v/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fsx?color=blue)](https://pypistats.org/packages/mypy-boto3-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FSx 1.26.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[boto3.FSx 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-fsx docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/).
 
 See how it helps to find and fix potential bugs:
 
@@ -393,82 +393,84 @@
 
 ```python
 from mypy_boto3_fsx.type_defs import (
     ActiveDirectoryBackupAttributesTypeDef,
     AdministrativeActionFailureDetailsTypeDef,
     AliasTypeDef,
     AssociateFileSystemAliasesRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     AutoExportPolicyTypeDef,
     AutoImportPolicyTypeDef,
     BackupFailureDetailsTypeDef,
     TagTypeDef,
     CancelDataRepositoryTaskRequestRequestTypeDef,
+    CancelDataRepositoryTaskResponseTypeDef,
     CompletionReportTypeDef,
     FileCacheLustreMetadataConfigurationTypeDef,
+    CreateFileSystemFromBackupResponseTypeDef,
     LustreLogCreateConfigurationTypeDef,
     LustreRootSquashConfigurationTypeDef,
     DiskIopsConfigurationTypeDef,
+    CreateFileSystemResponseTypeDef,
     SelfManagedActiveDirectoryConfigurationTypeDef,
     WindowsAuditLogCreateConfigurationTypeDef,
     TieringPolicyTypeDef,
     CreateOpenZFSOriginSnapshotConfigurationTypeDef,
     OpenZFSUserOrGroupQuotaTypeDef,
     DataRepositoryFailureDetailsTypeDef,
     DataRepositoryTaskFailureDetailsTypeDef,
     DataRepositoryTaskFilterTypeDef,
     DataRepositoryTaskStatusTypeDef,
     DeleteBackupRequestRequestTypeDef,
+    DeleteBackupResponseTypeDef,
     DeleteDataRepositoryAssociationRequestRequestTypeDef,
+    DeleteDataRepositoryAssociationResponseTypeDef,
     DeleteFileCacheRequestRequestTypeDef,
+    DeleteFileCacheResponseTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
+    DeleteSnapshotResponseTypeDef,
     DeleteStorageVirtualMachineRequestRequestTypeDef,
+    DeleteStorageVirtualMachineResponseTypeDef,
     DeleteVolumeOpenZFSConfigurationTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
     DescribeFileCachesRequestRequestTypeDef,
     DescribeFileSystemAliasesRequestRequestTypeDef,
+    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
+    DescribeFileSystemsResponseTypeDef,
     SnapshotFilterTypeDef,
     StorageVirtualMachineFilterTypeDef,
     VolumeFilterTypeDef,
     DisassociateFileSystemAliasesRequestRequestTypeDef,
     FileCacheFailureDetailsTypeDef,
     FileCacheNFSConfigurationTypeDef,
     LustreLogConfigurationTypeDef,
     FileSystemEndpointTypeDef,
     FileSystemFailureDetailsTypeDef,
     LifecycleTransitionReasonTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     OpenZFSClientConfigurationTypeDef,
     OpenZFSOriginSnapshotConfigurationTypeDef,
+    PaginatorConfigTypeDef,
     ReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
+    ReleaseFileSystemNfsV3LocksResponseTypeDef,
+    ResponseMetadataTypeDef,
     RestoreVolumeFromSnapshotRequestRequestTypeDef,
+    RestoreVolumeFromSnapshotResponseTypeDef,
     SelfManagedActiveDirectoryAttributesTypeDef,
     SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
     SvmEndpointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
+    UpdateFileSystemResponseTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     WindowsAuditLogConfigurationTypeDef,
     AssociateFileSystemAliasesResponseTypeDef,
-    CancelDataRepositoryTaskResponseTypeDef,
-    CreateFileSystemFromBackupResponseTypeDef,
-    CreateFileSystemResponseTypeDef,
-    DeleteBackupResponseTypeDef,
-    DeleteDataRepositoryAssociationResponseTypeDef,
-    DeleteFileCacheResponseTypeDef,
-    DeleteSnapshotResponseTypeDef,
-    DeleteStorageVirtualMachineResponseTypeDef,
     DescribeFileSystemAliasesResponseTypeDef,
-    DescribeFileSystemsResponseTypeDef,
     DisassociateFileSystemAliasesResponseTypeDef,
-    ReleaseFileSystemNfsV3LocksResponseTypeDef,
-    RestoreVolumeFromSnapshotResponseTypeDef,
-    UpdateFileSystemResponseTypeDef,
     NFSDataRepositoryConfigurationTypeDef,
     S3DataRepositoryConfigurationTypeDef,
     CopyBackupRequestRequestTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     DeleteFileSystemLustreConfigurationTypeDef,
     DeleteFileSystemLustreResponseTypeDef,
@@ -492,19 +494,17 @@
     CreateFileSystemWindowsConfigurationTypeDef,
     CreateOntapVolumeConfigurationTypeDef,
     OntapVolumeConfigurationTypeDef,
     UpdateOntapVolumeConfigurationTypeDef,
     DataRepositoryConfigurationTypeDef,
     DescribeDataRepositoryTasksRequestRequestTypeDef,
     DataRepositoryTaskTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeBackupsRequestRequestTypeDef,
     DescribeDataRepositoryAssociationsRequestRequestTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
-    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef,
     DescribeStorageVirtualMachinesRequestRequestTypeDef,
     DescribeVolumesRequestDescribeVolumesPaginateTypeDef,
     DescribeVolumesRequestRequestTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
     FileCacheLustreConfigurationTypeDef,
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

### Comparing `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/SOURCES.txt` & `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.26.37/setup.py` & `mypy-boto3-fsx-1.27.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-fsx.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-fsx",
-    version="1.26.37",
+    version="1.27.0",
     packages=["mypy_boto3_fsx"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FSx 1.26.37 service generated with mypy-boto3-builder 7.12.2"
+        "Type annotations for boto3.FSx 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/",
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


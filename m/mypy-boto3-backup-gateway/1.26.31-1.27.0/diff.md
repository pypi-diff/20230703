# Comparing `tmp/mypy-boto3-backup-gateway-1.26.31.tar.gz` & `tmp/mypy-boto3-backup-gateway-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-backup-gateway-1.26.31.tar", last modified: Thu Dec 15 20:33:05 2022, max compression
+gzip compressed data, was "mypy-boto3-backup-gateway-1.27.0.tar", last modified: Mon Jul  3 19:50:24 2023, max compression
```

## Comparing `mypy-boto3-backup-gateway-1.26.31.tar` & `mypy-boto3-backup-gateway-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 20:33:05.768164 mypy-boto3-backup-gateway-1.26.31/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-15 20:31:56.000000 mypy-boto3-backup-gateway-1.26.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15921 2022-12-15 20:33:05.768164 mypy-boto3-backup-gateway-1.26.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14407 2022-12-15 20:31:56.000000 mypy-boto3-backup-gateway-1.26.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 20:33:05.768164 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2022-12-15 20:31:56.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2022-12-15 20:31:56.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2022-12-15 20:31:56.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20008 2022-12-15 20:31:57.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19973 2022-12-15 20:31:57.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2022-12-15 20:31:57.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8291 2022-12-15 20:31:57.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2022-12-15 20:31:57.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2022-12-15 20:31:57.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 20:31:56.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19636 2022-12-15 20:31:57.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19619 2022-12-15 20:31:57.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-15 20:31:56.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 20:33:05.768164 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15921 2022-12-15 20:33:05.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2022-12-15 20:33:05.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 20:33:05.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 20:33:05.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-15 20:33:05.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-15 20:33:05.000000 mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-15 20:33:05.768164 mypy-boto3-backup-gateway-1.26.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2022-12-15 20:31:56.000000 mypy-boto3-backup-gateway-1.26.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.950865 mypy-boto3-backup-gateway-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15904 2023-07-03 19:50:24.950865 mypy-boto3-backup-gateway-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.938865 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19973 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-07-03 19:33:04.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19690 2023-07-03 19:33:04.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-07-03 19:33:04.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.950865 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15904 2023-07-03 19:50:24.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 19:50:24.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:24.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:50:24.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:24.950865 mypy-boto3-backup-gateway-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/setup.py
```

### Comparing `mypy-boto3-backup-gateway-1.26.31/LICENSE` & `mypy-boto3-backup-gateway-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-backup-gateway-1.26.31/PKG-INFO` & `mypy-boto3-backup-gateway-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup-gateway
-Version: 1.26.31
-Summary: Type annotations for boto3.BackupGateway 1.26.31 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.BackupGateway 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-backup-gateway"></a>
 
 # mypy-boto3-backup-gateway
 
 [![PyPI - mypy-boto3-backup-gateway](https://img.shields.io/pypi/v/mypy-boto3-backup-gateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup-gateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup-gateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup-gateway)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backup-gateway?color=blue)](https://pypistats.org/packages/mypy-boto3-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupGateway 1.26.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
+[boto3.BackupGateway 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
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
 [mypy-boto3-backup-gateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,74 +334,74 @@
 
 `mypy_boto3_backup_gateway.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_backup_gateway.type_defs import (
     AssociateGatewayToServerInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateGatewayToServerOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     TagTypeDef,
+    CreateGatewayOutputTypeDef,
     DeleteGatewayInputRequestTypeDef,
+    DeleteGatewayOutputTypeDef,
     DeleteHypervisorInputRequestTypeDef,
+    DeleteHypervisorOutputTypeDef,
     DisassociateGatewayFromServerInputRequestTypeDef,
+    DisassociateGatewayFromServerOutputTypeDef,
     MaintenanceStartTimeTypeDef,
     GatewayTypeDef,
     GetBandwidthRateLimitScheduleInputRequestTypeDef,
     GetGatewayInputRequestTypeDef,
     GetHypervisorInputRequestTypeDef,
     HypervisorDetailsTypeDef,
     GetHypervisorPropertyMappingsInputRequestTypeDef,
     VmwareToAwsTagMappingTypeDef,
     GetVirtualMachineInputRequestTypeDef,
     HypervisorTypeDef,
-    PaginatorConfigTypeDef,
+    ImportHypervisorConfigurationOutputTypeDef,
+    ListGatewaysInputListGatewaysPaginateTypeDef,
     ListGatewaysInputRequestTypeDef,
+    ListHypervisorsInputListHypervisorsPaginateTypeDef,
     ListHypervisorsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
     ListVirtualMachinesInputRequestTypeDef,
     VirtualMachineTypeDef,
-    PutMaintenanceStartTimeInputRequestTypeDef,
-    StartVirtualMachinesMetadataSyncInputRequestTypeDef,
-    TestHypervisorConfigurationInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateGatewayInformationInputRequestTypeDef,
-    UpdateGatewaySoftwareNowInputRequestTypeDef,
-    UpdateHypervisorInputRequestTypeDef,
-    VmwareTagTypeDef,
-    AssociateGatewayToServerOutputTypeDef,
-    CreateGatewayOutputTypeDef,
-    DeleteGatewayOutputTypeDef,
-    DeleteHypervisorOutputTypeDef,
-    DisassociateGatewayFromServerOutputTypeDef,
-    ImportHypervisorConfigurationOutputTypeDef,
+    PaginatorConfigTypeDef,
     PutBandwidthRateLimitScheduleOutputTypeDef,
     PutHypervisorPropertyMappingsOutputTypeDef,
+    PutMaintenanceStartTimeInputRequestTypeDef,
     PutMaintenanceStartTimeOutputTypeDef,
+    ResponseMetadataTypeDef,
+    StartVirtualMachinesMetadataSyncInputRequestTypeDef,
     StartVirtualMachinesMetadataSyncOutputTypeDef,
     TagResourceOutputTypeDef,
+    TestHypervisorConfigurationInputRequestTypeDef,
+    UntagResourceInputRequestTypeDef,
     UntagResourceOutputTypeDef,
+    UpdateGatewayInformationInputRequestTypeDef,
     UpdateGatewayInformationOutputTypeDef,
+    UpdateGatewaySoftwareNowInputRequestTypeDef,
     UpdateGatewaySoftwareNowOutputTypeDef,
+    UpdateHypervisorInputRequestTypeDef,
     UpdateHypervisorOutputTypeDef,
+    VmwareTagTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
     PutBandwidthRateLimitScheduleInputRequestTypeDef,
     CreateGatewayInputRequestTypeDef,
     ImportHypervisorConfigurationInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     GatewayDetailsTypeDef,
     ListGatewaysOutputTypeDef,
     GetHypervisorOutputTypeDef,
     GetHypervisorPropertyMappingsOutputTypeDef,
     PutHypervisorPropertyMappingsInputRequestTypeDef,
     ListHypervisorsOutputTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
-    ListHypervisorsInputListHypervisorsPaginateTypeDef,
-    ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
     ListVirtualMachinesOutputTypeDef,
     VirtualMachineDetailsTypeDef,
     GetGatewayOutputTypeDef,
     GetVirtualMachineOutputTypeDef,
 )
 
 
@@ -412,42 +412,42 @@
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

### Comparing `mypy-boto3-backup-gateway-1.26.31/README.md` & `mypy-boto3-backup-gateway-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-backup-gateway"></a>
 
 # mypy-boto3-backup-gateway
 
 [![PyPI - mypy-boto3-backup-gateway](https://img.shields.io/pypi/v/mypy-boto3-backup-gateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup-gateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup-gateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup-gateway)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backup-gateway?color=blue)](https://pypistats.org/packages/mypy-boto3-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupGateway 1.26.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
+[boto3.BackupGateway 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
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
 [mypy-boto3-backup-gateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,74 +302,74 @@
 
 `mypy_boto3_backup_gateway.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_backup_gateway.type_defs import (
     AssociateGatewayToServerInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateGatewayToServerOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     TagTypeDef,
+    CreateGatewayOutputTypeDef,
     DeleteGatewayInputRequestTypeDef,
+    DeleteGatewayOutputTypeDef,
     DeleteHypervisorInputRequestTypeDef,
+    DeleteHypervisorOutputTypeDef,
     DisassociateGatewayFromServerInputRequestTypeDef,
+    DisassociateGatewayFromServerOutputTypeDef,
     MaintenanceStartTimeTypeDef,
     GatewayTypeDef,
     GetBandwidthRateLimitScheduleInputRequestTypeDef,
     GetGatewayInputRequestTypeDef,
     GetHypervisorInputRequestTypeDef,
     HypervisorDetailsTypeDef,
     GetHypervisorPropertyMappingsInputRequestTypeDef,
     VmwareToAwsTagMappingTypeDef,
     GetVirtualMachineInputRequestTypeDef,
     HypervisorTypeDef,
-    PaginatorConfigTypeDef,
+    ImportHypervisorConfigurationOutputTypeDef,
+    ListGatewaysInputListGatewaysPaginateTypeDef,
     ListGatewaysInputRequestTypeDef,
+    ListHypervisorsInputListHypervisorsPaginateTypeDef,
     ListHypervisorsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
     ListVirtualMachinesInputRequestTypeDef,
     VirtualMachineTypeDef,
-    PutMaintenanceStartTimeInputRequestTypeDef,
-    StartVirtualMachinesMetadataSyncInputRequestTypeDef,
-    TestHypervisorConfigurationInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateGatewayInformationInputRequestTypeDef,
-    UpdateGatewaySoftwareNowInputRequestTypeDef,
-    UpdateHypervisorInputRequestTypeDef,
-    VmwareTagTypeDef,
-    AssociateGatewayToServerOutputTypeDef,
-    CreateGatewayOutputTypeDef,
-    DeleteGatewayOutputTypeDef,
-    DeleteHypervisorOutputTypeDef,
-    DisassociateGatewayFromServerOutputTypeDef,
-    ImportHypervisorConfigurationOutputTypeDef,
+    PaginatorConfigTypeDef,
     PutBandwidthRateLimitScheduleOutputTypeDef,
     PutHypervisorPropertyMappingsOutputTypeDef,
+    PutMaintenanceStartTimeInputRequestTypeDef,
     PutMaintenanceStartTimeOutputTypeDef,
+    ResponseMetadataTypeDef,
+    StartVirtualMachinesMetadataSyncInputRequestTypeDef,
     StartVirtualMachinesMetadataSyncOutputTypeDef,
     TagResourceOutputTypeDef,
+    TestHypervisorConfigurationInputRequestTypeDef,
+    UntagResourceInputRequestTypeDef,
     UntagResourceOutputTypeDef,
+    UpdateGatewayInformationInputRequestTypeDef,
     UpdateGatewayInformationOutputTypeDef,
+    UpdateGatewaySoftwareNowInputRequestTypeDef,
     UpdateGatewaySoftwareNowOutputTypeDef,
+    UpdateHypervisorInputRequestTypeDef,
     UpdateHypervisorOutputTypeDef,
+    VmwareTagTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
     PutBandwidthRateLimitScheduleInputRequestTypeDef,
     CreateGatewayInputRequestTypeDef,
     ImportHypervisorConfigurationInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     GatewayDetailsTypeDef,
     ListGatewaysOutputTypeDef,
     GetHypervisorOutputTypeDef,
     GetHypervisorPropertyMappingsOutputTypeDef,
     PutHypervisorPropertyMappingsInputRequestTypeDef,
     ListHypervisorsOutputTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
-    ListHypervisorsInputListHypervisorsPaginateTypeDef,
-    ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
     ListVirtualMachinesOutputTypeDef,
     VirtualMachineDetailsTypeDef,
     GetGatewayOutputTypeDef,
     GetVirtualMachineOutputTypeDef,
 )
 
 
@@ -380,42 +380,42 @@
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

### Comparing `mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/__init__.py` & `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/__init__.pyi` & `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/__main__.py` & `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.BackupGateway 1.26.31\nVersion:         1.26.31\nBuilder"
-        " version: 7.12.0\nDocs:           "
+        "Type annotations for boto3.BackupGateway 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.31")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/client.py` & `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/client.pyi` & `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/literals.py` & `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
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
@@ -80,31 +81,34 @@
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
@@ -183,14 +187,15 @@
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
@@ -201,34 +206,38 @@
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
@@ -241,14 +250,15 @@
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
@@ -267,16 +277,19 @@
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
@@ -356,18 +369,21 @@
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

### Comparing `mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/literals.pyi` & `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
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
@@ -78,31 +79,34 @@
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
@@ -181,14 +185,15 @@
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
@@ -199,34 +204,38 @@
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
@@ -239,14 +248,15 @@
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
@@ -265,16 +275,19 @@
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
@@ -354,18 +367,21 @@
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

### Comparing `mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/paginator.py` & `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,61 +32,56 @@
     ListHypervisorsOutputTypeDef,
     ListVirtualMachinesOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListGatewaysPaginator", "ListHypervisorsPaginator", "ListVirtualMachinesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/paginators/#listgatewayspaginator)
         """
 
-
 class ListHypervisorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListHypervisors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/paginators/#listhypervisorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHypervisorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListHypervisors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/paginators/#listhypervisorspaginator)
         """
 
-
 class ListVirtualMachinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListVirtualMachines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/paginators/#listvirtualmachinespaginator)
     """
 
     def paginate(
-        self, *, HypervisorArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, HypervisorArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVirtualMachinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListVirtualMachines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/paginators/#listvirtualmachinespaginator)
         """
```

### Comparing `mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/paginator.pyi` & `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,56 +32,61 @@
     ListHypervisorsOutputTypeDef,
     ListVirtualMachinesOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListGatewaysPaginator", "ListHypervisorsPaginator", "ListVirtualMachinesPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/paginators/#listgatewayspaginator)
         """
 
+
 class ListHypervisorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListHypervisors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/paginators/#listhypervisorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHypervisorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListHypervisors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/paginators/#listhypervisorspaginator)
         """
 
+
 class ListVirtualMachinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListVirtualMachines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/paginators/#listvirtualmachinespaginator)
     """
 
     def paginate(
-        self, *, HypervisorArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, HypervisorArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVirtualMachinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListVirtualMachines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/paginators/#listvirtualmachinespaginator)
         """
```

### Comparing `mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/type_defs.py` & `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -22,99 +22,95 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateGatewayToServerInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateGatewayToServerOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
     "TagTypeDef",
+    "CreateGatewayOutputTypeDef",
     "DeleteGatewayInputRequestTypeDef",
+    "DeleteGatewayOutputTypeDef",
     "DeleteHypervisorInputRequestTypeDef",
+    "DeleteHypervisorOutputTypeDef",
     "DisassociateGatewayFromServerInputRequestTypeDef",
+    "DisassociateGatewayFromServerOutputTypeDef",
     "MaintenanceStartTimeTypeDef",
     "GatewayTypeDef",
     "GetBandwidthRateLimitScheduleInputRequestTypeDef",
     "GetGatewayInputRequestTypeDef",
     "GetHypervisorInputRequestTypeDef",
     "HypervisorDetailsTypeDef",
     "GetHypervisorPropertyMappingsInputRequestTypeDef",
     "VmwareToAwsTagMappingTypeDef",
     "GetVirtualMachineInputRequestTypeDef",
     "HypervisorTypeDef",
-    "PaginatorConfigTypeDef",
+    "ImportHypervisorConfigurationOutputTypeDef",
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
     "ListGatewaysInputRequestTypeDef",
+    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
     "ListHypervisorsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
     "ListVirtualMachinesInputRequestTypeDef",
     "VirtualMachineTypeDef",
-    "PutMaintenanceStartTimeInputRequestTypeDef",
-    "StartVirtualMachinesMetadataSyncInputRequestTypeDef",
-    "TestHypervisorConfigurationInputRequestTypeDef",
-    "UntagResourceInputRequestTypeDef",
-    "UpdateGatewayInformationInputRequestTypeDef",
-    "UpdateGatewaySoftwareNowInputRequestTypeDef",
-    "UpdateHypervisorInputRequestTypeDef",
-    "VmwareTagTypeDef",
-    "AssociateGatewayToServerOutputTypeDef",
-    "CreateGatewayOutputTypeDef",
-    "DeleteGatewayOutputTypeDef",
-    "DeleteHypervisorOutputTypeDef",
-    "DisassociateGatewayFromServerOutputTypeDef",
-    "ImportHypervisorConfigurationOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "PutBandwidthRateLimitScheduleOutputTypeDef",
     "PutHypervisorPropertyMappingsOutputTypeDef",
+    "PutMaintenanceStartTimeInputRequestTypeDef",
     "PutMaintenanceStartTimeOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartVirtualMachinesMetadataSyncInputRequestTypeDef",
     "StartVirtualMachinesMetadataSyncOutputTypeDef",
     "TagResourceOutputTypeDef",
+    "TestHypervisorConfigurationInputRequestTypeDef",
+    "UntagResourceInputRequestTypeDef",
     "UntagResourceOutputTypeDef",
+    "UpdateGatewayInformationInputRequestTypeDef",
     "UpdateGatewayInformationOutputTypeDef",
+    "UpdateGatewaySoftwareNowInputRequestTypeDef",
     "UpdateGatewaySoftwareNowOutputTypeDef",
+    "UpdateHypervisorInputRequestTypeDef",
     "UpdateHypervisorOutputTypeDef",
+    "VmwareTagTypeDef",
     "GetBandwidthRateLimitScheduleOutputTypeDef",
     "PutBandwidthRateLimitScheduleInputRequestTypeDef",
     "CreateGatewayInputRequestTypeDef",
     "ImportHypervisorConfigurationInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "GatewayDetailsTypeDef",
     "ListGatewaysOutputTypeDef",
     "GetHypervisorOutputTypeDef",
     "GetHypervisorPropertyMappingsOutputTypeDef",
     "PutHypervisorPropertyMappingsInputRequestTypeDef",
     "ListHypervisorsOutputTypeDef",
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
-    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
-    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
     "ListVirtualMachinesOutputTypeDef",
     "VirtualMachineDetailsTypeDef",
     "GetGatewayOutputTypeDef",
     "GetVirtualMachineOutputTypeDef",
 )
 
 AssociateGatewayToServerInputRequestTypeDef = TypedDict(
     "AssociateGatewayToServerInputRequestTypeDef",
     {
         "GatewayArn": str,
         "ServerArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateGatewayToServerOutputTypeDef = TypedDict(
+    "AssociateGatewayToServerOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_RequiredBandwidthRateLimitIntervalTypeDef",
     {
         "DaysOfWeek": List[int],
@@ -128,50 +124,80 @@
     "_OptionalBandwidthRateLimitIntervalTypeDef",
     {
         "AverageUploadRateLimitInBitsPerSec": int,
     },
     total=False,
 )
 
-
 class BandwidthRateLimitIntervalTypeDef(
     _RequiredBandwidthRateLimitIntervalTypeDef, _OptionalBandwidthRateLimitIntervalTypeDef
 ):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateGatewayOutputTypeDef = TypedDict(
+    "CreateGatewayOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteGatewayInputRequestTypeDef = TypedDict(
     "DeleteGatewayInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
+DeleteGatewayOutputTypeDef = TypedDict(
+    "DeleteGatewayOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteHypervisorInputRequestTypeDef = TypedDict(
     "DeleteHypervisorInputRequestTypeDef",
     {
         "HypervisorArn": str,
     },
 )
 
+DeleteHypervisorOutputTypeDef = TypedDict(
+    "DeleteHypervisorOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateGatewayFromServerInputRequestTypeDef = TypedDict(
     "DisassociateGatewayFromServerInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
+DisassociateGatewayFromServerOutputTypeDef = TypedDict(
+    "DisassociateGatewayFromServerOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredMaintenanceStartTimeTypeDef = TypedDict(
     "_RequiredMaintenanceStartTimeTypeDef",
     {
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
 )
@@ -180,21 +206,19 @@
     {
         "DayOfMonth": int,
         "DayOfWeek": int,
     },
     total=False,
 )
 
-
 class MaintenanceStartTimeTypeDef(
     _RequiredMaintenanceStartTimeTypeDef, _OptionalMaintenanceStartTimeTypeDef
 ):
     pass
 
-
 GatewayTypeDef = TypedDict(
     "GatewayTypeDef",
     {
         "GatewayArn": str,
         "GatewayDisplayName": str,
         "GatewayType": Literal["BACKUP_VM"],
         "HypervisorId": str,
@@ -272,33 +296,47 @@
         "KmsKeyArn": str,
         "Name": str,
         "State": HypervisorStateType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ImportHypervisorConfigurationOutputTypeDef = TypedDict(
+    "ImportHypervisorConfigurationOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "HypervisorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListGatewaysInputRequestTypeDef = TypedDict(
     "ListGatewaysInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListHypervisorsInputListHypervisorsPaginateTypeDef = TypedDict(
+    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListHypervisorsInputRequestTypeDef = TypedDict(
     "ListHypervisorsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -307,14 +345,23 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef = TypedDict(
+    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
+    {
+        "HypervisorArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListVirtualMachinesInputRequestTypeDef = TypedDict(
     "ListVirtualMachinesInputRequestTypeDef",
     {
         "HypervisorArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -330,14 +377,40 @@
         "Name": str,
         "Path": str,
         "ResourceArn": str,
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
+PutBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
+    "PutBandwidthRateLimitScheduleOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutHypervisorPropertyMappingsOutputTypeDef = TypedDict(
+    "PutHypervisorPropertyMappingsOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "_RequiredPutMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayArn": str,
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
@@ -347,29 +420,62 @@
     {
         "DayOfMonth": int,
         "DayOfWeek": int,
     },
     total=False,
 )
 
-
 class PutMaintenanceStartTimeInputRequestTypeDef(
     _RequiredPutMaintenanceStartTimeInputRequestTypeDef,
     _OptionalPutMaintenanceStartTimeInputRequestTypeDef,
 ):
     pass
 
+PutMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "PutMaintenanceStartTimeOutputTypeDef",
+    {
+        "GatewayArn": str,
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
 
 StartVirtualMachinesMetadataSyncInputRequestTypeDef = TypedDict(
     "StartVirtualMachinesMetadataSyncInputRequestTypeDef",
     {
         "HypervisorArn": str,
     },
 )
 
+StartVirtualMachinesMetadataSyncOutputTypeDef = TypedDict(
+    "StartVirtualMachinesMetadataSyncOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TagResourceOutputTypeDef = TypedDict(
+    "TagResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredTestHypervisorConfigurationInputRequestTypeDef = TypedDict(
     "_RequiredTestHypervisorConfigurationInputRequestTypeDef",
     {
         "GatewayArn": str,
         "Host": str,
     },
 )
@@ -378,59 +484,79 @@
     {
         "Password": str,
         "Username": str,
     },
     total=False,
 )
 
-
 class TestHypervisorConfigurationInputRequestTypeDef(
     _RequiredTestHypervisorConfigurationInputRequestTypeDef,
     _OptionalTestHypervisorConfigurationInputRequestTypeDef,
 ):
     pass
 
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UntagResourceOutputTypeDef = TypedDict(
+    "UntagResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateGatewayInformationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayInformationInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 _OptionalUpdateGatewayInformationInputRequestTypeDef = TypedDict(
     "_OptionalUpdateGatewayInformationInputRequestTypeDef",
     {
         "GatewayDisplayName": str,
     },
     total=False,
 )
 
-
 class UpdateGatewayInformationInputRequestTypeDef(
     _RequiredUpdateGatewayInformationInputRequestTypeDef,
     _OptionalUpdateGatewayInformationInputRequestTypeDef,
 ):
     pass
 
+UpdateGatewayInformationOutputTypeDef = TypedDict(
+    "UpdateGatewayInformationOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 UpdateGatewaySoftwareNowInputRequestTypeDef = TypedDict(
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
+UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
+    "UpdateGatewaySoftwareNowOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateHypervisorInputRequestTypeDef = TypedDict(
     "_RequiredUpdateHypervisorInputRequestTypeDef",
     {
         "HypervisorArn": str,
     },
 )
 _OptionalUpdateHypervisorInputRequestTypeDef = TypedDict(
@@ -441,157 +567,43 @@
         "Name": str,
         "Password": str,
         "Username": str,
     },
     total=False,
 )
 
-
 class UpdateHypervisorInputRequestTypeDef(
     _RequiredUpdateHypervisorInputRequestTypeDef, _OptionalUpdateHypervisorInputRequestTypeDef
 ):
     pass
 
+UpdateHypervisorOutputTypeDef = TypedDict(
+    "UpdateHypervisorOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 VmwareTagTypeDef = TypedDict(
     "VmwareTagTypeDef",
     {
         "VmwareCategory": str,
         "VmwareTagDescription": str,
         "VmwareTagName": str,
     },
     total=False,
 )
 
-AssociateGatewayToServerOutputTypeDef = TypedDict(
-    "AssociateGatewayToServerOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGatewayOutputTypeDef = TypedDict(
-    "CreateGatewayOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteGatewayOutputTypeDef = TypedDict(
-    "DeleteGatewayOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteHypervisorOutputTypeDef = TypedDict(
-    "DeleteHypervisorOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateGatewayFromServerOutputTypeDef = TypedDict(
-    "DisassociateGatewayFromServerOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ImportHypervisorConfigurationOutputTypeDef = TypedDict(
-    "ImportHypervisorConfigurationOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
-    "PutBandwidthRateLimitScheduleOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutHypervisorPropertyMappingsOutputTypeDef = TypedDict(
-    "PutHypervisorPropertyMappingsOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "PutMaintenanceStartTimeOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartVirtualMachinesMetadataSyncOutputTypeDef = TypedDict(
-    "StartVirtualMachinesMetadataSyncOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TagResourceOutputTypeDef = TypedDict(
-    "TagResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UntagResourceOutputTypeDef = TypedDict(
-    "UntagResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGatewayInformationOutputTypeDef = TypedDict(
-    "UpdateGatewayInformationOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
-    "UpdateGatewaySoftwareNowOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateHypervisorOutputTypeDef = TypedDict(
-    "UpdateHypervisorOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
     "GetBandwidthRateLimitScheduleOutputTypeDef",
     {
         "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
         "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "PutBandwidthRateLimitScheduleInputRequestTypeDef",
     {
         "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
@@ -611,21 +623,19 @@
     "_OptionalCreateGatewayInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateGatewayInputRequestTypeDef(
     _RequiredCreateGatewayInputRequestTypeDef, _OptionalCreateGatewayInputRequestTypeDef
 ):
     pass
 
-
 _RequiredImportHypervisorConfigurationInputRequestTypeDef = TypedDict(
     "_RequiredImportHypervisorConfigurationInputRequestTypeDef",
     {
         "Host": str,
         "Name": str,
     },
 )
@@ -636,28 +646,26 @@
         "Password": str,
         "Tags": Sequence[TagTypeDef],
         "Username": str,
     },
     total=False,
 )
 
-
 class ImportHypervisorConfigurationInputRequestTypeDef(
     _RequiredImportHypervisorConfigurationInputRequestTypeDef,
     _OptionalImportHypervisorConfigurationInputRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
@@ -681,33 +689,33 @@
 )
 
 ListGatewaysOutputTypeDef = TypedDict(
     "ListGatewaysOutputTypeDef",
     {
         "Gateways": List[GatewayTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetHypervisorOutputTypeDef = TypedDict(
     "GetHypervisorOutputTypeDef",
     {
         "Hypervisor": HypervisorDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetHypervisorPropertyMappingsOutputTypeDef = TypedDict(
     "GetHypervisorPropertyMappingsOutputTypeDef",
     {
         "HypervisorArn": str,
         "IamRoleArn": str,
         "VmwareToAwsTagMappings": List[VmwareToAwsTagMappingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutHypervisorPropertyMappingsInputRequestTypeDef = TypedDict(
     "PutHypervisorPropertyMappingsInputRequestTypeDef",
     {
         "HypervisorArn": str,
@@ -717,49 +725,24 @@
 )
 
 ListHypervisorsOutputTypeDef = TypedDict(
     "ListHypervisorsOutputTypeDef",
     {
         "Hypervisors": List[HypervisorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
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
-ListHypervisorsInputListHypervisorsPaginateTypeDef = TypedDict(
-    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef = TypedDict(
-    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
-    {
-        "HypervisorArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ListVirtualMachinesOutputTypeDef = TypedDict(
     "ListVirtualMachinesOutputTypeDef",
     {
         "NextToken": str,
         "VirtualMachines": List[VirtualMachineTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VirtualMachineDetailsTypeDef = TypedDict(
     "VirtualMachineDetailsTypeDef",
     {
         "HostName": str,
@@ -773,18 +756,18 @@
     total=False,
 )
 
 GetGatewayOutputTypeDef = TypedDict(
     "GetGatewayOutputTypeDef",
     {
         "Gateway": GatewayDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVirtualMachineOutputTypeDef = TypedDict(
     "GetVirtualMachineOutputTypeDef",
     {
         "VirtualMachine": VirtualMachineDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway/type_defs.pyi` & `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,98 +22,96 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateGatewayToServerInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateGatewayToServerOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
     "TagTypeDef",
+    "CreateGatewayOutputTypeDef",
     "DeleteGatewayInputRequestTypeDef",
+    "DeleteGatewayOutputTypeDef",
     "DeleteHypervisorInputRequestTypeDef",
+    "DeleteHypervisorOutputTypeDef",
     "DisassociateGatewayFromServerInputRequestTypeDef",
+    "DisassociateGatewayFromServerOutputTypeDef",
     "MaintenanceStartTimeTypeDef",
     "GatewayTypeDef",
     "GetBandwidthRateLimitScheduleInputRequestTypeDef",
     "GetGatewayInputRequestTypeDef",
     "GetHypervisorInputRequestTypeDef",
     "HypervisorDetailsTypeDef",
     "GetHypervisorPropertyMappingsInputRequestTypeDef",
     "VmwareToAwsTagMappingTypeDef",
     "GetVirtualMachineInputRequestTypeDef",
     "HypervisorTypeDef",
-    "PaginatorConfigTypeDef",
+    "ImportHypervisorConfigurationOutputTypeDef",
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
     "ListGatewaysInputRequestTypeDef",
+    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
     "ListHypervisorsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
     "ListVirtualMachinesInputRequestTypeDef",
     "VirtualMachineTypeDef",
-    "PutMaintenanceStartTimeInputRequestTypeDef",
-    "StartVirtualMachinesMetadataSyncInputRequestTypeDef",
-    "TestHypervisorConfigurationInputRequestTypeDef",
-    "UntagResourceInputRequestTypeDef",
-    "UpdateGatewayInformationInputRequestTypeDef",
-    "UpdateGatewaySoftwareNowInputRequestTypeDef",
-    "UpdateHypervisorInputRequestTypeDef",
-    "VmwareTagTypeDef",
-    "AssociateGatewayToServerOutputTypeDef",
-    "CreateGatewayOutputTypeDef",
-    "DeleteGatewayOutputTypeDef",
-    "DeleteHypervisorOutputTypeDef",
-    "DisassociateGatewayFromServerOutputTypeDef",
-    "ImportHypervisorConfigurationOutputTypeDef",
+    "PaginatorConfigTypeDef",
     "PutBandwidthRateLimitScheduleOutputTypeDef",
     "PutHypervisorPropertyMappingsOutputTypeDef",
+    "PutMaintenanceStartTimeInputRequestTypeDef",
     "PutMaintenanceStartTimeOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartVirtualMachinesMetadataSyncInputRequestTypeDef",
     "StartVirtualMachinesMetadataSyncOutputTypeDef",
     "TagResourceOutputTypeDef",
+    "TestHypervisorConfigurationInputRequestTypeDef",
+    "UntagResourceInputRequestTypeDef",
     "UntagResourceOutputTypeDef",
+    "UpdateGatewayInformationInputRequestTypeDef",
     "UpdateGatewayInformationOutputTypeDef",
+    "UpdateGatewaySoftwareNowInputRequestTypeDef",
     "UpdateGatewaySoftwareNowOutputTypeDef",
+    "UpdateHypervisorInputRequestTypeDef",
     "UpdateHypervisorOutputTypeDef",
+    "VmwareTagTypeDef",
     "GetBandwidthRateLimitScheduleOutputTypeDef",
     "PutBandwidthRateLimitScheduleInputRequestTypeDef",
     "CreateGatewayInputRequestTypeDef",
     "ImportHypervisorConfigurationInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "GatewayDetailsTypeDef",
     "ListGatewaysOutputTypeDef",
     "GetHypervisorOutputTypeDef",
     "GetHypervisorPropertyMappingsOutputTypeDef",
     "PutHypervisorPropertyMappingsInputRequestTypeDef",
     "ListHypervisorsOutputTypeDef",
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
-    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
-    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
     "ListVirtualMachinesOutputTypeDef",
     "VirtualMachineDetailsTypeDef",
     "GetGatewayOutputTypeDef",
     "GetVirtualMachineOutputTypeDef",
 )
 
 AssociateGatewayToServerInputRequestTypeDef = TypedDict(
     "AssociateGatewayToServerInputRequestTypeDef",
     {
         "GatewayArn": str,
         "ServerArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateGatewayToServerOutputTypeDef = TypedDict(
+    "AssociateGatewayToServerOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_RequiredBandwidthRateLimitIntervalTypeDef",
     {
         "DaysOfWeek": List[int],
@@ -127,48 +125,82 @@
     "_OptionalBandwidthRateLimitIntervalTypeDef",
     {
         "AverageUploadRateLimitInBitsPerSec": int,
     },
     total=False,
 )
 
+
 class BandwidthRateLimitIntervalTypeDef(
     _RequiredBandwidthRateLimitIntervalTypeDef, _OptionalBandwidthRateLimitIntervalTypeDef
 ):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateGatewayOutputTypeDef = TypedDict(
+    "CreateGatewayOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteGatewayInputRequestTypeDef = TypedDict(
     "DeleteGatewayInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
+DeleteGatewayOutputTypeDef = TypedDict(
+    "DeleteGatewayOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteHypervisorInputRequestTypeDef = TypedDict(
     "DeleteHypervisorInputRequestTypeDef",
     {
         "HypervisorArn": str,
     },
 )
 
+DeleteHypervisorOutputTypeDef = TypedDict(
+    "DeleteHypervisorOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateGatewayFromServerInputRequestTypeDef = TypedDict(
     "DisassociateGatewayFromServerInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
+DisassociateGatewayFromServerOutputTypeDef = TypedDict(
+    "DisassociateGatewayFromServerOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredMaintenanceStartTimeTypeDef = TypedDict(
     "_RequiredMaintenanceStartTimeTypeDef",
     {
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
 )
@@ -177,19 +209,21 @@
     {
         "DayOfMonth": int,
         "DayOfWeek": int,
     },
     total=False,
 )
 
+
 class MaintenanceStartTimeTypeDef(
     _RequiredMaintenanceStartTimeTypeDef, _OptionalMaintenanceStartTimeTypeDef
 ):
     pass
 
+
 GatewayTypeDef = TypedDict(
     "GatewayTypeDef",
     {
         "GatewayArn": str,
         "GatewayDisplayName": str,
         "GatewayType": Literal["BACKUP_VM"],
         "HypervisorId": str,
@@ -267,33 +301,47 @@
         "KmsKeyArn": str,
         "Name": str,
         "State": HypervisorStateType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ImportHypervisorConfigurationOutputTypeDef = TypedDict(
+    "ImportHypervisorConfigurationOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "HypervisorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListGatewaysInputRequestTypeDef = TypedDict(
     "ListGatewaysInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListHypervisorsInputListHypervisorsPaginateTypeDef = TypedDict(
+    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListHypervisorsInputRequestTypeDef = TypedDict(
     "ListHypervisorsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -302,14 +350,23 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef = TypedDict(
+    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
+    {
+        "HypervisorArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListVirtualMachinesInputRequestTypeDef = TypedDict(
     "ListVirtualMachinesInputRequestTypeDef",
     {
         "HypervisorArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -325,14 +382,40 @@
         "Name": str,
         "Path": str,
         "ResourceArn": str,
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
+PutBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
+    "PutBandwidthRateLimitScheduleOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutHypervisorPropertyMappingsOutputTypeDef = TypedDict(
+    "PutHypervisorPropertyMappingsOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "_RequiredPutMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayArn": str,
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
@@ -342,27 +425,64 @@
     {
         "DayOfMonth": int,
         "DayOfWeek": int,
     },
     total=False,
 )
 
+
 class PutMaintenanceStartTimeInputRequestTypeDef(
     _RequiredPutMaintenanceStartTimeInputRequestTypeDef,
     _OptionalPutMaintenanceStartTimeInputRequestTypeDef,
 ):
     pass
 
+
+PutMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "PutMaintenanceStartTimeOutputTypeDef",
+    {
+        "GatewayArn": str,
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
 StartVirtualMachinesMetadataSyncInputRequestTypeDef = TypedDict(
     "StartVirtualMachinesMetadataSyncInputRequestTypeDef",
     {
         "HypervisorArn": str,
     },
 )
 
+StartVirtualMachinesMetadataSyncOutputTypeDef = TypedDict(
+    "StartVirtualMachinesMetadataSyncOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TagResourceOutputTypeDef = TypedDict(
+    "TagResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredTestHypervisorConfigurationInputRequestTypeDef = TypedDict(
     "_RequiredTestHypervisorConfigurationInputRequestTypeDef",
     {
         "GatewayArn": str,
         "Host": str,
     },
 )
@@ -371,55 +491,83 @@
     {
         "Password": str,
         "Username": str,
     },
     total=False,
 )
 
+
 class TestHypervisorConfigurationInputRequestTypeDef(
     _RequiredTestHypervisorConfigurationInputRequestTypeDef,
     _OptionalTestHypervisorConfigurationInputRequestTypeDef,
 ):
     pass
 
+
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UntagResourceOutputTypeDef = TypedDict(
+    "UntagResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateGatewayInformationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayInformationInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 _OptionalUpdateGatewayInformationInputRequestTypeDef = TypedDict(
     "_OptionalUpdateGatewayInformationInputRequestTypeDef",
     {
         "GatewayDisplayName": str,
     },
     total=False,
 )
 
+
 class UpdateGatewayInformationInputRequestTypeDef(
     _RequiredUpdateGatewayInformationInputRequestTypeDef,
     _OptionalUpdateGatewayInformationInputRequestTypeDef,
 ):
     pass
 
+
+UpdateGatewayInformationOutputTypeDef = TypedDict(
+    "UpdateGatewayInformationOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateGatewaySoftwareNowInputRequestTypeDef = TypedDict(
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
+UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
+    "UpdateGatewaySoftwareNowOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateHypervisorInputRequestTypeDef = TypedDict(
     "_RequiredUpdateHypervisorInputRequestTypeDef",
     {
         "HypervisorArn": str,
     },
 )
 _OptionalUpdateHypervisorInputRequestTypeDef = TypedDict(
@@ -430,155 +578,45 @@
         "Name": str,
         "Password": str,
         "Username": str,
     },
     total=False,
 )
 
+
 class UpdateHypervisorInputRequestTypeDef(
     _RequiredUpdateHypervisorInputRequestTypeDef, _OptionalUpdateHypervisorInputRequestTypeDef
 ):
     pass
 
-VmwareTagTypeDef = TypedDict(
-    "VmwareTagTypeDef",
-    {
-        "VmwareCategory": str,
-        "VmwareTagDescription": str,
-        "VmwareTagName": str,
-    },
-    total=False,
-)
-
-AssociateGatewayToServerOutputTypeDef = TypedDict(
-    "AssociateGatewayToServerOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGatewayOutputTypeDef = TypedDict(
-    "CreateGatewayOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteGatewayOutputTypeDef = TypedDict(
-    "DeleteGatewayOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteHypervisorOutputTypeDef = TypedDict(
-    "DeleteHypervisorOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateGatewayFromServerOutputTypeDef = TypedDict(
-    "DisassociateGatewayFromServerOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ImportHypervisorConfigurationOutputTypeDef = TypedDict(
-    "ImportHypervisorConfigurationOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
-    "PutBandwidthRateLimitScheduleOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutHypervisorPropertyMappingsOutputTypeDef = TypedDict(
-    "PutHypervisorPropertyMappingsOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-PutMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "PutMaintenanceStartTimeOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartVirtualMachinesMetadataSyncOutputTypeDef = TypedDict(
-    "StartVirtualMachinesMetadataSyncOutputTypeDef",
+UpdateHypervisorOutputTypeDef = TypedDict(
+    "UpdateHypervisorOutputTypeDef",
     {
         "HypervisorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TagResourceOutputTypeDef = TypedDict(
-    "TagResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UntagResourceOutputTypeDef = TypedDict(
-    "UntagResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGatewayInformationOutputTypeDef = TypedDict(
-    "UpdateGatewayInformationOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
-    "UpdateGatewaySoftwareNowOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateHypervisorOutputTypeDef = TypedDict(
-    "UpdateHypervisorOutputTypeDef",
+VmwareTagTypeDef = TypedDict(
+    "VmwareTagTypeDef",
     {
-        "HypervisorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "VmwareCategory": str,
+        "VmwareTagDescription": str,
+        "VmwareTagName": str,
     },
+    total=False,
 )
 
 GetBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
     "GetBandwidthRateLimitScheduleOutputTypeDef",
     {
         "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
         "GatewayArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "PutBandwidthRateLimitScheduleInputRequestTypeDef",
     {
         "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
@@ -598,19 +636,21 @@
     "_OptionalCreateGatewayInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateGatewayInputRequestTypeDef(
     _RequiredCreateGatewayInputRequestTypeDef, _OptionalCreateGatewayInputRequestTypeDef
 ):
     pass
 
+
 _RequiredImportHypervisorConfigurationInputRequestTypeDef = TypedDict(
     "_RequiredImportHypervisorConfigurationInputRequestTypeDef",
     {
         "Host": str,
         "Name": str,
     },
 )
@@ -621,26 +661,28 @@
         "Password": str,
         "Tags": Sequence[TagTypeDef],
         "Username": str,
     },
     total=False,
 )
 
+
 class ImportHypervisorConfigurationInputRequestTypeDef(
     _RequiredImportHypervisorConfigurationInputRequestTypeDef,
     _OptionalImportHypervisorConfigurationInputRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
@@ -664,33 +706,33 @@
 )
 
 ListGatewaysOutputTypeDef = TypedDict(
     "ListGatewaysOutputTypeDef",
     {
         "Gateways": List[GatewayTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetHypervisorOutputTypeDef = TypedDict(
     "GetHypervisorOutputTypeDef",
     {
         "Hypervisor": HypervisorDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetHypervisorPropertyMappingsOutputTypeDef = TypedDict(
     "GetHypervisorPropertyMappingsOutputTypeDef",
     {
         "HypervisorArn": str,
         "IamRoleArn": str,
         "VmwareToAwsTagMappings": List[VmwareToAwsTagMappingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutHypervisorPropertyMappingsInputRequestTypeDef = TypedDict(
     "PutHypervisorPropertyMappingsInputRequestTypeDef",
     {
         "HypervisorArn": str,
@@ -700,49 +742,24 @@
 )
 
 ListHypervisorsOutputTypeDef = TypedDict(
     "ListHypervisorsOutputTypeDef",
     {
         "Hypervisors": List[HypervisorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListHypervisorsInputListHypervisorsPaginateTypeDef = TypedDict(
-    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef = TypedDict(
-    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
-    {
-        "HypervisorArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListVirtualMachinesOutputTypeDef = TypedDict(
     "ListVirtualMachinesOutputTypeDef",
     {
         "NextToken": str,
         "VirtualMachines": List[VirtualMachineTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VirtualMachineDetailsTypeDef = TypedDict(
     "VirtualMachineDetailsTypeDef",
     {
         "HostName": str,
@@ -756,18 +773,18 @@
     total=False,
 )
 
 GetGatewayOutputTypeDef = TypedDict(
     "GetGatewayOutputTypeDef",
     {
         "Gateway": GatewayDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVirtualMachineOutputTypeDef = TypedDict(
     "GetVirtualMachineOutputTypeDef",
     {
         "VirtualMachine": VirtualMachineDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway.egg-info/PKG-INFO` & `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup-gateway
-Version: 1.26.31
-Summary: Type annotations for boto3.BackupGateway 1.26.31 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.BackupGateway 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-backup-gateway"></a>
 
 # mypy-boto3-backup-gateway
 
 [![PyPI - mypy-boto3-backup-gateway](https://img.shields.io/pypi/v/mypy-boto3-backup-gateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup-gateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup-gateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup-gateway)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backup-gateway?color=blue)](https://pypistats.org/packages/mypy-boto3-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupGateway 1.26.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
+[boto3.BackupGateway 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
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
 [mypy-boto3-backup-gateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,74 +334,74 @@
 
 `mypy_boto3_backup_gateway.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_backup_gateway.type_defs import (
     AssociateGatewayToServerInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateGatewayToServerOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     TagTypeDef,
+    CreateGatewayOutputTypeDef,
     DeleteGatewayInputRequestTypeDef,
+    DeleteGatewayOutputTypeDef,
     DeleteHypervisorInputRequestTypeDef,
+    DeleteHypervisorOutputTypeDef,
     DisassociateGatewayFromServerInputRequestTypeDef,
+    DisassociateGatewayFromServerOutputTypeDef,
     MaintenanceStartTimeTypeDef,
     GatewayTypeDef,
     GetBandwidthRateLimitScheduleInputRequestTypeDef,
     GetGatewayInputRequestTypeDef,
     GetHypervisorInputRequestTypeDef,
     HypervisorDetailsTypeDef,
     GetHypervisorPropertyMappingsInputRequestTypeDef,
     VmwareToAwsTagMappingTypeDef,
     GetVirtualMachineInputRequestTypeDef,
     HypervisorTypeDef,
-    PaginatorConfigTypeDef,
+    ImportHypervisorConfigurationOutputTypeDef,
+    ListGatewaysInputListGatewaysPaginateTypeDef,
     ListGatewaysInputRequestTypeDef,
+    ListHypervisorsInputListHypervisorsPaginateTypeDef,
     ListHypervisorsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
     ListVirtualMachinesInputRequestTypeDef,
     VirtualMachineTypeDef,
-    PutMaintenanceStartTimeInputRequestTypeDef,
-    StartVirtualMachinesMetadataSyncInputRequestTypeDef,
-    TestHypervisorConfigurationInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    UpdateGatewayInformationInputRequestTypeDef,
-    UpdateGatewaySoftwareNowInputRequestTypeDef,
-    UpdateHypervisorInputRequestTypeDef,
-    VmwareTagTypeDef,
-    AssociateGatewayToServerOutputTypeDef,
-    CreateGatewayOutputTypeDef,
-    DeleteGatewayOutputTypeDef,
-    DeleteHypervisorOutputTypeDef,
-    DisassociateGatewayFromServerOutputTypeDef,
-    ImportHypervisorConfigurationOutputTypeDef,
+    PaginatorConfigTypeDef,
     PutBandwidthRateLimitScheduleOutputTypeDef,
     PutHypervisorPropertyMappingsOutputTypeDef,
+    PutMaintenanceStartTimeInputRequestTypeDef,
     PutMaintenanceStartTimeOutputTypeDef,
+    ResponseMetadataTypeDef,
+    StartVirtualMachinesMetadataSyncInputRequestTypeDef,
     StartVirtualMachinesMetadataSyncOutputTypeDef,
     TagResourceOutputTypeDef,
+    TestHypervisorConfigurationInputRequestTypeDef,
+    UntagResourceInputRequestTypeDef,
     UntagResourceOutputTypeDef,
+    UpdateGatewayInformationInputRequestTypeDef,
     UpdateGatewayInformationOutputTypeDef,
+    UpdateGatewaySoftwareNowInputRequestTypeDef,
     UpdateGatewaySoftwareNowOutputTypeDef,
+    UpdateHypervisorInputRequestTypeDef,
     UpdateHypervisorOutputTypeDef,
+    VmwareTagTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
     PutBandwidthRateLimitScheduleInputRequestTypeDef,
     CreateGatewayInputRequestTypeDef,
     ImportHypervisorConfigurationInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     GatewayDetailsTypeDef,
     ListGatewaysOutputTypeDef,
     GetHypervisorOutputTypeDef,
     GetHypervisorPropertyMappingsOutputTypeDef,
     PutHypervisorPropertyMappingsInputRequestTypeDef,
     ListHypervisorsOutputTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
-    ListHypervisorsInputListHypervisorsPaginateTypeDef,
-    ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
     ListVirtualMachinesOutputTypeDef,
     VirtualMachineDetailsTypeDef,
     GetGatewayOutputTypeDef,
     GetVirtualMachineOutputTypeDef,
 )
 
 
@@ -412,42 +412,42 @@
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

### Comparing `mypy-boto3-backup-gateway-1.26.31/mypy_boto3_backup_gateway.egg-info/SOURCES.txt` & `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.26.31/setup.py` & `mypy-boto3-backup-gateway-1.27.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-backup-gateway.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-backup-gateway",
-    version="1.26.31",
+    version="1.27.0",
     packages=["mypy_boto3_backup_gateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.BackupGateway 1.26.31 service generated with mypy-boto3-builder"
-        " 7.12.0"
+        "Type annotations for boto3.BackupGateway 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/",
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


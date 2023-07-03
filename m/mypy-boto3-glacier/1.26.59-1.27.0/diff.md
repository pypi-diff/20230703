# Comparing `tmp/mypy-boto3-glacier-1.26.59.tar.gz` & `tmp/mypy-boto3-glacier-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-glacier-1.26.59.tar", last modified: Fri Jan 27 20:32:50 2023, max compression
+gzip compressed data, was "mypy-boto3-glacier-1.27.0.tar", last modified: Mon Jul  3 19:50:48 2023, max compression
```

## Comparing `mypy-boto3-glacier-1.26.59.tar` & `mypy-boto3-glacier-1.27.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.572096 mypy-boto3-glacier-1.26.59/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-27 20:32:07.000000 mypy-boto3-glacier-1.26.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20202 2023-01-27 20:32:50.572096 mypy-boto3-glacier-1.26.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18715 2023-01-27 20:32:07.000000 mypy-boto3-glacier-1.26.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.572096 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-01-27 20:32:07.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-01-27 20:32:07.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-01-27 20:32:07.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26613 2023-01-27 20:32:07.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26567 2023-01-27 20:32:07.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-01-27 20:32:08.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-01-27 20:32:08.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-01-27 20:32:08.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-01-27 20:32:08.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:07.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39259 2023-01-27 20:32:08.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    39151 2023-01-27 20:32:08.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    40485 2023-01-27 20:32:09.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40413 2023-01-27 20:32:08.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-27 20:32:07.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-01-27 20:32:08.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-01-27 20:32:08.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.572096 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20202 2023-01-27 20:32:50.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-01-27 20:32:50.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:50.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:50.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-27 20:32:50.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-27 20:32:50.000000 mypy-boto3-glacier-1.26.59/mypy_boto3_glacier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 20:32:50.572096 mypy-boto3-glacier-1.26.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-01-27 20:32:07.000000 mypy-boto3-glacier-1.26.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:48.515295 mypy-boto3-glacier-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-07-03 19:50:48.515295 mypy-boto3-glacier-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:48.511294 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26623 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26577 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39259 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39151 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    38670 2023-07-03 19:38:17.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38598 2023-07-03 19:38:17.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:48.515295 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-07-03 19:50:48.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-03 19:50:48.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:48.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:48.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:48.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:50:48.000000 mypy-boto3-glacier-1.27.0/mypy_boto3_glacier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:48.515295 mypy-boto3-glacier-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:38:15.000000 mypy-boto3-glacier-1.27.0/setup.py
```

### Comparing `mypy-boto3-glacier-1.26.59/LICENSE` & `mypy-boto3-glacier-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-glacier-1.26.59/PKG-INFO` & `mypy-boto3-glacier-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glacier
-Version: 1.26.59
-Summary: Type annotations for boto3.Glacier 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Glacier 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-glacier"></a>
 
 # mypy-boto3-glacier
 
 [![PyPI - mypy-boto3-glacier](https://img.shields.io/pypi/v/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glacier?color=blue)](https://pypistats.org/packages/mypy-boto3-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glacier 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[boto3.Glacier 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
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
 [mypy-boto3-glacier docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/).
 
 See how it helps to find and fix potential bugs:
 
@@ -438,105 +438,95 @@
 `mypy_boto3_glacier.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_glacier.type_defs import (
     AbortMultipartUploadInputRequestTypeDef,
     AbortVaultLockInputRequestTypeDef,
-    AccountVaultRequestTypeDef,
     AddTagsToVaultInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    ArchiveCreationOutputTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
     CompleteMultipartUploadInputMultipartUploadCompleteTypeDef,
     CompleteMultipartUploadInputRequestTypeDef,
     CompleteVaultLockInputRequestTypeDef,
     CreateVaultInputAccountCreateVaultTypeDef,
     CreateVaultInputRequestTypeDef,
     CreateVaultInputServiceResourceCreateVaultTypeDef,
+    CreateVaultOutputTypeDef,
     DataRetrievalRuleTypeDef,
     DeleteArchiveInputRequestTypeDef,
     DeleteVaultAccessPolicyInputRequestTypeDef,
     DeleteVaultInputRequestTypeDef,
     DeleteVaultNotificationsInputRequestTypeDef,
     DescribeJobInputRequestTypeDef,
     DescribeVaultInputRequestTypeDef,
     WaiterConfigTypeDef,
+    DescribeVaultOutputResponseMetadataTypeDef,
     DescribeVaultOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionTypeDef,
     GetDataRetrievalPolicyInputRequestTypeDef,
     GetJobOutputInputJobGetOutputTypeDef,
     GetJobOutputInputRequestTypeDef,
+    GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyInputRequestTypeDef,
     VaultAccessPolicyTypeDef,
     GetVaultLockInputRequestTypeDef,
+    GetVaultLockOutputTypeDef,
     GetVaultNotificationsInputRequestTypeDef,
     VaultNotificationConfigTypeDef,
     InventoryRetrievalJobDescriptionTypeDef,
     GranteeTypeDef,
+    InitiateJobOutputTypeDef,
     InitiateMultipartUploadInputRequestTypeDef,
     InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef,
+    InitiateMultipartUploadOutputTypeDef,
     VaultLockPolicyTypeDef,
+    InitiateVaultLockOutputTypeDef,
+    InventoryRetrievalJobDescriptionResponseMetadataTypeDef,
     InventoryRetrievalJobInputTypeDef,
-    PaginatorConfigTypeDef,
+    ListJobsInputListJobsPaginateTypeDef,
     ListJobsInputRequestTypeDef,
+    ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
     ListMultipartUploadsInputRequestTypeDef,
     UploadListElementTypeDef,
+    ListPartsInputListPartsPaginateTypeDef,
     ListPartsInputMultipartUploadPartsTypeDef,
     ListPartsInputRequestTypeDef,
     PartListElementTypeDef,
     ListProvisionedCapacityInputRequestTypeDef,
     ProvisionedCapacityDescriptionTypeDef,
     ListTagsForVaultInputRequestTypeDef,
+    ListTagsForVaultOutputTypeDef,
+    ListVaultsInputListVaultsPaginateTypeDef,
     ListVaultsInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PurchaseProvisionedCapacityInputRequestTypeDef,
+    PurchaseProvisionedCapacityOutputTypeDef,
     RemoveTagsFromVaultInputRequestTypeDef,
-    ServiceResourceAccountRequestTypeDef,
-    ServiceResourceArchiveRequestTypeDef,
-    ServiceResourceJobRequestTypeDef,
-    ServiceResourceMultipartUploadRequestTypeDef,
-    ServiceResourceNotificationRequestTypeDef,
-    ServiceResourceVaultRequestTypeDef,
+    ResponseMetadataTypeDef,
     UploadArchiveInputRequestTypeDef,
     UploadArchiveInputVaultUploadArchiveTypeDef,
     UploadMultipartPartInputMultipartUploadUploadPartTypeDef,
     UploadMultipartPartInputRequestTypeDef,
-    VaultArchiveRequestTypeDef,
-    VaultJobRequestTypeDef,
-    VaultMultipartUploadRequestTypeDef,
-    ArchiveCreationOutputTypeDef,
-    CreateVaultOutputTypeDef,
-    DescribeVaultOutputResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetJobOutputOutputTypeDef,
-    GetVaultLockOutputTypeDef,
-    InitiateJobOutputTypeDef,
-    InitiateMultipartUploadOutputTypeDef,
-    InitiateVaultLockOutputTypeDef,
-    InventoryRetrievalJobDescriptionResponseMetadataTypeDef,
-    ListTagsForVaultOutputTypeDef,
-    PurchaseProvisionedCapacityOutputTypeDef,
     UploadMultipartPartOutputTypeDef,
     InputSerializationTypeDef,
     OutputSerializationTypeDef,
     DataRetrievalPolicyTypeDef,
     DescribeVaultInputVaultExistsWaitTypeDef,
     DescribeVaultInputVaultNotExistsWaitTypeDef,
     ListVaultsOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
     SetVaultAccessPolicyInputRequestTypeDef,
     GetVaultNotificationsOutputTypeDef,
     SetVaultNotificationsInputNotificationSetTypeDef,
     SetVaultNotificationsInputRequestTypeDef,
     GrantTypeDef,
     InitiateVaultLockInputRequestTypeDef,
-    ListJobsInputListJobsPaginateTypeDef,
-    ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
-    ListPartsInputListPartsPaginateTypeDef,
-    ListVaultsInputListVaultsPaginateTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListPartsOutputTypeDef,
     ListProvisionedCapacityOutputTypeDef,
     SelectParametersResponseMetadataTypeDef,
     SelectParametersTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     SetDataRetrievalPolicyInputRequestTypeDef,
@@ -558,42 +548,42 @@
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

### Comparing `mypy-boto3-glacier-1.26.59/README.md` & `mypy-boto3-glacier-1.27.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-glacier"></a>
 
 # mypy-boto3-glacier
 
 [![PyPI - mypy-boto3-glacier](https://img.shields.io/pypi/v/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glacier?color=blue)](https://pypistats.org/packages/mypy-boto3-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glacier 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[boto3.Glacier 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
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
 [mypy-boto3-glacier docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/).
 
 See how it helps to find and fix potential bugs:
 
@@ -406,105 +406,95 @@
 `mypy_boto3_glacier.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_glacier.type_defs import (
     AbortMultipartUploadInputRequestTypeDef,
     AbortVaultLockInputRequestTypeDef,
-    AccountVaultRequestTypeDef,
     AddTagsToVaultInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    ArchiveCreationOutputTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
     CompleteMultipartUploadInputMultipartUploadCompleteTypeDef,
     CompleteMultipartUploadInputRequestTypeDef,
     CompleteVaultLockInputRequestTypeDef,
     CreateVaultInputAccountCreateVaultTypeDef,
     CreateVaultInputRequestTypeDef,
     CreateVaultInputServiceResourceCreateVaultTypeDef,
+    CreateVaultOutputTypeDef,
     DataRetrievalRuleTypeDef,
     DeleteArchiveInputRequestTypeDef,
     DeleteVaultAccessPolicyInputRequestTypeDef,
     DeleteVaultInputRequestTypeDef,
     DeleteVaultNotificationsInputRequestTypeDef,
     DescribeJobInputRequestTypeDef,
     DescribeVaultInputRequestTypeDef,
     WaiterConfigTypeDef,
+    DescribeVaultOutputResponseMetadataTypeDef,
     DescribeVaultOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionTypeDef,
     GetDataRetrievalPolicyInputRequestTypeDef,
     GetJobOutputInputJobGetOutputTypeDef,
     GetJobOutputInputRequestTypeDef,
+    GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyInputRequestTypeDef,
     VaultAccessPolicyTypeDef,
     GetVaultLockInputRequestTypeDef,
+    GetVaultLockOutputTypeDef,
     GetVaultNotificationsInputRequestTypeDef,
     VaultNotificationConfigTypeDef,
     InventoryRetrievalJobDescriptionTypeDef,
     GranteeTypeDef,
+    InitiateJobOutputTypeDef,
     InitiateMultipartUploadInputRequestTypeDef,
     InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef,
+    InitiateMultipartUploadOutputTypeDef,
     VaultLockPolicyTypeDef,
+    InitiateVaultLockOutputTypeDef,
+    InventoryRetrievalJobDescriptionResponseMetadataTypeDef,
     InventoryRetrievalJobInputTypeDef,
-    PaginatorConfigTypeDef,
+    ListJobsInputListJobsPaginateTypeDef,
     ListJobsInputRequestTypeDef,
+    ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
     ListMultipartUploadsInputRequestTypeDef,
     UploadListElementTypeDef,
+    ListPartsInputListPartsPaginateTypeDef,
     ListPartsInputMultipartUploadPartsTypeDef,
     ListPartsInputRequestTypeDef,
     PartListElementTypeDef,
     ListProvisionedCapacityInputRequestTypeDef,
     ProvisionedCapacityDescriptionTypeDef,
     ListTagsForVaultInputRequestTypeDef,
+    ListTagsForVaultOutputTypeDef,
+    ListVaultsInputListVaultsPaginateTypeDef,
     ListVaultsInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PurchaseProvisionedCapacityInputRequestTypeDef,
+    PurchaseProvisionedCapacityOutputTypeDef,
     RemoveTagsFromVaultInputRequestTypeDef,
-    ServiceResourceAccountRequestTypeDef,
-    ServiceResourceArchiveRequestTypeDef,
-    ServiceResourceJobRequestTypeDef,
-    ServiceResourceMultipartUploadRequestTypeDef,
-    ServiceResourceNotificationRequestTypeDef,
-    ServiceResourceVaultRequestTypeDef,
+    ResponseMetadataTypeDef,
     UploadArchiveInputRequestTypeDef,
     UploadArchiveInputVaultUploadArchiveTypeDef,
     UploadMultipartPartInputMultipartUploadUploadPartTypeDef,
     UploadMultipartPartInputRequestTypeDef,
-    VaultArchiveRequestTypeDef,
-    VaultJobRequestTypeDef,
-    VaultMultipartUploadRequestTypeDef,
-    ArchiveCreationOutputTypeDef,
-    CreateVaultOutputTypeDef,
-    DescribeVaultOutputResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetJobOutputOutputTypeDef,
-    GetVaultLockOutputTypeDef,
-    InitiateJobOutputTypeDef,
-    InitiateMultipartUploadOutputTypeDef,
-    InitiateVaultLockOutputTypeDef,
-    InventoryRetrievalJobDescriptionResponseMetadataTypeDef,
-    ListTagsForVaultOutputTypeDef,
-    PurchaseProvisionedCapacityOutputTypeDef,
     UploadMultipartPartOutputTypeDef,
     InputSerializationTypeDef,
     OutputSerializationTypeDef,
     DataRetrievalPolicyTypeDef,
     DescribeVaultInputVaultExistsWaitTypeDef,
     DescribeVaultInputVaultNotExistsWaitTypeDef,
     ListVaultsOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
     SetVaultAccessPolicyInputRequestTypeDef,
     GetVaultNotificationsOutputTypeDef,
     SetVaultNotificationsInputNotificationSetTypeDef,
     SetVaultNotificationsInputRequestTypeDef,
     GrantTypeDef,
     InitiateVaultLockInputRequestTypeDef,
-    ListJobsInputListJobsPaginateTypeDef,
-    ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
-    ListPartsInputListPartsPaginateTypeDef,
-    ListVaultsInputListVaultsPaginateTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListPartsOutputTypeDef,
     ListProvisionedCapacityOutputTypeDef,
     SelectParametersResponseMetadataTypeDef,
     SelectParametersTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     SetDataRetrievalPolicyInputRequestTypeDef,
@@ -526,42 +516,42 @@
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

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/__init__.py` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/__init__.pyi` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/__main__.py` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Glacier 1.26.59\nVersion:         1.26.59\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Glacier 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.59")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/client.py` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.get_vault_access_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#get_vault_access_policy)
         """
 
     def get_vault_lock(self, *, vaultName: str, accountId: str = "-") -> GetVaultLockOutputTypeDef:
         """
         This operation retrieves the following attributes from the `lock-policy`
-        subresource set on the specified vault * The vault lock policy set on the vault.
+        subresource set on the specified vault: * The vault lock policy set on the
+        vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.get_vault_lock)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#get_vault_lock)
         """
 
     def get_vault_notifications(
         self, *, vaultName: str, accountId: str = "-"
@@ -343,15 +344,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#initiate_multipart_upload)
         """
 
     def initiate_vault_lock(
         self, *, vaultName: str, accountId: str = "-", policy: VaultLockPolicyTypeDef = ...
     ) -> InitiateVaultLockOutputTypeDef:
         """
-        This operation initiates the vault locking process by doing the following *
+        This operation initiates the vault locking process by doing the following: *
         Installing a vault lock policy on the specified vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.initiate_vault_lock)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#initiate_vault_lock)
         """
 
     def list_jobs(
```

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/client.pyi` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.get_vault_access_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#get_vault_access_policy)
         """
     def get_vault_lock(self, *, vaultName: str, accountId: str = "-") -> GetVaultLockOutputTypeDef:
         """
         This operation retrieves the following attributes from the `lock-policy`
-        subresource set on the specified vault * The vault lock policy set on the vault.
+        subresource set on the specified vault: * The vault lock policy set on the
+        vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.get_vault_lock)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#get_vault_lock)
         """
     def get_vault_notifications(
         self, *, vaultName: str, accountId: str = "-"
     ) -> GetVaultNotificationsOutputTypeDef:
@@ -316,15 +317,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.initiate_multipart_upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#initiate_multipart_upload)
         """
     def initiate_vault_lock(
         self, *, vaultName: str, accountId: str = "-", policy: VaultLockPolicyTypeDef = ...
     ) -> InitiateVaultLockOutputTypeDef:
         """
-        This operation initiates the vault locking process by doing the following *
+        This operation initiates the vault locking process by doing the following: *
         Installing a vault lock policy on the specified vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.initiate_vault_lock)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#initiate_vault_lock)
         """
     def list_jobs(
         self,
```

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/literals.py` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/literals.py`

 * *Files 2% similar despite different names*

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
@@ -120,21 +121,23 @@
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
@@ -213,14 +216,15 @@
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
@@ -231,14 +235,15 @@
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
@@ -274,14 +279,15 @@
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
@@ -300,16 +306,19 @@
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
@@ -389,18 +398,21 @@
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

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/literals.pyi` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/literals.pyi`

 * *Files 2% similar despite different names*

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
@@ -118,21 +119,23 @@
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
@@ -211,14 +214,15 @@
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
@@ -229,14 +233,15 @@
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
@@ -272,14 +277,15 @@
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
@@ -298,16 +304,19 @@
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
@@ -387,18 +396,21 @@
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

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/paginator.py` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,30 +64,30 @@
     def paginate(
         self,
         *,
         accountId: str,
         vaultName: str,
         statuscode: str = ...,
         completed: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listjobspaginator)
         """
 
 
 class ListMultipartUploadsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListMultipartUploads)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listmultipartuploadspaginator)
     """
 
     def paginate(
-        self, *, accountId: str, vaultName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, accountId: str, vaultName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMultipartUploadsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListMultipartUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listmultipartuploadspaginator)
         """
 
 
@@ -99,28 +99,28 @@
 
     def paginate(
         self,
         *,
         accountId: str,
         vaultName: str,
         uploadId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPartsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listpartspaginator)
         """
 
 
 class ListVaultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListVaults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listvaultspaginator)
     """
 
     def paginate(
-        self, *, accountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, accountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVaultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListVaults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listvaultspaginator)
         """
```

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/paginator.pyi` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,29 +61,29 @@
     def paginate(
         self,
         *,
         accountId: str,
         vaultName: str,
         statuscode: str = ...,
         completed: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listjobspaginator)
         """
 
 class ListMultipartUploadsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListMultipartUploads)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listmultipartuploadspaginator)
     """
 
     def paginate(
-        self, *, accountId: str, vaultName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, accountId: str, vaultName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMultipartUploadsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListMultipartUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listmultipartuploadspaginator)
         """
 
 class ListPartsPaginator(Paginator):
@@ -94,27 +94,27 @@
 
     def paginate(
         self,
         *,
         accountId: str,
         vaultName: str,
         uploadId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPartsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listpartspaginator)
         """
 
 class ListVaultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListVaults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listvaultspaginator)
     """
 
     def paginate(
-        self, *, accountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, accountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVaultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListVaults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/paginators/#listvaultspaginator)
         """
```

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/service_resource.py` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/service_resource.pyi` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/type_defs.py` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -33,109 +33,98 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AbortMultipartUploadInputRequestTypeDef",
     "AbortVaultLockInputRequestTypeDef",
-    "AccountVaultRequestTypeDef",
     "AddTagsToVaultInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "ArchiveCreationOutputTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
     "CompleteMultipartUploadInputMultipartUploadCompleteTypeDef",
     "CompleteMultipartUploadInputRequestTypeDef",
     "CompleteVaultLockInputRequestTypeDef",
     "CreateVaultInputAccountCreateVaultTypeDef",
     "CreateVaultInputRequestTypeDef",
     "CreateVaultInputServiceResourceCreateVaultTypeDef",
+    "CreateVaultOutputTypeDef",
     "DataRetrievalRuleTypeDef",
     "DeleteArchiveInputRequestTypeDef",
     "DeleteVaultAccessPolicyInputRequestTypeDef",
     "DeleteVaultInputRequestTypeDef",
     "DeleteVaultNotificationsInputRequestTypeDef",
     "DescribeJobInputRequestTypeDef",
     "DescribeVaultInputRequestTypeDef",
     "WaiterConfigTypeDef",
+    "DescribeVaultOutputResponseMetadataTypeDef",
     "DescribeVaultOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionTypeDef",
     "GetDataRetrievalPolicyInputRequestTypeDef",
     "GetJobOutputInputJobGetOutputTypeDef",
     "GetJobOutputInputRequestTypeDef",
+    "GetJobOutputOutputTypeDef",
     "GetVaultAccessPolicyInputRequestTypeDef",
     "VaultAccessPolicyTypeDef",
     "GetVaultLockInputRequestTypeDef",
+    "GetVaultLockOutputTypeDef",
     "GetVaultNotificationsInputRequestTypeDef",
     "VaultNotificationConfigTypeDef",
     "InventoryRetrievalJobDescriptionTypeDef",
     "GranteeTypeDef",
+    "InitiateJobOutputTypeDef",
     "InitiateMultipartUploadInputRequestTypeDef",
     "InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef",
+    "InitiateMultipartUploadOutputTypeDef",
     "VaultLockPolicyTypeDef",
+    "InitiateVaultLockOutputTypeDef",
+    "InventoryRetrievalJobDescriptionResponseMetadataTypeDef",
     "InventoryRetrievalJobInputTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListJobsInputListJobsPaginateTypeDef",
     "ListJobsInputRequestTypeDef",
+    "ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
     "ListMultipartUploadsInputRequestTypeDef",
     "UploadListElementTypeDef",
+    "ListPartsInputListPartsPaginateTypeDef",
     "ListPartsInputMultipartUploadPartsTypeDef",
     "ListPartsInputRequestTypeDef",
     "PartListElementTypeDef",
     "ListProvisionedCapacityInputRequestTypeDef",
     "ProvisionedCapacityDescriptionTypeDef",
     "ListTagsForVaultInputRequestTypeDef",
+    "ListTagsForVaultOutputTypeDef",
+    "ListVaultsInputListVaultsPaginateTypeDef",
     "ListVaultsInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PurchaseProvisionedCapacityInputRequestTypeDef",
+    "PurchaseProvisionedCapacityOutputTypeDef",
     "RemoveTagsFromVaultInputRequestTypeDef",
-    "ServiceResourceAccountRequestTypeDef",
-    "ServiceResourceArchiveRequestTypeDef",
-    "ServiceResourceJobRequestTypeDef",
-    "ServiceResourceMultipartUploadRequestTypeDef",
-    "ServiceResourceNotificationRequestTypeDef",
-    "ServiceResourceVaultRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UploadArchiveInputRequestTypeDef",
     "UploadArchiveInputVaultUploadArchiveTypeDef",
     "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
     "UploadMultipartPartInputRequestTypeDef",
-    "VaultArchiveRequestTypeDef",
-    "VaultJobRequestTypeDef",
-    "VaultMultipartUploadRequestTypeDef",
-    "ArchiveCreationOutputTypeDef",
-    "CreateVaultOutputTypeDef",
-    "DescribeVaultOutputResponseMetadataTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetJobOutputOutputTypeDef",
-    "GetVaultLockOutputTypeDef",
-    "InitiateJobOutputTypeDef",
-    "InitiateMultipartUploadOutputTypeDef",
-    "InitiateVaultLockOutputTypeDef",
-    "InventoryRetrievalJobDescriptionResponseMetadataTypeDef",
-    "ListTagsForVaultOutputTypeDef",
-    "PurchaseProvisionedCapacityOutputTypeDef",
     "UploadMultipartPartOutputTypeDef",
     "InputSerializationTypeDef",
     "OutputSerializationTypeDef",
     "DataRetrievalPolicyTypeDef",
     "DescribeVaultInputVaultExistsWaitTypeDef",
     "DescribeVaultInputVaultNotExistsWaitTypeDef",
     "ListVaultsOutputTypeDef",
     "GetVaultAccessPolicyOutputTypeDef",
     "SetVaultAccessPolicyInputRequestTypeDef",
     "GetVaultNotificationsOutputTypeDef",
     "SetVaultNotificationsInputNotificationSetTypeDef",
     "SetVaultNotificationsInputRequestTypeDef",
     "GrantTypeDef",
     "InitiateVaultLockInputRequestTypeDef",
-    "ListJobsInputListJobsPaginateTypeDef",
-    "ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
-    "ListPartsInputListPartsPaginateTypeDef",
-    "ListVaultsInputListVaultsPaginateTypeDef",
     "ListMultipartUploadsOutputTypeDef",
     "ListPartsOutputTypeDef",
     "ListProvisionedCapacityOutputTypeDef",
     "SelectParametersResponseMetadataTypeDef",
     "SelectParametersTypeDef",
     "GetDataRetrievalPolicyOutputTypeDef",
     "SetDataRetrievalPolicyInputRequestTypeDef",
@@ -160,50 +149,39 @@
     "_OptionalAbortMultipartUploadInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class AbortMultipartUploadInputRequestTypeDef(
     _RequiredAbortMultipartUploadInputRequestTypeDef,
     _OptionalAbortMultipartUploadInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredAbortVaultLockInputRequestTypeDef = TypedDict(
     "_RequiredAbortVaultLockInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalAbortVaultLockInputRequestTypeDef = TypedDict(
     "_OptionalAbortVaultLockInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class AbortVaultLockInputRequestTypeDef(
     _RequiredAbortVaultLockInputRequestTypeDef, _OptionalAbortVaultLockInputRequestTypeDef
 ):
     pass
 
-
-AccountVaultRequestTypeDef = TypedDict(
-    "AccountVaultRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-
 _RequiredAddTagsToVaultInputRequestTypeDef = TypedDict(
     "_RequiredAddTagsToVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalAddTagsToVaultInputRequestTypeDef = TypedDict(
@@ -211,29 +189,26 @@
     {
         "accountId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class AddTagsToVaultInputRequestTypeDef(
     _RequiredAddTagsToVaultInputRequestTypeDef, _OptionalAddTagsToVaultInputRequestTypeDef
 ):
     pass
 
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ArchiveCreationOutputTypeDef = TypedDict(
+    "ArchiveCreationOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "location": str,
+        "checksum": str,
+        "archiveId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CSVInputTypeDef = TypedDict(
     "CSVInputTypeDef",
     {
         "FileHeaderInfo": FileHeaderInfoType,
@@ -280,22 +255,20 @@
         "accountId": str,
         "archiveSize": str,
         "checksum": str,
     },
     total=False,
 )
 
-
 class CompleteMultipartUploadInputRequestTypeDef(
     _RequiredCompleteMultipartUploadInputRequestTypeDef,
     _OptionalCompleteMultipartUploadInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredCompleteVaultLockInputRequestTypeDef = TypedDict(
     "_RequiredCompleteVaultLockInputRequestTypeDef",
     {
         "vaultName": str,
         "lockId": str,
     },
 )
@@ -303,21 +276,19 @@
     "_OptionalCompleteVaultLockInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class CompleteVaultLockInputRequestTypeDef(
     _RequiredCompleteVaultLockInputRequestTypeDef, _OptionalCompleteVaultLockInputRequestTypeDef
 ):
     pass
 
-
 CreateVaultInputAccountCreateVaultTypeDef = TypedDict(
     "CreateVaultInputAccountCreateVaultTypeDef",
     {
         "vaultName": str,
     },
 )
 
@@ -331,42 +302,46 @@
     "_OptionalCreateVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class CreateVaultInputRequestTypeDef(
     _RequiredCreateVaultInputRequestTypeDef, _OptionalCreateVaultInputRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateVaultInputServiceResourceCreateVaultTypeDef = TypedDict(
     "_RequiredCreateVaultInputServiceResourceCreateVaultTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalCreateVaultInputServiceResourceCreateVaultTypeDef = TypedDict(
     "_OptionalCreateVaultInputServiceResourceCreateVaultTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class CreateVaultInputServiceResourceCreateVaultTypeDef(
     _RequiredCreateVaultInputServiceResourceCreateVaultTypeDef,
     _OptionalCreateVaultInputServiceResourceCreateVaultTypeDef,
 ):
     pass
 
+CreateVaultOutputTypeDef = TypedDict(
+    "CreateVaultOutputTypeDef",
+    {
+        "location": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 DataRetrievalRuleTypeDef = TypedDict(
     "DataRetrievalRuleTypeDef",
     {
         "Strategy": str,
         "BytesPerHour": int,
     },
@@ -384,86 +359,78 @@
     "_OptionalDeleteArchiveInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class DeleteArchiveInputRequestTypeDef(
     _RequiredDeleteArchiveInputRequestTypeDef, _OptionalDeleteArchiveInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVaultAccessPolicyInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDeleteVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_OptionalDeleteVaultAccessPolicyInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class DeleteVaultAccessPolicyInputRequestTypeDef(
     _RequiredDeleteVaultAccessPolicyInputRequestTypeDef,
     _OptionalDeleteVaultAccessPolicyInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteVaultInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDeleteVaultInputRequestTypeDef = TypedDict(
     "_OptionalDeleteVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class DeleteVaultInputRequestTypeDef(
     _RequiredDeleteVaultInputRequestTypeDef, _OptionalDeleteVaultInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteVaultNotificationsInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVaultNotificationsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDeleteVaultNotificationsInputRequestTypeDef = TypedDict(
     "_OptionalDeleteVaultNotificationsInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class DeleteVaultNotificationsInputRequestTypeDef(
     _RequiredDeleteVaultNotificationsInputRequestTypeDef,
     _OptionalDeleteVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeJobInputRequestTypeDef = TypedDict(
     "_RequiredDescribeJobInputRequestTypeDef",
     {
         "vaultName": str,
         "jobId": str,
     },
 )
@@ -471,64 +438,80 @@
     "_OptionalDescribeJobInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class DescribeJobInputRequestTypeDef(
     _RequiredDescribeJobInputRequestTypeDef, _OptionalDescribeJobInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeVaultInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDescribeVaultInputRequestTypeDef = TypedDict(
     "_OptionalDescribeVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class DescribeVaultInputRequestTypeDef(
     _RequiredDescribeVaultInputRequestTypeDef, _OptionalDescribeVaultInputRequestTypeDef
 ):
     pass
 
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
+DescribeVaultOutputResponseMetadataTypeDef = TypedDict(
+    "DescribeVaultOutputResponseMetadataTypeDef",
+    {
+        "VaultARN": str,
+        "VaultName": str,
+        "CreationDate": str,
+        "LastInventoryDate": str,
+        "NumberOfArchives": int,
+        "SizeInBytes": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeVaultOutputTypeDef = TypedDict(
     "DescribeVaultOutputTypeDef",
     {
         "VaultARN": str,
         "VaultName": str,
         "CreationDate": str,
         "LastInventoryDate": str,
         "NumberOfArchives": int,
         "SizeInBytes": int,
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
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "EncryptionType": EncryptionTypeType,
         "KMSKeyId": str,
         "KMSContext": str,
     },
@@ -563,20 +546,32 @@
     {
         "accountId": str,
         "range": str,
     },
     total=False,
 )
 
-
 class GetJobOutputInputRequestTypeDef(
     _RequiredGetJobOutputInputRequestTypeDef, _OptionalGetJobOutputInputRequestTypeDef
 ):
     pass
 
+GetJobOutputOutputTypeDef = TypedDict(
+    "GetJobOutputOutputTypeDef",
+    {
+        "body": StreamingBody,
+        "checksum": str,
+        "status": int,
+        "contentRange": str,
+        "acceptRanges": str,
+        "contentType": str,
+        "archiveDescription": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredGetVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredGetVaultAccessPolicyInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
@@ -584,22 +579,20 @@
     "_OptionalGetVaultAccessPolicyInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class GetVaultAccessPolicyInputRequestTypeDef(
     _RequiredGetVaultAccessPolicyInputRequestTypeDef,
     _OptionalGetVaultAccessPolicyInputRequestTypeDef,
 ):
     pass
 
-
 VaultAccessPolicyTypeDef = TypedDict(
     "VaultAccessPolicyTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
@@ -614,20 +607,29 @@
     "_OptionalGetVaultLockInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class GetVaultLockInputRequestTypeDef(
     _RequiredGetVaultLockInputRequestTypeDef, _OptionalGetVaultLockInputRequestTypeDef
 ):
     pass
 
+GetVaultLockOutputTypeDef = TypedDict(
+    "GetVaultLockOutputTypeDef",
+    {
+        "Policy": str,
+        "State": str,
+        "ExpirationDate": str,
+        "CreationDate": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredGetVaultNotificationsInputRequestTypeDef = TypedDict(
     "_RequiredGetVaultNotificationsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
@@ -635,22 +637,20 @@
     "_OptionalGetVaultNotificationsInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class GetVaultNotificationsInputRequestTypeDef(
     _RequiredGetVaultNotificationsInputRequestTypeDef,
     _OptionalGetVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
-
 VaultNotificationConfigTypeDef = TypedDict(
     "VaultNotificationConfigTypeDef",
     {
         "SNSTopic": str,
         "Events": List[str],
     },
     total=False,
@@ -681,18 +681,26 @@
         "URI": str,
         "ID": str,
         "EmailAddress": str,
     },
     total=False,
 )
 
-
 class GranteeTypeDef(_RequiredGranteeTypeDef, _OptionalGranteeTypeDef):
     pass
 
+InitiateJobOutputTypeDef = TypedDict(
+    "InitiateJobOutputTypeDef",
+    {
+        "location": str,
+        "jobId": str,
+        "jobOutputPath": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredInitiateMultipartUploadInputRequestTypeDef = TypedDict(
     "_RequiredInitiateMultipartUploadInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
@@ -702,60 +710,99 @@
         "accountId": str,
         "archiveDescription": str,
         "partSize": str,
     },
     total=False,
 )
 
-
 class InitiateMultipartUploadInputRequestTypeDef(
     _RequiredInitiateMultipartUploadInputRequestTypeDef,
     _OptionalInitiateMultipartUploadInputRequestTypeDef,
 ):
     pass
 
-
 InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef = TypedDict(
     "InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef",
     {
         "archiveDescription": str,
         "partSize": str,
     },
     total=False,
 )
 
+InitiateMultipartUploadOutputTypeDef = TypedDict(
+    "InitiateMultipartUploadOutputTypeDef",
+    {
+        "location": str,
+        "uploadId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VaultLockPolicyTypeDef = TypedDict(
     "VaultLockPolicyTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
 
+InitiateVaultLockOutputTypeDef = TypedDict(
+    "InitiateVaultLockOutputTypeDef",
+    {
+        "lockId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+InventoryRetrievalJobDescriptionResponseMetadataTypeDef = TypedDict(
+    "InventoryRetrievalJobDescriptionResponseMetadataTypeDef",
+    {
+        "Format": str,
+        "StartDate": str,
+        "EndDate": str,
+        "Limit": str,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InventoryRetrievalJobInputTypeDef = TypedDict(
     "InventoryRetrievalJobInputTypeDef",
     {
         "StartDate": str,
         "EndDate": str,
         "Limit": str,
         "Marker": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListJobsInputListJobsPaginateTypeDef = TypedDict(
+    "_RequiredListJobsInputListJobsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "accountId": str,
+        "vaultName": str,
+    },
+)
+_OptionalListJobsInputListJobsPaginateTypeDef = TypedDict(
+    "_OptionalListJobsInputListJobsPaginateTypeDef",
+    {
+        "statuscode": str,
+        "completed": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListJobsInputListJobsPaginateTypeDef(
+    _RequiredListJobsInputListJobsPaginateTypeDef, _OptionalListJobsInputListJobsPaginateTypeDef
+):
+    pass
+
 _RequiredListJobsInputRequestTypeDef = TypedDict(
     "_RequiredListJobsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalListJobsInputRequestTypeDef = TypedDict(
@@ -766,20 +813,39 @@
         "marker": str,
         "statuscode": str,
         "completed": str,
     },
     total=False,
 )
 
-
 class ListJobsInputRequestTypeDef(
     _RequiredListJobsInputRequestTypeDef, _OptionalListJobsInputRequestTypeDef
 ):
     pass
 
+_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
+    {
+        "accountId": str,
+        "vaultName": str,
+    },
+)
+_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef(
+    _RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
+    _OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
+):
+    pass
 
 _RequiredListMultipartUploadsInputRequestTypeDef = TypedDict(
     "_RequiredListMultipartUploadsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
@@ -789,34 +855,53 @@
         "accountId": str,
         "marker": str,
         "limit": str,
     },
     total=False,
 )
 
-
 class ListMultipartUploadsInputRequestTypeDef(
     _RequiredListMultipartUploadsInputRequestTypeDef,
     _OptionalListMultipartUploadsInputRequestTypeDef,
 ):
     pass
 
-
 UploadListElementTypeDef = TypedDict(
     "UploadListElementTypeDef",
     {
         "MultipartUploadId": str,
         "VaultARN": str,
         "ArchiveDescription": str,
         "PartSizeInBytes": int,
         "CreationDate": str,
     },
     total=False,
 )
 
+_RequiredListPartsInputListPartsPaginateTypeDef = TypedDict(
+    "_RequiredListPartsInputListPartsPaginateTypeDef",
+    {
+        "accountId": str,
+        "vaultName": str,
+        "uploadId": str,
+    },
+)
+_OptionalListPartsInputListPartsPaginateTypeDef = TypedDict(
+    "_OptionalListPartsInputListPartsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPartsInputListPartsPaginateTypeDef(
+    _RequiredListPartsInputListPartsPaginateTypeDef, _OptionalListPartsInputListPartsPaginateTypeDef
+):
+    pass
+
 ListPartsInputMultipartUploadPartsTypeDef = TypedDict(
     "ListPartsInputMultipartUploadPartsTypeDef",
     {
         "marker": str,
         "limit": str,
     },
     total=False,
@@ -835,21 +920,19 @@
         "accountId": str,
         "marker": str,
         "limit": str,
     },
     total=False,
 )
 
-
 class ListPartsInputRequestTypeDef(
     _RequiredListPartsInputRequestTypeDef, _OptionalListPartsInputRequestTypeDef
 ):
     pass
 
-
 PartListElementTypeDef = TypedDict(
     "PartListElementTypeDef",
     {
         "RangeInBytes": str,
         "SHA256TreeHash": str,
     },
     total=False,
@@ -883,39 +966,83 @@
     "_OptionalListTagsForVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class ListTagsForVaultInputRequestTypeDef(
     _RequiredListTagsForVaultInputRequestTypeDef, _OptionalListTagsForVaultInputRequestTypeDef
 ):
     pass
 
+ListTagsForVaultOutputTypeDef = TypedDict(
+    "ListTagsForVaultOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListVaultsInputListVaultsPaginateTypeDef = TypedDict(
+    "_RequiredListVaultsInputListVaultsPaginateTypeDef",
+    {
+        "accountId": str,
+    },
+)
+_OptionalListVaultsInputListVaultsPaginateTypeDef = TypedDict(
+    "_OptionalListVaultsInputListVaultsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListVaultsInputListVaultsPaginateTypeDef(
+    _RequiredListVaultsInputListVaultsPaginateTypeDef,
+    _OptionalListVaultsInputListVaultsPaginateTypeDef,
+):
+    pass
 
 ListVaultsInputRequestTypeDef = TypedDict(
     "ListVaultsInputRequestTypeDef",
     {
         "accountId": str,
         "marker": str,
         "limit": str,
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
 PurchaseProvisionedCapacityInputRequestTypeDef = TypedDict(
     "PurchaseProvisionedCapacityInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+PurchaseProvisionedCapacityOutputTypeDef = TypedDict(
+    "PurchaseProvisionedCapacityOutputTypeDef",
+    {
+        "capacityId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRemoveTagsFromVaultInputRequestTypeDef = TypedDict(
     "_RequiredRemoveTagsFromVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalRemoveTagsFromVaultInputRequestTypeDef = TypedDict(
@@ -923,68 +1050,27 @@
     {
         "accountId": str,
         "TagKeys": Sequence[str],
     },
     total=False,
 )
 
-
 class RemoveTagsFromVaultInputRequestTypeDef(
     _RequiredRemoveTagsFromVaultInputRequestTypeDef, _OptionalRemoveTagsFromVaultInputRequestTypeDef
 ):
     pass
 
-
-ServiceResourceAccountRequestTypeDef = TypedDict(
-    "ServiceResourceAccountRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-
-ServiceResourceArchiveRequestTypeDef = TypedDict(
-    "ServiceResourceArchiveRequestTypeDef",
-    {
-        "account_id": str,
-        "vault_name": str,
-        "id": str,
-    },
-)
-
-ServiceResourceJobRequestTypeDef = TypedDict(
-    "ServiceResourceJobRequestTypeDef",
-    {
-        "account_id": str,
-        "vault_name": str,
-        "id": str,
-    },
-)
-
-ServiceResourceMultipartUploadRequestTypeDef = TypedDict(
-    "ServiceResourceMultipartUploadRequestTypeDef",
-    {
-        "account_id": str,
-        "vault_name": str,
-        "id": str,
-    },
-)
-
-ServiceResourceNotificationRequestTypeDef = TypedDict(
-    "ServiceResourceNotificationRequestTypeDef",
-    {
-        "account_id": str,
-        "vault_name": str,
-    },
-)
-
-ServiceResourceVaultRequestTypeDef = TypedDict(
-    "ServiceResourceVaultRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "account_id": str,
-        "name": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredUploadArchiveInputRequestTypeDef = TypedDict(
     "_RequiredUploadArchiveInputRequestTypeDef",
     {
         "vaultName": str,
@@ -997,21 +1083,19 @@
         "archiveDescription": str,
         "checksum": str,
         "body": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-
 class UploadArchiveInputRequestTypeDef(
     _RequiredUploadArchiveInputRequestTypeDef, _OptionalUploadArchiveInputRequestTypeDef
 ):
     pass
 
-
 UploadArchiveInputVaultUploadArchiveTypeDef = TypedDict(
     "UploadArchiveInputVaultUploadArchiveTypeDef",
     {
         "archiveDescription": str,
         "checksum": str,
         "body": Union[str, bytes, IO[Any], StreamingBody],
     },
@@ -1042,165 +1126,24 @@
         "checksum": str,
         "range": str,
         "body": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-
 class UploadMultipartPartInputRequestTypeDef(
     _RequiredUploadMultipartPartInputRequestTypeDef, _OptionalUploadMultipartPartInputRequestTypeDef
 ):
     pass
 
-
-VaultArchiveRequestTypeDef = TypedDict(
-    "VaultArchiveRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-
-VaultJobRequestTypeDef = TypedDict(
-    "VaultJobRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-
-VaultMultipartUploadRequestTypeDef = TypedDict(
-    "VaultMultipartUploadRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-
-ArchiveCreationOutputTypeDef = TypedDict(
-    "ArchiveCreationOutputTypeDef",
-    {
-        "location": str,
-        "checksum": str,
-        "archiveId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateVaultOutputTypeDef = TypedDict(
-    "CreateVaultOutputTypeDef",
-    {
-        "location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeVaultOutputResponseMetadataTypeDef = TypedDict(
-    "DescribeVaultOutputResponseMetadataTypeDef",
-    {
-        "VaultARN": str,
-        "VaultName": str,
-        "CreationDate": str,
-        "LastInventoryDate": str,
-        "NumberOfArchives": int,
-        "SizeInBytes": int,
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
-GetJobOutputOutputTypeDef = TypedDict(
-    "GetJobOutputOutputTypeDef",
-    {
-        "body": StreamingBody,
-        "checksum": str,
-        "status": int,
-        "contentRange": str,
-        "acceptRanges": str,
-        "contentType": str,
-        "archiveDescription": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetVaultLockOutputTypeDef = TypedDict(
-    "GetVaultLockOutputTypeDef",
-    {
-        "Policy": str,
-        "State": str,
-        "ExpirationDate": str,
-        "CreationDate": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InitiateJobOutputTypeDef = TypedDict(
-    "InitiateJobOutputTypeDef",
-    {
-        "location": str,
-        "jobId": str,
-        "jobOutputPath": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InitiateMultipartUploadOutputTypeDef = TypedDict(
-    "InitiateMultipartUploadOutputTypeDef",
-    {
-        "location": str,
-        "uploadId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InitiateVaultLockOutputTypeDef = TypedDict(
-    "InitiateVaultLockOutputTypeDef",
-    {
-        "lockId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InventoryRetrievalJobDescriptionResponseMetadataTypeDef = TypedDict(
-    "InventoryRetrievalJobDescriptionResponseMetadataTypeDef",
-    {
-        "Format": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Limit": str,
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForVaultOutputTypeDef = TypedDict(
-    "ListTagsForVaultOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PurchaseProvisionedCapacityOutputTypeDef = TypedDict(
-    "PurchaseProvisionedCapacityOutputTypeDef",
-    {
-        "capacityId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UploadMultipartPartOutputTypeDef = TypedDict(
     "UploadMultipartPartOutputTypeDef",
     {
         "checksum": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputSerializationTypeDef = TypedDict(
     "InputSerializationTypeDef",
     {
         "csv": CSVInputTypeDef,
@@ -1235,22 +1178,20 @@
     "_OptionalDescribeVaultInputVaultExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeVaultInputVaultExistsWaitTypeDef(
     _RequiredDescribeVaultInputVaultExistsWaitTypeDef,
     _OptionalDescribeVaultInputVaultExistsWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeVaultInputVaultNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeVaultInputVaultNotExistsWaitTypeDef",
     {
         "accountId": str,
         "vaultName": str,
     },
 )
@@ -1258,36 +1199,34 @@
     "_OptionalDescribeVaultInputVaultNotExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeVaultInputVaultNotExistsWaitTypeDef(
     _RequiredDescribeVaultInputVaultNotExistsWaitTypeDef,
     _OptionalDescribeVaultInputVaultNotExistsWaitTypeDef,
 ):
     pass
 
-
 ListVaultsOutputTypeDef = TypedDict(
     "ListVaultsOutputTypeDef",
     {
         "VaultList": List[DescribeVaultOutputTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVaultAccessPolicyOutputTypeDef = TypedDict(
     "GetVaultAccessPolicyOutputTypeDef",
     {
         "policy": VaultAccessPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredSetVaultAccessPolicyInputRequestTypeDef",
     {
         "vaultName": str,
@@ -1298,27 +1237,25 @@
     {
         "accountId": str,
         "policy": VaultAccessPolicyTypeDef,
     },
     total=False,
 )
 
-
 class SetVaultAccessPolicyInputRequestTypeDef(
     _RequiredSetVaultAccessPolicyInputRequestTypeDef,
     _OptionalSetVaultAccessPolicyInputRequestTypeDef,
 ):
     pass
 
-
 GetVaultNotificationsOutputTypeDef = TypedDict(
     "GetVaultNotificationsOutputTypeDef",
     {
         "vaultNotificationConfig": VaultNotificationConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetVaultNotificationsInputNotificationSetTypeDef = TypedDict(
     "SetVaultNotificationsInputNotificationSetTypeDef",
     {
         "vaultNotificationConfig": VaultNotificationConfigTypeDef,
@@ -1337,22 +1274,20 @@
     {
         "accountId": str,
         "vaultNotificationConfig": VaultNotificationConfigTypeDef,
     },
     total=False,
 )
 
-
 class SetVaultNotificationsInputRequestTypeDef(
     _RequiredSetVaultNotificationsInputRequestTypeDef,
     _OptionalSetVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
-
 GrantTypeDef = TypedDict(
     "GrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": PermissionType,
     },
     total=False,
@@ -1369,152 +1304,58 @@
     {
         "accountId": str,
         "policy": VaultLockPolicyTypeDef,
     },
     total=False,
 )
 
-
 class InitiateVaultLockInputRequestTypeDef(
     _RequiredInitiateVaultLockInputRequestTypeDef, _OptionalInitiateVaultLockInputRequestTypeDef
 ):
     pass
 
-
-_RequiredListJobsInputListJobsPaginateTypeDef = TypedDict(
-    "_RequiredListJobsInputListJobsPaginateTypeDef",
-    {
-        "accountId": str,
-        "vaultName": str,
-    },
-)
-_OptionalListJobsInputListJobsPaginateTypeDef = TypedDict(
-    "_OptionalListJobsInputListJobsPaginateTypeDef",
-    {
-        "statuscode": str,
-        "completed": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListJobsInputListJobsPaginateTypeDef(
-    _RequiredListJobsInputListJobsPaginateTypeDef, _OptionalListJobsInputListJobsPaginateTypeDef
-):
-    pass
-
-
-_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
-    {
-        "accountId": str,
-        "vaultName": str,
-    },
-)
-_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef(
-    _RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
-    _OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListPartsInputListPartsPaginateTypeDef = TypedDict(
-    "_RequiredListPartsInputListPartsPaginateTypeDef",
-    {
-        "accountId": str,
-        "vaultName": str,
-        "uploadId": str,
-    },
-)
-_OptionalListPartsInputListPartsPaginateTypeDef = TypedDict(
-    "_OptionalListPartsInputListPartsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPartsInputListPartsPaginateTypeDef(
-    _RequiredListPartsInputListPartsPaginateTypeDef, _OptionalListPartsInputListPartsPaginateTypeDef
-):
-    pass
-
-
-_RequiredListVaultsInputListVaultsPaginateTypeDef = TypedDict(
-    "_RequiredListVaultsInputListVaultsPaginateTypeDef",
-    {
-        "accountId": str,
-    },
-)
-_OptionalListVaultsInputListVaultsPaginateTypeDef = TypedDict(
-    "_OptionalListVaultsInputListVaultsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListVaultsInputListVaultsPaginateTypeDef(
-    _RequiredListVaultsInputListVaultsPaginateTypeDef,
-    _OptionalListVaultsInputListVaultsPaginateTypeDef,
-):
-    pass
-
-
 ListMultipartUploadsOutputTypeDef = TypedDict(
     "ListMultipartUploadsOutputTypeDef",
     {
         "UploadsList": List[UploadListElementTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPartsOutputTypeDef = TypedDict(
     "ListPartsOutputTypeDef",
     {
         "MultipartUploadId": str,
         "VaultARN": str,
         "ArchiveDescription": str,
         "PartSizeInBytes": int,
         "CreationDate": str,
         "Parts": List[PartListElementTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProvisionedCapacityOutputTypeDef = TypedDict(
     "ListProvisionedCapacityOutputTypeDef",
     {
         "ProvisionedCapacityList": List[ProvisionedCapacityDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SelectParametersResponseMetadataTypeDef = TypedDict(
     "SelectParametersResponseMetadataTypeDef",
     {
         "InputSerialization": InputSerializationTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
         "OutputSerialization": OutputSerializationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SelectParametersTypeDef = TypedDict(
     "SelectParametersTypeDef",
     {
         "InputSerialization": InputSerializationTypeDef,
@@ -1525,15 +1366,15 @@
     total=False,
 )
 
 GetDataRetrievalPolicyOutputTypeDef = TypedDict(
     "GetDataRetrievalPolicyOutputTypeDef",
     {
         "Policy": DataRetrievalPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetDataRetrievalPolicyInputRequestTypeDef = TypedDict(
     "SetDataRetrievalPolicyInputRequestTypeDef",
     {
         "accountId": str,
@@ -1557,15 +1398,15 @@
     total=False,
 )
 
 OutputLocationResponseMetadataTypeDef = TypedDict(
     "OutputLocationResponseMetadataTypeDef",
     {
         "S3": S3LocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OutputLocationTypeDef = TypedDict(
     "OutputLocationTypeDef",
     {
         "S3": S3LocationTypeDef,
@@ -1593,15 +1434,15 @@
         "ArchiveSHA256TreeHash": str,
         "RetrievalByteRange": str,
         "Tier": str,
         "InventoryRetrievalParameters": InventoryRetrievalJobDescriptionTypeDef,
         "JobOutputPath": str,
         "SelectParameters": SelectParametersTypeDef,
         "OutputLocation": OutputLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GlacierJobDescriptionTypeDef = TypedDict(
     "GlacierJobDescriptionTypeDef",
     {
         "JobId": str,
@@ -1647,15 +1488,15 @@
 )
 
 ListJobsOutputTypeDef = TypedDict(
     "ListJobsOutputTypeDef",
     {
         "JobList": List[GlacierJobDescriptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredInitiateJobInputRequestTypeDef = TypedDict(
     "_RequiredInitiateJobInputRequestTypeDef",
     {
         "vaultName": str,
@@ -1666,12 +1507,11 @@
     {
         "accountId": str,
         "jobParameters": JobParametersTypeDef,
     },
     total=False,
 )
 
-
 class InitiateJobInputRequestTypeDef(
     _RequiredInitiateJobInputRequestTypeDef, _OptionalInitiateJobInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/type_defs.pyi` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,108 +33,99 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AbortMultipartUploadInputRequestTypeDef",
     "AbortVaultLockInputRequestTypeDef",
-    "AccountVaultRequestTypeDef",
     "AddTagsToVaultInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "ArchiveCreationOutputTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
     "CompleteMultipartUploadInputMultipartUploadCompleteTypeDef",
     "CompleteMultipartUploadInputRequestTypeDef",
     "CompleteVaultLockInputRequestTypeDef",
     "CreateVaultInputAccountCreateVaultTypeDef",
     "CreateVaultInputRequestTypeDef",
     "CreateVaultInputServiceResourceCreateVaultTypeDef",
+    "CreateVaultOutputTypeDef",
     "DataRetrievalRuleTypeDef",
     "DeleteArchiveInputRequestTypeDef",
     "DeleteVaultAccessPolicyInputRequestTypeDef",
     "DeleteVaultInputRequestTypeDef",
     "DeleteVaultNotificationsInputRequestTypeDef",
     "DescribeJobInputRequestTypeDef",
     "DescribeVaultInputRequestTypeDef",
     "WaiterConfigTypeDef",
+    "DescribeVaultOutputResponseMetadataTypeDef",
     "DescribeVaultOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionTypeDef",
     "GetDataRetrievalPolicyInputRequestTypeDef",
     "GetJobOutputInputJobGetOutputTypeDef",
     "GetJobOutputInputRequestTypeDef",
+    "GetJobOutputOutputTypeDef",
     "GetVaultAccessPolicyInputRequestTypeDef",
     "VaultAccessPolicyTypeDef",
     "GetVaultLockInputRequestTypeDef",
+    "GetVaultLockOutputTypeDef",
     "GetVaultNotificationsInputRequestTypeDef",
     "VaultNotificationConfigTypeDef",
     "InventoryRetrievalJobDescriptionTypeDef",
     "GranteeTypeDef",
+    "InitiateJobOutputTypeDef",
     "InitiateMultipartUploadInputRequestTypeDef",
     "InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef",
+    "InitiateMultipartUploadOutputTypeDef",
     "VaultLockPolicyTypeDef",
+    "InitiateVaultLockOutputTypeDef",
+    "InventoryRetrievalJobDescriptionResponseMetadataTypeDef",
     "InventoryRetrievalJobInputTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListJobsInputListJobsPaginateTypeDef",
     "ListJobsInputRequestTypeDef",
+    "ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
     "ListMultipartUploadsInputRequestTypeDef",
     "UploadListElementTypeDef",
+    "ListPartsInputListPartsPaginateTypeDef",
     "ListPartsInputMultipartUploadPartsTypeDef",
     "ListPartsInputRequestTypeDef",
     "PartListElementTypeDef",
     "ListProvisionedCapacityInputRequestTypeDef",
     "ProvisionedCapacityDescriptionTypeDef",
     "ListTagsForVaultInputRequestTypeDef",
+    "ListTagsForVaultOutputTypeDef",
+    "ListVaultsInputListVaultsPaginateTypeDef",
     "ListVaultsInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PurchaseProvisionedCapacityInputRequestTypeDef",
+    "PurchaseProvisionedCapacityOutputTypeDef",
     "RemoveTagsFromVaultInputRequestTypeDef",
-    "ServiceResourceAccountRequestTypeDef",
-    "ServiceResourceArchiveRequestTypeDef",
-    "ServiceResourceJobRequestTypeDef",
-    "ServiceResourceMultipartUploadRequestTypeDef",
-    "ServiceResourceNotificationRequestTypeDef",
-    "ServiceResourceVaultRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UploadArchiveInputRequestTypeDef",
     "UploadArchiveInputVaultUploadArchiveTypeDef",
     "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
     "UploadMultipartPartInputRequestTypeDef",
-    "VaultArchiveRequestTypeDef",
-    "VaultJobRequestTypeDef",
-    "VaultMultipartUploadRequestTypeDef",
-    "ArchiveCreationOutputTypeDef",
-    "CreateVaultOutputTypeDef",
-    "DescribeVaultOutputResponseMetadataTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetJobOutputOutputTypeDef",
-    "GetVaultLockOutputTypeDef",
-    "InitiateJobOutputTypeDef",
-    "InitiateMultipartUploadOutputTypeDef",
-    "InitiateVaultLockOutputTypeDef",
-    "InventoryRetrievalJobDescriptionResponseMetadataTypeDef",
-    "ListTagsForVaultOutputTypeDef",
-    "PurchaseProvisionedCapacityOutputTypeDef",
     "UploadMultipartPartOutputTypeDef",
     "InputSerializationTypeDef",
     "OutputSerializationTypeDef",
     "DataRetrievalPolicyTypeDef",
     "DescribeVaultInputVaultExistsWaitTypeDef",
     "DescribeVaultInputVaultNotExistsWaitTypeDef",
     "ListVaultsOutputTypeDef",
     "GetVaultAccessPolicyOutputTypeDef",
     "SetVaultAccessPolicyInputRequestTypeDef",
     "GetVaultNotificationsOutputTypeDef",
     "SetVaultNotificationsInputNotificationSetTypeDef",
     "SetVaultNotificationsInputRequestTypeDef",
     "GrantTypeDef",
     "InitiateVaultLockInputRequestTypeDef",
-    "ListJobsInputListJobsPaginateTypeDef",
-    "ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
-    "ListPartsInputListPartsPaginateTypeDef",
-    "ListVaultsInputListVaultsPaginateTypeDef",
     "ListMultipartUploadsOutputTypeDef",
     "ListPartsOutputTypeDef",
     "ListProvisionedCapacityOutputTypeDef",
     "SelectParametersResponseMetadataTypeDef",
     "SelectParametersTypeDef",
     "GetDataRetrievalPolicyOutputTypeDef",
     "SetDataRetrievalPolicyInputRequestTypeDef",
@@ -159,45 +150,42 @@
     "_OptionalAbortMultipartUploadInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class AbortMultipartUploadInputRequestTypeDef(
     _RequiredAbortMultipartUploadInputRequestTypeDef,
     _OptionalAbortMultipartUploadInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredAbortVaultLockInputRequestTypeDef = TypedDict(
     "_RequiredAbortVaultLockInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalAbortVaultLockInputRequestTypeDef = TypedDict(
     "_OptionalAbortVaultLockInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class AbortVaultLockInputRequestTypeDef(
     _RequiredAbortVaultLockInputRequestTypeDef, _OptionalAbortVaultLockInputRequestTypeDef
 ):
     pass
 
-AccountVaultRequestTypeDef = TypedDict(
-    "AccountVaultRequestTypeDef",
-    {
-        "name": str,
-    },
-)
 
 _RequiredAddTagsToVaultInputRequestTypeDef = TypedDict(
     "_RequiredAddTagsToVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
@@ -206,27 +194,28 @@
     {
         "accountId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class AddTagsToVaultInputRequestTypeDef(
     _RequiredAddTagsToVaultInputRequestTypeDef, _OptionalAddTagsToVaultInputRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+ArchiveCreationOutputTypeDef = TypedDict(
+    "ArchiveCreationOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "location": str,
+        "checksum": str,
+        "archiveId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CSVInputTypeDef = TypedDict(
     "CSVInputTypeDef",
     {
         "FileHeaderInfo": FileHeaderInfoType,
@@ -273,20 +262,22 @@
         "accountId": str,
         "archiveSize": str,
         "checksum": str,
     },
     total=False,
 )
 
+
 class CompleteMultipartUploadInputRequestTypeDef(
     _RequiredCompleteMultipartUploadInputRequestTypeDef,
     _OptionalCompleteMultipartUploadInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredCompleteVaultLockInputRequestTypeDef = TypedDict(
     "_RequiredCompleteVaultLockInputRequestTypeDef",
     {
         "vaultName": str,
         "lockId": str,
     },
 )
@@ -294,19 +285,21 @@
     "_OptionalCompleteVaultLockInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class CompleteVaultLockInputRequestTypeDef(
     _RequiredCompleteVaultLockInputRequestTypeDef, _OptionalCompleteVaultLockInputRequestTypeDef
 ):
     pass
 
+
 CreateVaultInputAccountCreateVaultTypeDef = TypedDict(
     "CreateVaultInputAccountCreateVaultTypeDef",
     {
         "vaultName": str,
     },
 )
 
@@ -320,39 +313,51 @@
     "_OptionalCreateVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class CreateVaultInputRequestTypeDef(
     _RequiredCreateVaultInputRequestTypeDef, _OptionalCreateVaultInputRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateVaultInputServiceResourceCreateVaultTypeDef = TypedDict(
     "_RequiredCreateVaultInputServiceResourceCreateVaultTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalCreateVaultInputServiceResourceCreateVaultTypeDef = TypedDict(
     "_OptionalCreateVaultInputServiceResourceCreateVaultTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class CreateVaultInputServiceResourceCreateVaultTypeDef(
     _RequiredCreateVaultInputServiceResourceCreateVaultTypeDef,
     _OptionalCreateVaultInputServiceResourceCreateVaultTypeDef,
 ):
     pass
 
+
+CreateVaultOutputTypeDef = TypedDict(
+    "CreateVaultOutputTypeDef",
+    {
+        "location": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataRetrievalRuleTypeDef = TypedDict(
     "DataRetrievalRuleTypeDef",
     {
         "Strategy": str,
         "BytesPerHour": int,
     },
     total=False,
@@ -369,78 +374,86 @@
     "_OptionalDeleteArchiveInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class DeleteArchiveInputRequestTypeDef(
     _RequiredDeleteArchiveInputRequestTypeDef, _OptionalDeleteArchiveInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVaultAccessPolicyInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDeleteVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_OptionalDeleteVaultAccessPolicyInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class DeleteVaultAccessPolicyInputRequestTypeDef(
     _RequiredDeleteVaultAccessPolicyInputRequestTypeDef,
     _OptionalDeleteVaultAccessPolicyInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteVaultInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDeleteVaultInputRequestTypeDef = TypedDict(
     "_OptionalDeleteVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class DeleteVaultInputRequestTypeDef(
     _RequiredDeleteVaultInputRequestTypeDef, _OptionalDeleteVaultInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteVaultNotificationsInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVaultNotificationsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDeleteVaultNotificationsInputRequestTypeDef = TypedDict(
     "_OptionalDeleteVaultNotificationsInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class DeleteVaultNotificationsInputRequestTypeDef(
     _RequiredDeleteVaultNotificationsInputRequestTypeDef,
     _OptionalDeleteVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeJobInputRequestTypeDef = TypedDict(
     "_RequiredDescribeJobInputRequestTypeDef",
     {
         "vaultName": str,
         "jobId": str,
     },
 )
@@ -448,60 +461,84 @@
     "_OptionalDescribeJobInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class DescribeJobInputRequestTypeDef(
     _RequiredDescribeJobInputRequestTypeDef, _OptionalDescribeJobInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeVaultInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDescribeVaultInputRequestTypeDef = TypedDict(
     "_OptionalDescribeVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class DescribeVaultInputRequestTypeDef(
     _RequiredDescribeVaultInputRequestTypeDef, _OptionalDescribeVaultInputRequestTypeDef
 ):
     pass
 
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
+DescribeVaultOutputResponseMetadataTypeDef = TypedDict(
+    "DescribeVaultOutputResponseMetadataTypeDef",
+    {
+        "VaultARN": str,
+        "VaultName": str,
+        "CreationDate": str,
+        "LastInventoryDate": str,
+        "NumberOfArchives": int,
+        "SizeInBytes": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeVaultOutputTypeDef = TypedDict(
     "DescribeVaultOutputTypeDef",
     {
         "VaultARN": str,
         "VaultName": str,
         "CreationDate": str,
         "LastInventoryDate": str,
         "NumberOfArchives": int,
         "SizeInBytes": int,
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
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "EncryptionType": EncryptionTypeType,
         "KMSKeyId": str,
         "KMSContext": str,
     },
@@ -536,39 +573,57 @@
     {
         "accountId": str,
         "range": str,
     },
     total=False,
 )
 
+
 class GetJobOutputInputRequestTypeDef(
     _RequiredGetJobOutputInputRequestTypeDef, _OptionalGetJobOutputInputRequestTypeDef
 ):
     pass
 
+
+GetJobOutputOutputTypeDef = TypedDict(
+    "GetJobOutputOutputTypeDef",
+    {
+        "body": StreamingBody,
+        "checksum": str,
+        "status": int,
+        "contentRange": str,
+        "acceptRanges": str,
+        "contentType": str,
+        "archiveDescription": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredGetVaultAccessPolicyInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalGetVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_OptionalGetVaultAccessPolicyInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class GetVaultAccessPolicyInputRequestTypeDef(
     _RequiredGetVaultAccessPolicyInputRequestTypeDef,
     _OptionalGetVaultAccessPolicyInputRequestTypeDef,
 ):
     pass
 
+
 VaultAccessPolicyTypeDef = TypedDict(
     "VaultAccessPolicyTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
@@ -583,39 +638,54 @@
     "_OptionalGetVaultLockInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class GetVaultLockInputRequestTypeDef(
     _RequiredGetVaultLockInputRequestTypeDef, _OptionalGetVaultLockInputRequestTypeDef
 ):
     pass
 
+
+GetVaultLockOutputTypeDef = TypedDict(
+    "GetVaultLockOutputTypeDef",
+    {
+        "Policy": str,
+        "State": str,
+        "ExpirationDate": str,
+        "CreationDate": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetVaultNotificationsInputRequestTypeDef = TypedDict(
     "_RequiredGetVaultNotificationsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalGetVaultNotificationsInputRequestTypeDef = TypedDict(
     "_OptionalGetVaultNotificationsInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class GetVaultNotificationsInputRequestTypeDef(
     _RequiredGetVaultNotificationsInputRequestTypeDef,
     _OptionalGetVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
+
 VaultNotificationConfigTypeDef = TypedDict(
     "VaultNotificationConfigTypeDef",
     {
         "SNSTopic": str,
         "Events": List[str],
     },
     total=False,
@@ -646,17 +716,29 @@
         "URI": str,
         "ID": str,
         "EmailAddress": str,
     },
     total=False,
 )
 
+
 class GranteeTypeDef(_RequiredGranteeTypeDef, _OptionalGranteeTypeDef):
     pass
 
+
+InitiateJobOutputTypeDef = TypedDict(
+    "InitiateJobOutputTypeDef",
+    {
+        "location": str,
+        "jobId": str,
+        "jobOutputPath": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredInitiateMultipartUploadInputRequestTypeDef = TypedDict(
     "_RequiredInitiateMultipartUploadInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalInitiateMultipartUploadInputRequestTypeDef = TypedDict(
@@ -665,58 +747,103 @@
         "accountId": str,
         "archiveDescription": str,
         "partSize": str,
     },
     total=False,
 )
 
+
 class InitiateMultipartUploadInputRequestTypeDef(
     _RequiredInitiateMultipartUploadInputRequestTypeDef,
     _OptionalInitiateMultipartUploadInputRequestTypeDef,
 ):
     pass
 
+
 InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef = TypedDict(
     "InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef",
     {
         "archiveDescription": str,
         "partSize": str,
     },
     total=False,
 )
 
+InitiateMultipartUploadOutputTypeDef = TypedDict(
+    "InitiateMultipartUploadOutputTypeDef",
+    {
+        "location": str,
+        "uploadId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 VaultLockPolicyTypeDef = TypedDict(
     "VaultLockPolicyTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
 
+InitiateVaultLockOutputTypeDef = TypedDict(
+    "InitiateVaultLockOutputTypeDef",
+    {
+        "lockId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+InventoryRetrievalJobDescriptionResponseMetadataTypeDef = TypedDict(
+    "InventoryRetrievalJobDescriptionResponseMetadataTypeDef",
+    {
+        "Format": str,
+        "StartDate": str,
+        "EndDate": str,
+        "Limit": str,
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InventoryRetrievalJobInputTypeDef = TypedDict(
     "InventoryRetrievalJobInputTypeDef",
     {
         "StartDate": str,
         "EndDate": str,
         "Limit": str,
         "Marker": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListJobsInputListJobsPaginateTypeDef = TypedDict(
+    "_RequiredListJobsInputListJobsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "accountId": str,
+        "vaultName": str,
+    },
+)
+_OptionalListJobsInputListJobsPaginateTypeDef = TypedDict(
+    "_OptionalListJobsInputListJobsPaginateTypeDef",
+    {
+        "statuscode": str,
+        "completed": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListJobsInputListJobsPaginateTypeDef(
+    _RequiredListJobsInputListJobsPaginateTypeDef, _OptionalListJobsInputListJobsPaginateTypeDef
+):
+    pass
+
+
 _RequiredListJobsInputRequestTypeDef = TypedDict(
     "_RequiredListJobsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalListJobsInputRequestTypeDef = TypedDict(
@@ -727,19 +854,44 @@
         "marker": str,
         "statuscode": str,
         "completed": str,
     },
     total=False,
 )
 
+
 class ListJobsInputRequestTypeDef(
     _RequiredListJobsInputRequestTypeDef, _OptionalListJobsInputRequestTypeDef
 ):
     pass
 
+
+_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
+    {
+        "accountId": str,
+        "vaultName": str,
+    },
+)
+_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef(
+    _RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
+    _OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListMultipartUploadsInputRequestTypeDef = TypedDict(
     "_RequiredListMultipartUploadsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalListMultipartUploadsInputRequestTypeDef = TypedDict(
@@ -748,32 +900,57 @@
         "accountId": str,
         "marker": str,
         "limit": str,
     },
     total=False,
 )
 
+
 class ListMultipartUploadsInputRequestTypeDef(
     _RequiredListMultipartUploadsInputRequestTypeDef,
     _OptionalListMultipartUploadsInputRequestTypeDef,
 ):
     pass
 
+
 UploadListElementTypeDef = TypedDict(
     "UploadListElementTypeDef",
     {
         "MultipartUploadId": str,
         "VaultARN": str,
         "ArchiveDescription": str,
         "PartSizeInBytes": int,
         "CreationDate": str,
     },
     total=False,
 )
 
+_RequiredListPartsInputListPartsPaginateTypeDef = TypedDict(
+    "_RequiredListPartsInputListPartsPaginateTypeDef",
+    {
+        "accountId": str,
+        "vaultName": str,
+        "uploadId": str,
+    },
+)
+_OptionalListPartsInputListPartsPaginateTypeDef = TypedDict(
+    "_OptionalListPartsInputListPartsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPartsInputListPartsPaginateTypeDef(
+    _RequiredListPartsInputListPartsPaginateTypeDef, _OptionalListPartsInputListPartsPaginateTypeDef
+):
+    pass
+
+
 ListPartsInputMultipartUploadPartsTypeDef = TypedDict(
     "ListPartsInputMultipartUploadPartsTypeDef",
     {
         "marker": str,
         "limit": str,
     },
     total=False,
@@ -792,19 +969,21 @@
         "accountId": str,
         "marker": str,
         "limit": str,
     },
     total=False,
 )
 
+
 class ListPartsInputRequestTypeDef(
     _RequiredListPartsInputRequestTypeDef, _OptionalListPartsInputRequestTypeDef
 ):
     pass
 
+
 PartListElementTypeDef = TypedDict(
     "PartListElementTypeDef",
     {
         "RangeInBytes": str,
         "SHA256TreeHash": str,
     },
     total=False,
@@ -838,37 +1017,87 @@
     "_OptionalListTagsForVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class ListTagsForVaultInputRequestTypeDef(
     _RequiredListTagsForVaultInputRequestTypeDef, _OptionalListTagsForVaultInputRequestTypeDef
 ):
     pass
 
+
+ListTagsForVaultOutputTypeDef = TypedDict(
+    "ListTagsForVaultOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListVaultsInputListVaultsPaginateTypeDef = TypedDict(
+    "_RequiredListVaultsInputListVaultsPaginateTypeDef",
+    {
+        "accountId": str,
+    },
+)
+_OptionalListVaultsInputListVaultsPaginateTypeDef = TypedDict(
+    "_OptionalListVaultsInputListVaultsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListVaultsInputListVaultsPaginateTypeDef(
+    _RequiredListVaultsInputListVaultsPaginateTypeDef,
+    _OptionalListVaultsInputListVaultsPaginateTypeDef,
+):
+    pass
+
+
 ListVaultsInputRequestTypeDef = TypedDict(
     "ListVaultsInputRequestTypeDef",
     {
         "accountId": str,
         "marker": str,
         "limit": str,
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
 PurchaseProvisionedCapacityInputRequestTypeDef = TypedDict(
     "PurchaseProvisionedCapacityInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+PurchaseProvisionedCapacityOutputTypeDef = TypedDict(
+    "PurchaseProvisionedCapacityOutputTypeDef",
+    {
+        "capacityId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRemoveTagsFromVaultInputRequestTypeDef = TypedDict(
     "_RequiredRemoveTagsFromVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalRemoveTagsFromVaultInputRequestTypeDef = TypedDict(
@@ -876,66 +1105,29 @@
     {
         "accountId": str,
         "TagKeys": Sequence[str],
     },
     total=False,
 )
 
+
 class RemoveTagsFromVaultInputRequestTypeDef(
     _RequiredRemoveTagsFromVaultInputRequestTypeDef, _OptionalRemoveTagsFromVaultInputRequestTypeDef
 ):
     pass
 
-ServiceResourceAccountRequestTypeDef = TypedDict(
-    "ServiceResourceAccountRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-
-ServiceResourceArchiveRequestTypeDef = TypedDict(
-    "ServiceResourceArchiveRequestTypeDef",
-    {
-        "account_id": str,
-        "vault_name": str,
-        "id": str,
-    },
-)
 
-ServiceResourceJobRequestTypeDef = TypedDict(
-    "ServiceResourceJobRequestTypeDef",
-    {
-        "account_id": str,
-        "vault_name": str,
-        "id": str,
-    },
-)
-
-ServiceResourceMultipartUploadRequestTypeDef = TypedDict(
-    "ServiceResourceMultipartUploadRequestTypeDef",
-    {
-        "account_id": str,
-        "vault_name": str,
-        "id": str,
-    },
-)
-
-ServiceResourceNotificationRequestTypeDef = TypedDict(
-    "ServiceResourceNotificationRequestTypeDef",
-    {
-        "account_id": str,
-        "vault_name": str,
-    },
-)
-
-ServiceResourceVaultRequestTypeDef = TypedDict(
-    "ServiceResourceVaultRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "account_id": str,
-        "name": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredUploadArchiveInputRequestTypeDef = TypedDict(
     "_RequiredUploadArchiveInputRequestTypeDef",
     {
         "vaultName": str,
@@ -948,19 +1140,21 @@
         "archiveDescription": str,
         "checksum": str,
         "body": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
+
 class UploadArchiveInputRequestTypeDef(
     _RequiredUploadArchiveInputRequestTypeDef, _OptionalUploadArchiveInputRequestTypeDef
 ):
     pass
 
+
 UploadArchiveInputVaultUploadArchiveTypeDef = TypedDict(
     "UploadArchiveInputVaultUploadArchiveTypeDef",
     {
         "archiveDescription": str,
         "checksum": str,
         "body": Union[str, bytes, IO[Any], StreamingBody],
     },
@@ -991,163 +1185,26 @@
         "checksum": str,
         "range": str,
         "body": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
+
 class UploadMultipartPartInputRequestTypeDef(
     _RequiredUploadMultipartPartInputRequestTypeDef, _OptionalUploadMultipartPartInputRequestTypeDef
 ):
     pass
 
-VaultArchiveRequestTypeDef = TypedDict(
-    "VaultArchiveRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-
-VaultJobRequestTypeDef = TypedDict(
-    "VaultJobRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-
-VaultMultipartUploadRequestTypeDef = TypedDict(
-    "VaultMultipartUploadRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-
-ArchiveCreationOutputTypeDef = TypedDict(
-    "ArchiveCreationOutputTypeDef",
-    {
-        "location": str,
-        "checksum": str,
-        "archiveId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateVaultOutputTypeDef = TypedDict(
-    "CreateVaultOutputTypeDef",
-    {
-        "location": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeVaultOutputResponseMetadataTypeDef = TypedDict(
-    "DescribeVaultOutputResponseMetadataTypeDef",
-    {
-        "VaultARN": str,
-        "VaultName": str,
-        "CreationDate": str,
-        "LastInventoryDate": str,
-        "NumberOfArchives": int,
-        "SizeInBytes": int,
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
-GetJobOutputOutputTypeDef = TypedDict(
-    "GetJobOutputOutputTypeDef",
-    {
-        "body": StreamingBody,
-        "checksum": str,
-        "status": int,
-        "contentRange": str,
-        "acceptRanges": str,
-        "contentType": str,
-        "archiveDescription": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetVaultLockOutputTypeDef = TypedDict(
-    "GetVaultLockOutputTypeDef",
-    {
-        "Policy": str,
-        "State": str,
-        "ExpirationDate": str,
-        "CreationDate": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InitiateJobOutputTypeDef = TypedDict(
-    "InitiateJobOutputTypeDef",
-    {
-        "location": str,
-        "jobId": str,
-        "jobOutputPath": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InitiateMultipartUploadOutputTypeDef = TypedDict(
-    "InitiateMultipartUploadOutputTypeDef",
-    {
-        "location": str,
-        "uploadId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InitiateVaultLockOutputTypeDef = TypedDict(
-    "InitiateVaultLockOutputTypeDef",
-    {
-        "lockId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InventoryRetrievalJobDescriptionResponseMetadataTypeDef = TypedDict(
-    "InventoryRetrievalJobDescriptionResponseMetadataTypeDef",
-    {
-        "Format": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Limit": str,
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForVaultOutputTypeDef = TypedDict(
-    "ListTagsForVaultOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PurchaseProvisionedCapacityOutputTypeDef = TypedDict(
-    "PurchaseProvisionedCapacityOutputTypeDef",
-    {
-        "capacityId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 UploadMultipartPartOutputTypeDef = TypedDict(
     "UploadMultipartPartOutputTypeDef",
     {
         "checksum": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InputSerializationTypeDef = TypedDict(
     "InputSerializationTypeDef",
     {
         "csv": CSVInputTypeDef,
@@ -1182,20 +1239,22 @@
     "_OptionalDescribeVaultInputVaultExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeVaultInputVaultExistsWaitTypeDef(
     _RequiredDescribeVaultInputVaultExistsWaitTypeDef,
     _OptionalDescribeVaultInputVaultExistsWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeVaultInputVaultNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeVaultInputVaultNotExistsWaitTypeDef",
     {
         "accountId": str,
         "vaultName": str,
     },
 )
@@ -1203,34 +1262,36 @@
     "_OptionalDescribeVaultInputVaultNotExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeVaultInputVaultNotExistsWaitTypeDef(
     _RequiredDescribeVaultInputVaultNotExistsWaitTypeDef,
     _OptionalDescribeVaultInputVaultNotExistsWaitTypeDef,
 ):
     pass
 
+
 ListVaultsOutputTypeDef = TypedDict(
     "ListVaultsOutputTypeDef",
     {
         "VaultList": List[DescribeVaultOutputTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVaultAccessPolicyOutputTypeDef = TypedDict(
     "GetVaultAccessPolicyOutputTypeDef",
     {
         "policy": VaultAccessPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredSetVaultAccessPolicyInputRequestTypeDef",
     {
         "vaultName": str,
@@ -1241,25 +1302,27 @@
     {
         "accountId": str,
         "policy": VaultAccessPolicyTypeDef,
     },
     total=False,
 )
 
+
 class SetVaultAccessPolicyInputRequestTypeDef(
     _RequiredSetVaultAccessPolicyInputRequestTypeDef,
     _OptionalSetVaultAccessPolicyInputRequestTypeDef,
 ):
     pass
 
+
 GetVaultNotificationsOutputTypeDef = TypedDict(
     "GetVaultNotificationsOutputTypeDef",
     {
         "vaultNotificationConfig": VaultNotificationConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetVaultNotificationsInputNotificationSetTypeDef = TypedDict(
     "SetVaultNotificationsInputNotificationSetTypeDef",
     {
         "vaultNotificationConfig": VaultNotificationConfigTypeDef,
@@ -1278,20 +1341,22 @@
     {
         "accountId": str,
         "vaultNotificationConfig": VaultNotificationConfigTypeDef,
     },
     total=False,
 )
 
+
 class SetVaultNotificationsInputRequestTypeDef(
     _RequiredSetVaultNotificationsInputRequestTypeDef,
     _OptionalSetVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
+
 GrantTypeDef = TypedDict(
     "GrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": PermissionType,
     },
     total=False,
@@ -1308,142 +1373,60 @@
     {
         "accountId": str,
         "policy": VaultLockPolicyTypeDef,
     },
     total=False,
 )
 
+
 class InitiateVaultLockInputRequestTypeDef(
     _RequiredInitiateVaultLockInputRequestTypeDef, _OptionalInitiateVaultLockInputRequestTypeDef
 ):
     pass
 
-_RequiredListJobsInputListJobsPaginateTypeDef = TypedDict(
-    "_RequiredListJobsInputListJobsPaginateTypeDef",
-    {
-        "accountId": str,
-        "vaultName": str,
-    },
-)
-_OptionalListJobsInputListJobsPaginateTypeDef = TypedDict(
-    "_OptionalListJobsInputListJobsPaginateTypeDef",
-    {
-        "statuscode": str,
-        "completed": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListJobsInputListJobsPaginateTypeDef(
-    _RequiredListJobsInputListJobsPaginateTypeDef, _OptionalListJobsInputListJobsPaginateTypeDef
-):
-    pass
-
-_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
-    {
-        "accountId": str,
-        "vaultName": str,
-    },
-)
-_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef(
-    _RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
-    _OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
-):
-    pass
-
-_RequiredListPartsInputListPartsPaginateTypeDef = TypedDict(
-    "_RequiredListPartsInputListPartsPaginateTypeDef",
-    {
-        "accountId": str,
-        "vaultName": str,
-        "uploadId": str,
-    },
-)
-_OptionalListPartsInputListPartsPaginateTypeDef = TypedDict(
-    "_OptionalListPartsInputListPartsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPartsInputListPartsPaginateTypeDef(
-    _RequiredListPartsInputListPartsPaginateTypeDef, _OptionalListPartsInputListPartsPaginateTypeDef
-):
-    pass
-
-_RequiredListVaultsInputListVaultsPaginateTypeDef = TypedDict(
-    "_RequiredListVaultsInputListVaultsPaginateTypeDef",
-    {
-        "accountId": str,
-    },
-)
-_OptionalListVaultsInputListVaultsPaginateTypeDef = TypedDict(
-    "_OptionalListVaultsInputListVaultsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListVaultsInputListVaultsPaginateTypeDef(
-    _RequiredListVaultsInputListVaultsPaginateTypeDef,
-    _OptionalListVaultsInputListVaultsPaginateTypeDef,
-):
-    pass
 
 ListMultipartUploadsOutputTypeDef = TypedDict(
     "ListMultipartUploadsOutputTypeDef",
     {
         "UploadsList": List[UploadListElementTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPartsOutputTypeDef = TypedDict(
     "ListPartsOutputTypeDef",
     {
         "MultipartUploadId": str,
         "VaultARN": str,
         "ArchiveDescription": str,
         "PartSizeInBytes": int,
         "CreationDate": str,
         "Parts": List[PartListElementTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProvisionedCapacityOutputTypeDef = TypedDict(
     "ListProvisionedCapacityOutputTypeDef",
     {
         "ProvisionedCapacityList": List[ProvisionedCapacityDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SelectParametersResponseMetadataTypeDef = TypedDict(
     "SelectParametersResponseMetadataTypeDef",
     {
         "InputSerialization": InputSerializationTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
         "OutputSerialization": OutputSerializationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SelectParametersTypeDef = TypedDict(
     "SelectParametersTypeDef",
     {
         "InputSerialization": InputSerializationTypeDef,
@@ -1454,15 +1437,15 @@
     total=False,
 )
 
 GetDataRetrievalPolicyOutputTypeDef = TypedDict(
     "GetDataRetrievalPolicyOutputTypeDef",
     {
         "Policy": DataRetrievalPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetDataRetrievalPolicyInputRequestTypeDef = TypedDict(
     "SetDataRetrievalPolicyInputRequestTypeDef",
     {
         "accountId": str,
@@ -1486,15 +1469,15 @@
     total=False,
 )
 
 OutputLocationResponseMetadataTypeDef = TypedDict(
     "OutputLocationResponseMetadataTypeDef",
     {
         "S3": S3LocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OutputLocationTypeDef = TypedDict(
     "OutputLocationTypeDef",
     {
         "S3": S3LocationTypeDef,
@@ -1522,15 +1505,15 @@
         "ArchiveSHA256TreeHash": str,
         "RetrievalByteRange": str,
         "Tier": str,
         "InventoryRetrievalParameters": InventoryRetrievalJobDescriptionTypeDef,
         "JobOutputPath": str,
         "SelectParameters": SelectParametersTypeDef,
         "OutputLocation": OutputLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GlacierJobDescriptionTypeDef = TypedDict(
     "GlacierJobDescriptionTypeDef",
     {
         "JobId": str,
@@ -1576,15 +1559,15 @@
 )
 
 ListJobsOutputTypeDef = TypedDict(
     "ListJobsOutputTypeDef",
     {
         "JobList": List[GlacierJobDescriptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredInitiateJobInputRequestTypeDef = TypedDict(
     "_RequiredInitiateJobInputRequestTypeDef",
     {
         "vaultName": str,
@@ -1595,11 +1578,12 @@
     {
         "accountId": str,
         "jobParameters": JobParametersTypeDef,
     },
     total=False,
 )
 
+
 class InitiateJobInputRequestTypeDef(
     _RequiredInitiateJobInputRequestTypeDef, _OptionalInitiateJobInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/waiter.py` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier/waiter.pyi` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier.egg-info/PKG-INFO` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glacier
-Version: 1.26.59
-Summary: Type annotations for boto3.Glacier 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Glacier 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-glacier"></a>
 
 # mypy-boto3-glacier
 
 [![PyPI - mypy-boto3-glacier](https://img.shields.io/pypi/v/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glacier?color=blue)](https://pypistats.org/packages/mypy-boto3-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glacier 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[boto3.Glacier 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
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
 [mypy-boto3-glacier docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/).
 
 See how it helps to find and fix potential bugs:
 
@@ -438,105 +438,95 @@
 `mypy_boto3_glacier.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_glacier.type_defs import (
     AbortMultipartUploadInputRequestTypeDef,
     AbortVaultLockInputRequestTypeDef,
-    AccountVaultRequestTypeDef,
     AddTagsToVaultInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    ArchiveCreationOutputTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
     CompleteMultipartUploadInputMultipartUploadCompleteTypeDef,
     CompleteMultipartUploadInputRequestTypeDef,
     CompleteVaultLockInputRequestTypeDef,
     CreateVaultInputAccountCreateVaultTypeDef,
     CreateVaultInputRequestTypeDef,
     CreateVaultInputServiceResourceCreateVaultTypeDef,
+    CreateVaultOutputTypeDef,
     DataRetrievalRuleTypeDef,
     DeleteArchiveInputRequestTypeDef,
     DeleteVaultAccessPolicyInputRequestTypeDef,
     DeleteVaultInputRequestTypeDef,
     DeleteVaultNotificationsInputRequestTypeDef,
     DescribeJobInputRequestTypeDef,
     DescribeVaultInputRequestTypeDef,
     WaiterConfigTypeDef,
+    DescribeVaultOutputResponseMetadataTypeDef,
     DescribeVaultOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionTypeDef,
     GetDataRetrievalPolicyInputRequestTypeDef,
     GetJobOutputInputJobGetOutputTypeDef,
     GetJobOutputInputRequestTypeDef,
+    GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyInputRequestTypeDef,
     VaultAccessPolicyTypeDef,
     GetVaultLockInputRequestTypeDef,
+    GetVaultLockOutputTypeDef,
     GetVaultNotificationsInputRequestTypeDef,
     VaultNotificationConfigTypeDef,
     InventoryRetrievalJobDescriptionTypeDef,
     GranteeTypeDef,
+    InitiateJobOutputTypeDef,
     InitiateMultipartUploadInputRequestTypeDef,
     InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef,
+    InitiateMultipartUploadOutputTypeDef,
     VaultLockPolicyTypeDef,
+    InitiateVaultLockOutputTypeDef,
+    InventoryRetrievalJobDescriptionResponseMetadataTypeDef,
     InventoryRetrievalJobInputTypeDef,
-    PaginatorConfigTypeDef,
+    ListJobsInputListJobsPaginateTypeDef,
     ListJobsInputRequestTypeDef,
+    ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
     ListMultipartUploadsInputRequestTypeDef,
     UploadListElementTypeDef,
+    ListPartsInputListPartsPaginateTypeDef,
     ListPartsInputMultipartUploadPartsTypeDef,
     ListPartsInputRequestTypeDef,
     PartListElementTypeDef,
     ListProvisionedCapacityInputRequestTypeDef,
     ProvisionedCapacityDescriptionTypeDef,
     ListTagsForVaultInputRequestTypeDef,
+    ListTagsForVaultOutputTypeDef,
+    ListVaultsInputListVaultsPaginateTypeDef,
     ListVaultsInputRequestTypeDef,
+    PaginatorConfigTypeDef,
     PurchaseProvisionedCapacityInputRequestTypeDef,
+    PurchaseProvisionedCapacityOutputTypeDef,
     RemoveTagsFromVaultInputRequestTypeDef,
-    ServiceResourceAccountRequestTypeDef,
-    ServiceResourceArchiveRequestTypeDef,
-    ServiceResourceJobRequestTypeDef,
-    ServiceResourceMultipartUploadRequestTypeDef,
-    ServiceResourceNotificationRequestTypeDef,
-    ServiceResourceVaultRequestTypeDef,
+    ResponseMetadataTypeDef,
     UploadArchiveInputRequestTypeDef,
     UploadArchiveInputVaultUploadArchiveTypeDef,
     UploadMultipartPartInputMultipartUploadUploadPartTypeDef,
     UploadMultipartPartInputRequestTypeDef,
-    VaultArchiveRequestTypeDef,
-    VaultJobRequestTypeDef,
-    VaultMultipartUploadRequestTypeDef,
-    ArchiveCreationOutputTypeDef,
-    CreateVaultOutputTypeDef,
-    DescribeVaultOutputResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetJobOutputOutputTypeDef,
-    GetVaultLockOutputTypeDef,
-    InitiateJobOutputTypeDef,
-    InitiateMultipartUploadOutputTypeDef,
-    InitiateVaultLockOutputTypeDef,
-    InventoryRetrievalJobDescriptionResponseMetadataTypeDef,
-    ListTagsForVaultOutputTypeDef,
-    PurchaseProvisionedCapacityOutputTypeDef,
     UploadMultipartPartOutputTypeDef,
     InputSerializationTypeDef,
     OutputSerializationTypeDef,
     DataRetrievalPolicyTypeDef,
     DescribeVaultInputVaultExistsWaitTypeDef,
     DescribeVaultInputVaultNotExistsWaitTypeDef,
     ListVaultsOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
     SetVaultAccessPolicyInputRequestTypeDef,
     GetVaultNotificationsOutputTypeDef,
     SetVaultNotificationsInputNotificationSetTypeDef,
     SetVaultNotificationsInputRequestTypeDef,
     GrantTypeDef,
     InitiateVaultLockInputRequestTypeDef,
-    ListJobsInputListJobsPaginateTypeDef,
-    ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
-    ListPartsInputListPartsPaginateTypeDef,
-    ListVaultsInputListVaultsPaginateTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListPartsOutputTypeDef,
     ListProvisionedCapacityOutputTypeDef,
     SelectParametersResponseMetadataTypeDef,
     SelectParametersTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     SetDataRetrievalPolicyInputRequestTypeDef,
@@ -558,42 +548,42 @@
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

### Comparing `mypy-boto3-glacier-1.26.59/mypy_boto3_glacier.egg-info/SOURCES.txt` & `mypy-boto3-glacier-1.27.0/mypy_boto3_glacier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.26.59/setup.py` & `mypy-boto3-glacier-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 Setup script for mypy-boto3-glacier.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-glacier",
-    version="1.26.59",
+    version="1.27.0",
     packages=["mypy_boto3_glacier"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Glacier 1.26.59 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.Glacier 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/",
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


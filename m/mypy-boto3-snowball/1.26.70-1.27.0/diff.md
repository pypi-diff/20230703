# Comparing `tmp/mypy-boto3-snowball-1.26.70.tar.gz` & `tmp/mypy-boto3-snowball-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-snowball-1.26.70.tar", last modified: Mon Feb 13 20:27:09 2023, max compression
+gzip compressed data, was "mypy-boto3-snowball-1.27.0.tar", last modified: Mon Jul  3 19:51:29 2023, max compression
```

## Comparing `mypy-boto3-snowball-1.26.70.tar` & `mypy-boto3-snowball-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:27:09.130620 mypy-boto3-snowball-1.26.70/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-02-13 20:27:09.130620 mypy-boto3-snowball-1.26.70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15277 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:27:09.130620 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23307 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26960 2023-02-13 20:27:00.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26939 2023-02-13 20:27:00.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 20:27:09.130620 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-02-13 20:27:09.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-13 20:27:09.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 20:27:09.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 20:27:09.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-13 20:27:09.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-13 20:27:09.000000 mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 20:27:09.130620 mypy-boto3-snowball-1.26.70/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-13 20:26:59.000000 mypy-boto3-snowball-1.26.70/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:29.568033 mypy-boto3-snowball-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:21.000000 mypy-boto3-snowball-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16788 2023-07-03 19:51:29.568033 mypy-boto3-snowball-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15299 2023-07-03 19:48:21.000000 mypy-boto3-snowball-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:29.568033 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-03 19:48:21.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-03 19:48:21.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:48:21.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23506 2023-07-03 19:48:21.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23467 2023-07-03 19:48:21.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-07-03 19:48:21.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-03 19:48:21.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-07-03 19:48:21.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-03 19:48:21.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:21.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-07-03 19:48:22.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27587 2023-07-03 19:48:22.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:21.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:29.568033 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16788 2023-07-03 19:51:29.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 19:51:29.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:29.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:29.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:29.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:29.000000 mypy-boto3-snowball-1.27.0/mypy_boto3_snowball.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:29.568033 mypy-boto3-snowball-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:48:21.000000 mypy-boto3-snowball-1.27.0/setup.py
```

### Comparing `mypy-boto3-snowball-1.26.70/LICENSE` & `mypy-boto3-snowball-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-snowball-1.26.70/PKG-INFO` & `mypy-boto3-snowball-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-snowball
-Version: 1.26.70
-Summary: Type annotations for boto3.Snowball 1.26.70 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Snowball 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-snowball"></a>
 
 # mypy-boto3-snowball
 
 [![PyPI - mypy-boto3-snowball](https://img.shields.io/pypi/v/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snowball?color=blue)](https://pypistats.org/packages/mypy-boto3-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Snowball 1.26.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[boto3.Snowball 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
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
 [mypy-boto3-snowball docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,74 +361,75 @@
 from mypy_boto3_snowball.type_defs import (
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
     NotificationTypeDef,
     CompatibleImageTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAddressResultTypeDef,
+    JobListEntryTypeDef,
+    CreateJobResultTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
+    CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
+    CreateReturnShippingLabelResultTypeDef,
     DataTransferTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
     DescribeAddressesRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeReturnShippingLabelRequestRequestTypeDef,
+    DescribeReturnShippingLabelResultTypeDef,
     EKSOnDeviceServiceConfigurationTypeDef,
     Ec2AmiResourceTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
+    GetJobManifestResultTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
+    GetJobUnlockCodeResultTypeDef,
+    GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
+    GetSoftwareUpdatesResultTypeDef,
     INDTaxDocumentsTypeDef,
-    JobListEntryTypeDef,
     JobLogsTypeDef,
     KeyRangeTypeDef,
+    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClusterJobsRequestRequestTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
+    S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
     CreateAddressRequestRequestTypeDef,
-    CreateAddressResultTypeDef,
-    CreateClusterResultTypeDef,
-    CreateJobResultTypeDef,
-    CreateLongTermPricingResultTypeDef,
-    CreateReturnShippingLabelResultTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
-    DescribeReturnShippingLabelResultTypeDef,
-    GetJobManifestResultTypeDef,
-    GetJobUnlockCodeResultTypeDef,
-    GetSnowballUsageResultTypeDef,
-    GetSoftwareUpdatesResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
+    CreateClusterResultTypeDef,
+    ListClusterJobsResultTypeDef,
+    ListJobsResultTypeDef,
     DependentServiceTypeDef,
-    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
-    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     LambdaResourceTypeDef,
     TaxDocumentsTypeDef,
-    ListClusterJobsResultTypeDef,
-    ListJobsResultTypeDef,
     ListLongTermPricingResultTypeDef,
     OnDeviceServiceConfigurationTypeDef,
     S3ResourceTypeDef,
     ShippingDetailsTypeDef,
     SnowconeDeviceConfigurationTypeDef,
     ListServiceVersionsRequestRequestTypeDef,
     ListServiceVersionsResultTypeDef,
@@ -452,42 +453,42 @@
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

### Comparing `mypy-boto3-snowball-1.26.70/README.md` & `mypy-boto3-snowball-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-snowball"></a>
 
 # mypy-boto3-snowball
 
 [![PyPI - mypy-boto3-snowball](https://img.shields.io/pypi/v/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snowball?color=blue)](https://pypistats.org/packages/mypy-boto3-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Snowball 1.26.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[boto3.Snowball 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
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
 [mypy-boto3-snowball docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,74 +329,75 @@
 from mypy_boto3_snowball.type_defs import (
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
     NotificationTypeDef,
     CompatibleImageTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAddressResultTypeDef,
+    JobListEntryTypeDef,
+    CreateJobResultTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
+    CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
+    CreateReturnShippingLabelResultTypeDef,
     DataTransferTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
     DescribeAddressesRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeReturnShippingLabelRequestRequestTypeDef,
+    DescribeReturnShippingLabelResultTypeDef,
     EKSOnDeviceServiceConfigurationTypeDef,
     Ec2AmiResourceTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
+    GetJobManifestResultTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
+    GetJobUnlockCodeResultTypeDef,
+    GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
+    GetSoftwareUpdatesResultTypeDef,
     INDTaxDocumentsTypeDef,
-    JobListEntryTypeDef,
     JobLogsTypeDef,
     KeyRangeTypeDef,
+    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClusterJobsRequestRequestTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
+    S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
     CreateAddressRequestRequestTypeDef,
-    CreateAddressResultTypeDef,
-    CreateClusterResultTypeDef,
-    CreateJobResultTypeDef,
-    CreateLongTermPricingResultTypeDef,
-    CreateReturnShippingLabelResultTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
-    DescribeReturnShippingLabelResultTypeDef,
-    GetJobManifestResultTypeDef,
-    GetJobUnlockCodeResultTypeDef,
-    GetSnowballUsageResultTypeDef,
-    GetSoftwareUpdatesResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
+    CreateClusterResultTypeDef,
+    ListClusterJobsResultTypeDef,
+    ListJobsResultTypeDef,
     DependentServiceTypeDef,
-    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
-    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     LambdaResourceTypeDef,
     TaxDocumentsTypeDef,
-    ListClusterJobsResultTypeDef,
-    ListJobsResultTypeDef,
     ListLongTermPricingResultTypeDef,
     OnDeviceServiceConfigurationTypeDef,
     S3ResourceTypeDef,
     ShippingDetailsTypeDef,
     SnowconeDeviceConfigurationTypeDef,
     ListServiceVersionsRequestRequestTypeDef,
     ListServiceVersionsResultTypeDef,
@@ -420,42 +421,42 @@
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

### Comparing `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/__init__.py` & `mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/__init__.pyi` & `mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/__main__.py` & `mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Snowball 1.26.70\nVersion:         1.26.70\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Snowball 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.70")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/client.py` & `mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,26 +155,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_address)
         """
 
     def create_cluster(
         self,
         *,
         JobType: JobTypeType,
-        Resources: JobResourceTypeDef,
         AddressId: str,
-        RoleARN: str,
         SnowballType: SnowballTypeType,
         ShippingOption: ShippingOptionType,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         KmsKeyARN: str = ...,
+        RoleARN: str = ...,
         Notification: NotificationTypeDef = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
-        RemoteManagement: RemoteManagementType = ...
+        RemoteManagement: RemoteManagementType = ...,
+        InitialClusterSize: int = ...,
+        ForceCreateJobs: bool = ...,
+        LongTermPricingIds: Sequence[str] = ...,
+        SnowballCapacityPreference: SnowballCapacityType = ...
     ) -> CreateClusterResultTypeDef:
         """
         Creates an empty cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_cluster)
         """
@@ -320,15 +324,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.get_snowball_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#get_snowball_usage)
         """
 
     def get_software_updates(self, *, JobId: str) -> GetSoftwareUpdatesResultTypeDef:
         """
         Returns an Amazon S3 presigned URL for an update file associated with a
-        specified `JobId` .
+        specified `JobId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.get_software_updates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#get_software_updates)
         """
 
     def list_cluster_jobs(
         self, *, ClusterId: str, MaxResults: int = ..., NextToken: str = ...
@@ -427,15 +431,15 @@
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Description: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ForwardingAddressId: str = ...
     ) -> Dict[str, Any]:
         """
-        While a job's `JobState` value is `New` , you can update some of the information
+        While a job's `JobState` value is `New`, you can update some of the information
         associated with a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#update_job)
         """
 
     def update_job_shipment_state(
```

### Comparing `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/client.pyi` & `mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -145,26 +145,30 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_address)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_address)
         """
     def create_cluster(
         self,
         *,
         JobType: JobTypeType,
-        Resources: JobResourceTypeDef,
         AddressId: str,
-        RoleARN: str,
         SnowballType: SnowballTypeType,
         ShippingOption: ShippingOptionType,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         KmsKeyARN: str = ...,
+        RoleARN: str = ...,
         Notification: NotificationTypeDef = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
-        RemoteManagement: RemoteManagementType = ...
+        RemoteManagement: RemoteManagementType = ...,
+        InitialClusterSize: int = ...,
+        ForceCreateJobs: bool = ...,
+        LongTermPricingIds: Sequence[str] = ...,
+        SnowballCapacityPreference: SnowballCapacityType = ...
     ) -> CreateClusterResultTypeDef:
         """
         Creates an empty cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#create_cluster)
         """
@@ -297,15 +301,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.get_snowball_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#get_snowball_usage)
         """
     def get_software_updates(self, *, JobId: str) -> GetSoftwareUpdatesResultTypeDef:
         """
         Returns an Amazon S3 presigned URL for an update file associated with a
-        specified `JobId` .
+        specified `JobId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.get_software_updates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#get_software_updates)
         """
     def list_cluster_jobs(
         self, *, ClusterId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListClusterJobsResultTypeDef:
@@ -396,15 +400,15 @@
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Description: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ForwardingAddressId: str = ...
     ) -> Dict[str, Any]:
         """
-        While a job's `JobState` value is `New` , you can update some of the information
+        While a job's `JobState` value is `New`, you can update some of the information
         associated with a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/client/#update_job)
         """
     def update_job_shipment_state(
         self, *, JobId: str, ShipmentState: ShipmentStateType
```

### Comparing `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/literals.py` & `mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,25 +68,25 @@
 ]
 JobTypeType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 ListClusterJobsPaginatorName = Literal["list_cluster_jobs"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListCompatibleImagesPaginatorName = Literal["list_compatible_images"]
 ListJobsPaginatorName = Literal["list_jobs"]
 ListLongTermPricingPaginatorName = Literal["list_long_term_pricing"]
-LongTermPricingTypeType = Literal["OneYear", "ThreeYear"]
+LongTermPricingTypeType = Literal["OneMonth", "OneYear", "ThreeYear"]
 RemoteManagementType = Literal["INSTALLED_AUTOSTART", "INSTALLED_ONLY"]
 ServiceNameType = Literal["EKS_ANYWHERE", "KUBERNETES"]
 ShipmentStateType = Literal["RECEIVED", "RETURNED"]
 ShippingLabelStatusType = Literal["Failed", "InProgress", "Succeeded", "TimedOut"]
 ShippingOptionType = Literal["EXPRESS", "NEXT_DAY", "SECOND_DAY", "STANDARD"]
 SnowballCapacityType = Literal[
-    "NoPreference", "T100", "T14", "T32", "T42", "T50", "T8", "T80", "T98"
+    "NoPreference", "T100", "T14", "T240", "T32", "T42", "T50", "T8", "T80", "T98"
 ]
 SnowballTypeType = Literal[
-    "EDGE", "EDGE_C", "EDGE_CG", "EDGE_S", "SNC1_HDD", "SNC1_SSD", "STANDARD", "V3_5C"
+    "EDGE", "EDGE_C", "EDGE_CG", "EDGE_S", "SNC1_HDD", "SNC1_SSD", "STANDARD", "V3_5C", "V3_5S"
 ]
 StorageUnitType = Literal["TB"]
 TransferOptionType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 SnowballServiceName = Literal["snowball"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -98,14 +98,15 @@
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
@@ -145,14 +146,15 @@
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
@@ -249,14 +252,15 @@
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
@@ -292,14 +296,15 @@
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
@@ -318,16 +323,19 @@
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
@@ -407,18 +415,21 @@
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
@@ -461,13 +472,14 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/literals.pyi` & `mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -66,25 +66,25 @@
 ]
 JobTypeType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 ListClusterJobsPaginatorName = Literal["list_cluster_jobs"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListCompatibleImagesPaginatorName = Literal["list_compatible_images"]
 ListJobsPaginatorName = Literal["list_jobs"]
 ListLongTermPricingPaginatorName = Literal["list_long_term_pricing"]
-LongTermPricingTypeType = Literal["OneYear", "ThreeYear"]
+LongTermPricingTypeType = Literal["OneMonth", "OneYear", "ThreeYear"]
 RemoteManagementType = Literal["INSTALLED_AUTOSTART", "INSTALLED_ONLY"]
 ServiceNameType = Literal["EKS_ANYWHERE", "KUBERNETES"]
 ShipmentStateType = Literal["RECEIVED", "RETURNED"]
 ShippingLabelStatusType = Literal["Failed", "InProgress", "Succeeded", "TimedOut"]
 ShippingOptionType = Literal["EXPRESS", "NEXT_DAY", "SECOND_DAY", "STANDARD"]
 SnowballCapacityType = Literal[
-    "NoPreference", "T100", "T14", "T32", "T42", "T50", "T8", "T80", "T98"
+    "NoPreference", "T100", "T14", "T240", "T32", "T42", "T50", "T8", "T80", "T98"
 ]
 SnowballTypeType = Literal[
-    "EDGE", "EDGE_C", "EDGE_CG", "EDGE_S", "SNC1_HDD", "SNC1_SSD", "STANDARD", "V3_5C"
+    "EDGE", "EDGE_C", "EDGE_CG", "EDGE_S", "SNC1_HDD", "SNC1_SSD", "STANDARD", "V3_5C", "V3_5S"
 ]
 StorageUnitType = Literal["TB"]
 TransferOptionType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 SnowballServiceName = Literal["snowball"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -96,14 +96,15 @@
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
@@ -143,14 +144,15 @@
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
@@ -229,14 +231,15 @@
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
@@ -247,14 +250,15 @@
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
@@ -290,14 +294,15 @@
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
@@ -316,16 +321,19 @@
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
@@ -405,18 +413,21 @@
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
@@ -459,13 +470,14 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/paginator.py` & `mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,88 +66,88 @@
 class DescribeAddressesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#describeaddressespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAddressesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#describeaddressespaginator)
         """
 
 
 class ListClusterJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterjobspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClusterJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterjobspaginator)
         """
 
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterspaginator)
         """
 
 
 class ListCompatibleImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listcompatibleimagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCompatibleImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listcompatibleimagespaginator)
         """
 
 
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listjobspaginator)
         """
 
 
 class ListLongTermPricingPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listlongtermpricingpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLongTermPricingResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listlongtermpricingpaginator)
         """
```

### Comparing `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/paginator.pyi` & `mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -63,83 +63,83 @@
 class DescribeAddressesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#describeaddressespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeAddressesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#describeaddressespaginator)
         """
 
 class ListClusterJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterjobspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClusterJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterjobspaginator)
         """
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listclusterspaginator)
         """
 
 class ListCompatibleImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listcompatibleimagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCompatibleImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listcompatibleimagespaginator)
         """
 
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listjobspaginator)
         """
 
 class ListLongTermPricingPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listlongtermpricingpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLongTermPricingResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/paginators/#listlongtermpricingpaginator)
         """
```

### Comparing `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/type_defs.py` & `mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,74 +44,75 @@
 __all__ = (
     "AddressTypeDef",
     "CancelClusterRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ClusterListEntryTypeDef",
     "NotificationTypeDef",
     "CompatibleImageTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAddressResultTypeDef",
+    "JobListEntryTypeDef",
+    "CreateJobResultTypeDef",
     "CreateLongTermPricingRequestRequestTypeDef",
+    "CreateLongTermPricingResultTypeDef",
     "CreateReturnShippingLabelRequestRequestTypeDef",
+    "CreateReturnShippingLabelResultTypeDef",
     "DataTransferTypeDef",
     "ServiceVersionTypeDef",
     "DescribeAddressRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     "DescribeAddressesRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeReturnShippingLabelRequestRequestTypeDef",
+    "DescribeReturnShippingLabelResultTypeDef",
     "EKSOnDeviceServiceConfigurationTypeDef",
     "Ec2AmiResourceTypeDef",
     "EventTriggerDefinitionTypeDef",
     "GetJobManifestRequestRequestTypeDef",
+    "GetJobManifestResultTypeDef",
     "GetJobUnlockCodeRequestRequestTypeDef",
+    "GetJobUnlockCodeResultTypeDef",
+    "GetSnowballUsageResultTypeDef",
     "GetSoftwareUpdatesRequestRequestTypeDef",
+    "GetSoftwareUpdatesResultTypeDef",
     "INDTaxDocumentsTypeDef",
-    "JobListEntryTypeDef",
     "JobLogsTypeDef",
     "KeyRangeTypeDef",
+    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
     "ListClusterJobsRequestRequestTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
     "ListCompatibleImagesRequestRequestTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "ListLongTermPricingRequestRequestTypeDef",
     "LongTermPricingListEntryTypeDef",
     "NFSOnDeviceServiceConfigurationTypeDef",
+    "S3OnDeviceServiceConfigurationTypeDef",
     "TGWOnDeviceServiceConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TargetOnDeviceServiceTypeDef",
     "ShipmentTypeDef",
     "WirelessConnectionTypeDef",
     "UpdateJobShipmentStateRequestRequestTypeDef",
     "UpdateLongTermPricingRequestRequestTypeDef",
     "CreateAddressRequestRequestTypeDef",
-    "CreateAddressResultTypeDef",
-    "CreateClusterResultTypeDef",
-    "CreateJobResultTypeDef",
-    "CreateLongTermPricingResultTypeDef",
-    "CreateReturnShippingLabelResultTypeDef",
     "DescribeAddressResultTypeDef",
     "DescribeAddressesResultTypeDef",
-    "DescribeReturnShippingLabelResultTypeDef",
-    "GetJobManifestResultTypeDef",
-    "GetJobUnlockCodeResultTypeDef",
-    "GetSnowballUsageResultTypeDef",
-    "GetSoftwareUpdatesResultTypeDef",
     "ListClustersResultTypeDef",
     "ListCompatibleImagesResultTypeDef",
+    "CreateClusterResultTypeDef",
+    "ListClusterJobsResultTypeDef",
+    "ListJobsResultTypeDef",
     "DependentServiceTypeDef",
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
-    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "LambdaResourceTypeDef",
     "TaxDocumentsTypeDef",
-    "ListClusterJobsResultTypeDef",
-    "ListJobsResultTypeDef",
     "ListLongTermPricingResultTypeDef",
     "OnDeviceServiceConfigurationTypeDef",
     "S3ResourceTypeDef",
     "ShippingDetailsTypeDef",
     "SnowconeDeviceConfigurationTypeDef",
     "ListServiceVersionsRequestRequestTypeDef",
     "ListServiceVersionsResultTypeDef",
@@ -188,22 +189,41 @@
     {
         "AmiId": str,
         "Name": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAddressResultTypeDef = TypedDict(
+    "CreateAddressResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AddressId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+JobListEntryTypeDef = TypedDict(
+    "JobListEntryTypeDef",
+    {
+        "JobId": str,
+        "JobState": JobStateType,
+        "IsMaster": bool,
+        "JobType": JobTypeType,
+        "SnowballType": SnowballTypeType,
+        "CreationDate": datetime,
+        "Description": str,
+    },
+    total=False,
+)
+
+CreateJobResultTypeDef = TypedDict(
+    "CreateJobResultTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLongTermPricingRequestRequestTypeDef",
     {
         "LongTermPricingType": LongTermPricingTypeType,
@@ -222,14 +242,22 @@
 class CreateLongTermPricingRequestRequestTypeDef(
     _RequiredCreateLongTermPricingRequestRequestTypeDef,
     _OptionalCreateLongTermPricingRequestRequestTypeDef,
 ):
     pass
 
 
+CreateLongTermPricingResultTypeDef = TypedDict(
+    "CreateLongTermPricingResultTypeDef",
+    {
+        "LongTermPricingId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
@@ -244,14 +272,22 @@
 class CreateReturnShippingLabelRequestRequestTypeDef(
     _RequiredCreateReturnShippingLabelRequestRequestTypeDef,
     _OptionalCreateReturnShippingLabelRequestRequestTypeDef,
 ):
     pass
 
 
+CreateReturnShippingLabelResultTypeDef = TypedDict(
+    "CreateReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataTransferTypeDef = TypedDict(
     "DataTransferTypeDef",
     {
         "BytesTransferred": int,
         "ObjectsTransferred": int,
         "TotalBytes": int,
         "TotalObjects": int,
@@ -270,20 +306,18 @@
 DescribeAddressRequestRequestTypeDef = TypedDict(
     "DescribeAddressRequestRequestTypeDef",
     {
         "AddressId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAddressesRequestRequestTypeDef = TypedDict(
     "DescribeAddressesRequestRequestTypeDef",
     {
@@ -310,14 +344,24 @@
 DescribeReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "DescribeReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+DescribeReturnShippingLabelResultTypeDef = TypedDict(
+    "DescribeReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ExpirationDate": datetime,
+        "ReturnShippingLabelURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EKSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "EKSOnDeviceServiceConfigurationTypeDef",
     {
         "KubernetesVersion": str,
         "EKSAnywhereVersion": str,
     },
     total=False,
@@ -353,46 +397,65 @@
 GetJobManifestRequestRequestTypeDef = TypedDict(
     "GetJobManifestRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetJobManifestResultTypeDef = TypedDict(
+    "GetJobManifestResultTypeDef",
+    {
+        "ManifestURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetJobUnlockCodeRequestRequestTypeDef = TypedDict(
     "GetJobUnlockCodeRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetJobUnlockCodeResultTypeDef = TypedDict(
+    "GetJobUnlockCodeResultTypeDef",
+    {
+        "UnlockCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSnowballUsageResultTypeDef = TypedDict(
+    "GetSnowballUsageResultTypeDef",
+    {
+        "SnowballLimit": int,
+        "SnowballsInUse": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSoftwareUpdatesRequestRequestTypeDef = TypedDict(
     "GetSoftwareUpdatesRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-INDTaxDocumentsTypeDef = TypedDict(
-    "INDTaxDocumentsTypeDef",
+GetSoftwareUpdatesResultTypeDef = TypedDict(
+    "GetSoftwareUpdatesResultTypeDef",
     {
-        "GSTIN": str,
+        "UpdatesURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-JobListEntryTypeDef = TypedDict(
-    "JobListEntryTypeDef",
+INDTaxDocumentsTypeDef = TypedDict(
+    "INDTaxDocumentsTypeDef",
     {
-        "JobId": str,
-        "JobState": JobStateType,
-        "IsMaster": bool,
-        "JobType": JobTypeType,
-        "SnowballType": SnowballTypeType,
-        "CreationDate": datetime,
-        "Description": str,
+        "GSTIN": str,
     },
     total=False,
 )
 
 JobLogsTypeDef = TypedDict(
     "JobLogsTypeDef",
     {
@@ -408,14 +471,36 @@
     {
         "BeginMarker": str,
         "EndMarker": str,
     },
     total=False,
 )
 
+_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
+    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
+    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListClusterJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterJobsRequestRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListClusterJobsRequestRequestTypeDef = TypedDict(
@@ -430,41 +515,73 @@
 
 class ListClusterJobsRequestRequestTypeDef(
     _RequiredListClusterJobsRequestRequestTypeDef, _OptionalListClusterJobsRequestRequestTypeDef
 ):
     pass
 
 
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCompatibleImagesRequestRequestTypeDef = TypedDict(
     "ListCompatibleImagesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLongTermPricingRequestRequestTypeDef = TypedDict(
     "ListLongTermPricingRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -492,23 +609,55 @@
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
 )
 
+S3OnDeviceServiceConfigurationTypeDef = TypedDict(
+    "S3OnDeviceServiceConfigurationTypeDef",
+    {
+        "StorageLimit": float,
+        "StorageUnit": Literal["TB"],
+        "ServiceSize": int,
+        "FaultTolerance": int,
+    },
+    total=False,
+)
+
 TGWOnDeviceServiceConfigurationTypeDef = TypedDict(
     "TGWOnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
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
 TargetOnDeviceServiceTypeDef = TypedDict(
     "TargetOnDeviceServiceTypeDef",
     {
         "ServiceName": DeviceServiceNameType,
         "TransferOption": TransferOptionType,
     },
     total=False,
@@ -565,199 +714,81 @@
 CreateAddressRequestRequestTypeDef = TypedDict(
     "CreateAddressRequestRequestTypeDef",
     {
         "Address": AddressTypeDef,
     },
 )
 
-CreateAddressResultTypeDef = TypedDict(
-    "CreateAddressResultTypeDef",
-    {
-        "AddressId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateClusterResultTypeDef = TypedDict(
-    "CreateClusterResultTypeDef",
-    {
-        "ClusterId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobResultTypeDef = TypedDict(
-    "CreateJobResultTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLongTermPricingResultTypeDef = TypedDict(
-    "CreateLongTermPricingResultTypeDef",
-    {
-        "LongTermPricingId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateReturnShippingLabelResultTypeDef = TypedDict(
-    "CreateReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAddressResultTypeDef = TypedDict(
     "DescribeAddressResultTypeDef",
     {
         "Address": AddressTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAddressesResultTypeDef = TypedDict(
     "DescribeAddressesResultTypeDef",
     {
         "Addresses": List[AddressTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeReturnShippingLabelResultTypeDef = TypedDict(
-    "DescribeReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ExpirationDate": datetime,
-        "ReturnShippingLabelURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetJobManifestResultTypeDef = TypedDict(
-    "GetJobManifestResultTypeDef",
-    {
-        "ManifestURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetJobUnlockCodeResultTypeDef = TypedDict(
-    "GetJobUnlockCodeResultTypeDef",
-    {
-        "UnlockCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSnowballUsageResultTypeDef = TypedDict(
-    "GetSnowballUsageResultTypeDef",
-    {
-        "SnowballLimit": int,
-        "SnowballsInUse": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSoftwareUpdatesResultTypeDef = TypedDict(
-    "GetSoftwareUpdatesResultTypeDef",
-    {
-        "UpdatesURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClustersResultTypeDef = TypedDict(
     "ListClustersResultTypeDef",
     {
         "ClusterListEntries": List[ClusterListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCompatibleImagesResultTypeDef = TypedDict(
     "ListCompatibleImagesResultTypeDef",
     {
         "CompatibleImages": List[CompatibleImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DependentServiceTypeDef = TypedDict(
-    "DependentServiceTypeDef",
-    {
-        "ServiceName": ServiceNameType,
-        "ServiceVersion": ServiceVersionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
+CreateClusterResultTypeDef = TypedDict(
+    "CreateClusterResultTypeDef",
     {
         "ClusterId": str,
+        "JobListEntries": List[JobListEntryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
-    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
-):
-    pass
-
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
-ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
+ListClusterJobsResultTypeDef = TypedDict(
+    "ListClusterJobsResultTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "JobListEntries": List[JobListEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
+ListJobsResultTypeDef = TypedDict(
+    "ListJobsResultTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "JobListEntries": List[JobListEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
+DependentServiceTypeDef = TypedDict(
+    "DependentServiceTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ServiceName": ServiceNameType,
+        "ServiceVersion": ServiceVersionTypeDef,
     },
     total=False,
 )
 
 LambdaResourceTypeDef = TypedDict(
     "LambdaResourceTypeDef",
     {
@@ -771,47 +802,30 @@
     "TaxDocumentsTypeDef",
     {
         "IND": INDTaxDocumentsTypeDef,
     },
     total=False,
 )
 
-ListClusterJobsResultTypeDef = TypedDict(
-    "ListClusterJobsResultTypeDef",
-    {
-        "JobListEntries": List[JobListEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListJobsResultTypeDef = TypedDict(
-    "ListJobsResultTypeDef",
-    {
-        "JobListEntries": List[JobListEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListLongTermPricingResultTypeDef = TypedDict(
     "ListLongTermPricingResultTypeDef",
     {
         "LongTermPricingEntries": List[LongTermPricingListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OnDeviceServiceConfigurationTypeDef = TypedDict(
     "OnDeviceServiceConfigurationTypeDef",
     {
         "NFSOnDeviceService": NFSOnDeviceServiceConfigurationTypeDef,
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationTypeDef,
         "EKSOnDeviceService": EKSOnDeviceServiceConfigurationTypeDef,
+        "S3OnDeviceService": S3OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
 S3ResourceTypeDef = TypedDict(
     "S3ResourceTypeDef",
     {
@@ -867,15 +881,15 @@
 ListServiceVersionsResultTypeDef = TypedDict(
     "ListServiceVersionsResultTypeDef",
     {
         "ServiceVersions": List[ServiceVersionTypeDef],
         "ServiceName": ServiceNameType,
         "DependentServices": List[DependentServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JobResourceTypeDef = TypedDict(
     "JobResourceTypeDef",
     {
         "S3Resources": Sequence[S3ResourceTypeDef],
@@ -915,31 +929,35 @@
     total=False,
 )
 
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "JobType": JobTypeType,
-        "Resources": JobResourceTypeDef,
         "AddressId": str,
-        "RoleARN": str,
         "SnowballType": SnowballTypeType,
         "ShippingOption": ShippingOptionType,
     },
 )
 _OptionalCreateClusterRequestRequestTypeDef = TypedDict(
     "_OptionalCreateClusterRequestRequestTypeDef",
     {
+        "Resources": JobResourceTypeDef,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
         "Description": str,
         "KmsKeyARN": str,
+        "RoleARN": str,
         "Notification": NotificationTypeDef,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "RemoteManagement": RemoteManagementType,
+        "InitialClusterSize": int,
+        "ForceCreateJobs": bool,
+        "LongTermPricingIds": Sequence[str],
+        "SnowballCapacityPreference": SnowballCapacityType,
     },
     total=False,
 )
 
 
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
@@ -1057,19 +1075,19 @@
     total=False,
 )
 
 DescribeClusterResultTypeDef = TypedDict(
     "DescribeClusterResultTypeDef",
     {
         "ClusterMetadata": ClusterMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "JobMetadata": JobMetadataTypeDef,
         "SubJobMetadata": List[JobMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball/type_defs.pyi` & `mypy-boto3-snowball-1.27.0/mypy_boto3_snowball/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -43,74 +43,75 @@
 __all__ = (
     "AddressTypeDef",
     "CancelClusterRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ClusterListEntryTypeDef",
     "NotificationTypeDef",
     "CompatibleImageTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAddressResultTypeDef",
+    "JobListEntryTypeDef",
+    "CreateJobResultTypeDef",
     "CreateLongTermPricingRequestRequestTypeDef",
+    "CreateLongTermPricingResultTypeDef",
     "CreateReturnShippingLabelRequestRequestTypeDef",
+    "CreateReturnShippingLabelResultTypeDef",
     "DataTransferTypeDef",
     "ServiceVersionTypeDef",
     "DescribeAddressRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     "DescribeAddressesRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeReturnShippingLabelRequestRequestTypeDef",
+    "DescribeReturnShippingLabelResultTypeDef",
     "EKSOnDeviceServiceConfigurationTypeDef",
     "Ec2AmiResourceTypeDef",
     "EventTriggerDefinitionTypeDef",
     "GetJobManifestRequestRequestTypeDef",
+    "GetJobManifestResultTypeDef",
     "GetJobUnlockCodeRequestRequestTypeDef",
+    "GetJobUnlockCodeResultTypeDef",
+    "GetSnowballUsageResultTypeDef",
     "GetSoftwareUpdatesRequestRequestTypeDef",
+    "GetSoftwareUpdatesResultTypeDef",
     "INDTaxDocumentsTypeDef",
-    "JobListEntryTypeDef",
     "JobLogsTypeDef",
     "KeyRangeTypeDef",
+    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
     "ListClusterJobsRequestRequestTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
     "ListCompatibleImagesRequestRequestTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "ListLongTermPricingRequestRequestTypeDef",
     "LongTermPricingListEntryTypeDef",
     "NFSOnDeviceServiceConfigurationTypeDef",
+    "S3OnDeviceServiceConfigurationTypeDef",
     "TGWOnDeviceServiceConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TargetOnDeviceServiceTypeDef",
     "ShipmentTypeDef",
     "WirelessConnectionTypeDef",
     "UpdateJobShipmentStateRequestRequestTypeDef",
     "UpdateLongTermPricingRequestRequestTypeDef",
     "CreateAddressRequestRequestTypeDef",
-    "CreateAddressResultTypeDef",
-    "CreateClusterResultTypeDef",
-    "CreateJobResultTypeDef",
-    "CreateLongTermPricingResultTypeDef",
-    "CreateReturnShippingLabelResultTypeDef",
     "DescribeAddressResultTypeDef",
     "DescribeAddressesResultTypeDef",
-    "DescribeReturnShippingLabelResultTypeDef",
-    "GetJobManifestResultTypeDef",
-    "GetJobUnlockCodeResultTypeDef",
-    "GetSnowballUsageResultTypeDef",
-    "GetSoftwareUpdatesResultTypeDef",
     "ListClustersResultTypeDef",
     "ListCompatibleImagesResultTypeDef",
+    "CreateClusterResultTypeDef",
+    "ListClusterJobsResultTypeDef",
+    "ListJobsResultTypeDef",
     "DependentServiceTypeDef",
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
-    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "LambdaResourceTypeDef",
     "TaxDocumentsTypeDef",
-    "ListClusterJobsResultTypeDef",
-    "ListJobsResultTypeDef",
     "ListLongTermPricingResultTypeDef",
     "OnDeviceServiceConfigurationTypeDef",
     "S3ResourceTypeDef",
     "ShippingDetailsTypeDef",
     "SnowconeDeviceConfigurationTypeDef",
     "ListServiceVersionsRequestRequestTypeDef",
     "ListServiceVersionsResultTypeDef",
@@ -187,22 +188,41 @@
     {
         "AmiId": str,
         "Name": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAddressResultTypeDef = TypedDict(
+    "CreateAddressResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AddressId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+JobListEntryTypeDef = TypedDict(
+    "JobListEntryTypeDef",
+    {
+        "JobId": str,
+        "JobState": JobStateType,
+        "IsMaster": bool,
+        "JobType": JobTypeType,
+        "SnowballType": SnowballTypeType,
+        "CreationDate": datetime,
+        "Description": str,
+    },
+    total=False,
+)
+
+CreateJobResultTypeDef = TypedDict(
+    "CreateJobResultTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLongTermPricingRequestRequestTypeDef",
     {
         "LongTermPricingType": LongTermPricingTypeType,
@@ -219,14 +239,22 @@
 
 class CreateLongTermPricingRequestRequestTypeDef(
     _RequiredCreateLongTermPricingRequestRequestTypeDef,
     _OptionalCreateLongTermPricingRequestRequestTypeDef,
 ):
     pass
 
+CreateLongTermPricingResultTypeDef = TypedDict(
+    "CreateLongTermPricingResultTypeDef",
+    {
+        "LongTermPricingId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
@@ -239,14 +267,22 @@
 
 class CreateReturnShippingLabelRequestRequestTypeDef(
     _RequiredCreateReturnShippingLabelRequestRequestTypeDef,
     _OptionalCreateReturnShippingLabelRequestRequestTypeDef,
 ):
     pass
 
+CreateReturnShippingLabelResultTypeDef = TypedDict(
+    "CreateReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataTransferTypeDef = TypedDict(
     "DataTransferTypeDef",
     {
         "BytesTransferred": int,
         "ObjectsTransferred": int,
         "TotalBytes": int,
         "TotalObjects": int,
@@ -265,20 +301,18 @@
 DescribeAddressRequestRequestTypeDef = TypedDict(
     "DescribeAddressRequestRequestTypeDef",
     {
         "AddressId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeAddressesRequestRequestTypeDef = TypedDict(
     "DescribeAddressesRequestRequestTypeDef",
     {
@@ -305,14 +339,24 @@
 DescribeReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "DescribeReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+DescribeReturnShippingLabelResultTypeDef = TypedDict(
+    "DescribeReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ExpirationDate": datetime,
+        "ReturnShippingLabelURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EKSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "EKSOnDeviceServiceConfigurationTypeDef",
     {
         "KubernetesVersion": str,
         "EKSAnywhereVersion": str,
     },
     total=False,
@@ -346,46 +390,65 @@
 GetJobManifestRequestRequestTypeDef = TypedDict(
     "GetJobManifestRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetJobManifestResultTypeDef = TypedDict(
+    "GetJobManifestResultTypeDef",
+    {
+        "ManifestURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetJobUnlockCodeRequestRequestTypeDef = TypedDict(
     "GetJobUnlockCodeRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+GetJobUnlockCodeResultTypeDef = TypedDict(
+    "GetJobUnlockCodeResultTypeDef",
+    {
+        "UnlockCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSnowballUsageResultTypeDef = TypedDict(
+    "GetSnowballUsageResultTypeDef",
+    {
+        "SnowballLimit": int,
+        "SnowballsInUse": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSoftwareUpdatesRequestRequestTypeDef = TypedDict(
     "GetSoftwareUpdatesRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-INDTaxDocumentsTypeDef = TypedDict(
-    "INDTaxDocumentsTypeDef",
+GetSoftwareUpdatesResultTypeDef = TypedDict(
+    "GetSoftwareUpdatesResultTypeDef",
     {
-        "GSTIN": str,
+        "UpdatesURI": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-JobListEntryTypeDef = TypedDict(
-    "JobListEntryTypeDef",
+INDTaxDocumentsTypeDef = TypedDict(
+    "INDTaxDocumentsTypeDef",
     {
-        "JobId": str,
-        "JobState": JobStateType,
-        "IsMaster": bool,
-        "JobType": JobTypeType,
-        "SnowballType": SnowballTypeType,
-        "CreationDate": datetime,
-        "Description": str,
+        "GSTIN": str,
     },
     total=False,
 )
 
 JobLogsTypeDef = TypedDict(
     "JobLogsTypeDef",
     {
@@ -401,14 +464,34 @@
     {
         "BeginMarker": str,
         "EndMarker": str,
     },
     total=False,
 )
 
+_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
+    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
+    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
+):
+    pass
+
 _RequiredListClusterJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterJobsRequestRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListClusterJobsRequestRequestTypeDef = TypedDict(
@@ -421,41 +504,73 @@
 )
 
 class ListClusterJobsRequestRequestTypeDef(
     _RequiredListClusterJobsRequestRequestTypeDef, _OptionalListClusterJobsRequestRequestTypeDef
 ):
     pass
 
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCompatibleImagesRequestRequestTypeDef = TypedDict(
     "ListCompatibleImagesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLongTermPricingRequestRequestTypeDef = TypedDict(
     "ListLongTermPricingRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -483,23 +598,55 @@
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
 )
 
+S3OnDeviceServiceConfigurationTypeDef = TypedDict(
+    "S3OnDeviceServiceConfigurationTypeDef",
+    {
+        "StorageLimit": float,
+        "StorageUnit": Literal["TB"],
+        "ServiceSize": int,
+        "FaultTolerance": int,
+    },
+    total=False,
+)
+
 TGWOnDeviceServiceConfigurationTypeDef = TypedDict(
     "TGWOnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
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
 TargetOnDeviceServiceTypeDef = TypedDict(
     "TargetOnDeviceServiceTypeDef",
     {
         "ServiceName": DeviceServiceNameType,
         "TransferOption": TransferOptionType,
     },
     total=False,
@@ -554,197 +701,81 @@
 CreateAddressRequestRequestTypeDef = TypedDict(
     "CreateAddressRequestRequestTypeDef",
     {
         "Address": AddressTypeDef,
     },
 )
 
-CreateAddressResultTypeDef = TypedDict(
-    "CreateAddressResultTypeDef",
-    {
-        "AddressId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateClusterResultTypeDef = TypedDict(
-    "CreateClusterResultTypeDef",
-    {
-        "ClusterId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobResultTypeDef = TypedDict(
-    "CreateJobResultTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLongTermPricingResultTypeDef = TypedDict(
-    "CreateLongTermPricingResultTypeDef",
-    {
-        "LongTermPricingId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateReturnShippingLabelResultTypeDef = TypedDict(
-    "CreateReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeAddressResultTypeDef = TypedDict(
     "DescribeAddressResultTypeDef",
     {
         "Address": AddressTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAddressesResultTypeDef = TypedDict(
     "DescribeAddressesResultTypeDef",
     {
         "Addresses": List[AddressTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeReturnShippingLabelResultTypeDef = TypedDict(
-    "DescribeReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ExpirationDate": datetime,
-        "ReturnShippingLabelURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetJobManifestResultTypeDef = TypedDict(
-    "GetJobManifestResultTypeDef",
-    {
-        "ManifestURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetJobUnlockCodeResultTypeDef = TypedDict(
-    "GetJobUnlockCodeResultTypeDef",
-    {
-        "UnlockCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSnowballUsageResultTypeDef = TypedDict(
-    "GetSnowballUsageResultTypeDef",
-    {
-        "SnowballLimit": int,
-        "SnowballsInUse": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSoftwareUpdatesResultTypeDef = TypedDict(
-    "GetSoftwareUpdatesResultTypeDef",
-    {
-        "UpdatesURI": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClustersResultTypeDef = TypedDict(
     "ListClustersResultTypeDef",
     {
         "ClusterListEntries": List[ClusterListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCompatibleImagesResultTypeDef = TypedDict(
     "ListCompatibleImagesResultTypeDef",
     {
         "CompatibleImages": List[CompatibleImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DependentServiceTypeDef = TypedDict(
-    "DependentServiceTypeDef",
-    {
-        "ServiceName": ServiceNameType,
-        "ServiceVersion": ServiceVersionTypeDef,
-    },
-    total=False,
-)
-
-DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
+CreateClusterResultTypeDef = TypedDict(
+    "CreateClusterResultTypeDef",
     {
         "ClusterId": str,
+        "JobListEntries": List[JobListEntryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
-    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
-):
-    pass
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
-ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
+ListClusterJobsResultTypeDef = TypedDict(
+    "ListClusterJobsResultTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "JobListEntries": List[JobListEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
+ListJobsResultTypeDef = TypedDict(
+    "ListJobsResultTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "JobListEntries": List[JobListEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
+DependentServiceTypeDef = TypedDict(
+    "DependentServiceTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ServiceName": ServiceNameType,
+        "ServiceVersion": ServiceVersionTypeDef,
     },
     total=False,
 )
 
 LambdaResourceTypeDef = TypedDict(
     "LambdaResourceTypeDef",
     {
@@ -758,47 +789,30 @@
     "TaxDocumentsTypeDef",
     {
         "IND": INDTaxDocumentsTypeDef,
     },
     total=False,
 )
 
-ListClusterJobsResultTypeDef = TypedDict(
-    "ListClusterJobsResultTypeDef",
-    {
-        "JobListEntries": List[JobListEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListJobsResultTypeDef = TypedDict(
-    "ListJobsResultTypeDef",
-    {
-        "JobListEntries": List[JobListEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListLongTermPricingResultTypeDef = TypedDict(
     "ListLongTermPricingResultTypeDef",
     {
         "LongTermPricingEntries": List[LongTermPricingListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OnDeviceServiceConfigurationTypeDef = TypedDict(
     "OnDeviceServiceConfigurationTypeDef",
     {
         "NFSOnDeviceService": NFSOnDeviceServiceConfigurationTypeDef,
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationTypeDef,
         "EKSOnDeviceService": EKSOnDeviceServiceConfigurationTypeDef,
+        "S3OnDeviceService": S3OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
 S3ResourceTypeDef = TypedDict(
     "S3ResourceTypeDef",
     {
@@ -852,15 +866,15 @@
 ListServiceVersionsResultTypeDef = TypedDict(
     "ListServiceVersionsResultTypeDef",
     {
         "ServiceVersions": List[ServiceVersionTypeDef],
         "ServiceName": ServiceNameType,
         "DependentServices": List[DependentServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JobResourceTypeDef = TypedDict(
     "JobResourceTypeDef",
     {
         "S3Resources": Sequence[S3ResourceTypeDef],
@@ -900,31 +914,35 @@
     total=False,
 )
 
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "JobType": JobTypeType,
-        "Resources": JobResourceTypeDef,
         "AddressId": str,
-        "RoleARN": str,
         "SnowballType": SnowballTypeType,
         "ShippingOption": ShippingOptionType,
     },
 )
 _OptionalCreateClusterRequestRequestTypeDef = TypedDict(
     "_OptionalCreateClusterRequestRequestTypeDef",
     {
+        "Resources": JobResourceTypeDef,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
         "Description": str,
         "KmsKeyARN": str,
+        "RoleARN": str,
         "Notification": NotificationTypeDef,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "RemoteManagement": RemoteManagementType,
+        "InitialClusterSize": int,
+        "ForceCreateJobs": bool,
+        "LongTermPricingIds": Sequence[str],
+        "SnowballCapacityPreference": SnowballCapacityType,
     },
     total=False,
 )
 
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
@@ -1036,19 +1054,19 @@
     total=False,
 )
 
 DescribeClusterResultTypeDef = TypedDict(
     "DescribeClusterResultTypeDef",
     {
         "ClusterMetadata": ClusterMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "JobMetadata": JobMetadataTypeDef,
         "SubJobMetadata": List[JobMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/PKG-INFO` & `mypy-boto3-snowball-1.27.0/mypy_boto3_snowball.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-snowball
-Version: 1.26.70
-Summary: Type annotations for boto3.Snowball 1.26.70 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Snowball 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-snowball"></a>
 
 # mypy-boto3-snowball
 
 [![PyPI - mypy-boto3-snowball](https://img.shields.io/pypi/v/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snowball.svg?color=blue)](https://pypi.org/project/mypy-boto3-snowball)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snowball?color=blue)](https://pypistats.org/packages/mypy-boto3-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Snowball 1.26.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
+[boto3.Snowball 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
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
 [mypy-boto3-snowball docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,74 +361,75 @@
 from mypy_boto3_snowball.type_defs import (
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
     NotificationTypeDef,
     CompatibleImageTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAddressResultTypeDef,
+    JobListEntryTypeDef,
+    CreateJobResultTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
+    CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
+    CreateReturnShippingLabelResultTypeDef,
     DataTransferTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
     DescribeAddressesRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeReturnShippingLabelRequestRequestTypeDef,
+    DescribeReturnShippingLabelResultTypeDef,
     EKSOnDeviceServiceConfigurationTypeDef,
     Ec2AmiResourceTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
+    GetJobManifestResultTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
+    GetJobUnlockCodeResultTypeDef,
+    GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
+    GetSoftwareUpdatesResultTypeDef,
     INDTaxDocumentsTypeDef,
-    JobListEntryTypeDef,
     JobLogsTypeDef,
     KeyRangeTypeDef,
+    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClusterJobsRequestRequestTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
+    S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
     CreateAddressRequestRequestTypeDef,
-    CreateAddressResultTypeDef,
-    CreateClusterResultTypeDef,
-    CreateJobResultTypeDef,
-    CreateLongTermPricingResultTypeDef,
-    CreateReturnShippingLabelResultTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
-    DescribeReturnShippingLabelResultTypeDef,
-    GetJobManifestResultTypeDef,
-    GetJobUnlockCodeResultTypeDef,
-    GetSnowballUsageResultTypeDef,
-    GetSoftwareUpdatesResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
+    CreateClusterResultTypeDef,
+    ListClusterJobsResultTypeDef,
+    ListJobsResultTypeDef,
     DependentServiceTypeDef,
-    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
-    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     LambdaResourceTypeDef,
     TaxDocumentsTypeDef,
-    ListClusterJobsResultTypeDef,
-    ListJobsResultTypeDef,
     ListLongTermPricingResultTypeDef,
     OnDeviceServiceConfigurationTypeDef,
     S3ResourceTypeDef,
     ShippingDetailsTypeDef,
     SnowconeDeviceConfigurationTypeDef,
     ListServiceVersionsRequestRequestTypeDef,
     ListServiceVersionsResultTypeDef,
@@ -452,42 +453,42 @@
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

### Comparing `mypy-boto3-snowball-1.26.70/mypy_boto3_snowball.egg-info/SOURCES.txt` & `mypy-boto3-snowball-1.27.0/mypy_boto3_snowball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snowball-1.26.70/setup.py` & `mypy-boto3-snowball-1.27.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-snowball.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-snowball",
-    version="1.26.70",
+    version="1.27.0",
     packages=["mypy_boto3_snowball"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Snowball 1.26.70 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.Snowball 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snowball/",
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


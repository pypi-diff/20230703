# Comparing `tmp/mypy-boto3-panorama-1.26.53.tar.gz` & `tmp/mypy-boto3-panorama-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-panorama-1.26.53.tar", last modified: Thu Jan 19 22:27:41 2023, max compression
+gzip compressed data, was "mypy-boto3-panorama-1.27.0.tar", last modified: Mon Jul  3 19:51:13 2023, max compression
```

## Comparing `mypy-boto3-panorama-1.26.53.tar` & `mypy-boto3-panorama-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:27:41.197141 mypy-boto3-panorama-1.26.53/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-19 22:27:08.000000 mypy-boto3-panorama-1.26.53/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-01-19 22:27:41.197141 mypy-boto3-panorama-1.26.53/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14952 2023-01-19 22:27:08.000000 mypy-boto3-panorama-1.26.53/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:27:41.197141 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-01-19 22:27:08.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-01-19 22:27:08.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-01-19 22:27:08.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23775 2023-01-19 22:27:08.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23734 2023-01-19 22:27:08.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10703 2023-01-19 22:27:08.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-01-19 22:27:08.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 22:27:08.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37298 2023-01-19 22:27:09.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37257 2023-01-19 22:27:09.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-19 22:27:08.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:27:41.197141 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-01-19 22:27:41.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-01-19 22:27:41.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 22:27:41.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 22:27:41.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-19 22:27:41.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-19 22:27:41.000000 mypy-boto3-panorama-1.26.53/mypy_boto3_panorama.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 22:27:41.197141 mypy-boto3-panorama-1.26.53/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-01-19 22:27:08.000000 mypy-boto3-panorama-1.26.53/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:13.267771 mypy-boto3-panorama-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:16.000000 mypy-boto3-panorama-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16420 2023-07-03 19:51:13.267771 mypy-boto3-panorama-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-07-03 19:43:16.000000 mypy-boto3-panorama-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:13.263771 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 19:43:16.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 19:43:16.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:43:16.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23775 2023-07-03 19:43:16.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23734 2023-07-03 19:43:16.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-07-03 19:43:16.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-07-03 19:43:16.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:16.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37354 2023-07-03 19:43:17.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37313 2023-07-03 19:43:16.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:16.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:13.267771 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16420 2023-07-03 19:51:13.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-03 19:51:13.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:13.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:13.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:13.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:13.000000 mypy-boto3-panorama-1.27.0/mypy_boto3_panorama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:13.267771 mypy-boto3-panorama-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:43:15.000000 mypy-boto3-panorama-1.27.0/setup.py
```

### Comparing `mypy-boto3-panorama-1.26.53/LICENSE` & `mypy-boto3-panorama-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-panorama-1.26.53/PKG-INFO` & `mypy-boto3-panorama-1.27.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-panorama
-Version: 1.26.53
-Summary: Type annotations for boto3.Panorama 1.26.53 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Panorama 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-panorama"></a>
 
 # mypy-boto3-panorama
 
 [![PyPI - mypy-boto3-panorama](https://img.shields.io/pypi/v/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-panorama?color=blue)](https://pypistats.org/packages/mypy-boto3-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Panorama 1.26.53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
+[boto3.Panorama 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [mypy-boto3-panorama docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,32 +324,37 @@
 
 ```python
 from mypy_boto3_panorama.type_defs import (
     AlternateSoftwareMetadataTypeDef,
     ReportedRuntimeContextStateTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
-    ResponseMetadataTypeDef,
+    CreateApplicationInstanceResponseTypeDef,
     JobTypeDef,
     JobResourceTagsTypeDef,
+    CreateNodeFromTemplateJobResponseTypeDef,
+    CreatePackageImportJobResponseTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
+    DeleteDeviceResponseTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
+    DescribeDeviceJobResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
     DescribeNodeRequestRequestTypeDef,
     DescribePackageImportJobRequestRequestTypeDef,
     DescribePackageRequestRequestTypeDef,
     DescribePackageVersionRequestRequestTypeDef,
+    DescribePackageVersionResponseTypeDef,
     OTAJobConfigTypeDef,
     DeviceJobTypeDef,
     StaticIpConnectionInfoTypeDef,
     EthernetStatusTypeDef,
     ListApplicationInstanceDependenciesRequestRequestTypeDef,
     PackageObjectTypeDef,
     ListApplicationInstanceNodeInstancesRequestRequestTypeDef,
@@ -362,41 +367,36 @@
     ListNodesRequestRequestTypeDef,
     NodeTypeDef,
     ListPackageImportJobsRequestRequestTypeDef,
     PackageImportJobTypeDef,
     ListPackagesRequestRequestTypeDef,
     PackageListItemTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NtpPayloadTypeDef,
     NtpStatusTypeDef,
     NodeInputPortTypeDef,
     NodeOutputPortTypeDef,
     NodeSignalTypeDef,
     OutPutS3LocationTypeDef,
     PackageVersionOutputConfigTypeDef,
     S3LocationTypeDef,
+    ProvisionDeviceResponseTypeDef,
     RegisterPackageVersionRequestRequestTypeDef,
     RemoveApplicationInstanceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    SignalApplicationInstanceNodeInstancesResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceMetadataRequestRequestTypeDef,
+    UpdateDeviceMetadataResponseTypeDef,
     ApplicationInstanceTypeDef,
+    DescribeApplicationInstanceResponseTypeDef,
     CreateApplicationInstanceRequestRequestTypeDef,
-    CreateApplicationInstanceResponseTypeDef,
-    CreateNodeFromTemplateJobResponseTypeDef,
-    CreatePackageImportJobResponseTypeDef,
-    DeleteDeviceResponseTypeDef,
     DescribeApplicationInstanceDetailsResponseTypeDef,
-    DescribeApplicationInstanceResponseTypeDef,
-    DescribeDeviceJobResponseTypeDef,
-    DescribePackageVersionResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ProvisionDeviceResponseTypeDef,
-    SignalApplicationInstanceNodeInstancesResponseTypeDef,
-    UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
     CreateNodeFromTemplateJobRequestRequestTypeDef,
     DescribeNodeFromTemplateJobResponseTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
     DeviceTypeDef,
     DeviceJobConfigTypeDef,
@@ -434,42 +434,42 @@
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

### Comparing `mypy-boto3-panorama-1.26.53/README.md` & `mypy-boto3-panorama-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-panorama"></a>
 
 # mypy-boto3-panorama
 
 [![PyPI - mypy-boto3-panorama](https://img.shields.io/pypi/v/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-panorama?color=blue)](https://pypistats.org/packages/mypy-boto3-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Panorama 1.26.53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
+[boto3.Panorama 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [mypy-boto3-panorama docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/).
 
 See how it helps to find and fix potential bugs:
 
@@ -292,32 +292,37 @@
 
 ```python
 from mypy_boto3_panorama.type_defs import (
     AlternateSoftwareMetadataTypeDef,
     ReportedRuntimeContextStateTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
-    ResponseMetadataTypeDef,
+    CreateApplicationInstanceResponseTypeDef,
     JobTypeDef,
     JobResourceTagsTypeDef,
+    CreateNodeFromTemplateJobResponseTypeDef,
+    CreatePackageImportJobResponseTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
+    DeleteDeviceResponseTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
+    DescribeDeviceJobResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
     DescribeNodeRequestRequestTypeDef,
     DescribePackageImportJobRequestRequestTypeDef,
     DescribePackageRequestRequestTypeDef,
     DescribePackageVersionRequestRequestTypeDef,
+    DescribePackageVersionResponseTypeDef,
     OTAJobConfigTypeDef,
     DeviceJobTypeDef,
     StaticIpConnectionInfoTypeDef,
     EthernetStatusTypeDef,
     ListApplicationInstanceDependenciesRequestRequestTypeDef,
     PackageObjectTypeDef,
     ListApplicationInstanceNodeInstancesRequestRequestTypeDef,
@@ -330,41 +335,36 @@
     ListNodesRequestRequestTypeDef,
     NodeTypeDef,
     ListPackageImportJobsRequestRequestTypeDef,
     PackageImportJobTypeDef,
     ListPackagesRequestRequestTypeDef,
     PackageListItemTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NtpPayloadTypeDef,
     NtpStatusTypeDef,
     NodeInputPortTypeDef,
     NodeOutputPortTypeDef,
     NodeSignalTypeDef,
     OutPutS3LocationTypeDef,
     PackageVersionOutputConfigTypeDef,
     S3LocationTypeDef,
+    ProvisionDeviceResponseTypeDef,
     RegisterPackageVersionRequestRequestTypeDef,
     RemoveApplicationInstanceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    SignalApplicationInstanceNodeInstancesResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceMetadataRequestRequestTypeDef,
+    UpdateDeviceMetadataResponseTypeDef,
     ApplicationInstanceTypeDef,
+    DescribeApplicationInstanceResponseTypeDef,
     CreateApplicationInstanceRequestRequestTypeDef,
-    CreateApplicationInstanceResponseTypeDef,
-    CreateNodeFromTemplateJobResponseTypeDef,
-    CreatePackageImportJobResponseTypeDef,
-    DeleteDeviceResponseTypeDef,
     DescribeApplicationInstanceDetailsResponseTypeDef,
-    DescribeApplicationInstanceResponseTypeDef,
-    DescribeDeviceJobResponseTypeDef,
-    DescribePackageVersionResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ProvisionDeviceResponseTypeDef,
-    SignalApplicationInstanceNodeInstancesResponseTypeDef,
-    UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
     CreateNodeFromTemplateJobRequestRequestTypeDef,
     DescribeNodeFromTemplateJobResponseTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
     DeviceTypeDef,
     DeviceJobConfigTypeDef,
@@ -402,42 +402,42 @@
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

### Comparing `mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/__main__.py` & `mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Panorama 1.26.53\nVersion:         1.26.53\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Panorama 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.53")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/client.py` & `mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/client.pyi` & `mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/literals.py` & `mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,14 +139,15 @@
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
@@ -178,21 +179,23 @@
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
@@ -271,14 +274,15 @@
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
@@ -289,14 +293,15 @@
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
@@ -332,14 +337,15 @@
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
@@ -358,16 +364,19 @@
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
@@ -447,18 +456,21 @@
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

### Comparing `mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/literals.pyi` & `mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,15 @@
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
@@ -176,21 +177,23 @@
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
@@ -269,14 +272,15 @@
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
@@ -287,14 +291,15 @@
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
@@ -330,14 +335,15 @@
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
@@ -356,16 +362,19 @@
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
@@ -445,18 +454,21 @@
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

### Comparing `mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/type_defs.py` & `mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,32 +53,37 @@
 
 
 __all__ = (
     "AlternateSoftwareMetadataTypeDef",
     "ReportedRuntimeContextStateTypeDef",
     "ManifestOverridesPayloadTypeDef",
     "ManifestPayloadTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateApplicationInstanceResponseTypeDef",
     "JobTypeDef",
     "JobResourceTagsTypeDef",
+    "CreateNodeFromTemplateJobResponseTypeDef",
+    "CreatePackageImportJobResponseTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "StorageLocationTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
+    "DeleteDeviceResponseTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeregisterPackageVersionRequestRequestTypeDef",
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     "DescribeApplicationInstanceRequestRequestTypeDef",
     "DescribeDeviceJobRequestRequestTypeDef",
+    "DescribeDeviceJobResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "LatestDeviceJobTypeDef",
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
     "DescribeNodeRequestRequestTypeDef",
     "DescribePackageImportJobRequestRequestTypeDef",
     "DescribePackageRequestRequestTypeDef",
     "DescribePackageVersionRequestRequestTypeDef",
+    "DescribePackageVersionResponseTypeDef",
     "OTAJobConfigTypeDef",
     "DeviceJobTypeDef",
     "StaticIpConnectionInfoTypeDef",
     "EthernetStatusTypeDef",
     "ListApplicationInstanceDependenciesRequestRequestTypeDef",
     "PackageObjectTypeDef",
     "ListApplicationInstanceNodeInstancesRequestRequestTypeDef",
@@ -91,41 +96,36 @@
     "ListNodesRequestRequestTypeDef",
     "NodeTypeDef",
     "ListPackageImportJobsRequestRequestTypeDef",
     "PackageImportJobTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "PackageListItemTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "NtpPayloadTypeDef",
     "NtpStatusTypeDef",
     "NodeInputPortTypeDef",
     "NodeOutputPortTypeDef",
     "NodeSignalTypeDef",
     "OutPutS3LocationTypeDef",
     "PackageVersionOutputConfigTypeDef",
     "S3LocationTypeDef",
+    "ProvisionDeviceResponseTypeDef",
     "RegisterPackageVersionRequestRequestTypeDef",
     "RemoveApplicationInstanceRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceMetadataRequestRequestTypeDef",
+    "UpdateDeviceMetadataResponseTypeDef",
     "ApplicationInstanceTypeDef",
+    "DescribeApplicationInstanceResponseTypeDef",
     "CreateApplicationInstanceRequestRequestTypeDef",
-    "CreateApplicationInstanceResponseTypeDef",
-    "CreateNodeFromTemplateJobResponseTypeDef",
-    "CreatePackageImportJobResponseTypeDef",
-    "DeleteDeviceResponseTypeDef",
     "DescribeApplicationInstanceDetailsResponseTypeDef",
-    "DescribeApplicationInstanceResponseTypeDef",
-    "DescribeDeviceJobResponseTypeDef",
-    "DescribePackageVersionResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ProvisionDeviceResponseTypeDef",
-    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
-    "UpdateDeviceMetadataResponseTypeDef",
     "CreateJobForDevicesResponseTypeDef",
     "CreateNodeFromTemplateJobRequestRequestTypeDef",
     "DescribeNodeFromTemplateJobResponseTypeDef",
     "CreatePackageResponseTypeDef",
     "DescribePackageResponseTypeDef",
     "DeviceTypeDef",
     "DeviceJobConfigTypeDef",
@@ -185,22 +185,19 @@
     "ManifestPayloadTypeDef",
     {
         "PayloadData": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateApplicationInstanceResponseTypeDef = TypedDict(
+    "CreateApplicationInstanceResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ApplicationInstanceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "DeviceId": str,
@@ -213,14 +210,30 @@
     "JobResourceTagsTypeDef",
     {
         "ResourceType": Literal["PACKAGE"],
         "Tags": Mapping[str, str],
     },
 )
 
+CreateNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "CreateNodeFromTemplateJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePackageImportJobResponseTypeDef = TypedDict(
+    "CreatePackageImportJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageRequestRequestTypeDef",
     {
         "PackageName": str,
     },
 )
 _OptionalCreatePackageRequestRequestTypeDef = TypedDict(
@@ -252,14 +265,22 @@
 DeleteDeviceRequestRequestTypeDef = TypedDict(
     "DeleteDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
+DeleteDeviceResponseTypeDef = TypedDict(
+    "DeleteDeviceResponseTypeDef",
+    {
+        "DeviceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeletePackageRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePackageRequestRequestTypeDef",
     {
         "PackageId": str,
     },
 )
 _OptionalDeletePackageRequestRequestTypeDef = TypedDict(
@@ -319,14 +340,30 @@
 DescribeDeviceJobRequestRequestTypeDef = TypedDict(
     "DescribeDeviceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+DescribeDeviceJobResponseTypeDef = TypedDict(
+    "DescribeDeviceJobResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "DeviceArn": str,
+        "DeviceId": str,
+        "DeviceName": str,
+        "DeviceType": DeviceTypeType,
+        "ImageVersion": str,
+        "JobId": str,
+        "JobType": JobTypeType,
+        "Status": UpdateProgressType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
@@ -402,14 +439,31 @@
 class DescribePackageVersionRequestRequestTypeDef(
     _RequiredDescribePackageVersionRequestRequestTypeDef,
     _OptionalDescribePackageVersionRequestRequestTypeDef,
 ):
     pass
 
 
+DescribePackageVersionResponseTypeDef = TypedDict(
+    "DescribePackageVersionResponseTypeDef",
+    {
+        "IsLatestPatch": bool,
+        "OwnerAccount": str,
+        "PackageArn": str,
+        "PackageId": str,
+        "PackageName": str,
+        "PackageVersion": str,
+        "PatchVersion": str,
+        "RegisteredTime": datetime,
+        "Status": PackageVersionStatusType,
+        "StatusDescription": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredOTAJobConfigTypeDef = TypedDict(
     "_RequiredOTAJobConfigTypeDef",
     {
         "ImageVersion": str,
     },
 )
 _OptionalOTAJobConfigTypeDef = TypedDict(
@@ -680,14 +734,22 @@
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
 NtpPayloadTypeDef = TypedDict(
     "NtpPayloadTypeDef",
     {
         "NtpServers": List[str],
     },
 )
 
@@ -777,14 +839,26 @@
 )
 
 
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
 
+ProvisionDeviceResponseTypeDef = TypedDict(
+    "ProvisionDeviceResponseTypeDef",
+    {
+        "Arn": str,
+        "Certificates": bytes,
+        "DeviceId": str,
+        "IotThingName": str,
+        "Status": DeviceStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRegisterPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterPackageVersionRequestRequestTypeDef",
     {
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -809,14 +883,33 @@
 RemoveApplicationInstanceRequestRequestTypeDef = TypedDict(
     "RemoveApplicationInstanceRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
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
+SignalApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
+    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -847,14 +940,22 @@
 class UpdateDeviceMetadataRequestRequestTypeDef(
     _RequiredUpdateDeviceMetadataRequestRequestTypeDef,
     _OptionalUpdateDeviceMetadataRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateDeviceMetadataResponseTypeDef = TypedDict(
+    "UpdateDeviceMetadataResponseTypeDef",
+    {
+        "DeviceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ApplicationInstanceTypeDef = TypedDict(
     "ApplicationInstanceTypeDef",
     {
         "ApplicationInstanceId": str,
         "Arn": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
@@ -866,14 +967,36 @@
         "Status": ApplicationInstanceStatusType,
         "StatusDescription": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+DescribeApplicationInstanceResponseTypeDef = TypedDict(
+    "DescribeApplicationInstanceResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ApplicationInstanceIdToReplace": str,
+        "Arn": str,
+        "CreatedTime": datetime,
+        "DefaultRuntimeContextDevice": str,
+        "DefaultRuntimeContextDeviceName": str,
+        "Description": str,
+        "HealthStatus": ApplicationInstanceHealthStatusType,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "RuntimeContextStates": List[ReportedRuntimeContextStateTypeDef],
+        "RuntimeRoleArn": str,
+        "Status": ApplicationInstanceStatusType,
+        "StatusDescription": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateApplicationInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationInstanceRequestRequestTypeDef",
     {
         "DefaultRuntimeContextDevice": str,
         "ManifestPayload": ManifestPayloadTypeDef,
     },
 )
@@ -894,157 +1017,34 @@
 class CreateApplicationInstanceRequestRequestTypeDef(
     _RequiredCreateApplicationInstanceRequestRequestTypeDef,
     _OptionalCreateApplicationInstanceRequestRequestTypeDef,
 ):
     pass
 
 
-CreateApplicationInstanceResponseTypeDef = TypedDict(
-    "CreateApplicationInstanceResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "CreateNodeFromTemplateJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePackageImportJobResponseTypeDef = TypedDict(
-    "CreatePackageImportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDeviceResponseTypeDef = TypedDict(
-    "DeleteDeviceResponseTypeDef",
-    {
-        "DeviceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeApplicationInstanceDetailsResponseTypeDef = TypedDict(
     "DescribeApplicationInstanceDetailsResponseTypeDef",
     {
         "ApplicationInstanceId": str,
         "ApplicationInstanceIdToReplace": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
         "Description": str,
         "ManifestOverridesPayload": ManifestOverridesPayloadTypeDef,
         "ManifestPayload": ManifestPayloadTypeDef,
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeApplicationInstanceResponseTypeDef = TypedDict(
-    "DescribeApplicationInstanceResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ApplicationInstanceIdToReplace": str,
-        "Arn": str,
-        "CreatedTime": datetime,
-        "DefaultRuntimeContextDevice": str,
-        "DefaultRuntimeContextDeviceName": str,
-        "Description": str,
-        "HealthStatus": ApplicationInstanceHealthStatusType,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "RuntimeContextStates": List[ReportedRuntimeContextStateTypeDef],
-        "RuntimeRoleArn": str,
-        "Status": ApplicationInstanceStatusType,
-        "StatusDescription": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDeviceJobResponseTypeDef = TypedDict(
-    "DescribeDeviceJobResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "DeviceArn": str,
-        "DeviceId": str,
-        "DeviceName": str,
-        "DeviceType": DeviceTypeType,
-        "ImageVersion": str,
-        "JobId": str,
-        "JobType": JobTypeType,
-        "Status": UpdateProgressType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribePackageVersionResponseTypeDef = TypedDict(
-    "DescribePackageVersionResponseTypeDef",
-    {
-        "IsLatestPatch": bool,
-        "OwnerAccount": str,
-        "PackageArn": str,
-        "PackageId": str,
-        "PackageName": str,
-        "PackageVersion": str,
-        "PatchVersion": str,
-        "RegisteredTime": datetime,
-        "Status": PackageVersionStatusType,
-        "StatusDescription": str,
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
-ProvisionDeviceResponseTypeDef = TypedDict(
-    "ProvisionDeviceResponseTypeDef",
-    {
-        "Arn": str,
-        "Certificates": bytes,
-        "DeviceId": str,
-        "IotThingName": str,
-        "Status": DeviceStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SignalApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
-    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDeviceMetadataResponseTypeDef = TypedDict(
-    "UpdateDeviceMetadataResponseTypeDef",
-    {
-        "DeviceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateJobForDevicesResponseTypeDef = TypedDict(
     "CreateJobForDevicesResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
     {
         "NodeName": str,
@@ -1082,40 +1082,40 @@
         "NodeName": str,
         "OutputPackageName": str,
         "OutputPackageVersion": str,
         "Status": NodeFromTemplateJobStatusType,
         "StatusMessage": str,
         "TemplateParameters": Dict[str, str],
         "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "Arn": str,
         "PackageId": str,
         "StorageLocation": StorageLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackageResponseTypeDef = TypedDict(
     "DescribePackageResponseTypeDef",
     {
         "Arn": str,
         "CreatedTime": datetime,
         "PackageId": str,
         "PackageName": str,
         "ReadAccessPrincipalArns": List[str],
         "StorageLocation": StorageLocationTypeDef,
         "Tags": Dict[str, str],
         "WriteAccessPrincipalArns": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
         "Brand": DeviceBrandType,
@@ -1144,15 +1144,15 @@
 )
 
 ListDevicesJobsResponseTypeDef = TypedDict(
     "ListDevicesJobsResponseTypeDef",
     {
         "DeviceJobs": List[DeviceJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEthernetPayloadTypeDef = TypedDict(
     "_RequiredEthernetPayloadTypeDef",
     {
         "ConnectionType": ConnectionTypeType,
@@ -1172,60 +1172,60 @@
 
 
 ListApplicationInstanceDependenciesResponseTypeDef = TypedDict(
     "ListApplicationInstanceDependenciesResponseTypeDef",
     {
         "NextToken": str,
         "PackageObjects": List[PackageObjectTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     {
         "NextToken": str,
         "NodeInstances": List[NodeInstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNodeFromTemplateJobsResponseTypeDef = TypedDict(
     "ListNodeFromTemplateJobsResponseTypeDef",
     {
         "NextToken": str,
         "NodeFromTemplateJobs": List[NodeFromTemplateJobTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNodesResponseTypeDef = TypedDict(
     "ListNodesResponseTypeDef",
     {
         "NextToken": str,
         "Nodes": List[NodeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPackageImportJobsResponseTypeDef = TypedDict(
     "ListPackageImportJobsResponseTypeDef",
     {
         "NextToken": str,
         "PackageImportJobs": List[PackageImportJobTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPackagesResponseTypeDef = TypedDict(
     "ListPackagesResponseTypeDef",
     {
         "NextToken": str,
         "Packages": List[PackageListItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NetworkStatusTypeDef = TypedDict(
     "NetworkStatusTypeDef",
     {
         "Ethernet0Status": EthernetStatusTypeDef,
@@ -1278,24 +1278,24 @@
 )
 
 ListApplicationInstancesResponseTypeDef = TypedDict(
     "ListApplicationInstancesResponseTypeDef",
     {
         "ApplicationInstances": List[ApplicationInstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateJobForDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobForDevicesRequestRequestTypeDef",
     {
         "DeviceIds": Sequence[str],
@@ -1341,15 +1341,15 @@
         "NodeInterface": NodeInterfaceTypeDef,
         "OwnerAccount": str,
         "PackageArn": str,
         "PackageId": str,
         "PackageName": str,
         "PackageVersion": str,
         "PatchVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PackageImportJobInputConfigTypeDef = TypedDict(
     "PackageImportJobInputConfigTypeDef",
     {
         "PackageVersionInputConfig": PackageVersionInputConfigTypeDef,
@@ -1376,15 +1376,15 @@
         "LeaseExpirationTime": datetime,
         "Name": str,
         "NetworkingConfiguration": NetworkPayloadTypeDef,
         "ProvisioningStatus": DeviceStatusType,
         "SerialNumber": str,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredProvisionDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionDeviceRequestRequestTypeDef",
     {
         "Name": str,
@@ -1442,10 +1442,10 @@
         "JobTags": List[JobResourceTagsTypeDef],
         "JobType": PackageImportJobTypeType,
         "LastUpdatedTime": datetime,
         "Output": PackageImportJobOutputTypeDef,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
         "Status": PackageImportJobStatusType,
         "StatusMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-panorama-1.26.53/mypy_boto3_panorama/type_defs.pyi` & `mypy-boto3-panorama-1.27.0/mypy_boto3_panorama/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -52,32 +52,37 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlternateSoftwareMetadataTypeDef",
     "ReportedRuntimeContextStateTypeDef",
     "ManifestOverridesPayloadTypeDef",
     "ManifestPayloadTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateApplicationInstanceResponseTypeDef",
     "JobTypeDef",
     "JobResourceTagsTypeDef",
+    "CreateNodeFromTemplateJobResponseTypeDef",
+    "CreatePackageImportJobResponseTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "StorageLocationTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
+    "DeleteDeviceResponseTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeregisterPackageVersionRequestRequestTypeDef",
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     "DescribeApplicationInstanceRequestRequestTypeDef",
     "DescribeDeviceJobRequestRequestTypeDef",
+    "DescribeDeviceJobResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "LatestDeviceJobTypeDef",
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
     "DescribeNodeRequestRequestTypeDef",
     "DescribePackageImportJobRequestRequestTypeDef",
     "DescribePackageRequestRequestTypeDef",
     "DescribePackageVersionRequestRequestTypeDef",
+    "DescribePackageVersionResponseTypeDef",
     "OTAJobConfigTypeDef",
     "DeviceJobTypeDef",
     "StaticIpConnectionInfoTypeDef",
     "EthernetStatusTypeDef",
     "ListApplicationInstanceDependenciesRequestRequestTypeDef",
     "PackageObjectTypeDef",
     "ListApplicationInstanceNodeInstancesRequestRequestTypeDef",
@@ -90,41 +95,36 @@
     "ListNodesRequestRequestTypeDef",
     "NodeTypeDef",
     "ListPackageImportJobsRequestRequestTypeDef",
     "PackageImportJobTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "PackageListItemTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "NtpPayloadTypeDef",
     "NtpStatusTypeDef",
     "NodeInputPortTypeDef",
     "NodeOutputPortTypeDef",
     "NodeSignalTypeDef",
     "OutPutS3LocationTypeDef",
     "PackageVersionOutputConfigTypeDef",
     "S3LocationTypeDef",
+    "ProvisionDeviceResponseTypeDef",
     "RegisterPackageVersionRequestRequestTypeDef",
     "RemoveApplicationInstanceRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceMetadataRequestRequestTypeDef",
+    "UpdateDeviceMetadataResponseTypeDef",
     "ApplicationInstanceTypeDef",
+    "DescribeApplicationInstanceResponseTypeDef",
     "CreateApplicationInstanceRequestRequestTypeDef",
-    "CreateApplicationInstanceResponseTypeDef",
-    "CreateNodeFromTemplateJobResponseTypeDef",
-    "CreatePackageImportJobResponseTypeDef",
-    "DeleteDeviceResponseTypeDef",
     "DescribeApplicationInstanceDetailsResponseTypeDef",
-    "DescribeApplicationInstanceResponseTypeDef",
-    "DescribeDeviceJobResponseTypeDef",
-    "DescribePackageVersionResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ProvisionDeviceResponseTypeDef",
-    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
-    "UpdateDeviceMetadataResponseTypeDef",
     "CreateJobForDevicesResponseTypeDef",
     "CreateNodeFromTemplateJobRequestRequestTypeDef",
     "DescribeNodeFromTemplateJobResponseTypeDef",
     "CreatePackageResponseTypeDef",
     "DescribePackageResponseTypeDef",
     "DeviceTypeDef",
     "DeviceJobConfigTypeDef",
@@ -184,22 +184,19 @@
     "ManifestPayloadTypeDef",
     {
         "PayloadData": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateApplicationInstanceResponseTypeDef = TypedDict(
+    "CreateApplicationInstanceResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ApplicationInstanceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "DeviceId": str,
@@ -212,14 +209,30 @@
     "JobResourceTagsTypeDef",
     {
         "ResourceType": Literal["PACKAGE"],
         "Tags": Mapping[str, str],
     },
 )
 
+CreateNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "CreateNodeFromTemplateJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePackageImportJobResponseTypeDef = TypedDict(
+    "CreatePackageImportJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageRequestRequestTypeDef",
     {
         "PackageName": str,
     },
 )
 _OptionalCreatePackageRequestRequestTypeDef = TypedDict(
@@ -249,14 +262,22 @@
 DeleteDeviceRequestRequestTypeDef = TypedDict(
     "DeleteDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
+DeleteDeviceResponseTypeDef = TypedDict(
+    "DeleteDeviceResponseTypeDef",
+    {
+        "DeviceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeletePackageRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePackageRequestRequestTypeDef",
     {
         "PackageId": str,
     },
 )
 _OptionalDeletePackageRequestRequestTypeDef = TypedDict(
@@ -312,14 +333,30 @@
 DescribeDeviceJobRequestRequestTypeDef = TypedDict(
     "DescribeDeviceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+DescribeDeviceJobResponseTypeDef = TypedDict(
+    "DescribeDeviceJobResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "DeviceArn": str,
+        "DeviceId": str,
+        "DeviceName": str,
+        "DeviceType": DeviceTypeType,
+        "ImageVersion": str,
+        "JobId": str,
+        "JobType": JobTypeType,
+        "Status": UpdateProgressType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
@@ -391,14 +428,31 @@
 
 class DescribePackageVersionRequestRequestTypeDef(
     _RequiredDescribePackageVersionRequestRequestTypeDef,
     _OptionalDescribePackageVersionRequestRequestTypeDef,
 ):
     pass
 
+DescribePackageVersionResponseTypeDef = TypedDict(
+    "DescribePackageVersionResponseTypeDef",
+    {
+        "IsLatestPatch": bool,
+        "OwnerAccount": str,
+        "PackageArn": str,
+        "PackageId": str,
+        "PackageName": str,
+        "PackageVersion": str,
+        "PatchVersion": str,
+        "RegisteredTime": datetime,
+        "Status": PackageVersionStatusType,
+        "StatusDescription": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredOTAJobConfigTypeDef = TypedDict(
     "_RequiredOTAJobConfigTypeDef",
     {
         "ImageVersion": str,
     },
 )
 _OptionalOTAJobConfigTypeDef = TypedDict(
@@ -659,14 +713,22 @@
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
 NtpPayloadTypeDef = TypedDict(
     "NtpPayloadTypeDef",
     {
         "NtpServers": List[str],
     },
 )
 
@@ -752,14 +814,26 @@
     },
     total=False,
 )
 
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
+ProvisionDeviceResponseTypeDef = TypedDict(
+    "ProvisionDeviceResponseTypeDef",
+    {
+        "Arn": str,
+        "Certificates": bytes,
+        "DeviceId": str,
+        "IotThingName": str,
+        "Status": DeviceStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRegisterPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterPackageVersionRequestRequestTypeDef",
     {
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -782,14 +856,33 @@
 RemoveApplicationInstanceRequestRequestTypeDef = TypedDict(
     "RemoveApplicationInstanceRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
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
+SignalApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
+    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -818,14 +911,22 @@
 
 class UpdateDeviceMetadataRequestRequestTypeDef(
     _RequiredUpdateDeviceMetadataRequestRequestTypeDef,
     _OptionalUpdateDeviceMetadataRequestRequestTypeDef,
 ):
     pass
 
+UpdateDeviceMetadataResponseTypeDef = TypedDict(
+    "UpdateDeviceMetadataResponseTypeDef",
+    {
+        "DeviceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ApplicationInstanceTypeDef = TypedDict(
     "ApplicationInstanceTypeDef",
     {
         "ApplicationInstanceId": str,
         "Arn": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
@@ -837,14 +938,36 @@
         "Status": ApplicationInstanceStatusType,
         "StatusDescription": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+DescribeApplicationInstanceResponseTypeDef = TypedDict(
+    "DescribeApplicationInstanceResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ApplicationInstanceIdToReplace": str,
+        "Arn": str,
+        "CreatedTime": datetime,
+        "DefaultRuntimeContextDevice": str,
+        "DefaultRuntimeContextDeviceName": str,
+        "Description": str,
+        "HealthStatus": ApplicationInstanceHealthStatusType,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "RuntimeContextStates": List[ReportedRuntimeContextStateTypeDef],
+        "RuntimeRoleArn": str,
+        "Status": ApplicationInstanceStatusType,
+        "StatusDescription": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateApplicationInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationInstanceRequestRequestTypeDef",
     {
         "DefaultRuntimeContextDevice": str,
         "ManifestPayload": ManifestPayloadTypeDef,
     },
 )
@@ -863,157 +986,34 @@
 
 class CreateApplicationInstanceRequestRequestTypeDef(
     _RequiredCreateApplicationInstanceRequestRequestTypeDef,
     _OptionalCreateApplicationInstanceRequestRequestTypeDef,
 ):
     pass
 
-CreateApplicationInstanceResponseTypeDef = TypedDict(
-    "CreateApplicationInstanceResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "CreateNodeFromTemplateJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePackageImportJobResponseTypeDef = TypedDict(
-    "CreatePackageImportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDeviceResponseTypeDef = TypedDict(
-    "DeleteDeviceResponseTypeDef",
-    {
-        "DeviceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeApplicationInstanceDetailsResponseTypeDef = TypedDict(
     "DescribeApplicationInstanceDetailsResponseTypeDef",
     {
         "ApplicationInstanceId": str,
         "ApplicationInstanceIdToReplace": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
         "Description": str,
         "ManifestOverridesPayload": ManifestOverridesPayloadTypeDef,
         "ManifestPayload": ManifestPayloadTypeDef,
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeApplicationInstanceResponseTypeDef = TypedDict(
-    "DescribeApplicationInstanceResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ApplicationInstanceIdToReplace": str,
-        "Arn": str,
-        "CreatedTime": datetime,
-        "DefaultRuntimeContextDevice": str,
-        "DefaultRuntimeContextDeviceName": str,
-        "Description": str,
-        "HealthStatus": ApplicationInstanceHealthStatusType,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "RuntimeContextStates": List[ReportedRuntimeContextStateTypeDef],
-        "RuntimeRoleArn": str,
-        "Status": ApplicationInstanceStatusType,
-        "StatusDescription": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDeviceJobResponseTypeDef = TypedDict(
-    "DescribeDeviceJobResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "DeviceArn": str,
-        "DeviceId": str,
-        "DeviceName": str,
-        "DeviceType": DeviceTypeType,
-        "ImageVersion": str,
-        "JobId": str,
-        "JobType": JobTypeType,
-        "Status": UpdateProgressType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribePackageVersionResponseTypeDef = TypedDict(
-    "DescribePackageVersionResponseTypeDef",
-    {
-        "IsLatestPatch": bool,
-        "OwnerAccount": str,
-        "PackageArn": str,
-        "PackageId": str,
-        "PackageName": str,
-        "PackageVersion": str,
-        "PatchVersion": str,
-        "RegisteredTime": datetime,
-        "Status": PackageVersionStatusType,
-        "StatusDescription": str,
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
-ProvisionDeviceResponseTypeDef = TypedDict(
-    "ProvisionDeviceResponseTypeDef",
-    {
-        "Arn": str,
-        "Certificates": bytes,
-        "DeviceId": str,
-        "IotThingName": str,
-        "Status": DeviceStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SignalApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
-    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDeviceMetadataResponseTypeDef = TypedDict(
-    "UpdateDeviceMetadataResponseTypeDef",
-    {
-        "DeviceId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateJobForDevicesResponseTypeDef = TypedDict(
     "CreateJobForDevicesResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
     {
         "NodeName": str,
@@ -1049,40 +1049,40 @@
         "NodeName": str,
         "OutputPackageName": str,
         "OutputPackageVersion": str,
         "Status": NodeFromTemplateJobStatusType,
         "StatusMessage": str,
         "TemplateParameters": Dict[str, str],
         "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "Arn": str,
         "PackageId": str,
         "StorageLocation": StorageLocationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackageResponseTypeDef = TypedDict(
     "DescribePackageResponseTypeDef",
     {
         "Arn": str,
         "CreatedTime": datetime,
         "PackageId": str,
         "PackageName": str,
         "ReadAccessPrincipalArns": List[str],
         "StorageLocation": StorageLocationTypeDef,
         "Tags": Dict[str, str],
         "WriteAccessPrincipalArns": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
         "Brand": DeviceBrandType,
@@ -1111,15 +1111,15 @@
 )
 
 ListDevicesJobsResponseTypeDef = TypedDict(
     "ListDevicesJobsResponseTypeDef",
     {
         "DeviceJobs": List[DeviceJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEthernetPayloadTypeDef = TypedDict(
     "_RequiredEthernetPayloadTypeDef",
     {
         "ConnectionType": ConnectionTypeType,
@@ -1137,60 +1137,60 @@
     pass
 
 ListApplicationInstanceDependenciesResponseTypeDef = TypedDict(
     "ListApplicationInstanceDependenciesResponseTypeDef",
     {
         "NextToken": str,
         "PackageObjects": List[PackageObjectTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     {
         "NextToken": str,
         "NodeInstances": List[NodeInstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNodeFromTemplateJobsResponseTypeDef = TypedDict(
     "ListNodeFromTemplateJobsResponseTypeDef",
     {
         "NextToken": str,
         "NodeFromTemplateJobs": List[NodeFromTemplateJobTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListNodesResponseTypeDef = TypedDict(
     "ListNodesResponseTypeDef",
     {
         "NextToken": str,
         "Nodes": List[NodeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPackageImportJobsResponseTypeDef = TypedDict(
     "ListPackageImportJobsResponseTypeDef",
     {
         "NextToken": str,
         "PackageImportJobs": List[PackageImportJobTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPackagesResponseTypeDef = TypedDict(
     "ListPackagesResponseTypeDef",
     {
         "NextToken": str,
         "Packages": List[PackageListItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NetworkStatusTypeDef = TypedDict(
     "NetworkStatusTypeDef",
     {
         "Ethernet0Status": EthernetStatusTypeDef,
@@ -1243,24 +1243,24 @@
 )
 
 ListApplicationInstancesResponseTypeDef = TypedDict(
     "ListApplicationInstancesResponseTypeDef",
     {
         "ApplicationInstances": List[ApplicationInstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateJobForDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobForDevicesRequestRequestTypeDef",
     {
         "DeviceIds": Sequence[str],
@@ -1304,15 +1304,15 @@
         "NodeInterface": NodeInterfaceTypeDef,
         "OwnerAccount": str,
         "PackageArn": str,
         "PackageId": str,
         "PackageName": str,
         "PackageVersion": str,
         "PatchVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PackageImportJobInputConfigTypeDef = TypedDict(
     "PackageImportJobInputConfigTypeDef",
     {
         "PackageVersionInputConfig": PackageVersionInputConfigTypeDef,
@@ -1339,15 +1339,15 @@
         "LeaseExpirationTime": datetime,
         "Name": str,
         "NetworkingConfiguration": NetworkPayloadTypeDef,
         "ProvisioningStatus": DeviceStatusType,
         "SerialNumber": str,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredProvisionDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionDeviceRequestRequestTypeDef",
     {
         "Name": str,
@@ -1401,10 +1401,10 @@
         "JobTags": List[JobResourceTagsTypeDef],
         "JobType": PackageImportJobTypeType,
         "LastUpdatedTime": datetime,
         "Output": PackageImportJobOutputTypeDef,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
         "Status": PackageImportJobStatusType,
         "StatusMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-panorama-1.26.53/mypy_boto3_panorama.egg-info/PKG-INFO` & `mypy-boto3-panorama-1.27.0/mypy_boto3_panorama.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-panorama
-Version: 1.26.53
-Summary: Type annotations for boto3.Panorama 1.26.53 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Panorama 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-panorama"></a>
 
 # mypy-boto3-panorama
 
 [![PyPI - mypy-boto3-panorama](https://img.shields.io/pypi/v/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-panorama?color=blue)](https://pypistats.org/packages/mypy-boto3-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Panorama 1.26.53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
+[boto3.Panorama 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [mypy-boto3-panorama docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,32 +324,37 @@
 
 ```python
 from mypy_boto3_panorama.type_defs import (
     AlternateSoftwareMetadataTypeDef,
     ReportedRuntimeContextStateTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
-    ResponseMetadataTypeDef,
+    CreateApplicationInstanceResponseTypeDef,
     JobTypeDef,
     JobResourceTagsTypeDef,
+    CreateNodeFromTemplateJobResponseTypeDef,
+    CreatePackageImportJobResponseTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
+    DeleteDeviceResponseTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
+    DescribeDeviceJobResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
     DescribeNodeRequestRequestTypeDef,
     DescribePackageImportJobRequestRequestTypeDef,
     DescribePackageRequestRequestTypeDef,
     DescribePackageVersionRequestRequestTypeDef,
+    DescribePackageVersionResponseTypeDef,
     OTAJobConfigTypeDef,
     DeviceJobTypeDef,
     StaticIpConnectionInfoTypeDef,
     EthernetStatusTypeDef,
     ListApplicationInstanceDependenciesRequestRequestTypeDef,
     PackageObjectTypeDef,
     ListApplicationInstanceNodeInstancesRequestRequestTypeDef,
@@ -362,41 +367,36 @@
     ListNodesRequestRequestTypeDef,
     NodeTypeDef,
     ListPackageImportJobsRequestRequestTypeDef,
     PackageImportJobTypeDef,
     ListPackagesRequestRequestTypeDef,
     PackageListItemTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NtpPayloadTypeDef,
     NtpStatusTypeDef,
     NodeInputPortTypeDef,
     NodeOutputPortTypeDef,
     NodeSignalTypeDef,
     OutPutS3LocationTypeDef,
     PackageVersionOutputConfigTypeDef,
     S3LocationTypeDef,
+    ProvisionDeviceResponseTypeDef,
     RegisterPackageVersionRequestRequestTypeDef,
     RemoveApplicationInstanceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    SignalApplicationInstanceNodeInstancesResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceMetadataRequestRequestTypeDef,
+    UpdateDeviceMetadataResponseTypeDef,
     ApplicationInstanceTypeDef,
+    DescribeApplicationInstanceResponseTypeDef,
     CreateApplicationInstanceRequestRequestTypeDef,
-    CreateApplicationInstanceResponseTypeDef,
-    CreateNodeFromTemplateJobResponseTypeDef,
-    CreatePackageImportJobResponseTypeDef,
-    DeleteDeviceResponseTypeDef,
     DescribeApplicationInstanceDetailsResponseTypeDef,
-    DescribeApplicationInstanceResponseTypeDef,
-    DescribeDeviceJobResponseTypeDef,
-    DescribePackageVersionResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ProvisionDeviceResponseTypeDef,
-    SignalApplicationInstanceNodeInstancesResponseTypeDef,
-    UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
     CreateNodeFromTemplateJobRequestRequestTypeDef,
     DescribeNodeFromTemplateJobResponseTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
     DeviceTypeDef,
     DeviceJobConfigTypeDef,
@@ -434,42 +434,42 @@
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

### Comparing `mypy-boto3-panorama-1.26.53/mypy_boto3_panorama.egg-info/SOURCES.txt` & `mypy-boto3-panorama-1.27.0/mypy_boto3_panorama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.26.53/setup.py` & `mypy-boto3-panorama-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-panorama.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-panorama",
-    version="1.26.53",
+    version="1.27.0",
     packages=["mypy_boto3_panorama"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Panorama 1.26.53 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.Panorama 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/",
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


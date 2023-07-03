# Comparing `tmp/mypy-boto3-snow-device-management-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-snow-device-management-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-snow-device-management-1.26.0.post1.tar", last modified: Tue Nov  1 21:44:01 2022, max compression
+gzip compressed data, was "mypy-boto3-snow-device-management-1.27.0.tar", last modified: Mon Jul  3 19:51:29 2023, max compression
```

## Comparing `mypy-boto3-snow-device-management-1.26.0.post1.tar` & `mypy-boto3-snow-device-management-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:01.532851 mypy-boto3-snow-device-management-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:41:32.000000 mypy-boto3-snow-device-management-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15482 2022-11-01 21:44:01.532851 mypy-boto3-snow-device-management-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13983 2022-11-01 21:41:31.000000 mypy-boto3-snow-device-management-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:01.528851 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-11-01 21:41:32.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-11-01 21:41:32.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-11-01 21:41:32.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13520 2022-11-01 21:41:32.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    13496 2022-11-01 21:41:32.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8145 2022-11-01 21:41:32.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8143 2022-11-01 21:41:32.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5518 2022-11-01 21:41:32.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5512 2022-11-01 21:41:32.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:41:32.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    14737 2022-11-01 21:41:32.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    14722 2022-11-01 21:41:32.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:41:32.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:01.532851 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15482 2022-11-01 21:44:01.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-11-01 21:44:01.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:01.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:01.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:44:01.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-01 21:44:01.000000 mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:44:01.532851 mypy-boto3-snow-device-management-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-11-01 21:41:31.000000 mypy-boto3-snow-device-management-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:29.232028 mypy-boto3-snow-device-management-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:17.000000 mypy-boto3-snow-device-management-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-07-03 19:51:29.228028 mypy-boto3-snow-device-management-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-07-03 19:48:17.000000 mypy-boto3-snow-device-management-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:29.224028 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-03 19:48:17.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-03 19:48:17.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-03 19:48:17.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-07-03 19:48:17.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-07-03 19:48:17.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-07-03 19:48:18.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-07-03 19:48:17.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-03 19:48:17.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-03 19:48:17.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:17.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14769 2023-07-03 19:48:18.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-07-03 19:48:18.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:17.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:29.228028 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-07-03 19:51:29.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-03 19:51:29.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:29.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:29.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:29.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-03 19:51:29.000000 mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:29.232028 mypy-boto3-snow-device-management-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-03 19:48:17.000000 mypy-boto3-snow-device-management-1.27.0/setup.py
```

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/LICENSE` & `mypy-boto3-snow-device-management-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/PKG-INFO` & `mypy-boto3-snow-device-management-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-snow-device-management
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.SnowDeviceManagement 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.SnowDeviceManagement 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/
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
 
 <a id="mypy-boto3-snow-device-management"></a>
 
 # mypy-boto3-snow-device-management
 
 [![PyPI - mypy-boto3-snow-device-management](https://img.shields.io/pypi/v/mypy-boto3-snow-device-management.svg?color=blue)](https://pypi.org/project/mypy-boto3-snow-device-management)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snow-device-management.svg?color=blue)](https://pypi.org/project/mypy-boto3-snow-device-management)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snow-device-management?color=blue)](https://pypistats.org/packages/mypy-boto3-snow-device-management)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SnowDeviceManagement 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
+[boto3.SnowDeviceManagement 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
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
 [mypy-boto3-snow-device-management docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,54 +340,54 @@
 
 `mypy_boto3_snow_device_management.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_snow_device_management.type_defs import (
     CancelTaskInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelTaskOutputTypeDef,
     CapacityTypeDef,
     CommandTypeDef,
     CpuOptionsTypeDef,
+    CreateTaskOutputTypeDef,
     DescribeDeviceEc2InputRequestTypeDef,
     DescribeDeviceInputRequestTypeDef,
     PhysicalNetworkInterfaceTypeDef,
     SoftwareInformationTypeDef,
     DescribeExecutionInputRequestTypeDef,
+    DescribeExecutionOutputTypeDef,
     DescribeTaskInputRequestTypeDef,
+    DescribeTaskOutputTypeDef,
     DeviceSummaryTypeDef,
     EbsInstanceBlockDeviceTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExecutionSummaryTypeDef,
     InstanceStateTypeDef,
     SecurityGroupIdentifierTypeDef,
-    PaginatorConfigTypeDef,
+    ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
     ListDeviceResourcesInputRequestTypeDef,
     ResourceSummaryTypeDef,
+    ListDevicesInputListDevicesPaginateTypeDef,
     ListDevicesInputRequestTypeDef,
+    ListExecutionsInputListExecutionsPaginateTypeDef,
     ListExecutionsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListTasksInputListTasksPaginateTypeDef,
     ListTasksInputRequestTypeDef,
     TaskSummaryTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    CancelTaskOutputTypeDef,
-    CreateTaskOutputTypeDef,
-    DescribeExecutionOutputTypeDef,
-    DescribeTaskOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceOutputTypeDef,
     CreateTaskInputRequestTypeDef,
     DescribeDeviceOutputTypeDef,
     ListDevicesOutputTypeDef,
     InstanceBlockDeviceMappingTypeDef,
     ListExecutionsOutputTypeDef,
-    ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
-    ListDevicesInputListDevicesPaginateTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
-    ListTasksInputListTasksPaginateTypeDef,
     ListDeviceResourcesOutputTypeDef,
     ListTasksOutputTypeDef,
     InstanceTypeDef,
     InstanceSummaryTypeDef,
     DescribeDeviceEc2OutputTypeDef,
 )
 
@@ -398,42 +399,42 @@
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

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/README.md` & `mypy-boto3-snow-device-management-1.27.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-snow-device-management"></a>
 
 # mypy-boto3-snow-device-management
 
 [![PyPI - mypy-boto3-snow-device-management](https://img.shields.io/pypi/v/mypy-boto3-snow-device-management.svg?color=blue)](https://pypi.org/project/mypy-boto3-snow-device-management)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snow-device-management.svg?color=blue)](https://pypi.org/project/mypy-boto3-snow-device-management)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snow-device-management?color=blue)](https://pypistats.org/packages/mypy-boto3-snow-device-management)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SnowDeviceManagement 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
+[boto3.SnowDeviceManagement 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
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
 [mypy-boto3-snow-device-management docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/).
 
 See how it helps to find and fix potential bugs:
 
@@ -308,54 +308,54 @@
 
 `mypy_boto3_snow_device_management.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_snow_device_management.type_defs import (
     CancelTaskInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelTaskOutputTypeDef,
     CapacityTypeDef,
     CommandTypeDef,
     CpuOptionsTypeDef,
+    CreateTaskOutputTypeDef,
     DescribeDeviceEc2InputRequestTypeDef,
     DescribeDeviceInputRequestTypeDef,
     PhysicalNetworkInterfaceTypeDef,
     SoftwareInformationTypeDef,
     DescribeExecutionInputRequestTypeDef,
+    DescribeExecutionOutputTypeDef,
     DescribeTaskInputRequestTypeDef,
+    DescribeTaskOutputTypeDef,
     DeviceSummaryTypeDef,
     EbsInstanceBlockDeviceTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExecutionSummaryTypeDef,
     InstanceStateTypeDef,
     SecurityGroupIdentifierTypeDef,
-    PaginatorConfigTypeDef,
+    ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
     ListDeviceResourcesInputRequestTypeDef,
     ResourceSummaryTypeDef,
+    ListDevicesInputListDevicesPaginateTypeDef,
     ListDevicesInputRequestTypeDef,
+    ListExecutionsInputListExecutionsPaginateTypeDef,
     ListExecutionsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListTasksInputListTasksPaginateTypeDef,
     ListTasksInputRequestTypeDef,
     TaskSummaryTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    CancelTaskOutputTypeDef,
-    CreateTaskOutputTypeDef,
-    DescribeExecutionOutputTypeDef,
-    DescribeTaskOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceOutputTypeDef,
     CreateTaskInputRequestTypeDef,
     DescribeDeviceOutputTypeDef,
     ListDevicesOutputTypeDef,
     InstanceBlockDeviceMappingTypeDef,
     ListExecutionsOutputTypeDef,
-    ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
-    ListDevicesInputListDevicesPaginateTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
-    ListTasksInputListTasksPaginateTypeDef,
     ListDeviceResourcesOutputTypeDef,
     ListTasksOutputTypeDef,
     InstanceTypeDef,
     InstanceSummaryTypeDef,
     DescribeDeviceEc2OutputTypeDef,
 )
 
@@ -367,42 +367,42 @@
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

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/__init__.py` & `mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/__init__.pyi` & `mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/__main__.py` & `mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SnowDeviceManagement 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.SnowDeviceManagement 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement\nOther"
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

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/client.py` & `mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/client.pyi` & `mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/literals.py` & `mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/literals.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,23 +65,25 @@
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
@@ -91,30 +93,35 @@
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
@@ -140,14 +147,15 @@
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
@@ -192,51 +200,57 @@
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
@@ -249,14 +263,15 @@
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
@@ -268,28 +283,35 @@
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
@@ -298,14 +320,15 @@
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
@@ -316,55 +339,64 @@
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
```

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/literals.pyi` & `mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/literals.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -63,23 +63,25 @@
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
@@ -89,30 +91,35 @@
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
@@ -138,14 +145,15 @@
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
@@ -190,51 +198,57 @@
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
@@ -247,14 +261,15 @@
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
@@ -266,28 +281,35 @@
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
@@ -296,14 +318,15 @@
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
@@ -314,55 +337,64 @@
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
```

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/paginator.py` & `mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -41,84 +41,78 @@
 __all__ = (
     "ListDeviceResourcesPaginator",
     "ListDevicesPaginator",
     "ListExecutionsPaginator",
     "ListTasksPaginator",
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
 class ListDeviceResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDeviceResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listdeviceresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         managedDeviceId: str,
         type: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeviceResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDeviceResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listdeviceresourcespaginator)
         """
 
-
 class ListDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listdevicespaginator)
     """
 
     def paginate(
-        self, *, jobId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, jobId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDevicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listdevicespaginator)
         """
 
-
 class ListExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listexecutionspaginator)
     """
 
     def paginate(
         self,
         *,
         taskId: str,
         state: ExecutionStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listexecutionspaginator)
         """
 
-
 class ListTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listtaskspaginator)
     """
 
     def paginate(
-        self, *, state: TaskStateType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, state: TaskStateType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTasksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listtaskspaginator)
         """
```

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/paginator.pyi` & `mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,78 +41,84 @@
 __all__ = (
     "ListDeviceResourcesPaginator",
     "ListDevicesPaginator",
     "ListExecutionsPaginator",
     "ListTasksPaginator",
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
 class ListDeviceResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDeviceResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listdeviceresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         managedDeviceId: str,
         type: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeviceResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDeviceResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listdeviceresourcespaginator)
         """
 
+
 class ListDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listdevicespaginator)
     """
 
     def paginate(
-        self, *, jobId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, jobId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDevicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listdevicespaginator)
         """
 
+
 class ListExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listexecutionspaginator)
     """
 
     def paginate(
         self,
         *,
         taskId: str,
         state: ExecutionStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listexecutionspaginator)
         """
 
+
 class ListTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listtaskspaginator)
     """
 
     def paginate(
-        self, *, state: TaskStateType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, state: TaskStateType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTasksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Paginator.ListTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/paginators/#listtaskspaginator)
         """
```

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/type_defs.py` & `mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,76 +29,73 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelTaskInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelTaskOutputTypeDef",
     "CapacityTypeDef",
     "CommandTypeDef",
     "CpuOptionsTypeDef",
+    "CreateTaskOutputTypeDef",
     "DescribeDeviceEc2InputRequestTypeDef",
     "DescribeDeviceInputRequestTypeDef",
     "PhysicalNetworkInterfaceTypeDef",
     "SoftwareInformationTypeDef",
     "DescribeExecutionInputRequestTypeDef",
+    "DescribeExecutionOutputTypeDef",
     "DescribeTaskInputRequestTypeDef",
+    "DescribeTaskOutputTypeDef",
     "DeviceSummaryTypeDef",
     "EbsInstanceBlockDeviceTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExecutionSummaryTypeDef",
     "InstanceStateTypeDef",
     "SecurityGroupIdentifierTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
     "ListDeviceResourcesInputRequestTypeDef",
     "ResourceSummaryTypeDef",
+    "ListDevicesInputListDevicesPaginateTypeDef",
     "ListDevicesInputRequestTypeDef",
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
     "ListExecutionsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "ListTasksInputListTasksPaginateTypeDef",
     "ListTasksInputRequestTypeDef",
     "TaskSummaryTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "CancelTaskOutputTypeDef",
-    "CreateTaskOutputTypeDef",
-    "DescribeExecutionOutputTypeDef",
-    "DescribeTaskOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "CreateTaskInputRequestTypeDef",
     "DescribeDeviceOutputTypeDef",
     "ListDevicesOutputTypeDef",
     "InstanceBlockDeviceMappingTypeDef",
     "ListExecutionsOutputTypeDef",
-    "ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
-    "ListDevicesInputListDevicesPaginateTypeDef",
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
-    "ListTasksInputListTasksPaginateTypeDef",
     "ListDeviceResourcesOutputTypeDef",
     "ListTasksOutputTypeDef",
     "InstanceTypeDef",
     "InstanceSummaryTypeDef",
     "DescribeDeviceEc2OutputTypeDef",
 )
 
 CancelTaskInputRequestTypeDef = TypedDict(
     "CancelTaskInputRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelTaskOutputTypeDef = TypedDict(
+    "CancelTaskOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CapacityTypeDef = TypedDict(
     "CapacityTypeDef",
     {
         "available": int,
@@ -124,14 +121,23 @@
     {
         "coreCount": int,
         "threadsPerCore": int,
     },
     total=False,
 )
 
+CreateTaskOutputTypeDef = TypedDict(
+    "CreateTaskOutputTypeDef",
+    {
+        "taskArn": str,
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDeviceEc2InputRequestTypeDef = TypedDict(
     "DescribeDeviceEc2InputRequestTypeDef",
     {
         "instanceIds": Sequence[str],
         "managedDeviceId": str,
     },
 )
@@ -171,21 +177,50 @@
     "DescribeExecutionInputRequestTypeDef",
     {
         "managedDeviceId": str,
         "taskId": str,
     },
 )
 
+DescribeExecutionOutputTypeDef = TypedDict(
+    "DescribeExecutionOutputTypeDef",
+    {
+        "executionId": str,
+        "lastUpdatedAt": datetime,
+        "managedDeviceId": str,
+        "startedAt": datetime,
+        "state": ExecutionStateType,
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeTaskInputRequestTypeDef = TypedDict(
     "DescribeTaskInputRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
+DescribeTaskOutputTypeDef = TypedDict(
+    "DescribeTaskOutputTypeDef",
+    {
+        "completedAt": datetime,
+        "createdAt": datetime,
+        "description": str,
+        "lastUpdatedAt": datetime,
+        "state": TaskStateType,
+        "tags": Dict[str, str],
+        "targets": List[str],
+        "taskArn": str,
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "associatedWithJob": str,
         "managedDeviceArn": str,
         "managedDeviceId": str,
         "tags": Dict[str, str],
@@ -200,14 +235,21 @@
         "deleteOnTermination": bool,
         "status": AttachmentStatusType,
         "volumeId": str,
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
 ExecutionSummaryTypeDef = TypedDict(
     "ExecutionSummaryTypeDef",
     {
         "executionId": str,
         "managedDeviceId": str,
         "state": ExecutionStateType,
         "taskId": str,
@@ -229,24 +271,37 @@
     {
         "groupId": str,
         "groupName": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "managedDeviceId": str,
+    },
+)
+_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
+    {
+        "type": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef(
+    _RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
+    _OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDeviceResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListDeviceResourcesInputRequestTypeDef",
     {
         "managedDeviceId": str,
     },
 )
 _OptionalListDeviceResourcesInputRequestTypeDef = TypedDict(
@@ -282,24 +337,56 @@
 )
 
 
 class ResourceSummaryTypeDef(_RequiredResourceSummaryTypeDef, _OptionalResourceSummaryTypeDef):
     pass
 
 
+ListDevicesInputListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesInputListDevicesPaginateTypeDef",
+    {
+        "jobId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDevicesInputRequestTypeDef = TypedDict(
     "ListDevicesInputRequestTypeDef",
     {
         "jobId": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListExecutionsInputListExecutionsPaginateTypeDef",
+    {
+        "taskId": str,
+    },
+)
+_OptionalListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListExecutionsInputListExecutionsPaginateTypeDef",
+    {
+        "state": ExecutionStateType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListExecutionsInputListExecutionsPaginateTypeDef(
+    _RequiredListExecutionsInputListExecutionsPaginateTypeDef,
+    _OptionalListExecutionsInputListExecutionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListExecutionsInputRequestTypeDef",
     {
         "taskId": str,
     },
 )
 _OptionalListExecutionsInputRequestTypeDef = TypedDict(
@@ -322,14 +409,31 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTasksInputListTasksPaginateTypeDef = TypedDict(
+    "ListTasksInputListTasksPaginateTypeDef",
+    {
+        "state": TaskStateType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTasksInputRequestTypeDef = TypedDict(
     "ListTasksInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "state": TaskStateType,
     },
@@ -353,88 +457,48 @@
 )
 
 
 class TaskSummaryTypeDef(_RequiredTaskSummaryTypeDef, _OptionalTaskSummaryTypeDef):
     pass
 
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Mapping[str, str],
-    },
-)
-
-UntagResourceInputRequestTypeDef = TypedDict(
-    "UntagResourceInputRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
-    },
-)
-
-CancelTaskOutputTypeDef = TypedDict(
-    "CancelTaskOutputTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTaskOutputTypeDef = TypedDict(
-    "CreateTaskOutputTypeDef",
-    {
-        "taskArn": str,
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeExecutionOutputTypeDef = TypedDict(
-    "DescribeExecutionOutputTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "executionId": str,
-        "lastUpdatedAt": datetime,
-        "managedDeviceId": str,
-        "startedAt": datetime,
-        "state": ExecutionStateType,
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-DescribeTaskOutputTypeDef = TypedDict(
-    "DescribeTaskOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "completedAt": datetime,
-        "createdAt": datetime,
-        "description": str,
-        "lastUpdatedAt": datetime,
-        "state": TaskStateType,
-        "tags": Dict[str, str],
-        "targets": List[str],
-        "taskArn": str,
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tags": Mapping[str, str],
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+UntagResourceInputRequestTypeDef = TypedDict(
+    "UntagResourceInputRequestTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
 _RequiredCreateTaskInputRequestTypeDef = TypedDict(
     "_RequiredCreateTaskInputRequestTypeDef",
     {
         "command": CommandTypeDef,
@@ -468,24 +532,24 @@
         "lastReachedOutAt": datetime,
         "lastUpdatedAt": datetime,
         "managedDeviceArn": str,
         "managedDeviceId": str,
         "physicalNetworkInterfaces": List[PhysicalNetworkInterfaceTypeDef],
         "software": SoftwareInformationTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDevicesOutputTypeDef = TypedDict(
     "ListDevicesOutputTypeDef",
     {
         "devices": List[DeviceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceBlockDeviceMappingTypeDef = TypedDict(
     "InstanceBlockDeviceMappingTypeDef",
     {
         "deviceName": str,
@@ -495,97 +559,33 @@
 )
 
 ListExecutionsOutputTypeDef = TypedDict(
     "ListExecutionsOutputTypeDef",
     {
         "executions": List[ExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
-    {
-        "managedDeviceId": str,
-    },
-)
-_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
-    {
-        "type": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef(
-    _RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
-    _OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
-):
-    pass
-
-
-ListDevicesInputListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesInputListDevicesPaginateTypeDef",
-    {
-        "jobId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListExecutionsInputListExecutionsPaginateTypeDef",
-    {
-        "taskId": str,
-    },
-)
-_OptionalListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListExecutionsInputListExecutionsPaginateTypeDef",
-    {
-        "state": ExecutionStateType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListExecutionsInputListExecutionsPaginateTypeDef(
-    _RequiredListExecutionsInputListExecutionsPaginateTypeDef,
-    _OptionalListExecutionsInputListExecutionsPaginateTypeDef,
-):
-    pass
-
-
-ListTasksInputListTasksPaginateTypeDef = TypedDict(
-    "ListTasksInputListTasksPaginateTypeDef",
-    {
-        "state": TaskStateType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListDeviceResourcesOutputTypeDef = TypedDict(
     "ListDeviceResourcesOutputTypeDef",
     {
         "nextToken": str,
         "resources": List[ResourceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTasksOutputTypeDef = TypedDict(
     "ListTasksOutputTypeDef",
     {
         "nextToken": str,
         "tasks": List[TaskSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "amiLaunchIndex": int,
@@ -614,10 +614,10 @@
     total=False,
 )
 
 DescribeDeviceEc2OutputTypeDef = TypedDict(
     "DescribeDeviceEc2OutputTypeDef",
     {
         "instances": List[InstanceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management/type_defs.pyi` & `mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -28,76 +28,73 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelTaskInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelTaskOutputTypeDef",
     "CapacityTypeDef",
     "CommandTypeDef",
     "CpuOptionsTypeDef",
+    "CreateTaskOutputTypeDef",
     "DescribeDeviceEc2InputRequestTypeDef",
     "DescribeDeviceInputRequestTypeDef",
     "PhysicalNetworkInterfaceTypeDef",
     "SoftwareInformationTypeDef",
     "DescribeExecutionInputRequestTypeDef",
+    "DescribeExecutionOutputTypeDef",
     "DescribeTaskInputRequestTypeDef",
+    "DescribeTaskOutputTypeDef",
     "DeviceSummaryTypeDef",
     "EbsInstanceBlockDeviceTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExecutionSummaryTypeDef",
     "InstanceStateTypeDef",
     "SecurityGroupIdentifierTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
     "ListDeviceResourcesInputRequestTypeDef",
     "ResourceSummaryTypeDef",
+    "ListDevicesInputListDevicesPaginateTypeDef",
     "ListDevicesInputRequestTypeDef",
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
     "ListExecutionsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "ListTasksInputListTasksPaginateTypeDef",
     "ListTasksInputRequestTypeDef",
     "TaskSummaryTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "CancelTaskOutputTypeDef",
-    "CreateTaskOutputTypeDef",
-    "DescribeExecutionOutputTypeDef",
-    "DescribeTaskOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "CreateTaskInputRequestTypeDef",
     "DescribeDeviceOutputTypeDef",
     "ListDevicesOutputTypeDef",
     "InstanceBlockDeviceMappingTypeDef",
     "ListExecutionsOutputTypeDef",
-    "ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
-    "ListDevicesInputListDevicesPaginateTypeDef",
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
-    "ListTasksInputListTasksPaginateTypeDef",
     "ListDeviceResourcesOutputTypeDef",
     "ListTasksOutputTypeDef",
     "InstanceTypeDef",
     "InstanceSummaryTypeDef",
     "DescribeDeviceEc2OutputTypeDef",
 )
 
 CancelTaskInputRequestTypeDef = TypedDict(
     "CancelTaskInputRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelTaskOutputTypeDef = TypedDict(
+    "CancelTaskOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CapacityTypeDef = TypedDict(
     "CapacityTypeDef",
     {
         "available": int,
@@ -123,14 +120,23 @@
     {
         "coreCount": int,
         "threadsPerCore": int,
     },
     total=False,
 )
 
+CreateTaskOutputTypeDef = TypedDict(
+    "CreateTaskOutputTypeDef",
+    {
+        "taskArn": str,
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDeviceEc2InputRequestTypeDef = TypedDict(
     "DescribeDeviceEc2InputRequestTypeDef",
     {
         "instanceIds": Sequence[str],
         "managedDeviceId": str,
     },
 )
@@ -170,21 +176,50 @@
     "DescribeExecutionInputRequestTypeDef",
     {
         "managedDeviceId": str,
         "taskId": str,
     },
 )
 
+DescribeExecutionOutputTypeDef = TypedDict(
+    "DescribeExecutionOutputTypeDef",
+    {
+        "executionId": str,
+        "lastUpdatedAt": datetime,
+        "managedDeviceId": str,
+        "startedAt": datetime,
+        "state": ExecutionStateType,
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeTaskInputRequestTypeDef = TypedDict(
     "DescribeTaskInputRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
+DescribeTaskOutputTypeDef = TypedDict(
+    "DescribeTaskOutputTypeDef",
+    {
+        "completedAt": datetime,
+        "createdAt": datetime,
+        "description": str,
+        "lastUpdatedAt": datetime,
+        "state": TaskStateType,
+        "tags": Dict[str, str],
+        "targets": List[str],
+        "taskArn": str,
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "associatedWithJob": str,
         "managedDeviceArn": str,
         "managedDeviceId": str,
         "tags": Dict[str, str],
@@ -199,14 +234,21 @@
         "deleteOnTermination": bool,
         "status": AttachmentStatusType,
         "volumeId": str,
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
 ExecutionSummaryTypeDef = TypedDict(
     "ExecutionSummaryTypeDef",
     {
         "executionId": str,
         "managedDeviceId": str,
         "state": ExecutionStateType,
         "taskId": str,
@@ -228,24 +270,35 @@
     {
         "groupId": str,
         "groupName": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "managedDeviceId": str,
+    },
+)
+_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
+    {
+        "type": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef(
+    _RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
+    _OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
+):
+    pass
+
 _RequiredListDeviceResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListDeviceResourcesInputRequestTypeDef",
     {
         "managedDeviceId": str,
     },
 )
 _OptionalListDeviceResourcesInputRequestTypeDef = TypedDict(
@@ -277,24 +330,54 @@
     },
     total=False,
 )
 
 class ResourceSummaryTypeDef(_RequiredResourceSummaryTypeDef, _OptionalResourceSummaryTypeDef):
     pass
 
+ListDevicesInputListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesInputListDevicesPaginateTypeDef",
+    {
+        "jobId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDevicesInputRequestTypeDef = TypedDict(
     "ListDevicesInputRequestTypeDef",
     {
         "jobId": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListExecutionsInputListExecutionsPaginateTypeDef",
+    {
+        "taskId": str,
+    },
+)
+_OptionalListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListExecutionsInputListExecutionsPaginateTypeDef",
+    {
+        "state": ExecutionStateType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListExecutionsInputListExecutionsPaginateTypeDef(
+    _RequiredListExecutionsInputListExecutionsPaginateTypeDef,
+    _OptionalListExecutionsInputListExecutionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListExecutionsInputRequestTypeDef",
     {
         "taskId": str,
     },
 )
 _OptionalListExecutionsInputRequestTypeDef = TypedDict(
@@ -315,14 +398,31 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTasksInputListTasksPaginateTypeDef = TypedDict(
+    "ListTasksInputListTasksPaginateTypeDef",
+    {
+        "state": TaskStateType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTasksInputRequestTypeDef = TypedDict(
     "ListTasksInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "state": TaskStateType,
     },
@@ -344,88 +444,48 @@
     },
     total=False,
 )
 
 class TaskSummaryTypeDef(_RequiredTaskSummaryTypeDef, _OptionalTaskSummaryTypeDef):
     pass
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Mapping[str, str],
-    },
-)
-
-UntagResourceInputRequestTypeDef = TypedDict(
-    "UntagResourceInputRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
-    },
-)
-
-CancelTaskOutputTypeDef = TypedDict(
-    "CancelTaskOutputTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTaskOutputTypeDef = TypedDict(
-    "CreateTaskOutputTypeDef",
-    {
-        "taskArn": str,
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeExecutionOutputTypeDef = TypedDict(
-    "DescribeExecutionOutputTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "executionId": str,
-        "lastUpdatedAt": datetime,
-        "managedDeviceId": str,
-        "startedAt": datetime,
-        "state": ExecutionStateType,
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-DescribeTaskOutputTypeDef = TypedDict(
-    "DescribeTaskOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "completedAt": datetime,
-        "createdAt": datetime,
-        "description": str,
-        "lastUpdatedAt": datetime,
-        "state": TaskStateType,
-        "tags": Dict[str, str],
-        "targets": List[str],
-        "taskArn": str,
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tags": Mapping[str, str],
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+UntagResourceInputRequestTypeDef = TypedDict(
+    "UntagResourceInputRequestTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
 _RequiredCreateTaskInputRequestTypeDef = TypedDict(
     "_RequiredCreateTaskInputRequestTypeDef",
     {
         "command": CommandTypeDef,
@@ -457,24 +517,24 @@
         "lastReachedOutAt": datetime,
         "lastUpdatedAt": datetime,
         "managedDeviceArn": str,
         "managedDeviceId": str,
         "physicalNetworkInterfaces": List[PhysicalNetworkInterfaceTypeDef],
         "software": SoftwareInformationTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDevicesOutputTypeDef = TypedDict(
     "ListDevicesOutputTypeDef",
     {
         "devices": List[DeviceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceBlockDeviceMappingTypeDef = TypedDict(
     "InstanceBlockDeviceMappingTypeDef",
     {
         "deviceName": str,
@@ -484,93 +544,33 @@
 )
 
 ListExecutionsOutputTypeDef = TypedDict(
     "ListExecutionsOutputTypeDef",
     {
         "executions": List[ExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
-    {
-        "managedDeviceId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef",
-    {
-        "type": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef(
-    _RequiredListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
-    _OptionalListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
-):
-    pass
-
-ListDevicesInputListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesInputListDevicesPaginateTypeDef",
-    {
-        "jobId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListExecutionsInputListExecutionsPaginateTypeDef",
-    {
-        "taskId": str,
-    },
-)
-_OptionalListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListExecutionsInputListExecutionsPaginateTypeDef",
-    {
-        "state": ExecutionStateType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListExecutionsInputListExecutionsPaginateTypeDef(
-    _RequiredListExecutionsInputListExecutionsPaginateTypeDef,
-    _OptionalListExecutionsInputListExecutionsPaginateTypeDef,
-):
-    pass
-
-ListTasksInputListTasksPaginateTypeDef = TypedDict(
-    "ListTasksInputListTasksPaginateTypeDef",
-    {
-        "state": TaskStateType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
 ListDeviceResourcesOutputTypeDef = TypedDict(
     "ListDeviceResourcesOutputTypeDef",
     {
         "nextToken": str,
         "resources": List[ResourceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTasksOutputTypeDef = TypedDict(
     "ListTasksOutputTypeDef",
     {
         "nextToken": str,
         "tasks": List[TaskSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "amiLaunchIndex": int,
@@ -599,10 +599,10 @@
     total=False,
 )
 
 DescribeDeviceEc2OutputTypeDef = TypedDict(
     "DescribeDeviceEc2OutputTypeDef",
     {
         "instances": List[InstanceSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management.egg-info/PKG-INFO` & `mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-snow-device-management
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.SnowDeviceManagement 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.SnowDeviceManagement 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/
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
 
 <a id="mypy-boto3-snow-device-management"></a>
 
 # mypy-boto3-snow-device-management
 
 [![PyPI - mypy-boto3-snow-device-management](https://img.shields.io/pypi/v/mypy-boto3-snow-device-management.svg?color=blue)](https://pypi.org/project/mypy-boto3-snow-device-management)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-snow-device-management.svg?color=blue)](https://pypi.org/project/mypy-boto3-snow-device-management)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-snow-device-management?color=blue)](https://pypistats.org/packages/mypy-boto3-snow-device-management)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SnowDeviceManagement 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
+[boto3.SnowDeviceManagement 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
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
 [mypy-boto3-snow-device-management docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,54 +340,54 @@
 
 `mypy_boto3_snow_device_management.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_snow_device_management.type_defs import (
     CancelTaskInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelTaskOutputTypeDef,
     CapacityTypeDef,
     CommandTypeDef,
     CpuOptionsTypeDef,
+    CreateTaskOutputTypeDef,
     DescribeDeviceEc2InputRequestTypeDef,
     DescribeDeviceInputRequestTypeDef,
     PhysicalNetworkInterfaceTypeDef,
     SoftwareInformationTypeDef,
     DescribeExecutionInputRequestTypeDef,
+    DescribeExecutionOutputTypeDef,
     DescribeTaskInputRequestTypeDef,
+    DescribeTaskOutputTypeDef,
     DeviceSummaryTypeDef,
     EbsInstanceBlockDeviceTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExecutionSummaryTypeDef,
     InstanceStateTypeDef,
     SecurityGroupIdentifierTypeDef,
-    PaginatorConfigTypeDef,
+    ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
     ListDeviceResourcesInputRequestTypeDef,
     ResourceSummaryTypeDef,
+    ListDevicesInputListDevicesPaginateTypeDef,
     ListDevicesInputRequestTypeDef,
+    ListExecutionsInputListExecutionsPaginateTypeDef,
     ListExecutionsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListTasksInputListTasksPaginateTypeDef,
     ListTasksInputRequestTypeDef,
     TaskSummaryTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    CancelTaskOutputTypeDef,
-    CreateTaskOutputTypeDef,
-    DescribeExecutionOutputTypeDef,
-    DescribeTaskOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceOutputTypeDef,
     CreateTaskInputRequestTypeDef,
     DescribeDeviceOutputTypeDef,
     ListDevicesOutputTypeDef,
     InstanceBlockDeviceMappingTypeDef,
     ListExecutionsOutputTypeDef,
-    ListDeviceResourcesInputListDeviceResourcesPaginateTypeDef,
-    ListDevicesInputListDevicesPaginateTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
-    ListTasksInputListTasksPaginateTypeDef,
     ListDeviceResourcesOutputTypeDef,
     ListTasksOutputTypeDef,
     InstanceTypeDef,
     InstanceSummaryTypeDef,
     DescribeDeviceEc2OutputTypeDef,
 )
 
@@ -398,42 +399,42 @@
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

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/mypy_boto3_snow_device_management.egg-info/SOURCES.txt` & `mypy-boto3-snow-device-management-1.27.0/mypy_boto3_snow_device_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-snow-device-management-1.26.0.post1/setup.py` & `mypy-boto3-snow-device-management-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 """
 Setup script for mypy-boto3-snow-device-management.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-snow-device-management",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_snow_device_management"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SnowDeviceManagement 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.SnowDeviceManagement 1.27.0 service generated with"
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
     keywords="boto3 snow-device-management type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_snow_device_management": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_snow_device_management": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_snow_device_management/"
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


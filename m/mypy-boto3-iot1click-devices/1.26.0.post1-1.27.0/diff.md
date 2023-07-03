# Comparing `tmp/mypy-boto3-iot1click-devices-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-iot1click-devices-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot1click-devices-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:32 2022, max compression
+gzip compressed data, was "mypy-boto3-iot1click-devices-1.27.0.tar", last modified: Mon Jul  3 19:50:52 2023, max compression
```

## Comparing `mypy-boto3-iot1click-devices-1.26.0.post1.tar` & `mypy-boto3-iot1click-devices-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:32.588828 mypy-boto3-iot1click-devices-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14467 2022-11-01 21:43:32.584828 mypy-boto3-iot1click-devices-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12980 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:32.580828 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12625 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    12603 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7180 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7178 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3234 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     9713 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     9702 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:32.584828 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14467 2022-11-01 21:43:32.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-11-01 21:43:32.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:32.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:32.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:32.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-01 21:43:32.000000 mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:32.588828 mypy-boto3-iot1click-devices-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2044 2022-11-01 21:36:04.000000 mypy-boto3-iot1click-devices-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.623398 mypy-boto3-iot1click-devices-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-07-03 19:50:52.623398 mypy-boto3-iot1click-devices-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12968 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.623398 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.623398 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-07-03 19:50:52.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-03 19:50:52.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:52.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:52.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:52.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 19:50:52.000000 mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:52.623398 mypy-boto3-iot1click-devices-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-03 19:39:32.000000 mypy-boto3-iot1click-devices-1.27.0/setup.py
```

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/LICENSE` & `mypy-boto3-iot1click-devices-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/PKG-INFO` & `mypy-boto3-iot1click-devices-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-devices
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IoT1ClickDevicesService 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.IoT1ClickDevicesService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/
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
 
 <a id="mypy-boto3-iot1click-devices"></a>
 
 # mypy-boto3-iot1click-devices
 
 [![PyPI - mypy-boto3-iot1click-devices](https://img.shields.io/pypi/v/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot1click-devices?color=blue)](https://pypistats.org/packages/mypy-boto3-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickDevicesService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
+[boto3.IoT1ClickDevicesService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [mypy-boto3-iot1click-devices docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,44 +322,44 @@
 
 `mypy_boto3_iot1click_devices.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    ClaimDevicesByClaimCodeResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     DeviceDescriptionTypeDef,
     DeviceTypeDef,
     DeviceMethodTypeDef,
+    EmptyResponseMetadataTypeDef,
     FinalizeDeviceClaimRequestRequestTypeDef,
+    FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsRequestRequestTypeDef,
     InitiateDeviceClaimRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    InitiateDeviceClaimResponseTypeDef,
+    InvokeDeviceMethodResponseTypeDef,
+    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     ListDeviceEventsRequestRequestTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UnclaimDeviceRequestRequestTypeDef,
+    UnclaimDeviceResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceStateRequestRequestTypeDef,
-    ClaimDevicesByClaimCodeResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FinalizeDeviceClaimResponseTypeDef,
-    InitiateDeviceClaimResponseTypeDef,
-    InvokeDeviceMethodResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UnclaimDeviceResponseTypeDef,
     DescribeDeviceResponseTypeDef,
     ListDevicesResponseTypeDef,
     DeviceEventTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InvokeDeviceMethodRequestRequestTypeDef,
-    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDeviceEventsResponseTypeDef,
 )
 
 
 def get_structure() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
     return {...}
 ```
@@ -366,42 +367,42 @@
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

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/README.md` & `mypy-boto3-iot1click-devices-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iot1click-devices"></a>
 
 # mypy-boto3-iot1click-devices
 
 [![PyPI - mypy-boto3-iot1click-devices](https://img.shields.io/pypi/v/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot1click-devices?color=blue)](https://pypistats.org/packages/mypy-boto3-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickDevicesService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
+[boto3.IoT1ClickDevicesService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [mypy-boto3-iot1click-devices docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,44 +290,44 @@
 
 `mypy_boto3_iot1click_devices.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    ClaimDevicesByClaimCodeResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     DeviceDescriptionTypeDef,
     DeviceTypeDef,
     DeviceMethodTypeDef,
+    EmptyResponseMetadataTypeDef,
     FinalizeDeviceClaimRequestRequestTypeDef,
+    FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsRequestRequestTypeDef,
     InitiateDeviceClaimRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    InitiateDeviceClaimResponseTypeDef,
+    InvokeDeviceMethodResponseTypeDef,
+    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     ListDeviceEventsRequestRequestTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UnclaimDeviceRequestRequestTypeDef,
+    UnclaimDeviceResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceStateRequestRequestTypeDef,
-    ClaimDevicesByClaimCodeResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FinalizeDeviceClaimResponseTypeDef,
-    InitiateDeviceClaimResponseTypeDef,
-    InvokeDeviceMethodResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UnclaimDeviceResponseTypeDef,
     DescribeDeviceResponseTypeDef,
     ListDevicesResponseTypeDef,
     DeviceEventTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InvokeDeviceMethodRequestRequestTypeDef,
-    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDeviceEventsResponseTypeDef,
 )
 
 
 def get_structure() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
     return {...}
 ```
@@ -335,42 +335,42 @@
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

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/__init__.py` & `mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/__init__.pyi` & `mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/client.py` & `mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/client.pyi` & `mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/literals.py` & `mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,23 +43,25 @@
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
@@ -69,30 +71,35 @@
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
@@ -118,14 +125,15 @@
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
@@ -170,51 +178,57 @@
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
@@ -227,14 +241,15 @@
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
@@ -246,28 +261,35 @@
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
@@ -276,14 +298,15 @@
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
@@ -294,55 +317,64 @@
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

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/literals.pyi` & `mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -41,23 +41,25 @@
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
@@ -67,30 +69,35 @@
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
@@ -116,14 +123,15 @@
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
@@ -168,51 +176,57 @@
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
@@ -225,14 +239,15 @@
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
@@ -244,28 +259,35 @@
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
@@ -274,14 +296,15 @@
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
@@ -292,55 +315,64 @@
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

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/paginator.py` & `mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,28 +53,28 @@
 
     def paginate(
         self,
         *,
         DeviceId: str,
         FromTimeStamp: Union[datetime, str],
         ToTimeStamp: Union[datetime, str],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeviceEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDeviceEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdeviceeventspaginator)
         """
 
 
 class ListDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdevicespaginator)
     """
 
     def paginate(
-        self, *, DeviceType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DeviceType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdevicespaginator)
         """
```

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/paginator.pyi` & `mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/paginator.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -50,27 +50,27 @@
 
     def paginate(
         self,
         *,
         DeviceId: str,
         FromTimeStamp: Union[datetime, str],
         ToTimeStamp: Union[datetime, str],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeviceEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDeviceEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdeviceeventspaginator)
         """
 
 class ListDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdevicespaginator)
     """
 
     def paginate(
-        self, *, DeviceType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DeviceType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdevicespaginator)
         """
```

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/type_defs.py` & `mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,62 +19,60 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "ClaimDevicesByClaimCodeResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "DeviceDescriptionTypeDef",
     "DeviceTypeDef",
     "DeviceMethodTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "FinalizeDeviceClaimRequestRequestTypeDef",
+    "FinalizeDeviceClaimResponseTypeDef",
     "GetDeviceMethodsRequestRequestTypeDef",
     "InitiateDeviceClaimRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "InitiateDeviceClaimResponseTypeDef",
+    "InvokeDeviceMethodResponseTypeDef",
+    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
     "ListDeviceEventsRequestRequestTypeDef",
+    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnclaimDeviceRequestRequestTypeDef",
+    "UnclaimDeviceResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceStateRequestRequestTypeDef",
-    "ClaimDevicesByClaimCodeResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "FinalizeDeviceClaimResponseTypeDef",
-    "InitiateDeviceClaimResponseTypeDef",
-    "InvokeDeviceMethodResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UnclaimDeviceResponseTypeDef",
     "DescribeDeviceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "DeviceEventTypeDef",
     "GetDeviceMethodsResponseTypeDef",
     "InvokeDeviceMethodRequestRequestTypeDef",
-    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
-    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListDeviceEventsResponseTypeDef",
 )
 
 ClaimDevicesByClaimCodeRequestRequestTypeDef = TypedDict(
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
     {
         "ClaimCode": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ClaimDevicesByClaimCodeResponseTypeDef = TypedDict(
+    "ClaimDevicesByClaimCodeResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ClaimCode": str,
+        "Total": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
@@ -110,14 +108,21 @@
     {
         "DeviceType": str,
         "MethodName": str,
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
 _RequiredFinalizeDeviceClaimRequestRequestTypeDef = TypedDict(
     "_RequiredFinalizeDeviceClaimRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 _OptionalFinalizeDeviceClaimRequestRequestTypeDef = TypedDict(
@@ -132,38 +137,76 @@
 class FinalizeDeviceClaimRequestRequestTypeDef(
     _RequiredFinalizeDeviceClaimRequestRequestTypeDef,
     _OptionalFinalizeDeviceClaimRequestRequestTypeDef,
 ):
     pass
 
 
+FinalizeDeviceClaimResponseTypeDef = TypedDict(
+    "FinalizeDeviceClaimResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDeviceMethodsRequestRequestTypeDef = TypedDict(
     "GetDeviceMethodsRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
 InitiateDeviceClaimRequestRequestTypeDef = TypedDict(
     "InitiateDeviceClaimRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+InitiateDeviceClaimResponseTypeDef = TypedDict(
+    "InitiateDeviceClaimResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "State": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+InvokeDeviceMethodResponseTypeDef = TypedDict(
+    "InvokeDeviceMethodResponseTypeDef",
+    {
+        "DeviceMethodResponse": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    {
+        "DeviceId": str,
+        "FromTimeStamp": Union[datetime, str],
+        "ToTimeStamp": Union[datetime, str],
+    },
+)
+_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
+    _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDeviceEventsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceEventsRequestRequestTypeDef",
     {
         "DeviceId": str,
         "FromTimeStamp": Union[datetime, str],
         "ToTimeStamp": Union[datetime, str],
     },
@@ -180,14 +223,23 @@
 
 class ListDeviceEventsRequestRequestTypeDef(
     _RequiredListDeviceEventsRequestRequestTypeDef, _OptionalListDeviceEventsRequestRequestTypeDef
 ):
     pass
 
 
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "DeviceType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDevicesRequestRequestTypeDef = TypedDict(
     "ListDevicesRequestRequestTypeDef",
     {
         "DeviceType": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -197,14 +249,43 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -212,14 +293,22 @@
 UnclaimDeviceRequestRequestTypeDef = TypedDict(
     "UnclaimDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
+UnclaimDeviceResponseTypeDef = TypedDict(
+    "UnclaimDeviceResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -241,84 +330,28 @@
 
 class UpdateDeviceStateRequestRequestTypeDef(
     _RequiredUpdateDeviceStateRequestRequestTypeDef, _OptionalUpdateDeviceStateRequestRequestTypeDef
 ):
     pass
 
 
-ClaimDevicesByClaimCodeResponseTypeDef = TypedDict(
-    "ClaimDevicesByClaimCodeResponseTypeDef",
-    {
-        "ClaimCode": str,
-        "Total": int,
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
-FinalizeDeviceClaimResponseTypeDef = TypedDict(
-    "FinalizeDeviceClaimResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InitiateDeviceClaimResponseTypeDef = TypedDict(
-    "InitiateDeviceClaimResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InvokeDeviceMethodResponseTypeDef = TypedDict(
-    "InvokeDeviceMethodResponseTypeDef",
-    {
-        "DeviceMethodResponse": str,
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
-UnclaimDeviceResponseTypeDef = TypedDict(
-    "UnclaimDeviceResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeDeviceResponseTypeDef = TypedDict(
     "DescribeDeviceResponseTypeDef",
     {
         "DeviceDescription": DeviceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeviceEventTypeDef = TypedDict(
     "DeviceEventTypeDef",
     {
         "Device": DeviceTypeDef,
@@ -327,15 +360,15 @@
     total=False,
 )
 
 GetDeviceMethodsResponseTypeDef = TypedDict(
     "GetDeviceMethodsResponseTypeDef",
     {
         "DeviceMethods": List[DeviceMethodTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredInvokeDeviceMethodRequestRequestTypeDef = TypedDict(
     "_RequiredInvokeDeviceMethodRequestRequestTypeDef",
     {
         "DeviceId": str,
@@ -354,48 +387,15 @@
 class InvokeDeviceMethodRequestRequestTypeDef(
     _RequiredInvokeDeviceMethodRequestRequestTypeDef,
     _OptionalInvokeDeviceMethodRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
-    {
-        "DeviceId": str,
-        "FromTimeStamp": Union[datetime, str],
-        "ToTimeStamp": Union[datetime, str],
-    },
-)
-_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
-    _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-    _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-):
-    pass
-
-
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    {
-        "DeviceType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListDeviceEventsResponseTypeDef = TypedDict(
     "ListDeviceEventsResponseTypeDef",
     {
         "Events": List[DeviceEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices/type_defs.pyi` & `mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -18,62 +18,60 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "ClaimDevicesByClaimCodeResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "DeviceDescriptionTypeDef",
     "DeviceTypeDef",
     "DeviceMethodTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "FinalizeDeviceClaimRequestRequestTypeDef",
+    "FinalizeDeviceClaimResponseTypeDef",
     "GetDeviceMethodsRequestRequestTypeDef",
     "InitiateDeviceClaimRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "InitiateDeviceClaimResponseTypeDef",
+    "InvokeDeviceMethodResponseTypeDef",
+    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
     "ListDeviceEventsRequestRequestTypeDef",
+    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnclaimDeviceRequestRequestTypeDef",
+    "UnclaimDeviceResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceStateRequestRequestTypeDef",
-    "ClaimDevicesByClaimCodeResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "FinalizeDeviceClaimResponseTypeDef",
-    "InitiateDeviceClaimResponseTypeDef",
-    "InvokeDeviceMethodResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UnclaimDeviceResponseTypeDef",
     "DescribeDeviceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "DeviceEventTypeDef",
     "GetDeviceMethodsResponseTypeDef",
     "InvokeDeviceMethodRequestRequestTypeDef",
-    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
-    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListDeviceEventsResponseTypeDef",
 )
 
 ClaimDevicesByClaimCodeRequestRequestTypeDef = TypedDict(
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
     {
         "ClaimCode": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ClaimDevicesByClaimCodeResponseTypeDef = TypedDict(
+    "ClaimDevicesByClaimCodeResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ClaimCode": str,
+        "Total": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
@@ -109,14 +107,21 @@
     {
         "DeviceType": str,
         "MethodName": str,
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
 _RequiredFinalizeDeviceClaimRequestRequestTypeDef = TypedDict(
     "_RequiredFinalizeDeviceClaimRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 _OptionalFinalizeDeviceClaimRequestRequestTypeDef = TypedDict(
@@ -129,38 +134,74 @@
 
 class FinalizeDeviceClaimRequestRequestTypeDef(
     _RequiredFinalizeDeviceClaimRequestRequestTypeDef,
     _OptionalFinalizeDeviceClaimRequestRequestTypeDef,
 ):
     pass
 
+FinalizeDeviceClaimResponseTypeDef = TypedDict(
+    "FinalizeDeviceClaimResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDeviceMethodsRequestRequestTypeDef = TypedDict(
     "GetDeviceMethodsRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
 InitiateDeviceClaimRequestRequestTypeDef = TypedDict(
     "InitiateDeviceClaimRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+InitiateDeviceClaimResponseTypeDef = TypedDict(
+    "InitiateDeviceClaimResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "State": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+InvokeDeviceMethodResponseTypeDef = TypedDict(
+    "InvokeDeviceMethodResponseTypeDef",
+    {
+        "DeviceMethodResponse": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    {
+        "DeviceId": str,
+        "FromTimeStamp": Union[datetime, str],
+        "ToTimeStamp": Union[datetime, str],
+    },
+)
+_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
+    _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDeviceEventsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceEventsRequestRequestTypeDef",
     {
         "DeviceId": str,
         "FromTimeStamp": Union[datetime, str],
         "ToTimeStamp": Union[datetime, str],
     },
@@ -175,14 +216,23 @@
 )
 
 class ListDeviceEventsRequestRequestTypeDef(
     _RequiredListDeviceEventsRequestRequestTypeDef, _OptionalListDeviceEventsRequestRequestTypeDef
 ):
     pass
 
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "DeviceType": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDevicesRequestRequestTypeDef = TypedDict(
     "ListDevicesRequestRequestTypeDef",
     {
         "DeviceType": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -192,14 +242,43 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -207,14 +286,22 @@
 UnclaimDeviceRequestRequestTypeDef = TypedDict(
     "UnclaimDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
+UnclaimDeviceResponseTypeDef = TypedDict(
+    "UnclaimDeviceResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -234,84 +321,28 @@
 )
 
 class UpdateDeviceStateRequestRequestTypeDef(
     _RequiredUpdateDeviceStateRequestRequestTypeDef, _OptionalUpdateDeviceStateRequestRequestTypeDef
 ):
     pass
 
-ClaimDevicesByClaimCodeResponseTypeDef = TypedDict(
-    "ClaimDevicesByClaimCodeResponseTypeDef",
-    {
-        "ClaimCode": str,
-        "Total": int,
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
-FinalizeDeviceClaimResponseTypeDef = TypedDict(
-    "FinalizeDeviceClaimResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InitiateDeviceClaimResponseTypeDef = TypedDict(
-    "InitiateDeviceClaimResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InvokeDeviceMethodResponseTypeDef = TypedDict(
-    "InvokeDeviceMethodResponseTypeDef",
-    {
-        "DeviceMethodResponse": str,
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
-UnclaimDeviceResponseTypeDef = TypedDict(
-    "UnclaimDeviceResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeDeviceResponseTypeDef = TypedDict(
     "DescribeDeviceResponseTypeDef",
     {
         "DeviceDescription": DeviceDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeviceEventTypeDef = TypedDict(
     "DeviceEventTypeDef",
     {
         "Device": DeviceTypeDef,
@@ -320,15 +351,15 @@
     total=False,
 )
 
 GetDeviceMethodsResponseTypeDef = TypedDict(
     "GetDeviceMethodsResponseTypeDef",
     {
         "DeviceMethods": List[DeviceMethodTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredInvokeDeviceMethodRequestRequestTypeDef = TypedDict(
     "_RequiredInvokeDeviceMethodRequestRequestTypeDef",
     {
         "DeviceId": str,
@@ -345,46 +376,15 @@
 
 class InvokeDeviceMethodRequestRequestTypeDef(
     _RequiredInvokeDeviceMethodRequestRequestTypeDef,
     _OptionalInvokeDeviceMethodRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
-    {
-        "DeviceId": str,
-        "FromTimeStamp": Union[datetime, str],
-        "ToTimeStamp": Union[datetime, str],
-    },
-)
-_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
-    _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-    _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-):
-    pass
-
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    {
-        "DeviceType": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListDeviceEventsResponseTypeDef = TypedDict(
     "ListDeviceEventsResponseTypeDef",
     {
         "Events": List[DeviceEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices.egg-info/PKG-INFO` & `mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-devices
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IoT1ClickDevicesService 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.IoT1ClickDevicesService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/
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
 
 <a id="mypy-boto3-iot1click-devices"></a>
 
 # mypy-boto3-iot1click-devices
 
 [![PyPI - mypy-boto3-iot1click-devices](https://img.shields.io/pypi/v/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot1click-devices?color=blue)](https://pypistats.org/packages/mypy-boto3-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickDevicesService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
+[boto3.IoT1ClickDevicesService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [mypy-boto3-iot1click-devices docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,44 +322,44 @@
 
 `mypy_boto3_iot1click_devices.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    ClaimDevicesByClaimCodeResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     DeviceDescriptionTypeDef,
     DeviceTypeDef,
     DeviceMethodTypeDef,
+    EmptyResponseMetadataTypeDef,
     FinalizeDeviceClaimRequestRequestTypeDef,
+    FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsRequestRequestTypeDef,
     InitiateDeviceClaimRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    InitiateDeviceClaimResponseTypeDef,
+    InvokeDeviceMethodResponseTypeDef,
+    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     ListDeviceEventsRequestRequestTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UnclaimDeviceRequestRequestTypeDef,
+    UnclaimDeviceResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceStateRequestRequestTypeDef,
-    ClaimDevicesByClaimCodeResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    FinalizeDeviceClaimResponseTypeDef,
-    InitiateDeviceClaimResponseTypeDef,
-    InvokeDeviceMethodResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UnclaimDeviceResponseTypeDef,
     DescribeDeviceResponseTypeDef,
     ListDevicesResponseTypeDef,
     DeviceEventTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InvokeDeviceMethodRequestRequestTypeDef,
-    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDeviceEventsResponseTypeDef,
 )
 
 
 def get_structure() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
     return {...}
 ```
@@ -366,42 +367,42 @@
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

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt` & `mypy-boto3-iot1click-devices-1.27.0/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.26.0.post1/setup.py` & `mypy-boto3-iot1click-devices-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-iot1click-devices.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot1click-devices",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_iot1click_devices"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoT1ClickDevicesService 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.IoT1ClickDevicesService 1.27.0 service generated with"
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
     keywords="boto3 iot1click-devices type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_iot1click_devices": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_iot1click_devices": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/",
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


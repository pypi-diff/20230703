# Comparing `tmp/mypy-boto3-iot-roborunner-1.26.13.post9.tar.gz` & `tmp/mypy-boto3-iot-roborunner-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot-roborunner-1.26.13.post9.tar", last modified: Fri Nov 18 23:30:00 2022, max compression
+gzip compressed data, was "mypy-boto3-iot-roborunner-1.27.0.tar", last modified: Mon Jul  3 19:50:54 2023, max compression
```

## Comparing `mypy-boto3-iot-roborunner-1.26.13.post9.tar` & `mypy-boto3-iot-roborunner-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 23:30:00.536253 mypy-boto3-iot-roborunner-1.26.13.post9/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-18 23:29:17.000000 mypy-boto3-iot-roborunner-1.26.13.post9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15135 2022-11-18 23:30:00.536253 mypy-boto3-iot-roborunner-1.26.13.post9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13665 2022-11-18 23:29:17.000000 mypy-boto3-iot-roborunner-1.26.13.post9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 23:30:00.528252 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-11-18 23:29:17.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-11-18 23:29:17.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-11-18 23:29:18.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19292 2022-11-18 23:29:18.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    19261 2022-11-18 23:29:18.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7608 2022-11-18 23:29:18.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7606 2022-11-18 23:29:18.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-11-18 23:29:18.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5188 2022-11-18 23:29:18.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 23:29:18.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    20216 2022-11-18 23:29:18.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    20177 2022-11-18 23:29:18.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-11-18 23:29:17.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 23:30:00.536253 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15135 2022-11-18 23:30:00.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-11-18 23:30:00.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 23:30:00.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 23:30:00.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-18 23:30:00.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-18 23:30:00.000000 mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-18 23:30:00.536253 mypy-boto3-iot-roborunner-1.26.13.post9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-11-18 23:29:17.000000 mypy-boto3-iot-roborunner-1.26.13.post9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.327428 mypy-boto3-iot-roborunner-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:29.000000 mypy-boto3-iot-roborunner-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15161 2023-07-03 19:50:54.323428 mypy-boto3-iot-roborunner-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-07-03 19:39:29.000000 mypy-boto3-iot-roborunner-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.323428 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-03 19:39:29.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-03 19:39:29.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:39:29.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-07-03 19:39:30.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-07-03 19:39:29.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-03 19:39:30.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-03 19:39:30.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-03 19:39:30.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-03 19:39:30.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:29.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20256 2023-07-03 19:39:31.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20217 2023-07-03 19:39:31.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:29.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.323428 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15161 2023-07-03 19:50:54.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 19:50:54.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:54.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:54.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:54.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:50:54.000000 mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:54.327428 mypy-boto3-iot-roborunner-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-03 19:39:29.000000 mypy-boto3-iot-roborunner-1.27.0/setup.py
```

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/LICENSE` & `mypy-boto3-iot-roborunner-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/PKG-INFO` & `mypy-boto3-iot-roborunner-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot-roborunner
-Version: 1.26.13.post9
-Summary: Type annotations for boto3.IoTRoboRunner 1.26.13 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTRoboRunner 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/
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
 
 <a id="mypy-boto3-iot-roborunner"></a>
 
 # mypy-boto3-iot-roborunner
 
 [![PyPI - mypy-boto3-iot-roborunner](https://img.shields.io/pypi/v/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot-roborunner?color=blue)](https://pypistats.org/packages/mypy-boto3-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTRoboRunner 1.26.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[boto3.IoTRoboRunner 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iot-roborunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,54 +334,54 @@
 `mypy_boto3_iot_roborunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot_roborunner.type_defs import (
     CartesianCoordinatesTypeDef,
     CreateDestinationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateDestinationResponseTypeDef,
     CreateSiteRequestRequestTypeDef,
+    CreateSiteResponseTypeDef,
     CreateWorkerFleetRequestRequestTypeDef,
+    CreateWorkerFleetResponseTypeDef,
     OrientationTypeDef,
     VendorPropertiesTypeDef,
+    CreateWorkerResponseTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteSiteRequestRequestTypeDef,
     DeleteWorkerFleetRequestRequestTypeDef,
     DeleteWorkerRequestRequestTypeDef,
     DestinationTypeDef,
     GetDestinationRequestRequestTypeDef,
+    GetDestinationResponseTypeDef,
     GetSiteRequestRequestTypeDef,
+    GetSiteResponseTypeDef,
     GetWorkerFleetRequestRequestTypeDef,
+    GetWorkerFleetResponseTypeDef,
     GetWorkerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListDestinationsRequestListDestinationsPaginateTypeDef,
     ListDestinationsRequestRequestTypeDef,
+    ListSitesRequestListSitesPaginateTypeDef,
     ListSitesRequestRequestTypeDef,
     SiteTypeDef,
+    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
     ListWorkerFleetsRequestRequestTypeDef,
     WorkerFleetTypeDef,
+    ListWorkersRequestListWorkersPaginateTypeDef,
     ListWorkersRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UpdateDestinationRequestRequestTypeDef,
-    UpdateSiteRequestRequestTypeDef,
-    UpdateWorkerFleetRequestRequestTypeDef,
-    PositionCoordinatesTypeDef,
-    CreateDestinationResponseTypeDef,
-    CreateSiteResponseTypeDef,
-    CreateWorkerFleetResponseTypeDef,
-    CreateWorkerResponseTypeDef,
-    GetDestinationResponseTypeDef,
-    GetSiteResponseTypeDef,
-    GetWorkerFleetResponseTypeDef,
     UpdateDestinationResponseTypeDef,
+    UpdateSiteRequestRequestTypeDef,
     UpdateSiteResponseTypeDef,
+    UpdateWorkerFleetRequestRequestTypeDef,
     UpdateWorkerFleetResponseTypeDef,
+    PositionCoordinatesTypeDef,
     ListDestinationsResponseTypeDef,
-    ListDestinationsRequestListDestinationsPaginateTypeDef,
-    ListSitesRequestListSitesPaginateTypeDef,
-    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-    ListWorkersRequestListWorkersPaginateTypeDef,
     ListSitesResponseTypeDef,
     ListWorkerFleetsResponseTypeDef,
     CreateWorkerRequestRequestTypeDef,
     GetWorkerResponseTypeDef,
     UpdateWorkerRequestRequestTypeDef,
     UpdateWorkerResponseTypeDef,
     WorkerTypeDef,
@@ -395,42 +396,42 @@
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

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/README.md` & `mypy-boto3-iot-roborunner-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iot-roborunner"></a>
 
 # mypy-boto3-iot-roborunner
 
 [![PyPI - mypy-boto3-iot-roborunner](https://img.shields.io/pypi/v/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot-roborunner?color=blue)](https://pypistats.org/packages/mypy-boto3-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTRoboRunner 1.26.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[boto3.IoTRoboRunner 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iot-roborunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,54 +302,54 @@
 `mypy_boto3_iot_roborunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot_roborunner.type_defs import (
     CartesianCoordinatesTypeDef,
     CreateDestinationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateDestinationResponseTypeDef,
     CreateSiteRequestRequestTypeDef,
+    CreateSiteResponseTypeDef,
     CreateWorkerFleetRequestRequestTypeDef,
+    CreateWorkerFleetResponseTypeDef,
     OrientationTypeDef,
     VendorPropertiesTypeDef,
+    CreateWorkerResponseTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteSiteRequestRequestTypeDef,
     DeleteWorkerFleetRequestRequestTypeDef,
     DeleteWorkerRequestRequestTypeDef,
     DestinationTypeDef,
     GetDestinationRequestRequestTypeDef,
+    GetDestinationResponseTypeDef,
     GetSiteRequestRequestTypeDef,
+    GetSiteResponseTypeDef,
     GetWorkerFleetRequestRequestTypeDef,
+    GetWorkerFleetResponseTypeDef,
     GetWorkerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListDestinationsRequestListDestinationsPaginateTypeDef,
     ListDestinationsRequestRequestTypeDef,
+    ListSitesRequestListSitesPaginateTypeDef,
     ListSitesRequestRequestTypeDef,
     SiteTypeDef,
+    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
     ListWorkerFleetsRequestRequestTypeDef,
     WorkerFleetTypeDef,
+    ListWorkersRequestListWorkersPaginateTypeDef,
     ListWorkersRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UpdateDestinationRequestRequestTypeDef,
-    UpdateSiteRequestRequestTypeDef,
-    UpdateWorkerFleetRequestRequestTypeDef,
-    PositionCoordinatesTypeDef,
-    CreateDestinationResponseTypeDef,
-    CreateSiteResponseTypeDef,
-    CreateWorkerFleetResponseTypeDef,
-    CreateWorkerResponseTypeDef,
-    GetDestinationResponseTypeDef,
-    GetSiteResponseTypeDef,
-    GetWorkerFleetResponseTypeDef,
     UpdateDestinationResponseTypeDef,
+    UpdateSiteRequestRequestTypeDef,
     UpdateSiteResponseTypeDef,
+    UpdateWorkerFleetRequestRequestTypeDef,
     UpdateWorkerFleetResponseTypeDef,
+    PositionCoordinatesTypeDef,
     ListDestinationsResponseTypeDef,
-    ListDestinationsRequestListDestinationsPaginateTypeDef,
-    ListSitesRequestListSitesPaginateTypeDef,
-    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-    ListWorkersRequestListWorkersPaginateTypeDef,
     ListSitesResponseTypeDef,
     ListWorkerFleetsResponseTypeDef,
     CreateWorkerRequestRequestTypeDef,
     GetWorkerResponseTypeDef,
     UpdateWorkerRequestRequestTypeDef,
     UpdateWorkerResponseTypeDef,
     WorkerTypeDef,
@@ -364,42 +364,42 @@
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

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/__init__.py` & `mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/__init__.pyi` & `mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/__main__.py` & `mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTRoboRunner 1.26.13\nVersion:         1.26.13.post9\nBuilder"
-        " version: 7.11.11\nDocs:           "
+        "Type annotations for boto3.IoTRoboRunner 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.13.post9")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/client.py` & `mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/client.pyi` & `mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/literals.py` & `mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,23 +50,25 @@
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
@@ -77,30 +79,34 @@
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
@@ -126,14 +132,15 @@
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
@@ -178,14 +185,15 @@
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
@@ -196,34 +204,38 @@
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
@@ -236,14 +248,15 @@
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
@@ -255,28 +268,35 @@
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
@@ -304,30 +324,34 @@
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
     "scheduler",
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
@@ -343,18 +367,21 @@
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

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/literals.pyi` & `mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -48,23 +48,25 @@
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
@@ -75,30 +77,34 @@
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
@@ -124,14 +130,15 @@
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
@@ -176,14 +183,15 @@
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
@@ -194,34 +202,38 @@
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
@@ -234,14 +246,15 @@
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
@@ -253,28 +266,35 @@
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
@@ -302,30 +322,34 @@
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
     "scheduler",
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
@@ -341,18 +365,21 @@
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

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/paginator.py` & `mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,58 +63,58 @@
     """
 
     def paginate(
         self,
         *,
         site: str,
         state: DestinationStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listdestinationspaginator)
         """
 
 
 class ListSitesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListSites)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listsitespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListSites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listsitespaginator)
         """
 
 
 class ListWorkerFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkerFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerfleetspaginator)
     """
 
     def paginate(
-        self, *, site: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, site: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkerFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkerFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerfleetspaginator)
         """
 
 
 class ListWorkersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerspaginator)
     """
 
     def paginate(
-        self, *, site: str, fleet: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, site: str, fleet: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerspaginator)
         """
```

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/paginator.pyi` & `mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -60,55 +60,55 @@
     """
 
     def paginate(
         self,
         *,
         site: str,
         state: DestinationStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listdestinationspaginator)
         """
 
 class ListSitesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListSites)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listsitespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListSites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listsitespaginator)
         """
 
 class ListWorkerFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkerFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerfleetspaginator)
     """
 
     def paginate(
-        self, *, site: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, site: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkerFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkerFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerfleetspaginator)
         """
 
 class ListWorkersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerspaginator)
     """
 
     def paginate(
-        self, *, site: str, fleet: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, site: str, fleet: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerspaginator)
         """
```

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/type_defs.py` & `mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,54 +22,54 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CartesianCoordinatesTypeDef",
     "CreateDestinationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateDestinationResponseTypeDef",
     "CreateSiteRequestRequestTypeDef",
+    "CreateSiteResponseTypeDef",
     "CreateWorkerFleetRequestRequestTypeDef",
+    "CreateWorkerFleetResponseTypeDef",
     "OrientationTypeDef",
     "VendorPropertiesTypeDef",
+    "CreateWorkerResponseTypeDef",
     "DeleteDestinationRequestRequestTypeDef",
     "DeleteSiteRequestRequestTypeDef",
     "DeleteWorkerFleetRequestRequestTypeDef",
     "DeleteWorkerRequestRequestTypeDef",
     "DestinationTypeDef",
     "GetDestinationRequestRequestTypeDef",
+    "GetDestinationResponseTypeDef",
     "GetSiteRequestRequestTypeDef",
+    "GetSiteResponseTypeDef",
     "GetWorkerFleetRequestRequestTypeDef",
+    "GetWorkerFleetResponseTypeDef",
     "GetWorkerRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDestinationsRequestListDestinationsPaginateTypeDef",
     "ListDestinationsRequestRequestTypeDef",
+    "ListSitesRequestListSitesPaginateTypeDef",
     "ListSitesRequestRequestTypeDef",
     "SiteTypeDef",
+    "ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
     "ListWorkerFleetsRequestRequestTypeDef",
     "WorkerFleetTypeDef",
+    "ListWorkersRequestListWorkersPaginateTypeDef",
     "ListWorkersRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
-    "UpdateSiteRequestRequestTypeDef",
-    "UpdateWorkerFleetRequestRequestTypeDef",
-    "PositionCoordinatesTypeDef",
-    "CreateDestinationResponseTypeDef",
-    "CreateSiteResponseTypeDef",
-    "CreateWorkerFleetResponseTypeDef",
-    "CreateWorkerResponseTypeDef",
-    "GetDestinationResponseTypeDef",
-    "GetSiteResponseTypeDef",
-    "GetWorkerFleetResponseTypeDef",
     "UpdateDestinationResponseTypeDef",
+    "UpdateSiteRequestRequestTypeDef",
     "UpdateSiteResponseTypeDef",
+    "UpdateWorkerFleetRequestRequestTypeDef",
     "UpdateWorkerFleetResponseTypeDef",
+    "PositionCoordinatesTypeDef",
     "ListDestinationsResponseTypeDef",
-    "ListDestinationsRequestListDestinationsPaginateTypeDef",
-    "ListSitesRequestListSitesPaginateTypeDef",
-    "ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
-    "ListWorkersRequestListWorkersPaginateTypeDef",
     "ListSitesResponseTypeDef",
     "ListWorkerFleetsResponseTypeDef",
     "CreateWorkerRequestRequestTypeDef",
     "GetWorkerResponseTypeDef",
     "UpdateWorkerRequestRequestTypeDef",
     "UpdateWorkerResponseTypeDef",
     "WorkerTypeDef",
@@ -118,22 +118,23 @@
 
 class CreateDestinationRequestRequestTypeDef(
     _RequiredCreateDestinationRequestRequestTypeDef, _OptionalCreateDestinationRequestRequestTypeDef
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateDestinationResponseTypeDef = TypedDict(
+    "CreateDestinationResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "state": DestinationStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSiteRequestRequestTypeDef",
     {
         "name": str,
@@ -152,14 +153,25 @@
 
 class CreateSiteRequestRequestTypeDef(
     _RequiredCreateSiteRequestRequestTypeDef, _OptionalCreateSiteRequestRequestTypeDef
 ):
     pass
 
 
+CreateSiteResponseTypeDef = TypedDict(
+    "CreateSiteResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateWorkerFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerFleetRequestRequestTypeDef",
     {
         "name": str,
         "site": str,
     },
 )
@@ -175,14 +187,25 @@
 
 class CreateWorkerFleetRequestRequestTypeDef(
     _RequiredCreateWorkerFleetRequestRequestTypeDef, _OptionalCreateWorkerFleetRequestRequestTypeDef
 ):
     pass
 
 
+CreateWorkerFleetResponseTypeDef = TypedDict(
+    "CreateWorkerFleetResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 OrientationTypeDef = TypedDict(
     "OrientationTypeDef",
     {
         "degrees": float,
     },
     total=False,
 )
@@ -204,14 +227,26 @@
 )
 
 
 class VendorPropertiesTypeDef(_RequiredVendorPropertiesTypeDef, _OptionalVendorPropertiesTypeDef):
     pass
 
 
+CreateWorkerResponseTypeDef = TypedDict(
+    "CreateWorkerResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "site": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteDestinationRequestRequestTypeDef = TypedDict(
     "DeleteDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -264,45 +299,101 @@
 GetDestinationRequestRequestTypeDef = TypedDict(
     "GetDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+GetDestinationResponseTypeDef = TypedDict(
+    "GetDestinationResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "site": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "state": DestinationStateType,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSiteRequestRequestTypeDef = TypedDict(
     "GetSiteRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+GetSiteResponseTypeDef = TypedDict(
+    "GetSiteResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "countryCode": str,
+        "description": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetWorkerFleetRequestRequestTypeDef = TypedDict(
     "GetWorkerFleetRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+GetWorkerFleetResponseTypeDef = TypedDict(
+    "GetWorkerFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "site": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetWorkerRequestRequestTypeDef = TypedDict(
     "GetWorkerRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
+    "_RequiredListDestinationsRequestListDestinationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "site": str,
+    },
+)
+_OptionalListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
+    "_OptionalListDestinationsRequestListDestinationsPaginateTypeDef",
+    {
+        "state": DestinationStateType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListDestinationsRequestListDestinationsPaginateTypeDef(
+    _RequiredListDestinationsRequestListDestinationsPaginateTypeDef,
+    _OptionalListDestinationsRequestListDestinationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDestinationsRequestRequestTypeDef = TypedDict(
     "_RequiredListDestinationsRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListDestinationsRequestRequestTypeDef = TypedDict(
@@ -318,14 +409,22 @@
 
 class ListDestinationsRequestRequestTypeDef(
     _RequiredListDestinationsRequestRequestTypeDef, _OptionalListDestinationsRequestRequestTypeDef
 ):
     pass
 
 
+ListSitesRequestListSitesPaginateTypeDef = TypedDict(
+    "ListSitesRequestListSitesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSitesRequestRequestTypeDef = TypedDict(
     "ListSitesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -337,14 +436,36 @@
         "arn": str,
         "name": str,
         "countryCode": str,
         "createdAt": datetime,
     },
 )
 
+_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
+    "_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    {
+        "site": str,
+    },
+)
+_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
+    "_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef(
+    _RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+    _OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListWorkerFleetsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkerFleetsRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListWorkerFleetsRequestRequestTypeDef = TypedDict(
@@ -383,14 +504,37 @@
 )
 
 
 class WorkerFleetTypeDef(_RequiredWorkerFleetTypeDef, _OptionalWorkerFleetTypeDef):
     pass
 
 
+_RequiredListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
+    "_RequiredListWorkersRequestListWorkersPaginateTypeDef",
+    {
+        "site": str,
+    },
+)
+_OptionalListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
+    "_OptionalListWorkersRequestListWorkersPaginateTypeDef",
+    {
+        "fleet": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListWorkersRequestListWorkersPaginateTypeDef(
+    _RequiredListWorkersRequestListWorkersPaginateTypeDef,
+    _OptionalListWorkersRequestListWorkersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListWorkersRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkersRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListWorkersRequestRequestTypeDef = TypedDict(
@@ -406,14 +550,35 @@
 
 class ListWorkersRequestRequestTypeDef(
     _RequiredListWorkersRequestRequestTypeDef, _OptionalListWorkersRequestRequestTypeDef
 ):
     pass
 
 
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
 _RequiredUpdateDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateDestinationRequestRequestTypeDef = TypedDict(
@@ -429,14 +594,27 @@
 
 class UpdateDestinationRequestRequestTypeDef(
     _RequiredUpdateDestinationRequestRequestTypeDef, _OptionalUpdateDestinationRequestRequestTypeDef
 ):
     pass
 
 
+UpdateDestinationResponseTypeDef = TypedDict(
+    "UpdateDestinationResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "updatedAt": datetime,
+        "state": DestinationStateType,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateSiteRequestRequestTypeDef = TypedDict(
@@ -452,14 +630,27 @@
 
 class UpdateSiteRequestRequestTypeDef(
     _RequiredUpdateSiteRequestRequestTypeDef, _OptionalUpdateSiteRequestRequestTypeDef
 ):
     pass
 
 
+UpdateSiteResponseTypeDef = TypedDict(
+    "UpdateSiteResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "countryCode": str,
+        "description": str,
+        "updatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateWorkerFleetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkerFleetRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateWorkerFleetRequestRequestTypeDef = TypedDict(
@@ -474,249 +665,58 @@
 
 class UpdateWorkerFleetRequestRequestTypeDef(
     _RequiredUpdateWorkerFleetRequestRequestTypeDef, _OptionalUpdateWorkerFleetRequestRequestTypeDef
 ):
     pass
 
 
-PositionCoordinatesTypeDef = TypedDict(
-    "PositionCoordinatesTypeDef",
-    {
-        "cartesianCoordinates": CartesianCoordinatesTypeDef,
-    },
-    total=False,
-)
-
-CreateDestinationResponseTypeDef = TypedDict(
-    "CreateDestinationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSiteResponseTypeDef = TypedDict(
-    "CreateSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkerFleetResponseTypeDef = TypedDict(
-    "CreateWorkerFleetResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkerResponseTypeDef = TypedDict(
-    "CreateWorkerResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "site": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDestinationResponseTypeDef = TypedDict(
-    "GetDestinationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "site": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSiteResponseTypeDef = TypedDict(
-    "GetSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "countryCode": str,
-        "description": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetWorkerFleetResponseTypeDef = TypedDict(
-    "GetWorkerFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "site": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDestinationResponseTypeDef = TypedDict(
-    "UpdateDestinationResponseTypeDef",
+UpdateWorkerFleetResponseTypeDef = TypedDict(
+    "UpdateWorkerFleetResponseTypeDef",
     {
         "arn": str,
         "id": str,
         "name": str,
         "updatedAt": datetime,
-        "state": DestinationStateType,
         "additionalFixedProperties": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateSiteResponseTypeDef = TypedDict(
-    "UpdateSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "countryCode": str,
-        "description": str,
-        "updatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateWorkerFleetResponseTypeDef = TypedDict(
-    "UpdateWorkerFleetResponseTypeDef",
+PositionCoordinatesTypeDef = TypedDict(
+    "PositionCoordinatesTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "updatedAt": datetime,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "cartesianCoordinates": CartesianCoordinatesTypeDef,
     },
+    total=False,
 )
 
 ListDestinationsResponseTypeDef = TypedDict(
     "ListDestinationsResponseTypeDef",
     {
         "nextToken": str,
         "destinations": List[DestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
-    "_RequiredListDestinationsRequestListDestinationsPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
-    "_OptionalListDestinationsRequestListDestinationsPaginateTypeDef",
-    {
-        "state": DestinationStateType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDestinationsRequestListDestinationsPaginateTypeDef(
-    _RequiredListDestinationsRequestListDestinationsPaginateTypeDef,
-    _OptionalListDestinationsRequestListDestinationsPaginateTypeDef,
-):
-    pass
-
-
-ListSitesRequestListSitesPaginateTypeDef = TypedDict(
-    "ListSitesRequestListSitesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
-    "_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
-    "_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef(
-    _RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-    _OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
-    "_RequiredListWorkersRequestListWorkersPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
-    "_OptionalListWorkersRequestListWorkersPaginateTypeDef",
-    {
-        "fleet": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListWorkersRequestListWorkersPaginateTypeDef(
-    _RequiredListWorkersRequestListWorkersPaginateTypeDef,
-    _OptionalListWorkersRequestListWorkersPaginateTypeDef,
-):
-    pass
-
-
 ListSitesResponseTypeDef = TypedDict(
     "ListSitesResponseTypeDef",
     {
         "nextToken": str,
         "sites": List[SiteTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkerFleetsResponseTypeDef = TypedDict(
     "ListWorkerFleetsResponseTypeDef",
     {
         "nextToken": str,
         "workerFleets": List[WorkerFleetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateWorkerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerRequestRequestTypeDef",
     {
         "name": str,
@@ -754,15 +754,15 @@
         "updatedAt": datetime,
         "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
         "orientation": OrientationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateWorkerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkerRequestRequestTypeDef",
     {
         "id": str,
@@ -797,15 +797,15 @@
         "updatedAt": datetime,
         "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
         "orientation": OrientationTypeDef,
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredWorkerTypeDef = TypedDict(
     "_RequiredWorkerTypeDef",
     {
         "arn": str,
@@ -835,10 +835,10 @@
 
 
 ListWorkersResponseTypeDef = TypedDict(
     "ListWorkersResponseTypeDef",
     {
         "nextToken": str,
         "workers": List[WorkerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner/type_defs.pyi` & `mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,54 +21,54 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CartesianCoordinatesTypeDef",
     "CreateDestinationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateDestinationResponseTypeDef",
     "CreateSiteRequestRequestTypeDef",
+    "CreateSiteResponseTypeDef",
     "CreateWorkerFleetRequestRequestTypeDef",
+    "CreateWorkerFleetResponseTypeDef",
     "OrientationTypeDef",
     "VendorPropertiesTypeDef",
+    "CreateWorkerResponseTypeDef",
     "DeleteDestinationRequestRequestTypeDef",
     "DeleteSiteRequestRequestTypeDef",
     "DeleteWorkerFleetRequestRequestTypeDef",
     "DeleteWorkerRequestRequestTypeDef",
     "DestinationTypeDef",
     "GetDestinationRequestRequestTypeDef",
+    "GetDestinationResponseTypeDef",
     "GetSiteRequestRequestTypeDef",
+    "GetSiteResponseTypeDef",
     "GetWorkerFleetRequestRequestTypeDef",
+    "GetWorkerFleetResponseTypeDef",
     "GetWorkerRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDestinationsRequestListDestinationsPaginateTypeDef",
     "ListDestinationsRequestRequestTypeDef",
+    "ListSitesRequestListSitesPaginateTypeDef",
     "ListSitesRequestRequestTypeDef",
     "SiteTypeDef",
+    "ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
     "ListWorkerFleetsRequestRequestTypeDef",
     "WorkerFleetTypeDef",
+    "ListWorkersRequestListWorkersPaginateTypeDef",
     "ListWorkersRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
-    "UpdateSiteRequestRequestTypeDef",
-    "UpdateWorkerFleetRequestRequestTypeDef",
-    "PositionCoordinatesTypeDef",
-    "CreateDestinationResponseTypeDef",
-    "CreateSiteResponseTypeDef",
-    "CreateWorkerFleetResponseTypeDef",
-    "CreateWorkerResponseTypeDef",
-    "GetDestinationResponseTypeDef",
-    "GetSiteResponseTypeDef",
-    "GetWorkerFleetResponseTypeDef",
     "UpdateDestinationResponseTypeDef",
+    "UpdateSiteRequestRequestTypeDef",
     "UpdateSiteResponseTypeDef",
+    "UpdateWorkerFleetRequestRequestTypeDef",
     "UpdateWorkerFleetResponseTypeDef",
+    "PositionCoordinatesTypeDef",
     "ListDestinationsResponseTypeDef",
-    "ListDestinationsRequestListDestinationsPaginateTypeDef",
-    "ListSitesRequestListSitesPaginateTypeDef",
-    "ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
-    "ListWorkersRequestListWorkersPaginateTypeDef",
     "ListSitesResponseTypeDef",
     "ListWorkerFleetsResponseTypeDef",
     "CreateWorkerRequestRequestTypeDef",
     "GetWorkerResponseTypeDef",
     "UpdateWorkerRequestRequestTypeDef",
     "UpdateWorkerResponseTypeDef",
     "WorkerTypeDef",
@@ -113,22 +113,23 @@
 )
 
 class CreateDestinationRequestRequestTypeDef(
     _RequiredCreateDestinationRequestRequestTypeDef, _OptionalCreateDestinationRequestRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateDestinationResponseTypeDef = TypedDict(
+    "CreateDestinationResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "state": DestinationStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSiteRequestRequestTypeDef",
     {
         "name": str,
@@ -145,14 +146,25 @@
 )
 
 class CreateSiteRequestRequestTypeDef(
     _RequiredCreateSiteRequestRequestTypeDef, _OptionalCreateSiteRequestRequestTypeDef
 ):
     pass
 
+CreateSiteResponseTypeDef = TypedDict(
+    "CreateSiteResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateWorkerFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerFleetRequestRequestTypeDef",
     {
         "name": str,
         "site": str,
     },
 )
@@ -166,14 +178,25 @@
 )
 
 class CreateWorkerFleetRequestRequestTypeDef(
     _RequiredCreateWorkerFleetRequestRequestTypeDef, _OptionalCreateWorkerFleetRequestRequestTypeDef
 ):
     pass
 
+CreateWorkerFleetResponseTypeDef = TypedDict(
+    "CreateWorkerFleetResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 OrientationTypeDef = TypedDict(
     "OrientationTypeDef",
     {
         "degrees": float,
     },
     total=False,
 )
@@ -193,14 +216,26 @@
     },
     total=False,
 )
 
 class VendorPropertiesTypeDef(_RequiredVendorPropertiesTypeDef, _OptionalVendorPropertiesTypeDef):
     pass
 
+CreateWorkerResponseTypeDef = TypedDict(
+    "CreateWorkerResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "site": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteDestinationRequestRequestTypeDef = TypedDict(
     "DeleteDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -251,45 +286,99 @@
 GetDestinationRequestRequestTypeDef = TypedDict(
     "GetDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+GetDestinationResponseTypeDef = TypedDict(
+    "GetDestinationResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "site": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "state": DestinationStateType,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSiteRequestRequestTypeDef = TypedDict(
     "GetSiteRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+GetSiteResponseTypeDef = TypedDict(
+    "GetSiteResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "countryCode": str,
+        "description": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetWorkerFleetRequestRequestTypeDef = TypedDict(
     "GetWorkerFleetRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+GetWorkerFleetResponseTypeDef = TypedDict(
+    "GetWorkerFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "site": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetWorkerRequestRequestTypeDef = TypedDict(
     "GetWorkerRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
+    "_RequiredListDestinationsRequestListDestinationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "site": str,
+    },
+)
+_OptionalListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
+    "_OptionalListDestinationsRequestListDestinationsPaginateTypeDef",
+    {
+        "state": DestinationStateType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListDestinationsRequestListDestinationsPaginateTypeDef(
+    _RequiredListDestinationsRequestListDestinationsPaginateTypeDef,
+    _OptionalListDestinationsRequestListDestinationsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDestinationsRequestRequestTypeDef = TypedDict(
     "_RequiredListDestinationsRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListDestinationsRequestRequestTypeDef = TypedDict(
@@ -303,14 +392,22 @@
 )
 
 class ListDestinationsRequestRequestTypeDef(
     _RequiredListDestinationsRequestRequestTypeDef, _OptionalListDestinationsRequestRequestTypeDef
 ):
     pass
 
+ListSitesRequestListSitesPaginateTypeDef = TypedDict(
+    "ListSitesRequestListSitesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSitesRequestRequestTypeDef = TypedDict(
     "ListSitesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -322,14 +419,34 @@
         "arn": str,
         "name": str,
         "countryCode": str,
         "createdAt": datetime,
     },
 )
 
+_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
+    "_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    {
+        "site": str,
+    },
+)
+_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
+    "_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef(
+    _RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+    _OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+):
+    pass
+
 _RequiredListWorkerFleetsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkerFleetsRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListWorkerFleetsRequestRequestTypeDef = TypedDict(
@@ -364,14 +481,35 @@
     },
     total=False,
 )
 
 class WorkerFleetTypeDef(_RequiredWorkerFleetTypeDef, _OptionalWorkerFleetTypeDef):
     pass
 
+_RequiredListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
+    "_RequiredListWorkersRequestListWorkersPaginateTypeDef",
+    {
+        "site": str,
+    },
+)
+_OptionalListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
+    "_OptionalListWorkersRequestListWorkersPaginateTypeDef",
+    {
+        "fleet": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListWorkersRequestListWorkersPaginateTypeDef(
+    _RequiredListWorkersRequestListWorkersPaginateTypeDef,
+    _OptionalListWorkersRequestListWorkersPaginateTypeDef,
+):
+    pass
+
 _RequiredListWorkersRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkersRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListWorkersRequestRequestTypeDef = TypedDict(
@@ -385,14 +523,35 @@
 )
 
 class ListWorkersRequestRequestTypeDef(
     _RequiredListWorkersRequestRequestTypeDef, _OptionalListWorkersRequestRequestTypeDef
 ):
     pass
 
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
 _RequiredUpdateDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateDestinationRequestRequestTypeDef = TypedDict(
@@ -406,14 +565,27 @@
 )
 
 class UpdateDestinationRequestRequestTypeDef(
     _RequiredUpdateDestinationRequestRequestTypeDef, _OptionalUpdateDestinationRequestRequestTypeDef
 ):
     pass
 
+UpdateDestinationResponseTypeDef = TypedDict(
+    "UpdateDestinationResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "updatedAt": datetime,
+        "state": DestinationStateType,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateSiteRequestRequestTypeDef = TypedDict(
@@ -427,263 +599,91 @@
 )
 
 class UpdateSiteRequestRequestTypeDef(
     _RequiredUpdateSiteRequestRequestTypeDef, _OptionalUpdateSiteRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateWorkerFleetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateWorkerFleetRequestRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalUpdateWorkerFleetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateWorkerFleetRequestRequestTypeDef",
-    {
-        "name": str,
-        "additionalFixedProperties": str,
-    },
-    total=False,
-)
-
-class UpdateWorkerFleetRequestRequestTypeDef(
-    _RequiredUpdateWorkerFleetRequestRequestTypeDef, _OptionalUpdateWorkerFleetRequestRequestTypeDef
-):
-    pass
-
-PositionCoordinatesTypeDef = TypedDict(
-    "PositionCoordinatesTypeDef",
-    {
-        "cartesianCoordinates": CartesianCoordinatesTypeDef,
-    },
-    total=False,
-)
-
-CreateDestinationResponseTypeDef = TypedDict(
-    "CreateDestinationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSiteResponseTypeDef = TypedDict(
-    "CreateSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkerFleetResponseTypeDef = TypedDict(
-    "CreateWorkerFleetResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkerResponseTypeDef = TypedDict(
-    "CreateWorkerResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "site": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDestinationResponseTypeDef = TypedDict(
-    "GetDestinationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "site": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSiteResponseTypeDef = TypedDict(
-    "GetSiteResponseTypeDef",
+UpdateSiteResponseTypeDef = TypedDict(
+    "UpdateSiteResponseTypeDef",
     {
         "arn": str,
         "id": str,
         "name": str,
         "countryCode": str,
         "description": str,
-        "createdAt": datetime,
         "updatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetWorkerFleetResponseTypeDef = TypedDict(
-    "GetWorkerFleetResponseTypeDef",
+_RequiredUpdateWorkerFleetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateWorkerFleetRequestRequestTypeDef",
     {
         "id": str,
-        "arn": str,
-        "name": str,
-        "site": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-UpdateDestinationResponseTypeDef = TypedDict(
-    "UpdateDestinationResponseTypeDef",
+_OptionalUpdateWorkerFleetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateWorkerFleetRequestRequestTypeDef",
     {
-        "arn": str,
-        "id": str,
         "name": str,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
         "additionalFixedProperties": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-UpdateSiteResponseTypeDef = TypedDict(
-    "UpdateSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "countryCode": str,
-        "description": str,
-        "updatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UpdateWorkerFleetRequestRequestTypeDef(
+    _RequiredUpdateWorkerFleetRequestRequestTypeDef, _OptionalUpdateWorkerFleetRequestRequestTypeDef
+):
+    pass
 
 UpdateWorkerFleetResponseTypeDef = TypedDict(
     "UpdateWorkerFleetResponseTypeDef",
     {
         "arn": str,
         "id": str,
         "name": str,
         "updatedAt": datetime,
         "additionalFixedProperties": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDestinationsResponseTypeDef = TypedDict(
-    "ListDestinationsResponseTypeDef",
-    {
-        "nextToken": str,
-        "destinations": List[DestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
-    "_RequiredListDestinationsRequestListDestinationsPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
-    "_OptionalListDestinationsRequestListDestinationsPaginateTypeDef",
-    {
-        "state": DestinationStateType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDestinationsRequestListDestinationsPaginateTypeDef(
-    _RequiredListDestinationsRequestListDestinationsPaginateTypeDef,
-    _OptionalListDestinationsRequestListDestinationsPaginateTypeDef,
-):
-    pass
-
-ListSitesRequestListSitesPaginateTypeDef = TypedDict(
-    "ListSitesRequestListSitesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
-    "_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
-    "_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+PositionCoordinatesTypeDef = TypedDict(
+    "PositionCoordinatesTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "cartesianCoordinates": CartesianCoordinatesTypeDef,
     },
     total=False,
 )
 
-class ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef(
-    _RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-    _OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-):
-    pass
-
-_RequiredListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
-    "_RequiredListWorkersRequestListWorkersPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
-    "_OptionalListWorkersRequestListWorkersPaginateTypeDef",
+ListDestinationsResponseTypeDef = TypedDict(
+    "ListDestinationsResponseTypeDef",
     {
-        "fleet": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "nextToken": str,
+        "destinations": List[DestinationTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class ListWorkersRequestListWorkersPaginateTypeDef(
-    _RequiredListWorkersRequestListWorkersPaginateTypeDef,
-    _OptionalListWorkersRequestListWorkersPaginateTypeDef,
-):
-    pass
-
 ListSitesResponseTypeDef = TypedDict(
     "ListSitesResponseTypeDef",
     {
         "nextToken": str,
         "sites": List[SiteTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkerFleetsResponseTypeDef = TypedDict(
     "ListWorkerFleetsResponseTypeDef",
     {
         "nextToken": str,
         "workerFleets": List[WorkerFleetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateWorkerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerRequestRequestTypeDef",
     {
         "name": str,
@@ -719,15 +719,15 @@
         "updatedAt": datetime,
         "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
         "orientation": OrientationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateWorkerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkerRequestRequestTypeDef",
     {
         "id": str,
@@ -760,15 +760,15 @@
         "updatedAt": datetime,
         "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
         "orientation": OrientationTypeDef,
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredWorkerTypeDef = TypedDict(
     "_RequiredWorkerTypeDef",
     {
         "arn": str,
@@ -796,10 +796,10 @@
     pass
 
 ListWorkersResponseTypeDef = TypedDict(
     "ListWorkersResponseTypeDef",
     {
         "nextToken": str,
         "workers": List[WorkerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner.egg-info/PKG-INFO` & `mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot-roborunner
-Version: 1.26.13.post9
-Summary: Type annotations for boto3.IoTRoboRunner 1.26.13 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTRoboRunner 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/
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
 
 <a id="mypy-boto3-iot-roborunner"></a>
 
 # mypy-boto3-iot-roborunner
 
 [![PyPI - mypy-boto3-iot-roborunner](https://img.shields.io/pypi/v/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot-roborunner?color=blue)](https://pypistats.org/packages/mypy-boto3-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTRoboRunner 1.26.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[boto3.IoTRoboRunner 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iot-roborunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,54 +334,54 @@
 `mypy_boto3_iot_roborunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot_roborunner.type_defs import (
     CartesianCoordinatesTypeDef,
     CreateDestinationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateDestinationResponseTypeDef,
     CreateSiteRequestRequestTypeDef,
+    CreateSiteResponseTypeDef,
     CreateWorkerFleetRequestRequestTypeDef,
+    CreateWorkerFleetResponseTypeDef,
     OrientationTypeDef,
     VendorPropertiesTypeDef,
+    CreateWorkerResponseTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteSiteRequestRequestTypeDef,
     DeleteWorkerFleetRequestRequestTypeDef,
     DeleteWorkerRequestRequestTypeDef,
     DestinationTypeDef,
     GetDestinationRequestRequestTypeDef,
+    GetDestinationResponseTypeDef,
     GetSiteRequestRequestTypeDef,
+    GetSiteResponseTypeDef,
     GetWorkerFleetRequestRequestTypeDef,
+    GetWorkerFleetResponseTypeDef,
     GetWorkerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListDestinationsRequestListDestinationsPaginateTypeDef,
     ListDestinationsRequestRequestTypeDef,
+    ListSitesRequestListSitesPaginateTypeDef,
     ListSitesRequestRequestTypeDef,
     SiteTypeDef,
+    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
     ListWorkerFleetsRequestRequestTypeDef,
     WorkerFleetTypeDef,
+    ListWorkersRequestListWorkersPaginateTypeDef,
     ListWorkersRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UpdateDestinationRequestRequestTypeDef,
-    UpdateSiteRequestRequestTypeDef,
-    UpdateWorkerFleetRequestRequestTypeDef,
-    PositionCoordinatesTypeDef,
-    CreateDestinationResponseTypeDef,
-    CreateSiteResponseTypeDef,
-    CreateWorkerFleetResponseTypeDef,
-    CreateWorkerResponseTypeDef,
-    GetDestinationResponseTypeDef,
-    GetSiteResponseTypeDef,
-    GetWorkerFleetResponseTypeDef,
     UpdateDestinationResponseTypeDef,
+    UpdateSiteRequestRequestTypeDef,
     UpdateSiteResponseTypeDef,
+    UpdateWorkerFleetRequestRequestTypeDef,
     UpdateWorkerFleetResponseTypeDef,
+    PositionCoordinatesTypeDef,
     ListDestinationsResponseTypeDef,
-    ListDestinationsRequestListDestinationsPaginateTypeDef,
-    ListSitesRequestListSitesPaginateTypeDef,
-    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-    ListWorkersRequestListWorkersPaginateTypeDef,
     ListSitesResponseTypeDef,
     ListWorkerFleetsResponseTypeDef,
     CreateWorkerRequestRequestTypeDef,
     GetWorkerResponseTypeDef,
     UpdateWorkerRequestRequestTypeDef,
     UpdateWorkerResponseTypeDef,
     WorkerTypeDef,
@@ -395,42 +396,42 @@
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

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt` & `mypy-boto3-iot-roborunner-1.27.0/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.26.13.post9/setup.py` & `mypy-boto3-iot-roborunner-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-iot-roborunner.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot-roborunner",
-    version="1.26.13.post9",
+    version="1.27.0",
     packages=["mypy_boto3_iot_roborunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTRoboRunner 1.26.13 service generated with mypy-boto3-builder"
-        " 7.11.11"
+        "Type annotations for boto3.IoTRoboRunner 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 iot-roborunner type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_iot_roborunner": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_iot_roborunner": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/",
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


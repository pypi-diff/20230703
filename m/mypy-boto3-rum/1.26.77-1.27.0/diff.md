# Comparing `tmp/mypy-boto3-rum-1.26.77.tar.gz` & `tmp/mypy-boto3-rum-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rum-1.26.77.tar", last modified: Wed Feb 22 20:34:22 2023, max compression
+gzip compressed data, was "mypy-boto3-rum-1.27.0.tar", last modified: Mon Jul  3 19:51:22 2023, max compression
```

## Comparing `mypy-boto3-rum-1.26.77.tar` & `mypy-boto3-rum-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.514112 mypy-boto3-rum-1.26.77/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-22 20:34:02.000000 mypy-boto3-rum-1.26.77/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-02-22 20:34:22.514112 mypy-boto3-rum-1.26.77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-02-22 20:34:02.000000 mypy-boto3-rum-1.26.77/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.514112 mypy-boto3-rum-1.26.77/mypy_boto3_rum/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-02-22 20:34:02.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-02-22 20:34:02.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-22 20:34:02.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-02-22 20:34:02.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-02-22 20:34:02.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-02-22 20:34:02.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-02-22 20:34:02.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-02-22 20:34:02.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-02-22 20:34:02.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:02.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20106 2023-02-22 20:34:03.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-02-22 20:34:02.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-22 20:34:02.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.514112 mypy-boto3-rum-1.26.77/mypy_boto3_rum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-02-22 20:34:22.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-22 20:34:22.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-22 20:34:22.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-22 20:34:22.000000 mypy-boto3-rum-1.26.77/mypy_boto3_rum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 20:34:22.514112 mypy-boto3-rum-1.26.77/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-02-22 20:34:02.000000 mypy-boto3-rum-1.26.77/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:22.255909 mypy-boto3-rum-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:42.000000 mypy-boto3-rum-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-07-03 19:51:22.251909 mypy-boto3-rum-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-07-03 19:46:42.000000 mypy-boto3-rum-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:22.251909 mypy-boto3-rum-1.27.0/mypy_boto3_rum/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-03 19:46:42.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-03 19:46:42.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:46:42.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-07-03 19:46:42.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-07-03 19:46:42.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-07-03 19:46:42.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-03 19:46:42.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-03 19:46:42.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-03 19:46:42.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:42.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20132 2023-07-03 19:46:42.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-07-03 19:46:42.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:42.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:22.251909 mypy-boto3-rum-1.27.0/mypy_boto3_rum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-07-03 19:51:22.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:51:22.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:22.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:22.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:22.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:22.000000 mypy-boto3-rum-1.27.0/mypy_boto3_rum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:22.255909 mypy-boto3-rum-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 19:46:41.000000 mypy-boto3-rum-1.27.0/setup.py
```

### Comparing `mypy-boto3-rum-1.26.77/LICENSE` & `mypy-boto3-rum-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-rum-1.26.77/PKG-INFO` & `mypy-boto3-rum-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rum
-Version: 1.26.77
-Summary: Type annotations for boto3.CloudWatchRUM 1.26.77 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudWatchRUM 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-rum"></a>
 
 # mypy-boto3-rum
 
 [![PyPI - mypy-boto3-rum](https://img.shields.io/pypi/v/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rum?color=blue)](https://pypistats.org/packages/mypy-boto3-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchRUM 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[boto3.CloudWatchRUM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-rum docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,48 +344,48 @@
 from mypy_boto3_rum.type_defs import (
     AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     AppMonitorSummaryTypeDef,
     CustomEventsTypeDef,
     MetricDefinitionRequestTypeDef,
     MetricDefinitionTypeDef,
-    ResponseMetadataTypeDef,
     BatchDeleteRumMetricDefinitionsErrorTypeDef,
     BatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
     BatchGetRumMetricDefinitionsRequestRequestTypeDef,
+    CreateAppMonitorResponseTypeDef,
     CwLogTypeDef,
     DeleteAppMonitorRequestRequestTypeDef,
     DeleteRumMetricsDestinationRequestRequestTypeDef,
     QueryFilterTypeDef,
     TimeRangeTypeDef,
+    GetAppMonitorDataResponseTypeDef,
     GetAppMonitorRequestRequestTypeDef,
+    ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
     ListAppMonitorsRequestRequestTypeDef,
+    ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
     ListRumMetricsDestinationsRequestRequestTypeDef,
     MetricDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     RumEventTypeDef,
     UserDetailsTypeDef,
     PutRumMetricsDestinationRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ListAppMonitorsResponseTypeDef,
     CreateAppMonitorRequestRequestTypeDef,
     UpdateAppMonitorRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsErrorTypeDef,
     BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
     UpdateRumMetricDefinitionRequestRequestTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
-    CreateAppMonitorResponseTypeDef,
-    GetAppMonitorDataResponseTypeDef,
-    ListAppMonitorsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
-    BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
-    ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
-    ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
     DataStorageTypeDef,
     GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
     GetAppMonitorDataRequestRequestTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
     PutRumEventsRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     AppMonitorTypeDef,
@@ -400,42 +400,42 @@
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

### Comparing `mypy-boto3-rum-1.26.77/README.md` & `mypy-boto3-rum-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-rum"></a>
 
 # mypy-boto3-rum
 
 [![PyPI - mypy-boto3-rum](https://img.shields.io/pypi/v/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rum?color=blue)](https://pypistats.org/packages/mypy-boto3-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchRUM 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[boto3.CloudWatchRUM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-rum docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,48 +312,48 @@
 from mypy_boto3_rum.type_defs import (
     AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     AppMonitorSummaryTypeDef,
     CustomEventsTypeDef,
     MetricDefinitionRequestTypeDef,
     MetricDefinitionTypeDef,
-    ResponseMetadataTypeDef,
     BatchDeleteRumMetricDefinitionsErrorTypeDef,
     BatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
     BatchGetRumMetricDefinitionsRequestRequestTypeDef,
+    CreateAppMonitorResponseTypeDef,
     CwLogTypeDef,
     DeleteAppMonitorRequestRequestTypeDef,
     DeleteRumMetricsDestinationRequestRequestTypeDef,
     QueryFilterTypeDef,
     TimeRangeTypeDef,
+    GetAppMonitorDataResponseTypeDef,
     GetAppMonitorRequestRequestTypeDef,
+    ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
     ListAppMonitorsRequestRequestTypeDef,
+    ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
     ListRumMetricsDestinationsRequestRequestTypeDef,
     MetricDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     RumEventTypeDef,
     UserDetailsTypeDef,
     PutRumMetricsDestinationRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ListAppMonitorsResponseTypeDef,
     CreateAppMonitorRequestRequestTypeDef,
     UpdateAppMonitorRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsErrorTypeDef,
     BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
     UpdateRumMetricDefinitionRequestRequestTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
-    CreateAppMonitorResponseTypeDef,
-    GetAppMonitorDataResponseTypeDef,
-    ListAppMonitorsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
-    BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
-    ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
-    ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
     DataStorageTypeDef,
     GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
     GetAppMonitorDataRequestRequestTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
     PutRumEventsRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     AppMonitorTypeDef,
@@ -368,42 +368,42 @@
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

### Comparing `mypy-boto3-rum-1.26.77/mypy_boto3_rum/__init__.py` & `mypy-boto3-rum-1.27.0/mypy_boto3_rum/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.26.77/mypy_boto3_rum/__init__.pyi` & `mypy-boto3-rum-1.27.0/mypy_boto3_rum/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.26.77/mypy_boto3_rum/__main__.py` & `mypy-boto3-rum-1.27.0/mypy_boto3_rum/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchRUM 1.26.77\nVersion:         1.26.77\nBuilder"
-        " version: 7.12.4\nDocs:           "
+        "Type annotations for boto3.CloudWatchRUM 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.77")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-rum-1.26.77/mypy_boto3_rum/client.py` & `mypy-boto3-rum-1.27.0/mypy_boto3_rum/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.26.77/mypy_boto3_rum/client.pyi` & `mypy-boto3-rum-1.27.0/mypy_boto3_rum/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.26.77/mypy_boto3_rum/literals.py` & `mypy-boto3-rum-1.27.0/mypy_boto3_rum/literals.pyi`

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
     "BatchGetRumMetricDefinitionsPaginatorName",
     "CustomEventsStatusType",
     "GetAppMonitorDataPaginatorName",
     "ListAppMonitorsPaginatorName",
     "ListRumMetricsDestinationsPaginatorName",
     "MetricDestinationType",
@@ -31,15 +30,14 @@
     "CloudWatchRUMServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BatchGetRumMetricDefinitionsPaginatorName = Literal["batch_get_rum_metric_definitions"]
 CustomEventsStatusType = Literal["DISABLED", "ENABLED"]
 GetAppMonitorDataPaginatorName = Literal["get_app_monitor_data"]
 ListAppMonitorsPaginatorName = Literal["list_app_monitors"]
 ListRumMetricsDestinationsPaginatorName = Literal["list_rum_metrics_destinations"]
 MetricDestinationType = Literal["CloudWatch", "Evidently"]
 StateEnumType = Literal["ACTIVE", "CREATED", "DELETING"]
@@ -56,14 +54,15 @@
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
@@ -103,14 +102,15 @@
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
@@ -189,14 +189,15 @@
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
@@ -207,14 +208,15 @@
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
@@ -250,14 +252,15 @@
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
@@ -276,16 +279,19 @@
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
@@ -369,15 +375,17 @@
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

### Comparing `mypy-boto3-rum-1.26.77/mypy_boto3_rum/literals.pyi` & `mypy-boto3-rum-1.27.0/mypy_boto3_rum/literals.py`

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
     "BatchGetRumMetricDefinitionsPaginatorName",
     "CustomEventsStatusType",
     "GetAppMonitorDataPaginatorName",
     "ListAppMonitorsPaginatorName",
     "ListRumMetricsDestinationsPaginatorName",
     "MetricDestinationType",
@@ -30,14 +31,15 @@
     "CloudWatchRUMServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 BatchGetRumMetricDefinitionsPaginatorName = Literal["batch_get_rum_metric_definitions"]
 CustomEventsStatusType = Literal["DISABLED", "ENABLED"]
 GetAppMonitorDataPaginatorName = Literal["get_app_monitor_data"]
 ListAppMonitorsPaginatorName = Literal["list_app_monitors"]
 ListRumMetricsDestinationsPaginatorName = Literal["list_rum_metrics_destinations"]
 MetricDestinationType = Literal["CloudWatch", "Evidently"]
 StateEnumType = Literal["ACTIVE", "CREATED", "DELETING"]
@@ -54,14 +56,15 @@
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
@@ -101,14 +104,15 @@
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
@@ -187,14 +191,15 @@
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
@@ -205,14 +210,15 @@
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
@@ -248,14 +254,15 @@
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
@@ -274,16 +281,19 @@
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
@@ -367,15 +377,17 @@
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

### Comparing `mypy-boto3-rum-1.26.77/mypy_boto3_rum/paginator.py` & `mypy-boto3-rum-1.27.0/mypy_boto3_rum/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -43,86 +43,80 @@
 __all__ = (
     "BatchGetRumMetricDefinitionsPaginator",
     "GetAppMonitorDataPaginator",
     "ListAppMonitorsPaginator",
     "ListRumMetricsDestinationsPaginator",
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
 class BatchGetRumMetricDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.BatchGetRumMetricDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#batchgetrummetricdefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         DestinationArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[BatchGetRumMetricDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.BatchGetRumMetricDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#batchgetrummetricdefinitionspaginator)
         """
 
-
 class GetAppMonitorDataPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.GetAppMonitorData)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#getappmonitordatapaginator)
     """
 
     def paginate(
         self,
         *,
         Name: str,
         TimeRange: TimeRangeTypeDef,
         Filters: Sequence[QueryFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetAppMonitorDataResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.GetAppMonitorData.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#getappmonitordatapaginator)
         """
 
-
 class ListAppMonitorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListAppMonitors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listappmonitorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAppMonitorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListAppMonitors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listappmonitorspaginator)
         """
 
-
 class ListRumMetricsDestinationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListRumMetricsDestinations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listrummetricsdestinationspaginator)
     """
 
     def paginate(
-        self, *, AppMonitorName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AppMonitorName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRumMetricsDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListRumMetricsDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listrummetricsdestinationspaginator)
         """
```

### Comparing `mypy-boto3-rum-1.26.77/mypy_boto3_rum/paginator.pyi` & `mypy-boto3-rum-1.27.0/mypy_boto3_rum/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,80 +43,86 @@
 __all__ = (
     "BatchGetRumMetricDefinitionsPaginator",
     "GetAppMonitorDataPaginator",
     "ListAppMonitorsPaginator",
     "ListRumMetricsDestinationsPaginator",
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
 class BatchGetRumMetricDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.BatchGetRumMetricDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#batchgetrummetricdefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         DestinationArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[BatchGetRumMetricDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.BatchGetRumMetricDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#batchgetrummetricdefinitionspaginator)
         """
 
+
 class GetAppMonitorDataPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.GetAppMonitorData)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#getappmonitordatapaginator)
     """
 
     def paginate(
         self,
         *,
         Name: str,
         TimeRange: TimeRangeTypeDef,
         Filters: Sequence[QueryFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetAppMonitorDataResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.GetAppMonitorData.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#getappmonitordatapaginator)
         """
 
+
 class ListAppMonitorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListAppMonitors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listappmonitorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAppMonitorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListAppMonitors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listappmonitorspaginator)
         """
 
+
 class ListRumMetricsDestinationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListRumMetricsDestinations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listrummetricsdestinationspaginator)
     """
 
     def paginate(
-        self, *, AppMonitorName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AppMonitorName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRumMetricsDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.ListRumMetricsDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/paginators/#listrummetricsdestinationspaginator)
         """
```

### Comparing `mypy-boto3-rum-1.26.77/mypy_boto3_rum/type_defs.py` & `mypy-boto3-rum-1.27.0/mypy_boto3_rum/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,48 +26,48 @@
 __all__ = (
     "AppMonitorConfigurationTypeDef",
     "AppMonitorDetailsTypeDef",
     "AppMonitorSummaryTypeDef",
     "CustomEventsTypeDef",
     "MetricDefinitionRequestTypeDef",
     "MetricDefinitionTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchDeleteRumMetricDefinitionsErrorTypeDef",
     "BatchDeleteRumMetricDefinitionsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
     "BatchGetRumMetricDefinitionsRequestRequestTypeDef",
+    "CreateAppMonitorResponseTypeDef",
     "CwLogTypeDef",
     "DeleteAppMonitorRequestRequestTypeDef",
     "DeleteRumMetricsDestinationRequestRequestTypeDef",
     "QueryFilterTypeDef",
     "TimeRangeTypeDef",
+    "GetAppMonitorDataResponseTypeDef",
     "GetAppMonitorRequestRequestTypeDef",
+    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
     "ListAppMonitorsRequestRequestTypeDef",
+    "ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
     "ListRumMetricsDestinationsRequestRequestTypeDef",
     "MetricDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "RumEventTypeDef",
     "UserDetailsTypeDef",
     "PutRumMetricsDestinationRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "ListAppMonitorsResponseTypeDef",
     "CreateAppMonitorRequestRequestTypeDef",
     "UpdateAppMonitorRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
     "BatchCreateRumMetricDefinitionsRequestRequestTypeDef",
     "UpdateRumMetricDefinitionRequestRequestTypeDef",
     "BatchGetRumMetricDefinitionsResponseTypeDef",
-    "CreateAppMonitorResponseTypeDef",
-    "GetAppMonitorDataResponseTypeDef",
-    "ListAppMonitorsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "BatchDeleteRumMetricDefinitionsResponseTypeDef",
-    "BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
-    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
-    "ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
     "DataStorageTypeDef",
     "GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef",
     "GetAppMonitorDataRequestRequestTypeDef",
     "ListRumMetricsDestinationsResponseTypeDef",
     "PutRumEventsRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     "AppMonitorTypeDef",
@@ -165,25 +165,14 @@
 )
 
 
 class MetricDefinitionTypeDef(_RequiredMetricDefinitionTypeDef, _OptionalMetricDefinitionTypeDef):
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
 BatchDeleteRumMetricDefinitionsErrorTypeDef = TypedDict(
     "BatchDeleteRumMetricDefinitionsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "MetricDefinitionId": str,
     },
@@ -209,24 +198,38 @@
 class BatchDeleteRumMetricDefinitionsRequestRequestTypeDef(
     _RequiredBatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
     _OptionalBatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
+    "_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "AppMonitorName": str,
+        "Destination": MetricDestinationType,
+    },
+)
+_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
+    "_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
+    {
+        "DestinationArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef(
+    _RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
+    _OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredBatchGetRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetRumMetricDefinitionsRequestRequestTypeDef",
     {
         "AppMonitorName": str,
         "Destination": MetricDestinationType,
     },
 )
@@ -244,14 +247,22 @@
 class BatchGetRumMetricDefinitionsRequestRequestTypeDef(
     _RequiredBatchGetRumMetricDefinitionsRequestRequestTypeDef,
     _OptionalBatchGetRumMetricDefinitionsRequestRequestTypeDef,
 ):
     pass
 
 
+CreateAppMonitorResponseTypeDef = TypedDict(
+    "CreateAppMonitorResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CwLogTypeDef = TypedDict(
     "CwLogTypeDef",
     {
         "CwLogEnabled": bool,
         "CwLogGroup": str,
     },
     total=False,
@@ -311,30 +322,69 @@
 )
 
 
 class TimeRangeTypeDef(_RequiredTimeRangeTypeDef, _OptionalTimeRangeTypeDef):
     pass
 
 
+GetAppMonitorDataResponseTypeDef = TypedDict(
+    "GetAppMonitorDataResponseTypeDef",
+    {
+        "Events": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAppMonitorRequestRequestTypeDef = TypedDict(
     "GetAppMonitorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+ListAppMonitorsRequestListAppMonitorsPaginateTypeDef = TypedDict(
+    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListAppMonitorsRequestRequestTypeDef = TypedDict(
     "ListAppMonitorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
+    "_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
+    {
+        "AppMonitorName": str,
+    },
+)
+_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
+    "_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef(
+    _RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
+    _OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRumMetricsDestinationsRequestRequestTypeDef = TypedDict(
     "_RequiredListRumMetricsDestinationsRequestRequestTypeDef",
     {
         "AppMonitorName": str,
     },
 )
 _OptionalListRumMetricsDestinationsRequestRequestTypeDef = TypedDict(
@@ -367,14 +417,33 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
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
 _RequiredRumEventTypeDef = TypedDict(
     "_RequiredRumEventTypeDef",
     {
         "details": str,
         "id": str,
         "timestamp": Union[datetime, str],
         "type": str,
@@ -422,14 +491,25 @@
 class PutRumMetricsDestinationRequestRequestTypeDef(
     _RequiredPutRumMetricsDestinationRequestRequestTypeDef,
     _OptionalPutRumMetricsDestinationRequestRequestTypeDef,
 ):
     pass
 
 
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
@@ -438,14 +518,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+ListAppMonitorsResponseTypeDef = TypedDict(
+    "ListAppMonitorsResponseTypeDef",
+    {
+        "AppMonitorSummaries": List[AppMonitorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateAppMonitorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppMonitorRequestRequestTypeDef",
     {
         "Domain": str,
         "Name": str,
     },
 )
@@ -550,115 +639,26 @@
 
 
 BatchGetRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchGetRumMetricDefinitionsResponseTypeDef",
     {
         "MetricDefinitions": List[MetricDefinitionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAppMonitorResponseTypeDef = TypedDict(
-    "CreateAppMonitorResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAppMonitorDataResponseTypeDef = TypedDict(
-    "GetAppMonitorDataResponseTypeDef",
-    {
-        "Events": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAppMonitorsResponseTypeDef = TypedDict(
-    "ListAppMonitorsResponseTypeDef",
-    {
-        "AppMonitorSummaries": List[AppMonitorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchDeleteRumMetricDefinitionsResponseTypeDef",
     {
         "Errors": List[BatchDeleteRumMetricDefinitionsErrorTypeDef],
         "MetricDefinitionIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
-    "_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
-    {
-        "AppMonitorName": str,
-        "Destination": MetricDestinationType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
-    "_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
-    {
-        "DestinationArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef(
-    _RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
-    _OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
-):
-    pass
-
-
-ListAppMonitorsRequestListAppMonitorsPaginateTypeDef = TypedDict(
-    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
-    "_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
-    {
-        "AppMonitorName": str,
-    },
-)
-_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
-    "_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef(
-    _RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
-    _OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
-):
-    pass
-
 
 DataStorageTypeDef = TypedDict(
     "DataStorageTypeDef",
     {
         "CwLog": CwLogTypeDef,
     },
     total=False,
@@ -671,15 +671,15 @@
         "TimeRange": TimeRangeTypeDef,
     },
 )
 _OptionalGetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef = TypedDict(
     "_OptionalGetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef",
     {
         "Filters": Sequence[QueryFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef(
     _RequiredGetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
@@ -713,15 +713,15 @@
 
 
 ListRumMetricsDestinationsResponseTypeDef = TypedDict(
     "ListRumMetricsDestinationsResponseTypeDef",
     {
         "Destinations": List[MetricDestinationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRumEventsRequestRequestTypeDef = TypedDict(
     "PutRumEventsRequestRequestTypeDef",
     {
         "AppMonitorDetails": AppMonitorDetailsTypeDef,
@@ -733,15 +733,15 @@
 )
 
 BatchCreateRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     {
         "Errors": List[BatchCreateRumMetricDefinitionsErrorTypeDef],
         "MetricDefinitions": List[MetricDefinitionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AppMonitorTypeDef = TypedDict(
     "AppMonitorTypeDef",
     {
         "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
@@ -758,10 +758,10 @@
     total=False,
 )
 
 GetAppMonitorResponseTypeDef = TypedDict(
     "GetAppMonitorResponseTypeDef",
     {
         "AppMonitor": AppMonitorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-rum-1.26.77/mypy_boto3_rum/type_defs.pyi` & `mypy-boto3-rum-1.27.0/mypy_boto3_rum/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,48 +25,48 @@
 __all__ = (
     "AppMonitorConfigurationTypeDef",
     "AppMonitorDetailsTypeDef",
     "AppMonitorSummaryTypeDef",
     "CustomEventsTypeDef",
     "MetricDefinitionRequestTypeDef",
     "MetricDefinitionTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchDeleteRumMetricDefinitionsErrorTypeDef",
     "BatchDeleteRumMetricDefinitionsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
     "BatchGetRumMetricDefinitionsRequestRequestTypeDef",
+    "CreateAppMonitorResponseTypeDef",
     "CwLogTypeDef",
     "DeleteAppMonitorRequestRequestTypeDef",
     "DeleteRumMetricsDestinationRequestRequestTypeDef",
     "QueryFilterTypeDef",
     "TimeRangeTypeDef",
+    "GetAppMonitorDataResponseTypeDef",
     "GetAppMonitorRequestRequestTypeDef",
+    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
     "ListAppMonitorsRequestRequestTypeDef",
+    "ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
     "ListRumMetricsDestinationsRequestRequestTypeDef",
     "MetricDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "RumEventTypeDef",
     "UserDetailsTypeDef",
     "PutRumMetricsDestinationRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "ListAppMonitorsResponseTypeDef",
     "CreateAppMonitorRequestRequestTypeDef",
     "UpdateAppMonitorRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
     "BatchCreateRumMetricDefinitionsRequestRequestTypeDef",
     "UpdateRumMetricDefinitionRequestRequestTypeDef",
     "BatchGetRumMetricDefinitionsResponseTypeDef",
-    "CreateAppMonitorResponseTypeDef",
-    "GetAppMonitorDataResponseTypeDef",
-    "ListAppMonitorsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "BatchDeleteRumMetricDefinitionsResponseTypeDef",
-    "BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
-    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
-    "ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
     "DataStorageTypeDef",
     "GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef",
     "GetAppMonitorDataRequestRequestTypeDef",
     "ListRumMetricsDestinationsResponseTypeDef",
     "PutRumEventsRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     "AppMonitorTypeDef",
@@ -160,25 +160,14 @@
     },
     total=False,
 )
 
 class MetricDefinitionTypeDef(_RequiredMetricDefinitionTypeDef, _OptionalMetricDefinitionTypeDef):
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
 BatchDeleteRumMetricDefinitionsErrorTypeDef = TypedDict(
     "BatchDeleteRumMetricDefinitionsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "MetricDefinitionId": str,
     },
@@ -202,24 +191,36 @@
 
 class BatchDeleteRumMetricDefinitionsRequestRequestTypeDef(
     _RequiredBatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
     _OptionalBatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
+    "_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "AppMonitorName": str,
+        "Destination": MetricDestinationType,
+    },
+)
+_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
+    "_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
+    {
+        "DestinationArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef(
+    _RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
+    _OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
+):
+    pass
+
 _RequiredBatchGetRumMetricDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetRumMetricDefinitionsRequestRequestTypeDef",
     {
         "AppMonitorName": str,
         "Destination": MetricDestinationType,
     },
 )
@@ -235,14 +236,22 @@
 
 class BatchGetRumMetricDefinitionsRequestRequestTypeDef(
     _RequiredBatchGetRumMetricDefinitionsRequestRequestTypeDef,
     _OptionalBatchGetRumMetricDefinitionsRequestRequestTypeDef,
 ):
     pass
 
+CreateAppMonitorResponseTypeDef = TypedDict(
+    "CreateAppMonitorResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CwLogTypeDef = TypedDict(
     "CwLogTypeDef",
     {
         "CwLogEnabled": bool,
         "CwLogGroup": str,
     },
     total=False,
@@ -298,30 +307,67 @@
     },
     total=False,
 )
 
 class TimeRangeTypeDef(_RequiredTimeRangeTypeDef, _OptionalTimeRangeTypeDef):
     pass
 
+GetAppMonitorDataResponseTypeDef = TypedDict(
+    "GetAppMonitorDataResponseTypeDef",
+    {
+        "Events": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAppMonitorRequestRequestTypeDef = TypedDict(
     "GetAppMonitorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+ListAppMonitorsRequestListAppMonitorsPaginateTypeDef = TypedDict(
+    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListAppMonitorsRequestRequestTypeDef = TypedDict(
     "ListAppMonitorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
+    "_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
+    {
+        "AppMonitorName": str,
+    },
+)
+_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
+    "_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef(
+    _RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
+    _OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
+):
+    pass
+
 _RequiredListRumMetricsDestinationsRequestRequestTypeDef = TypedDict(
     "_RequiredListRumMetricsDestinationsRequestRequestTypeDef",
     {
         "AppMonitorName": str,
     },
 )
 _OptionalListRumMetricsDestinationsRequestRequestTypeDef = TypedDict(
@@ -352,14 +398,33 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
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
 _RequiredRumEventTypeDef = TypedDict(
     "_RequiredRumEventTypeDef",
     {
         "details": str,
         "id": str,
         "timestamp": Union[datetime, str],
         "type": str,
@@ -403,14 +468,25 @@
 
 class PutRumMetricsDestinationRequestRequestTypeDef(
     _RequiredPutRumMetricsDestinationRequestRequestTypeDef,
     _OptionalPutRumMetricsDestinationRequestRequestTypeDef,
 ):
     pass
 
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
@@ -419,14 +495,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+ListAppMonitorsResponseTypeDef = TypedDict(
+    "ListAppMonitorsResponseTypeDef",
+    {
+        "AppMonitorSummaries": List[AppMonitorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateAppMonitorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppMonitorRequestRequestTypeDef",
     {
         "Domain": str,
         "Name": str,
     },
 )
@@ -523,112 +608,27 @@
     pass
 
 BatchGetRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchGetRumMetricDefinitionsResponseTypeDef",
     {
         "MetricDefinitions": List[MetricDefinitionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAppMonitorResponseTypeDef = TypedDict(
-    "CreateAppMonitorResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAppMonitorDataResponseTypeDef = TypedDict(
-    "GetAppMonitorDataResponseTypeDef",
-    {
-        "Events": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAppMonitorsResponseTypeDef = TypedDict(
-    "ListAppMonitorsResponseTypeDef",
-    {
-        "AppMonitorSummaries": List[AppMonitorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchDeleteRumMetricDefinitionsResponseTypeDef",
     {
         "Errors": List[BatchDeleteRumMetricDefinitionsErrorTypeDef],
         "MetricDefinitionIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
-    "_RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
-    {
-        "AppMonitorName": str,
-        "Destination": MetricDestinationType,
-    },
-)
-_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef = TypedDict(
-    "_OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
-    {
-        "DestinationArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef(
-    _RequiredBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
-    _OptionalBatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
-):
-    pass
-
-ListAppMonitorsRequestListAppMonitorsPaginateTypeDef = TypedDict(
-    "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
-    "_RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
-    {
-        "AppMonitorName": str,
-    },
-)
-_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef = TypedDict(
-    "_OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef(
-    _RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
-    _OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
-):
-    pass
-
 DataStorageTypeDef = TypedDict(
     "DataStorageTypeDef",
     {
         "CwLog": CwLogTypeDef,
     },
     total=False,
 )
@@ -640,15 +640,15 @@
         "TimeRange": TimeRangeTypeDef,
     },
 )
 _OptionalGetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef = TypedDict(
     "_OptionalGetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef",
     {
         "Filters": Sequence[QueryFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef(
     _RequiredGetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
     _OptionalGetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
@@ -678,15 +678,15 @@
     pass
 
 ListRumMetricsDestinationsResponseTypeDef = TypedDict(
     "ListRumMetricsDestinationsResponseTypeDef",
     {
         "Destinations": List[MetricDestinationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRumEventsRequestRequestTypeDef = TypedDict(
     "PutRumEventsRequestRequestTypeDef",
     {
         "AppMonitorDetails": AppMonitorDetailsTypeDef,
@@ -698,15 +698,15 @@
 )
 
 BatchCreateRumMetricDefinitionsResponseTypeDef = TypedDict(
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     {
         "Errors": List[BatchCreateRumMetricDefinitionsErrorTypeDef],
         "MetricDefinitions": List[MetricDefinitionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AppMonitorTypeDef = TypedDict(
     "AppMonitorTypeDef",
     {
         "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
@@ -723,10 +723,10 @@
     total=False,
 )
 
 GetAppMonitorResponseTypeDef = TypedDict(
     "GetAppMonitorResponseTypeDef",
     {
         "AppMonitor": AppMonitorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-rum-1.26.77/mypy_boto3_rum.egg-info/PKG-INFO` & `mypy-boto3-rum-1.27.0/mypy_boto3_rum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rum
-Version: 1.26.77
-Summary: Type annotations for boto3.CloudWatchRUM 1.26.77 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudWatchRUM 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-rum"></a>
 
 # mypy-boto3-rum
 
 [![PyPI - mypy-boto3-rum](https://img.shields.io/pypi/v/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rum?color=blue)](https://pypistats.org/packages/mypy-boto3-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchRUM 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[boto3.CloudWatchRUM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-rum docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,48 +344,48 @@
 from mypy_boto3_rum.type_defs import (
     AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     AppMonitorSummaryTypeDef,
     CustomEventsTypeDef,
     MetricDefinitionRequestTypeDef,
     MetricDefinitionTypeDef,
-    ResponseMetadataTypeDef,
     BatchDeleteRumMetricDefinitionsErrorTypeDef,
     BatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
     BatchGetRumMetricDefinitionsRequestRequestTypeDef,
+    CreateAppMonitorResponseTypeDef,
     CwLogTypeDef,
     DeleteAppMonitorRequestRequestTypeDef,
     DeleteRumMetricsDestinationRequestRequestTypeDef,
     QueryFilterTypeDef,
     TimeRangeTypeDef,
+    GetAppMonitorDataResponseTypeDef,
     GetAppMonitorRequestRequestTypeDef,
+    ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
     ListAppMonitorsRequestRequestTypeDef,
+    ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
     ListRumMetricsDestinationsRequestRequestTypeDef,
     MetricDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     RumEventTypeDef,
     UserDetailsTypeDef,
     PutRumMetricsDestinationRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ListAppMonitorsResponseTypeDef,
     CreateAppMonitorRequestRequestTypeDef,
     UpdateAppMonitorRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsErrorTypeDef,
     BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
     UpdateRumMetricDefinitionRequestRequestTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
-    CreateAppMonitorResponseTypeDef,
-    GetAppMonitorDataResponseTypeDef,
-    ListAppMonitorsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
-    BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
-    ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
-    ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
     DataStorageTypeDef,
     GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
     GetAppMonitorDataRequestRequestTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
     PutRumEventsRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     AppMonitorTypeDef,
@@ -400,42 +400,42 @@
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

### Comparing `mypy-boto3-rum-1.26.77/mypy_boto3_rum.egg-info/SOURCES.txt` & `mypy-boto3-rum-1.27.0/mypy_boto3_rum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.26.77/setup.py` & `mypy-boto3-rum-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-rum.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rum",
-    version="1.26.77",
+    version="1.27.0",
     packages=["mypy_boto3_rum"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchRUM 1.26.77 service generated with mypy-boto3-builder"
-        " 7.12.4"
+        "Type annotations for boto3.CloudWatchRUM 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/",
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


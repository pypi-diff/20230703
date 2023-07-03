# Comparing `tmp/mypy-boto3-sagemaker-metrics-1.26.30.tar.gz` & `tmp/mypy-boto3-sagemaker-metrics-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-metrics-1.26.30.tar", last modified: Wed Dec 14 20:47:11 2022, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-metrics-1.27.0.tar", last modified: Mon Jul  3 19:51:24 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-metrics-1.26.30.tar` & `mypy-boto3-sagemaker-metrics-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 20:47:11.629212 mypy-boto3-sagemaker-metrics-1.26.30/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-14 20:47:03.000000 mypy-boto3-sagemaker-metrics-1.26.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12514 2022-12-14 20:47:11.629212 mypy-boto3-sagemaker-metrics-1.26.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10988 2022-12-14 20:47:03.000000 mypy-boto3-sagemaker-metrics-1.26.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 20:47:11.629212 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2022-12-14 20:47:03.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2022-12-14 20:47:03.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2022-12-14 20:47:03.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2022-12-14 20:47:03.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2022-12-14 20:47:03.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2022-12-14 20:47:03.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2022-12-14 20:47:03.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 20:47:03.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2022-12-14 20:47:03.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2022-12-14 20:47:03.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-14 20:47:03.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 20:47:11.629212 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12514 2022-12-14 20:47:11.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2022-12-14 20:47:11.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 20:47:11.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 20:47:11.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-14 20:47:11.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-14 20:47:11.000000 mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-14 20:47:11.629212 mypy-boto3-sagemaker-metrics-1.26.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2022-12-14 20:47:03.000000 mypy-boto3-sagemaker-metrics-1.26.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:24.347944 mypy-boto3-sagemaker-metrics-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:47:27.000000 mypy-boto3-sagemaker-metrics-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-07-03 19:51:24.347944 mypy-boto3-sagemaker-metrics-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-07-03 19:47:27.000000 mypy-boto3-sagemaker-metrics-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:24.343944 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-03 19:47:27.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-03 19:47:27.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 19:47:27.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-03 19:47:27.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-03 19:47:27.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-07-03 19:47:27.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-07-03 19:47:27.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:47:27.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-03 19:47:27.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-03 19:47:27.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:47:27.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:24.347944 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:24.347944 mypy-boto3-sagemaker-metrics-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-03 19:47:27.000000 mypy-boto3-sagemaker-metrics-1.27.0/setup.py
```

### Comparing `mypy-boto3-sagemaker-metrics-1.26.30/LICENSE` & `mypy-boto3-sagemaker-metrics-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-sagemaker-metrics-1.26.30/PKG-INFO` & `mypy-boto3-sagemaker-metrics-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-metrics
-Version: 1.26.30
-Summary: Type annotations for boto3.SageMakerMetrics 1.26.30 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.SageMakerMetrics 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-sagemaker-metrics"></a>
 
 # mypy-boto3-sagemaker-metrics
 
 [![PyPI - mypy-boto3-sagemaker-metrics](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-metrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-metrics)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-metrics?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-metrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerMetrics 1.26.30](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
+[boto3.SageMakerMetrics 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
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
 [mypy-boto3-sagemaker-metrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,58 +301,58 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_metrics.type_defs import (
     BatchPutMetricsErrorTypeDef,
     RawMetricDataTypeDef,
     ResponseMetadataTypeDef,
-    BatchPutMetricsRequestRequestTypeDef,
     BatchPutMetricsResponseTypeDef,
+    BatchPutMetricsRequestRequestTypeDef,
 )
 
 
 def get_structure() -> BatchPutMetricsErrorTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-sagemaker-metrics-1.26.30/README.md` & `mypy-boto3-sagemaker-metrics-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sagemaker-metrics"></a>
 
 # mypy-boto3-sagemaker-metrics
 
 [![PyPI - mypy-boto3-sagemaker-metrics](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-metrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-metrics)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-metrics?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-metrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerMetrics 1.26.30](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
+[boto3.SageMakerMetrics 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
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
 [mypy-boto3-sagemaker-metrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,58 +269,58 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_metrics.type_defs import (
     BatchPutMetricsErrorTypeDef,
     RawMetricDataTypeDef,
     ResponseMetadataTypeDef,
-    BatchPutMetricsRequestRequestTypeDef,
     BatchPutMetricsResponseTypeDef,
+    BatchPutMetricsRequestRequestTypeDef,
 )
 
 
 def get_structure() -> BatchPutMetricsErrorTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/__main__.py` & `mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMakerMetrics 1.26.30\nVersion:         1.26.30\nBuilder"
-        " version: 7.12.0\nDocs:           "
+        "Type annotations for boto3.SageMakerMetrics 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.30")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/client.py` & `mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/client.pyi` & `mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/literals.py` & `mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,24 +14,22 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "PutMetricsErrorCodeType",
     "SageMakerMetricsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 PutMetricsErrorCodeType = Literal[
     "CONFLICT_ERROR", "INTERNAL_ERROR", "METRIC_LIMIT_EXCEEDED", "VALIDATION_ERROR"
 ]
 SageMakerMetricsServiceName = Literal["sagemaker-metrics"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -43,14 +41,15 @@
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
@@ -71,31 +70,34 @@
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
@@ -174,14 +176,15 @@
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
@@ -192,34 +195,38 @@
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
@@ -232,14 +239,15 @@
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
@@ -258,16 +266,19 @@
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
@@ -347,18 +358,21 @@
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
@@ -383,23 +397,28 @@
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
+    "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/literals.pyi` & `mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "PutMetricsErrorCodeType",
     "SageMakerMetricsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 PutMetricsErrorCodeType = Literal[
     "CONFLICT_ERROR", "INTERNAL_ERROR", "METRIC_LIMIT_EXCEEDED", "VALIDATION_ERROR"
 ]
 SageMakerMetricsServiceName = Literal["sagemaker-metrics"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -41,14 +43,15 @@
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
@@ -69,31 +72,34 @@
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
@@ -172,14 +178,15 @@
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
@@ -190,34 +197,38 @@
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
@@ -230,14 +241,15 @@
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
@@ -256,16 +268,19 @@
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
@@ -345,18 +360,21 @@
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
@@ -381,23 +399,28 @@
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
+    "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/type_defs.py` & `mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,20 @@
 from .literals import PutMetricsErrorCodeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BatchPutMetricsErrorTypeDef",
     "RawMetricDataTypeDef",
     "ResponseMetadataTypeDef",
-    "BatchPutMetricsRequestRequestTypeDef",
     "BatchPutMetricsResponseTypeDef",
+    "BatchPutMetricsRequestRequestTypeDef",
 )
 
 BatchPutMetricsErrorTypeDef = TypedDict(
     "BatchPutMetricsErrorTypeDef",
     {
         "Code": PutMetricsErrorCodeType,
         "MetricIndex": int,
@@ -52,38 +51,36 @@
     "_OptionalRawMetricDataTypeDef",
     {
         "Step": int,
     },
     total=False,
 )
 
-
 class RawMetricDataTypeDef(_RequiredRawMetricDataTypeDef, _OptionalRawMetricDataTypeDef):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-BatchPutMetricsRequestRequestTypeDef = TypedDict(
-    "BatchPutMetricsRequestRequestTypeDef",
+BatchPutMetricsResponseTypeDef = TypedDict(
+    "BatchPutMetricsResponseTypeDef",
     {
-        "TrialComponentName": str,
-        "MetricData": Sequence[RawMetricDataTypeDef],
+        "Errors": List[BatchPutMetricsErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-BatchPutMetricsResponseTypeDef = TypedDict(
-    "BatchPutMetricsResponseTypeDef",
+BatchPutMetricsRequestRequestTypeDef = TypedDict(
+    "BatchPutMetricsRequestRequestTypeDef",
     {
-        "Errors": List[BatchPutMetricsErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TrialComponentName": str,
+        "MetricData": Sequence[RawMetricDataTypeDef],
     },
 )
```

### Comparing `mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics/type_defs.pyi` & `mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,20 +18,21 @@
 from .literals import PutMetricsErrorCodeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BatchPutMetricsErrorTypeDef",
     "RawMetricDataTypeDef",
     "ResponseMetadataTypeDef",
-    "BatchPutMetricsRequestRequestTypeDef",
     "BatchPutMetricsResponseTypeDef",
+    "BatchPutMetricsRequestRequestTypeDef",
 )
 
 BatchPutMetricsErrorTypeDef = TypedDict(
     "BatchPutMetricsErrorTypeDef",
     {
         "Code": PutMetricsErrorCodeType,
         "MetricIndex": int,
@@ -51,36 +52,38 @@
     "_OptionalRawMetricDataTypeDef",
     {
         "Step": int,
     },
     total=False,
 )
 
+
 class RawMetricDataTypeDef(_RequiredRawMetricDataTypeDef, _OptionalRawMetricDataTypeDef):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-BatchPutMetricsRequestRequestTypeDef = TypedDict(
-    "BatchPutMetricsRequestRequestTypeDef",
+BatchPutMetricsResponseTypeDef = TypedDict(
+    "BatchPutMetricsResponseTypeDef",
     {
-        "TrialComponentName": str,
-        "MetricData": Sequence[RawMetricDataTypeDef],
+        "Errors": List[BatchPutMetricsErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-BatchPutMetricsResponseTypeDef = TypedDict(
-    "BatchPutMetricsResponseTypeDef",
+BatchPutMetricsRequestRequestTypeDef = TypedDict(
+    "BatchPutMetricsRequestRequestTypeDef",
     {
-        "Errors": List[BatchPutMetricsErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TrialComponentName": str,
+        "MetricData": Sequence[RawMetricDataTypeDef],
     },
 )
```

### Comparing `mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-metrics
-Version: 1.26.30
-Summary: Type annotations for boto3.SageMakerMetrics 1.26.30 service generated with mypy-boto3-builder 7.12.0
+Version: 1.27.0
+Summary: Type annotations for boto3.SageMakerMetrics 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-sagemaker-metrics"></a>
 
 # mypy-boto3-sagemaker-metrics
 
 [![PyPI - mypy-boto3-sagemaker-metrics](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-metrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-metrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-metrics)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-metrics?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-metrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakerMetrics 1.26.30](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
+[boto3.SageMakerMetrics 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
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
 [mypy-boto3-sagemaker-metrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,58 +301,58 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_metrics.type_defs import (
     BatchPutMetricsErrorTypeDef,
     RawMetricDataTypeDef,
     ResponseMetadataTypeDef,
-    BatchPutMetricsRequestRequestTypeDef,
     BatchPutMetricsResponseTypeDef,
+    BatchPutMetricsRequestRequestTypeDef,
 )
 
 
 def get_structure() -> BatchPutMetricsErrorTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-sagemaker-metrics-1.26.30/mypy_boto3_sagemaker_metrics.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-metrics-1.27.0/mypy_boto3_sagemaker_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-metrics-1.26.30/setup.py` & `mypy-boto3-sagemaker-metrics-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-sagemaker-metrics.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-metrics",
-    version="1.26.30",
+    version="1.27.0",
     packages=["mypy_boto3_sagemaker_metrics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMakerMetrics 1.26.30 service generated with"
-        " mypy-boto3-builder 7.12.0"
+        "Type annotations for boto3.SageMakerMetrics 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_metrics/",
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


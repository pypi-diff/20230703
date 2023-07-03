# Comparing `tmp/mypy-boto3-braket-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-braket-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-braket-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:09 2022, max compression
+gzip compressed data, was "mypy-boto3-braket-1.27.0.tar", last modified: Mon Jul  3 19:50:26 2023, max compression
```

## Comparing `mypy-boto3-braket-1.26.0.post1.tar` & `mypy-boto3-braket-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:09.768836 mypy-boto3-braket-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14607 2022-11-01 21:43:09.768836 mypy-boto3-braket-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13170 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:09.756837 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12403 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    12380 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9359 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9357 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4132 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4127 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    17637 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    17606 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:09.768836 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14607 2022-11-01 21:43:09.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-11-01 21:43:09.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:09.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:09.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:09.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-01 21:43:09.000000 mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:09.768836 mypy-boto3-braket-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-11-01 21:31:01.000000 mypy-boto3-braket-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:26.970900 mypy-boto3-braket-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:10.000000 mypy-boto3-braket-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14628 2023-07-03 19:50:26.966900 mypy-boto3-braket-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-07-03 19:33:10.000000 mypy-boto3-braket-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:26.966900 mypy-boto3-braket-1.27.0/mypy_boto3_braket/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-03 19:33:10.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-03 19:33:10.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-03 19:33:10.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-07-03 19:33:10.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-03 19:33:10.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-03 19:33:11.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-07-03 19:33:11.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-03 19:33:11.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-03 19:33:10.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:10.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-07-03 19:33:11.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17634 2023-07-03 19:33:11.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:10.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:26.966900 mypy-boto3-braket-1.27.0/mypy_boto3_braket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14628 2023-07-03 19:50:26.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 19:50:26.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:26.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:26.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:26.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 19:50:26.000000 mypy-boto3-braket-1.27.0/mypy_boto3_braket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:26.970900 mypy-boto3-braket-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 19:33:10.000000 mypy-boto3-braket-1.27.0/setup.py
```

### Comparing `mypy-boto3-braket-1.26.0.post1/LICENSE` & `mypy-boto3-braket-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-braket-1.26.0.post1/PKG-INFO` & `mypy-boto3-braket-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-braket
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Braket 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Braket 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/
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
 
 <a id="mypy-boto3-braket"></a>
 
 # mypy-boto3-braket
 
 [![PyPI - mypy-boto3-braket](https://img.shields.io/pypi/v/mypy-boto3-braket.svg?color=blue)](https://pypi.org/project/mypy-boto3-braket)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-braket.svg?color=blue)](https://pypi.org/project/mypy-boto3-braket)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-braket?color=blue)](https://pypistats.org/packages/mypy-boto3-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Braket 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
+[boto3.Braket 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
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
 [mypy-boto3-braket docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,45 +341,45 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_braket.type_defs import (
     ContainerImageTypeDef,
     ScriptModeConfigTypeDef,
     CancelJobRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJobResponseTypeDef,
     CancelQuantumTaskRequestRequestTypeDef,
+    CancelQuantumTaskResponseTypeDef,
     DeviceConfigTypeDef,
     InstanceConfigTypeDef,
     JobCheckpointConfigTypeDef,
     JobOutputDataConfigTypeDef,
     JobStoppingConditionTypeDef,
+    CreateJobResponseTypeDef,
     CreateQuantumTaskRequestRequestTypeDef,
+    CreateQuantumTaskResponseTypeDef,
     S3DataSourceTypeDef,
     DeviceSummaryTypeDef,
     GetDeviceRequestRequestTypeDef,
+    GetDeviceResponseTypeDef,
     GetJobRequestRequestTypeDef,
     JobEventDetailsTypeDef,
     GetQuantumTaskRequestRequestTypeDef,
+    GetQuantumTaskResponseTypeDef,
     JobSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     QuantumTaskSummaryTypeDef,
+    ResponseMetadataTypeDef,
     SearchDevicesFilterTypeDef,
     SearchJobsFilterTypeDef,
     SearchQuantumTasksFilterTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AlgorithmSpecificationTypeDef,
-    CancelJobResponseTypeDef,
-    CancelQuantumTaskResponseTypeDef,
-    CreateJobResponseTypeDef,
-    CreateQuantumTaskResponseTypeDef,
-    GetDeviceResponseTypeDef,
-    GetQuantumTaskResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     DataSourceTypeDef,
     SearchDevicesResponseTypeDef,
     SearchJobsResponseTypeDef,
     SearchQuantumTasksResponseTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchJobsRequestRequestTypeDef,
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

### Comparing `mypy-boto3-braket-1.26.0.post1/README.md` & `mypy-boto3-braket-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-braket"></a>
 
 # mypy-boto3-braket
 
 [![PyPI - mypy-boto3-braket](https://img.shields.io/pypi/v/mypy-boto3-braket.svg?color=blue)](https://pypi.org/project/mypy-boto3-braket)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-braket.svg?color=blue)](https://pypi.org/project/mypy-boto3-braket)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-braket?color=blue)](https://pypistats.org/packages/mypy-boto3-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Braket 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
+[boto3.Braket 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
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
 [mypy-boto3-braket docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,45 +309,45 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_braket.type_defs import (
     ContainerImageTypeDef,
     ScriptModeConfigTypeDef,
     CancelJobRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJobResponseTypeDef,
     CancelQuantumTaskRequestRequestTypeDef,
+    CancelQuantumTaskResponseTypeDef,
     DeviceConfigTypeDef,
     InstanceConfigTypeDef,
     JobCheckpointConfigTypeDef,
     JobOutputDataConfigTypeDef,
     JobStoppingConditionTypeDef,
+    CreateJobResponseTypeDef,
     CreateQuantumTaskRequestRequestTypeDef,
+    CreateQuantumTaskResponseTypeDef,
     S3DataSourceTypeDef,
     DeviceSummaryTypeDef,
     GetDeviceRequestRequestTypeDef,
+    GetDeviceResponseTypeDef,
     GetJobRequestRequestTypeDef,
     JobEventDetailsTypeDef,
     GetQuantumTaskRequestRequestTypeDef,
+    GetQuantumTaskResponseTypeDef,
     JobSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     QuantumTaskSummaryTypeDef,
+    ResponseMetadataTypeDef,
     SearchDevicesFilterTypeDef,
     SearchJobsFilterTypeDef,
     SearchQuantumTasksFilterTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AlgorithmSpecificationTypeDef,
-    CancelJobResponseTypeDef,
-    CancelQuantumTaskResponseTypeDef,
-    CreateJobResponseTypeDef,
-    CreateQuantumTaskResponseTypeDef,
-    GetDeviceResponseTypeDef,
-    GetQuantumTaskResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     DataSourceTypeDef,
     SearchDevicesResponseTypeDef,
     SearchJobsResponseTypeDef,
     SearchQuantumTasksResponseTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchJobsRequestRequestTypeDef,
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

### Comparing `mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/__init__.py` & `mypy-boto3-braket-1.27.0/mypy_boto3_braket/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/__init__.pyi` & `mypy-boto3-braket-1.27.0/mypy_boto3_braket/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/__main__.py` & `mypy-boto3-braket-1.27.0/mypy_boto3_braket/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Braket 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.Braket 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket\nOther"
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

### Comparing `mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/client.py` & `mypy-boto3-braket-1.27.0/mypy_boto3_braket/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/client.pyi` & `mypy-boto3-braket-1.27.0/mypy_boto3_braket/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/literals.py` & `mypy-boto3-braket-1.27.0/mypy_boto3_braket/literals.py`

 * *Files 9% similar despite different names*

```diff
@@ -122,23 +122,25 @@
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
@@ -148,30 +150,35 @@
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
@@ -197,14 +204,15 @@
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
@@ -249,51 +257,57 @@
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
@@ -306,14 +320,15 @@
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
@@ -325,28 +340,35 @@
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
@@ -355,14 +377,15 @@
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
@@ -373,55 +396,64 @@
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

### Comparing `mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/literals.pyi` & `mypy-boto3-braket-1.27.0/mypy_boto3_braket/literals.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -120,23 +120,25 @@
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
@@ -146,30 +148,35 @@
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
@@ -195,14 +202,15 @@
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
@@ -247,51 +255,57 @@
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
@@ -304,14 +318,15 @@
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
@@ -323,28 +338,35 @@
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
@@ -353,14 +375,15 @@
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
@@ -371,55 +394,64 @@
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

### Comparing `mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/paginator.py` & `mypy-boto3-braket-1.27.0/mypy_boto3_braket/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -35,70 +35,65 @@
     SearchJobsResponseTypeDef,
     SearchQuantumTasksFilterTypeDef,
     SearchQuantumTasksResponseTypeDef,
 )
 
 __all__ = ("SearchDevicesPaginator", "SearchJobsPaginator", "SearchQuantumTasksPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class SearchDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchdevicespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchDevicesFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchdevicespaginator)
         """
 
-
 class SearchJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchJobsFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchjobspaginator)
         """
 
-
 class SearchQuantumTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchQuantumTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchquantumtaskspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchQuantumTasksFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchQuantumTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchQuantumTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchquantumtaskspaginator)
         """
```

### Comparing `mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/paginator.pyi` & `mypy-boto3-braket-1.27.0/mypy_boto3_braket/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,65 +35,70 @@
     SearchJobsResponseTypeDef,
     SearchQuantumTasksFilterTypeDef,
     SearchQuantumTasksResponseTypeDef,
 )
 
 __all__ = ("SearchDevicesPaginator", "SearchJobsPaginator", "SearchQuantumTasksPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class SearchDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchdevicespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchDevicesFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchdevicespaginator)
         """
 
+
 class SearchJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchJobsFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchjobspaginator)
         """
 
+
 class SearchQuantumTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchQuantumTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchquantumtaskspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchQuantumTasksFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchQuantumTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchQuantumTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchquantumtaskspaginator)
         """
```

### Comparing `mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/type_defs.py` & `mypy-boto3-braket-1.27.0/mypy_boto3_braket/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -29,50 +29,49 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ContainerImageTypeDef",
     "ScriptModeConfigTypeDef",
     "CancelJobRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelJobResponseTypeDef",
     "CancelQuantumTaskRequestRequestTypeDef",
+    "CancelQuantumTaskResponseTypeDef",
     "DeviceConfigTypeDef",
     "InstanceConfigTypeDef",
     "JobCheckpointConfigTypeDef",
     "JobOutputDataConfigTypeDef",
     "JobStoppingConditionTypeDef",
+    "CreateJobResponseTypeDef",
     "CreateQuantumTaskRequestRequestTypeDef",
+    "CreateQuantumTaskResponseTypeDef",
     "S3DataSourceTypeDef",
     "DeviceSummaryTypeDef",
     "GetDeviceRequestRequestTypeDef",
+    "GetDeviceResponseTypeDef",
     "GetJobRequestRequestTypeDef",
     "JobEventDetailsTypeDef",
     "GetQuantumTaskRequestRequestTypeDef",
+    "GetQuantumTaskResponseTypeDef",
     "JobSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "QuantumTaskSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "SearchDevicesFilterTypeDef",
     "SearchJobsFilterTypeDef",
     "SearchQuantumTasksFilterTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AlgorithmSpecificationTypeDef",
-    "CancelJobResponseTypeDef",
-    "CancelQuantumTaskResponseTypeDef",
-    "CreateJobResponseTypeDef",
-    "CreateQuantumTaskResponseTypeDef",
-    "GetDeviceResponseTypeDef",
-    "GetQuantumTaskResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "DataSourceTypeDef",
     "SearchDevicesResponseTypeDef",
     "SearchJobsResponseTypeDef",
     "SearchQuantumTasksResponseTypeDef",
     "SearchDevicesRequestRequestTypeDef",
     "SearchDevicesRequestSearchDevicesPaginateTypeDef",
     "SearchJobsRequestRequestTypeDef",
@@ -102,45 +101,50 @@
     "_OptionalScriptModeConfigTypeDef",
     {
         "compressionType": CompressionTypeType,
     },
     total=False,
 )
 
-
 class ScriptModeConfigTypeDef(_RequiredScriptModeConfigTypeDef, _OptionalScriptModeConfigTypeDef):
     pass
 
-
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelJobResponseTypeDef = TypedDict(
+    "CancelJobResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "cancellationStatus": CancellationStatusType,
+        "jobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CancelQuantumTaskRequestRequestTypeDef = TypedDict(
     "CancelQuantumTaskRequestRequestTypeDef",
     {
         "clientToken": str,
         "quantumTaskArn": str,
     },
 )
 
+CancelQuantumTaskResponseTypeDef = TypedDict(
+    "CancelQuantumTaskResponseTypeDef",
+    {
+        "cancellationStatus": CancellationStatusType,
+        "quantumTaskArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeviceConfigTypeDef = TypedDict(
     "DeviceConfigTypeDef",
     {
         "device": str,
     },
 )
 
@@ -155,69 +159,71 @@
     "_OptionalInstanceConfigTypeDef",
     {
         "instanceCount": int,
     },
     total=False,
 )
 
-
 class InstanceConfigTypeDef(_RequiredInstanceConfigTypeDef, _OptionalInstanceConfigTypeDef):
     pass
 
-
 _RequiredJobCheckpointConfigTypeDef = TypedDict(
     "_RequiredJobCheckpointConfigTypeDef",
     {
         "s3Uri": str,
     },
 )
 _OptionalJobCheckpointConfigTypeDef = TypedDict(
     "_OptionalJobCheckpointConfigTypeDef",
     {
         "localPath": str,
     },
     total=False,
 )
 
-
 class JobCheckpointConfigTypeDef(
     _RequiredJobCheckpointConfigTypeDef, _OptionalJobCheckpointConfigTypeDef
 ):
     pass
 
-
 _RequiredJobOutputDataConfigTypeDef = TypedDict(
     "_RequiredJobOutputDataConfigTypeDef",
     {
         "s3Path": str,
     },
 )
 _OptionalJobOutputDataConfigTypeDef = TypedDict(
     "_OptionalJobOutputDataConfigTypeDef",
     {
         "kmsKeyId": str,
     },
     total=False,
 )
 
-
 class JobOutputDataConfigTypeDef(
     _RequiredJobOutputDataConfigTypeDef, _OptionalJobOutputDataConfigTypeDef
 ):
     pass
 
-
 JobStoppingConditionTypeDef = TypedDict(
     "JobStoppingConditionTypeDef",
     {
         "maxRuntimeInSeconds": int,
     },
     total=False,
 )
 
+CreateJobResponseTypeDef = TypedDict(
+    "CreateJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateQuantumTaskRequestRequestTypeDef = TypedDict(
     "_RequiredCreateQuantumTaskRequestRequestTypeDef",
     {
         "action": str,
         "clientToken": str,
         "deviceArn": str,
         "outputS3Bucket": str,
@@ -231,20 +237,26 @@
         "deviceParameters": str,
         "jobToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateQuantumTaskRequestRequestTypeDef(
     _RequiredCreateQuantumTaskRequestRequestTypeDef, _OptionalCreateQuantumTaskRequestRequestTypeDef
 ):
     pass
 
+CreateQuantumTaskResponseTypeDef = TypedDict(
+    "CreateQuantumTaskResponseTypeDef",
+    {
+        "quantumTaskArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 S3DataSourceTypeDef = TypedDict(
     "S3DataSourceTypeDef",
     {
         "s3Uri": str,
     },
 )
@@ -263,14 +275,27 @@
 GetDeviceRequestRequestTypeDef = TypedDict(
     "GetDeviceRequestRequestTypeDef",
     {
         "deviceArn": str,
     },
 )
 
+GetDeviceResponseTypeDef = TypedDict(
+    "GetDeviceResponseTypeDef",
+    {
+        "deviceArn": str,
+        "deviceCapabilities": str,
+        "deviceName": str,
+        "deviceStatus": DeviceStatusType,
+        "deviceType": DeviceTypeType,
+        "providerName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetJobRequestRequestTypeDef = TypedDict(
     "GetJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
@@ -287,14 +312,33 @@
 GetQuantumTaskRequestRequestTypeDef = TypedDict(
     "GetQuantumTaskRequestRequestTypeDef",
     {
         "quantumTaskArn": str,
     },
 )
 
+GetQuantumTaskResponseTypeDef = TypedDict(
+    "GetQuantumTaskResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "deviceArn": str,
+        "deviceParameters": str,
+        "endedAt": datetime,
+        "failureReason": str,
+        "jobArn": str,
+        "outputS3Bucket": str,
+        "outputS3Directory": str,
+        "quantumTaskArn": str,
+        "shots": int,
+        "status": QuantumTaskStatusType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredJobSummaryTypeDef = TypedDict(
     "_RequiredJobSummaryTypeDef",
     {
         "createdAt": datetime,
         "device": str,
         "jobArn": str,
         "jobName": str,
@@ -307,26 +351,32 @@
         "endedAt": datetime,
         "startedAt": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class JobSummaryTypeDef(_RequiredJobSummaryTypeDef, _OptionalJobSummaryTypeDef):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -350,20 +400,29 @@
     {
         "endedAt": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class QuantumTaskSummaryTypeDef(
     _RequiredQuantumTaskSummaryTypeDef, _OptionalQuantumTaskSummaryTypeDef
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
 
 SearchDevicesFilterTypeDef = TypedDict(
     "SearchDevicesFilterTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
@@ -408,119 +467,45 @@
     {
         "containerImage": ContainerImageTypeDef,
         "scriptModeConfig": ScriptModeConfigTypeDef,
     },
     total=False,
 )
 
-CancelJobResponseTypeDef = TypedDict(
-    "CancelJobResponseTypeDef",
-    {
-        "cancellationStatus": CancellationStatusType,
-        "jobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelQuantumTaskResponseTypeDef = TypedDict(
-    "CancelQuantumTaskResponseTypeDef",
-    {
-        "cancellationStatus": CancellationStatusType,
-        "quantumTaskArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobResponseTypeDef = TypedDict(
-    "CreateJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateQuantumTaskResponseTypeDef = TypedDict(
-    "CreateQuantumTaskResponseTypeDef",
-    {
-        "quantumTaskArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDeviceResponseTypeDef = TypedDict(
-    "GetDeviceResponseTypeDef",
-    {
-        "deviceArn": str,
-        "deviceCapabilities": str,
-        "deviceName": str,
-        "deviceStatus": DeviceStatusType,
-        "deviceType": DeviceTypeType,
-        "providerName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetQuantumTaskResponseTypeDef = TypedDict(
-    "GetQuantumTaskResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "deviceArn": str,
-        "deviceParameters": str,
-        "endedAt": datetime,
-        "failureReason": str,
-        "jobArn": str,
-        "outputS3Bucket": str,
-        "outputS3Directory": str,
-        "quantumTaskArn": str,
-        "shots": int,
-        "status": QuantumTaskStatusType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "s3DataSource": S3DataSourceTypeDef,
     },
 )
 
 SearchDevicesResponseTypeDef = TypedDict(
     "SearchDevicesResponseTypeDef",
     {
         "devices": List[DeviceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchJobsResponseTypeDef = TypedDict(
     "SearchJobsResponseTypeDef",
     {
         "jobs": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchQuantumTasksResponseTypeDef = TypedDict(
     "SearchQuantumTasksResponseTypeDef",
     {
         "nextToken": str,
         "quantumTasks": List[QuantumTaskSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchDevicesRequestRequestTypeDef",
     {
         "filters": Sequence[SearchDevicesFilterTypeDef],
@@ -531,43 +516,39 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class SearchDevicesRequestRequestTypeDef(
     _RequiredSearchDevicesRequestRequestTypeDef, _OptionalSearchDevicesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef = TypedDict(
     "_RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef",
     {
         "filters": Sequence[SearchDevicesFilterTypeDef],
     },
 )
 _OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef = TypedDict(
     "_OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchDevicesRequestSearchDevicesPaginateTypeDef(
     _RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef,
     _OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSearchJobsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchJobsRequestRequestTypeDef",
     {
         "filters": Sequence[SearchJobsFilterTypeDef],
     },
 )
 _OptionalSearchJobsRequestRequestTypeDef = TypedDict(
@@ -575,43 +556,39 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class SearchJobsRequestRequestTypeDef(
     _RequiredSearchJobsRequestRequestTypeDef, _OptionalSearchJobsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSearchJobsRequestSearchJobsPaginateTypeDef = TypedDict(
     "_RequiredSearchJobsRequestSearchJobsPaginateTypeDef",
     {
         "filters": Sequence[SearchJobsFilterTypeDef],
     },
 )
 _OptionalSearchJobsRequestSearchJobsPaginateTypeDef = TypedDict(
     "_OptionalSearchJobsRequestSearchJobsPaginateTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchJobsRequestSearchJobsPaginateTypeDef(
     _RequiredSearchJobsRequestSearchJobsPaginateTypeDef,
     _OptionalSearchJobsRequestSearchJobsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSearchQuantumTasksRequestRequestTypeDef = TypedDict(
     "_RequiredSearchQuantumTasksRequestRequestTypeDef",
     {
         "filters": Sequence[SearchQuantumTasksFilterTypeDef],
     },
 )
 _OptionalSearchQuantumTasksRequestRequestTypeDef = TypedDict(
@@ -619,44 +596,40 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class SearchQuantumTasksRequestRequestTypeDef(
     _RequiredSearchQuantumTasksRequestRequestTypeDef,
     _OptionalSearchQuantumTasksRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef = TypedDict(
     "_RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
     {
         "filters": Sequence[SearchQuantumTasksFilterTypeDef],
     },
 )
 _OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef = TypedDict(
     "_OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef(
     _RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
     _OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
 ):
     pass
 
-
 _RequiredInputFileConfigTypeDef = TypedDict(
     "_RequiredInputFileConfigTypeDef",
     {
         "channelName": str,
         "dataSource": DataSourceTypeDef,
     },
 )
@@ -664,19 +637,17 @@
     "_OptionalInputFileConfigTypeDef",
     {
         "contentType": str,
     },
     total=False,
 )
 
-
 class InputFileConfigTypeDef(_RequiredInputFileConfigTypeDef, _OptionalInputFileConfigTypeDef):
     pass
 
-
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "algorithmSpecification": AlgorithmSpecificationTypeDef,
         "clientToken": str,
         "deviceConfig": DeviceConfigTypeDef,
         "instanceConfig": InstanceConfigTypeDef,
@@ -693,21 +664,19 @@
         "inputDataConfig": Sequence[InputFileConfigTypeDef],
         "stoppingCondition": JobStoppingConditionTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
-
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "algorithmSpecification": AlgorithmSpecificationTypeDef,
         "billableDuration": int,
         "checkpointConfig": JobCheckpointConfigTypeDef,
         "createdAt": datetime,
@@ -722,10 +691,10 @@
         "jobName": str,
         "outputDataConfig": JobOutputDataConfigTypeDef,
         "roleArn": str,
         "startedAt": datetime,
         "status": JobPrimaryStatusType,
         "stoppingCondition": JobStoppingConditionTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket/type_defs.pyi` & `mypy-boto3-braket-1.27.0/mypy_boto3_braket/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,49 +29,50 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ContainerImageTypeDef",
     "ScriptModeConfigTypeDef",
     "CancelJobRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelJobResponseTypeDef",
     "CancelQuantumTaskRequestRequestTypeDef",
+    "CancelQuantumTaskResponseTypeDef",
     "DeviceConfigTypeDef",
     "InstanceConfigTypeDef",
     "JobCheckpointConfigTypeDef",
     "JobOutputDataConfigTypeDef",
     "JobStoppingConditionTypeDef",
+    "CreateJobResponseTypeDef",
     "CreateQuantumTaskRequestRequestTypeDef",
+    "CreateQuantumTaskResponseTypeDef",
     "S3DataSourceTypeDef",
     "DeviceSummaryTypeDef",
     "GetDeviceRequestRequestTypeDef",
+    "GetDeviceResponseTypeDef",
     "GetJobRequestRequestTypeDef",
     "JobEventDetailsTypeDef",
     "GetQuantumTaskRequestRequestTypeDef",
+    "GetQuantumTaskResponseTypeDef",
     "JobSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "QuantumTaskSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "SearchDevicesFilterTypeDef",
     "SearchJobsFilterTypeDef",
     "SearchQuantumTasksFilterTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AlgorithmSpecificationTypeDef",
-    "CancelJobResponseTypeDef",
-    "CancelQuantumTaskResponseTypeDef",
-    "CreateJobResponseTypeDef",
-    "CreateQuantumTaskResponseTypeDef",
-    "GetDeviceResponseTypeDef",
-    "GetQuantumTaskResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "DataSourceTypeDef",
     "SearchDevicesResponseTypeDef",
     "SearchJobsResponseTypeDef",
     "SearchQuantumTasksResponseTypeDef",
     "SearchDevicesRequestRequestTypeDef",
     "SearchDevicesRequestSearchDevicesPaginateTypeDef",
     "SearchJobsRequestRequestTypeDef",
@@ -101,43 +102,52 @@
     "_OptionalScriptModeConfigTypeDef",
     {
         "compressionType": CompressionTypeType,
     },
     total=False,
 )
 
+
 class ScriptModeConfigTypeDef(_RequiredScriptModeConfigTypeDef, _OptionalScriptModeConfigTypeDef):
     pass
 
+
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelJobResponseTypeDef = TypedDict(
+    "CancelJobResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "cancellationStatus": CancellationStatusType,
+        "jobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CancelQuantumTaskRequestRequestTypeDef = TypedDict(
     "CancelQuantumTaskRequestRequestTypeDef",
     {
         "clientToken": str,
         "quantumTaskArn": str,
     },
 )
 
+CancelQuantumTaskResponseTypeDef = TypedDict(
+    "CancelQuantumTaskResponseTypeDef",
+    {
+        "cancellationStatus": CancellationStatusType,
+        "quantumTaskArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeviceConfigTypeDef = TypedDict(
     "DeviceConfigTypeDef",
     {
         "device": str,
     },
 )
 
@@ -152,63 +162,77 @@
     "_OptionalInstanceConfigTypeDef",
     {
         "instanceCount": int,
     },
     total=False,
 )
 
+
 class InstanceConfigTypeDef(_RequiredInstanceConfigTypeDef, _OptionalInstanceConfigTypeDef):
     pass
 
+
 _RequiredJobCheckpointConfigTypeDef = TypedDict(
     "_RequiredJobCheckpointConfigTypeDef",
     {
         "s3Uri": str,
     },
 )
 _OptionalJobCheckpointConfigTypeDef = TypedDict(
     "_OptionalJobCheckpointConfigTypeDef",
     {
         "localPath": str,
     },
     total=False,
 )
 
+
 class JobCheckpointConfigTypeDef(
     _RequiredJobCheckpointConfigTypeDef, _OptionalJobCheckpointConfigTypeDef
 ):
     pass
 
+
 _RequiredJobOutputDataConfigTypeDef = TypedDict(
     "_RequiredJobOutputDataConfigTypeDef",
     {
         "s3Path": str,
     },
 )
 _OptionalJobOutputDataConfigTypeDef = TypedDict(
     "_OptionalJobOutputDataConfigTypeDef",
     {
         "kmsKeyId": str,
     },
     total=False,
 )
 
+
 class JobOutputDataConfigTypeDef(
     _RequiredJobOutputDataConfigTypeDef, _OptionalJobOutputDataConfigTypeDef
 ):
     pass
 
+
 JobStoppingConditionTypeDef = TypedDict(
     "JobStoppingConditionTypeDef",
     {
         "maxRuntimeInSeconds": int,
     },
     total=False,
 )
 
+CreateJobResponseTypeDef = TypedDict(
+    "CreateJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateQuantumTaskRequestRequestTypeDef = TypedDict(
     "_RequiredCreateQuantumTaskRequestRequestTypeDef",
     {
         "action": str,
         "clientToken": str,
         "deviceArn": str,
         "outputS3Bucket": str,
@@ -222,19 +246,29 @@
         "deviceParameters": str,
         "jobToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateQuantumTaskRequestRequestTypeDef(
     _RequiredCreateQuantumTaskRequestRequestTypeDef, _OptionalCreateQuantumTaskRequestRequestTypeDef
 ):
     pass
 
+
+CreateQuantumTaskResponseTypeDef = TypedDict(
+    "CreateQuantumTaskResponseTypeDef",
+    {
+        "quantumTaskArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 S3DataSourceTypeDef = TypedDict(
     "S3DataSourceTypeDef",
     {
         "s3Uri": str,
     },
 )
 
@@ -252,14 +286,27 @@
 GetDeviceRequestRequestTypeDef = TypedDict(
     "GetDeviceRequestRequestTypeDef",
     {
         "deviceArn": str,
     },
 )
 
+GetDeviceResponseTypeDef = TypedDict(
+    "GetDeviceResponseTypeDef",
+    {
+        "deviceArn": str,
+        "deviceCapabilities": str,
+        "deviceName": str,
+        "deviceStatus": DeviceStatusType,
+        "deviceType": DeviceTypeType,
+        "providerName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetJobRequestRequestTypeDef = TypedDict(
     "GetJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
@@ -276,14 +323,33 @@
 GetQuantumTaskRequestRequestTypeDef = TypedDict(
     "GetQuantumTaskRequestRequestTypeDef",
     {
         "quantumTaskArn": str,
     },
 )
 
+GetQuantumTaskResponseTypeDef = TypedDict(
+    "GetQuantumTaskResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "deviceArn": str,
+        "deviceParameters": str,
+        "endedAt": datetime,
+        "failureReason": str,
+        "jobArn": str,
+        "outputS3Bucket": str,
+        "outputS3Directory": str,
+        "quantumTaskArn": str,
+        "shots": int,
+        "status": QuantumTaskStatusType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredJobSummaryTypeDef = TypedDict(
     "_RequiredJobSummaryTypeDef",
     {
         "createdAt": datetime,
         "device": str,
         "jobArn": str,
         "jobName": str,
@@ -296,24 +362,34 @@
         "endedAt": datetime,
         "startedAt": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class JobSummaryTypeDef(_RequiredJobSummaryTypeDef, _OptionalJobSummaryTypeDef):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -337,19 +413,32 @@
     {
         "endedAt": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class QuantumTaskSummaryTypeDef(
     _RequiredQuantumTaskSummaryTypeDef, _OptionalQuantumTaskSummaryTypeDef
 ):
     pass
 
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
 SearchDevicesFilterTypeDef = TypedDict(
     "SearchDevicesFilterTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
 )
@@ -393,119 +482,45 @@
     {
         "containerImage": ContainerImageTypeDef,
         "scriptModeConfig": ScriptModeConfigTypeDef,
     },
     total=False,
 )
 
-CancelJobResponseTypeDef = TypedDict(
-    "CancelJobResponseTypeDef",
-    {
-        "cancellationStatus": CancellationStatusType,
-        "jobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelQuantumTaskResponseTypeDef = TypedDict(
-    "CancelQuantumTaskResponseTypeDef",
-    {
-        "cancellationStatus": CancellationStatusType,
-        "quantumTaskArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobResponseTypeDef = TypedDict(
-    "CreateJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateQuantumTaskResponseTypeDef = TypedDict(
-    "CreateQuantumTaskResponseTypeDef",
-    {
-        "quantumTaskArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDeviceResponseTypeDef = TypedDict(
-    "GetDeviceResponseTypeDef",
-    {
-        "deviceArn": str,
-        "deviceCapabilities": str,
-        "deviceName": str,
-        "deviceStatus": DeviceStatusType,
-        "deviceType": DeviceTypeType,
-        "providerName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetQuantumTaskResponseTypeDef = TypedDict(
-    "GetQuantumTaskResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "deviceArn": str,
-        "deviceParameters": str,
-        "endedAt": datetime,
-        "failureReason": str,
-        "jobArn": str,
-        "outputS3Bucket": str,
-        "outputS3Directory": str,
-        "quantumTaskArn": str,
-        "shots": int,
-        "status": QuantumTaskStatusType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "s3DataSource": S3DataSourceTypeDef,
     },
 )
 
 SearchDevicesResponseTypeDef = TypedDict(
     "SearchDevicesResponseTypeDef",
     {
         "devices": List[DeviceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchJobsResponseTypeDef = TypedDict(
     "SearchJobsResponseTypeDef",
     {
         "jobs": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchQuantumTasksResponseTypeDef = TypedDict(
     "SearchQuantumTasksResponseTypeDef",
     {
         "nextToken": str,
         "quantumTasks": List[QuantumTaskSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchDevicesRequestRequestTypeDef",
     {
         "filters": Sequence[SearchDevicesFilterTypeDef],
@@ -516,39 +531,43 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class SearchDevicesRequestRequestTypeDef(
     _RequiredSearchDevicesRequestRequestTypeDef, _OptionalSearchDevicesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef = TypedDict(
     "_RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef",
     {
         "filters": Sequence[SearchDevicesFilterTypeDef],
     },
 )
 _OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef = TypedDict(
     "_OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchDevicesRequestSearchDevicesPaginateTypeDef(
     _RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef,
     _OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSearchJobsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchJobsRequestRequestTypeDef",
     {
         "filters": Sequence[SearchJobsFilterTypeDef],
     },
 )
 _OptionalSearchJobsRequestRequestTypeDef = TypedDict(
@@ -556,39 +575,43 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class SearchJobsRequestRequestTypeDef(
     _RequiredSearchJobsRequestRequestTypeDef, _OptionalSearchJobsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSearchJobsRequestSearchJobsPaginateTypeDef = TypedDict(
     "_RequiredSearchJobsRequestSearchJobsPaginateTypeDef",
     {
         "filters": Sequence[SearchJobsFilterTypeDef],
     },
 )
 _OptionalSearchJobsRequestSearchJobsPaginateTypeDef = TypedDict(
     "_OptionalSearchJobsRequestSearchJobsPaginateTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchJobsRequestSearchJobsPaginateTypeDef(
     _RequiredSearchJobsRequestSearchJobsPaginateTypeDef,
     _OptionalSearchJobsRequestSearchJobsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSearchQuantumTasksRequestRequestTypeDef = TypedDict(
     "_RequiredSearchQuantumTasksRequestRequestTypeDef",
     {
         "filters": Sequence[SearchQuantumTasksFilterTypeDef],
     },
 )
 _OptionalSearchQuantumTasksRequestRequestTypeDef = TypedDict(
@@ -596,40 +619,44 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class SearchQuantumTasksRequestRequestTypeDef(
     _RequiredSearchQuantumTasksRequestRequestTypeDef,
     _OptionalSearchQuantumTasksRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef = TypedDict(
     "_RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
     {
         "filters": Sequence[SearchQuantumTasksFilterTypeDef],
     },
 )
 _OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef = TypedDict(
     "_OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef(
     _RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
     _OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
 ):
     pass
 
+
 _RequiredInputFileConfigTypeDef = TypedDict(
     "_RequiredInputFileConfigTypeDef",
     {
         "channelName": str,
         "dataSource": DataSourceTypeDef,
     },
 )
@@ -637,17 +664,19 @@
     "_OptionalInputFileConfigTypeDef",
     {
         "contentType": str,
     },
     total=False,
 )
 
+
 class InputFileConfigTypeDef(_RequiredInputFileConfigTypeDef, _OptionalInputFileConfigTypeDef):
     pass
 
+
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "algorithmSpecification": AlgorithmSpecificationTypeDef,
         "clientToken": str,
         "deviceConfig": DeviceConfigTypeDef,
         "instanceConfig": InstanceConfigTypeDef,
@@ -664,19 +693,21 @@
         "inputDataConfig": Sequence[InputFileConfigTypeDef],
         "stoppingCondition": JobStoppingConditionTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
+
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "algorithmSpecification": AlgorithmSpecificationTypeDef,
         "billableDuration": int,
         "checkpointConfig": JobCheckpointConfigTypeDef,
         "createdAt": datetime,
@@ -691,10 +722,10 @@
         "jobName": str,
         "outputDataConfig": JobOutputDataConfigTypeDef,
         "roleArn": str,
         "startedAt": datetime,
         "status": JobPrimaryStatusType,
         "stoppingCondition": JobStoppingConditionTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket.egg-info/PKG-INFO` & `mypy-boto3-braket-1.27.0/mypy_boto3_braket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-braket
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Braket 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Braket 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/
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
 
 <a id="mypy-boto3-braket"></a>
 
 # mypy-boto3-braket
 
 [![PyPI - mypy-boto3-braket](https://img.shields.io/pypi/v/mypy-boto3-braket.svg?color=blue)](https://pypi.org/project/mypy-boto3-braket)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-braket.svg?color=blue)](https://pypi.org/project/mypy-boto3-braket)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-braket?color=blue)](https://pypistats.org/packages/mypy-boto3-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Braket 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
+[boto3.Braket 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
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
 [mypy-boto3-braket docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,45 +341,45 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_braket.type_defs import (
     ContainerImageTypeDef,
     ScriptModeConfigTypeDef,
     CancelJobRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJobResponseTypeDef,
     CancelQuantumTaskRequestRequestTypeDef,
+    CancelQuantumTaskResponseTypeDef,
     DeviceConfigTypeDef,
     InstanceConfigTypeDef,
     JobCheckpointConfigTypeDef,
     JobOutputDataConfigTypeDef,
     JobStoppingConditionTypeDef,
+    CreateJobResponseTypeDef,
     CreateQuantumTaskRequestRequestTypeDef,
+    CreateQuantumTaskResponseTypeDef,
     S3DataSourceTypeDef,
     DeviceSummaryTypeDef,
     GetDeviceRequestRequestTypeDef,
+    GetDeviceResponseTypeDef,
     GetJobRequestRequestTypeDef,
     JobEventDetailsTypeDef,
     GetQuantumTaskRequestRequestTypeDef,
+    GetQuantumTaskResponseTypeDef,
     JobSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     QuantumTaskSummaryTypeDef,
+    ResponseMetadataTypeDef,
     SearchDevicesFilterTypeDef,
     SearchJobsFilterTypeDef,
     SearchQuantumTasksFilterTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AlgorithmSpecificationTypeDef,
-    CancelJobResponseTypeDef,
-    CancelQuantumTaskResponseTypeDef,
-    CreateJobResponseTypeDef,
-    CreateQuantumTaskResponseTypeDef,
-    GetDeviceResponseTypeDef,
-    GetQuantumTaskResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     DataSourceTypeDef,
     SearchDevicesResponseTypeDef,
     SearchJobsResponseTypeDef,
     SearchQuantumTasksResponseTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchJobsRequestRequestTypeDef,
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

### Comparing `mypy-boto3-braket-1.26.0.post1/mypy_boto3_braket.egg-info/SOURCES.txt` & `mypy-boto3-braket-1.27.0/mypy_boto3_braket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.26.0.post1/setup.py` & `mypy-boto3-braket-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-braket.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-braket",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_braket"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Braket 1.26.0 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.Braket 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 braket type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_braket": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_braket": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/",
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


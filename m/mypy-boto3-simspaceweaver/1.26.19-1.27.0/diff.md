# Comparing `tmp/mypy-boto3-simspaceweaver-1.26.19.tar.gz` & `tmp/mypy-boto3-simspaceweaver-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-simspaceweaver-1.26.19.tar", last modified: Tue Nov 29 20:35:12 2022, max compression
+gzip compressed data, was "mypy-boto3-simspaceweaver-1.27.0.tar", last modified: Mon Jul  3 19:51:28 2023, max compression
```

## Comparing `mypy-boto3-simspaceweaver-1.26.19.tar` & `mypy-boto3-simspaceweaver-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:12.121234 mypy-boto3-simspaceweaver-1.26.19/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    13509 2022-11-29 20:35:12.121234 mypy-boto3-simspaceweaver-1.26.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12044 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:12.117234 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/
--rw-r--r--   0 runner    (1001) docker     (122)      429 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      936 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11206 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    11185 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     8118 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)     8116 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    10034 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10027 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 20:35:12.121234 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    13509 2022-11-29 20:35:11.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      734 2022-11-29 20:35:11.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 20:35:11.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 20:35:11.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-29 20:35:11.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2022-11-29 20:35:11.000000 mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-29 20:35:12.121234 mypy-boto3-simspaceweaver-1.26.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2013 2022-11-29 20:35:01.000000 mypy-boto3-simspaceweaver-1.26.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:28.764020 mypy-boto3-simspaceweaver-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:14.000000 mypy-boto3-simspaceweaver-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-07-03 19:51:28.764020 mypy-boto3-simspaceweaver-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-03 19:48:14.000000 mypy-boto3-simspaceweaver-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:28.756020 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-03 19:48:14.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-03 19:48:14.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 19:48:14.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-07-03 19:48:14.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-03 19:48:14.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-03 19:48:14.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-03 19:48:14.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:14.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-07-03 19:48:15.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-07-03 19:48:14.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:14.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:28.764020 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-07-03 19:51:28.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-03 19:51:28.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:28.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:28.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:28.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:51:28.000000 mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:28.764020 mypy-boto3-simspaceweaver-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-03 19:48:14.000000 mypy-boto3-simspaceweaver-1.27.0/setup.py
```

### Comparing `mypy-boto3-simspaceweaver-1.26.19/LICENSE` & `mypy-boto3-simspaceweaver-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-simspaceweaver-1.26.19/PKG-INFO` & `mypy-boto3-simspaceweaver-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-simspaceweaver
-Version: 1.26.19
-Summary: Type annotations for boto3.SimSpaceWeaver 1.26.19 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.SimSpaceWeaver 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/
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
 
 <a id="mypy-boto3-simspaceweaver"></a>
 
 # mypy-boto3-simspaceweaver
 
 [![PyPI - mypy-boto3-simspaceweaver](https://img.shields.io/pypi/v/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-simspaceweaver?color=blue)](https://pypistats.org/packages/mypy-boto3-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimSpaceWeaver 1.26.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[boto3.SimSpaceWeaver 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
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
 [mypy-boto3-simspaceweaver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,40 +305,42 @@
 
 `mypy_boto3_simspaceweaver.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_simspaceweaver.type_defs import (
     CloudWatchLogsLogGroupTypeDef,
+    S3DestinationTypeDef,
     DeleteAppInputRequestTypeDef,
     DeleteSimulationInputRequestTypeDef,
     DescribeAppInputRequestTypeDef,
     LaunchOverridesTypeDef,
-    ResponseMetadataTypeDef,
     DescribeSimulationInputRequestTypeDef,
     S3LocationTypeDef,
     DomainTypeDef,
     ListAppsInputRequestTypeDef,
     SimulationAppMetadataTypeDef,
     ListSimulationsInputRequestTypeDef,
     SimulationMetadataTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     SimulationClockTypeDef,
+    ResponseMetadataTypeDef,
     SimulationAppPortMappingTypeDef,
+    StartAppOutputTypeDef,
     StartClockInputRequestTypeDef,
+    StartSimulationOutputTypeDef,
     StopAppInputRequestTypeDef,
     StopClockInputRequestTypeDef,
     StopSimulationInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     LogDestinationTypeDef,
+    CreateSnapshotInputRequestTypeDef,
     StartAppInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    StartAppOutputTypeDef,
-    StartSimulationOutputTypeDef,
     StartSimulationInputRequestTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     LiveSimulationStateTypeDef,
     SimulationAppEndpointInfoTypeDef,
     LoggingConfigurationTypeDef,
     DescribeAppOutputTypeDef,
@@ -352,42 +355,42 @@
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

### Comparing `mypy-boto3-simspaceweaver-1.26.19/README.md` & `mypy-boto3-simspaceweaver-1.27.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-simspaceweaver"></a>
 
 # mypy-boto3-simspaceweaver
 
 [![PyPI - mypy-boto3-simspaceweaver](https://img.shields.io/pypi/v/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-simspaceweaver?color=blue)](https://pypistats.org/packages/mypy-boto3-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimSpaceWeaver 1.26.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[boto3.SimSpaceWeaver 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
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
 [mypy-boto3-simspaceweaver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -273,40 +273,42 @@
 
 `mypy_boto3_simspaceweaver.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_simspaceweaver.type_defs import (
     CloudWatchLogsLogGroupTypeDef,
+    S3DestinationTypeDef,
     DeleteAppInputRequestTypeDef,
     DeleteSimulationInputRequestTypeDef,
     DescribeAppInputRequestTypeDef,
     LaunchOverridesTypeDef,
-    ResponseMetadataTypeDef,
     DescribeSimulationInputRequestTypeDef,
     S3LocationTypeDef,
     DomainTypeDef,
     ListAppsInputRequestTypeDef,
     SimulationAppMetadataTypeDef,
     ListSimulationsInputRequestTypeDef,
     SimulationMetadataTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     SimulationClockTypeDef,
+    ResponseMetadataTypeDef,
     SimulationAppPortMappingTypeDef,
+    StartAppOutputTypeDef,
     StartClockInputRequestTypeDef,
+    StartSimulationOutputTypeDef,
     StopAppInputRequestTypeDef,
     StopClockInputRequestTypeDef,
     StopSimulationInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     LogDestinationTypeDef,
+    CreateSnapshotInputRequestTypeDef,
     StartAppInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    StartAppOutputTypeDef,
-    StartSimulationOutputTypeDef,
     StartSimulationInputRequestTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     LiveSimulationStateTypeDef,
     SimulationAppEndpointInfoTypeDef,
     LoggingConfigurationTypeDef,
     DescribeAppOutputTypeDef,
@@ -321,42 +323,42 @@
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

### Comparing `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/__main__.py` & `mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SimSpaceWeaver 1.26.19\nVersion:         1.26.19\nBuilder"
-        " version: 7.11.11\nDocs:           "
+        "Type annotations for boto3.SimSpaceWeaver 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.19")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/client.py` & `mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .type_defs import (
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
     LaunchOverridesTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    S3DestinationTypeDef,
     S3LocationTypeDef,
     StartAppOutputTypeDef,
     StartSimulationOutputTypeDef,
 )
 
 __all__ = ("SimSpaceWeaverClient",)
 
@@ -80,14 +81,24 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#close)
         """
 
+    def create_snapshot(
+        self, *, Destination: S3DestinationTypeDef, Simulation: str
+    ) -> Dict[str, Any]:
+        """
+        Creates a snapshot of the specified simulation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.create_snapshot)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#create_snapshot)
+        """
+
     def delete_app(self, *, App: str, Domain: str, Simulation: str) -> Dict[str, Any]:
         """
         Deletes the instance of the given custom app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.delete_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#delete_app)
         """
@@ -106,15 +117,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.describe_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#describe_app)
         """
 
     def describe_simulation(self, *, Simulation: str) -> DescribeSimulationOutputTypeDef:
         """
-        .
+        Returns the current state of the given simulation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.describe_simulation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#describe_simulation)
         """
 
     def generate_presigned_url(
         self,
@@ -185,22 +196,23 @@
         """
 
     def start_simulation(
         self,
         *,
         Name: str,
         RoleArn: str,
-        SchemaS3Location: S3LocationTypeDef,
         ClientToken: str = ...,
         Description: str = ...,
         MaximumDuration: str = ...,
+        SchemaS3Location: S3LocationTypeDef = ...,
+        SnapshotS3Location: S3LocationTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> StartSimulationOutputTypeDef:
         """
-        .
+        Starts a simulation with the given name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.start_simulation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#start_simulation)
         """
 
     def stop_app(self, *, App: str, Domain: str, Simulation: str) -> Dict[str, Any]:
         """
```

### Comparing `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/client.pyi` & `mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .type_defs import (
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
     LaunchOverridesTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    S3DestinationTypeDef,
     S3LocationTypeDef,
     StartAppOutputTypeDef,
     StartSimulationOutputTypeDef,
 )
 
 __all__ = ("SimSpaceWeaverClient",)
 
@@ -74,14 +75,23 @@
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#close)
         """
+    def create_snapshot(
+        self, *, Destination: S3DestinationTypeDef, Simulation: str
+    ) -> Dict[str, Any]:
+        """
+        Creates a snapshot of the specified simulation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.create_snapshot)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#create_snapshot)
+        """
     def delete_app(self, *, App: str, Domain: str, Simulation: str) -> Dict[str, Any]:
         """
         Deletes the instance of the given custom app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.delete_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#delete_app)
         """
@@ -97,15 +107,15 @@
         Returns the state of the given custom app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.describe_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#describe_app)
         """
     def describe_simulation(self, *, Simulation: str) -> DescribeSimulationOutputTypeDef:
         """
-        .
+        Returns the current state of the given simulation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.describe_simulation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#describe_simulation)
         """
     def generate_presigned_url(
         self,
         ClientMethod: str,
@@ -169,22 +179,23 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#start_clock)
         """
     def start_simulation(
         self,
         *,
         Name: str,
         RoleArn: str,
-        SchemaS3Location: S3LocationTypeDef,
         ClientToken: str = ...,
         Description: str = ...,
         MaximumDuration: str = ...,
+        SchemaS3Location: S3LocationTypeDef = ...,
+        SnapshotS3Location: S3LocationTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> StartSimulationOutputTypeDef:
         """
-        .
+        Starts a simulation with the given name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.start_simulation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/client/#start_simulation)
         """
     def stop_app(self, *, App: str, Domain: str, Simulation: str) -> Dict[str, Any]:
         """
         Stops the given custom app and shuts down all of its allocated compute
```

### Comparing `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/literals.py` & `mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,23 @@
 ClockTargetStatusType = Literal["STARTED", "STOPPED", "UNKNOWN"]
 LifecycleManagementStrategyType = Literal[
     "ByRequest", "BySpatialSubdivision", "PerWorker", "Unknown"
 ]
 SimulationAppStatusType = Literal["ERROR", "STARTED", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"]
 SimulationAppTargetStatusType = Literal["STARTED", "STOPPED", "UNKNOWN"]
 SimulationStatusType = Literal[
-    "DELETED", "DELETING", "FAILED", "STARTED", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"
+    "DELETED",
+    "DELETING",
+    "FAILED",
+    "SNAPSHOT_IN_PROGRESS",
+    "STARTED",
+    "STARTING",
+    "STOPPED",
+    "STOPPING",
+    "UNKNOWN",
 ]
 SimulationTargetStatusType = Literal["DELETED", "STARTED", "STOPPED", "UNKNOWN"]
 SimSpaceWeaverServiceName = Literal["simspaceweaver"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -57,14 +65,15 @@
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
@@ -85,30 +94,34 @@
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
@@ -134,14 +147,15 @@
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
@@ -186,14 +200,15 @@
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
@@ -204,34 +219,38 @@
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
@@ -244,14 +263,15 @@
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
@@ -270,24 +290,28 @@
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
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -315,14 +339,16 @@
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
@@ -356,18 +382,21 @@
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

### Comparing `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/literals.pyi` & `mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,23 @@
 ClockTargetStatusType = Literal["STARTED", "STOPPED", "UNKNOWN"]
 LifecycleManagementStrategyType = Literal[
     "ByRequest", "BySpatialSubdivision", "PerWorker", "Unknown"
 ]
 SimulationAppStatusType = Literal["ERROR", "STARTED", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"]
 SimulationAppTargetStatusType = Literal["STARTED", "STOPPED", "UNKNOWN"]
 SimulationStatusType = Literal[
-    "DELETED", "DELETING", "FAILED", "STARTED", "STARTING", "STOPPED", "STOPPING", "UNKNOWN"
+    "DELETED",
+    "DELETING",
+    "FAILED",
+    "SNAPSHOT_IN_PROGRESS",
+    "STARTED",
+    "STARTING",
+    "STOPPED",
+    "STOPPING",
+    "UNKNOWN",
 ]
 SimulationTargetStatusType = Literal["DELETED", "STARTED", "STOPPED", "UNKNOWN"]
 SimSpaceWeaverServiceName = Literal["simspaceweaver"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -55,14 +63,15 @@
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
@@ -83,30 +92,34 @@
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
@@ -132,14 +145,15 @@
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
@@ -184,14 +198,15 @@
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
@@ -202,34 +217,38 @@
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
@@ -242,14 +261,15 @@
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
@@ -268,24 +288,28 @@
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
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -313,14 +337,16 @@
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
@@ -354,18 +380,21 @@
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

### Comparing `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/type_defs.py` & `mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,40 +29,42 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CloudWatchLogsLogGroupTypeDef",
+    "S3DestinationTypeDef",
     "DeleteAppInputRequestTypeDef",
     "DeleteSimulationInputRequestTypeDef",
     "DescribeAppInputRequestTypeDef",
     "LaunchOverridesTypeDef",
-    "ResponseMetadataTypeDef",
     "DescribeSimulationInputRequestTypeDef",
     "S3LocationTypeDef",
     "DomainTypeDef",
     "ListAppsInputRequestTypeDef",
     "SimulationAppMetadataTypeDef",
     "ListSimulationsInputRequestTypeDef",
     "SimulationMetadataTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "SimulationClockTypeDef",
+    "ResponseMetadataTypeDef",
     "SimulationAppPortMappingTypeDef",
+    "StartAppOutputTypeDef",
     "StartClockInputRequestTypeDef",
+    "StartSimulationOutputTypeDef",
     "StopAppInputRequestTypeDef",
     "StopClockInputRequestTypeDef",
     "StopSimulationInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "LogDestinationTypeDef",
+    "CreateSnapshotInputRequestTypeDef",
     "StartAppInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "StartAppOutputTypeDef",
-    "StartSimulationOutputTypeDef",
     "StartSimulationInputRequestTypeDef",
     "ListAppsOutputTypeDef",
     "ListSimulationsOutputTypeDef",
     "LiveSimulationStateTypeDef",
     "SimulationAppEndpointInfoTypeDef",
     "LoggingConfigurationTypeDef",
     "DescribeAppOutputTypeDef",
@@ -73,14 +75,23 @@
     "CloudWatchLogsLogGroupTypeDef",
     {
         "LogGroupArn": str,
     },
     total=False,
 )
 
+S3DestinationTypeDef = TypedDict(
+    "S3DestinationTypeDef",
+    {
+        "BucketName": str,
+        "ObjectKeyPrefix": str,
+    },
+    total=False,
+)
+
 DeleteAppInputRequestTypeDef = TypedDict(
     "DeleteAppInputRequestTypeDef",
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
@@ -106,25 +117,14 @@
     "LaunchOverridesTypeDef",
     {
         "LaunchCommands": List[str],
     },
     total=False,
 )
 
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
 DescribeSimulationInputRequestTypeDef = TypedDict(
     "DescribeSimulationInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 
@@ -205,39 +205,78 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SimulationClockTypeDef = TypedDict(
     "SimulationClockTypeDef",
     {
         "Status": ClockStatusType,
         "TargetStatus": ClockTargetStatusType,
     },
     total=False,
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
 SimulationAppPortMappingTypeDef = TypedDict(
     "SimulationAppPortMappingTypeDef",
     {
         "Actual": int,
         "Declared": int,
     },
     total=False,
 )
 
+StartAppOutputTypeDef = TypedDict(
+    "StartAppOutputTypeDef",
+    {
+        "Domain": str,
+        "Name": str,
+        "Simulation": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartClockInputRequestTypeDef = TypedDict(
     "StartClockInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 
+StartSimulationOutputTypeDef = TypedDict(
+    "StartSimulationOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "ExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopAppInputRequestTypeDef = TypedDict(
     "StopAppInputRequestTypeDef",
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
@@ -277,14 +316,22 @@
     "LogDestinationTypeDef",
     {
         "CloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
     },
     total=False,
 )
 
+CreateSnapshotInputRequestTypeDef = TypedDict(
+    "CreateSnapshotInputRequestTypeDef",
+    {
+        "Destination": S3DestinationTypeDef,
+        "Simulation": str,
+    },
+)
+
 _RequiredStartAppInputRequestTypeDef = TypedDict(
     "_RequiredStartAppInputRequestTypeDef",
     {
         "Domain": str,
         "Name": str,
         "Simulation": str,
     },
@@ -302,56 +349,29 @@
 
 class StartAppInputRequestTypeDef(
     _RequiredStartAppInputRequestTypeDef, _OptionalStartAppInputRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartAppOutputTypeDef = TypedDict(
-    "StartAppOutputTypeDef",
-    {
-        "Domain": str,
-        "Name": str,
-        "Simulation": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartSimulationOutputTypeDef = TypedDict(
-    "StartSimulationOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "ExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredStartSimulationInputRequestTypeDef = TypedDict(
     "_RequiredStartSimulationInputRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
-        "SchemaS3Location": S3LocationTypeDef,
     },
 )
 _OptionalStartSimulationInputRequestTypeDef = TypedDict(
     "_OptionalStartSimulationInputRequestTypeDef",
     {
         "ClientToken": str,
         "Description": str,
         "MaximumDuration": str,
+        "SchemaS3Location": S3LocationTypeDef,
+        "SnapshotS3Location": S3LocationTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class StartSimulationInputRequestTypeDef(
@@ -361,24 +381,24 @@
 
 
 ListAppsOutputTypeDef = TypedDict(
     "ListAppsOutputTypeDef",
     {
         "Apps": List[SimulationAppMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSimulationsOutputTypeDef = TypedDict(
     "ListSimulationsOutputTypeDef",
     {
         "NextToken": str,
         "Simulations": List[SimulationMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LiveSimulationStateTypeDef = TypedDict(
     "LiveSimulationStateTypeDef",
     {
         "Clocks": List[SimulationClockTypeDef],
@@ -411,15 +431,15 @@
         "Domain": str,
         "EndpointInfo": SimulationAppEndpointInfoTypeDef,
         "LaunchOverrides": LaunchOverridesTypeDef,
         "Name": str,
         "Simulation": str,
         "Status": SimulationAppStatusType,
         "TargetStatus": SimulationAppTargetStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSimulationOutputTypeDef = TypedDict(
     "DescribeSimulationOutputTypeDef",
     {
         "Arn": str,
@@ -429,12 +449,14 @@
         "LiveSimulationState": LiveSimulationStateTypeDef,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
         "MaximumDuration": str,
         "Name": str,
         "RoleArn": str,
         "SchemaError": str,
         "SchemaS3Location": S3LocationTypeDef,
+        "SnapshotS3Location": S3LocationTypeDef,
+        "StartError": str,
         "Status": SimulationStatusType,
         "TargetStatus": SimulationTargetStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver/type_defs.pyi` & `mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -28,40 +28,42 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CloudWatchLogsLogGroupTypeDef",
+    "S3DestinationTypeDef",
     "DeleteAppInputRequestTypeDef",
     "DeleteSimulationInputRequestTypeDef",
     "DescribeAppInputRequestTypeDef",
     "LaunchOverridesTypeDef",
-    "ResponseMetadataTypeDef",
     "DescribeSimulationInputRequestTypeDef",
     "S3LocationTypeDef",
     "DomainTypeDef",
     "ListAppsInputRequestTypeDef",
     "SimulationAppMetadataTypeDef",
     "ListSimulationsInputRequestTypeDef",
     "SimulationMetadataTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "SimulationClockTypeDef",
+    "ResponseMetadataTypeDef",
     "SimulationAppPortMappingTypeDef",
+    "StartAppOutputTypeDef",
     "StartClockInputRequestTypeDef",
+    "StartSimulationOutputTypeDef",
     "StopAppInputRequestTypeDef",
     "StopClockInputRequestTypeDef",
     "StopSimulationInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "LogDestinationTypeDef",
+    "CreateSnapshotInputRequestTypeDef",
     "StartAppInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "StartAppOutputTypeDef",
-    "StartSimulationOutputTypeDef",
     "StartSimulationInputRequestTypeDef",
     "ListAppsOutputTypeDef",
     "ListSimulationsOutputTypeDef",
     "LiveSimulationStateTypeDef",
     "SimulationAppEndpointInfoTypeDef",
     "LoggingConfigurationTypeDef",
     "DescribeAppOutputTypeDef",
@@ -72,14 +74,23 @@
     "CloudWatchLogsLogGroupTypeDef",
     {
         "LogGroupArn": str,
     },
     total=False,
 )
 
+S3DestinationTypeDef = TypedDict(
+    "S3DestinationTypeDef",
+    {
+        "BucketName": str,
+        "ObjectKeyPrefix": str,
+    },
+    total=False,
+)
+
 DeleteAppInputRequestTypeDef = TypedDict(
     "DeleteAppInputRequestTypeDef",
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
@@ -105,25 +116,14 @@
     "LaunchOverridesTypeDef",
     {
         "LaunchCommands": List[str],
     },
     total=False,
 )
 
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
 DescribeSimulationInputRequestTypeDef = TypedDict(
     "DescribeSimulationInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 
@@ -202,39 +202,78 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SimulationClockTypeDef = TypedDict(
     "SimulationClockTypeDef",
     {
         "Status": ClockStatusType,
         "TargetStatus": ClockTargetStatusType,
     },
     total=False,
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
 SimulationAppPortMappingTypeDef = TypedDict(
     "SimulationAppPortMappingTypeDef",
     {
         "Actual": int,
         "Declared": int,
     },
     total=False,
 )
 
+StartAppOutputTypeDef = TypedDict(
+    "StartAppOutputTypeDef",
+    {
+        "Domain": str,
+        "Name": str,
+        "Simulation": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartClockInputRequestTypeDef = TypedDict(
     "StartClockInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 
+StartSimulationOutputTypeDef = TypedDict(
+    "StartSimulationOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "ExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopAppInputRequestTypeDef = TypedDict(
     "StopAppInputRequestTypeDef",
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
@@ -274,14 +313,22 @@
     "LogDestinationTypeDef",
     {
         "CloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
     },
     total=False,
 )
 
+CreateSnapshotInputRequestTypeDef = TypedDict(
+    "CreateSnapshotInputRequestTypeDef",
+    {
+        "Destination": S3DestinationTypeDef,
+        "Simulation": str,
+    },
+)
+
 _RequiredStartAppInputRequestTypeDef = TypedDict(
     "_RequiredStartAppInputRequestTypeDef",
     {
         "Domain": str,
         "Name": str,
         "Simulation": str,
     },
@@ -297,56 +344,29 @@
 )
 
 class StartAppInputRequestTypeDef(
     _RequiredStartAppInputRequestTypeDef, _OptionalStartAppInputRequestTypeDef
 ):
     pass
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartAppOutputTypeDef = TypedDict(
-    "StartAppOutputTypeDef",
-    {
-        "Domain": str,
-        "Name": str,
-        "Simulation": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartSimulationOutputTypeDef = TypedDict(
-    "StartSimulationOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "ExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredStartSimulationInputRequestTypeDef = TypedDict(
     "_RequiredStartSimulationInputRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
-        "SchemaS3Location": S3LocationTypeDef,
     },
 )
 _OptionalStartSimulationInputRequestTypeDef = TypedDict(
     "_OptionalStartSimulationInputRequestTypeDef",
     {
         "ClientToken": str,
         "Description": str,
         "MaximumDuration": str,
+        "SchemaS3Location": S3LocationTypeDef,
+        "SnapshotS3Location": S3LocationTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 class StartSimulationInputRequestTypeDef(
     _RequiredStartSimulationInputRequestTypeDef, _OptionalStartSimulationInputRequestTypeDef
@@ -354,24 +374,24 @@
     pass
 
 ListAppsOutputTypeDef = TypedDict(
     "ListAppsOutputTypeDef",
     {
         "Apps": List[SimulationAppMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSimulationsOutputTypeDef = TypedDict(
     "ListSimulationsOutputTypeDef",
     {
         "NextToken": str,
         "Simulations": List[SimulationMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LiveSimulationStateTypeDef = TypedDict(
     "LiveSimulationStateTypeDef",
     {
         "Clocks": List[SimulationClockTypeDef],
@@ -404,15 +424,15 @@
         "Domain": str,
         "EndpointInfo": SimulationAppEndpointInfoTypeDef,
         "LaunchOverrides": LaunchOverridesTypeDef,
         "Name": str,
         "Simulation": str,
         "Status": SimulationAppStatusType,
         "TargetStatus": SimulationAppTargetStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSimulationOutputTypeDef = TypedDict(
     "DescribeSimulationOutputTypeDef",
     {
         "Arn": str,
@@ -422,12 +442,14 @@
         "LiveSimulationState": LiveSimulationStateTypeDef,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
         "MaximumDuration": str,
         "Name": str,
         "RoleArn": str,
         "SchemaError": str,
         "SchemaS3Location": S3LocationTypeDef,
+        "SnapshotS3Location": S3LocationTypeDef,
+        "StartError": str,
         "Status": SimulationStatusType,
         "TargetStatus": SimulationTargetStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/PKG-INFO` & `mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-simspaceweaver
-Version: 1.26.19
-Summary: Type annotations for boto3.SimSpaceWeaver 1.26.19 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.SimSpaceWeaver 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/
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
 
 <a id="mypy-boto3-simspaceweaver"></a>
 
 # mypy-boto3-simspaceweaver
 
 [![PyPI - mypy-boto3-simspaceweaver](https://img.shields.io/pypi/v/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-simspaceweaver?color=blue)](https://pypistats.org/packages/mypy-boto3-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimSpaceWeaver 1.26.19](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[boto3.SimSpaceWeaver 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
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
 [mypy-boto3-simspaceweaver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,40 +305,42 @@
 
 `mypy_boto3_simspaceweaver.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_simspaceweaver.type_defs import (
     CloudWatchLogsLogGroupTypeDef,
+    S3DestinationTypeDef,
     DeleteAppInputRequestTypeDef,
     DeleteSimulationInputRequestTypeDef,
     DescribeAppInputRequestTypeDef,
     LaunchOverridesTypeDef,
-    ResponseMetadataTypeDef,
     DescribeSimulationInputRequestTypeDef,
     S3LocationTypeDef,
     DomainTypeDef,
     ListAppsInputRequestTypeDef,
     SimulationAppMetadataTypeDef,
     ListSimulationsInputRequestTypeDef,
     SimulationMetadataTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     SimulationClockTypeDef,
+    ResponseMetadataTypeDef,
     SimulationAppPortMappingTypeDef,
+    StartAppOutputTypeDef,
     StartClockInputRequestTypeDef,
+    StartSimulationOutputTypeDef,
     StopAppInputRequestTypeDef,
     StopClockInputRequestTypeDef,
     StopSimulationInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     LogDestinationTypeDef,
+    CreateSnapshotInputRequestTypeDef,
     StartAppInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    StartAppOutputTypeDef,
-    StartSimulationOutputTypeDef,
     StartSimulationInputRequestTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     LiveSimulationStateTypeDef,
     SimulationAppEndpointInfoTypeDef,
     LoggingConfigurationTypeDef,
     DescribeAppOutputTypeDef,
@@ -352,42 +355,42 @@
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

### Comparing `mypy-boto3-simspaceweaver-1.26.19/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt` & `mypy-boto3-simspaceweaver-1.27.0/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-simspaceweaver-1.26.19/setup.py` & `mypy-boto3-simspaceweaver-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-simspaceweaver.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-simspaceweaver",
-    version="1.26.19",
+    version="1.27.0",
     packages=["mypy_boto3_simspaceweaver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SimSpaceWeaver 1.26.19 service generated with"
-        " mypy-boto3-builder 7.11.11"
+        "Type annotations for boto3.SimSpaceWeaver 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 simspaceweaver type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_simspaceweaver": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_simspaceweaver": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/",
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


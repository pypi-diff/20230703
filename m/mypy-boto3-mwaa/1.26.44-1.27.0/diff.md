# Comparing `tmp/mypy-boto3-mwaa-1.26.44.tar.gz` & `tmp/mypy-boto3-mwaa-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mwaa-1.26.44.tar", last modified: Thu Jan  5 20:26:50 2023, max compression
+gzip compressed data, was "mypy-boto3-mwaa-1.27.0.tar", last modified: Mon Jul  3 19:51:10 2023, max compression
```

## Comparing `mypy-boto3-mwaa-1.26.44.tar` & `mypy-boto3-mwaa-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:50.947952 mypy-boto3-mwaa-1.26.44/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13646 2023-01-05 20:26:50.947952 mypy-boto3-mwaa-1.26.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:50.943952 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:50.943952 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13646 2023-01-05 20:26:50.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-01-05 20:26:50.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 20:26:50.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 20:26:50.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-05 20:26:50.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-05 20:26:50.000000 mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 20:26:50.947952 mypy-boto3-mwaa-1.26.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-01-05 20:26:32.000000 mypy-boto3-mwaa-1.26.44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.479722 mypy-boto3-mwaa-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-03 19:51:10.479722 mypy-boto3-mwaa-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.475722 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-07-03 19:42:36.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-07-03 19:42:36.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-07-03 19:42:36.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-07-03 19:42:36.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.479722 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-03 19:51:10.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-03 19:51:10.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:10.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 19:51:10.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:10.479722 mypy-boto3-mwaa-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/setup.py
```

### Comparing `mypy-boto3-mwaa-1.26.44/LICENSE` & `mypy-boto3-mwaa-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-mwaa-1.26.44/PKG-INFO` & `mypy-boto3-mwaa-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mwaa
-Version: 1.26.44
-Summary: Type annotations for boto3.MWAA 1.26.44 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.MWAA 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-mwaa"></a>
 
 # mypy-boto3-mwaa
 
 [![PyPI - mypy-boto3-mwaa](https://img.shields.io/pypi/v/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mwaa?color=blue)](https://pypistats.org/packages/mypy-boto3-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MWAA 1.26.44](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[boto3.MWAA 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mwaa docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,38 +324,38 @@
 
 `mypy_boto3_mwaa.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mwaa.type_defs import (
     CreateCliTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateCliTokenResponseTypeDef,
     NetworkConfigurationTypeDef,
+    CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenRequestRequestTypeDef,
+    CreateWebLoginTokenResponseTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DimensionTypeDef,
     GetEnvironmentInputRequestTypeDef,
     UpdateErrorTypeDef,
-    PaginatorConfigTypeDef,
+    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     ListEnvironmentsInputRequestTypeDef,
+    ListEnvironmentsOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ModuleLoggingConfigurationInputTypeDef,
     ModuleLoggingConfigurationTypeDef,
     StatisticSetTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
-    CreateCliTokenResponseTypeDef,
-    CreateEnvironmentOutputTypeDef,
-    CreateWebLoginTokenResponseTypeDef,
-    ListEnvironmentsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
     LastUpdateTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     LoggingConfigurationInputTypeDef,
     LoggingConfigurationTypeDef,
     MetricDatumTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
     EnvironmentTypeDef,
     PublishMetricsInputRequestTypeDef,
@@ -370,42 +370,42 @@
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

### Comparing `mypy-boto3-mwaa-1.26.44/README.md` & `mypy-boto3-mwaa-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mwaa"></a>
 
 # mypy-boto3-mwaa
 
 [![PyPI - mypy-boto3-mwaa](https://img.shields.io/pypi/v/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mwaa?color=blue)](https://pypistats.org/packages/mypy-boto3-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MWAA 1.26.44](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[boto3.MWAA 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mwaa docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/).
 
 See how it helps to find and fix potential bugs:
 
@@ -292,38 +292,38 @@
 
 `mypy_boto3_mwaa.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mwaa.type_defs import (
     CreateCliTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateCliTokenResponseTypeDef,
     NetworkConfigurationTypeDef,
+    CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenRequestRequestTypeDef,
+    CreateWebLoginTokenResponseTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DimensionTypeDef,
     GetEnvironmentInputRequestTypeDef,
     UpdateErrorTypeDef,
-    PaginatorConfigTypeDef,
+    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     ListEnvironmentsInputRequestTypeDef,
+    ListEnvironmentsOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ModuleLoggingConfigurationInputTypeDef,
     ModuleLoggingConfigurationTypeDef,
     StatisticSetTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
-    CreateCliTokenResponseTypeDef,
-    CreateEnvironmentOutputTypeDef,
-    CreateWebLoginTokenResponseTypeDef,
-    ListEnvironmentsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
     LastUpdateTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     LoggingConfigurationInputTypeDef,
     LoggingConfigurationTypeDef,
     MetricDatumTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
     EnvironmentTypeDef,
     PublishMetricsInputRequestTypeDef,
@@ -338,42 +338,42 @@
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

### Comparing `mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/__init__.py` & `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/__init__.pyi` & `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/__main__.py` & `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MWAA 1.26.44\nVersion:         1.26.44\nBuilder version:"
-        " 7.12.2\nDocs:           "
+        "Type annotations for boto3.MWAA 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.44")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/client.py` & `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,16 @@
         MaxWorkers: int = ...,
         MinWorkers: int = ...,
         PluginsS3ObjectVersion: str = ...,
         PluginsS3Path: str = ...,
         RequirementsS3ObjectVersion: str = ...,
         RequirementsS3Path: str = ...,
         Schedulers: int = ...,
+        StartupScriptS3ObjectVersion: str = ...,
+        StartupScriptS3Path: str = ...,
         Tags: Mapping[str, str] = ...,
         WebserverAccessMode: WebserverAccessModeType = ...,
         WeeklyMaintenanceWindowStart: str = ...
     ) -> CreateEnvironmentOutputTypeDef:
         """
         Creates an Amazon Managed Workflows for Apache Airflow (MWAA) environment.
 
@@ -231,14 +233,16 @@
         NetworkConfiguration: UpdateNetworkConfigurationInputTypeDef = ...,
         PluginsS3ObjectVersion: str = ...,
         PluginsS3Path: str = ...,
         RequirementsS3ObjectVersion: str = ...,
         RequirementsS3Path: str = ...,
         Schedulers: int = ...,
         SourceBucketArn: str = ...,
+        StartupScriptS3ObjectVersion: str = ...,
+        StartupScriptS3Path: str = ...,
         WebserverAccessMode: WebserverAccessModeType = ...,
         WeeklyMaintenanceWindowStart: str = ...
     ) -> UpdateEnvironmentOutputTypeDef:
         """
         Updates an Amazon Managed Workflows for Apache Airflow (MWAA) environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Client.update_environment)
```

### Comparing `mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/client.pyi` & `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,16 @@
         MaxWorkers: int = ...,
         MinWorkers: int = ...,
         PluginsS3ObjectVersion: str = ...,
         PluginsS3Path: str = ...,
         RequirementsS3ObjectVersion: str = ...,
         RequirementsS3Path: str = ...,
         Schedulers: int = ...,
+        StartupScriptS3ObjectVersion: str = ...,
+        StartupScriptS3Path: str = ...,
         Tags: Mapping[str, str] = ...,
         WebserverAccessMode: WebserverAccessModeType = ...,
         WeeklyMaintenanceWindowStart: str = ...
     ) -> CreateEnvironmentOutputTypeDef:
         """
         Creates an Amazon Managed Workflows for Apache Airflow (MWAA) environment.
 
@@ -213,14 +215,16 @@
         NetworkConfiguration: UpdateNetworkConfigurationInputTypeDef = ...,
         PluginsS3ObjectVersion: str = ...,
         PluginsS3Path: str = ...,
         RequirementsS3ObjectVersion: str = ...,
         RequirementsS3Path: str = ...,
         Schedulers: int = ...,
         SourceBucketArn: str = ...,
+        StartupScriptS3ObjectVersion: str = ...,
+        StartupScriptS3Path: str = ...,
         WebserverAccessMode: WebserverAccessModeType = ...,
         WeeklyMaintenanceWindowStart: str = ...
     ) -> UpdateEnvironmentOutputTypeDef:
         """
         Updates an Amazon Managed Workflows for Apache Airflow (MWAA) environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Client.update_environment)
```

### Comparing `mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/literals.py` & `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,16 +34,18 @@
 )
 
 
 EnvironmentStatusType = Literal[
     "AVAILABLE",
     "CREATE_FAILED",
     "CREATING",
+    "CREATING_SNAPSHOT",
     "DELETED",
     "DELETING",
+    "ROLLING_BACK",
     "UNAVAILABLE",
     "UPDATE_FAILED",
     "UPDATING",
 ]
 ListEnvironmentsPaginatorName = Literal["list_environments"]
 LoggingLevelType = Literal["CRITICAL", "DEBUG", "ERROR", "INFO", "WARNING"]
 UnitType = Literal[
@@ -89,14 +91,15 @@
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
@@ -117,31 +120,34 @@
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
@@ -220,14 +226,15 @@
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
@@ -238,18 +245,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -280,14 +289,15 @@
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
@@ -306,16 +316,19 @@
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
@@ -395,18 +408,21 @@
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

### Comparing `mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/literals.pyi` & `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,18 @@
     "RegionName",
 )
 
 EnvironmentStatusType = Literal[
     "AVAILABLE",
     "CREATE_FAILED",
     "CREATING",
+    "CREATING_SNAPSHOT",
     "DELETED",
     "DELETING",
+    "ROLLING_BACK",
     "UNAVAILABLE",
     "UPDATE_FAILED",
     "UPDATING",
 ]
 ListEnvironmentsPaginatorName = Literal["list_environments"]
 LoggingLevelType = Literal["CRITICAL", "DEBUG", "ERROR", "INFO", "WARNING"]
 UnitType = Literal[
@@ -87,14 +89,15 @@
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
@@ -115,31 +118,34 @@
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
@@ -218,14 +224,15 @@
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
@@ -236,18 +243,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -278,14 +287,15 @@
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
@@ -304,16 +314,19 @@
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
@@ -393,18 +406,21 @@
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

### Comparing `mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/paginator.py` & `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -23,31 +23,28 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import ListEnvironmentsOutputTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListEnvironmentsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/paginators/#listenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/paginator.pyi` & `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,28 +23,31 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import ListEnvironmentsOutputTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListEnvironmentsPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/paginators/#listenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/type_defs.py` & `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -24,41 +24,40 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CreateCliTokenRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateCliTokenResponseTypeDef",
     "NetworkConfigurationTypeDef",
+    "CreateEnvironmentOutputTypeDef",
     "CreateWebLoginTokenRequestRequestTypeDef",
+    "CreateWebLoginTokenResponseTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DimensionTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "UpdateErrorTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
+    "ListEnvironmentsOutputTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ModuleLoggingConfigurationInputTypeDef",
     "ModuleLoggingConfigurationTypeDef",
     "StatisticSetTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateNetworkConfigurationInputTypeDef",
-    "CreateCliTokenResponseTypeDef",
-    "CreateEnvironmentOutputTypeDef",
-    "CreateWebLoginTokenResponseTypeDef",
-    "ListEnvironmentsOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "UpdateEnvironmentOutputTypeDef",
     "LastUpdateTypeDef",
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "LoggingConfigurationInputTypeDef",
     "LoggingConfigurationTypeDef",
     "MetricDatumTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
     "EnvironmentTypeDef",
     "PublishMetricsInputRequestTypeDef",
@@ -68,41 +67,56 @@
 CreateCliTokenRequestRequestTypeDef = TypedDict(
     "CreateCliTokenRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateCliTokenResponseTypeDef = TypedDict(
+    "CreateCliTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "CliToken": str,
+        "WebServerHostname": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
+CreateEnvironmentOutputTypeDef = TypedDict(
+    "CreateEnvironmentOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateWebLoginTokenRequestRequestTypeDef = TypedDict(
     "CreateWebLoginTokenRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+CreateWebLoginTokenResponseTypeDef = TypedDict(
+    "CreateWebLoginTokenResponseTypeDef",
+    {
+        "WebServerHostname": str,
+        "WebToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteEnvironmentInputRequestTypeDef = TypedDict(
     "DeleteEnvironmentInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -126,40 +140,55 @@
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListEnvironmentsInputRequestTypeDef = TypedDict(
     "ListEnvironmentsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListEnvironmentsOutputTypeDef = TypedDict(
+    "ListEnvironmentsOutputTypeDef",
+    {
+        "Environments": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
 ModuleLoggingConfigurationInputTypeDef = TypedDict(
     "ModuleLoggingConfigurationInputTypeDef",
     {
         "Enabled": bool,
         "LogLevel": LoggingLevelType,
     },
 )
@@ -181,14 +210,35 @@
         "Minimum": float,
         "SampleCount": int,
         "Sum": float,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -204,84 +254,33 @@
 UpdateNetworkConfigurationInputTypeDef = TypedDict(
     "UpdateNetworkConfigurationInputTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
 )
 
-CreateCliTokenResponseTypeDef = TypedDict(
-    "CreateCliTokenResponseTypeDef",
-    {
-        "CliToken": str,
-        "WebServerHostname": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEnvironmentOutputTypeDef = TypedDict(
-    "CreateEnvironmentOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWebLoginTokenResponseTypeDef = TypedDict(
-    "CreateWebLoginTokenResponseTypeDef",
-    {
-        "WebServerHostname": str,
-        "WebToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListEnvironmentsOutputTypeDef = TypedDict(
-    "ListEnvironmentsOutputTypeDef",
-    {
-        "Environments": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateEnvironmentOutputTypeDef = TypedDict(
     "UpdateEnvironmentOutputTypeDef",
     {
         "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LastUpdateTypeDef = TypedDict(
     "LastUpdateTypeDef",
     {
         "CreatedAt": datetime,
         "Error": UpdateErrorTypeDef,
         "Source": str,
         "Status": UpdateStatusType,
     },
     total=False,
 )
 
-ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 LoggingConfigurationInputTypeDef = TypedDict(
     "LoggingConfigurationInputTypeDef",
     {
         "DagProcessingLogs": ModuleLoggingConfigurationInputTypeDef,
         "SchedulerLogs": ModuleLoggingConfigurationInputTypeDef,
         "TaskLogs": ModuleLoggingConfigurationInputTypeDef,
         "WebserverLogs": ModuleLoggingConfigurationInputTypeDef,
@@ -316,19 +315,17 @@
         "StatisticValues": StatisticSetTypeDef,
         "Unit": UnitType,
         "Value": float,
     },
     total=False,
 )
 
-
 class MetricDatumTypeDef(_RequiredMetricDatumTypeDef, _OptionalMetricDatumTypeDef):
     pass
 
-
 _RequiredCreateEnvironmentInputRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentInputRequestTypeDef",
     {
         "DagS3Path": str,
         "ExecutionRoleArn": str,
         "Name": str,
         "NetworkConfiguration": NetworkConfigurationTypeDef,
@@ -346,28 +343,28 @@
         "MaxWorkers": int,
         "MinWorkers": int,
         "PluginsS3ObjectVersion": str,
         "PluginsS3Path": str,
         "RequirementsS3ObjectVersion": str,
         "RequirementsS3Path": str,
         "Schedulers": int,
+        "StartupScriptS3ObjectVersion": str,
+        "StartupScriptS3Path": str,
         "Tags": Mapping[str, str],
         "WebserverAccessMode": WebserverAccessModeType,
         "WeeklyMaintenanceWindowStart": str,
     },
     total=False,
 )
 
-
 class CreateEnvironmentInputRequestTypeDef(
     _RequiredCreateEnvironmentInputRequestTypeDef, _OptionalCreateEnvironmentInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateEnvironmentInputRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateEnvironmentInputRequestTypeDef = TypedDict(
@@ -384,27 +381,27 @@
         "NetworkConfiguration": UpdateNetworkConfigurationInputTypeDef,
         "PluginsS3ObjectVersion": str,
         "PluginsS3Path": str,
         "RequirementsS3ObjectVersion": str,
         "RequirementsS3Path": str,
         "Schedulers": int,
         "SourceBucketArn": str,
+        "StartupScriptS3ObjectVersion": str,
+        "StartupScriptS3Path": str,
         "WebserverAccessMode": WebserverAccessModeType,
         "WeeklyMaintenanceWindowStart": str,
     },
     total=False,
 )
 
-
 class UpdateEnvironmentInputRequestTypeDef(
     _RequiredUpdateEnvironmentInputRequestTypeDef, _OptionalUpdateEnvironmentInputRequestTypeDef
 ):
     pass
 
-
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "AirflowConfigurationOptions": Dict[str, str],
         "AirflowVersion": str,
         "Arn": str,
         "CreatedAt": datetime,
@@ -421,14 +418,16 @@
         "PluginsS3ObjectVersion": str,
         "PluginsS3Path": str,
         "RequirementsS3ObjectVersion": str,
         "RequirementsS3Path": str,
         "Schedulers": int,
         "ServiceRoleArn": str,
         "SourceBucketArn": str,
+        "StartupScriptS3ObjectVersion": str,
+        "StartupScriptS3Path": str,
         "Status": EnvironmentStatusType,
         "Tags": Dict[str, str],
         "WebserverAccessMode": WebserverAccessModeType,
         "WebserverUrl": str,
         "WeeklyMaintenanceWindowStart": str,
     },
     total=False,
@@ -442,10 +441,10 @@
     },
 )
 
 GetEnvironmentOutputTypeDef = TypedDict(
     "GetEnvironmentOutputTypeDef",
     {
         "Environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa/type_defs.pyi` & `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,40 +24,41 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CreateCliTokenRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateCliTokenResponseTypeDef",
     "NetworkConfigurationTypeDef",
+    "CreateEnvironmentOutputTypeDef",
     "CreateWebLoginTokenRequestRequestTypeDef",
+    "CreateWebLoginTokenResponseTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DimensionTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "UpdateErrorTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
+    "ListEnvironmentsOutputTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ModuleLoggingConfigurationInputTypeDef",
     "ModuleLoggingConfigurationTypeDef",
     "StatisticSetTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateNetworkConfigurationInputTypeDef",
-    "CreateCliTokenResponseTypeDef",
-    "CreateEnvironmentOutputTypeDef",
-    "CreateWebLoginTokenResponseTypeDef",
-    "ListEnvironmentsOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "UpdateEnvironmentOutputTypeDef",
     "LastUpdateTypeDef",
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "LoggingConfigurationInputTypeDef",
     "LoggingConfigurationTypeDef",
     "MetricDatumTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
     "EnvironmentTypeDef",
     "PublishMetricsInputRequestTypeDef",
@@ -67,41 +68,56 @@
 CreateCliTokenRequestRequestTypeDef = TypedDict(
     "CreateCliTokenRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateCliTokenResponseTypeDef = TypedDict(
+    "CreateCliTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "CliToken": str,
+        "WebServerHostname": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
+CreateEnvironmentOutputTypeDef = TypedDict(
+    "CreateEnvironmentOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateWebLoginTokenRequestRequestTypeDef = TypedDict(
     "CreateWebLoginTokenRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+CreateWebLoginTokenResponseTypeDef = TypedDict(
+    "CreateWebLoginTokenResponseTypeDef",
+    {
+        "WebServerHostname": str,
+        "WebToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteEnvironmentInputRequestTypeDef = TypedDict(
     "DeleteEnvironmentInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -125,40 +141,55 @@
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListEnvironmentsInputRequestTypeDef = TypedDict(
     "ListEnvironmentsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListEnvironmentsOutputTypeDef = TypedDict(
+    "ListEnvironmentsOutputTypeDef",
+    {
+        "Environments": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
 ModuleLoggingConfigurationInputTypeDef = TypedDict(
     "ModuleLoggingConfigurationInputTypeDef",
     {
         "Enabled": bool,
         "LogLevel": LoggingLevelType,
     },
 )
@@ -180,14 +211,35 @@
         "Minimum": float,
         "SampleCount": int,
         "Sum": float,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -203,84 +255,33 @@
 UpdateNetworkConfigurationInputTypeDef = TypedDict(
     "UpdateNetworkConfigurationInputTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
 )
 
-CreateCliTokenResponseTypeDef = TypedDict(
-    "CreateCliTokenResponseTypeDef",
-    {
-        "CliToken": str,
-        "WebServerHostname": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEnvironmentOutputTypeDef = TypedDict(
-    "CreateEnvironmentOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWebLoginTokenResponseTypeDef = TypedDict(
-    "CreateWebLoginTokenResponseTypeDef",
-    {
-        "WebServerHostname": str,
-        "WebToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListEnvironmentsOutputTypeDef = TypedDict(
-    "ListEnvironmentsOutputTypeDef",
-    {
-        "Environments": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateEnvironmentOutputTypeDef = TypedDict(
     "UpdateEnvironmentOutputTypeDef",
     {
         "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LastUpdateTypeDef = TypedDict(
     "LastUpdateTypeDef",
     {
         "CreatedAt": datetime,
         "Error": UpdateErrorTypeDef,
         "Source": str,
         "Status": UpdateStatusType,
     },
     total=False,
 )
 
-ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 LoggingConfigurationInputTypeDef = TypedDict(
     "LoggingConfigurationInputTypeDef",
     {
         "DagProcessingLogs": ModuleLoggingConfigurationInputTypeDef,
         "SchedulerLogs": ModuleLoggingConfigurationInputTypeDef,
         "TaskLogs": ModuleLoggingConfigurationInputTypeDef,
         "WebserverLogs": ModuleLoggingConfigurationInputTypeDef,
@@ -315,17 +316,19 @@
         "StatisticValues": StatisticSetTypeDef,
         "Unit": UnitType,
         "Value": float,
     },
     total=False,
 )
 
+
 class MetricDatumTypeDef(_RequiredMetricDatumTypeDef, _OptionalMetricDatumTypeDef):
     pass
 
+
 _RequiredCreateEnvironmentInputRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentInputRequestTypeDef",
     {
         "DagS3Path": str,
         "ExecutionRoleArn": str,
         "Name": str,
         "NetworkConfiguration": NetworkConfigurationTypeDef,
@@ -343,26 +346,30 @@
         "MaxWorkers": int,
         "MinWorkers": int,
         "PluginsS3ObjectVersion": str,
         "PluginsS3Path": str,
         "RequirementsS3ObjectVersion": str,
         "RequirementsS3Path": str,
         "Schedulers": int,
+        "StartupScriptS3ObjectVersion": str,
+        "StartupScriptS3Path": str,
         "Tags": Mapping[str, str],
         "WebserverAccessMode": WebserverAccessModeType,
         "WeeklyMaintenanceWindowStart": str,
     },
     total=False,
 )
 
+
 class CreateEnvironmentInputRequestTypeDef(
     _RequiredCreateEnvironmentInputRequestTypeDef, _OptionalCreateEnvironmentInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateEnvironmentInputRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateEnvironmentInputRequestTypeDef = TypedDict(
@@ -379,25 +386,29 @@
         "NetworkConfiguration": UpdateNetworkConfigurationInputTypeDef,
         "PluginsS3ObjectVersion": str,
         "PluginsS3Path": str,
         "RequirementsS3ObjectVersion": str,
         "RequirementsS3Path": str,
         "Schedulers": int,
         "SourceBucketArn": str,
+        "StartupScriptS3ObjectVersion": str,
+        "StartupScriptS3Path": str,
         "WebserverAccessMode": WebserverAccessModeType,
         "WeeklyMaintenanceWindowStart": str,
     },
     total=False,
 )
 
+
 class UpdateEnvironmentInputRequestTypeDef(
     _RequiredUpdateEnvironmentInputRequestTypeDef, _OptionalUpdateEnvironmentInputRequestTypeDef
 ):
     pass
 
+
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "AirflowConfigurationOptions": Dict[str, str],
         "AirflowVersion": str,
         "Arn": str,
         "CreatedAt": datetime,
@@ -414,14 +425,16 @@
         "PluginsS3ObjectVersion": str,
         "PluginsS3Path": str,
         "RequirementsS3ObjectVersion": str,
         "RequirementsS3Path": str,
         "Schedulers": int,
         "ServiceRoleArn": str,
         "SourceBucketArn": str,
+        "StartupScriptS3ObjectVersion": str,
+        "StartupScriptS3Path": str,
         "Status": EnvironmentStatusType,
         "Tags": Dict[str, str],
         "WebserverAccessMode": WebserverAccessModeType,
         "WebserverUrl": str,
         "WeeklyMaintenanceWindowStart": str,
     },
     total=False,
@@ -435,10 +448,10 @@
     },
 )
 
 GetEnvironmentOutputTypeDef = TypedDict(
     "GetEnvironmentOutputTypeDef",
     {
         "Environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa.egg-info/PKG-INFO` & `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mwaa
-Version: 1.26.44
-Summary: Type annotations for boto3.MWAA 1.26.44 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.MWAA 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-mwaa"></a>
 
 # mypy-boto3-mwaa
 
 [![PyPI - mypy-boto3-mwaa](https://img.shields.io/pypi/v/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mwaa?color=blue)](https://pypistats.org/packages/mypy-boto3-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MWAA 1.26.44](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[boto3.MWAA 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mwaa docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,38 +324,38 @@
 
 `mypy_boto3_mwaa.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mwaa.type_defs import (
     CreateCliTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateCliTokenResponseTypeDef,
     NetworkConfigurationTypeDef,
+    CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenRequestRequestTypeDef,
+    CreateWebLoginTokenResponseTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DimensionTypeDef,
     GetEnvironmentInputRequestTypeDef,
     UpdateErrorTypeDef,
-    PaginatorConfigTypeDef,
+    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     ListEnvironmentsInputRequestTypeDef,
+    ListEnvironmentsOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ModuleLoggingConfigurationInputTypeDef,
     ModuleLoggingConfigurationTypeDef,
     StatisticSetTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
-    CreateCliTokenResponseTypeDef,
-    CreateEnvironmentOutputTypeDef,
-    CreateWebLoginTokenResponseTypeDef,
-    ListEnvironmentsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
     LastUpdateTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     LoggingConfigurationInputTypeDef,
     LoggingConfigurationTypeDef,
     MetricDatumTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
     EnvironmentTypeDef,
     PublishMetricsInputRequestTypeDef,
@@ -370,42 +370,42 @@
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

### Comparing `mypy-boto3-mwaa-1.26.44/mypy_boto3_mwaa.egg-info/SOURCES.txt` & `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.26.44/setup.py` & `mypy-boto3-mwaa-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-mwaa.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mwaa",
-    version="1.26.44",
+    version="1.27.0",
     packages=["mypy_boto3_mwaa"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MWAA 1.26.44 service generated with mypy-boto3-builder 7.12.2"
+        "Type annotations for boto3.MWAA 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -44,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/",
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


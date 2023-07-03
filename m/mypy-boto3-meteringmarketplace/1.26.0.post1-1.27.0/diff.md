# Comparing `tmp/mypy-boto3-meteringmarketplace-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-meteringmarketplace-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-meteringmarketplace-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:45 2022, max compression
+gzip compressed data, was "mypy-boto3-meteringmarketplace-1.27.0.tar", last modified: Mon Jul  3 19:51:08 2023, max compression
```

## Comparing `mypy-boto3-meteringmarketplace-1.26.0.post1.tar` & `mypy-boto3-meteringmarketplace-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:45.000836 mypy-boto3-meteringmarketplace-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:38:16.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12832 2022-11-01 21:43:45.000836 mypy-boto3-meteringmarketplace-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11343 2022-11-01 21:38:16.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:45.000836 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-11-01 21:38:16.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-11-01 21:38:16.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-11-01 21:38:16.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6918 2022-11-01 21:38:16.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     6908 2022-11-01 21:38:16.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7519 2022-11-01 21:38:16.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7517 2022-11-01 21:38:16.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:38:16.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4831 2022-11-01 21:38:16.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4822 2022-11-01 21:38:16.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:38:16.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:45.000836 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12832 2022-11-01 21:43:44.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-11-01 21:43:44.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:44.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:44.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:44.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-11-01 21:43:44.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:45.000836 mypy-boto3-meteringmarketplace-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2022-11-01 21:38:16.000000 mypy-boto3-meteringmarketplace-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.271681 mypy-boto3-meteringmarketplace-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:17.000000 mypy-boto3-meteringmarketplace-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-07-03 19:51:08.263681 mypy-boto3-meteringmarketplace-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-03 19:42:17.000000 mypy-boto3-meteringmarketplace-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.263681 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-03 19:42:17.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-03 19:42:17.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-03 19:42:17.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-03 19:42:17.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-03 19:42:17.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-03 19:42:17.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-03 19:42:17.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:17.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-03 19:42:17.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-03 19:42:17.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:17.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.263681 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-07-03 19:51:08.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-03 19:51:08.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:08.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:08.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:08.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 19:51:08.000000 mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:08.271681 mypy-boto3-meteringmarketplace-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-03 19:42:17.000000 mypy-boto3-meteringmarketplace-1.27.0/setup.py
```

### Comparing `mypy-boto3-meteringmarketplace-1.26.0.post1/LICENSE` & `mypy-boto3-meteringmarketplace-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-meteringmarketplace-1.26.0.post1/PKG-INFO` & `mypy-boto3-meteringmarketplace-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-meteringmarketplace
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.MarketplaceMetering 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.MarketplaceMetering 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/
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
 
 <a id="mypy-boto3-meteringmarketplace"></a>
 
 # mypy-boto3-meteringmarketplace
 
 [![PyPI - mypy-boto3-meteringmarketplace](https://img.shields.io/pypi/v/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-meteringmarketplace?color=blue)](https://pypistats.org/packages/mypy-boto3-meteringmarketplace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceMetering 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
+[boto3.MarketplaceMetering 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
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
 [mypy-boto3-meteringmarketplace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,69 +298,69 @@
 ### Typed dictionaries
 
 `mypy_boto3_meteringmarketplace.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_meteringmarketplace.type_defs import (
-    ResponseMetadataTypeDef,
-    RegisterUsageRequestRequestTypeDef,
-    ResolveCustomerRequestRequestTypeDef,
-    TagTypeDef,
     MeterUsageResultTypeDef,
+    RegisterUsageRequestRequestTypeDef,
     RegisterUsageResultTypeDef,
+    ResolveCustomerRequestRequestTypeDef,
     ResolveCustomerResultTypeDef,
+    ResponseMetadataTypeDef,
+    TagTypeDef,
     UsageAllocationTypeDef,
     MeterUsageRequestRequestTypeDef,
     UsageRecordTypeDef,
     BatchMeterUsageRequestRequestTypeDef,
     UsageRecordResultTypeDef,
     BatchMeterUsageResultTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> MeterUsageResultTypeDef:
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

### Comparing `mypy-boto3-meteringmarketplace-1.26.0.post1/README.md` & `mypy-boto3-meteringmarketplace-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-meteringmarketplace"></a>
 
 # mypy-boto3-meteringmarketplace
 
 [![PyPI - mypy-boto3-meteringmarketplace](https://img.shields.io/pypi/v/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-meteringmarketplace?color=blue)](https://pypistats.org/packages/mypy-boto3-meteringmarketplace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceMetering 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
+[boto3.MarketplaceMetering 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
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
 [mypy-boto3-meteringmarketplace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,69 +266,69 @@
 ### Typed dictionaries
 
 `mypy_boto3_meteringmarketplace.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_meteringmarketplace.type_defs import (
-    ResponseMetadataTypeDef,
-    RegisterUsageRequestRequestTypeDef,
-    ResolveCustomerRequestRequestTypeDef,
-    TagTypeDef,
     MeterUsageResultTypeDef,
+    RegisterUsageRequestRequestTypeDef,
     RegisterUsageResultTypeDef,
+    ResolveCustomerRequestRequestTypeDef,
     ResolveCustomerResultTypeDef,
+    ResponseMetadataTypeDef,
+    TagTypeDef,
     UsageAllocationTypeDef,
     MeterUsageRequestRequestTypeDef,
     UsageRecordTypeDef,
     BatchMeterUsageRequestRequestTypeDef,
     UsageRecordResultTypeDef,
     BatchMeterUsageResultTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> MeterUsageResultTypeDef:
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

### Comparing `mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/__main__.py` & `mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MarketplaceMetering 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.MarketplaceMetering 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering\nOther"
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

### Comparing `mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/client.py` & `mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/client.pyi` & `mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/literals.py` & `mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/literals.py`

 * *Files 6% similar despite different names*

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
@@ -365,21 +397,25 @@
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
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/literals.pyi` & `mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -39,23 +39,25 @@
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
@@ -65,30 +67,35 @@
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
@@ -114,14 +121,15 @@
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
@@ -166,51 +174,57 @@
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
@@ -223,14 +237,15 @@
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
@@ -242,28 +257,35 @@
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
@@ -272,14 +294,15 @@
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
@@ -290,55 +313,64 @@
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
@@ -363,21 +395,25 @@
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
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/type_defs.py` & `mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for meteringmarketplace service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_meteringmarketplace.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_meteringmarketplace.type_defs import MeterUsageResultTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: MeterUsageResultTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import UsageRecordResultStatusType
@@ -20,37 +20,34 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ResponseMetadataTypeDef",
-    "RegisterUsageRequestRequestTypeDef",
-    "ResolveCustomerRequestRequestTypeDef",
-    "TagTypeDef",
     "MeterUsageResultTypeDef",
+    "RegisterUsageRequestRequestTypeDef",
     "RegisterUsageResultTypeDef",
+    "ResolveCustomerRequestRequestTypeDef",
     "ResolveCustomerResultTypeDef",
+    "ResponseMetadataTypeDef",
+    "TagTypeDef",
     "UsageAllocationTypeDef",
     "MeterUsageRequestRequestTypeDef",
     "UsageRecordTypeDef",
     "BatchMeterUsageRequestRequestTypeDef",
     "UsageRecordResultTypeDef",
     "BatchMeterUsageResultTypeDef",
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+MeterUsageResultTypeDef = TypedDict(
+    "MeterUsageResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "MeteringRecordId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRegisterUsageRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterUsageRequestRequestTypeDef",
     {
         "ProductCode": str,
@@ -68,53 +65,56 @@
 
 class RegisterUsageRequestRequestTypeDef(
     _RequiredRegisterUsageRequestRequestTypeDef, _OptionalRegisterUsageRequestRequestTypeDef
 ):
     pass
 
 
-ResolveCustomerRequestRequestTypeDef = TypedDict(
-    "ResolveCustomerRequestRequestTypeDef",
+RegisterUsageResultTypeDef = TypedDict(
+    "RegisterUsageResultTypeDef",
     {
-        "RegistrationToken": str,
+        "PublicKeyRotationTimestamp": datetime,
+        "Signature": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+ResolveCustomerRequestRequestTypeDef = TypedDict(
+    "ResolveCustomerRequestRequestTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "RegistrationToken": str,
     },
 )
 
-MeterUsageResultTypeDef = TypedDict(
-    "MeterUsageResultTypeDef",
+ResolveCustomerResultTypeDef = TypedDict(
+    "ResolveCustomerResultTypeDef",
     {
-        "MeteringRecordId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CustomerIdentifier": str,
+        "ProductCode": str,
+        "CustomerAWSAccountId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RegisterUsageResultTypeDef = TypedDict(
-    "RegisterUsageResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "PublicKeyRotationTimestamp": datetime,
-        "Signature": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-ResolveCustomerResultTypeDef = TypedDict(
-    "ResolveCustomerResultTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "CustomerIdentifier": str,
-        "ProductCode": str,
-        "CustomerAWSAccountId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Key": str,
+        "Value": str,
     },
 )
 
 _RequiredUsageAllocationTypeDef = TypedDict(
     "_RequiredUsageAllocationTypeDef",
     {
         "AllocatedUsageQuantity": int,
@@ -199,10 +199,10 @@
 )
 
 BatchMeterUsageResultTypeDef = TypedDict(
     "BatchMeterUsageResultTypeDef",
     {
         "Results": List[UsageRecordResultTypeDef],
         "UnprocessedRecords": List[UsageRecordTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace/type_defs.pyi` & `mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,54 +2,51 @@
 Type annotations for meteringmarketplace service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_meteringmarketplace.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_meteringmarketplace.type_defs import MeterUsageResultTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: MeterUsageResultTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import UsageRecordResultStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ResponseMetadataTypeDef",
-    "RegisterUsageRequestRequestTypeDef",
-    "ResolveCustomerRequestRequestTypeDef",
-    "TagTypeDef",
     "MeterUsageResultTypeDef",
+    "RegisterUsageRequestRequestTypeDef",
     "RegisterUsageResultTypeDef",
+    "ResolveCustomerRequestRequestTypeDef",
     "ResolveCustomerResultTypeDef",
+    "ResponseMetadataTypeDef",
+    "TagTypeDef",
     "UsageAllocationTypeDef",
     "MeterUsageRequestRequestTypeDef",
     "UsageRecordTypeDef",
     "BatchMeterUsageRequestRequestTypeDef",
     "UsageRecordResultTypeDef",
     "BatchMeterUsageResultTypeDef",
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+MeterUsageResultTypeDef = TypedDict(
+    "MeterUsageResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "MeteringRecordId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRegisterUsageRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterUsageRequestRequestTypeDef",
     {
         "ProductCode": str,
@@ -65,53 +62,56 @@
 )
 
 class RegisterUsageRequestRequestTypeDef(
     _RequiredRegisterUsageRequestRequestTypeDef, _OptionalRegisterUsageRequestRequestTypeDef
 ):
     pass
 
-ResolveCustomerRequestRequestTypeDef = TypedDict(
-    "ResolveCustomerRequestRequestTypeDef",
+RegisterUsageResultTypeDef = TypedDict(
+    "RegisterUsageResultTypeDef",
     {
-        "RegistrationToken": str,
+        "PublicKeyRotationTimestamp": datetime,
+        "Signature": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+ResolveCustomerRequestRequestTypeDef = TypedDict(
+    "ResolveCustomerRequestRequestTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "RegistrationToken": str,
     },
 )
 
-MeterUsageResultTypeDef = TypedDict(
-    "MeterUsageResultTypeDef",
+ResolveCustomerResultTypeDef = TypedDict(
+    "ResolveCustomerResultTypeDef",
     {
-        "MeteringRecordId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CustomerIdentifier": str,
+        "ProductCode": str,
+        "CustomerAWSAccountId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RegisterUsageResultTypeDef = TypedDict(
-    "RegisterUsageResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "PublicKeyRotationTimestamp": datetime,
-        "Signature": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-ResolveCustomerResultTypeDef = TypedDict(
-    "ResolveCustomerResultTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "CustomerIdentifier": str,
-        "ProductCode": str,
-        "CustomerAWSAccountId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Key": str,
+        "Value": str,
     },
 )
 
 _RequiredUsageAllocationTypeDef = TypedDict(
     "_RequiredUsageAllocationTypeDef",
     {
         "AllocatedUsageQuantity": int,
@@ -190,10 +190,10 @@
 )
 
 BatchMeterUsageResultTypeDef = TypedDict(
     "BatchMeterUsageResultTypeDef",
     {
         "Results": List[UsageRecordResultTypeDef],
         "UnprocessedRecords": List[UsageRecordTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO` & `mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-meteringmarketplace
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.MarketplaceMetering 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.MarketplaceMetering 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/
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
 
 <a id="mypy-boto3-meteringmarketplace"></a>
 
 # mypy-boto3-meteringmarketplace
 
 [![PyPI - mypy-boto3-meteringmarketplace](https://img.shields.io/pypi/v/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-meteringmarketplace?color=blue)](https://pypistats.org/packages/mypy-boto3-meteringmarketplace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceMetering 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
+[boto3.MarketplaceMetering 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
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
 [mypy-boto3-meteringmarketplace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,69 +298,69 @@
 ### Typed dictionaries
 
 `mypy_boto3_meteringmarketplace.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_meteringmarketplace.type_defs import (
-    ResponseMetadataTypeDef,
-    RegisterUsageRequestRequestTypeDef,
-    ResolveCustomerRequestRequestTypeDef,
-    TagTypeDef,
     MeterUsageResultTypeDef,
+    RegisterUsageRequestRequestTypeDef,
     RegisterUsageResultTypeDef,
+    ResolveCustomerRequestRequestTypeDef,
     ResolveCustomerResultTypeDef,
+    ResponseMetadataTypeDef,
+    TagTypeDef,
     UsageAllocationTypeDef,
     MeterUsageRequestRequestTypeDef,
     UsageRecordTypeDef,
     BatchMeterUsageRequestRequestTypeDef,
     UsageRecordResultTypeDef,
     BatchMeterUsageResultTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> MeterUsageResultTypeDef:
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

### Comparing `mypy-boto3-meteringmarketplace-1.26.0.post1/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt` & `mypy-boto3-meteringmarketplace-1.27.0/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.26.0.post1/setup.py` & `mypy-boto3-meteringmarketplace-1.27.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 """
 Setup script for mypy-boto3-meteringmarketplace.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-meteringmarketplace",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_meteringmarketplace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MarketplaceMetering 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.MarketplaceMetering 1.27.0 service generated with"
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
     keywords="boto3 meteringmarketplace type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_meteringmarketplace": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_meteringmarketplace": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/"
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


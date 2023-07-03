# Comparing `tmp/mypy-boto3-pi-1.26.83.tar.gz` & `tmp/mypy-boto3-pi-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pi-1.26.83.tar", last modified: Thu Mar  2 20:28:28 2023, max compression
+gzip compressed data, was "mypy-boto3-pi-1.27.0.tar", last modified: Mon Jul  3 19:51:15 2023, max compression
```

## Comparing `mypy-boto3-pi-1.26.83.tar` & `mypy-boto3-pi-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:28:28.003821 mypy-boto3-pi-1.26.83/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-02 20:27:43.000000 mypy-boto3-pi-1.26.83/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-03-02 20:28:28.003821 mypy-boto3-pi-1.26.83/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-03-02 20:27:43.000000 mypy-boto3-pi-1.26.83/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:28:27.995821 mypy-boto3-pi-1.26.83/mypy_boto3_pi/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-02 20:27:43.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-02 20:27:43.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-02 20:27:43.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-03-02 20:27:43.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-03-02 20:27:43.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-03-02 20:27:43.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-03-02 20:27:43.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 20:27:43.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-03-02 20:27:44.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-03-02 20:27:43.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-02 20:27:43.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:28:27.995821 mypy-boto3-pi-1.26.83/mypy_boto3_pi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-03-02 20:28:27.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-02 20:28:27.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 20:28:27.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 20:28:27.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-02 20:28:27.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-02 20:28:27.000000 mypy-boto3-pi-1.26.83/mypy_boto3_pi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 20:28:28.003821 mypy-boto3-pi-1.26.83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-03-02 20:27:43.000000 mypy-boto3-pi-1.26.83/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:15.027800 mypy-boto3-pi-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:27.000000 mypy-boto3-pi-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-07-03 19:51:15.027800 mypy-boto3-pi-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-07-03 19:43:27.000000 mypy-boto3-pi-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:15.007800 mypy-boto3-pi-1.27.0/mypy_boto3_pi/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-03 19:43:27.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-03 19:43:27.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-03 19:43:27.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-07-03 19:43:27.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-03 19:43:27.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-07-03 19:43:27.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-07-03 19:43:27.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:27.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-07-03 19:43:27.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-07-03 19:43:27.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:27.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:15.027800 mypy-boto3-pi-1.27.0/mypy_boto3_pi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-07-03 19:51:14.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-03 19:51:14.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:14.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:14.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:14.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 19:51:14.000000 mypy-boto3-pi-1.27.0/mypy_boto3_pi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:15.027800 mypy-boto3-pi-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-03 19:43:26.000000 mypy-boto3-pi-1.27.0/setup.py
```

### Comparing `mypy-boto3-pi-1.26.83/LICENSE` & `mypy-boto3-pi-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-pi-1.26.83/PKG-INFO` & `mypy-boto3-pi-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pi
-Version: 1.26.83
-Summary: Type annotations for boto3.PI 1.26.83 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.PI 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-pi"></a>
 
 # mypy-boto3-pi
 
 [![PyPI - mypy-boto3-pi](https://img.shields.io/pypi/v/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pi?color=blue)](https://pypistats.org/packages/mypy-boto3-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PI 1.26.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[boto3.PI 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,25 +302,25 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pi.type_defs import (
     DataPointTypeDef,
     DimensionGroupTypeDef,
     DimensionKeyDescriptionTypeDef,
-    ResponseMetadataTypeDef,
     ResponsePartitionKeyTypeDef,
     DimensionDetailTypeDef,
     DimensionKeyDetailTypeDef,
     FeatureMetadataTypeDef,
     GetDimensionKeyDetailsRequestRequestTypeDef,
     GetResourceMetadataRequestRequestTypeDef,
     ListAvailableResourceDimensionsRequestRequestTypeDef,
     ListAvailableResourceMetricsRequestRequestTypeDef,
     ResponseResourceMetricTypeDef,
     ResponseResourceMetricKeyTypeDef,
+    ResponseMetadataTypeDef,
     DescribeDimensionKeysRequestRequestTypeDef,
     MetricQueryTypeDef,
     DescribeDimensionKeysResponseTypeDef,
     DimensionGroupDetailTypeDef,
     GetDimensionKeyDetailsResponseTypeDef,
     GetResourceMetadataResponseTypeDef,
     ListAvailableResourceMetricsResponseTypeDef,
@@ -339,42 +339,42 @@
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

### Comparing `mypy-boto3-pi-1.26.83/README.md` & `mypy-boto3-pi-1.27.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-pi"></a>
 
 # mypy-boto3-pi
 
 [![PyPI - mypy-boto3-pi](https://img.shields.io/pypi/v/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pi?color=blue)](https://pypistats.org/packages/mypy-boto3-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PI 1.26.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[boto3.PI 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -270,25 +270,25 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pi.type_defs import (
     DataPointTypeDef,
     DimensionGroupTypeDef,
     DimensionKeyDescriptionTypeDef,
-    ResponseMetadataTypeDef,
     ResponsePartitionKeyTypeDef,
     DimensionDetailTypeDef,
     DimensionKeyDetailTypeDef,
     FeatureMetadataTypeDef,
     GetDimensionKeyDetailsRequestRequestTypeDef,
     GetResourceMetadataRequestRequestTypeDef,
     ListAvailableResourceDimensionsRequestRequestTypeDef,
     ListAvailableResourceMetricsRequestRequestTypeDef,
     ResponseResourceMetricTypeDef,
     ResponseResourceMetricKeyTypeDef,
+    ResponseMetadataTypeDef,
     DescribeDimensionKeysRequestRequestTypeDef,
     MetricQueryTypeDef,
     DescribeDimensionKeysResponseTypeDef,
     DimensionGroupDetailTypeDef,
     GetDimensionKeyDetailsResponseTypeDef,
     GetResourceMetadataResponseTypeDef,
     ListAvailableResourceMetricsResponseTypeDef,
@@ -307,42 +307,42 @@
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

### Comparing `mypy-boto3-pi-1.26.83/mypy_boto3_pi/__main__.py` & `mypy-boto3-pi-1.27.0/mypy_boto3_pi/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PI 1.26.83\nVersion:         1.26.83\nBuilder version:"
-        " 7.12.5\nDocs:           "
+        "Type annotations for boto3.PI 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.83")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-pi-1.26.83/mypy_boto3_pi/client.py` & `mypy-boto3-pi-1.27.0/mypy_boto3_pi/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pi-1.26.83/mypy_boto3_pi/client.pyi` & `mypy-boto3-pi-1.27.0/mypy_boto3_pi/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pi-1.26.83/mypy_boto3_pi/literals.py` & `mypy-boto3-pi-1.27.0/mypy_boto3_pi/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
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
@@ -101,14 +102,15 @@
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
@@ -206,14 +208,15 @@
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
@@ -249,14 +252,15 @@
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
@@ -275,16 +279,19 @@
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
@@ -368,15 +375,17 @@
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

### Comparing `mypy-boto3-pi-1.26.83/mypy_boto3_pi/literals.pyi` & `mypy-boto3-pi-1.27.0/mypy_boto3_pi/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
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
@@ -99,14 +100,15 @@
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
@@ -204,14 +206,15 @@
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
@@ -247,14 +250,15 @@
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
@@ -273,16 +277,19 @@
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
@@ -366,15 +373,17 @@
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

### Comparing `mypy-boto3-pi-1.26.83/mypy_boto3_pi/type_defs.py` & `mypy-boto3-pi-1.27.0/mypy_boto3_pi/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -18,30 +18,29 @@
 from .literals import DetailStatusType, FeatureStatusType, PeriodAlignmentType, ServiceTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "DataPointTypeDef",
     "DimensionGroupTypeDef",
     "DimensionKeyDescriptionTypeDef",
-    "ResponseMetadataTypeDef",
     "ResponsePartitionKeyTypeDef",
     "DimensionDetailTypeDef",
     "DimensionKeyDetailTypeDef",
     "FeatureMetadataTypeDef",
     "GetDimensionKeyDetailsRequestRequestTypeDef",
     "GetResourceMetadataRequestRequestTypeDef",
     "ListAvailableResourceDimensionsRequestRequestTypeDef",
     "ListAvailableResourceMetricsRequestRequestTypeDef",
     "ResponseResourceMetricTypeDef",
     "ResponseResourceMetricKeyTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeDimensionKeysRequestRequestTypeDef",
     "MetricQueryTypeDef",
     "DescribeDimensionKeysResponseTypeDef",
     "DimensionGroupDetailTypeDef",
     "GetDimensionKeyDetailsResponseTypeDef",
     "GetResourceMetadataResponseTypeDef",
     "ListAvailableResourceMetricsResponseTypeDef",
@@ -71,41 +70,28 @@
     {
         "Dimensions": Sequence[str],
         "Limit": int,
     },
     total=False,
 )
 
-
 class DimensionGroupTypeDef(_RequiredDimensionGroupTypeDef, _OptionalDimensionGroupTypeDef):
     pass
 
-
 DimensionKeyDescriptionTypeDef = TypedDict(
     "DimensionKeyDescriptionTypeDef",
     {
         "Dimensions": Dict[str, str],
         "Total": float,
         "AdditionalMetrics": Dict[str, float],
         "Partitions": List[float],
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
 ResponsePartitionKeyTypeDef = TypedDict(
     "ResponsePartitionKeyTypeDef",
     {
         "Dimensions": Dict[str, str],
     },
 )
 
@@ -148,22 +134,20 @@
     "_OptionalGetDimensionKeyDetailsRequestRequestTypeDef",
     {
         "RequestedDimensions": Sequence[str],
     },
     total=False,
 )
 
-
 class GetDimensionKeyDetailsRequestRequestTypeDef(
     _RequiredGetDimensionKeyDetailsRequestRequestTypeDef,
     _OptionalGetDimensionKeyDetailsRequestRequestTypeDef,
 ):
     pass
 
-
 GetResourceMetadataRequestRequestTypeDef = TypedDict(
     "GetResourceMetadataRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
     },
 )
@@ -181,22 +165,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAvailableResourceDimensionsRequestRequestTypeDef(
     _RequiredListAvailableResourceDimensionsRequestRequestTypeDef,
     _OptionalListAvailableResourceDimensionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAvailableResourceMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableResourceMetricsRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
         "MetricTypes": Sequence[str],
     },
@@ -206,22 +188,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListAvailableResourceMetricsRequestRequestTypeDef(
     _RequiredListAvailableResourceMetricsRequestRequestTypeDef,
     _OptionalListAvailableResourceMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 ResponseResourceMetricTypeDef = TypedDict(
     "ResponseResourceMetricTypeDef",
     {
         "Metric": str,
         "Description": str,
         "Unit": str,
     },
@@ -238,20 +218,29 @@
     "_OptionalResponseResourceMetricKeyTypeDef",
     {
         "Dimensions": Dict[str, str],
     },
     total=False,
 )
 
-
 class ResponseResourceMetricKeyTypeDef(
     _RequiredResponseResourceMetricKeyTypeDef, _OptionalResponseResourceMetricKeyTypeDef
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
 
 _RequiredDescribeDimensionKeysRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDimensionKeysRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
         "StartTime": Union[datetime, str],
@@ -269,22 +258,20 @@
         "Filter": Mapping[str, str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeDimensionKeysRequestRequestTypeDef(
     _RequiredDescribeDimensionKeysRequestRequestTypeDef,
     _OptionalDescribeDimensionKeysRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredMetricQueryTypeDef = TypedDict(
     "_RequiredMetricQueryTypeDef",
     {
         "Metric": str,
     },
 )
 _OptionalMetricQueryTypeDef = TypedDict(
@@ -292,28 +279,26 @@
     {
         "GroupBy": DimensionGroupTypeDef,
         "Filter": Mapping[str, str],
     },
     total=False,
 )
 
-
 class MetricQueryTypeDef(_RequiredMetricQueryTypeDef, _OptionalMetricQueryTypeDef):
     pass
 
-
 DescribeDimensionKeysResponseTypeDef = TypedDict(
     "DescribeDimensionKeysResponseTypeDef",
     {
         "AlignedStartTime": datetime,
         "AlignedEndTime": datetime,
         "PartitionKeys": List[ResponsePartitionKeyTypeDef],
         "Keys": List[DimensionKeyDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DimensionGroupDetailTypeDef = TypedDict(
     "DimensionGroupDetailTypeDef",
     {
         "Group": str,
@@ -322,33 +307,33 @@
     total=False,
 )
 
 GetDimensionKeyDetailsResponseTypeDef = TypedDict(
     "GetDimensionKeyDetailsResponseTypeDef",
     {
         "Dimensions": List[DimensionKeyDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceMetadataResponseTypeDef = TypedDict(
     "GetResourceMetadataResponseTypeDef",
     {
         "Identifier": str,
         "Features": Dict[str, FeatureMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAvailableResourceMetricsResponseTypeDef = TypedDict(
     "ListAvailableResourceMetricsResponseTypeDef",
     {
         "Metrics": List[ResponseResourceMetricTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricKeyDataPointsTypeDef = TypedDict(
     "MetricKeyDataPointsTypeDef",
     {
         "Key": ResponseResourceMetricKeyTypeDef,
@@ -374,22 +359,20 @@
         "MaxResults": int,
         "NextToken": str,
         "PeriodAlignment": PeriodAlignmentType,
     },
     total=False,
 )
 
-
 class GetResourceMetricsRequestRequestTypeDef(
     _RequiredGetResourceMetricsRequestRequestTypeDef,
     _OptionalGetResourceMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 MetricDimensionGroupsTypeDef = TypedDict(
     "MetricDimensionGroupsTypeDef",
     {
         "Metric": str,
         "Groups": List[DimensionGroupDetailTypeDef],
     },
     total=False,
@@ -399,19 +382,19 @@
     "GetResourceMetricsResponseTypeDef",
     {
         "AlignedStartTime": datetime,
         "AlignedEndTime": datetime,
         "Identifier": str,
         "MetricList": List[MetricKeyDataPointsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAvailableResourceDimensionsResponseTypeDef = TypedDict(
     "ListAvailableResourceDimensionsResponseTypeDef",
     {
         "MetricDimensions": List[MetricDimensionGroupsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-pi-1.26.83/mypy_boto3_pi/type_defs.pyi` & `mypy-boto3-pi-1.27.0/mypy_boto3_pi/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,29 +18,30 @@
 from .literals import DetailStatusType, FeatureStatusType, PeriodAlignmentType, ServiceTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "DataPointTypeDef",
     "DimensionGroupTypeDef",
     "DimensionKeyDescriptionTypeDef",
-    "ResponseMetadataTypeDef",
     "ResponsePartitionKeyTypeDef",
     "DimensionDetailTypeDef",
     "DimensionKeyDetailTypeDef",
     "FeatureMetadataTypeDef",
     "GetDimensionKeyDetailsRequestRequestTypeDef",
     "GetResourceMetadataRequestRequestTypeDef",
     "ListAvailableResourceDimensionsRequestRequestTypeDef",
     "ListAvailableResourceMetricsRequestRequestTypeDef",
     "ResponseResourceMetricTypeDef",
     "ResponseResourceMetricKeyTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeDimensionKeysRequestRequestTypeDef",
     "MetricQueryTypeDef",
     "DescribeDimensionKeysResponseTypeDef",
     "DimensionGroupDetailTypeDef",
     "GetDimensionKeyDetailsResponseTypeDef",
     "GetResourceMetadataResponseTypeDef",
     "ListAvailableResourceMetricsResponseTypeDef",
@@ -70,39 +71,30 @@
     {
         "Dimensions": Sequence[str],
         "Limit": int,
     },
     total=False,
 )
 
+
 class DimensionGroupTypeDef(_RequiredDimensionGroupTypeDef, _OptionalDimensionGroupTypeDef):
     pass
 
+
 DimensionKeyDescriptionTypeDef = TypedDict(
     "DimensionKeyDescriptionTypeDef",
     {
         "Dimensions": Dict[str, str],
         "Total": float,
         "AdditionalMetrics": Dict[str, float],
         "Partitions": List[float],
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
 ResponsePartitionKeyTypeDef = TypedDict(
     "ResponsePartitionKeyTypeDef",
     {
         "Dimensions": Dict[str, str],
     },
 )
 
@@ -145,20 +137,22 @@
     "_OptionalGetDimensionKeyDetailsRequestRequestTypeDef",
     {
         "RequestedDimensions": Sequence[str],
     },
     total=False,
 )
 
+
 class GetDimensionKeyDetailsRequestRequestTypeDef(
     _RequiredGetDimensionKeyDetailsRequestRequestTypeDef,
     _OptionalGetDimensionKeyDetailsRequestRequestTypeDef,
 ):
     pass
 
+
 GetResourceMetadataRequestRequestTypeDef = TypedDict(
     "GetResourceMetadataRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
     },
 )
@@ -176,20 +170,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAvailableResourceDimensionsRequestRequestTypeDef(
     _RequiredListAvailableResourceDimensionsRequestRequestTypeDef,
     _OptionalListAvailableResourceDimensionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAvailableResourceMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableResourceMetricsRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
         "MetricTypes": Sequence[str],
     },
@@ -199,20 +195,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListAvailableResourceMetricsRequestRequestTypeDef(
     _RequiredListAvailableResourceMetricsRequestRequestTypeDef,
     _OptionalListAvailableResourceMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 ResponseResourceMetricTypeDef = TypedDict(
     "ResponseResourceMetricTypeDef",
     {
         "Metric": str,
         "Description": str,
         "Unit": str,
     },
@@ -229,19 +227,32 @@
     "_OptionalResponseResourceMetricKeyTypeDef",
     {
         "Dimensions": Dict[str, str],
     },
     total=False,
 )
 
+
 class ResponseResourceMetricKeyTypeDef(
     _RequiredResponseResourceMetricKeyTypeDef, _OptionalResponseResourceMetricKeyTypeDef
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
 _RequiredDescribeDimensionKeysRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDimensionKeysRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -258,20 +269,22 @@
         "Filter": Mapping[str, str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeDimensionKeysRequestRequestTypeDef(
     _RequiredDescribeDimensionKeysRequestRequestTypeDef,
     _OptionalDescribeDimensionKeysRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredMetricQueryTypeDef = TypedDict(
     "_RequiredMetricQueryTypeDef",
     {
         "Metric": str,
     },
 )
 _OptionalMetricQueryTypeDef = TypedDict(
@@ -279,26 +292,28 @@
     {
         "GroupBy": DimensionGroupTypeDef,
         "Filter": Mapping[str, str],
     },
     total=False,
 )
 
+
 class MetricQueryTypeDef(_RequiredMetricQueryTypeDef, _OptionalMetricQueryTypeDef):
     pass
 
+
 DescribeDimensionKeysResponseTypeDef = TypedDict(
     "DescribeDimensionKeysResponseTypeDef",
     {
         "AlignedStartTime": datetime,
         "AlignedEndTime": datetime,
         "PartitionKeys": List[ResponsePartitionKeyTypeDef],
         "Keys": List[DimensionKeyDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DimensionGroupDetailTypeDef = TypedDict(
     "DimensionGroupDetailTypeDef",
     {
         "Group": str,
@@ -307,33 +322,33 @@
     total=False,
 )
 
 GetDimensionKeyDetailsResponseTypeDef = TypedDict(
     "GetDimensionKeyDetailsResponseTypeDef",
     {
         "Dimensions": List[DimensionKeyDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResourceMetadataResponseTypeDef = TypedDict(
     "GetResourceMetadataResponseTypeDef",
     {
         "Identifier": str,
         "Features": Dict[str, FeatureMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAvailableResourceMetricsResponseTypeDef = TypedDict(
     "ListAvailableResourceMetricsResponseTypeDef",
     {
         "Metrics": List[ResponseResourceMetricTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricKeyDataPointsTypeDef = TypedDict(
     "MetricKeyDataPointsTypeDef",
     {
         "Key": ResponseResourceMetricKeyTypeDef,
@@ -359,20 +374,22 @@
         "MaxResults": int,
         "NextToken": str,
         "PeriodAlignment": PeriodAlignmentType,
     },
     total=False,
 )
 
+
 class GetResourceMetricsRequestRequestTypeDef(
     _RequiredGetResourceMetricsRequestRequestTypeDef,
     _OptionalGetResourceMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 MetricDimensionGroupsTypeDef = TypedDict(
     "MetricDimensionGroupsTypeDef",
     {
         "Metric": str,
         "Groups": List[DimensionGroupDetailTypeDef],
     },
     total=False,
@@ -382,19 +399,19 @@
     "GetResourceMetricsResponseTypeDef",
     {
         "AlignedStartTime": datetime,
         "AlignedEndTime": datetime,
         "Identifier": str,
         "MetricList": List[MetricKeyDataPointsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAvailableResourceDimensionsResponseTypeDef = TypedDict(
     "ListAvailableResourceDimensionsResponseTypeDef",
     {
         "MetricDimensions": List[MetricDimensionGroupsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-pi-1.26.83/mypy_boto3_pi.egg-info/PKG-INFO` & `mypy-boto3-pi-1.27.0/mypy_boto3_pi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pi
-Version: 1.26.83
-Summary: Type annotations for boto3.PI 1.26.83 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.PI 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-pi"></a>
 
 # mypy-boto3-pi
 
 [![PyPI - mypy-boto3-pi](https://img.shields.io/pypi/v/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pi?color=blue)](https://pypistats.org/packages/mypy-boto3-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PI 1.26.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[boto3.PI 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,25 +302,25 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pi.type_defs import (
     DataPointTypeDef,
     DimensionGroupTypeDef,
     DimensionKeyDescriptionTypeDef,
-    ResponseMetadataTypeDef,
     ResponsePartitionKeyTypeDef,
     DimensionDetailTypeDef,
     DimensionKeyDetailTypeDef,
     FeatureMetadataTypeDef,
     GetDimensionKeyDetailsRequestRequestTypeDef,
     GetResourceMetadataRequestRequestTypeDef,
     ListAvailableResourceDimensionsRequestRequestTypeDef,
     ListAvailableResourceMetricsRequestRequestTypeDef,
     ResponseResourceMetricTypeDef,
     ResponseResourceMetricKeyTypeDef,
+    ResponseMetadataTypeDef,
     DescribeDimensionKeysRequestRequestTypeDef,
     MetricQueryTypeDef,
     DescribeDimensionKeysResponseTypeDef,
     DimensionGroupDetailTypeDef,
     GetDimensionKeyDetailsResponseTypeDef,
     GetResourceMetadataResponseTypeDef,
     ListAvailableResourceMetricsResponseTypeDef,
@@ -339,42 +339,42 @@
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

### Comparing `mypy-boto3-pi-1.26.83/mypy_boto3_pi.egg-info/SOURCES.txt` & `mypy-boto3-pi-1.27.0/mypy_boto3_pi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pi-1.26.83/setup.py` & `mypy-boto3-pi-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-pi.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pi",
-    version="1.26.83",
+    version="1.27.0",
     packages=["mypy_boto3_pi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PI 1.26.83 service generated with mypy-boto3-builder 7.12.5"
+        "Type annotations for boto3.PI 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/",
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


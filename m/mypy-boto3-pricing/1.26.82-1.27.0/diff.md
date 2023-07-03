# Comparing `tmp/mypy-boto3-pricing-1.26.82.tar.gz` & `tmp/mypy-boto3-pricing-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pricing-1.26.82.tar", last modified: Wed Mar  1 20:27:29 2023, max compression
+gzip compressed data, was "mypy-boto3-pricing-1.27.0.tar", last modified: Mon Jul  3 19:51:16 2023, max compression
```

## Comparing `mypy-boto3-pricing-1.26.82.tar` & `mypy-boto3-pricing-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:29.574109 mypy-boto3-pricing-1.26.82/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-03-01 20:27:29.570109 mypy-boto3-pricing-1.26.82/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:29.570109 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:29.570109 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-03-01 20:27:29.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-01 20:27:29.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 20:27:29.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 20:27:29.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-01 20:27:29.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-01 20:27:29.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 20:27:29.574109 mypy-boto3-pricing-1.26.82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-01 20:27:18.000000 mypy-boto3-pricing-1.26.82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:16.651826 mypy-boto3-pricing-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-07-03 19:51:16.651826 mypy-boto3-pricing-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:16.643826 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:16.651826 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-07-03 19:51:16.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-03 19:51:16.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:16.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:16.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:16.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:51:16.000000 mypy-boto3-pricing-1.27.0/mypy_boto3_pricing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:16.651826 mypy-boto3-pricing-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:43:46.000000 mypy-boto3-pricing-1.27.0/setup.py
```

### Comparing `mypy-boto3-pricing-1.26.82/LICENSE` & `mypy-boto3-pricing-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-pricing-1.26.82/PKG-INFO` & `mypy-boto3-pricing-1.27.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pricing
-Version: 1.26.82
-Summary: Type annotations for boto3.Pricing 1.26.82 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.Pricing 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-pricing"></a>
 
 # mypy-boto3-pricing
 
 [![PyPI - mypy-boto3-pricing](https://img.shields.io/pypi/v/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pricing?color=blue)](https://pypistats.org/packages/mypy-boto3-pricing)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pricing 1.26.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
+[boto3.Pricing 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
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
 [mypy-boto3-pricing docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,29 +333,29 @@
 
 `mypy_boto3_pricing.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pricing.type_defs import (
     AttributeValueTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeServicesRequestDescribeServicesPaginateTypeDef,
     DescribeServicesRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ServiceTypeDef,
     FilterTypeDef,
+    GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
     GetAttributeValuesRequestRequestTypeDef,
     GetPriceListFileUrlRequestRequestTypeDef,
+    GetPriceListFileUrlResponseTypeDef,
+    GetProductsResponseTypeDef,
+    ListPriceListsRequestListPriceListsPaginateTypeDef,
     ListPriceListsRequestRequestTypeDef,
     PriceListTypeDef,
-    DescribeServicesRequestDescribeServicesPaginateTypeDef,
-    GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
-    ListPriceListsRequestListPriceListsPaginateTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     GetAttributeValuesResponseTypeDef,
-    GetPriceListFileUrlResponseTypeDef,
-    GetProductsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     GetProductsRequestGetProductsPaginateTypeDef,
     GetProductsRequestRequestTypeDef,
     ListPriceListsResponseTypeDef,
 )
 
 
@@ -366,42 +366,42 @@
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

### Comparing `mypy-boto3-pricing-1.26.82/README.md` & `mypy-boto3-pricing-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-pricing"></a>
 
 # mypy-boto3-pricing
 
 [![PyPI - mypy-boto3-pricing](https://img.shields.io/pypi/v/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pricing?color=blue)](https://pypistats.org/packages/mypy-boto3-pricing)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pricing 1.26.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
+[boto3.Pricing 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
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
 [mypy-boto3-pricing docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,29 +301,29 @@
 
 `mypy_boto3_pricing.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pricing.type_defs import (
     AttributeValueTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeServicesRequestDescribeServicesPaginateTypeDef,
     DescribeServicesRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ServiceTypeDef,
     FilterTypeDef,
+    GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
     GetAttributeValuesRequestRequestTypeDef,
     GetPriceListFileUrlRequestRequestTypeDef,
+    GetPriceListFileUrlResponseTypeDef,
+    GetProductsResponseTypeDef,
+    ListPriceListsRequestListPriceListsPaginateTypeDef,
     ListPriceListsRequestRequestTypeDef,
     PriceListTypeDef,
-    DescribeServicesRequestDescribeServicesPaginateTypeDef,
-    GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
-    ListPriceListsRequestListPriceListsPaginateTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     GetAttributeValuesResponseTypeDef,
-    GetPriceListFileUrlResponseTypeDef,
-    GetProductsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     GetProductsRequestGetProductsPaginateTypeDef,
     GetProductsRequestRequestTypeDef,
     ListPriceListsResponseTypeDef,
 )
 
 
@@ -334,42 +334,42 @@
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

### Comparing `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/__init__.py` & `mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/__init__.pyi` & `mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/__main__.py` & `mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Pricing 1.26.82\nVersion:         1.26.82\nBuilder version:"
-        " 7.12.5\nDocs:           "
+        "Type annotations for boto3.Pricing 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.82")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/client.py` & `mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/client.pyi` & `mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/literals.py` & `mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
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
@@ -97,14 +98,15 @@
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
@@ -202,14 +204,15 @@
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
@@ -245,14 +248,15 @@
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
@@ -271,16 +275,19 @@
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
@@ -364,15 +371,17 @@
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

### Comparing `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/literals.pyi` & `mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
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
@@ -95,14 +96,15 @@
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
@@ -200,14 +202,15 @@
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
@@ -243,14 +246,15 @@
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
@@ -269,16 +273,19 @@
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
@@ -362,15 +369,17 @@
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

### Comparing `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/paginator.py` & `mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         FormatVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.DescribeServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#describeservicespaginator)
         """
 
 
@@ -83,15 +83,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         AttributeName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetAttributeValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.GetAttributeValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#getattributevaluespaginator)
         """
 
 
@@ -103,15 +103,15 @@
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         Filters: Sequence[FilterTypeDef] = ...,
         FormatVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetProductsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.GetProducts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#getproductspaginator)
         """
 
 
@@ -124,13 +124,13 @@
     def paginate(
         self,
         *,
         ServiceCode: str,
         EffectiveDate: Union[datetime, str],
         CurrencyCode: str,
         RegionCode: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPriceListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.ListPriceLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#listpricelistspaginator)
         """
```

### Comparing `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/paginator.pyi` & `mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         FormatVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.DescribeServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#describeservicespaginator)
         """
 
 class GetAttributeValuesPaginator(Paginator):
@@ -79,15 +79,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         AttributeName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetAttributeValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.GetAttributeValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#getattributevaluespaginator)
         """
 
 class GetProductsPaginator(Paginator):
@@ -98,15 +98,15 @@
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         Filters: Sequence[FilterTypeDef] = ...,
         FormatVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetProductsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.GetProducts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#getproductspaginator)
         """
 
 class ListPriceListsPaginator(Paginator):
@@ -118,13 +118,13 @@
     def paginate(
         self,
         *,
         ServiceCode: str,
         EffectiveDate: Union[datetime, str],
         CurrencyCode: str,
         RegionCode: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPriceListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.ListPriceLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/paginators/#listpricelistspaginator)
         """
```

### Comparing `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/type_defs.py` & `mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,49 +23,49 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AttributeValueTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
     "DescribeServicesRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ServiceTypeDef",
     "FilterTypeDef",
+    "GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
     "GetAttributeValuesRequestRequestTypeDef",
     "GetPriceListFileUrlRequestRequestTypeDef",
+    "GetPriceListFileUrlResponseTypeDef",
+    "GetProductsResponseTypeDef",
+    "ListPriceListsRequestListPriceListsPaginateTypeDef",
     "ListPriceListsRequestRequestTypeDef",
     "PriceListTypeDef",
-    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
-    "GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
-    "ListPriceListsRequestListPriceListsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "GetAttributeValuesResponseTypeDef",
-    "GetPriceListFileUrlResponseTypeDef",
-    "GetProductsResponseTypeDef",
     "DescribeServicesResponseTypeDef",
     "GetProductsRequestGetProductsPaginateTypeDef",
     "GetProductsRequestRequestTypeDef",
     "ListPriceListsResponseTypeDef",
 )
 
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeServicesRequestDescribeServicesPaginateTypeDef = TypedDict(
+    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ServiceCode": str,
+        "FormatVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeServicesRequestRequestTypeDef = TypedDict(
     "DescribeServicesRequestRequestTypeDef",
     {
@@ -73,25 +73,14 @@
         "FormatVersion": str,
         "NextToken": str,
         "MaxResults": int,
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
 _RequiredServiceTypeDef = TypedDict(
     "_RequiredServiceTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalServiceTypeDef = TypedDict(
@@ -112,189 +101,200 @@
     {
         "Type": Literal["TERM_MATCH"],
         "Field": str,
         "Value": str,
     },
 )
 
-_RequiredGetAttributeValuesRequestRequestTypeDef = TypedDict(
-    "_RequiredGetAttributeValuesRequestRequestTypeDef",
+_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
+    "_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
     {
         "ServiceCode": str,
         "AttributeName": str,
     },
 )
-_OptionalGetAttributeValuesRequestRequestTypeDef = TypedDict(
-    "_OptionalGetAttributeValuesRequestRequestTypeDef",
+_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
+    "_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class GetAttributeValuesRequestRequestTypeDef(
-    _RequiredGetAttributeValuesRequestRequestTypeDef,
-    _OptionalGetAttributeValuesRequestRequestTypeDef,
+class GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef(
+    _RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
+    _OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
 ):
     pass
 
 
-GetPriceListFileUrlRequestRequestTypeDef = TypedDict(
-    "GetPriceListFileUrlRequestRequestTypeDef",
-    {
-        "PriceListArn": str,
-        "FileFormat": str,
-    },
-)
-
-_RequiredListPriceListsRequestRequestTypeDef = TypedDict(
-    "_RequiredListPriceListsRequestRequestTypeDef",
+_RequiredGetAttributeValuesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetAttributeValuesRequestRequestTypeDef",
     {
         "ServiceCode": str,
-        "EffectiveDate": Union[datetime, str],
-        "CurrencyCode": str,
+        "AttributeName": str,
     },
 )
-_OptionalListPriceListsRequestRequestTypeDef = TypedDict(
-    "_OptionalListPriceListsRequestRequestTypeDef",
+_OptionalGetAttributeValuesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetAttributeValuesRequestRequestTypeDef",
     {
-        "RegionCode": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 
-class ListPriceListsRequestRequestTypeDef(
-    _RequiredListPriceListsRequestRequestTypeDef, _OptionalListPriceListsRequestRequestTypeDef
+class GetAttributeValuesRequestRequestTypeDef(
+    _RequiredGetAttributeValuesRequestRequestTypeDef,
+    _OptionalGetAttributeValuesRequestRequestTypeDef,
 ):
     pass
 
 
-PriceListTypeDef = TypedDict(
-    "PriceListTypeDef",
+GetPriceListFileUrlRequestRequestTypeDef = TypedDict(
+    "GetPriceListFileUrlRequestRequestTypeDef",
     {
         "PriceListArn": str,
-        "RegionCode": str,
-        "CurrencyCode": str,
-        "FileFormats": List[str],
+        "FileFormat": str,
     },
-    total=False,
 )
 
-DescribeServicesRequestDescribeServicesPaginateTypeDef = TypedDict(
-    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
+GetPriceListFileUrlResponseTypeDef = TypedDict(
+    "GetPriceListFileUrlResponseTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetProductsResponseTypeDef = TypedDict(
+    "GetProductsResponseTypeDef",
     {
-        "ServiceCode": str,
         "FormatVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PriceList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
-    "_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
+_RequiredListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
+    "_RequiredListPriceListsRequestListPriceListsPaginateTypeDef",
     {
         "ServiceCode": str,
-        "AttributeName": str,
+        "EffectiveDate": Union[datetime, str],
+        "CurrencyCode": str,
     },
 )
-_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
-    "_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
+_OptionalListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
+    "_OptionalListPriceListsRequestListPriceListsPaginateTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "RegionCode": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef(
-    _RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
-    _OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
+class ListPriceListsRequestListPriceListsPaginateTypeDef(
+    _RequiredListPriceListsRequestListPriceListsPaginateTypeDef,
+    _OptionalListPriceListsRequestListPriceListsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
-    "_RequiredListPriceListsRequestListPriceListsPaginateTypeDef",
+_RequiredListPriceListsRequestRequestTypeDef = TypedDict(
+    "_RequiredListPriceListsRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "EffectiveDate": Union[datetime, str],
         "CurrencyCode": str,
     },
 )
-_OptionalListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
-    "_OptionalListPriceListsRequestListPriceListsPaginateTypeDef",
+_OptionalListPriceListsRequestRequestTypeDef = TypedDict(
+    "_OptionalListPriceListsRequestRequestTypeDef",
     {
         "RegionCode": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
     },
     total=False,
 )
 
 
-class ListPriceListsRequestListPriceListsPaginateTypeDef(
-    _RequiredListPriceListsRequestListPriceListsPaginateTypeDef,
-    _OptionalListPriceListsRequestListPriceListsPaginateTypeDef,
+class ListPriceListsRequestRequestTypeDef(
+    _RequiredListPriceListsRequestRequestTypeDef, _OptionalListPriceListsRequestRequestTypeDef
 ):
     pass
 
 
-GetAttributeValuesResponseTypeDef = TypedDict(
-    "GetAttributeValuesResponseTypeDef",
+PriceListTypeDef = TypedDict(
+    "PriceListTypeDef",
     {
-        "AttributeValues": List[AttributeValueTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PriceListArn": str,
+        "RegionCode": str,
+        "CurrencyCode": str,
+        "FileFormats": List[str],
     },
+    total=False,
 )
 
-GetPriceListFileUrlResponseTypeDef = TypedDict(
-    "GetPriceListFileUrlResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-GetProductsResponseTypeDef = TypedDict(
-    "GetProductsResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "FormatVersion": str,
-        "PriceList": List[str],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+GetAttributeValuesResponseTypeDef = TypedDict(
+    "GetAttributeValuesResponseTypeDef",
+    {
+        "AttributeValues": List[AttributeValueTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "Services": List[ServiceTypeDef],
         "FormatVersion": str,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetProductsRequestGetProductsPaginateTypeDef = TypedDict(
     "_RequiredGetProductsRequestGetProductsPaginateTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalGetProductsRequestGetProductsPaginateTypeDef = TypedDict(
     "_OptionalGetProductsRequestGetProductsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "FormatVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class GetProductsRequestGetProductsPaginateTypeDef(
     _RequiredGetProductsRequestGetProductsPaginateTypeDef,
@@ -328,10 +328,10 @@
 
 
 ListPriceListsResponseTypeDef = TypedDict(
     "ListPriceListsResponseTypeDef",
     {
         "PriceLists": List[PriceListTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/type_defs.pyi` & `mypy-boto3-pricing-1.27.0/mypy_boto3_pricing/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,49 +22,49 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AttributeValueTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
     "DescribeServicesRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ServiceTypeDef",
     "FilterTypeDef",
+    "GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
     "GetAttributeValuesRequestRequestTypeDef",
     "GetPriceListFileUrlRequestRequestTypeDef",
+    "GetPriceListFileUrlResponseTypeDef",
+    "GetProductsResponseTypeDef",
+    "ListPriceListsRequestListPriceListsPaginateTypeDef",
     "ListPriceListsRequestRequestTypeDef",
     "PriceListTypeDef",
-    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
-    "GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
-    "ListPriceListsRequestListPriceListsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "GetAttributeValuesResponseTypeDef",
-    "GetPriceListFileUrlResponseTypeDef",
-    "GetProductsResponseTypeDef",
     "DescribeServicesResponseTypeDef",
     "GetProductsRequestGetProductsPaginateTypeDef",
     "GetProductsRequestRequestTypeDef",
     "ListPriceListsResponseTypeDef",
 )
 
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeServicesRequestDescribeServicesPaginateTypeDef = TypedDict(
+    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ServiceCode": str,
+        "FormatVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeServicesRequestRequestTypeDef = TypedDict(
     "DescribeServicesRequestRequestTypeDef",
     {
@@ -72,25 +72,14 @@
         "FormatVersion": str,
         "NextToken": str,
         "MaxResults": int,
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
 _RequiredServiceTypeDef = TypedDict(
     "_RequiredServiceTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalServiceTypeDef = TypedDict(
@@ -109,14 +98,35 @@
     {
         "Type": Literal["TERM_MATCH"],
         "Field": str,
         "Value": str,
     },
 )
 
+_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
+    "_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "AttributeName": str,
+    },
+)
+_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
+    "_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef(
+    _RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
+    _OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
+):
+    pass
+
 _RequiredGetAttributeValuesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAttributeValuesRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "AttributeName": str,
     },
 )
@@ -139,14 +149,55 @@
     "GetPriceListFileUrlRequestRequestTypeDef",
     {
         "PriceListArn": str,
         "FileFormat": str,
     },
 )
 
+GetPriceListFileUrlResponseTypeDef = TypedDict(
+    "GetPriceListFileUrlResponseTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetProductsResponseTypeDef = TypedDict(
+    "GetProductsResponseTypeDef",
+    {
+        "FormatVersion": str,
+        "PriceList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
+    "_RequiredListPriceListsRequestListPriceListsPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "EffectiveDate": Union[datetime, str],
+        "CurrencyCode": str,
+    },
+)
+_OptionalListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
+    "_OptionalListPriceListsRequestListPriceListsPaginateTypeDef",
+    {
+        "RegionCode": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPriceListsRequestListPriceListsPaginateTypeDef(
+    _RequiredListPriceListsRequestListPriceListsPaginateTypeDef,
+    _OptionalListPriceListsRequestListPriceListsPaginateTypeDef,
+):
+    pass
+
 _RequiredListPriceListsRequestRequestTypeDef = TypedDict(
     "_RequiredListPriceListsRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "EffectiveDate": Union[datetime, str],
         "CurrencyCode": str,
     },
@@ -173,117 +224,66 @@
         "RegionCode": str,
         "CurrencyCode": str,
         "FileFormats": List[str],
     },
     total=False,
 )
 
-DescribeServicesRequestDescribeServicesPaginateTypeDef = TypedDict(
-    "DescribeServicesRequestDescribeServicesPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "FormatVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
-    "_RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "AttributeName": str,
-    },
-)
-_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef = TypedDict(
-    "_OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef(
-    _RequiredGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
-    _OptionalGetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
-):
-    pass
-
-_RequiredListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
-    "_RequiredListPriceListsRequestListPriceListsPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "EffectiveDate": Union[datetime, str],
-        "CurrencyCode": str,
-    },
-)
-_OptionalListPriceListsRequestListPriceListsPaginateTypeDef = TypedDict(
-    "_OptionalListPriceListsRequestListPriceListsPaginateTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "RegionCode": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-class ListPriceListsRequestListPriceListsPaginateTypeDef(
-    _RequiredListPriceListsRequestListPriceListsPaginateTypeDef,
-    _OptionalListPriceListsRequestListPriceListsPaginateTypeDef,
-):
-    pass
-
 GetAttributeValuesResponseTypeDef = TypedDict(
     "GetAttributeValuesResponseTypeDef",
     {
         "AttributeValues": List[AttributeValueTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPriceListFileUrlResponseTypeDef = TypedDict(
-    "GetPriceListFileUrlResponseTypeDef",
-    {
-        "Url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetProductsResponseTypeDef = TypedDict(
-    "GetProductsResponseTypeDef",
-    {
-        "FormatVersion": str,
-        "PriceList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "Services": List[ServiceTypeDef],
         "FormatVersion": str,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetProductsRequestGetProductsPaginateTypeDef = TypedDict(
     "_RequiredGetProductsRequestGetProductsPaginateTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalGetProductsRequestGetProductsPaginateTypeDef = TypedDict(
     "_OptionalGetProductsRequestGetProductsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "FormatVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class GetProductsRequestGetProductsPaginateTypeDef(
     _RequiredGetProductsRequestGetProductsPaginateTypeDef,
     _OptionalGetProductsRequestGetProductsPaginateTypeDef,
@@ -313,10 +313,10 @@
     pass
 
 ListPriceListsResponseTypeDef = TypedDict(
     "ListPriceListsResponseTypeDef",
     {
         "PriceLists": List[PriceListTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/PKG-INFO` & `mypy-boto3-pricing-1.27.0/mypy_boto3_pricing.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pricing
-Version: 1.26.82
-Summary: Type annotations for boto3.Pricing 1.26.82 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.Pricing 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-pricing"></a>
 
 # mypy-boto3-pricing
 
 [![PyPI - mypy-boto3-pricing](https://img.shields.io/pypi/v/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pricing?color=blue)](https://pypistats.org/packages/mypy-boto3-pricing)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pricing 1.26.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
+[boto3.Pricing 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
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
 [mypy-boto3-pricing docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,29 +333,29 @@
 
 `mypy_boto3_pricing.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pricing.type_defs import (
     AttributeValueTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeServicesRequestDescribeServicesPaginateTypeDef,
     DescribeServicesRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ServiceTypeDef,
     FilterTypeDef,
+    GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
     GetAttributeValuesRequestRequestTypeDef,
     GetPriceListFileUrlRequestRequestTypeDef,
+    GetPriceListFileUrlResponseTypeDef,
+    GetProductsResponseTypeDef,
+    ListPriceListsRequestListPriceListsPaginateTypeDef,
     ListPriceListsRequestRequestTypeDef,
     PriceListTypeDef,
-    DescribeServicesRequestDescribeServicesPaginateTypeDef,
-    GetAttributeValuesRequestGetAttributeValuesPaginateTypeDef,
-    ListPriceListsRequestListPriceListsPaginateTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     GetAttributeValuesResponseTypeDef,
-    GetPriceListFileUrlResponseTypeDef,
-    GetProductsResponseTypeDef,
     DescribeServicesResponseTypeDef,
     GetProductsRequestGetProductsPaginateTypeDef,
     GetProductsRequestRequestTypeDef,
     ListPriceListsResponseTypeDef,
 )
 
 
@@ -366,42 +366,42 @@
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

### Comparing `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/SOURCES.txt` & `mypy-boto3-pricing-1.27.0/mypy_boto3_pricing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.26.82/setup.py` & `mypy-boto3-pricing-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 Setup script for mypy-boto3-pricing.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pricing",
-    version="1.26.82",
+    version="1.27.0",
     packages=["mypy_boto3_pricing"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Pricing 1.26.82 service generated with mypy-boto3-builder"
-        " 7.12.5"
+        "Type annotations for boto3.Pricing 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/",
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


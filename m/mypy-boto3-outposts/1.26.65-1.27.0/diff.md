# Comparing `tmp/mypy-boto3-outposts-1.26.65.tar.gz` & `tmp/mypy-boto3-outposts-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-outposts-1.26.65.tar", last modified: Mon Feb  6 20:47:28 2023, max compression
+gzip compressed data, was "mypy-boto3-outposts-1.27.0.tar", last modified: Mon Jul  3 19:51:13 2023, max compression
```

## Comparing `mypy-boto3-outposts-1.26.65.tar` & `mypy-boto3-outposts-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:28.141984 mypy-boto3-outposts-1.26.65/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-06 20:47:18.000000 mypy-boto3-outposts-1.26.65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-02-06 20:47:28.141984 mypy-boto3-outposts-1.26.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-02-06 20:47:18.000000 mypy-boto3-outposts-1.26.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:28.141984 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-02-06 20:47:18.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-06 20:47:18.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-06 20:47:18.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-02-06 20:47:18.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18508 2023-02-06 20:47:18.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-02-06 20:47:18.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10542 2023-02-06 20:47:18.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:18.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21380 2023-02-06 20:47:19.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21361 2023-02-06 20:47:18.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-06 20:47:18.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:28.141984 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-02-06 20:47:28.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-02-06 20:47:28.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 20:47:28.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 20:47:28.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-06 20:47:28.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-06 20:47:28.000000 mypy-boto3-outposts-1.26.65/mypy_boto3_outposts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 20:47:28.141984 mypy-boto3-outposts-1.26.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-06 20:47:18.000000 mypy-boto3-outposts-1.26.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:13.227770 mypy-boto3-outposts-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-03 19:51:13.227770 mypy-boto3-outposts-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:13.227770 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18508 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-07-03 19:43:15.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-07-03 19:43:15.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-07-03 19:43:15.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:13.227770 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-03 19:51:13.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-03 19:51:13.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:13.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:13.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:13.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:13.000000 mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:13.227770 mypy-boto3-outposts-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:43:14.000000 mypy-boto3-outposts-1.27.0/setup.py
```

### Comparing `mypy-boto3-outposts-1.26.65/LICENSE` & `mypy-boto3-outposts-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-outposts-1.26.65/PKG-INFO` & `mypy-boto3-outposts-1.27.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-outposts
-Version: 1.26.65
-Summary: Type annotations for boto3.Outposts 1.26.65 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Outposts 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-outposts"></a>
 
 # mypy-boto3-outposts
 
 [![PyPI - mypy-boto3-outposts](https://img.shields.io/pypi/v/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.26.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,15 +325,14 @@
     AddressTypeDef,
     AssetLocationTypeDef,
     ComputeAttributesTypeDef,
     CancelOrderInputRequestTypeDef,
     EC2CapacityTypeDef,
     ConnectionDetailsTypeDef,
     LineItemRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateOutpostInputRequestTypeDef,
     OutpostTypeDef,
     RackPhysicalPropertiesTypeDef,
     DeleteOutpostInputRequestTypeDef,
     DeleteSiteInputRequestTypeDef,
     GetCatalogItemInputRequestTypeDef,
     GetConnectionRequestRequestTypeDef,
@@ -348,29 +347,30 @@
     ListAssetsInputRequestTypeDef,
     ListCatalogItemsInputRequestTypeDef,
     ListOrdersInputRequestTypeDef,
     OrderSummaryTypeDef,
     ListOutpostsInputRequestTypeDef,
     ListSitesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     StartConnectionRequestRequestTypeDef,
+    StartConnectionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateOutpostInputRequestTypeDef,
     UpdateSiteInputRequestTypeDef,
     UpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
+    GetSiteAddressOutputTypeDef,
     UpdateSiteAddressInputRequestTypeDef,
+    UpdateSiteAddressOutputTypeDef,
     AssetInfoTypeDef,
     CatalogItemTypeDef,
-    CreateOrderInputRequestTypeDef,
     GetConnectionResponseTypeDef,
-    GetSiteAddressOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartConnectionResponseTypeDef,
-    UpdateSiteAddressOutputTypeDef,
+    CreateOrderInputRequestTypeDef,
     CreateOutpostOutputTypeDef,
     GetOutpostOutputTypeDef,
     ListOutpostsOutputTypeDef,
     UpdateOutpostOutputTypeDef,
     CreateSiteInputRequestTypeDef,
     SiteTypeDef,
     GetOutpostInstanceTypesOutputTypeDef,
@@ -397,42 +397,42 @@
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

### Comparing `mypy-boto3-outposts-1.26.65/README.md` & `mypy-boto3-outposts-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-outposts"></a>
 
 # mypy-boto3-outposts
 
 [![PyPI - mypy-boto3-outposts](https://img.shields.io/pypi/v/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.26.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,15 +293,14 @@
     AddressTypeDef,
     AssetLocationTypeDef,
     ComputeAttributesTypeDef,
     CancelOrderInputRequestTypeDef,
     EC2CapacityTypeDef,
     ConnectionDetailsTypeDef,
     LineItemRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateOutpostInputRequestTypeDef,
     OutpostTypeDef,
     RackPhysicalPropertiesTypeDef,
     DeleteOutpostInputRequestTypeDef,
     DeleteSiteInputRequestTypeDef,
     GetCatalogItemInputRequestTypeDef,
     GetConnectionRequestRequestTypeDef,
@@ -316,29 +315,30 @@
     ListAssetsInputRequestTypeDef,
     ListCatalogItemsInputRequestTypeDef,
     ListOrdersInputRequestTypeDef,
     OrderSummaryTypeDef,
     ListOutpostsInputRequestTypeDef,
     ListSitesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     StartConnectionRequestRequestTypeDef,
+    StartConnectionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateOutpostInputRequestTypeDef,
     UpdateSiteInputRequestTypeDef,
     UpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
+    GetSiteAddressOutputTypeDef,
     UpdateSiteAddressInputRequestTypeDef,
+    UpdateSiteAddressOutputTypeDef,
     AssetInfoTypeDef,
     CatalogItemTypeDef,
-    CreateOrderInputRequestTypeDef,
     GetConnectionResponseTypeDef,
-    GetSiteAddressOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartConnectionResponseTypeDef,
-    UpdateSiteAddressOutputTypeDef,
+    CreateOrderInputRequestTypeDef,
     CreateOutpostOutputTypeDef,
     GetOutpostOutputTypeDef,
     ListOutpostsOutputTypeDef,
     UpdateOutpostOutputTypeDef,
     CreateSiteInputRequestTypeDef,
     SiteTypeDef,
     GetOutpostInstanceTypesOutputTypeDef,
@@ -365,42 +365,42 @@
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

### Comparing `mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/__main__.py` & `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Outposts 1.26.65\nVersion:         1.26.65\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Outposts 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.65")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/client.py` & `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/client.pyi` & `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/literals.py` & `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,14 +133,15 @@
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
@@ -180,14 +181,15 @@
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
@@ -266,14 +268,15 @@
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
@@ -284,14 +287,15 @@
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
@@ -327,14 +331,15 @@
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
@@ -353,16 +358,19 @@
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
@@ -442,18 +450,21 @@
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

### Comparing `mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/literals.pyi` & `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -131,14 +131,15 @@
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
@@ -178,14 +179,15 @@
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
@@ -264,14 +266,15 @@
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
@@ -282,14 +285,15 @@
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
@@ -325,14 +329,15 @@
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
@@ -351,16 +356,19 @@
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
@@ -440,18 +448,21 @@
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

### Comparing `mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/type_defs.py` & `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     "AddressTypeDef",
     "AssetLocationTypeDef",
     "ComputeAttributesTypeDef",
     "CancelOrderInputRequestTypeDef",
     "EC2CapacityTypeDef",
     "ConnectionDetailsTypeDef",
     "LineItemRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateOutpostInputRequestTypeDef",
     "OutpostTypeDef",
     "RackPhysicalPropertiesTypeDef",
     "DeleteOutpostInputRequestTypeDef",
     "DeleteSiteInputRequestTypeDef",
     "GetCatalogItemInputRequestTypeDef",
     "GetConnectionRequestRequestTypeDef",
@@ -77,29 +76,30 @@
     "ListAssetsInputRequestTypeDef",
     "ListCatalogItemsInputRequestTypeDef",
     "ListOrdersInputRequestTypeDef",
     "OrderSummaryTypeDef",
     "ListOutpostsInputRequestTypeDef",
     "ListSitesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "StartConnectionRequestRequestTypeDef",
+    "StartConnectionResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateOutpostInputRequestTypeDef",
     "UpdateSiteInputRequestTypeDef",
     "UpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
+    "GetSiteAddressOutputTypeDef",
     "UpdateSiteAddressInputRequestTypeDef",
+    "UpdateSiteAddressOutputTypeDef",
     "AssetInfoTypeDef",
     "CatalogItemTypeDef",
-    "CreateOrderInputRequestTypeDef",
     "GetConnectionResponseTypeDef",
-    "GetSiteAddressOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartConnectionResponseTypeDef",
-    "UpdateSiteAddressOutputTypeDef",
+    "CreateOrderInputRequestTypeDef",
     "CreateOutpostOutputTypeDef",
     "GetOutpostOutputTypeDef",
     "ListOutpostsOutputTypeDef",
     "UpdateOutpostOutputTypeDef",
     "CreateSiteInputRequestTypeDef",
     "SiteTypeDef",
     "GetOutpostInstanceTypesOutputTypeDef",
@@ -198,25 +198,14 @@
     {
         "CatalogItemId": str,
         "Quantity": int,
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
 _RequiredCreateOutpostInputRequestTypeDef = TypedDict(
     "_RequiredCreateOutpostInputRequestTypeDef",
     {
         "Name": str,
         "SiteId": str,
     },
 )
@@ -467,24 +456,52 @@
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
 StartConnectionRequestRequestTypeDef = TypedDict(
     "StartConnectionRequestRequestTypeDef",
     {
         "DeviceSerialNumber": str,
         "AssetId": str,
         "ClientPublicKey": str,
         "NetworkInterfaceDeviceIndex": int,
     },
 )
 
+StartConnectionResponseTypeDef = TypedDict(
+    "StartConnectionResponseTypeDef",
+    {
+        "ConnectionId": str,
+        "UnderlayIpAddress": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -569,23 +586,42 @@
 class UpdateSiteRackPhysicalPropertiesInputRequestTypeDef(
     _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
     _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
 ):
     pass
 
 
+GetSiteAddressOutputTypeDef = TypedDict(
+    "GetSiteAddressOutputTypeDef",
+    {
+        "SiteId": str,
+        "AddressType": AddressTypeType,
+        "Address": AddressTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateSiteAddressInputRequestTypeDef = TypedDict(
     "UpdateSiteAddressInputRequestTypeDef",
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
         "Address": AddressTypeDef,
     },
 )
 
+UpdateSiteAddressOutputTypeDef = TypedDict(
+    "UpdateSiteAddressOutputTypeDef",
+    {
+        "AddressType": AddressTypeType,
+        "Address": AddressTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AssetInfoTypeDef = TypedDict(
     "AssetInfoTypeDef",
     {
         "AssetId": str,
         "RackId": str,
         "AssetType": Literal["COMPUTE"],
         "ComputeAttributes": ComputeAttributesTypeDef,
@@ -604,14 +640,23 @@
         "WeightLbs": int,
         "SupportedUplinkGbps": List[int],
         "SupportedStorage": List[SupportedStorageEnumType],
     },
     total=False,
 )
 
+GetConnectionResponseTypeDef = TypedDict(
+    "GetConnectionResponseTypeDef",
+    {
+        "ConnectionId": str,
+        "ConnectionDetails": ConnectionDetailsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateOrderInputRequestTypeDef = TypedDict(
     "_RequiredCreateOrderInputRequestTypeDef",
     {
         "OutpostIdentifier": str,
         "LineItems": Sequence[LineItemRequestTypeDef],
         "PaymentOption": PaymentOptionType,
     },
@@ -627,89 +672,44 @@
 
 class CreateOrderInputRequestTypeDef(
     _RequiredCreateOrderInputRequestTypeDef, _OptionalCreateOrderInputRequestTypeDef
 ):
     pass
 
 
-GetConnectionResponseTypeDef = TypedDict(
-    "GetConnectionResponseTypeDef",
-    {
-        "ConnectionId": str,
-        "ConnectionDetails": ConnectionDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSiteAddressOutputTypeDef = TypedDict(
-    "GetSiteAddressOutputTypeDef",
-    {
-        "SiteId": str,
-        "AddressType": AddressTypeType,
-        "Address": AddressTypeDef,
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
-StartConnectionResponseTypeDef = TypedDict(
-    "StartConnectionResponseTypeDef",
-    {
-        "ConnectionId": str,
-        "UnderlayIpAddress": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSiteAddressOutputTypeDef = TypedDict(
-    "UpdateSiteAddressOutputTypeDef",
-    {
-        "AddressType": AddressTypeType,
-        "Address": AddressTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateOutpostOutputTypeDef = TypedDict(
     "CreateOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOutpostOutputTypeDef = TypedDict(
     "GetOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOutpostsOutputTypeDef = TypedDict(
     "ListOutpostsOutputTypeDef",
     {
         "Outposts": List[OutpostTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateOutpostOutputTypeDef = TypedDict(
     "UpdateOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSiteInputRequestTypeDef = TypedDict(
     "_RequiredCreateSiteInputRequestTypeDef",
     {
         "Name": str,
@@ -756,15 +756,15 @@
 GetOutpostInstanceTypesOutputTypeDef = TypedDict(
     "GetOutpostInstanceTypesOutputTypeDef",
     {
         "InstanceTypes": List[InstanceTypeItemTypeDef],
         "NextToken": str,
         "OutpostId": str,
         "OutpostArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LineItemTypeDef = TypedDict(
     "LineItemTypeDef",
     {
         "CatalogItemId": str,
@@ -780,82 +780,82 @@
 )
 
 ListOrdersOutputTypeDef = TypedDict(
     "ListOrdersOutputTypeDef",
     {
         "Orders": List[OrderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssetsOutputTypeDef = TypedDict(
     "ListAssetsOutputTypeDef",
     {
         "Assets": List[AssetInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCatalogItemOutputTypeDef = TypedDict(
     "GetCatalogItemOutputTypeDef",
     {
         "CatalogItem": CatalogItemTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCatalogItemsOutputTypeDef = TypedDict(
     "ListCatalogItemsOutputTypeDef",
     {
         "CatalogItems": List[CatalogItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSiteOutputTypeDef = TypedDict(
     "CreateSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSiteOutputTypeDef = TypedDict(
     "GetSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSitesOutputTypeDef = TypedDict(
     "ListSitesOutputTypeDef",
     {
         "Sites": List[SiteTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSiteOutputTypeDef = TypedDict(
     "UpdateSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSiteRackPhysicalPropertiesOutputTypeDef = TypedDict(
     "UpdateSiteRackPhysicalPropertiesOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OrderTypeDef = TypedDict(
     "OrderTypeDef",
     {
         "OutpostId": str,
@@ -871,18 +871,18 @@
     total=False,
 )
 
 CreateOrderOutputTypeDef = TypedDict(
     "CreateOrderOutputTypeDef",
     {
         "Order": OrderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOrderOutputTypeDef = TypedDict(
     "GetOrderOutputTypeDef",
     {
         "Order": OrderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-outposts-1.26.65/mypy_boto3_outposts/type_defs.pyi` & `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,14 @@
     "AddressTypeDef",
     "AssetLocationTypeDef",
     "ComputeAttributesTypeDef",
     "CancelOrderInputRequestTypeDef",
     "EC2CapacityTypeDef",
     "ConnectionDetailsTypeDef",
     "LineItemRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateOutpostInputRequestTypeDef",
     "OutpostTypeDef",
     "RackPhysicalPropertiesTypeDef",
     "DeleteOutpostInputRequestTypeDef",
     "DeleteSiteInputRequestTypeDef",
     "GetCatalogItemInputRequestTypeDef",
     "GetConnectionRequestRequestTypeDef",
@@ -76,29 +75,30 @@
     "ListAssetsInputRequestTypeDef",
     "ListCatalogItemsInputRequestTypeDef",
     "ListOrdersInputRequestTypeDef",
     "OrderSummaryTypeDef",
     "ListOutpostsInputRequestTypeDef",
     "ListSitesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "StartConnectionRequestRequestTypeDef",
+    "StartConnectionResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateOutpostInputRequestTypeDef",
     "UpdateSiteInputRequestTypeDef",
     "UpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
+    "GetSiteAddressOutputTypeDef",
     "UpdateSiteAddressInputRequestTypeDef",
+    "UpdateSiteAddressOutputTypeDef",
     "AssetInfoTypeDef",
     "CatalogItemTypeDef",
-    "CreateOrderInputRequestTypeDef",
     "GetConnectionResponseTypeDef",
-    "GetSiteAddressOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartConnectionResponseTypeDef",
-    "UpdateSiteAddressOutputTypeDef",
+    "CreateOrderInputRequestTypeDef",
     "CreateOutpostOutputTypeDef",
     "GetOutpostOutputTypeDef",
     "ListOutpostsOutputTypeDef",
     "UpdateOutpostOutputTypeDef",
     "CreateSiteInputRequestTypeDef",
     "SiteTypeDef",
     "GetOutpostInstanceTypesOutputTypeDef",
@@ -195,25 +195,14 @@
     {
         "CatalogItemId": str,
         "Quantity": int,
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
 _RequiredCreateOutpostInputRequestTypeDef = TypedDict(
     "_RequiredCreateOutpostInputRequestTypeDef",
     {
         "Name": str,
         "SiteId": str,
     },
 )
@@ -458,24 +447,52 @@
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
 StartConnectionRequestRequestTypeDef = TypedDict(
     "StartConnectionRequestRequestTypeDef",
     {
         "DeviceSerialNumber": str,
         "AssetId": str,
         "ClientPublicKey": str,
         "NetworkInterfaceDeviceIndex": int,
     },
 )
 
+StartConnectionResponseTypeDef = TypedDict(
+    "StartConnectionResponseTypeDef",
+    {
+        "ConnectionId": str,
+        "UnderlayIpAddress": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -554,23 +571,42 @@
 
 class UpdateSiteRackPhysicalPropertiesInputRequestTypeDef(
     _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
     _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
 ):
     pass
 
+GetSiteAddressOutputTypeDef = TypedDict(
+    "GetSiteAddressOutputTypeDef",
+    {
+        "SiteId": str,
+        "AddressType": AddressTypeType,
+        "Address": AddressTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateSiteAddressInputRequestTypeDef = TypedDict(
     "UpdateSiteAddressInputRequestTypeDef",
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
         "Address": AddressTypeDef,
     },
 )
 
+UpdateSiteAddressOutputTypeDef = TypedDict(
+    "UpdateSiteAddressOutputTypeDef",
+    {
+        "AddressType": AddressTypeType,
+        "Address": AddressTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AssetInfoTypeDef = TypedDict(
     "AssetInfoTypeDef",
     {
         "AssetId": str,
         "RackId": str,
         "AssetType": Literal["COMPUTE"],
         "ComputeAttributes": ComputeAttributesTypeDef,
@@ -589,14 +625,23 @@
         "WeightLbs": int,
         "SupportedUplinkGbps": List[int],
         "SupportedStorage": List[SupportedStorageEnumType],
     },
     total=False,
 )
 
+GetConnectionResponseTypeDef = TypedDict(
+    "GetConnectionResponseTypeDef",
+    {
+        "ConnectionId": str,
+        "ConnectionDetails": ConnectionDetailsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateOrderInputRequestTypeDef = TypedDict(
     "_RequiredCreateOrderInputRequestTypeDef",
     {
         "OutpostIdentifier": str,
         "LineItems": Sequence[LineItemRequestTypeDef],
         "PaymentOption": PaymentOptionType,
     },
@@ -610,89 +655,44 @@
 )
 
 class CreateOrderInputRequestTypeDef(
     _RequiredCreateOrderInputRequestTypeDef, _OptionalCreateOrderInputRequestTypeDef
 ):
     pass
 
-GetConnectionResponseTypeDef = TypedDict(
-    "GetConnectionResponseTypeDef",
-    {
-        "ConnectionId": str,
-        "ConnectionDetails": ConnectionDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSiteAddressOutputTypeDef = TypedDict(
-    "GetSiteAddressOutputTypeDef",
-    {
-        "SiteId": str,
-        "AddressType": AddressTypeType,
-        "Address": AddressTypeDef,
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
-StartConnectionResponseTypeDef = TypedDict(
-    "StartConnectionResponseTypeDef",
-    {
-        "ConnectionId": str,
-        "UnderlayIpAddress": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSiteAddressOutputTypeDef = TypedDict(
-    "UpdateSiteAddressOutputTypeDef",
-    {
-        "AddressType": AddressTypeType,
-        "Address": AddressTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateOutpostOutputTypeDef = TypedDict(
     "CreateOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOutpostOutputTypeDef = TypedDict(
     "GetOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOutpostsOutputTypeDef = TypedDict(
     "ListOutpostsOutputTypeDef",
     {
         "Outposts": List[OutpostTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateOutpostOutputTypeDef = TypedDict(
     "UpdateOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSiteInputRequestTypeDef = TypedDict(
     "_RequiredCreateSiteInputRequestTypeDef",
     {
         "Name": str,
@@ -737,15 +737,15 @@
 GetOutpostInstanceTypesOutputTypeDef = TypedDict(
     "GetOutpostInstanceTypesOutputTypeDef",
     {
         "InstanceTypes": List[InstanceTypeItemTypeDef],
         "NextToken": str,
         "OutpostId": str,
         "OutpostArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LineItemTypeDef = TypedDict(
     "LineItemTypeDef",
     {
         "CatalogItemId": str,
@@ -761,82 +761,82 @@
 )
 
 ListOrdersOutputTypeDef = TypedDict(
     "ListOrdersOutputTypeDef",
     {
         "Orders": List[OrderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssetsOutputTypeDef = TypedDict(
     "ListAssetsOutputTypeDef",
     {
         "Assets": List[AssetInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCatalogItemOutputTypeDef = TypedDict(
     "GetCatalogItemOutputTypeDef",
     {
         "CatalogItem": CatalogItemTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCatalogItemsOutputTypeDef = TypedDict(
     "ListCatalogItemsOutputTypeDef",
     {
         "CatalogItems": List[CatalogItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSiteOutputTypeDef = TypedDict(
     "CreateSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSiteOutputTypeDef = TypedDict(
     "GetSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSitesOutputTypeDef = TypedDict(
     "ListSitesOutputTypeDef",
     {
         "Sites": List[SiteTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSiteOutputTypeDef = TypedDict(
     "UpdateSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSiteRackPhysicalPropertiesOutputTypeDef = TypedDict(
     "UpdateSiteRackPhysicalPropertiesOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OrderTypeDef = TypedDict(
     "OrderTypeDef",
     {
         "OutpostId": str,
@@ -852,18 +852,18 @@
     total=False,
 )
 
 CreateOrderOutputTypeDef = TypedDict(
     "CreateOrderOutputTypeDef",
     {
         "Order": OrderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOrderOutputTypeDef = TypedDict(
     "GetOrderOutputTypeDef",
     {
         "Order": OrderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-outposts-1.26.65/mypy_boto3_outposts.egg-info/PKG-INFO` & `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-outposts
-Version: 1.26.65
-Summary: Type annotations for boto3.Outposts 1.26.65 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Outposts 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-outposts"></a>
 
 # mypy-boto3-outposts
 
 [![PyPI - mypy-boto3-outposts](https://img.shields.io/pypi/v/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.26.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,15 +325,14 @@
     AddressTypeDef,
     AssetLocationTypeDef,
     ComputeAttributesTypeDef,
     CancelOrderInputRequestTypeDef,
     EC2CapacityTypeDef,
     ConnectionDetailsTypeDef,
     LineItemRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateOutpostInputRequestTypeDef,
     OutpostTypeDef,
     RackPhysicalPropertiesTypeDef,
     DeleteOutpostInputRequestTypeDef,
     DeleteSiteInputRequestTypeDef,
     GetCatalogItemInputRequestTypeDef,
     GetConnectionRequestRequestTypeDef,
@@ -348,29 +347,30 @@
     ListAssetsInputRequestTypeDef,
     ListCatalogItemsInputRequestTypeDef,
     ListOrdersInputRequestTypeDef,
     OrderSummaryTypeDef,
     ListOutpostsInputRequestTypeDef,
     ListSitesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     StartConnectionRequestRequestTypeDef,
+    StartConnectionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateOutpostInputRequestTypeDef,
     UpdateSiteInputRequestTypeDef,
     UpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
+    GetSiteAddressOutputTypeDef,
     UpdateSiteAddressInputRequestTypeDef,
+    UpdateSiteAddressOutputTypeDef,
     AssetInfoTypeDef,
     CatalogItemTypeDef,
-    CreateOrderInputRequestTypeDef,
     GetConnectionResponseTypeDef,
-    GetSiteAddressOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartConnectionResponseTypeDef,
-    UpdateSiteAddressOutputTypeDef,
+    CreateOrderInputRequestTypeDef,
     CreateOutpostOutputTypeDef,
     GetOutpostOutputTypeDef,
     ListOutpostsOutputTypeDef,
     UpdateOutpostOutputTypeDef,
     CreateSiteInputRequestTypeDef,
     SiteTypeDef,
     GetOutpostInstanceTypesOutputTypeDef,
@@ -397,42 +397,42 @@
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

### Comparing `mypy-boto3-outposts-1.26.65/mypy_boto3_outposts.egg-info/SOURCES.txt` & `mypy-boto3-outposts-1.27.0/mypy_boto3_outposts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.26.65/setup.py` & `mypy-boto3-outposts-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-outposts.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-outposts",
-    version="1.26.65",
+    version="1.27.0",
     packages=["mypy_boto3_outposts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Outposts 1.26.65 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.Outposts 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/",
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


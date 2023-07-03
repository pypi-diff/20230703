# Comparing `tmp/mypy-boto3-mediastore-data-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-mediastore-data-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediastore-data-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:44 2022, max compression
+gzip compressed data, was "mypy-boto3-mediastore-data-1.27.0.tar", last modified: Mon Jul  3 19:51:07 2023, max compression
```

## Comparing `mypy-boto3-mediastore-data-1.26.0.post1.tar` & `mypy-boto3-mediastore-data-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:44.184835 mypy-boto3-mediastore-data-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:38:10.000000 mypy-boto3-mediastore-data-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13357 2022-11-01 21:43:44.176835 mypy-boto3-mediastore-data-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11885 2022-11-01 21:38:10.000000 mypy-boto3-mediastore-data-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:44.172835 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-11-01 21:38:10.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-11-01 21:38:10.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-11-01 21:38:10.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6708 2022-11-01 21:38:10.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     6695 2022-11-01 21:38:10.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7407 2022-11-01 21:38:11.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7405 2022-11-01 21:38:11.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-11-01 21:38:11.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-11-01 21:38:11.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:38:10.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4689 2022-11-01 21:38:11.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4684 2022-11-01 21:38:11.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:38:10.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:44.176835 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13357 2022-11-01 21:43:44.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-11-01 21:43:44.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:44.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:44.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:44.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-01 21:43:44.000000 mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:44.184835 mypy-boto3-mediastore-data-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-11-01 21:38:10.000000 mypy-boto3-mediastore-data-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:07.695671 mypy-boto3-mediastore-data-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:10.000000 mypy-boto3-mediastore-data-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13387 2023-07-03 19:51:07.695671 mypy-boto3-mediastore-data-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-07-03 19:42:10.000000 mypy-boto3-mediastore-data-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:07.691671 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-03 19:42:10.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-03 19:42:10.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 19:42:10.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-07-03 19:42:10.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-03 19:42:10.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-03 19:42:10.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-03 19:42:10.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-03 19:42:10.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-03 19:42:10.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:10.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-03 19:42:11.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-03 19:42:10.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:10.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:07.695671 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13387 2023-07-03 19:51:07.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-03 19:51:07.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:07.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:07.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:07.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 19:51:07.000000 mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:07.695671 mypy-boto3-mediastore-data-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-03 19:42:10.000000 mypy-boto3-mediastore-data-1.27.0/setup.py
```

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/LICENSE` & `mypy-boto3-mediastore-data-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/PKG-INFO` & `mypy-boto3-mediastore-data-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore-data
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.MediaStoreData 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.MediaStoreData 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/
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
 
 <a id="mypy-boto3-mediastore-data"></a>
 
 # mypy-boto3-mediastore-data
 
 [![PyPI - mypy-boto3-mediastore-data](https://img.shields.io/pypi/v/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediastore-data?color=blue)](https://pypistats.org/packages/mypy-boto3-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStoreData 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[boto3.MediaStoreData 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
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
 [mypy-boto3-mediastore-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,67 +325,67 @@
 `mypy_boto3_mediastore_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediastore_data.type_defs import (
     DeleteObjectRequestRequestTypeDef,
     DescribeObjectRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeObjectResponseTypeDef,
     GetObjectRequestRequestTypeDef,
+    GetObjectResponseTypeDef,
     ItemTypeDef,
-    PaginatorConfigTypeDef,
+    ListItemsRequestListItemsPaginateTypeDef,
     ListItemsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutObjectRequestRequestTypeDef,
-    DescribeObjectResponseTypeDef,
-    GetObjectResponseTypeDef,
     PutObjectResponseTypeDef,
+    ResponseMetadataTypeDef,
     ListItemsResponseTypeDef,
-    ListItemsRequestListItemsPaginateTypeDef,
 )
 
 
 def get_structure() -> DeleteObjectRequestRequestTypeDef:
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

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/README.md` & `mypy-boto3-mediastore-data-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mediastore-data"></a>
 
 # mypy-boto3-mediastore-data
 
 [![PyPI - mypy-boto3-mediastore-data](https://img.shields.io/pypi/v/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediastore-data?color=blue)](https://pypistats.org/packages/mypy-boto3-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStoreData 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[boto3.MediaStoreData 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
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
 [mypy-boto3-mediastore-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,67 +293,67 @@
 `mypy_boto3_mediastore_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediastore_data.type_defs import (
     DeleteObjectRequestRequestTypeDef,
     DescribeObjectRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeObjectResponseTypeDef,
     GetObjectRequestRequestTypeDef,
+    GetObjectResponseTypeDef,
     ItemTypeDef,
-    PaginatorConfigTypeDef,
+    ListItemsRequestListItemsPaginateTypeDef,
     ListItemsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutObjectRequestRequestTypeDef,
-    DescribeObjectResponseTypeDef,
-    GetObjectResponseTypeDef,
     PutObjectResponseTypeDef,
+    ResponseMetadataTypeDef,
     ListItemsResponseTypeDef,
-    ListItemsRequestListItemsPaginateTypeDef,
 )
 
 
 def get_structure() -> DeleteObjectRequestRequestTypeDef:
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

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/__init__.py` & `mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/__init__.pyi` & `mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/client.py` & `mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/client.pyi` & `mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/literals.py` & `mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/literals.py`

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
@@ -74,30 +76,35 @@
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
@@ -123,14 +130,15 @@
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
@@ -175,51 +183,57 @@
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
@@ -232,14 +246,15 @@
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
@@ -251,28 +266,35 @@
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
@@ -281,14 +303,15 @@
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
@@ -299,55 +322,64 @@
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

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/literals.pyi` & `mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -46,23 +46,25 @@
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
@@ -72,30 +74,35 @@
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
@@ -121,14 +128,15 @@
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
@@ -173,51 +181,57 @@
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
@@ -230,14 +244,15 @@
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
@@ -249,28 +264,35 @@
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
@@ -279,14 +301,15 @@
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
@@ -297,55 +320,64 @@
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

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/paginator.py` & `mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData.Paginator.ListItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/paginators/#listitemspaginator)
     """
 
     def paginate(
-        self, *, Path: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Path: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData.Paginator.ListItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/paginators/#listitemspaginator)
         """
```

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/paginator.pyi` & `mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData.Paginator.ListItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/paginators/#listitemspaginator)
     """
 
     def paginate(
-        self, *, Path: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Path: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData.Paginator.ListItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/paginators/#listitemspaginator)
         """
```

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/type_defs.py` & `mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DeleteObjectRequestRequestTypeDef",
     "DescribeObjectRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DescribeObjectResponseTypeDef",
     "GetObjectRequestRequestTypeDef",
+    "GetObjectResponseTypeDef",
     "ItemTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListItemsRequestListItemsPaginateTypeDef",
     "ListItemsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutObjectRequestRequestTypeDef",
-    "DescribeObjectResponseTypeDef",
-    "GetObjectResponseTypeDef",
     "PutObjectResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ListItemsResponseTypeDef",
-    "ListItemsRequestListItemsPaginateTypeDef",
 )
 
 DeleteObjectRequestRequestTypeDef = TypedDict(
     "DeleteObjectRequestRequestTypeDef",
     {
         "Path": str,
     },
@@ -55,22 +55,23 @@
 DescribeObjectRequestRequestTypeDef = TypedDict(
     "DescribeObjectRequestRequestTypeDef",
     {
         "Path": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DescribeObjectResponseTypeDef = TypedDict(
+    "DescribeObjectResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ETag": str,
+        "ContentType": str,
+        "ContentLength": int,
+        "CacheControl": str,
+        "LastModified": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetObjectRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectRequestRequestTypeDef",
     {
         "Path": str,
@@ -87,47 +88,71 @@
 
 class GetObjectRequestRequestTypeDef(
     _RequiredGetObjectRequestRequestTypeDef, _OptionalGetObjectRequestRequestTypeDef
 ):
     pass
 
 
+GetObjectResponseTypeDef = TypedDict(
+    "GetObjectResponseTypeDef",
+    {
+        "Body": StreamingBody,
+        "CacheControl": str,
+        "ContentRange": str,
+        "ContentLength": int,
+        "ContentType": str,
+        "ETag": str,
+        "LastModified": datetime,
+        "StatusCode": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ItemTypeDef = TypedDict(
     "ItemTypeDef",
     {
         "Name": str,
         "Type": ItemTypeType,
         "ETag": str,
         "LastModified": datetime,
         "ContentType": str,
         "ContentLength": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListItemsRequestListItemsPaginateTypeDef = TypedDict(
+    "ListItemsRequestListItemsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Path": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListItemsRequestRequestTypeDef = TypedDict(
     "ListItemsRequestRequestTypeDef",
     {
         "Path": str,
         "MaxResults": int,
         "NextToken": str,
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
 _RequiredPutObjectRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectRequestRequestTypeDef",
     {
         "Body": Union[str, bytes, IO[Any], StreamingBody],
         "Path": str,
     },
 )
@@ -145,61 +170,36 @@
 
 class PutObjectRequestRequestTypeDef(
     _RequiredPutObjectRequestRequestTypeDef, _OptionalPutObjectRequestRequestTypeDef
 ):
     pass
 
 
-DescribeObjectResponseTypeDef = TypedDict(
-    "DescribeObjectResponseTypeDef",
-    {
-        "ETag": str,
-        "ContentType": str,
-        "ContentLength": int,
-        "CacheControl": str,
-        "LastModified": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetObjectResponseTypeDef = TypedDict(
-    "GetObjectResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "CacheControl": str,
-        "ContentRange": str,
-        "ContentLength": int,
-        "ContentType": str,
-        "ETag": str,
-        "LastModified": datetime,
-        "StatusCode": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PutObjectResponseTypeDef = TypedDict(
     "PutObjectResponseTypeDef",
     {
         "ContentSHA256": str,
         "ETag": str,
         "StorageClass": Literal["TEMPORAL"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListItemsResponseTypeDef = TypedDict(
-    "ListItemsResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Items": List[ItemTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-ListItemsRequestListItemsPaginateTypeDef = TypedDict(
-    "ListItemsRequestListItemsPaginateTypeDef",
+ListItemsResponseTypeDef = TypedDict(
+    "ListItemsResponseTypeDef",
     {
-        "Path": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Items": List[ItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
```

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data/type_defs.pyi` & `mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -27,25 +27,25 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DeleteObjectRequestRequestTypeDef",
     "DescribeObjectRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DescribeObjectResponseTypeDef",
     "GetObjectRequestRequestTypeDef",
+    "GetObjectResponseTypeDef",
     "ItemTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListItemsRequestListItemsPaginateTypeDef",
     "ListItemsRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutObjectRequestRequestTypeDef",
-    "DescribeObjectResponseTypeDef",
-    "GetObjectResponseTypeDef",
     "PutObjectResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ListItemsResponseTypeDef",
-    "ListItemsRequestListItemsPaginateTypeDef",
 )
 
 DeleteObjectRequestRequestTypeDef = TypedDict(
     "DeleteObjectRequestRequestTypeDef",
     {
         "Path": str,
     },
@@ -54,22 +54,23 @@
 DescribeObjectRequestRequestTypeDef = TypedDict(
     "DescribeObjectRequestRequestTypeDef",
     {
         "Path": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DescribeObjectResponseTypeDef = TypedDict(
+    "DescribeObjectResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ETag": str,
+        "ContentType": str,
+        "ContentLength": int,
+        "CacheControl": str,
+        "LastModified": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetObjectRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectRequestRequestTypeDef",
     {
         "Path": str,
@@ -84,47 +85,71 @@
 )
 
 class GetObjectRequestRequestTypeDef(
     _RequiredGetObjectRequestRequestTypeDef, _OptionalGetObjectRequestRequestTypeDef
 ):
     pass
 
+GetObjectResponseTypeDef = TypedDict(
+    "GetObjectResponseTypeDef",
+    {
+        "Body": StreamingBody,
+        "CacheControl": str,
+        "ContentRange": str,
+        "ContentLength": int,
+        "ContentType": str,
+        "ETag": str,
+        "LastModified": datetime,
+        "StatusCode": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ItemTypeDef = TypedDict(
     "ItemTypeDef",
     {
         "Name": str,
         "Type": ItemTypeType,
         "ETag": str,
         "LastModified": datetime,
         "ContentType": str,
         "ContentLength": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListItemsRequestListItemsPaginateTypeDef = TypedDict(
+    "ListItemsRequestListItemsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Path": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListItemsRequestRequestTypeDef = TypedDict(
     "ListItemsRequestRequestTypeDef",
     {
         "Path": str,
         "MaxResults": int,
         "NextToken": str,
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
 _RequiredPutObjectRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectRequestRequestTypeDef",
     {
         "Body": Union[str, bytes, IO[Any], StreamingBody],
         "Path": str,
     },
 )
@@ -140,61 +165,36 @@
 )
 
 class PutObjectRequestRequestTypeDef(
     _RequiredPutObjectRequestRequestTypeDef, _OptionalPutObjectRequestRequestTypeDef
 ):
     pass
 
-DescribeObjectResponseTypeDef = TypedDict(
-    "DescribeObjectResponseTypeDef",
-    {
-        "ETag": str,
-        "ContentType": str,
-        "ContentLength": int,
-        "CacheControl": str,
-        "LastModified": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetObjectResponseTypeDef = TypedDict(
-    "GetObjectResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "CacheControl": str,
-        "ContentRange": str,
-        "ContentLength": int,
-        "ContentType": str,
-        "ETag": str,
-        "LastModified": datetime,
-        "StatusCode": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PutObjectResponseTypeDef = TypedDict(
     "PutObjectResponseTypeDef",
     {
         "ContentSHA256": str,
         "ETag": str,
         "StorageClass": Literal["TEMPORAL"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListItemsResponseTypeDef = TypedDict(
-    "ListItemsResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Items": List[ItemTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-ListItemsRequestListItemsPaginateTypeDef = TypedDict(
-    "ListItemsRequestListItemsPaginateTypeDef",
+ListItemsResponseTypeDef = TypedDict(
+    "ListItemsResponseTypeDef",
     {
-        "Path": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Items": List[ItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
```

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data.egg-info/PKG-INFO` & `mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore-data
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.MediaStoreData 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.MediaStoreData 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/
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
 
 <a id="mypy-boto3-mediastore-data"></a>
 
 # mypy-boto3-mediastore-data
 
 [![PyPI - mypy-boto3-mediastore-data](https://img.shields.io/pypi/v/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediastore-data?color=blue)](https://pypistats.org/packages/mypy-boto3-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStoreData 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[boto3.MediaStoreData 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
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
 [mypy-boto3-mediastore-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,67 +325,67 @@
 `mypy_boto3_mediastore_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediastore_data.type_defs import (
     DeleteObjectRequestRequestTypeDef,
     DescribeObjectRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeObjectResponseTypeDef,
     GetObjectRequestRequestTypeDef,
+    GetObjectResponseTypeDef,
     ItemTypeDef,
-    PaginatorConfigTypeDef,
+    ListItemsRequestListItemsPaginateTypeDef,
     ListItemsRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutObjectRequestRequestTypeDef,
-    DescribeObjectResponseTypeDef,
-    GetObjectResponseTypeDef,
     PutObjectResponseTypeDef,
+    ResponseMetadataTypeDef,
     ListItemsResponseTypeDef,
-    ListItemsRequestListItemsPaginateTypeDef,
 )
 
 
 def get_structure() -> DeleteObjectRequestRequestTypeDef:
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

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/mypy_boto3_mediastore_data.egg-info/SOURCES.txt` & `mypy-boto3-mediastore-data-1.27.0/mypy_boto3_mediastore_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.26.0.post1/setup.py` & `mypy-boto3-mediastore-data-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-mediastore-data.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediastore-data",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_mediastore_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaStoreData 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.MediaStoreData 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 mediastore-data type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_mediastore_data": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_mediastore_data": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/",
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


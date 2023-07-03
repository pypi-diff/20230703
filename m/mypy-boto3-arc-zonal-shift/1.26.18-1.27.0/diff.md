# Comparing `tmp/mypy-boto3-arc-zonal-shift-1.26.18.tar.gz` & `tmp/mypy-boto3-arc-zonal-shift-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-arc-zonal-shift-1.26.18.tar", last modified: Tue Nov 29 06:12:18 2022, max compression
+gzip compressed data, was "mypy-boto3-arc-zonal-shift-1.27.0.tar", last modified: Mon Jul  3 19:50:24 2023, max compression
```

## Comparing `mypy-boto3-arc-zonal-shift-1.26.18.tar` & `mypy-boto3-arc-zonal-shift-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:12:18.225821 mypy-boto3-arc-zonal-shift-1.26.18/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    13816 2022-11-29 06:12:18.225821 mypy-boto3-arc-zonal-shift-1.26.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12349 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:12:18.225821 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/
--rw-r--r--   0 runner    (1001) docker     (122)      879 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      878 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      936 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8547 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     8532 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     7674 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)     7672 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     3142 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3138 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     5848 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5843 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:12:18.225821 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    13816 2022-11-29 06:12:18.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      832 2022-11-29 06:12:18.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 06:12:18.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 06:12:18.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-29 06:12:18.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2022-11-29 06:12:18.000000 mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-29 06:12:18.225821 mypy-boto3-arc-zonal-shift-1.26.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2018 2022-11-29 06:09:16.000000 mypy-boto3-arc-zonal-shift-1.26.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.730861 mypy-boto3-arc-zonal-shift-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-07-03 19:50:24.730861 mypy-boto3-arc-zonal-shift-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.730861 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.730861 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-07-03 19:50:24.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-03 19:50:24.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:24.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 19:50:24.000000 mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:24.730861 mypy-boto3-arc-zonal-shift-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-03 19:32:48.000000 mypy-boto3-arc-zonal-shift-1.27.0/setup.py
```

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/LICENSE` & `mypy-boto3-arc-zonal-shift-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/PKG-INFO` & `mypy-boto3-arc-zonal-shift-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-arc-zonal-shift
-Version: 1.26.18
-Summary: Type annotations for boto3.ARCZonalShift 1.26.18 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.ARCZonalShift 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/
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
 
 <a id="mypy-boto3-arc-zonal-shift"></a>
 
 # mypy-boto3-arc-zonal-shift
 
 [![PyPI - mypy-boto3-arc-zonal-shift](https://img.shields.io/pypi/v/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-arc-zonal-shift?color=blue)](https://pypistats.org/packages/mypy-boto3-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ARCZonalShift 1.26.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[boto3.ARCZonalShift 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [mypy-boto3-arc-zonal-shift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,27 +331,27 @@
 `mypy_boto3_arc_zonal_shift.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_arc_zonal_shift.type_defs import (
     CancelZonalShiftRequestRequestTypeDef,
     GetManagedResourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ZonalShiftInResourceTypeDef,
-    PaginatorConfigTypeDef,
+    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
     ListManagedResourcesRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
+    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListZonalShiftsRequestRequestTypeDef,
     ZonalShiftSummaryTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartZonalShiftRequestRequestTypeDef,
     UpdateZonalShiftRequestRequestTypeDef,
     ZonalShiftTypeDef,
     GetManagedResourceResponseTypeDef,
-    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
-    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListManagedResourcesResponseTypeDef,
     ListZonalShiftsResponseTypeDef,
 )
 
 
 def get_structure() -> CancelZonalShiftRequestRequestTypeDef:
     return {...}
@@ -359,42 +360,42 @@
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

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/README.md` & `mypy-boto3-arc-zonal-shift-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-arc-zonal-shift"></a>
 
 # mypy-boto3-arc-zonal-shift
 
 [![PyPI - mypy-boto3-arc-zonal-shift](https://img.shields.io/pypi/v/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-arc-zonal-shift?color=blue)](https://pypistats.org/packages/mypy-boto3-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ARCZonalShift 1.26.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[boto3.ARCZonalShift 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [mypy-boto3-arc-zonal-shift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,27 +299,27 @@
 `mypy_boto3_arc_zonal_shift.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_arc_zonal_shift.type_defs import (
     CancelZonalShiftRequestRequestTypeDef,
     GetManagedResourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ZonalShiftInResourceTypeDef,
-    PaginatorConfigTypeDef,
+    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
     ListManagedResourcesRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
+    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListZonalShiftsRequestRequestTypeDef,
     ZonalShiftSummaryTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartZonalShiftRequestRequestTypeDef,
     UpdateZonalShiftRequestRequestTypeDef,
     ZonalShiftTypeDef,
     GetManagedResourceResponseTypeDef,
-    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
-    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListManagedResourcesResponseTypeDef,
     ListZonalShiftsResponseTypeDef,
 )
 
 
 def get_structure() -> CancelZonalShiftRequestRequestTypeDef:
     return {...}
@@ -328,42 +328,42 @@
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

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/__init__.py` & `mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/__init__.pyi` & `mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/__main__.py` & `mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ARCZonalShift 1.26.18\nVersion:         1.26.18\nBuilder"
-        " version: 7.11.11\nDocs:           "
+        "Type annotations for boto3.ARCZonalShift 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.18")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/client.py` & `mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/client.pyi` & `mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/literals.py` & `mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/literals.py`

 * *Files 7% similar despite different names*

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
@@ -76,30 +77,34 @@
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
@@ -125,14 +130,15 @@
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
@@ -177,14 +183,15 @@
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
@@ -195,34 +202,38 @@
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
@@ -235,14 +246,15 @@
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
@@ -255,28 +267,34 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
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
@@ -304,30 +322,34 @@
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
@@ -343,18 +365,21 @@
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
@@ -374,17 +399,35 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_managed_resources", "list_zonal_shifts"]
 RegionName = Literal[
+    "af-south-1",
+    "ap-east-1",
     "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-northeast-3",
+    "ap-south-1",
+    "ap-south-2",
+    "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
+    "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
+    "eu-west-2",
+    "eu-west-3",
+    "me-central-1",
+    "me-south-1",
+    "sa-east-1",
     "us-east-1",
     "us-east-2",
+    "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/literals.pyi` & `mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,15 @@
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
@@ -74,30 +75,34 @@
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
@@ -123,14 +128,15 @@
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
@@ -175,14 +181,15 @@
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
@@ -193,34 +200,38 @@
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
@@ -233,14 +244,15 @@
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
@@ -253,28 +265,34 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
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
@@ -302,30 +320,34 @@
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
@@ -341,18 +363,21 @@
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
@@ -372,17 +397,35 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_managed_resources", "list_zonal_shifts"]
 RegionName = Literal[
+    "af-south-1",
+    "ap-east-1",
     "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-northeast-3",
+    "ap-south-1",
+    "ap-south-2",
+    "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
+    "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
+    "eu-west-2",
+    "eu-west-3",
+    "me-central-1",
+    "me-south-1",
+    "sa-east-1",
     "us-east-1",
     "us-east-2",
+    "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/paginator.py` & `mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,28 +48,31 @@
 class ListManagedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListManagedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listmanagedresourcespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListManagedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListManagedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listmanagedresourcespaginator)
         """
 
 
 class ListZonalShiftsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListZonalShifts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listzonalshiftspaginator)
     """
 
     def paginate(
-        self, *, status: ZonalShiftStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        status: ZonalShiftStatusType = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListZonalShiftsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListZonalShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listzonalshiftspaginator)
         """
```

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/paginator.pyi` & `mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -45,27 +45,30 @@
 class ListManagedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListManagedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listmanagedresourcespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListManagedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListManagedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listmanagedresourcespaginator)
         """
 
 class ListZonalShiftsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListZonalShifts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listzonalshiftspaginator)
     """
 
     def paginate(
-        self, *, status: ZonalShiftStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        status: ZonalShiftStatusType = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListZonalShiftsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListZonalShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listzonalshiftspaginator)
         """
```

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/type_defs.py` & `mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelZonalShiftRequestRequestTypeDef",
     "GetManagedResourceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ZonalShiftInResourceTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
     "ListManagedResourcesRequestRequestTypeDef",
     "ManagedResourceSummaryTypeDef",
+    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
     "ListZonalShiftsRequestRequestTypeDef",
     "ZonalShiftSummaryTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StartZonalShiftRequestRequestTypeDef",
     "UpdateZonalShiftRequestRequestTypeDef",
     "ZonalShiftTypeDef",
     "GetManagedResourceResponseTypeDef",
-    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
-    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
     "ListManagedResourcesResponseTypeDef",
     "ListZonalShiftsResponseTypeDef",
 )
 
 CancelZonalShiftRequestRequestTypeDef = TypedDict(
     "CancelZonalShiftRequestRequestTypeDef",
     {
@@ -53,44 +53,31 @@
 GetManagedResourceRequestRequestTypeDef = TypedDict(
     "GetManagedResourceRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
     },
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
 ZonalShiftInResourceTypeDef = TypedDict(
     "ZonalShiftInResourceTypeDef",
     {
         "appliedStatus": AppliedStatusType,
         "awayFrom": str,
         "comment": str,
         "expiryTime": datetime,
         "resourceIdentifier": str,
         "startTime": datetime,
         "zonalShiftId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListManagedResourcesRequestListManagedResourcesPaginateTypeDef = TypedDict(
+    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListManagedResourcesRequestRequestTypeDef = TypedDict(
     "ListManagedResourcesRequestRequestTypeDef",
     {
@@ -118,14 +105,23 @@
 
 class ManagedResourceSummaryTypeDef(
     _RequiredManagedResourceSummaryTypeDef, _OptionalManagedResourceSummaryTypeDef
 ):
     pass
 
 
+ListZonalShiftsRequestListZonalShiftsPaginateTypeDef = TypedDict(
+    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
+    {
+        "status": ZonalShiftStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListZonalShiftsRequestRequestTypeDef = TypedDict(
     "ListZonalShiftsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "status": ZonalShiftStatusType,
     },
@@ -141,14 +137,35 @@
         "resourceIdentifier": str,
         "startTime": datetime,
         "status": ZonalShiftStatusType,
         "zonalShiftId": str,
     },
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
 StartZonalShiftRequestRequestTypeDef = TypedDict(
     "StartZonalShiftRequestRequestTypeDef",
     {
         "awayFrom": str,
         "comment": str,
         "expiresIn": str,
         "resourceIdentifier": str,
@@ -183,56 +200,39 @@
         "awayFrom": str,
         "comment": str,
         "expiryTime": datetime,
         "resourceIdentifier": str,
         "startTime": datetime,
         "status": ZonalShiftStatusType,
         "zonalShiftId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetManagedResourceResponseTypeDef = TypedDict(
     "GetManagedResourceResponseTypeDef",
     {
         "appliedWeights": Dict[str, float],
         "arn": str,
         "name": str,
         "zonalShifts": List[ZonalShiftInResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListManagedResourcesRequestListManagedResourcesPaginateTypeDef = TypedDict(
-    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListZonalShiftsRequestListZonalShiftsPaginateTypeDef = TypedDict(
-    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
-    {
-        "status": ZonalShiftStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListManagedResourcesResponseTypeDef = TypedDict(
     "ListManagedResourcesResponseTypeDef",
     {
         "items": List[ManagedResourceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListZonalShiftsResponseTypeDef = TypedDict(
     "ListZonalShiftsResponseTypeDef",
     {
         "items": List[ZonalShiftSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift/type_defs.pyi` & `mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -21,27 +21,27 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelZonalShiftRequestRequestTypeDef",
     "GetManagedResourceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ZonalShiftInResourceTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
     "ListManagedResourcesRequestRequestTypeDef",
     "ManagedResourceSummaryTypeDef",
+    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
     "ListZonalShiftsRequestRequestTypeDef",
     "ZonalShiftSummaryTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StartZonalShiftRequestRequestTypeDef",
     "UpdateZonalShiftRequestRequestTypeDef",
     "ZonalShiftTypeDef",
     "GetManagedResourceResponseTypeDef",
-    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
-    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
     "ListManagedResourcesResponseTypeDef",
     "ListZonalShiftsResponseTypeDef",
 )
 
 CancelZonalShiftRequestRequestTypeDef = TypedDict(
     "CancelZonalShiftRequestRequestTypeDef",
     {
@@ -52,44 +52,31 @@
 GetManagedResourceRequestRequestTypeDef = TypedDict(
     "GetManagedResourceRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
     },
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
 ZonalShiftInResourceTypeDef = TypedDict(
     "ZonalShiftInResourceTypeDef",
     {
         "appliedStatus": AppliedStatusType,
         "awayFrom": str,
         "comment": str,
         "expiryTime": datetime,
         "resourceIdentifier": str,
         "startTime": datetime,
         "zonalShiftId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListManagedResourcesRequestListManagedResourcesPaginateTypeDef = TypedDict(
+    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListManagedResourcesRequestRequestTypeDef = TypedDict(
     "ListManagedResourcesRequestRequestTypeDef",
     {
@@ -115,14 +102,23 @@
 )
 
 class ManagedResourceSummaryTypeDef(
     _RequiredManagedResourceSummaryTypeDef, _OptionalManagedResourceSummaryTypeDef
 ):
     pass
 
+ListZonalShiftsRequestListZonalShiftsPaginateTypeDef = TypedDict(
+    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
+    {
+        "status": ZonalShiftStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListZonalShiftsRequestRequestTypeDef = TypedDict(
     "ListZonalShiftsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "status": ZonalShiftStatusType,
     },
@@ -138,14 +134,35 @@
         "resourceIdentifier": str,
         "startTime": datetime,
         "status": ZonalShiftStatusType,
         "zonalShiftId": str,
     },
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
 StartZonalShiftRequestRequestTypeDef = TypedDict(
     "StartZonalShiftRequestRequestTypeDef",
     {
         "awayFrom": str,
         "comment": str,
         "expiresIn": str,
         "resourceIdentifier": str,
@@ -178,56 +195,39 @@
         "awayFrom": str,
         "comment": str,
         "expiryTime": datetime,
         "resourceIdentifier": str,
         "startTime": datetime,
         "status": ZonalShiftStatusType,
         "zonalShiftId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetManagedResourceResponseTypeDef = TypedDict(
     "GetManagedResourceResponseTypeDef",
     {
         "appliedWeights": Dict[str, float],
         "arn": str,
         "name": str,
         "zonalShifts": List[ZonalShiftInResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListManagedResourcesRequestListManagedResourcesPaginateTypeDef = TypedDict(
-    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListZonalShiftsRequestListZonalShiftsPaginateTypeDef = TypedDict(
-    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
-    {
-        "status": ZonalShiftStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListManagedResourcesResponseTypeDef = TypedDict(
     "ListManagedResourcesResponseTypeDef",
     {
         "items": List[ManagedResourceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListZonalShiftsResponseTypeDef = TypedDict(
     "ListZonalShiftsResponseTypeDef",
     {
         "items": List[ZonalShiftSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO` & `mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-arc-zonal-shift
-Version: 1.26.18
-Summary: Type annotations for boto3.ARCZonalShift 1.26.18 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.ARCZonalShift 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/
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
 
 <a id="mypy-boto3-arc-zonal-shift"></a>
 
 # mypy-boto3-arc-zonal-shift
 
 [![PyPI - mypy-boto3-arc-zonal-shift](https://img.shields.io/pypi/v/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-arc-zonal-shift?color=blue)](https://pypistats.org/packages/mypy-boto3-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ARCZonalShift 1.26.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[boto3.ARCZonalShift 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [mypy-boto3-arc-zonal-shift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,27 +331,27 @@
 `mypy_boto3_arc_zonal_shift.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_arc_zonal_shift.type_defs import (
     CancelZonalShiftRequestRequestTypeDef,
     GetManagedResourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ZonalShiftInResourceTypeDef,
-    PaginatorConfigTypeDef,
+    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
     ListManagedResourcesRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
+    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListZonalShiftsRequestRequestTypeDef,
     ZonalShiftSummaryTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartZonalShiftRequestRequestTypeDef,
     UpdateZonalShiftRequestRequestTypeDef,
     ZonalShiftTypeDef,
     GetManagedResourceResponseTypeDef,
-    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
-    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListManagedResourcesResponseTypeDef,
     ListZonalShiftsResponseTypeDef,
 )
 
 
 def get_structure() -> CancelZonalShiftRequestRequestTypeDef:
     return {...}
@@ -359,42 +360,42 @@
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

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt` & `mypy-boto3-arc-zonal-shift-1.27.0/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.26.18/setup.py` & `mypy-boto3-arc-zonal-shift-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-arc-zonal-shift.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-arc-zonal-shift",
-    version="1.26.18",
+    version="1.27.0",
     packages=["mypy_boto3_arc_zonal_shift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ARCZonalShift 1.26.18 service generated with mypy-boto3-builder"
-        " 7.11.11"
+        "Type annotations for boto3.ARCZonalShift 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 arc-zonal-shift type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_arc_zonal_shift": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_arc_zonal_shift": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/",
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


# Comparing `tmp/mypy-boto3-cloudhsm-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-cloudhsm-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudhsm-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:11 2022, max compression
+gzip compressed data, was "mypy-boto3-cloudhsm-1.27.0.tar", last modified: Mon Jul  3 19:50:29 2023, max compression
```

## Comparing `mypy-boto3-cloudhsm-1.26.0.post1.tar` & `mypy-boto3-cloudhsm-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:11.972840 mypy-boto3-cloudhsm-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:31:32.000000 mypy-boto3-cloudhsm-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14510 2022-11-01 21:43:11.972840 mypy-boto3-cloudhsm-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13065 2022-11-01 21:31:32.000000 mypy-boto3-cloudhsm-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:11.968840 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-11-01 21:31:32.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-11-01 21:31:32.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-01 21:31:32.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15153 2022-11-01 21:31:32.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    15123 2022-11-01 21:31:32.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7579 2022-11-01 21:31:33.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7577 2022-11-01 21:31:32.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2022-11-01 21:31:32.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3746 2022-11-01 21:31:32.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:31:32.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    12585 2022-11-01 21:31:33.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    12576 2022-11-01 21:31:33.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:31:32.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:11.972840 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14510 2022-11-01 21:43:11.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-11-01 21:43:11.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:11.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:11.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:11.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-01 21:43:11.000000 mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:11.972840 mypy-boto3-cloudhsm-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1975 2022-11-01 21:31:32.000000 mypy-boto3-cloudhsm-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.562946 mypy-boto3-cloudhsm-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-07-03 19:50:29.562946 mypy-boto3-cloudhsm-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.554946 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.562946 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-07-03 19:50:29.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 19:50:29.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:29.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:29.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:29.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:50:29.000000 mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:29.562946 mypy-boto3-cloudhsm-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:33:54.000000 mypy-boto3-cloudhsm-1.27.0/setup.py
```

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/LICENSE` & `mypy-boto3-cloudhsm-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/PKG-INFO` & `mypy-boto3-cloudhsm-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudhsm
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CloudHSM 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudHSM 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/
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
 
 <a id="mypy-boto3-cloudhsm"></a>
 
 # mypy-boto3-cloudhsm
 
 [![PyPI - mypy-boto3-cloudhsm](https://img.shields.io/pypi/v/mypy-boto3-cloudhsm.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudhsm.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudhsm?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudHSM 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
+[boto3.CloudHSM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
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
 [mypy-boto3-cloudhsm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,100 +331,100 @@
 
 `mypy_boto3_cloudhsm.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudhsm.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    AddTagsToResourceResponseTypeDef,
     CreateHapgRequestRequestTypeDef,
+    CreateHapgResponseTypeDef,
     CreateHsmRequestRequestTypeDef,
+    CreateHsmResponseTypeDef,
     CreateLunaClientRequestRequestTypeDef,
+    CreateLunaClientResponseTypeDef,
     DeleteHapgRequestRequestTypeDef,
+    DeleteHapgResponseTypeDef,
     DeleteHsmRequestRequestTypeDef,
+    DeleteHsmResponseTypeDef,
     DeleteLunaClientRequestRequestTypeDef,
+    DeleteLunaClientResponseTypeDef,
     DescribeHapgRequestRequestTypeDef,
+    DescribeHapgResponseTypeDef,
     DescribeHsmRequestRequestTypeDef,
+    DescribeHsmResponseTypeDef,
     DescribeLunaClientRequestRequestTypeDef,
+    DescribeLunaClientResponseTypeDef,
     GetConfigRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetConfigResponseTypeDef,
+    ListAvailableZonesResponseTypeDef,
+    ListHapgsRequestListHapgsPaginateTypeDef,
     ListHapgsRequestRequestTypeDef,
+    ListHapgsResponseTypeDef,
+    ListHsmsRequestListHsmsPaginateTypeDef,
     ListHsmsRequestRequestTypeDef,
+    ListHsmsResponseTypeDef,
+    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
     ListLunaClientsRequestRequestTypeDef,
+    ListLunaClientsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyHapgRequestRequestTypeDef,
+    ModifyHapgResponseTypeDef,
     ModifyHsmRequestRequestTypeDef,
+    ModifyHsmResponseTypeDef,
     ModifyLunaClientRequestRequestTypeDef,
+    ModifyLunaClientResponseTypeDef,
+    PaginatorConfigTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
+    RemoveTagsFromResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
-    AddTagsToResourceResponseTypeDef,
-    CreateHapgResponseTypeDef,
-    CreateHsmResponseTypeDef,
-    CreateLunaClientResponseTypeDef,
-    DeleteHapgResponseTypeDef,
-    DeleteHsmResponseTypeDef,
-    DeleteLunaClientResponseTypeDef,
-    DescribeHapgResponseTypeDef,
-    DescribeHsmResponseTypeDef,
-    DescribeLunaClientResponseTypeDef,
-    GetConfigResponseTypeDef,
-    ListAvailableZonesResponseTypeDef,
-    ListHapgsResponseTypeDef,
-    ListHsmsResponseTypeDef,
-    ListLunaClientsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ModifyHapgResponseTypeDef,
-    ModifyHsmResponseTypeDef,
-    ModifyLunaClientResponseTypeDef,
-    RemoveTagsFromResourceResponseTypeDef,
-    ListHapgsRequestListHapgsPaginateTypeDef,
-    ListHsmsRequestListHsmsPaginateTypeDef,
-    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
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

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/README.md` & `mypy-boto3-cloudhsm-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cloudhsm"></a>
 
 # mypy-boto3-cloudhsm
 
 [![PyPI - mypy-boto3-cloudhsm](https://img.shields.io/pypi/v/mypy-boto3-cloudhsm.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudhsm.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudhsm?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudHSM 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
+[boto3.CloudHSM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
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
 [mypy-boto3-cloudhsm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,100 +299,100 @@
 
 `mypy_boto3_cloudhsm.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudhsm.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    AddTagsToResourceResponseTypeDef,
     CreateHapgRequestRequestTypeDef,
+    CreateHapgResponseTypeDef,
     CreateHsmRequestRequestTypeDef,
+    CreateHsmResponseTypeDef,
     CreateLunaClientRequestRequestTypeDef,
+    CreateLunaClientResponseTypeDef,
     DeleteHapgRequestRequestTypeDef,
+    DeleteHapgResponseTypeDef,
     DeleteHsmRequestRequestTypeDef,
+    DeleteHsmResponseTypeDef,
     DeleteLunaClientRequestRequestTypeDef,
+    DeleteLunaClientResponseTypeDef,
     DescribeHapgRequestRequestTypeDef,
+    DescribeHapgResponseTypeDef,
     DescribeHsmRequestRequestTypeDef,
+    DescribeHsmResponseTypeDef,
     DescribeLunaClientRequestRequestTypeDef,
+    DescribeLunaClientResponseTypeDef,
     GetConfigRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetConfigResponseTypeDef,
+    ListAvailableZonesResponseTypeDef,
+    ListHapgsRequestListHapgsPaginateTypeDef,
     ListHapgsRequestRequestTypeDef,
+    ListHapgsResponseTypeDef,
+    ListHsmsRequestListHsmsPaginateTypeDef,
     ListHsmsRequestRequestTypeDef,
+    ListHsmsResponseTypeDef,
+    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
     ListLunaClientsRequestRequestTypeDef,
+    ListLunaClientsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyHapgRequestRequestTypeDef,
+    ModifyHapgResponseTypeDef,
     ModifyHsmRequestRequestTypeDef,
+    ModifyHsmResponseTypeDef,
     ModifyLunaClientRequestRequestTypeDef,
+    ModifyLunaClientResponseTypeDef,
+    PaginatorConfigTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
+    RemoveTagsFromResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
-    AddTagsToResourceResponseTypeDef,
-    CreateHapgResponseTypeDef,
-    CreateHsmResponseTypeDef,
-    CreateLunaClientResponseTypeDef,
-    DeleteHapgResponseTypeDef,
-    DeleteHsmResponseTypeDef,
-    DeleteLunaClientResponseTypeDef,
-    DescribeHapgResponseTypeDef,
-    DescribeHsmResponseTypeDef,
-    DescribeLunaClientResponseTypeDef,
-    GetConfigResponseTypeDef,
-    ListAvailableZonesResponseTypeDef,
-    ListHapgsResponseTypeDef,
-    ListHsmsResponseTypeDef,
-    ListLunaClientsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ModifyHapgResponseTypeDef,
-    ModifyHsmResponseTypeDef,
-    ModifyLunaClientResponseTypeDef,
-    RemoveTagsFromResourceResponseTypeDef,
-    ListHapgsRequestListHapgsPaginateTypeDef,
-    ListHsmsRequestListHsmsPaginateTypeDef,
-    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
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

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/__init__.py` & `mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/__init__.pyi` & `mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/__main__.py` & `mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudHSM 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.CloudHSM 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM\nOther"
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

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/client.py` & `mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/client.pyi` & `mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/literals.py` & `mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,23 +56,25 @@
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
@@ -82,30 +84,35 @@
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
@@ -131,14 +138,15 @@
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
@@ -183,51 +191,57 @@
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
@@ -240,14 +254,15 @@
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
@@ -259,28 +274,35 @@
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
@@ -289,14 +311,15 @@
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
@@ -307,55 +330,64 @@
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

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/literals.pyi` & `mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,25 @@
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
@@ -80,30 +82,35 @@
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
@@ -129,14 +136,15 @@
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
@@ -181,51 +189,57 @@
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
@@ -238,14 +252,15 @@
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
@@ -257,28 +272,35 @@
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
@@ -287,14 +309,15 @@
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
@@ -305,55 +328,64 @@
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

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/paginator.py` & `mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/paginator.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,43 +50,43 @@
 class ListHapgsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHapgs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhapgspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHapgsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHapgs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhapgspaginator)
         """
 
 
 class ListHsmsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHsms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhsmspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHsmsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHsms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhsmspaginator)
         """
 
 
 class ListLunaClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListLunaClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listlunaclientspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLunaClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListLunaClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listlunaclientspaginator)
         """
```

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/paginator.pyi` & `mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/paginator.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -47,41 +47,41 @@
 class ListHapgsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHapgs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhapgspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHapgsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHapgs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhapgspaginator)
         """
 
 class ListHsmsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHsms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhsmspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListHsmsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHsms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhsmspaginator)
         """
 
 class ListLunaClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListLunaClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listlunaclientspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLunaClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListLunaClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listlunaclientspaginator)
         """
```

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/type_defs.py` & `mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,86 +24,91 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddTagsToResourceResponseTypeDef",
     "CreateHapgRequestRequestTypeDef",
+    "CreateHapgResponseTypeDef",
     "CreateHsmRequestRequestTypeDef",
+    "CreateHsmResponseTypeDef",
     "CreateLunaClientRequestRequestTypeDef",
+    "CreateLunaClientResponseTypeDef",
     "DeleteHapgRequestRequestTypeDef",
+    "DeleteHapgResponseTypeDef",
     "DeleteHsmRequestRequestTypeDef",
+    "DeleteHsmResponseTypeDef",
     "DeleteLunaClientRequestRequestTypeDef",
+    "DeleteLunaClientResponseTypeDef",
     "DescribeHapgRequestRequestTypeDef",
+    "DescribeHapgResponseTypeDef",
     "DescribeHsmRequestRequestTypeDef",
+    "DescribeHsmResponseTypeDef",
     "DescribeLunaClientRequestRequestTypeDef",
+    "DescribeLunaClientResponseTypeDef",
     "GetConfigRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetConfigResponseTypeDef",
+    "ListAvailableZonesResponseTypeDef",
+    "ListHapgsRequestListHapgsPaginateTypeDef",
     "ListHapgsRequestRequestTypeDef",
+    "ListHapgsResponseTypeDef",
+    "ListHsmsRequestListHsmsPaginateTypeDef",
     "ListHsmsRequestRequestTypeDef",
+    "ListHsmsResponseTypeDef",
+    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
     "ListLunaClientsRequestRequestTypeDef",
+    "ListLunaClientsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModifyHapgRequestRequestTypeDef",
+    "ModifyHapgResponseTypeDef",
     "ModifyHsmRequestRequestTypeDef",
+    "ModifyHsmResponseTypeDef",
     "ModifyLunaClientRequestRequestTypeDef",
+    "ModifyLunaClientResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
+    "RemoveTagsFromResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
-    "AddTagsToResourceResponseTypeDef",
-    "CreateHapgResponseTypeDef",
-    "CreateHsmResponseTypeDef",
-    "CreateLunaClientResponseTypeDef",
-    "DeleteHapgResponseTypeDef",
-    "DeleteHsmResponseTypeDef",
-    "DeleteLunaClientResponseTypeDef",
-    "DescribeHapgResponseTypeDef",
-    "DescribeHsmResponseTypeDef",
-    "DescribeLunaClientResponseTypeDef",
-    "GetConfigResponseTypeDef",
-    "ListAvailableZonesResponseTypeDef",
-    "ListHapgsResponseTypeDef",
-    "ListHsmsResponseTypeDef",
-    "ListLunaClientsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ModifyHapgResponseTypeDef",
-    "ModifyHsmResponseTypeDef",
-    "ModifyLunaClientResponseTypeDef",
-    "RemoveTagsFromResourceResponseTypeDef",
-    "ListHapgsRequestListHapgsPaginateTypeDef",
-    "ListHsmsRequestListHsmsPaginateTypeDef",
-    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddTagsToResourceResponseTypeDef = TypedDict(
+    "AddTagsToResourceResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateHapgRequestRequestTypeDef = TypedDict(
     "CreateHapgRequestRequestTypeDef",
     {
         "Label": str,
     },
 )
 
+CreateHapgResponseTypeDef = TypedDict(
+    "CreateHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateHsmRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHsmRequestRequestTypeDef",
     {
         "SubnetId": str,
         "SshKey": str,
         "IamRoleArn": str,
         "SubscriptionType": Literal["PRODUCTION"],
@@ -123,14 +128,22 @@
 
 class CreateHsmRequestRequestTypeDef(
     _RequiredCreateHsmRequestRequestTypeDef, _OptionalCreateHsmRequestRequestTypeDef
 ):
     pass
 
 
+CreateHsmResponseTypeDef = TypedDict(
+    "CreateHsmResponseTypeDef",
+    {
+        "HsmArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateLunaClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLunaClientRequestRequestTypeDef",
     {
         "Certificate": str,
     },
 )
 _OptionalCreateLunaClientRequestRequestTypeDef = TypedDict(
@@ -144,103 +157,250 @@
 
 class CreateLunaClientRequestRequestTypeDef(
     _RequiredCreateLunaClientRequestRequestTypeDef, _OptionalCreateLunaClientRequestRequestTypeDef
 ):
     pass
 
 
+CreateLunaClientResponseTypeDef = TypedDict(
+    "CreateLunaClientResponseTypeDef",
+    {
+        "ClientArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteHapgRequestRequestTypeDef = TypedDict(
     "DeleteHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 
+DeleteHapgResponseTypeDef = TypedDict(
+    "DeleteHapgResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteHsmRequestRequestTypeDef = TypedDict(
     "DeleteHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
     },
 )
 
+DeleteHsmResponseTypeDef = TypedDict(
+    "DeleteHsmResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteLunaClientRequestRequestTypeDef = TypedDict(
     "DeleteLunaClientRequestRequestTypeDef",
     {
         "ClientArn": str,
     },
 )
 
+DeleteLunaClientResponseTypeDef = TypedDict(
+    "DeleteLunaClientResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeHapgRequestRequestTypeDef = TypedDict(
     "DescribeHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 
+DescribeHapgResponseTypeDef = TypedDict(
+    "DescribeHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "HapgSerial": str,
+        "HsmsLastActionFailed": List[str],
+        "HsmsPendingDeletion": List[str],
+        "HsmsPendingRegistration": List[str],
+        "Label": str,
+        "LastModifiedTimestamp": str,
+        "PartitionSerialList": List[str],
+        "State": CloudHsmObjectStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeHsmRequestRequestTypeDef = TypedDict(
     "DescribeHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
         "HsmSerialNumber": str,
     },
     total=False,
 )
 
+DescribeHsmResponseTypeDef = TypedDict(
+    "DescribeHsmResponseTypeDef",
+    {
+        "HsmArn": str,
+        "Status": HsmStatusType,
+        "StatusDetails": str,
+        "AvailabilityZone": str,
+        "EniId": str,
+        "EniIp": str,
+        "SubscriptionType": Literal["PRODUCTION"],
+        "SubscriptionStartDate": str,
+        "SubscriptionEndDate": str,
+        "VpcId": str,
+        "SubnetId": str,
+        "IamRoleArn": str,
+        "SerialNumber": str,
+        "VendorName": str,
+        "HsmType": str,
+        "SoftwareVersion": str,
+        "SshPublicKey": str,
+        "SshKeyLastUpdated": str,
+        "ServerCertUri": str,
+        "ServerCertLastUpdated": str,
+        "Partitions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeLunaClientRequestRequestTypeDef = TypedDict(
     "DescribeLunaClientRequestRequestTypeDef",
     {
         "ClientArn": str,
         "CertificateFingerprint": str,
     },
     total=False,
 )
 
+DescribeLunaClientResponseTypeDef = TypedDict(
+    "DescribeLunaClientResponseTypeDef",
+    {
+        "ClientArn": str,
+        "Certificate": str,
+        "CertificateFingerprint": str,
+        "LastModifiedTimestamp": str,
+        "Label": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetConfigRequestRequestTypeDef = TypedDict(
     "GetConfigRequestRequestTypeDef",
     {
         "ClientArn": str,
         "ClientVersion": ClientVersionType,
         "HapgList": Sequence[str],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetConfigResponseTypeDef = TypedDict(
+    "GetConfigResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ConfigType": str,
+        "ConfigFile": str,
+        "ConfigCred": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAvailableZonesResponseTypeDef = TypedDict(
+    "ListAvailableZonesResponseTypeDef",
+    {
+        "AZList": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListHapgsRequestListHapgsPaginateTypeDef = TypedDict(
+    "ListHapgsRequestListHapgsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListHapgsRequestRequestTypeDef = TypedDict(
     "ListHapgsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+ListHapgsResponseTypeDef = TypedDict(
+    "ListHapgsResponseTypeDef",
+    {
+        "HapgList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListHsmsRequestListHsmsPaginateTypeDef = TypedDict(
+    "ListHsmsRequestListHsmsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListHsmsRequestRequestTypeDef = TypedDict(
     "ListHsmsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+ListHsmsResponseTypeDef = TypedDict(
+    "ListHsmsResponseTypeDef",
+    {
+        "HsmList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListLunaClientsRequestListLunaClientsPaginateTypeDef = TypedDict(
+    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLunaClientsRequestRequestTypeDef = TypedDict(
     "ListLunaClientsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+ListLunaClientsResponseTypeDef = TypedDict(
+    "ListLunaClientsResponseTypeDef",
+    {
+        "ClientList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -262,14 +422,22 @@
 
 class ModifyHapgRequestRequestTypeDef(
     _RequiredModifyHapgRequestRequestTypeDef, _OptionalModifyHapgRequestRequestTypeDef
 ):
     pass
 
 
+ModifyHapgResponseTypeDef = TypedDict(
+    "ModifyHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredModifyHsmRequestRequestTypeDef = TypedDict(
     "_RequiredModifyHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
     },
 )
 _OptionalModifyHsmRequestRequestTypeDef = TypedDict(
@@ -287,251 +455,83 @@
 
 class ModifyHsmRequestRequestTypeDef(
     _RequiredModifyHsmRequestRequestTypeDef, _OptionalModifyHsmRequestRequestTypeDef
 ):
     pass
 
 
-ModifyLunaClientRequestRequestTypeDef = TypedDict(
-    "ModifyLunaClientRequestRequestTypeDef",
-    {
-        "ClientArn": str,
-        "Certificate": str,
-    },
-)
-
-RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
-    "RemoveTagsFromResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagKeyList": Sequence[str],
-    },
-)
-
-AddTagsToResourceRequestRequestTypeDef = TypedDict(
-    "AddTagsToResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagList": Sequence[TagTypeDef],
-    },
-)
-
-AddTagsToResourceResponseTypeDef = TypedDict(
-    "AddTagsToResourceResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateHapgResponseTypeDef = TypedDict(
-    "CreateHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateHsmResponseTypeDef = TypedDict(
-    "CreateHsmResponseTypeDef",
-    {
-        "HsmArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLunaClientResponseTypeDef = TypedDict(
-    "CreateLunaClientResponseTypeDef",
-    {
-        "ClientArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteHapgResponseTypeDef = TypedDict(
-    "DeleteHapgResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteHsmResponseTypeDef = TypedDict(
-    "DeleteHsmResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteLunaClientResponseTypeDef = TypedDict(
-    "DeleteLunaClientResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeHapgResponseTypeDef = TypedDict(
-    "DescribeHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "HapgSerial": str,
-        "HsmsLastActionFailed": List[str],
-        "HsmsPendingDeletion": List[str],
-        "HsmsPendingRegistration": List[str],
-        "Label": str,
-        "LastModifiedTimestamp": str,
-        "PartitionSerialList": List[str],
-        "State": CloudHsmObjectStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeHsmResponseTypeDef = TypedDict(
-    "DescribeHsmResponseTypeDef",
+ModifyHsmResponseTypeDef = TypedDict(
+    "ModifyHsmResponseTypeDef",
     {
         "HsmArn": str,
-        "Status": HsmStatusType,
-        "StatusDetails": str,
-        "AvailabilityZone": str,
-        "EniId": str,
-        "EniIp": str,
-        "SubscriptionType": Literal["PRODUCTION"],
-        "SubscriptionStartDate": str,
-        "SubscriptionEndDate": str,
-        "VpcId": str,
-        "SubnetId": str,
-        "IamRoleArn": str,
-        "SerialNumber": str,
-        "VendorName": str,
-        "HsmType": str,
-        "SoftwareVersion": str,
-        "SshPublicKey": str,
-        "SshKeyLastUpdated": str,
-        "ServerCertUri": str,
-        "ServerCertLastUpdated": str,
-        "Partitions": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLunaClientResponseTypeDef = TypedDict(
-    "DescribeLunaClientResponseTypeDef",
+ModifyLunaClientRequestRequestTypeDef = TypedDict(
+    "ModifyLunaClientRequestRequestTypeDef",
     {
         "ClientArn": str,
         "Certificate": str,
-        "CertificateFingerprint": str,
-        "LastModifiedTimestamp": str,
-        "Label": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetConfigResponseTypeDef = TypedDict(
-    "GetConfigResponseTypeDef",
-    {
-        "ConfigType": str,
-        "ConfigFile": str,
-        "ConfigCred": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAvailableZonesResponseTypeDef = TypedDict(
-    "ListAvailableZonesResponseTypeDef",
-    {
-        "AZList": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListHapgsResponseTypeDef = TypedDict(
-    "ListHapgsResponseTypeDef",
-    {
-        "HapgList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListHsmsResponseTypeDef = TypedDict(
-    "ListHsmsResponseTypeDef",
-    {
-        "HsmList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListLunaClientsResponseTypeDef = TypedDict(
-    "ListLunaClientsResponseTypeDef",
-    {
-        "ClientList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyHapgResponseTypeDef = TypedDict(
-    "ModifyHapgResponseTypeDef",
+ModifyLunaClientResponseTypeDef = TypedDict(
+    "ModifyLunaClientResponseTypeDef",
     {
-        "HapgArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ClientArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyHsmResponseTypeDef = TypedDict(
-    "ModifyHsmResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "HsmArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-ModifyLunaClientResponseTypeDef = TypedDict(
-    "ModifyLunaClientResponseTypeDef",
+RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
+    "RemoveTagsFromResourceRequestRequestTypeDef",
     {
-        "ClientArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "TagKeyList": Sequence[str],
     },
 )
 
 RemoveTagsFromResourceResponseTypeDef = TypedDict(
     "RemoveTagsFromResourceResponseTypeDef",
     {
         "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListHapgsRequestListHapgsPaginateTypeDef = TypedDict(
-    "ListHapgsRequestListHapgsPaginateTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-ListHsmsRequestListHsmsPaginateTypeDef = TypedDict(
-    "ListHsmsRequestListHsmsPaginateTypeDef",
+AddTagsToResourceRequestRequestTypeDef = TypedDict(
+    "AddTagsToResourceRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResourceArn": str,
+        "TagList": Sequence[TagTypeDef],
     },
-    total=False,
 )
 
-ListLunaClientsRequestListLunaClientsPaginateTypeDef = TypedDict(
-    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
```

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm/type_defs.pyi` & `mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -23,86 +23,91 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddTagsToResourceResponseTypeDef",
     "CreateHapgRequestRequestTypeDef",
+    "CreateHapgResponseTypeDef",
     "CreateHsmRequestRequestTypeDef",
+    "CreateHsmResponseTypeDef",
     "CreateLunaClientRequestRequestTypeDef",
+    "CreateLunaClientResponseTypeDef",
     "DeleteHapgRequestRequestTypeDef",
+    "DeleteHapgResponseTypeDef",
     "DeleteHsmRequestRequestTypeDef",
+    "DeleteHsmResponseTypeDef",
     "DeleteLunaClientRequestRequestTypeDef",
+    "DeleteLunaClientResponseTypeDef",
     "DescribeHapgRequestRequestTypeDef",
+    "DescribeHapgResponseTypeDef",
     "DescribeHsmRequestRequestTypeDef",
+    "DescribeHsmResponseTypeDef",
     "DescribeLunaClientRequestRequestTypeDef",
+    "DescribeLunaClientResponseTypeDef",
     "GetConfigRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetConfigResponseTypeDef",
+    "ListAvailableZonesResponseTypeDef",
+    "ListHapgsRequestListHapgsPaginateTypeDef",
     "ListHapgsRequestRequestTypeDef",
+    "ListHapgsResponseTypeDef",
+    "ListHsmsRequestListHsmsPaginateTypeDef",
     "ListHsmsRequestRequestTypeDef",
+    "ListHsmsResponseTypeDef",
+    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
     "ListLunaClientsRequestRequestTypeDef",
+    "ListLunaClientsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModifyHapgRequestRequestTypeDef",
+    "ModifyHapgResponseTypeDef",
     "ModifyHsmRequestRequestTypeDef",
+    "ModifyHsmResponseTypeDef",
     "ModifyLunaClientRequestRequestTypeDef",
+    "ModifyLunaClientResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
+    "RemoveTagsFromResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
-    "AddTagsToResourceResponseTypeDef",
-    "CreateHapgResponseTypeDef",
-    "CreateHsmResponseTypeDef",
-    "CreateLunaClientResponseTypeDef",
-    "DeleteHapgResponseTypeDef",
-    "DeleteHsmResponseTypeDef",
-    "DeleteLunaClientResponseTypeDef",
-    "DescribeHapgResponseTypeDef",
-    "DescribeHsmResponseTypeDef",
-    "DescribeLunaClientResponseTypeDef",
-    "GetConfigResponseTypeDef",
-    "ListAvailableZonesResponseTypeDef",
-    "ListHapgsResponseTypeDef",
-    "ListHsmsResponseTypeDef",
-    "ListLunaClientsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ModifyHapgResponseTypeDef",
-    "ModifyHsmResponseTypeDef",
-    "ModifyLunaClientResponseTypeDef",
-    "RemoveTagsFromResourceResponseTypeDef",
-    "ListHapgsRequestListHapgsPaginateTypeDef",
-    "ListHsmsRequestListHsmsPaginateTypeDef",
-    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddTagsToResourceResponseTypeDef = TypedDict(
+    "AddTagsToResourceResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateHapgRequestRequestTypeDef = TypedDict(
     "CreateHapgRequestRequestTypeDef",
     {
         "Label": str,
     },
 )
 
+CreateHapgResponseTypeDef = TypedDict(
+    "CreateHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateHsmRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHsmRequestRequestTypeDef",
     {
         "SubnetId": str,
         "SshKey": str,
         "IamRoleArn": str,
         "SubscriptionType": Literal["PRODUCTION"],
@@ -120,14 +125,22 @@
 )
 
 class CreateHsmRequestRequestTypeDef(
     _RequiredCreateHsmRequestRequestTypeDef, _OptionalCreateHsmRequestRequestTypeDef
 ):
     pass
 
+CreateHsmResponseTypeDef = TypedDict(
+    "CreateHsmResponseTypeDef",
+    {
+        "HsmArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateLunaClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLunaClientRequestRequestTypeDef",
     {
         "Certificate": str,
     },
 )
 _OptionalCreateLunaClientRequestRequestTypeDef = TypedDict(
@@ -139,103 +152,250 @@
 )
 
 class CreateLunaClientRequestRequestTypeDef(
     _RequiredCreateLunaClientRequestRequestTypeDef, _OptionalCreateLunaClientRequestRequestTypeDef
 ):
     pass
 
+CreateLunaClientResponseTypeDef = TypedDict(
+    "CreateLunaClientResponseTypeDef",
+    {
+        "ClientArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteHapgRequestRequestTypeDef = TypedDict(
     "DeleteHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 
+DeleteHapgResponseTypeDef = TypedDict(
+    "DeleteHapgResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteHsmRequestRequestTypeDef = TypedDict(
     "DeleteHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
     },
 )
 
+DeleteHsmResponseTypeDef = TypedDict(
+    "DeleteHsmResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteLunaClientRequestRequestTypeDef = TypedDict(
     "DeleteLunaClientRequestRequestTypeDef",
     {
         "ClientArn": str,
     },
 )
 
+DeleteLunaClientResponseTypeDef = TypedDict(
+    "DeleteLunaClientResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeHapgRequestRequestTypeDef = TypedDict(
     "DescribeHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 
+DescribeHapgResponseTypeDef = TypedDict(
+    "DescribeHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "HapgSerial": str,
+        "HsmsLastActionFailed": List[str],
+        "HsmsPendingDeletion": List[str],
+        "HsmsPendingRegistration": List[str],
+        "Label": str,
+        "LastModifiedTimestamp": str,
+        "PartitionSerialList": List[str],
+        "State": CloudHsmObjectStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeHsmRequestRequestTypeDef = TypedDict(
     "DescribeHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
         "HsmSerialNumber": str,
     },
     total=False,
 )
 
+DescribeHsmResponseTypeDef = TypedDict(
+    "DescribeHsmResponseTypeDef",
+    {
+        "HsmArn": str,
+        "Status": HsmStatusType,
+        "StatusDetails": str,
+        "AvailabilityZone": str,
+        "EniId": str,
+        "EniIp": str,
+        "SubscriptionType": Literal["PRODUCTION"],
+        "SubscriptionStartDate": str,
+        "SubscriptionEndDate": str,
+        "VpcId": str,
+        "SubnetId": str,
+        "IamRoleArn": str,
+        "SerialNumber": str,
+        "VendorName": str,
+        "HsmType": str,
+        "SoftwareVersion": str,
+        "SshPublicKey": str,
+        "SshKeyLastUpdated": str,
+        "ServerCertUri": str,
+        "ServerCertLastUpdated": str,
+        "Partitions": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeLunaClientRequestRequestTypeDef = TypedDict(
     "DescribeLunaClientRequestRequestTypeDef",
     {
         "ClientArn": str,
         "CertificateFingerprint": str,
     },
     total=False,
 )
 
+DescribeLunaClientResponseTypeDef = TypedDict(
+    "DescribeLunaClientResponseTypeDef",
+    {
+        "ClientArn": str,
+        "Certificate": str,
+        "CertificateFingerprint": str,
+        "LastModifiedTimestamp": str,
+        "Label": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetConfigRequestRequestTypeDef = TypedDict(
     "GetConfigRequestRequestTypeDef",
     {
         "ClientArn": str,
         "ClientVersion": ClientVersionType,
         "HapgList": Sequence[str],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetConfigResponseTypeDef = TypedDict(
+    "GetConfigResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ConfigType": str,
+        "ConfigFile": str,
+        "ConfigCred": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAvailableZonesResponseTypeDef = TypedDict(
+    "ListAvailableZonesResponseTypeDef",
+    {
+        "AZList": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListHapgsRequestListHapgsPaginateTypeDef = TypedDict(
+    "ListHapgsRequestListHapgsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListHapgsRequestRequestTypeDef = TypedDict(
     "ListHapgsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+ListHapgsResponseTypeDef = TypedDict(
+    "ListHapgsResponseTypeDef",
+    {
+        "HapgList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListHsmsRequestListHsmsPaginateTypeDef = TypedDict(
+    "ListHsmsRequestListHsmsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListHsmsRequestRequestTypeDef = TypedDict(
     "ListHsmsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+ListHsmsResponseTypeDef = TypedDict(
+    "ListHsmsResponseTypeDef",
+    {
+        "HsmList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListLunaClientsRequestListLunaClientsPaginateTypeDef = TypedDict(
+    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLunaClientsRequestRequestTypeDef = TypedDict(
     "ListLunaClientsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+ListLunaClientsResponseTypeDef = TypedDict(
+    "ListLunaClientsResponseTypeDef",
+    {
+        "ClientList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -255,14 +415,22 @@
 )
 
 class ModifyHapgRequestRequestTypeDef(
     _RequiredModifyHapgRequestRequestTypeDef, _OptionalModifyHapgRequestRequestTypeDef
 ):
     pass
 
+ModifyHapgResponseTypeDef = TypedDict(
+    "ModifyHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredModifyHsmRequestRequestTypeDef = TypedDict(
     "_RequiredModifyHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
     },
 )
 _OptionalModifyHsmRequestRequestTypeDef = TypedDict(
@@ -278,251 +446,83 @@
 )
 
 class ModifyHsmRequestRequestTypeDef(
     _RequiredModifyHsmRequestRequestTypeDef, _OptionalModifyHsmRequestRequestTypeDef
 ):
     pass
 
-ModifyLunaClientRequestRequestTypeDef = TypedDict(
-    "ModifyLunaClientRequestRequestTypeDef",
-    {
-        "ClientArn": str,
-        "Certificate": str,
-    },
-)
-
-RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
-    "RemoveTagsFromResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagKeyList": Sequence[str],
-    },
-)
-
-AddTagsToResourceRequestRequestTypeDef = TypedDict(
-    "AddTagsToResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagList": Sequence[TagTypeDef],
-    },
-)
-
-AddTagsToResourceResponseTypeDef = TypedDict(
-    "AddTagsToResourceResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateHapgResponseTypeDef = TypedDict(
-    "CreateHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateHsmResponseTypeDef = TypedDict(
-    "CreateHsmResponseTypeDef",
-    {
-        "HsmArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateLunaClientResponseTypeDef = TypedDict(
-    "CreateLunaClientResponseTypeDef",
-    {
-        "ClientArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteHapgResponseTypeDef = TypedDict(
-    "DeleteHapgResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteHsmResponseTypeDef = TypedDict(
-    "DeleteHsmResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteLunaClientResponseTypeDef = TypedDict(
-    "DeleteLunaClientResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeHapgResponseTypeDef = TypedDict(
-    "DescribeHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "HapgSerial": str,
-        "HsmsLastActionFailed": List[str],
-        "HsmsPendingDeletion": List[str],
-        "HsmsPendingRegistration": List[str],
-        "Label": str,
-        "LastModifiedTimestamp": str,
-        "PartitionSerialList": List[str],
-        "State": CloudHsmObjectStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeHsmResponseTypeDef = TypedDict(
-    "DescribeHsmResponseTypeDef",
+ModifyHsmResponseTypeDef = TypedDict(
+    "ModifyHsmResponseTypeDef",
     {
         "HsmArn": str,
-        "Status": HsmStatusType,
-        "StatusDetails": str,
-        "AvailabilityZone": str,
-        "EniId": str,
-        "EniIp": str,
-        "SubscriptionType": Literal["PRODUCTION"],
-        "SubscriptionStartDate": str,
-        "SubscriptionEndDate": str,
-        "VpcId": str,
-        "SubnetId": str,
-        "IamRoleArn": str,
-        "SerialNumber": str,
-        "VendorName": str,
-        "HsmType": str,
-        "SoftwareVersion": str,
-        "SshPublicKey": str,
-        "SshKeyLastUpdated": str,
-        "ServerCertUri": str,
-        "ServerCertLastUpdated": str,
-        "Partitions": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLunaClientResponseTypeDef = TypedDict(
-    "DescribeLunaClientResponseTypeDef",
+ModifyLunaClientRequestRequestTypeDef = TypedDict(
+    "ModifyLunaClientRequestRequestTypeDef",
     {
         "ClientArn": str,
         "Certificate": str,
-        "CertificateFingerprint": str,
-        "LastModifiedTimestamp": str,
-        "Label": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetConfigResponseTypeDef = TypedDict(
-    "GetConfigResponseTypeDef",
-    {
-        "ConfigType": str,
-        "ConfigFile": str,
-        "ConfigCred": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAvailableZonesResponseTypeDef = TypedDict(
-    "ListAvailableZonesResponseTypeDef",
-    {
-        "AZList": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListHapgsResponseTypeDef = TypedDict(
-    "ListHapgsResponseTypeDef",
-    {
-        "HapgList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListHsmsResponseTypeDef = TypedDict(
-    "ListHsmsResponseTypeDef",
-    {
-        "HsmList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListLunaClientsResponseTypeDef = TypedDict(
-    "ListLunaClientsResponseTypeDef",
-    {
-        "ClientList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyHapgResponseTypeDef = TypedDict(
-    "ModifyHapgResponseTypeDef",
+ModifyLunaClientResponseTypeDef = TypedDict(
+    "ModifyLunaClientResponseTypeDef",
     {
-        "HapgArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ClientArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ModifyHsmResponseTypeDef = TypedDict(
-    "ModifyHsmResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "HsmArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-ModifyLunaClientResponseTypeDef = TypedDict(
-    "ModifyLunaClientResponseTypeDef",
+RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
+    "RemoveTagsFromResourceRequestRequestTypeDef",
     {
-        "ClientArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "TagKeyList": Sequence[str],
     },
 )
 
 RemoveTagsFromResourceResponseTypeDef = TypedDict(
     "RemoveTagsFromResourceResponseTypeDef",
     {
         "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListHapgsRequestListHapgsPaginateTypeDef = TypedDict(
-    "ListHapgsRequestListHapgsPaginateTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-ListHsmsRequestListHsmsPaginateTypeDef = TypedDict(
-    "ListHsmsRequestListHsmsPaginateTypeDef",
+AddTagsToResourceRequestRequestTypeDef = TypedDict(
+    "AddTagsToResourceRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResourceArn": str,
+        "TagList": Sequence[TagTypeDef],
     },
-    total=False,
 )
 
-ListLunaClientsRequestListLunaClientsPaginateTypeDef = TypedDict(
-    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
```

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm.egg-info/PKG-INFO` & `mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudhsm
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CloudHSM 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudHSM 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/
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
 
 <a id="mypy-boto3-cloudhsm"></a>
 
 # mypy-boto3-cloudhsm
 
 [![PyPI - mypy-boto3-cloudhsm](https://img.shields.io/pypi/v/mypy-boto3-cloudhsm.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudhsm.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudhsm?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudHSM 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
+[boto3.CloudHSM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
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
 [mypy-boto3-cloudhsm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,100 +331,100 @@
 
 `mypy_boto3_cloudhsm.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudhsm.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    AddTagsToResourceResponseTypeDef,
     CreateHapgRequestRequestTypeDef,
+    CreateHapgResponseTypeDef,
     CreateHsmRequestRequestTypeDef,
+    CreateHsmResponseTypeDef,
     CreateLunaClientRequestRequestTypeDef,
+    CreateLunaClientResponseTypeDef,
     DeleteHapgRequestRequestTypeDef,
+    DeleteHapgResponseTypeDef,
     DeleteHsmRequestRequestTypeDef,
+    DeleteHsmResponseTypeDef,
     DeleteLunaClientRequestRequestTypeDef,
+    DeleteLunaClientResponseTypeDef,
     DescribeHapgRequestRequestTypeDef,
+    DescribeHapgResponseTypeDef,
     DescribeHsmRequestRequestTypeDef,
+    DescribeHsmResponseTypeDef,
     DescribeLunaClientRequestRequestTypeDef,
+    DescribeLunaClientResponseTypeDef,
     GetConfigRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetConfigResponseTypeDef,
+    ListAvailableZonesResponseTypeDef,
+    ListHapgsRequestListHapgsPaginateTypeDef,
     ListHapgsRequestRequestTypeDef,
+    ListHapgsResponseTypeDef,
+    ListHsmsRequestListHsmsPaginateTypeDef,
     ListHsmsRequestRequestTypeDef,
+    ListHsmsResponseTypeDef,
+    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
     ListLunaClientsRequestRequestTypeDef,
+    ListLunaClientsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyHapgRequestRequestTypeDef,
+    ModifyHapgResponseTypeDef,
     ModifyHsmRequestRequestTypeDef,
+    ModifyHsmResponseTypeDef,
     ModifyLunaClientRequestRequestTypeDef,
+    ModifyLunaClientResponseTypeDef,
+    PaginatorConfigTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
+    RemoveTagsFromResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
-    AddTagsToResourceResponseTypeDef,
-    CreateHapgResponseTypeDef,
-    CreateHsmResponseTypeDef,
-    CreateLunaClientResponseTypeDef,
-    DeleteHapgResponseTypeDef,
-    DeleteHsmResponseTypeDef,
-    DeleteLunaClientResponseTypeDef,
-    DescribeHapgResponseTypeDef,
-    DescribeHsmResponseTypeDef,
-    DescribeLunaClientResponseTypeDef,
-    GetConfigResponseTypeDef,
-    ListAvailableZonesResponseTypeDef,
-    ListHapgsResponseTypeDef,
-    ListHsmsResponseTypeDef,
-    ListLunaClientsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ModifyHapgResponseTypeDef,
-    ModifyHsmResponseTypeDef,
-    ModifyLunaClientResponseTypeDef,
-    RemoveTagsFromResourceResponseTypeDef,
-    ListHapgsRequestListHapgsPaginateTypeDef,
-    ListHsmsRequestListHsmsPaginateTypeDef,
-    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
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

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/mypy_boto3_cloudhsm.egg-info/SOURCES.txt` & `mypy-boto3-cloudhsm-1.27.0/mypy_boto3_cloudhsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.26.0.post1/setup.py` & `mypy-boto3-cloudhsm-1.27.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-cloudhsm.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudhsm",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_cloudhsm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudHSM 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.CloudHSM 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 cloudhsm type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_cloudhsm": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_cloudhsm": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/",
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


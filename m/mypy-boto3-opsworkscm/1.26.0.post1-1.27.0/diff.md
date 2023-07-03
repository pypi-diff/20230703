# Comparing `tmp/mypy-boto3-opsworkscm-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-opsworkscm-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opsworkscm-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:48 2022, max compression
+gzip compressed data, was "mypy-boto3-opsworkscm-1.27.0.tar", last modified: Mon Jul  3 19:51:12 2023, max compression
```

## Comparing `mypy-boto3-opsworkscm-1.26.0.post1.tar` & `mypy-boto3-opsworkscm-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:48.796839 mypy-boto3-opsworkscm-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15769 2022-11-01 21:43:48.796839 mypy-boto3-opsworkscm-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14316 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:48.796839 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17661 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    17630 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8338 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8336 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5187 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5181 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    18758 2022-11-01 21:38:53.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    18731 2022-11-01 21:38:53.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:48.796839 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15769 2022-11-01 21:43:48.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-11-01 21:43:48.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:48.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:48.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:48.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-01 21:43:48.000000 mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:48.796839 mypy-boto3-opsworkscm-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-11-01 21:38:51.000000 mypy-boto3-opsworkscm-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:12.731762 mypy-boto3-opsworkscm-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:08.000000 mypy-boto3-opsworkscm-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-03 19:51:12.727762 mypy-boto3-opsworkscm-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-03 19:43:08.000000 mypy-boto3-opsworkscm-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:12.715762 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-03 19:43:08.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-03 19:43:08.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:43:08.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-07-03 19:43:09.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-07-03 19:43:08.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-07-03 19:43:09.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-03 19:43:09.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-03 19:43:09.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-07-03 19:43:09.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:08.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18796 2023-07-03 19:43:09.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-07-03 19:43:09.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:08.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-03 19:43:09.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-03 19:43:09.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:12.727762 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-03 19:51:12.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 19:51:12.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:12.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:12.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:12.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:51:12.000000 mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:12.731762 mypy-boto3-opsworkscm-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:43:08.000000 mypy-boto3-opsworkscm-1.27.0/setup.py
```

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/LICENSE` & `mypy-boto3-opsworkscm-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/PKG-INFO` & `mypy-boto3-opsworkscm-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworkscm
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.OpsWorksCM 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.OpsWorksCM 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/
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
 
 <a id="mypy-boto3-opsworkscm"></a>
 
 # mypy-boto3-opsworkscm
 
 [![PyPI - mypy-boto3-opsworkscm](https://img.shields.io/pypi/v/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opsworkscm?color=blue)](https://pypistats.org/packages/mypy-boto3-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorksCM 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[boto3.OpsWorksCM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [mypy-boto3-opsworkscm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -360,51 +361,51 @@
 `mypy_boto3_opsworkscm.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opsworkscm.type_defs import (
     AccountAttributeTypeDef,
     EngineAttributeTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateNodeResponseTypeDef,
     BackupTypeDef,
     TagTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteServerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeBackupsRequestRequestTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     ServerEventTypeDef,
     WaiterConfigTypeDef,
     DescribeNodeAssociationStatusRequestRequestTypeDef,
+    DescribeServersRequestDescribeServersPaginateTypeDef,
     DescribeServersRequestRequestTypeDef,
+    DisassociateNodeResponseTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RestoreServerRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateServerEngineAttributesRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
     AssociateNodeRequestRequestTypeDef,
+    DescribeNodeAssociationStatusResponseTypeDef,
     DisassociateNodeRequestRequestTypeDef,
     ExportServerEngineAttributeRequestRequestTypeDef,
+    ExportServerEngineAttributeResponseTypeDef,
     ServerTypeDef,
     StartMaintenanceRequestRequestTypeDef,
-    AssociateNodeResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
-    DescribeNodeAssociationStatusResponseTypeDef,
-    DisassociateNodeResponseTypeDef,
-    ExportServerEngineAttributeResponseTypeDef,
     CreateBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateServerRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
-    DescribeServersRequestDescribeServersPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
     CreateServerResponseTypeDef,
     DescribeServersResponseTypeDef,
     RestoreServerResponseTypeDef,
     StartMaintenanceResponseTypeDef,
     UpdateServerEngineAttributesResponseTypeDef,
@@ -419,42 +420,42 @@
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

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/README.md` & `mypy-boto3-opsworkscm-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-opsworkscm"></a>
 
 # mypy-boto3-opsworkscm
 
 [![PyPI - mypy-boto3-opsworkscm](https://img.shields.io/pypi/v/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opsworkscm?color=blue)](https://pypistats.org/packages/mypy-boto3-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorksCM 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[boto3.OpsWorksCM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [mypy-boto3-opsworkscm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,51 +329,51 @@
 `mypy_boto3_opsworkscm.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opsworkscm.type_defs import (
     AccountAttributeTypeDef,
     EngineAttributeTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateNodeResponseTypeDef,
     BackupTypeDef,
     TagTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteServerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeBackupsRequestRequestTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     ServerEventTypeDef,
     WaiterConfigTypeDef,
     DescribeNodeAssociationStatusRequestRequestTypeDef,
+    DescribeServersRequestDescribeServersPaginateTypeDef,
     DescribeServersRequestRequestTypeDef,
+    DisassociateNodeResponseTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RestoreServerRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateServerEngineAttributesRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
     AssociateNodeRequestRequestTypeDef,
+    DescribeNodeAssociationStatusResponseTypeDef,
     DisassociateNodeRequestRequestTypeDef,
     ExportServerEngineAttributeRequestRequestTypeDef,
+    ExportServerEngineAttributeResponseTypeDef,
     ServerTypeDef,
     StartMaintenanceRequestRequestTypeDef,
-    AssociateNodeResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
-    DescribeNodeAssociationStatusResponseTypeDef,
-    DisassociateNodeResponseTypeDef,
-    ExportServerEngineAttributeResponseTypeDef,
     CreateBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateServerRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
-    DescribeServersRequestDescribeServersPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
     CreateServerResponseTypeDef,
     DescribeServersResponseTypeDef,
     RestoreServerResponseTypeDef,
     StartMaintenanceResponseTypeDef,
     UpdateServerEngineAttributesResponseTypeDef,
@@ -388,42 +388,42 @@
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

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/__init__.py` & `mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/__init__.pyi` & `mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/client.py` & `mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,16 +282,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/client/#list_tags_for_resource)
         """
 
     def restore_server(
         self, *, BackupId: str, ServerName: str, InstanceType: str = ..., KeyPair: str = ...
     ) -> RestoreServerResponseTypeDef:
         """
-        Restores a backup to a server that is in a `CONNECTION_LOST` , `HEALTHY` ,
-        `RUNNING` , `UNHEALTHY` , or `TERMINATED` state.
+        Restores a backup to a server that is in a `CONNECTION_LOST`, `HEALTHY`,
+        `RUNNING`, `UNHEALTHY`, or `TERMINATED` state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.restore_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/client/#restore_server)
         """
 
     def start_maintenance(
         self, *, ServerName: str, EngineAttributes: Sequence[EngineAttributeTypeDef] = ...
```

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/client.pyi` & `mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -261,16 +261,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/client/#list_tags_for_resource)
         """
     def restore_server(
         self, *, BackupId: str, ServerName: str, InstanceType: str = ..., KeyPair: str = ...
     ) -> RestoreServerResponseTypeDef:
         """
-        Restores a backup to a server that is in a `CONNECTION_LOST` , `HEALTHY` ,
-        `RUNNING` , `UNHEALTHY` , or `TERMINATED` state.
+        Restores a backup to a server that is in a `CONNECTION_LOST`, `HEALTHY`,
+        `RUNNING`, `UNHEALTHY`, or `TERMINATED` state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client.restore_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/client/#restore_server)
         """
     def start_maintenance(
         self, *, ServerName: str, EngineAttributes: Sequence[EngineAttributeTypeDef] = ...
     ) -> StartMaintenanceResponseTypeDef:
```

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/literals.py` & `mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "BackupStatusType",
     "BackupTypeType",
     "DescribeBackupsPaginatorName",
     "DescribeEventsPaginatorName",
     "DescribeServersPaginatorName",
     "ListTagsForResourcePaginatorName",
@@ -34,15 +33,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 BackupStatusType = Literal["DELETING", "FAILED", "IN_PROGRESS", "OK"]
 BackupTypeType = Literal["AUTOMATED", "MANUAL"]
 DescribeBackupsPaginatorName = Literal["describe_backups"]
 DescribeEventsPaginatorName = Literal["describe_events"]
 DescribeServersPaginatorName = Literal["describe_servers"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 MaintenanceStatusType = Literal["FAILED", "SUCCESS"]
@@ -75,23 +73,25 @@
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
@@ -101,30 +101,35 @@
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
@@ -150,14 +155,15 @@
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
@@ -202,51 +208,57 @@
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
@@ -259,14 +271,15 @@
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
@@ -278,28 +291,35 @@
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
@@ -308,14 +328,15 @@
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
@@ -326,55 +347,64 @@
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

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/literals.pyi` & `mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "BackupStatusType",
     "BackupTypeType",
     "DescribeBackupsPaginatorName",
     "DescribeEventsPaginatorName",
     "DescribeServersPaginatorName",
     "ListTagsForResourcePaginatorName",
@@ -33,14 +34,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 BackupStatusType = Literal["DELETING", "FAILED", "IN_PROGRESS", "OK"]
 BackupTypeType = Literal["AUTOMATED", "MANUAL"]
 DescribeBackupsPaginatorName = Literal["describe_backups"]
 DescribeEventsPaginatorName = Literal["describe_events"]
 DescribeServersPaginatorName = Literal["describe_servers"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 MaintenanceStatusType = Literal["FAILED", "SUCCESS"]
@@ -73,23 +75,25 @@
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
@@ -99,30 +103,35 @@
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
@@ -148,14 +157,15 @@
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
@@ -200,51 +210,57 @@
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
@@ -257,14 +273,15 @@
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
@@ -276,28 +293,35 @@
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
@@ -306,14 +330,15 @@
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
@@ -324,55 +349,64 @@
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

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/paginator.py` & `mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,58 +62,58 @@
     """
 
     def paginate(
         self,
         *,
         BackupId: str = ...,
         ServerName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describebackupspaginator)
         """
 
 
 class DescribeEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeeventspaginator)
     """
 
     def paginate(
-        self, *, ServerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ServerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeeventspaginator)
         """
 
 
 class DescribeServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeserverspaginator)
     """
 
     def paginate(
-        self, *, ServerName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ServerName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeserverspaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/paginator.pyi` & `mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -59,55 +59,55 @@
     """
 
     def paginate(
         self,
         *,
         BackupId: str = ...,
         ServerName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describebackupspaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeeventspaginator)
     """
 
     def paginate(
-        self, *, ServerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ServerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeeventspaginator)
         """
 
 class DescribeServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeserverspaginator)
     """
 
     def paginate(
-        self, *, ServerName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ServerName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#describeserverspaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/type_defs.py` & `mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -24,55 +24,54 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountAttributeTypeDef",
     "EngineAttributeTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateNodeResponseTypeDef",
     "BackupTypeDef",
     "TagTypeDef",
     "DeleteBackupRequestRequestTypeDef",
     "DeleteServerRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "ServerEventTypeDef",
     "WaiterConfigTypeDef",
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
+    "DescribeServersRequestDescribeServersPaginateTypeDef",
     "DescribeServersRequestRequestTypeDef",
+    "DisassociateNodeResponseTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreServerRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateServerEngineAttributesRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
+    "DescribeAccountAttributesResponseTypeDef",
     "AssociateNodeRequestRequestTypeDef",
+    "DescribeNodeAssociationStatusResponseTypeDef",
     "DisassociateNodeRequestRequestTypeDef",
     "ExportServerEngineAttributeRequestRequestTypeDef",
+    "ExportServerEngineAttributeResponseTypeDef",
     "ServerTypeDef",
     "StartMaintenanceRequestRequestTypeDef",
-    "AssociateNodeResponseTypeDef",
-    "DescribeAccountAttributesResponseTypeDef",
-    "DescribeNodeAssociationStatusResponseTypeDef",
-    "DisassociateNodeResponseTypeDef",
-    "ExportServerEngineAttributeResponseTypeDef",
     "CreateBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
     "CreateBackupRequestRequestTypeDef",
     "CreateServerRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    "DescribeServersRequestDescribeServersPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
     "CreateServerResponseTypeDef",
     "DescribeServersResponseTypeDef",
     "RestoreServerResponseTypeDef",
     "StartMaintenanceResponseTypeDef",
     "UpdateServerEngineAttributesResponseTypeDef",
@@ -94,22 +93,19 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateNodeResponseTypeDef = TypedDict(
+    "AssociateNodeResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "NodeAssociationStatusToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BackupTypeDef = TypedDict(
     "BackupTypeDef",
     {
         "BackupArn": str,
@@ -158,20 +154,20 @@
 DeleteServerRequestRequestTypeDef = TypedDict(
     "DeleteServerRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "BackupId": str,
+        "ServerName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
@@ -179,14 +175,34 @@
         "ServerName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "ServerName": str,
+    },
+)
+_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeEventsRequestDescribeEventsPaginateTypeDef(
+    _RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef,
+    _OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeEventsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEventsRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 _OptionalDescribeEventsRequestRequestTypeDef = TypedDict(
@@ -194,21 +210,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeEventsRequestRequestTypeDef(
     _RequiredDescribeEventsRequestRequestTypeDef, _OptionalDescribeEventsRequestRequestTypeDef
 ):
     pass
 
-
 ServerEventTypeDef = TypedDict(
     "ServerEventTypeDef",
     {
         "CreatedAt": datetime,
         "ServerName": str,
         "Message": str,
         "LogUrl": str,
@@ -229,24 +243,61 @@
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
     {
         "NodeAssociationStatusToken": str,
         "ServerName": str,
     },
 )
 
+DescribeServersRequestDescribeServersPaginateTypeDef = TypedDict(
+    "DescribeServersRequestDescribeServersPaginateTypeDef",
+    {
+        "ServerName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeServersRequestRequestTypeDef = TypedDict(
     "DescribeServersRequestRequestTypeDef",
     {
         "ServerName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+DisassociateNodeResponseTypeDef = TypedDict(
+    "DisassociateNodeResponseTypeDef",
+    {
+        "NodeAssociationStatusToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -254,21 +305,40 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
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
 
 _RequiredRestoreServerRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreServerRequestRequestTypeDef",
     {
         "BackupId": str,
         "ServerName": str,
     },
@@ -278,21 +348,19 @@
     {
         "InstanceType": str,
         "KeyPair": str,
     },
     total=False,
 )
 
-
 class RestoreServerRequestRequestTypeDef(
     _RequiredRestoreServerRequestRequestTypeDef, _OptionalRestoreServerRequestRequestTypeDef
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -308,22 +376,20 @@
     "_OptionalUpdateServerEngineAttributesRequestRequestTypeDef",
     {
         "AttributeValue": str,
     },
     total=False,
 )
 
-
 class UpdateServerEngineAttributesRequestRequestTypeDef(
     _RequiredUpdateServerEngineAttributesRequestRequestTypeDef,
     _OptionalUpdateServerEngineAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateServerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServerRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 _OptionalUpdateServerRequestRequestTypeDef = TypedDict(
@@ -333,30 +399,45 @@
         "BackupRetentionCount": int,
         "PreferredMaintenanceWindow": str,
         "PreferredBackupWindow": str,
     },
     total=False,
 )
 
-
 class UpdateServerRequestRequestTypeDef(
     _RequiredUpdateServerRequestRequestTypeDef, _OptionalUpdateServerRequestRequestTypeDef
 ):
     pass
 
+DescribeAccountAttributesResponseTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseTypeDef",
+    {
+        "Attributes": List[AccountAttributeTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 AssociateNodeRequestRequestTypeDef = TypedDict(
     "AssociateNodeRequestRequestTypeDef",
     {
         "ServerName": str,
         "NodeName": str,
         "EngineAttributes": Sequence[EngineAttributeTypeDef],
     },
 )
 
+DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
+    "DescribeNodeAssociationStatusResponseTypeDef",
+    {
+        "NodeAssociationStatus": NodeAssociationStatusType,
+        "EngineAttributes": List[EngineAttributeTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDisassociateNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateNodeRequestRequestTypeDef",
     {
         "ServerName": str,
         "NodeName": str,
     },
 )
@@ -364,21 +445,19 @@
     "_OptionalDisassociateNodeRequestRequestTypeDef",
     {
         "EngineAttributes": Sequence[EngineAttributeTypeDef],
     },
     total=False,
 )
 
-
 class DisassociateNodeRequestRequestTypeDef(
     _RequiredDisassociateNodeRequestRequestTypeDef, _OptionalDisassociateNodeRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredExportServerEngineAttributeRequestRequestTypeDef = TypedDict(
     "_RequiredExportServerEngineAttributeRequestRequestTypeDef",
     {
         "ExportAttributeName": str,
         "ServerName": str,
     },
 )
@@ -386,21 +465,28 @@
     "_OptionalExportServerEngineAttributeRequestRequestTypeDef",
     {
         "InputAttributes": Sequence[EngineAttributeTypeDef],
     },
     total=False,
 )
 
-
 class ExportServerEngineAttributeRequestRequestTypeDef(
     _RequiredExportServerEngineAttributeRequestRequestTypeDef,
     _OptionalExportServerEngineAttributeRequestRequestTypeDef,
 ):
     pass
 
+ExportServerEngineAttributeResponseTypeDef = TypedDict(
+    "ExportServerEngineAttributeResponseTypeDef",
+    {
+        "EngineAttribute": EngineAttributeTypeDef,
+        "ServerName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 ServerTypeDef = TypedDict(
     "ServerTypeDef",
     {
         "AssociatePublicIpAddress": bool,
         "BackupRetentionCount": int,
         "ServerName": str,
@@ -439,77 +525,33 @@
     "_OptionalStartMaintenanceRequestRequestTypeDef",
     {
         "EngineAttributes": Sequence[EngineAttributeTypeDef],
     },
     total=False,
 )
 
-
 class StartMaintenanceRequestRequestTypeDef(
     _RequiredStartMaintenanceRequestRequestTypeDef, _OptionalStartMaintenanceRequestRequestTypeDef
 ):
     pass
 
-
-AssociateNodeResponseTypeDef = TypedDict(
-    "AssociateNodeResponseTypeDef",
-    {
-        "NodeAssociationStatusToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountAttributesResponseTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseTypeDef",
-    {
-        "Attributes": List[AccountAttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
-    "DescribeNodeAssociationStatusResponseTypeDef",
-    {
-        "NodeAssociationStatus": NodeAssociationStatusType,
-        "EngineAttributes": List[EngineAttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateNodeResponseTypeDef = TypedDict(
-    "DisassociateNodeResponseTypeDef",
-    {
-        "NodeAssociationStatusToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ExportServerEngineAttributeResponseTypeDef = TypedDict(
-    "ExportServerEngineAttributeResponseTypeDef",
-    {
-        "EngineAttribute": EngineAttributeTypeDef,
-        "ServerName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateBackupResponseTypeDef = TypedDict(
     "CreateBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBackupsResponseTypeDef = TypedDict(
     "DescribeBackupsResponseTypeDef",
     {
         "Backups": List[BackupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBackupRequestRequestTypeDef",
     {
         "ServerName": str,
@@ -520,21 +562,19 @@
     {
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateBackupRequestRequestTypeDef(
     _RequiredCreateBackupRequestRequestTypeDef, _OptionalCreateBackupRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateServerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServerRequestRequestTypeDef",
     {
         "Engine": str,
         "ServerName": str,
         "InstanceProfileArn": str,
         "InstanceType": str,
@@ -560,107 +600,42 @@
         "SubnetIds": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "BackupId": str,
     },
     total=False,
 )
 
-
 class CreateServerRequestRequestTypeDef(
     _RequiredCreateServerRequestRequestTypeDef, _OptionalCreateServerRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
-    {
-        "BackupId": str,
-        "ServerName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "ServerName": str,
-    },
-)
-_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeEventsRequestDescribeEventsPaginateTypeDef(
-    _RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef,
-    _OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef,
-):
-    pass
-
-
-DescribeServersRequestDescribeServersPaginateTypeDef = TypedDict(
-    "DescribeServersRequestDescribeServersPaginateTypeDef",
-    {
-        "ServerName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "ServerEvents": List[ServerEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef = TypedDict(
     "_RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
     {
         "NodeAssociationStatusToken": str,
@@ -671,63 +646,61 @@
     "_OptionalDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef(
     _RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
     _OptionalDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
 ):
     pass
 
-
 CreateServerResponseTypeDef = TypedDict(
     "CreateServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeServersResponseTypeDef = TypedDict(
     "DescribeServersResponseTypeDef",
     {
         "Servers": List[ServerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreServerResponseTypeDef = TypedDict(
     "RestoreServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartMaintenanceResponseTypeDef = TypedDict(
     "StartMaintenanceResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServerEngineAttributesResponseTypeDef = TypedDict(
     "UpdateServerEngineAttributesResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServerResponseTypeDef = TypedDict(
     "UpdateServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/type_defs.pyi` & `mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,54 +24,55 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountAttributeTypeDef",
     "EngineAttributeTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateNodeResponseTypeDef",
     "BackupTypeDef",
     "TagTypeDef",
     "DeleteBackupRequestRequestTypeDef",
     "DeleteServerRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "ServerEventTypeDef",
     "WaiterConfigTypeDef",
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
+    "DescribeServersRequestDescribeServersPaginateTypeDef",
     "DescribeServersRequestRequestTypeDef",
+    "DisassociateNodeResponseTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreServerRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateServerEngineAttributesRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
+    "DescribeAccountAttributesResponseTypeDef",
     "AssociateNodeRequestRequestTypeDef",
+    "DescribeNodeAssociationStatusResponseTypeDef",
     "DisassociateNodeRequestRequestTypeDef",
     "ExportServerEngineAttributeRequestRequestTypeDef",
+    "ExportServerEngineAttributeResponseTypeDef",
     "ServerTypeDef",
     "StartMaintenanceRequestRequestTypeDef",
-    "AssociateNodeResponseTypeDef",
-    "DescribeAccountAttributesResponseTypeDef",
-    "DescribeNodeAssociationStatusResponseTypeDef",
-    "DisassociateNodeResponseTypeDef",
-    "ExportServerEngineAttributeResponseTypeDef",
     "CreateBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
     "CreateBackupRequestRequestTypeDef",
     "CreateServerRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    "DescribeServersRequestDescribeServersPaginateTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
     "CreateServerResponseTypeDef",
     "DescribeServersResponseTypeDef",
     "RestoreServerResponseTypeDef",
     "StartMaintenanceResponseTypeDef",
     "UpdateServerEngineAttributesResponseTypeDef",
@@ -93,22 +94,19 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateNodeResponseTypeDef = TypedDict(
+    "AssociateNodeResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "NodeAssociationStatusToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BackupTypeDef = TypedDict(
     "BackupTypeDef",
     {
         "BackupArn": str,
@@ -157,20 +155,20 @@
 DeleteServerRequestRequestTypeDef = TypedDict(
     "DeleteServerRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "BackupId": str,
+        "ServerName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
@@ -178,14 +176,36 @@
         "ServerName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "ServerName": str,
+    },
+)
+_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeEventsRequestDescribeEventsPaginateTypeDef(
+    _RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef,
+    _OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeEventsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEventsRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 _OptionalDescribeEventsRequestRequestTypeDef = TypedDict(
@@ -193,19 +213,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeEventsRequestRequestTypeDef(
     _RequiredDescribeEventsRequestRequestTypeDef, _OptionalDescribeEventsRequestRequestTypeDef
 ):
     pass
 
+
 ServerEventTypeDef = TypedDict(
     "ServerEventTypeDef",
     {
         "CreatedAt": datetime,
         "ServerName": str,
         "Message": str,
         "LogUrl": str,
@@ -226,24 +248,63 @@
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
     {
         "NodeAssociationStatusToken": str,
         "ServerName": str,
     },
 )
 
+DescribeServersRequestDescribeServersPaginateTypeDef = TypedDict(
+    "DescribeServersRequestDescribeServersPaginateTypeDef",
+    {
+        "ServerName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeServersRequestRequestTypeDef = TypedDict(
     "DescribeServersRequestRequestTypeDef",
     {
         "ServerName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+DisassociateNodeResponseTypeDef = TypedDict(
+    "DisassociateNodeResponseTypeDef",
+    {
+        "NodeAssociationStatusToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -251,20 +312,43 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
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
 _RequiredRestoreServerRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreServerRequestRequestTypeDef",
     {
         "BackupId": str,
         "ServerName": str,
     },
 )
@@ -273,19 +357,21 @@
     {
         "InstanceType": str,
         "KeyPair": str,
     },
     total=False,
 )
 
+
 class RestoreServerRequestRequestTypeDef(
     _RequiredRestoreServerRequestRequestTypeDef, _OptionalRestoreServerRequestRequestTypeDef
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -301,20 +387,22 @@
     "_OptionalUpdateServerEngineAttributesRequestRequestTypeDef",
     {
         "AttributeValue": str,
     },
     total=False,
 )
 
+
 class UpdateServerEngineAttributesRequestRequestTypeDef(
     _RequiredUpdateServerEngineAttributesRequestRequestTypeDef,
     _OptionalUpdateServerEngineAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateServerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServerRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 _OptionalUpdateServerRequestRequestTypeDef = TypedDict(
@@ -324,28 +412,47 @@
         "BackupRetentionCount": int,
         "PreferredMaintenanceWindow": str,
         "PreferredBackupWindow": str,
     },
     total=False,
 )
 
+
 class UpdateServerRequestRequestTypeDef(
     _RequiredUpdateServerRequestRequestTypeDef, _OptionalUpdateServerRequestRequestTypeDef
 ):
     pass
 
+
+DescribeAccountAttributesResponseTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseTypeDef",
+    {
+        "Attributes": List[AccountAttributeTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AssociateNodeRequestRequestTypeDef = TypedDict(
     "AssociateNodeRequestRequestTypeDef",
     {
         "ServerName": str,
         "NodeName": str,
         "EngineAttributes": Sequence[EngineAttributeTypeDef],
     },
 )
 
+DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
+    "DescribeNodeAssociationStatusResponseTypeDef",
+    {
+        "NodeAssociationStatus": NodeAssociationStatusType,
+        "EngineAttributes": List[EngineAttributeTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDisassociateNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateNodeRequestRequestTypeDef",
     {
         "ServerName": str,
         "NodeName": str,
     },
 )
@@ -353,19 +460,21 @@
     "_OptionalDisassociateNodeRequestRequestTypeDef",
     {
         "EngineAttributes": Sequence[EngineAttributeTypeDef],
     },
     total=False,
 )
 
+
 class DisassociateNodeRequestRequestTypeDef(
     _RequiredDisassociateNodeRequestRequestTypeDef, _OptionalDisassociateNodeRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredExportServerEngineAttributeRequestRequestTypeDef = TypedDict(
     "_RequiredExportServerEngineAttributeRequestRequestTypeDef",
     {
         "ExportAttributeName": str,
         "ServerName": str,
     },
 )
@@ -373,20 +482,31 @@
     "_OptionalExportServerEngineAttributeRequestRequestTypeDef",
     {
         "InputAttributes": Sequence[EngineAttributeTypeDef],
     },
     total=False,
 )
 
+
 class ExportServerEngineAttributeRequestRequestTypeDef(
     _RequiredExportServerEngineAttributeRequestRequestTypeDef,
     _OptionalExportServerEngineAttributeRequestRequestTypeDef,
 ):
     pass
 
+
+ExportServerEngineAttributeResponseTypeDef = TypedDict(
+    "ExportServerEngineAttributeResponseTypeDef",
+    {
+        "EngineAttribute": EngineAttributeTypeDef,
+        "ServerName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ServerTypeDef = TypedDict(
     "ServerTypeDef",
     {
         "AssociatePublicIpAddress": bool,
         "BackupRetentionCount": int,
         "ServerName": str,
         "CreatedAt": datetime,
@@ -424,75 +544,35 @@
     "_OptionalStartMaintenanceRequestRequestTypeDef",
     {
         "EngineAttributes": Sequence[EngineAttributeTypeDef],
     },
     total=False,
 )
 
+
 class StartMaintenanceRequestRequestTypeDef(
     _RequiredStartMaintenanceRequestRequestTypeDef, _OptionalStartMaintenanceRequestRequestTypeDef
 ):
     pass
 
-AssociateNodeResponseTypeDef = TypedDict(
-    "AssociateNodeResponseTypeDef",
-    {
-        "NodeAssociationStatusToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountAttributesResponseTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseTypeDef",
-    {
-        "Attributes": List[AccountAttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
-    "DescribeNodeAssociationStatusResponseTypeDef",
-    {
-        "NodeAssociationStatus": NodeAssociationStatusType,
-        "EngineAttributes": List[EngineAttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateNodeResponseTypeDef = TypedDict(
-    "DisassociateNodeResponseTypeDef",
-    {
-        "NodeAssociationStatusToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ExportServerEngineAttributeResponseTypeDef = TypedDict(
-    "ExportServerEngineAttributeResponseTypeDef",
-    {
-        "EngineAttribute": EngineAttributeTypeDef,
-        "ServerName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 CreateBackupResponseTypeDef = TypedDict(
     "CreateBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBackupsResponseTypeDef = TypedDict(
     "DescribeBackupsResponseTypeDef",
     {
         "Backups": List[BackupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBackupRequestRequestTypeDef",
     {
         "ServerName": str,
@@ -503,19 +583,21 @@
     {
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateBackupRequestRequestTypeDef(
     _RequiredCreateBackupRequestRequestTypeDef, _OptionalCreateBackupRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateServerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServerRequestRequestTypeDef",
     {
         "Engine": str,
         "ServerName": str,
         "InstanceProfileArn": str,
         "InstanceType": str,
@@ -541,101 +623,44 @@
         "SubnetIds": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "BackupId": str,
     },
     total=False,
 )
 
+
 class CreateServerRequestRequestTypeDef(
     _RequiredCreateServerRequestRequestTypeDef, _OptionalCreateServerRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
-    {
-        "BackupId": str,
-        "ServerName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "ServerName": str,
-    },
-)
-_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeEventsRequestDescribeEventsPaginateTypeDef(
-    _RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef,
-    _OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef,
-):
-    pass
-
-DescribeServersRequestDescribeServersPaginateTypeDef = TypedDict(
-    "DescribeServersRequestDescribeServersPaginateTypeDef",
-    {
-        "ServerName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "ServerEvents": List[ServerEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef = TypedDict(
     "_RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
     {
         "NodeAssociationStatusToken": str,
@@ -646,61 +671,63 @@
     "_OptionalDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef(
     _RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
     _OptionalDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
 ):
     pass
 
+
 CreateServerResponseTypeDef = TypedDict(
     "CreateServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeServersResponseTypeDef = TypedDict(
     "DescribeServersResponseTypeDef",
     {
         "Servers": List[ServerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreServerResponseTypeDef = TypedDict(
     "RestoreServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartMaintenanceResponseTypeDef = TypedDict(
     "StartMaintenanceResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServerEngineAttributesResponseTypeDef = TypedDict(
     "UpdateServerEngineAttributesResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServerResponseTypeDef = TypedDict(
     "UpdateServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/waiter.py` & `mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm/waiter.pyi` & `mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm.egg-info/PKG-INFO` & `mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworkscm
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.OpsWorksCM 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.OpsWorksCM 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/
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
 
 <a id="mypy-boto3-opsworkscm"></a>
 
 # mypy-boto3-opsworkscm
 
 [![PyPI - mypy-boto3-opsworkscm](https://img.shields.io/pypi/v/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opsworkscm?color=blue)](https://pypistats.org/packages/mypy-boto3-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorksCM 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[boto3.OpsWorksCM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [mypy-boto3-opsworkscm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -360,51 +361,51 @@
 `mypy_boto3_opsworkscm.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opsworkscm.type_defs import (
     AccountAttributeTypeDef,
     EngineAttributeTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateNodeResponseTypeDef,
     BackupTypeDef,
     TagTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteServerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeBackupsRequestRequestTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     ServerEventTypeDef,
     WaiterConfigTypeDef,
     DescribeNodeAssociationStatusRequestRequestTypeDef,
+    DescribeServersRequestDescribeServersPaginateTypeDef,
     DescribeServersRequestRequestTypeDef,
+    DisassociateNodeResponseTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RestoreServerRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateServerEngineAttributesRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
     AssociateNodeRequestRequestTypeDef,
+    DescribeNodeAssociationStatusResponseTypeDef,
     DisassociateNodeRequestRequestTypeDef,
     ExportServerEngineAttributeRequestRequestTypeDef,
+    ExportServerEngineAttributeResponseTypeDef,
     ServerTypeDef,
     StartMaintenanceRequestRequestTypeDef,
-    AssociateNodeResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
-    DescribeNodeAssociationStatusResponseTypeDef,
-    DisassociateNodeResponseTypeDef,
-    ExportServerEngineAttributeResponseTypeDef,
     CreateBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateServerRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
-    DescribeServersRequestDescribeServersPaginateTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
     CreateServerResponseTypeDef,
     DescribeServersResponseTypeDef,
     RestoreServerResponseTypeDef,
     StartMaintenanceResponseTypeDef,
     UpdateServerEngineAttributesResponseTypeDef,
@@ -419,42 +420,42 @@
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

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/mypy_boto3_opsworkscm.egg-info/SOURCES.txt` & `mypy-boto3-opsworkscm-1.27.0/mypy_boto3_opsworkscm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.26.0.post1/setup.py` & `mypy-boto3-opsworkscm-1.27.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-opsworkscm.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opsworkscm",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_opsworkscm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpsWorksCM 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.OpsWorksCM 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 opsworkscm type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_opsworkscm": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_opsworkscm": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/",
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


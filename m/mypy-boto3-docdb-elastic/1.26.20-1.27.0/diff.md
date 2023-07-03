# Comparing `tmp/mypy-boto3-docdb-elastic-1.26.20.tar.gz` & `tmp/mypy-boto3-docdb-elastic-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-docdb-elastic-1.26.20.tar", last modified: Wed Nov 30 20:28:44 2022, max compression
+gzip compressed data, was "mypy-boto3-docdb-elastic-1.27.0.tar", last modified: Mon Jul  3 19:50:40 2023, max compression
```

## Comparing `mypy-boto3-docdb-elastic-1.26.20.tar` & `mypy-boto3-docdb-elastic-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 20:28:44.623351 mypy-boto3-docdb-elastic-1.26.20/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    14161 2022-11-30 20:28:44.619351 mypy-boto3-docdb-elastic-1.26.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12701 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 20:28:44.615351 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/
--rw-r--r--   0 runner    (1001) docker     (122)      829 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      828 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      930 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12867 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    12845 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     7712 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)     7710 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3004 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    10267 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10258 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 20:28:44.619351 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14161 2022-11-30 20:28:44.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      794 2022-11-30 20:28:44.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 20:28:44.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 20:28:44.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-30 20:28:44.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-30 20:28:44.000000 mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-30 20:28:44.623351 mypy-boto3-docdb-elastic-1.26.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2005 2022-11-30 20:27:59.000000 mypy-boto3-docdb-elastic-1.26.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.423141 mypy-boto3-docdb-elastic-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-07-03 19:50:40.423141 mypy-boto3-docdb-elastic-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.423141 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.423141 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-07-03 19:50:40.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 19:50:40.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:40.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 19:50:40.000000 mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:40.423141 mypy-boto3-docdb-elastic-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-03 19:35:49.000000 mypy-boto3-docdb-elastic-1.27.0/setup.py
```

### Comparing `mypy-boto3-docdb-elastic-1.26.20/LICENSE` & `mypy-boto3-docdb-elastic-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-docdb-elastic-1.26.20/PKG-INFO` & `mypy-boto3-docdb-elastic-1.27.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-docdb-elastic
-Version: 1.26.20
-Summary: Type annotations for boto3.DocDBElastic 1.26.20 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.DocDBElastic 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/
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
 
 <a id="mypy-boto3-docdb-elastic"></a>
 
 # mypy-boto3-docdb-elastic
 
 [![PyPI - mypy-boto3-docdb-elastic](https://img.shields.io/pypi/v/mypy-boto3-docdb-elastic.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb-elastic)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb-elastic.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb-elastic)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-docdb-elastic?color=blue)](https://pypistats.org/packages/mypy-boto3-docdb-elastic)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDBElastic 1.26.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
+[boto3.DocDBElastic 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
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
 [mypy-boto3-docdb-elastic docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,83 +329,83 @@
 ```python
 from mypy_boto3_docdb_elastic.type_defs import (
     ClusterInListTypeDef,
     ClusterSnapshotInListTypeDef,
     ClusterSnapshotTypeDef,
     ClusterTypeDef,
     CreateClusterInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateClusterSnapshotInputRequestTypeDef,
     DeleteClusterInputRequestTypeDef,
     DeleteClusterSnapshotInputRequestTypeDef,
     GetClusterInputRequestTypeDef,
     GetClusterSnapshotInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
     ListClusterSnapshotsInputRequestTypeDef,
+    ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RestoreClusterFromSnapshotInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterInputRequestTypeDef,
-    CreateClusterOutputTypeDef,
+    ListClustersOutputTypeDef,
+    ListClusterSnapshotsOutputTypeDef,
     CreateClusterSnapshotOutputTypeDef,
-    DeleteClusterOutputTypeDef,
     DeleteClusterSnapshotOutputTypeDef,
-    GetClusterOutputTypeDef,
     GetClusterSnapshotOutputTypeDef,
-    ListClusterSnapshotsOutputTypeDef,
-    ListClustersOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    CreateClusterOutputTypeDef,
+    DeleteClusterOutputTypeDef,
+    GetClusterOutputTypeDef,
     RestoreClusterFromSnapshotOutputTypeDef,
     UpdateClusterOutputTypeDef,
-    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
 )
 
 
 def get_structure() -> ClusterInListTypeDef:
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

### Comparing `mypy-boto3-docdb-elastic-1.26.20/README.md` & `mypy-boto3-docdb-elastic-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-docdb-elastic"></a>
 
 # mypy-boto3-docdb-elastic
 
 [![PyPI - mypy-boto3-docdb-elastic](https://img.shields.io/pypi/v/mypy-boto3-docdb-elastic.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb-elastic)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb-elastic.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb-elastic)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-docdb-elastic?color=blue)](https://pypistats.org/packages/mypy-boto3-docdb-elastic)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDBElastic 1.26.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
+[boto3.DocDBElastic 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
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
 [mypy-boto3-docdb-elastic docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,83 +297,83 @@
 ```python
 from mypy_boto3_docdb_elastic.type_defs import (
     ClusterInListTypeDef,
     ClusterSnapshotInListTypeDef,
     ClusterSnapshotTypeDef,
     ClusterTypeDef,
     CreateClusterInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateClusterSnapshotInputRequestTypeDef,
     DeleteClusterInputRequestTypeDef,
     DeleteClusterSnapshotInputRequestTypeDef,
     GetClusterInputRequestTypeDef,
     GetClusterSnapshotInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
     ListClusterSnapshotsInputRequestTypeDef,
+    ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RestoreClusterFromSnapshotInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterInputRequestTypeDef,
-    CreateClusterOutputTypeDef,
+    ListClustersOutputTypeDef,
+    ListClusterSnapshotsOutputTypeDef,
     CreateClusterSnapshotOutputTypeDef,
-    DeleteClusterOutputTypeDef,
     DeleteClusterSnapshotOutputTypeDef,
-    GetClusterOutputTypeDef,
     GetClusterSnapshotOutputTypeDef,
-    ListClusterSnapshotsOutputTypeDef,
-    ListClustersOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    CreateClusterOutputTypeDef,
+    DeleteClusterOutputTypeDef,
+    GetClusterOutputTypeDef,
     RestoreClusterFromSnapshotOutputTypeDef,
     UpdateClusterOutputTypeDef,
-    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
 )
 
 
 def get_structure() -> ClusterInListTypeDef:
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

### Comparing `mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/__init__.py` & `mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/__init__.pyi` & `mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/__main__.py` & `mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DocDBElastic 1.26.20\nVersion:         1.26.20\nBuilder"
-        " version: 7.11.11\nDocs:           "
+        "Type annotations for boto3.DocDBElastic 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.20")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/client.py` & `mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/client.pyi` & `mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/literals.py` & `mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
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
@@ -85,30 +86,34 @@
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
@@ -187,14 +192,15 @@
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
@@ -205,34 +211,38 @@
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
@@ -245,14 +255,15 @@
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
@@ -271,24 +282,28 @@
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
@@ -317,14 +332,15 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -358,18 +374,21 @@
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

### Comparing `mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/literals.pyi` & `mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
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
@@ -83,30 +84,34 @@
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
@@ -185,14 +190,15 @@
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
@@ -203,34 +209,38 @@
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
@@ -243,14 +253,15 @@
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
@@ -269,24 +280,28 @@
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
@@ -315,14 +330,15 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -356,18 +372,21 @@
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

### Comparing `mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/paginator.py` & `mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 class ListClusterSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusterSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclustersnapshotspaginator)
     """
 
     def paginate(
-        self, *, clusterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, clusterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClusterSnapshotsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusterSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclustersnapshotspaginator)
         """
 
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclusterspaginator)
         """
```

### Comparing `mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/paginator.pyi` & `mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 class ListClusterSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusterSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclustersnapshotspaginator)
     """
 
     def paginate(
-        self, *, clusterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, clusterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClusterSnapshotsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusterSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclustersnapshotspaginator)
         """
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclusterspaginator)
         """
```

### Comparing `mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/type_defs.py` & `mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -17,48 +17,47 @@
 from .literals import AuthType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ClusterInListTypeDef",
     "ClusterSnapshotInListTypeDef",
     "ClusterSnapshotTypeDef",
     "ClusterTypeDef",
     "CreateClusterInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateClusterSnapshotInputRequestTypeDef",
     "DeleteClusterInputRequestTypeDef",
     "DeleteClusterSnapshotInputRequestTypeDef",
     "GetClusterInputRequestTypeDef",
     "GetClusterSnapshotInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
     "ListClusterSnapshotsInputRequestTypeDef",
+    "ListClustersInputListClustersPaginateTypeDef",
     "ListClustersInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreClusterFromSnapshotInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateClusterInputRequestTypeDef",
-    "CreateClusterOutputTypeDef",
+    "ListClustersOutputTypeDef",
+    "ListClusterSnapshotsOutputTypeDef",
     "CreateClusterSnapshotOutputTypeDef",
-    "DeleteClusterOutputTypeDef",
     "DeleteClusterSnapshotOutputTypeDef",
-    "GetClusterOutputTypeDef",
     "GetClusterSnapshotOutputTypeDef",
-    "ListClusterSnapshotsOutputTypeDef",
-    "ListClustersOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "CreateClusterOutputTypeDef",
+    "DeleteClusterOutputTypeDef",
+    "GetClusterOutputTypeDef",
     "RestoreClusterFromSnapshotOutputTypeDef",
     "UpdateClusterOutputTypeDef",
-    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
-    "ListClustersInputListClustersPaginateTypeDef",
 )
 
 ClusterInListTypeDef = TypedDict(
     "ClusterInListTypeDef",
     {
         "clusterArn": str,
         "clusterName": str,
@@ -132,32 +131,19 @@
         "subnetIds": Sequence[str],
         "tags": Mapping[str, str],
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateClusterInputRequestTypeDef(
     _RequiredCreateClusterInputRequestTypeDef, _OptionalCreateClusterInputRequestTypeDef
 ):
     pass
 
-
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
 _RequiredCreateClusterSnapshotInputRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSnapshotInputRequestTypeDef",
     {
         "clusterArn": str,
         "snapshotName": str,
     },
 )
@@ -165,22 +151,20 @@
     "_OptionalCreateClusterSnapshotInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateClusterSnapshotInputRequestTypeDef(
     _RequiredCreateClusterSnapshotInputRequestTypeDef,
     _OptionalCreateClusterSnapshotInputRequestTypeDef,
 ):
     pass
 
-
 DeleteClusterInputRequestTypeDef = TypedDict(
     "DeleteClusterInputRequestTypeDef",
     {
         "clusterArn": str,
     },
 )
 
@@ -201,34 +185,41 @@
 GetClusterSnapshotInputRequestTypeDef = TypedDict(
     "GetClusterSnapshotInputRequestTypeDef",
     {
         "snapshotArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef = TypedDict(
+    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "clusterArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListClusterSnapshotsInputRequestTypeDef = TypedDict(
     "ListClusterSnapshotsInputRequestTypeDef",
     {
         "clusterArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListClustersInputListClustersPaginateTypeDef = TypedDict(
+    "ListClustersInputListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersInputRequestTypeDef = TypedDict(
     "ListClustersInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -237,14 +228,43 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
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
 _RequiredRestoreClusterFromSnapshotInputRequestTypeDef = TypedDict(
     "_RequiredRestoreClusterFromSnapshotInputRequestTypeDef",
     {
         "clusterName": str,
         "snapshotArn": str,
     },
 )
@@ -255,22 +275,20 @@
         "subnetIds": Sequence[str],
         "tags": Mapping[str, str],
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class RestoreClusterFromSnapshotInputRequestTypeDef(
     _RequiredRestoreClusterFromSnapshotInputRequestTypeDef,
     _OptionalRestoreClusterFromSnapshotInputRequestTypeDef,
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -300,120 +318,93 @@
         "shardCount": int,
         "subnetIds": Sequence[str],
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateClusterInputRequestTypeDef(
     _RequiredUpdateClusterInputRequestTypeDef, _OptionalUpdateClusterInputRequestTypeDef
 ):
     pass
 
-
-CreateClusterOutputTypeDef = TypedDict(
-    "CreateClusterOutputTypeDef",
+ListClustersOutputTypeDef = TypedDict(
+    "ListClustersOutputTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "clusters": List[ClusterInListTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateClusterSnapshotOutputTypeDef = TypedDict(
-    "CreateClusterSnapshotOutputTypeDef",
+ListClusterSnapshotsOutputTypeDef = TypedDict(
+    "ListClusterSnapshotsOutputTypeDef",
     {
-        "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "nextToken": str,
+        "snapshots": List[ClusterSnapshotInListTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteClusterOutputTypeDef = TypedDict(
-    "DeleteClusterOutputTypeDef",
+CreateClusterSnapshotOutputTypeDef = TypedDict(
+    "CreateClusterSnapshotOutputTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "snapshot": ClusterSnapshotTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteClusterSnapshotOutputTypeDef = TypedDict(
     "DeleteClusterSnapshotOutputTypeDef",
     {
         "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetClusterOutputTypeDef = TypedDict(
-    "GetClusterOutputTypeDef",
-    {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetClusterSnapshotOutputTypeDef = TypedDict(
     "GetClusterSnapshotOutputTypeDef",
     {
         "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListClusterSnapshotsOutputTypeDef = TypedDict(
-    "ListClusterSnapshotsOutputTypeDef",
+CreateClusterOutputTypeDef = TypedDict(
+    "CreateClusterOutputTypeDef",
     {
-        "nextToken": str,
-        "snapshots": List[ClusterSnapshotInListTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListClustersOutputTypeDef = TypedDict(
-    "ListClustersOutputTypeDef",
+DeleteClusterOutputTypeDef = TypedDict(
+    "DeleteClusterOutputTypeDef",
     {
-        "clusters": List[ClusterInListTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+GetClusterOutputTypeDef = TypedDict(
+    "GetClusterOutputTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreClusterFromSnapshotOutputTypeDef = TypedDict(
     "RestoreClusterFromSnapshotOutputTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterOutputTypeDef = TypedDict(
     "UpdateClusterOutputTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef = TypedDict(
-    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
-    {
-        "clusterArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-ListClustersInputListClustersPaginateTypeDef = TypedDict(
-    "ListClustersInputListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
```

### Comparing `mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic/type_defs.pyi` & `mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,47 +17,48 @@
 from .literals import AuthType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ClusterInListTypeDef",
     "ClusterSnapshotInListTypeDef",
     "ClusterSnapshotTypeDef",
     "ClusterTypeDef",
     "CreateClusterInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateClusterSnapshotInputRequestTypeDef",
     "DeleteClusterInputRequestTypeDef",
     "DeleteClusterSnapshotInputRequestTypeDef",
     "GetClusterInputRequestTypeDef",
     "GetClusterSnapshotInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
     "ListClusterSnapshotsInputRequestTypeDef",
+    "ListClustersInputListClustersPaginateTypeDef",
     "ListClustersInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreClusterFromSnapshotInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateClusterInputRequestTypeDef",
-    "CreateClusterOutputTypeDef",
+    "ListClustersOutputTypeDef",
+    "ListClusterSnapshotsOutputTypeDef",
     "CreateClusterSnapshotOutputTypeDef",
-    "DeleteClusterOutputTypeDef",
     "DeleteClusterSnapshotOutputTypeDef",
-    "GetClusterOutputTypeDef",
     "GetClusterSnapshotOutputTypeDef",
-    "ListClusterSnapshotsOutputTypeDef",
-    "ListClustersOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "CreateClusterOutputTypeDef",
+    "DeleteClusterOutputTypeDef",
+    "GetClusterOutputTypeDef",
     "RestoreClusterFromSnapshotOutputTypeDef",
     "UpdateClusterOutputTypeDef",
-    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
-    "ListClustersInputListClustersPaginateTypeDef",
 )
 
 ClusterInListTypeDef = TypedDict(
     "ClusterInListTypeDef",
     {
         "clusterArn": str,
         "clusterName": str,
@@ -131,29 +132,20 @@
         "subnetIds": Sequence[str],
         "tags": Mapping[str, str],
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateClusterInputRequestTypeDef(
     _RequiredCreateClusterInputRequestTypeDef, _OptionalCreateClusterInputRequestTypeDef
 ):
     pass
 
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
 
 _RequiredCreateClusterSnapshotInputRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSnapshotInputRequestTypeDef",
     {
         "clusterArn": str,
         "snapshotName": str,
     },
@@ -162,20 +154,22 @@
     "_OptionalCreateClusterSnapshotInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateClusterSnapshotInputRequestTypeDef(
     _RequiredCreateClusterSnapshotInputRequestTypeDef,
     _OptionalCreateClusterSnapshotInputRequestTypeDef,
 ):
     pass
 
+
 DeleteClusterInputRequestTypeDef = TypedDict(
     "DeleteClusterInputRequestTypeDef",
     {
         "clusterArn": str,
     },
 )
 
@@ -196,34 +190,41 @@
 GetClusterSnapshotInputRequestTypeDef = TypedDict(
     "GetClusterSnapshotInputRequestTypeDef",
     {
         "snapshotArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef = TypedDict(
+    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "clusterArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListClusterSnapshotsInputRequestTypeDef = TypedDict(
     "ListClusterSnapshotsInputRequestTypeDef",
     {
         "clusterArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListClustersInputListClustersPaginateTypeDef = TypedDict(
+    "ListClustersInputListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersInputRequestTypeDef = TypedDict(
     "ListClustersInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -232,14 +233,43 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
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
 _RequiredRestoreClusterFromSnapshotInputRequestTypeDef = TypedDict(
     "_RequiredRestoreClusterFromSnapshotInputRequestTypeDef",
     {
         "clusterName": str,
         "snapshotArn": str,
     },
 )
@@ -250,20 +280,22 @@
         "subnetIds": Sequence[str],
         "tags": Mapping[str, str],
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class RestoreClusterFromSnapshotInputRequestTypeDef(
     _RequiredRestoreClusterFromSnapshotInputRequestTypeDef,
     _OptionalRestoreClusterFromSnapshotInputRequestTypeDef,
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -293,118 +325,95 @@
         "shardCount": int,
         "subnetIds": Sequence[str],
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateClusterInputRequestTypeDef(
     _RequiredUpdateClusterInputRequestTypeDef, _OptionalUpdateClusterInputRequestTypeDef
 ):
     pass
 
-CreateClusterOutputTypeDef = TypedDict(
-    "CreateClusterOutputTypeDef",
+
+ListClustersOutputTypeDef = TypedDict(
+    "ListClustersOutputTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "clusters": List[ClusterInListTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateClusterSnapshotOutputTypeDef = TypedDict(
-    "CreateClusterSnapshotOutputTypeDef",
+ListClusterSnapshotsOutputTypeDef = TypedDict(
+    "ListClusterSnapshotsOutputTypeDef",
     {
-        "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "nextToken": str,
+        "snapshots": List[ClusterSnapshotInListTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteClusterOutputTypeDef = TypedDict(
-    "DeleteClusterOutputTypeDef",
+CreateClusterSnapshotOutputTypeDef = TypedDict(
+    "CreateClusterSnapshotOutputTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "snapshot": ClusterSnapshotTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteClusterSnapshotOutputTypeDef = TypedDict(
     "DeleteClusterSnapshotOutputTypeDef",
     {
         "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetClusterOutputTypeDef = TypedDict(
-    "GetClusterOutputTypeDef",
-    {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetClusterSnapshotOutputTypeDef = TypedDict(
     "GetClusterSnapshotOutputTypeDef",
     {
         "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListClusterSnapshotsOutputTypeDef = TypedDict(
-    "ListClusterSnapshotsOutputTypeDef",
+CreateClusterOutputTypeDef = TypedDict(
+    "CreateClusterOutputTypeDef",
     {
-        "nextToken": str,
-        "snapshots": List[ClusterSnapshotInListTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListClustersOutputTypeDef = TypedDict(
-    "ListClustersOutputTypeDef",
+DeleteClusterOutputTypeDef = TypedDict(
+    "DeleteClusterOutputTypeDef",
     {
-        "clusters": List[ClusterInListTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+GetClusterOutputTypeDef = TypedDict(
+    "GetClusterOutputTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreClusterFromSnapshotOutputTypeDef = TypedDict(
     "RestoreClusterFromSnapshotOutputTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterOutputTypeDef = TypedDict(
     "UpdateClusterOutputTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef = TypedDict(
-    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
-    {
-        "clusterArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-ListClustersInputListClustersPaginateTypeDef = TypedDict(
-    "ListClustersInputListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
```

### Comparing `mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic.egg-info/PKG-INFO` & `mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-docdb-elastic
-Version: 1.26.20
-Summary: Type annotations for boto3.DocDBElastic 1.26.20 service generated with mypy-boto3-builder 7.11.11
+Version: 1.27.0
+Summary: Type annotations for boto3.DocDBElastic 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/
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
 
 <a id="mypy-boto3-docdb-elastic"></a>
 
 # mypy-boto3-docdb-elastic
 
 [![PyPI - mypy-boto3-docdb-elastic](https://img.shields.io/pypi/v/mypy-boto3-docdb-elastic.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb-elastic)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb-elastic.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb-elastic)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-docdb-elastic?color=blue)](https://pypistats.org/packages/mypy-boto3-docdb-elastic)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDBElastic 1.26.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
+[boto3.DocDBElastic 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
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
 [mypy-boto3-docdb-elastic docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,83 +329,83 @@
 ```python
 from mypy_boto3_docdb_elastic.type_defs import (
     ClusterInListTypeDef,
     ClusterSnapshotInListTypeDef,
     ClusterSnapshotTypeDef,
     ClusterTypeDef,
     CreateClusterInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     CreateClusterSnapshotInputRequestTypeDef,
     DeleteClusterInputRequestTypeDef,
     DeleteClusterSnapshotInputRequestTypeDef,
     GetClusterInputRequestTypeDef,
     GetClusterSnapshotInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
     ListClusterSnapshotsInputRequestTypeDef,
+    ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     RestoreClusterFromSnapshotInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterInputRequestTypeDef,
-    CreateClusterOutputTypeDef,
+    ListClustersOutputTypeDef,
+    ListClusterSnapshotsOutputTypeDef,
     CreateClusterSnapshotOutputTypeDef,
-    DeleteClusterOutputTypeDef,
     DeleteClusterSnapshotOutputTypeDef,
-    GetClusterOutputTypeDef,
     GetClusterSnapshotOutputTypeDef,
-    ListClusterSnapshotsOutputTypeDef,
-    ListClustersOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    CreateClusterOutputTypeDef,
+    DeleteClusterOutputTypeDef,
+    GetClusterOutputTypeDef,
     RestoreClusterFromSnapshotOutputTypeDef,
     UpdateClusterOutputTypeDef,
-    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
 )
 
 
 def get_structure() -> ClusterInListTypeDef:
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

### Comparing `mypy-boto3-docdb-elastic-1.26.20/mypy_boto3_docdb_elastic.egg-info/SOURCES.txt` & `mypy-boto3-docdb-elastic-1.27.0/mypy_boto3_docdb_elastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-elastic-1.26.20/setup.py` & `mypy-boto3-docdb-elastic-1.27.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-docdb-elastic.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-docdb-elastic",
-    version="1.26.20",
+    version="1.27.0",
     packages=["mypy_boto3_docdb_elastic"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DocDBElastic 1.26.20 service generated with mypy-boto3-builder"
-        " 7.11.11"
+        "Type annotations for boto3.DocDBElastic 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 docdb-elastic type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_docdb_elastic": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_docdb_elastic": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/",
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


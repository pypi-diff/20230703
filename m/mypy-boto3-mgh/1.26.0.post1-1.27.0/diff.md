# Comparing `tmp/mypy-boto3-mgh-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-mgh-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mgh-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:45 2022, max compression
+gzip compressed data, was "mypy-boto3-mgh-1.27.0.tar", last modified: Mon Jul  3 19:51:08 2023, max compression
```

## Comparing `mypy-boto3-mgh-1.26.0.post1.tar` & `mypy-boto3-mgh-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:45.064836 mypy-boto3-mgh-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15033 2022-11-01 21:43:45.064836 mypy-boto3-mgh-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13599 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:45.060836 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/
--rw-r--r--   0 runner    (1001) docker     (121)     1609 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17062 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    17033 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8242 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8240 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6519 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6512 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    17664 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    17629 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:45.064836 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15033 2022-11-01 21:43:44.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-11-01 21:43:44.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:44.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:44.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:44.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-01 21:43:44.000000 mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:45.064836 mypy-boto3-mgh-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2022-11-01 21:38:17.000000 mypy-boto3-mgh-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.455685 mypy-boto3-mgh-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:18.000000 mypy-boto3-mgh-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15051 2023-07-03 19:51:08.455685 mypy-boto3-mgh-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13573 2023-07-03 19:42:18.000000 mypy-boto3-mgh-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.443685 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-03 19:42:18.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-03 19:42:18.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-03 19:42:18.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17205 2023-07-03 19:42:18.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-07-03 19:42:18.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-07-03 19:42:18.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-03 19:42:18.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-03 19:42:18.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-07-03 19:42:18.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:18.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-07-03 19:42:18.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-07-03 19:42:18.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:18.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.455685 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15051 2023-07-03 19:51:08.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:51:08.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:08.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:08.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:08.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:08.000000 mypy-boto3-mgh-1.27.0/mypy_boto3_mgh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:08.455685 mypy-boto3-mgh-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-03 19:42:17.000000 mypy-boto3-mgh-1.27.0/setup.py
```

### Comparing `mypy-boto3-mgh-1.26.0.post1/LICENSE` & `mypy-boto3-mgh-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-mgh-1.26.0.post1/PKG-INFO` & `mypy-boto3-mgh-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgh
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.MigrationHub 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.MigrationHub 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/
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
 
 <a id="mypy-boto3-mgh"></a>
 
 # mypy-boto3-mgh
 
 [![PyPI - mypy-boto3-mgh](https://img.shields.io/pypi/v/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mgh?color=blue)](https://pypistats.org/packages/mypy-boto3-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHub 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[boto3.MigrationHub 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
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
 [mypy-boto3-mgh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,41 +350,41 @@
 from mypy_boto3_mgh.type_defs import (
     ApplicationStateTypeDef,
     CreatedArtifactTypeDef,
     DiscoveredResourceTypeDef,
     CreateProgressUpdateStreamRequestRequestTypeDef,
     DeleteProgressUpdateStreamRequestRequestTypeDef,
     DescribeApplicationStateRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeApplicationStateResultTypeDef,
     DescribeMigrationTaskRequestRequestTypeDef,
     DisassociateCreatedArtifactRequestRequestTypeDef,
     DisassociateDiscoveredResourceRequestRequestTypeDef,
     ImportMigrationTaskRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
     ListApplicationStatesRequestRequestTypeDef,
+    ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
     ListCreatedArtifactsRequestRequestTypeDef,
+    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
+    ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
     ListMigrationTasksRequestRequestTypeDef,
     MigrationTaskSummaryTypeDef,
+    ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListProgressUpdateStreamsRequestRequestTypeDef,
     ProgressUpdateStreamSummaryTypeDef,
     ResourceAttributeTypeDef,
     TaskTypeDef,
     NotifyApplicationStateRequestRequestTypeDef,
-    AssociateCreatedArtifactRequestRequestTypeDef,
-    AssociateDiscoveredResourceRequestRequestTypeDef,
-    DescribeApplicationStateResultTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     ListApplicationStatesResultTypeDef,
+    AssociateCreatedArtifactRequestRequestTypeDef,
     ListCreatedArtifactsResultTypeDef,
+    AssociateDiscoveredResourceRequestRequestTypeDef,
     ListDiscoveredResourcesResultTypeDef,
-    ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
-    ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
-    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-    ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
-    ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListMigrationTasksResultTypeDef,
     ListProgressUpdateStreamsResultTypeDef,
     PutResourceAttributesRequestRequestTypeDef,
     MigrationTaskTypeDef,
     NotifyMigrationTaskStateRequestRequestTypeDef,
     DescribeMigrationTaskResultTypeDef,
 )
@@ -396,42 +397,42 @@
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

### Comparing `mypy-boto3-mgh-1.26.0.post1/README.md` & `mypy-boto3-mgh-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mgh"></a>
 
 # mypy-boto3-mgh
 
 [![PyPI - mypy-boto3-mgh](https://img.shields.io/pypi/v/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mgh?color=blue)](https://pypistats.org/packages/mypy-boto3-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHub 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[boto3.MigrationHub 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
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
 [mypy-boto3-mgh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,41 +318,41 @@
 from mypy_boto3_mgh.type_defs import (
     ApplicationStateTypeDef,
     CreatedArtifactTypeDef,
     DiscoveredResourceTypeDef,
     CreateProgressUpdateStreamRequestRequestTypeDef,
     DeleteProgressUpdateStreamRequestRequestTypeDef,
     DescribeApplicationStateRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeApplicationStateResultTypeDef,
     DescribeMigrationTaskRequestRequestTypeDef,
     DisassociateCreatedArtifactRequestRequestTypeDef,
     DisassociateDiscoveredResourceRequestRequestTypeDef,
     ImportMigrationTaskRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
     ListApplicationStatesRequestRequestTypeDef,
+    ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
     ListCreatedArtifactsRequestRequestTypeDef,
+    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
+    ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
     ListMigrationTasksRequestRequestTypeDef,
     MigrationTaskSummaryTypeDef,
+    ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListProgressUpdateStreamsRequestRequestTypeDef,
     ProgressUpdateStreamSummaryTypeDef,
     ResourceAttributeTypeDef,
     TaskTypeDef,
     NotifyApplicationStateRequestRequestTypeDef,
-    AssociateCreatedArtifactRequestRequestTypeDef,
-    AssociateDiscoveredResourceRequestRequestTypeDef,
-    DescribeApplicationStateResultTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     ListApplicationStatesResultTypeDef,
+    AssociateCreatedArtifactRequestRequestTypeDef,
     ListCreatedArtifactsResultTypeDef,
+    AssociateDiscoveredResourceRequestRequestTypeDef,
     ListDiscoveredResourcesResultTypeDef,
-    ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
-    ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
-    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-    ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
-    ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListMigrationTasksResultTypeDef,
     ListProgressUpdateStreamsResultTypeDef,
     PutResourceAttributesRequestRequestTypeDef,
     MigrationTaskTypeDef,
     NotifyMigrationTaskStateRequestRequestTypeDef,
     DescribeMigrationTaskResultTypeDef,
 )
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

### Comparing `mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/__init__.py` & `mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/__init__.pyi` & `mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/__main__.py` & `mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHub 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.MigrationHub 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub\nOther"
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

### Comparing `mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/client.py` & `mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListDiscoveredResourcesResultTypeDef:
         """
-        Lists discovered resources associated with the given `MigrationTask` .
+        Lists discovered resources associated with the given `MigrationTask`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.list_discovered_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/client/#list_discovered_resources)
         """
 
     def list_migration_tasks(
         self, *, NextToken: str = ..., MaxResults: int = ..., ResourceName: str = ...
@@ -337,15 +337,16 @@
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         ResourceAttributeList: Sequence[ResourceAttributeTypeDef],
         DryRun: bool = ...
     ) -> Dict[str, Any]:
         """
-        .
+        Provides identifying details of the resource being migrated so that it can be
+        associated in the Application Discovery Service repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.put_resource_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/client/#put_resource_attributes)
         """
 
     @overload
     def get_paginator(
```

### Comparing `mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/client.pyi` & `mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,15 @@
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListDiscoveredResourcesResultTypeDef:
         """
-        Lists discovered resources associated with the given `MigrationTask` .
+        Lists discovered resources associated with the given `MigrationTask`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.list_discovered_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/client/#list_discovered_resources)
         """
     def list_migration_tasks(
         self, *, NextToken: str = ..., MaxResults: int = ..., ResourceName: str = ...
     ) -> ListMigrationTasksResultTypeDef:
@@ -313,15 +313,16 @@
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         ResourceAttributeList: Sequence[ResourceAttributeTypeDef],
         DryRun: bool = ...
     ) -> Dict[str, Any]:
         """
-        .
+        Provides identifying details of the resource being migrated so that it can be
+        associated in the Application Discovery Service repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.put_resource_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/client/#put_resource_attributes)
         """
     @overload
     def get_paginator(
         self, operation_name: Literal["list_application_states"]
```

### Comparing `mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/literals.py` & `mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,23 +67,25 @@
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
@@ -93,30 +95,35 @@
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
@@ -142,14 +149,15 @@
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
@@ -194,51 +202,57 @@
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
@@ -251,14 +265,15 @@
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
@@ -270,28 +285,35 @@
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
@@ -300,14 +322,15 @@
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
@@ -318,55 +341,64 @@
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

### Comparing `mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/literals.pyi` & `mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -65,23 +65,25 @@
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
@@ -91,30 +93,35 @@
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
@@ -140,14 +147,15 @@
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
@@ -192,51 +200,57 @@
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
@@ -249,14 +263,15 @@
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
@@ -268,28 +283,35 @@
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
@@ -298,14 +320,15 @@
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
@@ -316,55 +339,64 @@
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

### Comparing `mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/paginator.py` & `mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,18 @@
 class ListApplicationStatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListApplicationStates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listapplicationstatespaginator)
     """
 
     def paginate(
-        self, *, ApplicationIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        ApplicationIds: Sequence[str] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationStatesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListApplicationStates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listapplicationstatespaginator)
         """
 
 
@@ -81,15 +84,15 @@
     """
 
     def paginate(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCreatedArtifactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListCreatedArtifacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listcreatedartifactspaginator)
         """
 
 
@@ -100,43 +103,43 @@
     """
 
     def paginate(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDiscoveredResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListDiscoveredResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listdiscoveredresourcespaginator)
         """
 
 
 class ListMigrationTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListMigrationTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listmigrationtaskspaginator)
     """
 
     def paginate(
-        self, *, ResourceName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMigrationTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListMigrationTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listmigrationtaskspaginator)
         """
 
 
 class ListProgressUpdateStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListProgressUpdateStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listprogressupdatestreamspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProgressUpdateStreamsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListProgressUpdateStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listprogressupdatestreamspaginator)
         """
```

### Comparing `mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/paginator.pyi` & `mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,18 @@
 class ListApplicationStatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListApplicationStates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listapplicationstatespaginator)
     """
 
     def paginate(
-        self, *, ApplicationIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        ApplicationIds: Sequence[str] = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationStatesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListApplicationStates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listapplicationstatespaginator)
         """
 
 class ListCreatedArtifactsPaginator(Paginator):
@@ -77,15 +80,15 @@
     """
 
     def paginate(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCreatedArtifactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListCreatedArtifacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listcreatedartifactspaginator)
         """
 
 class ListDiscoveredResourcesPaginator(Paginator):
@@ -95,41 +98,41 @@
     """
 
     def paginate(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDiscoveredResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListDiscoveredResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listdiscoveredresourcespaginator)
         """
 
 class ListMigrationTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListMigrationTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listmigrationtaskspaginator)
     """
 
     def paginate(
-        self, *, ResourceName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMigrationTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListMigrationTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listmigrationtaskspaginator)
         """
 
 class ListProgressUpdateStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListProgressUpdateStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listprogressupdatestreamspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProgressUpdateStreamsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListProgressUpdateStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listprogressupdatestreamspaginator)
         """
```

### Comparing `mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/type_defs.py` & `mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,41 +26,41 @@
 __all__ = (
     "ApplicationStateTypeDef",
     "CreatedArtifactTypeDef",
     "DiscoveredResourceTypeDef",
     "CreateProgressUpdateStreamRequestRequestTypeDef",
     "DeleteProgressUpdateStreamRequestRequestTypeDef",
     "DescribeApplicationStateRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DescribeApplicationStateResultTypeDef",
     "DescribeMigrationTaskRequestRequestTypeDef",
     "DisassociateCreatedArtifactRequestRequestTypeDef",
     "DisassociateDiscoveredResourceRequestRequestTypeDef",
     "ImportMigrationTaskRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
     "ListApplicationStatesRequestRequestTypeDef",
+    "ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
     "ListCreatedArtifactsRequestRequestTypeDef",
+    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
+    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
     "ListMigrationTasksRequestRequestTypeDef",
     "MigrationTaskSummaryTypeDef",
+    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
     "ListProgressUpdateStreamsRequestRequestTypeDef",
     "ProgressUpdateStreamSummaryTypeDef",
     "ResourceAttributeTypeDef",
     "TaskTypeDef",
     "NotifyApplicationStateRequestRequestTypeDef",
-    "AssociateCreatedArtifactRequestRequestTypeDef",
-    "AssociateDiscoveredResourceRequestRequestTypeDef",
-    "DescribeApplicationStateResultTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "ListApplicationStatesResultTypeDef",
+    "AssociateCreatedArtifactRequestRequestTypeDef",
     "ListCreatedArtifactsResultTypeDef",
+    "AssociateDiscoveredResourceRequestRequestTypeDef",
     "ListDiscoveredResourcesResultTypeDef",
-    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
-    "ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
-    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
-    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
     "ListMigrationTasksResultTypeDef",
     "ListProgressUpdateStreamsResultTypeDef",
     "PutResourceAttributesRequestRequestTypeDef",
     "MigrationTaskTypeDef",
     "NotifyMigrationTaskStateRequestRequestTypeDef",
     "DescribeMigrationTaskResultTypeDef",
 )
@@ -162,22 +162,20 @@
 DescribeApplicationStateRequestRequestTypeDef = TypedDict(
     "DescribeApplicationStateRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DescribeApplicationStateResultTypeDef = TypedDict(
+    "DescribeApplicationStateResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ApplicationStatus": ApplicationStatusType,
+        "LastUpdatedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMigrationTaskRequestRequestTypeDef = TypedDict(
     "DescribeMigrationTaskRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
@@ -252,34 +250,56 @@
 class ImportMigrationTaskRequestRequestTypeDef(
     _RequiredImportMigrationTaskRequestRequestTypeDef,
     _OptionalImportMigrationTaskRequestRequestTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListApplicationStatesRequestListApplicationStatesPaginateTypeDef = TypedDict(
+    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ApplicationIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationStatesRequestRequestTypeDef = TypedDict(
     "ListApplicationStatesRequestRequestTypeDef",
     {
         "ApplicationIds": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
+    "_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
+    {
+        "ProgressUpdateStream": str,
+        "MigrationTaskName": str,
+    },
+)
+_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
+    "_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef(
+    _RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
+    _OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListCreatedArtifactsRequestRequestTypeDef = TypedDict(
     "_RequiredListCreatedArtifactsRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
     },
 )
@@ -296,14 +316,37 @@
 class ListCreatedArtifactsRequestRequestTypeDef(
     _RequiredListCreatedArtifactsRequestRequestTypeDef,
     _OptionalListCreatedArtifactsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    {
+        "ProgressUpdateStream": str,
+        "MigrationTaskName": str,
+    },
+)
+_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
+    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
     },
 )
@@ -320,14 +363,23 @@
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
 
+ListMigrationTasksRequestListMigrationTasksPaginateTypeDef = TypedDict(
+    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
+    {
+        "ResourceName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMigrationTasksRequestRequestTypeDef = TypedDict(
     "ListMigrationTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResourceName": str,
     },
@@ -343,14 +395,22 @@
         "ProgressPercent": int,
         "StatusDetail": str,
         "UpdateDateTime": datetime,
     },
     total=False,
 )
 
+ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef = TypedDict(
+    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProgressUpdateStreamsRequestRequestTypeDef = TypedDict(
     "ListProgressUpdateStreamsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -412,14 +472,44 @@
 class NotifyApplicationStateRequestRequestTypeDef(
     _RequiredNotifyApplicationStateRequestRequestTypeDef,
     _OptionalNotifyApplicationStateRequestRequestTypeDef,
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
+
+ListApplicationStatesResultTypeDef = TypedDict(
+    "ListApplicationStatesResultTypeDef",
+    {
+        "ApplicationStateList": List[ApplicationStateTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAssociateCreatedArtifactRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateCreatedArtifactRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
         "CreatedArtifact": CreatedArtifactTypeDef,
     },
@@ -436,14 +526,23 @@
 class AssociateCreatedArtifactRequestRequestTypeDef(
     _RequiredAssociateCreatedArtifactRequestRequestTypeDef,
     _OptionalAssociateCreatedArtifactRequestRequestTypeDef,
 ):
     pass
 
 
+ListCreatedArtifactsResultTypeDef = TypedDict(
+    "ListCreatedArtifactsResultTypeDef",
+    {
+        "NextToken": str,
+        "CreatedArtifactList": List[CreatedArtifactTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAssociateDiscoveredResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateDiscoveredResourceRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
         "DiscoveredResource": DiscoveredResourceTypeDef,
     },
@@ -460,137 +559,38 @@
 class AssociateDiscoveredResourceRequestRequestTypeDef(
     _RequiredAssociateDiscoveredResourceRequestRequestTypeDef,
     _OptionalAssociateDiscoveredResourceRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeApplicationStateResultTypeDef = TypedDict(
-    "DescribeApplicationStateResultTypeDef",
-    {
-        "ApplicationStatus": ApplicationStatusType,
-        "LastUpdatedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationStatesResultTypeDef = TypedDict(
-    "ListApplicationStatesResultTypeDef",
-    {
-        "ApplicationStateList": List[ApplicationStateTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCreatedArtifactsResultTypeDef = TypedDict(
-    "ListCreatedArtifactsResultTypeDef",
-    {
-        "NextToken": str,
-        "CreatedArtifactList": List[CreatedArtifactTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListDiscoveredResourcesResultTypeDef = TypedDict(
     "ListDiscoveredResourcesResultTypeDef",
     {
         "NextToken": str,
         "DiscoveredResourceList": List[DiscoveredResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationStatesRequestListApplicationStatesPaginateTypeDef = TypedDict(
-    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
-    {
-        "ApplicationIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
-    "_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
-    {
-        "ProgressUpdateStream": str,
-        "MigrationTaskName": str,
-    },
-)
-_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
-    "_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef(
-    _RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
-    _OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "ProgressUpdateStream": str,
-        "MigrationTaskName": str,
-    },
-)
-_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
-    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-):
-    pass
-
-
-ListMigrationTasksRequestListMigrationTasksPaginateTypeDef = TypedDict(
-    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
-    {
-        "ResourceName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef = TypedDict(
-    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListMigrationTasksResultTypeDef = TypedDict(
     "ListMigrationTasksResultTypeDef",
     {
         "NextToken": str,
         "MigrationTaskSummaryList": List[MigrationTaskSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProgressUpdateStreamsResultTypeDef = TypedDict(
     "ListProgressUpdateStreamsResultTypeDef",
     {
         "ProgressUpdateStreamSummaryList": List[ProgressUpdateStreamSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutResourceAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourceAttributesRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
@@ -652,10 +652,10 @@
     pass
 
 
 DescribeMigrationTaskResultTypeDef = TypedDict(
     "DescribeMigrationTaskResultTypeDef",
     {
         "MigrationTask": MigrationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh/type_defs.pyi` & `mypy-boto3-mgh-1.27.0/mypy_boto3_mgh/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,41 +25,41 @@
 __all__ = (
     "ApplicationStateTypeDef",
     "CreatedArtifactTypeDef",
     "DiscoveredResourceTypeDef",
     "CreateProgressUpdateStreamRequestRequestTypeDef",
     "DeleteProgressUpdateStreamRequestRequestTypeDef",
     "DescribeApplicationStateRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DescribeApplicationStateResultTypeDef",
     "DescribeMigrationTaskRequestRequestTypeDef",
     "DisassociateCreatedArtifactRequestRequestTypeDef",
     "DisassociateDiscoveredResourceRequestRequestTypeDef",
     "ImportMigrationTaskRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
     "ListApplicationStatesRequestRequestTypeDef",
+    "ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
     "ListCreatedArtifactsRequestRequestTypeDef",
+    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
+    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
     "ListMigrationTasksRequestRequestTypeDef",
     "MigrationTaskSummaryTypeDef",
+    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
     "ListProgressUpdateStreamsRequestRequestTypeDef",
     "ProgressUpdateStreamSummaryTypeDef",
     "ResourceAttributeTypeDef",
     "TaskTypeDef",
     "NotifyApplicationStateRequestRequestTypeDef",
-    "AssociateCreatedArtifactRequestRequestTypeDef",
-    "AssociateDiscoveredResourceRequestRequestTypeDef",
-    "DescribeApplicationStateResultTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "ListApplicationStatesResultTypeDef",
+    "AssociateCreatedArtifactRequestRequestTypeDef",
     "ListCreatedArtifactsResultTypeDef",
+    "AssociateDiscoveredResourceRequestRequestTypeDef",
     "ListDiscoveredResourcesResultTypeDef",
-    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
-    "ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
-    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
-    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
     "ListMigrationTasksResultTypeDef",
     "ListProgressUpdateStreamsResultTypeDef",
     "PutResourceAttributesRequestRequestTypeDef",
     "MigrationTaskTypeDef",
     "NotifyMigrationTaskStateRequestRequestTypeDef",
     "DescribeMigrationTaskResultTypeDef",
 )
@@ -153,22 +153,20 @@
 DescribeApplicationStateRequestRequestTypeDef = TypedDict(
     "DescribeApplicationStateRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DescribeApplicationStateResultTypeDef = TypedDict(
+    "DescribeApplicationStateResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ApplicationStatus": ApplicationStatusType,
+        "LastUpdatedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMigrationTaskRequestRequestTypeDef = TypedDict(
     "DescribeMigrationTaskRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
@@ -237,34 +235,54 @@
 
 class ImportMigrationTaskRequestRequestTypeDef(
     _RequiredImportMigrationTaskRequestRequestTypeDef,
     _OptionalImportMigrationTaskRequestRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListApplicationStatesRequestListApplicationStatesPaginateTypeDef = TypedDict(
+    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ApplicationIds": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationStatesRequestRequestTypeDef = TypedDict(
     "ListApplicationStatesRequestRequestTypeDef",
     {
         "ApplicationIds": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
+    "_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
+    {
+        "ProgressUpdateStream": str,
+        "MigrationTaskName": str,
+    },
+)
+_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
+    "_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef(
+    _RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
+    _OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
+):
+    pass
+
 _RequiredListCreatedArtifactsRequestRequestTypeDef = TypedDict(
     "_RequiredListCreatedArtifactsRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
     },
 )
@@ -279,14 +297,35 @@
 
 class ListCreatedArtifactsRequestRequestTypeDef(
     _RequiredListCreatedArtifactsRequestRequestTypeDef,
     _OptionalListCreatedArtifactsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    {
+        "ProgressUpdateStream": str,
+        "MigrationTaskName": str,
+    },
+)
+_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
+    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+):
+    pass
+
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
     },
 )
@@ -301,14 +340,23 @@
 
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
+ListMigrationTasksRequestListMigrationTasksPaginateTypeDef = TypedDict(
+    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
+    {
+        "ResourceName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMigrationTasksRequestRequestTypeDef = TypedDict(
     "ListMigrationTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResourceName": str,
     },
@@ -324,14 +372,22 @@
         "ProgressPercent": int,
         "StatusDetail": str,
         "UpdateDateTime": datetime,
     },
     total=False,
 )
 
+ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef = TypedDict(
+    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProgressUpdateStreamsRequestRequestTypeDef = TypedDict(
     "ListProgressUpdateStreamsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -389,14 +445,44 @@
 
 class NotifyApplicationStateRequestRequestTypeDef(
     _RequiredNotifyApplicationStateRequestRequestTypeDef,
     _OptionalNotifyApplicationStateRequestRequestTypeDef,
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
+
+ListApplicationStatesResultTypeDef = TypedDict(
+    "ListApplicationStatesResultTypeDef",
+    {
+        "ApplicationStateList": List[ApplicationStateTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAssociateCreatedArtifactRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateCreatedArtifactRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
         "CreatedArtifact": CreatedArtifactTypeDef,
     },
@@ -411,14 +497,23 @@
 
 class AssociateCreatedArtifactRequestRequestTypeDef(
     _RequiredAssociateCreatedArtifactRequestRequestTypeDef,
     _OptionalAssociateCreatedArtifactRequestRequestTypeDef,
 ):
     pass
 
+ListCreatedArtifactsResultTypeDef = TypedDict(
+    "ListCreatedArtifactsResultTypeDef",
+    {
+        "NextToken": str,
+        "CreatedArtifactList": List[CreatedArtifactTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAssociateDiscoveredResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateDiscoveredResourceRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
         "DiscoveredResource": DiscoveredResourceTypeDef,
     },
@@ -433,133 +528,38 @@
 
 class AssociateDiscoveredResourceRequestRequestTypeDef(
     _RequiredAssociateDiscoveredResourceRequestRequestTypeDef,
     _OptionalAssociateDiscoveredResourceRequestRequestTypeDef,
 ):
     pass
 
-DescribeApplicationStateResultTypeDef = TypedDict(
-    "DescribeApplicationStateResultTypeDef",
-    {
-        "ApplicationStatus": ApplicationStatusType,
-        "LastUpdatedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationStatesResultTypeDef = TypedDict(
-    "ListApplicationStatesResultTypeDef",
-    {
-        "ApplicationStateList": List[ApplicationStateTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCreatedArtifactsResultTypeDef = TypedDict(
-    "ListCreatedArtifactsResultTypeDef",
-    {
-        "NextToken": str,
-        "CreatedArtifactList": List[CreatedArtifactTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListDiscoveredResourcesResultTypeDef = TypedDict(
     "ListDiscoveredResourcesResultTypeDef",
     {
         "NextToken": str,
         "DiscoveredResourceList": List[DiscoveredResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListApplicationStatesRequestListApplicationStatesPaginateTypeDef = TypedDict(
-    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
-    {
-        "ApplicationIds": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
-    "_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
-    {
-        "ProgressUpdateStream": str,
-        "MigrationTaskName": str,
-    },
-)
-_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
-    "_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef(
-    _RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
-    _OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
-):
-    pass
-
-_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "ProgressUpdateStream": str,
-        "MigrationTaskName": str,
-    },
-)
-_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
-    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-):
-    pass
-
-ListMigrationTasksRequestListMigrationTasksPaginateTypeDef = TypedDict(
-    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
-    {
-        "ResourceName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef = TypedDict(
-    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListMigrationTasksResultTypeDef = TypedDict(
     "ListMigrationTasksResultTypeDef",
     {
         "NextToken": str,
         "MigrationTaskSummaryList": List[MigrationTaskSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProgressUpdateStreamsResultTypeDef = TypedDict(
     "ListProgressUpdateStreamsResultTypeDef",
     {
         "ProgressUpdateStreamSummaryList": List[ProgressUpdateStreamSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutResourceAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourceAttributesRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
@@ -617,10 +617,10 @@
 ):
     pass
 
 DescribeMigrationTaskResultTypeDef = TypedDict(
     "DescribeMigrationTaskResultTypeDef",
     {
         "MigrationTask": MigrationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh.egg-info/PKG-INFO` & `mypy-boto3-mgh-1.27.0/mypy_boto3_mgh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgh
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.MigrationHub 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.MigrationHub 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/
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
 
 <a id="mypy-boto3-mgh"></a>
 
 # mypy-boto3-mgh
 
 [![PyPI - mypy-boto3-mgh](https://img.shields.io/pypi/v/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mgh?color=blue)](https://pypistats.org/packages/mypy-boto3-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHub 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[boto3.MigrationHub 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
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
 [mypy-boto3-mgh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,41 +350,41 @@
 from mypy_boto3_mgh.type_defs import (
     ApplicationStateTypeDef,
     CreatedArtifactTypeDef,
     DiscoveredResourceTypeDef,
     CreateProgressUpdateStreamRequestRequestTypeDef,
     DeleteProgressUpdateStreamRequestRequestTypeDef,
     DescribeApplicationStateRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeApplicationStateResultTypeDef,
     DescribeMigrationTaskRequestRequestTypeDef,
     DisassociateCreatedArtifactRequestRequestTypeDef,
     DisassociateDiscoveredResourceRequestRequestTypeDef,
     ImportMigrationTaskRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
     ListApplicationStatesRequestRequestTypeDef,
+    ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
     ListCreatedArtifactsRequestRequestTypeDef,
+    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
+    ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
     ListMigrationTasksRequestRequestTypeDef,
     MigrationTaskSummaryTypeDef,
+    ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListProgressUpdateStreamsRequestRequestTypeDef,
     ProgressUpdateStreamSummaryTypeDef,
     ResourceAttributeTypeDef,
     TaskTypeDef,
     NotifyApplicationStateRequestRequestTypeDef,
-    AssociateCreatedArtifactRequestRequestTypeDef,
-    AssociateDiscoveredResourceRequestRequestTypeDef,
-    DescribeApplicationStateResultTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     ListApplicationStatesResultTypeDef,
+    AssociateCreatedArtifactRequestRequestTypeDef,
     ListCreatedArtifactsResultTypeDef,
+    AssociateDiscoveredResourceRequestRequestTypeDef,
     ListDiscoveredResourcesResultTypeDef,
-    ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
-    ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
-    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-    ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
-    ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListMigrationTasksResultTypeDef,
     ListProgressUpdateStreamsResultTypeDef,
     PutResourceAttributesRequestRequestTypeDef,
     MigrationTaskTypeDef,
     NotifyMigrationTaskStateRequestRequestTypeDef,
     DescribeMigrationTaskResultTypeDef,
 )
@@ -396,42 +397,42 @@
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

### Comparing `mypy-boto3-mgh-1.26.0.post1/mypy_boto3_mgh.egg-info/SOURCES.txt` & `mypy-boto3-mgh-1.27.0/mypy_boto3_mgh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.26.0.post1/setup.py` & `mypy-boto3-mgh-1.27.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-mgh.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mgh",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_mgh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHub 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.MigrationHub 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 mgh type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_mgh": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_mgh": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/",
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


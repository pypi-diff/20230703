# Comparing `tmp/mypy-boto3-iot1click-projects-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-iot1click-projects-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot1click-projects-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:32 2022, max compression
+gzip compressed data, was "mypy-boto3-iot1click-projects-1.27.0.tar", last modified: Mon Jul  3 19:50:52 2023, max compression
```

## Comparing `mypy-boto3-iot1click-projects-1.26.0.post1.tar` & `mypy-boto3-iot1click-projects-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:32.676828 mypy-boto3-iot1click-projects-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14484 2022-11-01 21:43:32.676828 mypy-boto3-iot1click-projects-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13000 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:32.676828 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      959 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13289 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    13264 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7328 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7326 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3028 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    10864 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    10847 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:32.676828 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14484 2022-11-01 21:43:32.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-11-01 21:43:32.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:32.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:32.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:32.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-01 21:43:32.000000 mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:32.676828 mypy-boto3-iot1click-projects-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2068 2022-11-01 21:36:05.000000 mypy-boto3-iot1click-projects-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.711400 mypy-boto3-iot1click-projects-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-03 19:50:52.711400 mypy-boto3-iot1click-projects-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.711400 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.711400 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-03 19:50:52.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-03 19:50:52.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:52.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:52.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:52.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 19:50:52.000000 mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:52.711400 mypy-boto3-iot1click-projects-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-03 19:39:33.000000 mypy-boto3-iot1click-projects-1.27.0/setup.py
```

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/LICENSE` & `mypy-boto3-iot1click-projects-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/PKG-INFO` & `mypy-boto3-iot1click-projects-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-projects
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IoT1ClickProjects 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.IoT1ClickProjects 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/
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
 
 <a id="mypy-boto3-iot1click-projects"></a>
 
 # mypy-boto3-iot1click-projects
 
 [![PyPI - mypy-boto3-iot1click-projects](https://img.shields.io/pypi/v/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot1click-projects?color=blue)](https://pypistats.org/packages/mypy-boto3-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickProjects 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[boto3.IoT1ClickProjects 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
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
 [mypy-boto3-iot1click-projects docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,34 +328,34 @@
 from mypy_boto3_iot1click_projects.type_defs import (
     AssociateDeviceWithPlacementRequestRequestTypeDef,
     CreatePlacementRequestRequestTypeDef,
     DeletePlacementRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DescribePlacementRequestRequestTypeDef,
     PlacementDescriptionTypeDef,
-    ResponseMetadataTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DeviceTemplateTypeDef,
     DisassociateDeviceFromPlacementRequestRequestTypeDef,
     GetDevicesInPlacementRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetDevicesInPlacementResponseTypeDef,
+    ListPlacementsRequestListPlacementsPaginateTypeDef,
     ListPlacementsRequestRequestTypeDef,
     PlacementSummaryTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePlacementRequestRequestTypeDef,
     DescribePlacementResponseTypeDef,
-    GetDevicesInPlacementResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PlacementTemplateTypeDef,
-    ListPlacementsRequestListPlacementsPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectDescriptionTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
 )
@@ -367,42 +368,42 @@
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

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/README.md` & `mypy-boto3-iot1click-projects-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iot1click-projects"></a>
 
 # mypy-boto3-iot1click-projects
 
 [![PyPI - mypy-boto3-iot1click-projects](https://img.shields.io/pypi/v/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot1click-projects?color=blue)](https://pypistats.org/packages/mypy-boto3-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickProjects 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[boto3.IoT1ClickProjects 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
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
 [mypy-boto3-iot1click-projects docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,34 +296,34 @@
 from mypy_boto3_iot1click_projects.type_defs import (
     AssociateDeviceWithPlacementRequestRequestTypeDef,
     CreatePlacementRequestRequestTypeDef,
     DeletePlacementRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DescribePlacementRequestRequestTypeDef,
     PlacementDescriptionTypeDef,
-    ResponseMetadataTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DeviceTemplateTypeDef,
     DisassociateDeviceFromPlacementRequestRequestTypeDef,
     GetDevicesInPlacementRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetDevicesInPlacementResponseTypeDef,
+    ListPlacementsRequestListPlacementsPaginateTypeDef,
     ListPlacementsRequestRequestTypeDef,
     PlacementSummaryTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePlacementRequestRequestTypeDef,
     DescribePlacementResponseTypeDef,
-    GetDevicesInPlacementResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PlacementTemplateTypeDef,
-    ListPlacementsRequestListPlacementsPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectDescriptionTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
 )
@@ -336,42 +336,42 @@
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

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/__init__.py` & `mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/__init__.pyi` & `mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/__main__.py` & `mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoT1ClickProjects 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.IoT1ClickProjects 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects\nOther"
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

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/client.py` & `mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/client.pyi` & `mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/literals.py` & `mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,23 +44,25 @@
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
@@ -70,30 +72,35 @@
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
@@ -119,14 +126,15 @@
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
@@ -171,51 +179,57 @@
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
@@ -228,14 +242,15 @@
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
@@ -247,28 +262,35 @@
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
@@ -277,14 +299,15 @@
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
@@ -295,55 +318,64 @@
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

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/literals.pyi` & `mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -42,23 +42,25 @@
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
@@ -68,30 +70,35 @@
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
@@ -117,14 +124,15 @@
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
@@ -169,51 +177,57 @@
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
@@ -226,14 +240,15 @@
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
@@ -245,28 +260,35 @@
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
@@ -275,14 +297,15 @@
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
@@ -293,55 +316,64 @@
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

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/paginator.py` & `mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 class ListPlacementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListPlacements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listplacementspaginator)
     """
 
     def paginate(
-        self, *, projectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, projectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPlacementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListPlacements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listplacementspaginator)
         """
 
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listprojectspaginator)
         """
```

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/paginator.pyi` & `mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 class ListPlacementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListPlacements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listplacementspaginator)
     """
 
     def paginate(
-        self, *, projectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, projectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPlacementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListPlacements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listplacementspaginator)
         """
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listprojectspaginator)
         """
```

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/type_defs.py` & `mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -16,42 +16,41 @@
 from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     "CreatePlacementRequestRequestTypeDef",
     "DeletePlacementRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DescribePlacementRequestRequestTypeDef",
     "PlacementDescriptionTypeDef",
-    "ResponseMetadataTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DeviceTemplateTypeDef",
     "DisassociateDeviceFromPlacementRequestRequestTypeDef",
     "GetDevicesInPlacementRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetDevicesInPlacementResponseTypeDef",
+    "ListPlacementsRequestListPlacementsPaginateTypeDef",
     "ListPlacementsRequestRequestTypeDef",
     "PlacementSummaryTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePlacementRequestRequestTypeDef",
     "DescribePlacementResponseTypeDef",
-    "GetDevicesInPlacementResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PlacementTemplateTypeDef",
-    "ListPlacementsRequestListPlacementsPaginateTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListPlacementsResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectDescriptionTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
 )
@@ -77,21 +76,19 @@
     "_OptionalCreatePlacementRequestRequestTypeDef",
     {
         "attributes": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreatePlacementRequestRequestTypeDef(
     _RequiredCreatePlacementRequestRequestTypeDef, _OptionalCreatePlacementRequestRequestTypeDef
 ):
     pass
 
-
 DeletePlacementRequestRequestTypeDef = TypedDict(
     "DeletePlacementRequestRequestTypeDef",
     {
         "placementName": str,
         "projectName": str,
     },
 )
@@ -118,25 +115,14 @@
         "placementName": str,
         "attributes": Dict[str, str],
         "createdDate": datetime,
         "updatedDate": datetime,
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
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
@@ -162,24 +148,42 @@
     "GetDevicesInPlacementRequestRequestTypeDef",
     {
         "projectName": str,
         "placementName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetDevicesInPlacementResponseTypeDef = TypedDict(
+    "GetDevicesInPlacementResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "devices": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
+    "_RequiredListPlacementsRequestListPlacementsPaginateTypeDef",
+    {
+        "projectName": str,
+    },
+)
+_OptionalListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
+    "_OptionalListPlacementsRequestListPlacementsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListPlacementsRequestListPlacementsPaginateTypeDef(
+    _RequiredListPlacementsRequestListPlacementsPaginateTypeDef,
+    _OptionalListPlacementsRequestListPlacementsPaginateTypeDef,
+):
+    pass
+
 _RequiredListPlacementsRequestRequestTypeDef = TypedDict(
     "_RequiredListPlacementsRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalListPlacementsRequestRequestTypeDef = TypedDict(
@@ -187,31 +191,37 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListPlacementsRequestRequestTypeDef(
     _RequiredListPlacementsRequestRequestTypeDef, _OptionalListPlacementsRequestRequestTypeDef
 ):
     pass
 
-
 PlacementSummaryTypeDef = TypedDict(
     "PlacementSummaryTypeDef",
     {
         "projectName": str,
         "placementName": str,
         "createdDate": datetime,
         "updatedDate": datetime,
     },
 )
 
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -230,26 +240,53 @@
     {
         "arn": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
     pass
 
-
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -273,99 +310,51 @@
     "_OptionalUpdatePlacementRequestRequestTypeDef",
     {
         "attributes": Mapping[str, str],
     },
     total=False,
 )
 
-
 class UpdatePlacementRequestRequestTypeDef(
     _RequiredUpdatePlacementRequestRequestTypeDef, _OptionalUpdatePlacementRequestRequestTypeDef
 ):
     pass
 
-
 DescribePlacementResponseTypeDef = TypedDict(
     "DescribePlacementResponseTypeDef",
     {
         "placement": PlacementDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDevicesInPlacementResponseTypeDef = TypedDict(
-    "GetDevicesInPlacementResponseTypeDef",
-    {
-        "devices": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PlacementTemplateTypeDef = TypedDict(
     "PlacementTemplateTypeDef",
     {
         "defaultAttributes": Mapping[str, str],
         "deviceTemplates": Mapping[str, DeviceTemplateTypeDef],
     },
     total=False,
 )
 
-_RequiredListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
-    "_RequiredListPlacementsRequestListPlacementsPaginateTypeDef",
-    {
-        "projectName": str,
-    },
-)
-_OptionalListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
-    "_OptionalListPlacementsRequestListPlacementsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPlacementsRequestListPlacementsPaginateTypeDef(
-    _RequiredListPlacementsRequestListPlacementsPaginateTypeDef,
-    _OptionalListPlacementsRequestListPlacementsPaginateTypeDef,
-):
-    pass
-
-
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListPlacementsResponseTypeDef = TypedDict(
     "ListPlacementsResponseTypeDef",
     {
         "placements": List[PlacementSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "projectName": str,
@@ -377,21 +366,19 @@
         "description": str,
         "placementTemplate": PlacementTemplateTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredProjectDescriptionTypeDef = TypedDict(
     "_RequiredProjectDescriptionTypeDef",
     {
         "projectName": str,
         "createdDate": datetime,
         "updatedDate": datetime,
     },
@@ -403,21 +390,19 @@
         "description": str,
         "placementTemplate": PlacementTemplateTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class ProjectDescriptionTypeDef(
     _RequiredProjectDescriptionTypeDef, _OptionalProjectDescriptionTypeDef
 ):
     pass
 
-
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
@@ -425,21 +410,19 @@
     {
         "description": str,
         "placementTemplate": PlacementTemplateTypeDef,
     },
     total=False,
 )
 
-
 class UpdateProjectRequestRequestTypeDef(
     _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
 ):
     pass
 
-
 DescribeProjectResponseTypeDef = TypedDict(
     "DescribeProjectResponseTypeDef",
     {
         "project": ProjectDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects/type_defs.pyi` & `mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,41 +16,42 @@
 from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     "CreatePlacementRequestRequestTypeDef",
     "DeletePlacementRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DescribePlacementRequestRequestTypeDef",
     "PlacementDescriptionTypeDef",
-    "ResponseMetadataTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DeviceTemplateTypeDef",
     "DisassociateDeviceFromPlacementRequestRequestTypeDef",
     "GetDevicesInPlacementRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetDevicesInPlacementResponseTypeDef",
+    "ListPlacementsRequestListPlacementsPaginateTypeDef",
     "ListPlacementsRequestRequestTypeDef",
     "PlacementSummaryTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePlacementRequestRequestTypeDef",
     "DescribePlacementResponseTypeDef",
-    "GetDevicesInPlacementResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PlacementTemplateTypeDef",
-    "ListPlacementsRequestListPlacementsPaginateTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListPlacementsResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectDescriptionTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
 )
@@ -76,19 +77,21 @@
     "_OptionalCreatePlacementRequestRequestTypeDef",
     {
         "attributes": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreatePlacementRequestRequestTypeDef(
     _RequiredCreatePlacementRequestRequestTypeDef, _OptionalCreatePlacementRequestRequestTypeDef
 ):
     pass
 
+
 DeletePlacementRequestRequestTypeDef = TypedDict(
     "DeletePlacementRequestRequestTypeDef",
     {
         "placementName": str,
         "projectName": str,
     },
 )
@@ -115,25 +118,14 @@
         "placementName": str,
         "attributes": Dict[str, str],
         "createdDate": datetime,
         "updatedDate": datetime,
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
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
@@ -159,24 +151,44 @@
     "GetDevicesInPlacementRequestRequestTypeDef",
     {
         "projectName": str,
         "placementName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetDevicesInPlacementResponseTypeDef = TypedDict(
+    "GetDevicesInPlacementResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "devices": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
+    "_RequiredListPlacementsRequestListPlacementsPaginateTypeDef",
+    {
+        "projectName": str,
+    },
+)
+_OptionalListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
+    "_OptionalListPlacementsRequestListPlacementsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListPlacementsRequestListPlacementsPaginateTypeDef(
+    _RequiredListPlacementsRequestListPlacementsPaginateTypeDef,
+    _OptionalListPlacementsRequestListPlacementsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPlacementsRequestRequestTypeDef = TypedDict(
     "_RequiredListPlacementsRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalListPlacementsRequestRequestTypeDef = TypedDict(
@@ -184,29 +196,39 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListPlacementsRequestRequestTypeDef(
     _RequiredListPlacementsRequestRequestTypeDef, _OptionalListPlacementsRequestRequestTypeDef
 ):
     pass
 
+
 PlacementSummaryTypeDef = TypedDict(
     "PlacementSummaryTypeDef",
     {
         "projectName": str,
         "placementName": str,
         "createdDate": datetime,
         "updatedDate": datetime,
     },
 )
 
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -225,24 +247,55 @@
     {
         "arn": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
     pass
 
+
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -266,95 +319,53 @@
     "_OptionalUpdatePlacementRequestRequestTypeDef",
     {
         "attributes": Mapping[str, str],
     },
     total=False,
 )
 
+
 class UpdatePlacementRequestRequestTypeDef(
     _RequiredUpdatePlacementRequestRequestTypeDef, _OptionalUpdatePlacementRequestRequestTypeDef
 ):
     pass
 
+
 DescribePlacementResponseTypeDef = TypedDict(
     "DescribePlacementResponseTypeDef",
     {
         "placement": PlacementDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDevicesInPlacementResponseTypeDef = TypedDict(
-    "GetDevicesInPlacementResponseTypeDef",
-    {
-        "devices": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PlacementTemplateTypeDef = TypedDict(
     "PlacementTemplateTypeDef",
     {
         "defaultAttributes": Mapping[str, str],
         "deviceTemplates": Mapping[str, DeviceTemplateTypeDef],
     },
     total=False,
 )
 
-_RequiredListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
-    "_RequiredListPlacementsRequestListPlacementsPaginateTypeDef",
-    {
-        "projectName": str,
-    },
-)
-_OptionalListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
-    "_OptionalListPlacementsRequestListPlacementsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListPlacementsRequestListPlacementsPaginateTypeDef(
-    _RequiredListPlacementsRequestListPlacementsPaginateTypeDef,
-    _OptionalListPlacementsRequestListPlacementsPaginateTypeDef,
-):
-    pass
-
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListPlacementsResponseTypeDef = TypedDict(
     "ListPlacementsResponseTypeDef",
     {
         "placements": List[PlacementSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "projectName": str,
@@ -366,19 +377,21 @@
         "description": str,
         "placementTemplate": PlacementTemplateTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredProjectDescriptionTypeDef = TypedDict(
     "_RequiredProjectDescriptionTypeDef",
     {
         "projectName": str,
         "createdDate": datetime,
         "updatedDate": datetime,
     },
@@ -390,19 +403,21 @@
         "description": str,
         "placementTemplate": PlacementTemplateTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class ProjectDescriptionTypeDef(
     _RequiredProjectDescriptionTypeDef, _OptionalProjectDescriptionTypeDef
 ):
     pass
 
+
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
@@ -410,19 +425,21 @@
     {
         "description": str,
         "placementTemplate": PlacementTemplateTypeDef,
     },
     total=False,
 )
 
+
 class UpdateProjectRequestRequestTypeDef(
     _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
 ):
     pass
 
+
 DescribeProjectResponseTypeDef = TypedDict(
     "DescribeProjectResponseTypeDef",
     {
         "project": ProjectDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects.egg-info/PKG-INFO` & `mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-projects
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IoT1ClickProjects 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.IoT1ClickProjects 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/
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
 
 <a id="mypy-boto3-iot1click-projects"></a>
 
 # mypy-boto3-iot1click-projects
 
 [![PyPI - mypy-boto3-iot1click-projects](https://img.shields.io/pypi/v/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot1click-projects?color=blue)](https://pypistats.org/packages/mypy-boto3-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickProjects 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[boto3.IoT1ClickProjects 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
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
 [mypy-boto3-iot1click-projects docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,34 +328,34 @@
 from mypy_boto3_iot1click_projects.type_defs import (
     AssociateDeviceWithPlacementRequestRequestTypeDef,
     CreatePlacementRequestRequestTypeDef,
     DeletePlacementRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DescribePlacementRequestRequestTypeDef,
     PlacementDescriptionTypeDef,
-    ResponseMetadataTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DeviceTemplateTypeDef,
     DisassociateDeviceFromPlacementRequestRequestTypeDef,
     GetDevicesInPlacementRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetDevicesInPlacementResponseTypeDef,
+    ListPlacementsRequestListPlacementsPaginateTypeDef,
     ListPlacementsRequestRequestTypeDef,
     PlacementSummaryTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePlacementRequestRequestTypeDef,
     DescribePlacementResponseTypeDef,
-    GetDevicesInPlacementResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PlacementTemplateTypeDef,
-    ListPlacementsRequestListPlacementsPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectDescriptionTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
 )
@@ -367,42 +368,42 @@
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

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt` & `mypy-boto3-iot1click-projects-1.27.0/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.26.0.post1/setup.py` & `mypy-boto3-iot1click-projects-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 """
 Setup script for mypy-boto3-iot1click-projects.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot1click-projects",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_iot1click_projects"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoT1ClickProjects 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.IoT1ClickProjects 1.27.0 service generated with"
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
     keywords="boto3 iot1click-projects type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_iot1click_projects": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_iot1click_projects": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/"
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


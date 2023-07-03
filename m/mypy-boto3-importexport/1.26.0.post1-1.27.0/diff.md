# Comparing `tmp/mypy-boto3-importexport-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-importexport-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-importexport-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:32 2022, max compression
+gzip compressed data, was "mypy-boto3-importexport-1.27.0.tar", last modified: Mon Jul  3 19:50:52 2023, max compression
```

## Comparing `mypy-boto3-importexport-1.26.0.post1.tar` & `mypy-boto3-importexport-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:32.204827 mypy-boto3-importexport-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13196 2022-11-01 21:43:32.200827 mypy-boto3-importexport-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11735 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:32.196828 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8689 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     8675 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7018 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7016 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     6577 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6566 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:32.200827 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13196 2022-11-01 21:43:32.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-11-01 21:43:32.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:32.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:32.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:32.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-01 21:43:32.000000 mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:32.204827 mypy-boto3-importexport-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-11-01 21:35:47.000000 mypy-boto3-importexport-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.319393 mypy-boto3-importexport-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:07.000000 mypy-boto3-importexport-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-07-03 19:50:52.315393 mypy-boto3-importexport-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-07-03 19:39:07.000000 mypy-boto3-importexport-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.315393 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-03 19:39:07.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-03 19:39:07.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:39:07.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-07-03 19:39:07.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-07-03 19:39:07.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-03 19:39:08.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-07-03 19:39:07.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-03 19:39:07.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-03 19:39:07.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:07.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-07-03 19:39:08.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-03 19:39:08.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:07.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.315393 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-07-03 19:50:52.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:50:52.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:52.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:52.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:52.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:52.000000 mypy-boto3-importexport-1.27.0/mypy_boto3_importexport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:52.319393 mypy-boto3-importexport-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:39:07.000000 mypy-boto3-importexport-1.27.0/setup.py
```

### Comparing `mypy-boto3-importexport-1.26.0.post1/LICENSE` & `mypy-boto3-importexport-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-importexport-1.26.0.post1/PKG-INFO` & `mypy-boto3-importexport-1.27.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,60 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-importexport
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ImportExport 1.26.0 service generated with mypy-boto3-builder 7.11.10
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 importexport type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-importexport"></a>
 
 # mypy-boto3-importexport
 
 [![PyPI - mypy-boto3-importexport](https://img.shields.io/pypi/v/mypy-boto3-importexport.svg?color=blue)](https://pypi.org/project/mypy-boto3-importexport)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-importexport.svg?color=blue)](https://pypi.org/project/mypy-boto3-importexport)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-importexport?color=blue)](https://pypistats.org/packages/mypy-boto3-importexport)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ImportExport 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
+[boto3.ImportExport 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
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
 [mypy-boto3-importexport docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,71 +289,71 @@
 `mypy_boto3_importexport.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_importexport.type_defs import (
     ArtifactTypeDef,
     CancelJobInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJobOutputTypeDef,
     CreateJobInputRequestTypeDef,
     GetShippingLabelInputRequestTypeDef,
+    GetShippingLabelOutputTypeDef,
     GetStatusInputRequestTypeDef,
     JobTypeDef,
-    PaginatorConfigTypeDef,
+    ListJobsInputListJobsPaginateTypeDef,
     ListJobsInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UpdateJobInputRequestTypeDef,
-    CancelJobOutputTypeDef,
     CreateJobOutputTypeDef,
-    GetShippingLabelOutputTypeDef,
     GetStatusOutputTypeDef,
     UpdateJobOutputTypeDef,
     ListJobsOutputTypeDef,
-    ListJobsInputListJobsPaginateTypeDef,
 )
 
 
 def get_structure() -> ArtifactTypeDef:
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

### Comparing `mypy-boto3-importexport-1.26.0.post1/README.md` & `mypy-boto3-importexport-1.27.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-importexport
+Version: 1.27.0
+Summary: Type annotations for boto3.ImportExport 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 importexport type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-importexport"></a>
 
 # mypy-boto3-importexport
 
 [![PyPI - mypy-boto3-importexport](https://img.shields.io/pypi/v/mypy-boto3-importexport.svg?color=blue)](https://pypi.org/project/mypy-boto3-importexport)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-importexport.svg?color=blue)](https://pypi.org/project/mypy-boto3-importexport)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-importexport?color=blue)](https://pypistats.org/packages/mypy-boto3-importexport)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ImportExport 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
+[boto3.ImportExport 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
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
 [mypy-boto3-importexport docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,71 +321,71 @@
 `mypy_boto3_importexport.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_importexport.type_defs import (
     ArtifactTypeDef,
     CancelJobInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJobOutputTypeDef,
     CreateJobInputRequestTypeDef,
     GetShippingLabelInputRequestTypeDef,
+    GetShippingLabelOutputTypeDef,
     GetStatusInputRequestTypeDef,
     JobTypeDef,
-    PaginatorConfigTypeDef,
+    ListJobsInputListJobsPaginateTypeDef,
     ListJobsInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UpdateJobInputRequestTypeDef,
-    CancelJobOutputTypeDef,
     CreateJobOutputTypeDef,
-    GetShippingLabelOutputTypeDef,
     GetStatusOutputTypeDef,
     UpdateJobOutputTypeDef,
     ListJobsOutputTypeDef,
-    ListJobsInputListJobsPaginateTypeDef,
 )
 
 
 def get_structure() -> ArtifactTypeDef:
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

### Comparing `mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/__init__.py` & `mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/__init__.pyi` & `mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/__main__.py` & `mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ImportExport 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.ImportExport 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport\nOther"
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

### Comparing `mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/client.py` & `mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/client.pyi` & `mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/literals.py` & `mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,23 +43,25 @@
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
@@ -69,30 +71,35 @@
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
@@ -118,14 +125,15 @@
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
@@ -170,51 +178,57 @@
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
@@ -227,14 +241,15 @@
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
@@ -246,28 +261,35 @@
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
@@ -276,14 +298,15 @@
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
@@ -294,55 +317,64 @@
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

### Comparing `mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/literals.pyi` & `mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -41,23 +41,25 @@
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
@@ -67,30 +69,35 @@
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
@@ -116,14 +123,15 @@
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
@@ -168,51 +176,57 @@
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
@@ -225,14 +239,15 @@
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
@@ -244,28 +259,35 @@
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
@@ -274,14 +296,15 @@
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
@@ -292,55 +315,64 @@
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

### Comparing `mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/paginator.py` & `mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, APIVersion: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, APIVersion: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/paginators/#listjobspaginator)
         """
```

### Comparing `mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/paginator.pyi` & `mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, APIVersion: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, APIVersion: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/paginators/#listjobspaginator)
         """
```

### Comparing `mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/type_defs.py` & `mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -18,33 +18,32 @@
 from .literals import JobTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ArtifactTypeDef",
     "CancelJobInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelJobOutputTypeDef",
     "CreateJobInputRequestTypeDef",
     "GetShippingLabelInputRequestTypeDef",
+    "GetShippingLabelOutputTypeDef",
     "GetStatusInputRequestTypeDef",
     "JobTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListJobsInputListJobsPaginateTypeDef",
     "ListJobsInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateJobInputRequestTypeDef",
-    "CancelJobOutputTypeDef",
     "CreateJobOutputTypeDef",
-    "GetShippingLabelOutputTypeDef",
     "GetStatusOutputTypeDef",
     "UpdateJobOutputTypeDef",
     "ListJobsOutputTypeDef",
-    "ListJobsInputListJobsPaginateTypeDef",
 )
 
 ArtifactTypeDef = TypedDict(
     "ArtifactTypeDef",
     {
         "Description": str,
         "URL": str,
@@ -62,29 +61,24 @@
     "_OptionalCancelJobInputRequestTypeDef",
     {
         "APIVersion": str,
     },
     total=False,
 )
 
-
 class CancelJobInputRequestTypeDef(
     _RequiredCancelJobInputRequestTypeDef, _OptionalCancelJobInputRequestTypeDef
 ):
     pass
 
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelJobOutputTypeDef = TypedDict(
+    "CancelJobOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Success": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateJobInputRequestTypeDef = TypedDict(
     "_RequiredCreateJobInputRequestTypeDef",
     {
         "JobType": JobTypeType,
@@ -97,21 +91,19 @@
     {
         "ManifestAddendum": str,
         "APIVersion": str,
     },
     total=False,
 )
 
-
 class CreateJobInputRequestTypeDef(
     _RequiredCreateJobInputRequestTypeDef, _OptionalCreateJobInputRequestTypeDef
 ):
     pass
 
-
 _RequiredGetShippingLabelInputRequestTypeDef = TypedDict(
     "_RequiredGetShippingLabelInputRequestTypeDef",
     {
         "jobIds": Sequence[str],
     },
 )
 _OptionalGetShippingLabelInputRequestTypeDef = TypedDict(
@@ -128,20 +120,27 @@
         "street2": str,
         "street3": str,
         "APIVersion": str,
     },
     total=False,
 )
 
-
 class GetShippingLabelInputRequestTypeDef(
     _RequiredGetShippingLabelInputRequestTypeDef, _OptionalGetShippingLabelInputRequestTypeDef
 ):
     pass
 
+GetShippingLabelOutputTypeDef = TypedDict(
+    "GetShippingLabelOutputTypeDef",
+    {
+        "ShippingLabelURL": str,
+        "Warning": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredGetStatusInputRequestTypeDef = TypedDict(
     "_RequiredGetStatusInputRequestTypeDef",
     {
         "JobId": str,
     },
 )
@@ -149,52 +148,70 @@
     "_OptionalGetStatusInputRequestTypeDef",
     {
         "APIVersion": str,
     },
     total=False,
 )
 
-
 class GetStatusInputRequestTypeDef(
     _RequiredGetStatusInputRequestTypeDef, _OptionalGetStatusInputRequestTypeDef
 ):
     pass
 
-
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "JobId": str,
         "CreationDate": datetime,
         "IsCanceled": bool,
         "JobType": JobTypeType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListJobsInputListJobsPaginateTypeDef = TypedDict(
+    "ListJobsInputListJobsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "APIVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListJobsInputRequestTypeDef = TypedDict(
     "ListJobsInputRequestTypeDef",
     {
         "MaxJobs": int,
         "Marker": str,
         "APIVersion": str,
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
 _RequiredUpdateJobInputRequestTypeDef = TypedDict(
     "_RequiredUpdateJobInputRequestTypeDef",
     {
         "JobId": str,
         "Manifest": str,
         "JobType": JobTypeType,
         "ValidateOnly": bool,
@@ -204,48 +221,29 @@
     "_OptionalUpdateJobInputRequestTypeDef",
     {
         "APIVersion": str,
     },
     total=False,
 )
 
-
 class UpdateJobInputRequestTypeDef(
     _RequiredUpdateJobInputRequestTypeDef, _OptionalUpdateJobInputRequestTypeDef
 ):
     pass
 
-
-CancelJobOutputTypeDef = TypedDict(
-    "CancelJobOutputTypeDef",
-    {
-        "Success": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateJobOutputTypeDef = TypedDict(
     "CreateJobOutputTypeDef",
     {
         "JobId": str,
         "JobType": JobTypeType,
         "Signature": str,
         "SignatureFileContents": str,
         "WarningMessage": str,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetShippingLabelOutputTypeDef = TypedDict(
-    "GetShippingLabelOutputTypeDef",
-    {
-        "ShippingLabelURL": str,
-        "Warning": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStatusOutputTypeDef = TypedDict(
     "GetStatusOutputTypeDef",
     {
         "JobId": str,
@@ -260,38 +258,29 @@
         "LogKey": str,
         "ErrorCount": int,
         "Signature": str,
         "SignatureFileContents": str,
         "CurrentManifest": str,
         "CreationDate": datetime,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateJobOutputTypeDef = TypedDict(
     "UpdateJobOutputTypeDef",
     {
         "Success": bool,
         "WarningMessage": str,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsOutputTypeDef = TypedDict(
     "ListJobsOutputTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "IsTruncated": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-
-ListJobsInputListJobsPaginateTypeDef = TypedDict(
-    "ListJobsInputListJobsPaginateTypeDef",
-    {
-        "APIVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
```

### Comparing `mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport/type_defs.pyi` & `mypy-boto3-importexport-1.27.0/mypy_boto3_importexport/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,32 +18,33 @@
 from .literals import JobTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ArtifactTypeDef",
     "CancelJobInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelJobOutputTypeDef",
     "CreateJobInputRequestTypeDef",
     "GetShippingLabelInputRequestTypeDef",
+    "GetShippingLabelOutputTypeDef",
     "GetStatusInputRequestTypeDef",
     "JobTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListJobsInputListJobsPaginateTypeDef",
     "ListJobsInputRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateJobInputRequestTypeDef",
-    "CancelJobOutputTypeDef",
     "CreateJobOutputTypeDef",
-    "GetShippingLabelOutputTypeDef",
     "GetStatusOutputTypeDef",
     "UpdateJobOutputTypeDef",
     "ListJobsOutputTypeDef",
-    "ListJobsInputListJobsPaginateTypeDef",
 )
 
 ArtifactTypeDef = TypedDict(
     "ArtifactTypeDef",
     {
         "Description": str,
         "URL": str,
@@ -61,27 +62,26 @@
     "_OptionalCancelJobInputRequestTypeDef",
     {
         "APIVersion": str,
     },
     total=False,
 )
 
+
 class CancelJobInputRequestTypeDef(
     _RequiredCancelJobInputRequestTypeDef, _OptionalCancelJobInputRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+CancelJobOutputTypeDef = TypedDict(
+    "CancelJobOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Success": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateJobInputRequestTypeDef = TypedDict(
     "_RequiredCreateJobInputRequestTypeDef",
     {
         "JobType": JobTypeType,
@@ -94,19 +94,21 @@
     {
         "ManifestAddendum": str,
         "APIVersion": str,
     },
     total=False,
 )
 
+
 class CreateJobInputRequestTypeDef(
     _RequiredCreateJobInputRequestTypeDef, _OptionalCreateJobInputRequestTypeDef
 ):
     pass
 
+
 _RequiredGetShippingLabelInputRequestTypeDef = TypedDict(
     "_RequiredGetShippingLabelInputRequestTypeDef",
     {
         "jobIds": Sequence[str],
     },
 )
 _OptionalGetShippingLabelInputRequestTypeDef = TypedDict(
@@ -123,69 +125,102 @@
         "street2": str,
         "street3": str,
         "APIVersion": str,
     },
     total=False,
 )
 
+
 class GetShippingLabelInputRequestTypeDef(
     _RequiredGetShippingLabelInputRequestTypeDef, _OptionalGetShippingLabelInputRequestTypeDef
 ):
     pass
 
+
+GetShippingLabelOutputTypeDef = TypedDict(
+    "GetShippingLabelOutputTypeDef",
+    {
+        "ShippingLabelURL": str,
+        "Warning": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetStatusInputRequestTypeDef = TypedDict(
     "_RequiredGetStatusInputRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetStatusInputRequestTypeDef = TypedDict(
     "_OptionalGetStatusInputRequestTypeDef",
     {
         "APIVersion": str,
     },
     total=False,
 )
 
+
 class GetStatusInputRequestTypeDef(
     _RequiredGetStatusInputRequestTypeDef, _OptionalGetStatusInputRequestTypeDef
 ):
     pass
 
+
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "JobId": str,
         "CreationDate": datetime,
         "IsCanceled": bool,
         "JobType": JobTypeType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListJobsInputListJobsPaginateTypeDef = TypedDict(
+    "ListJobsInputListJobsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "APIVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListJobsInputRequestTypeDef = TypedDict(
     "ListJobsInputRequestTypeDef",
     {
         "MaxJobs": int,
         "Marker": str,
         "APIVersion": str,
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
 _RequiredUpdateJobInputRequestTypeDef = TypedDict(
     "_RequiredUpdateJobInputRequestTypeDef",
     {
         "JobId": str,
         "Manifest": str,
         "JobType": JobTypeType,
         "ValidateOnly": bool,
@@ -195,46 +230,31 @@
     "_OptionalUpdateJobInputRequestTypeDef",
     {
         "APIVersion": str,
     },
     total=False,
 )
 
+
 class UpdateJobInputRequestTypeDef(
     _RequiredUpdateJobInputRequestTypeDef, _OptionalUpdateJobInputRequestTypeDef
 ):
     pass
 
-CancelJobOutputTypeDef = TypedDict(
-    "CancelJobOutputTypeDef",
-    {
-        "Success": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 CreateJobOutputTypeDef = TypedDict(
     "CreateJobOutputTypeDef",
     {
         "JobId": str,
         "JobType": JobTypeType,
         "Signature": str,
         "SignatureFileContents": str,
         "WarningMessage": str,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetShippingLabelOutputTypeDef = TypedDict(
-    "GetShippingLabelOutputTypeDef",
-    {
-        "ShippingLabelURL": str,
-        "Warning": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStatusOutputTypeDef = TypedDict(
     "GetStatusOutputTypeDef",
     {
         "JobId": str,
@@ -249,38 +269,29 @@
         "LogKey": str,
         "ErrorCount": int,
         "Signature": str,
         "SignatureFileContents": str,
         "CurrentManifest": str,
         "CreationDate": datetime,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateJobOutputTypeDef = TypedDict(
     "UpdateJobOutputTypeDef",
     {
         "Success": bool,
         "WarningMessage": str,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsOutputTypeDef = TypedDict(
     "ListJobsOutputTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "IsTruncated": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-
-ListJobsInputListJobsPaginateTypeDef = TypedDict(
-    "ListJobsInputListJobsPaginateTypeDef",
-    {
-        "APIVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
```

### Comparing `mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport.egg-info/PKG-INFO` & `mypy-boto3-importexport-1.27.0/mypy_boto3_importexport.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-importexport
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ImportExport 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ImportExport 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/
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
 
 <a id="mypy-boto3-importexport"></a>
 
 # mypy-boto3-importexport
 
 [![PyPI - mypy-boto3-importexport](https://img.shields.io/pypi/v/mypy-boto3-importexport.svg?color=blue)](https://pypi.org/project/mypy-boto3-importexport)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-importexport.svg?color=blue)](https://pypi.org/project/mypy-boto3-importexport)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-importexport?color=blue)](https://pypistats.org/packages/mypy-boto3-importexport)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ImportExport 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
+[boto3.ImportExport 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
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
 [mypy-boto3-importexport docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,71 +321,71 @@
 `mypy_boto3_importexport.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_importexport.type_defs import (
     ArtifactTypeDef,
     CancelJobInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJobOutputTypeDef,
     CreateJobInputRequestTypeDef,
     GetShippingLabelInputRequestTypeDef,
+    GetShippingLabelOutputTypeDef,
     GetStatusInputRequestTypeDef,
     JobTypeDef,
-    PaginatorConfigTypeDef,
+    ListJobsInputListJobsPaginateTypeDef,
     ListJobsInputRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UpdateJobInputRequestTypeDef,
-    CancelJobOutputTypeDef,
     CreateJobOutputTypeDef,
-    GetShippingLabelOutputTypeDef,
     GetStatusOutputTypeDef,
     UpdateJobOutputTypeDef,
     ListJobsOutputTypeDef,
-    ListJobsInputListJobsPaginateTypeDef,
 )
 
 
 def get_structure() -> ArtifactTypeDef:
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

### Comparing `mypy-boto3-importexport-1.26.0.post1/mypy_boto3_importexport.egg-info/SOURCES.txt` & `mypy-boto3-importexport-1.27.0/mypy_boto3_importexport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-importexport-1.26.0.post1/setup.py` & `mypy-boto3-importexport-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-importexport.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-importexport",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_importexport"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ImportExport 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.ImportExport 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 importexport type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_importexport": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_importexport": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/",
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


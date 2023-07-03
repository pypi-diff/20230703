# Comparing `tmp/mypy-boto3-backupstorage-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-backupstorage-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-backupstorage-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:07 2022, max compression
+gzip compressed data, was "mypy-boto3-backupstorage-1.27.0.tar", last modified: Mon Jul  3 19:50:25 2023, max compression
```

## Comparing `mypy-boto3-backupstorage-1.26.0.post1.tar` & `mypy-boto3-backupstorage-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:07.904834 mypy-boto3-backupstorage-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:30:56.000000 mypy-boto3-backupstorage-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12824 2022-11-01 21:43:07.896834 mypy-boto3-backupstorage-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11359 2022-11-01 21:30:56.000000 mypy-boto3-backupstorage-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:07.896834 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-11-01 21:30:56.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-11-01 21:30:56.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-11-01 21:30:56.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9886 2022-11-01 21:30:56.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     9870 2022-11-01 21:30:56.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7115 2022-11-01 21:30:56.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7113 2022-11-01 21:30:56.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:30:56.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     8441 2022-11-01 21:30:56.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8428 2022-11-01 21:30:56.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:30:56.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:07.896834 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12824 2022-11-01 21:43:07.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-11-01 21:43:07.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:07.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:07.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:07.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:07.000000 mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:07.904834 mypy-boto3-backupstorage-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-11-01 21:30:56.000000 mypy-boto3-backupstorage-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:25.526875 mypy-boto3-backupstorage-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:04.000000 mypy-boto3-backupstorage-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-07-03 19:50:25.526875 mypy-boto3-backupstorage-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-03 19:33:04.000000 mypy-boto3-backupstorage-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:25.518875 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-03 19:33:04.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-03 19:33:04.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 19:33:04.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-03 19:33:04.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-07-03 19:33:04.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-03 19:33:05.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-07-03 19:33:04.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:04.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-07-03 19:33:05.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-03 19:33:05.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:04.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:25.526875 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-07-03 19:50:25.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-03 19:50:25.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:25.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:25.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:25.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 19:50:25.000000 mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:25.526875 mypy-boto3-backupstorage-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-03 19:33:04.000000 mypy-boto3-backupstorage-1.27.0/setup.py
```

### Comparing `mypy-boto3-backupstorage-1.26.0.post1/LICENSE` & `mypy-boto3-backupstorage-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-backupstorage-1.26.0.post1/PKG-INFO` & `mypy-boto3-backupstorage-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backupstorage
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.BackupStorage 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.BackupStorage 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/
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
 
 <a id="mypy-boto3-backupstorage"></a>
 
 # mypy-boto3-backupstorage
 
 [![PyPI - mypy-boto3-backupstorage](https://img.shields.io/pypi/v/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backupstorage?color=blue)](https://pypistats.org/packages/mypy-boto3-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupStorage 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[boto3.BackupStorage 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [mypy-boto3-backupstorage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,74 +301,74 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_backupstorage.type_defs import (
     BackupObjectTypeDef,
     ChunkTypeDef,
     DeleteObjectInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChunkInputRequestTypeDef,
+    GetChunkOutputTypeDef,
     GetObjectMetadataInputRequestTypeDef,
+    GetObjectMetadataOutputTypeDef,
     ListChunksInputRequestTypeDef,
     ListObjectsInputRequestTypeDef,
     NotifyObjectCompleteInputRequestTypeDef,
-    PutChunkInputRequestTypeDef,
-    PutObjectInputRequestTypeDef,
-    StartObjectInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetChunkOutputTypeDef,
-    GetObjectMetadataOutputTypeDef,
-    ListChunksOutputTypeDef,
-    ListObjectsOutputTypeDef,
     NotifyObjectCompleteOutputTypeDef,
+    PutChunkInputRequestTypeDef,
     PutChunkOutputTypeDef,
+    PutObjectInputRequestTypeDef,
     PutObjectOutputTypeDef,
+    ResponseMetadataTypeDef,
+    StartObjectInputRequestTypeDef,
     StartObjectOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    ListChunksOutputTypeDef,
 )
 
 
 def get_structure() -> BackupObjectTypeDef:
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

### Comparing `mypy-boto3-backupstorage-1.26.0.post1/README.md` & `mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-backupstorage
+Version: 1.27.0
+Summary: Type annotations for boto3.BackupStorage 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 backupstorage type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-backupstorage"></a>
 
 # mypy-boto3-backupstorage
 
 [![PyPI - mypy-boto3-backupstorage](https://img.shields.io/pypi/v/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backupstorage?color=blue)](https://pypistats.org/packages/mypy-boto3-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupStorage 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[boto3.BackupStorage 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [mypy-boto3-backupstorage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,74 +301,74 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_backupstorage.type_defs import (
     BackupObjectTypeDef,
     ChunkTypeDef,
     DeleteObjectInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChunkInputRequestTypeDef,
+    GetChunkOutputTypeDef,
     GetObjectMetadataInputRequestTypeDef,
+    GetObjectMetadataOutputTypeDef,
     ListChunksInputRequestTypeDef,
     ListObjectsInputRequestTypeDef,
     NotifyObjectCompleteInputRequestTypeDef,
-    PutChunkInputRequestTypeDef,
-    PutObjectInputRequestTypeDef,
-    StartObjectInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetChunkOutputTypeDef,
-    GetObjectMetadataOutputTypeDef,
-    ListChunksOutputTypeDef,
-    ListObjectsOutputTypeDef,
     NotifyObjectCompleteOutputTypeDef,
+    PutChunkInputRequestTypeDef,
     PutChunkOutputTypeDef,
+    PutObjectInputRequestTypeDef,
     PutObjectOutputTypeDef,
+    ResponseMetadataTypeDef,
+    StartObjectInputRequestTypeDef,
     StartObjectOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    ListChunksOutputTypeDef,
 )
 
 
 def get_structure() -> BackupObjectTypeDef:
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

### Comparing `mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/__main__.py` & `mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.BackupStorage 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.BackupStorage 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage\nOther"
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

### Comparing `mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/client.py` & `mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/client.pyi` & `mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/literals.py` & `mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/literals.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -14,25 +14,23 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DataChecksumAlgorithmType",
     "SummaryChecksumAlgorithmType",
     "BackupStorageServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 DataChecksumAlgorithmType = Literal["SHA256"]
 SummaryChecksumAlgorithmType = Literal["SUMMARY"]
 BackupStorageServiceName = Literal["backupstorage"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -43,23 +41,25 @@
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
@@ -69,30 +69,35 @@
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
@@ -118,14 +123,15 @@
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
@@ -170,51 +176,57 @@
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
@@ -227,14 +239,15 @@
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
@@ -246,28 +259,35 @@
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
@@ -276,14 +296,15 @@
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
@@ -294,55 +315,64 @@
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
@@ -360,8 +390,36 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-RegionName = Literal["eu-west-1", "us-east-1", "us-east-2", "us-west-2"]
+RegionName = Literal[
+    "af-south-1",
+    "ap-east-1",
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-northeast-3",
+    "ap-south-1",
+    "ap-south-2",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ap-southeast-3",
+    "ap-southeast-4",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-central-2",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
+    "eu-west-1",
+    "eu-west-2",
+    "eu-west-3",
+    "me-central-1",
+    "me-south-1",
+    "sa-east-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-1",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/literals.pyi` & `mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/literals.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DataChecksumAlgorithmType",
     "SummaryChecksumAlgorithmType",
     "BackupStorageServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 DataChecksumAlgorithmType = Literal["SHA256"]
 SummaryChecksumAlgorithmType = Literal["SUMMARY"]
 BackupStorageServiceName = Literal["backupstorage"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -41,23 +43,25 @@
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
@@ -67,30 +71,35 @@
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
@@ -116,14 +125,15 @@
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
@@ -168,51 +178,57 @@
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
@@ -225,14 +241,15 @@
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
@@ -244,28 +261,35 @@
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
@@ -274,14 +298,15 @@
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
@@ -292,55 +317,64 @@
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
@@ -358,8 +392,36 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-RegionName = Literal["eu-west-1", "us-east-1", "us-east-2", "us-west-2"]
+RegionName = Literal[
+    "af-south-1",
+    "ap-east-1",
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-northeast-3",
+    "ap-south-1",
+    "ap-south-2",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ap-southeast-3",
+    "ap-southeast-4",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-central-2",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-south-2",
+    "eu-west-1",
+    "eu-west-2",
+    "eu-west-3",
+    "me-central-1",
+    "me-south-1",
+    "sa-east-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-1",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/type_defs.py` & `mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,32 +27,32 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BackupObjectTypeDef",
     "ChunkTypeDef",
     "DeleteObjectInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetChunkInputRequestTypeDef",
+    "GetChunkOutputTypeDef",
     "GetObjectMetadataInputRequestTypeDef",
+    "GetObjectMetadataOutputTypeDef",
     "ListChunksInputRequestTypeDef",
     "ListObjectsInputRequestTypeDef",
     "NotifyObjectCompleteInputRequestTypeDef",
-    "PutChunkInputRequestTypeDef",
-    "PutObjectInputRequestTypeDef",
-    "StartObjectInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetChunkOutputTypeDef",
-    "GetObjectMetadataOutputTypeDef",
-    "ListChunksOutputTypeDef",
-    "ListObjectsOutputTypeDef",
     "NotifyObjectCompleteOutputTypeDef",
+    "PutChunkInputRequestTypeDef",
     "PutChunkOutputTypeDef",
+    "PutObjectInputRequestTypeDef",
     "PutObjectOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartObjectInputRequestTypeDef",
     "StartObjectOutputTypeDef",
+    "ListObjectsOutputTypeDef",
+    "ListChunksOutputTypeDef",
 )
 
 _RequiredBackupObjectTypeDef = TypedDict(
     "_RequiredBackupObjectTypeDef",
     {
         "Name": str,
         "ObjectChecksum": str,
@@ -89,41 +89,60 @@
     "DeleteObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChunkInputRequestTypeDef = TypedDict(
     "GetChunkInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ChunkToken": str,
     },
 )
 
+GetChunkOutputTypeDef = TypedDict(
+    "GetChunkOutputTypeDef",
+    {
+        "Data": StreamingBody,
+        "Length": int,
+        "Checksum": str,
+        "ChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetObjectMetadataInputRequestTypeDef = TypedDict(
     "GetObjectMetadataInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ObjectToken": str,
     },
 )
 
+GetObjectMetadataOutputTypeDef = TypedDict(
+    "GetObjectMetadataOutputTypeDef",
+    {
+        "MetadataString": str,
+        "MetadataBlob": StreamingBody,
+        "MetadataBlobLength": int,
+        "MetadataBlobChecksum": str,
+        "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListChunksInputRequestTypeDef = TypedDict(
     "_RequiredListChunksInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ObjectToken": str,
     },
 )
@@ -194,27 +213,45 @@
 class NotifyObjectCompleteInputRequestTypeDef(
     _RequiredNotifyObjectCompleteInputRequestTypeDef,
     _OptionalNotifyObjectCompleteInputRequestTypeDef,
 ):
     pass
 
 
+NotifyObjectCompleteOutputTypeDef = TypedDict(
+    "NotifyObjectCompleteOutputTypeDef",
+    {
+        "ObjectChecksum": str,
+        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutChunkInputRequestTypeDef = TypedDict(
     "PutChunkInputRequestTypeDef",
     {
         "BackupJobId": str,
         "UploadId": str,
         "ChunkIndex": int,
         "Data": Union[str, bytes, IO[Any], StreamingBody],
         "Length": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
     },
 )
 
+PutChunkOutputTypeDef = TypedDict(
+    "PutChunkOutputTypeDef",
+    {
+        "ChunkChecksum": str,
+        "ChunkChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutObjectInputRequestTypeDef = TypedDict(
     "_RequiredPutObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
     },
 )
@@ -236,14 +273,36 @@
 
 class PutObjectInputRequestTypeDef(
     _RequiredPutObjectInputRequestTypeDef, _OptionalPutObjectInputRequestTypeDef
 ):
     pass
 
 
+PutObjectOutputTypeDef = TypedDict(
+    "PutObjectOutputTypeDef",
+    {
+        "InlineChunkChecksum": str,
+        "InlineChunkChecksumAlgorithm": Literal["SHA256"],
+        "ObjectChecksum": str,
+        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
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
 _RequiredStartObjectInputRequestTypeDef = TypedDict(
     "_RequiredStartObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
     },
 )
@@ -258,91 +317,32 @@
 
 class StartObjectInputRequestTypeDef(
     _RequiredStartObjectInputRequestTypeDef, _OptionalStartObjectInputRequestTypeDef
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetChunkOutputTypeDef = TypedDict(
-    "GetChunkOutputTypeDef",
-    {
-        "Data": StreamingBody,
-        "Length": int,
-        "Checksum": str,
-        "ChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetObjectMetadataOutputTypeDef = TypedDict(
-    "GetObjectMetadataOutputTypeDef",
-    {
-        "MetadataString": str,
-        "MetadataBlob": StreamingBody,
-        "MetadataBlobLength": int,
-        "MetadataBlobChecksum": str,
-        "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListChunksOutputTypeDef = TypedDict(
-    "ListChunksOutputTypeDef",
+StartObjectOutputTypeDef = TypedDict(
+    "StartObjectOutputTypeDef",
     {
-        "ChunkList": List[ChunkTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "UploadId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListObjectsOutputTypeDef = TypedDict(
     "ListObjectsOutputTypeDef",
     {
         "ObjectList": List[BackupObjectTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-NotifyObjectCompleteOutputTypeDef = TypedDict(
-    "NotifyObjectCompleteOutputTypeDef",
-    {
-        "ObjectChecksum": str,
-        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutChunkOutputTypeDef = TypedDict(
-    "PutChunkOutputTypeDef",
-    {
-        "ChunkChecksum": str,
-        "ChunkChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectOutputTypeDef = TypedDict(
-    "PutObjectOutputTypeDef",
-    {
-        "InlineChunkChecksum": str,
-        "InlineChunkChecksumAlgorithm": Literal["SHA256"],
-        "ObjectChecksum": str,
-        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartObjectOutputTypeDef = TypedDict(
-    "StartObjectOutputTypeDef",
+ListChunksOutputTypeDef = TypedDict(
+    "ListChunksOutputTypeDef",
     {
-        "UploadId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ChunkList": List[ChunkTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage/type_defs.pyi` & `mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,32 +26,32 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BackupObjectTypeDef",
     "ChunkTypeDef",
     "DeleteObjectInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetChunkInputRequestTypeDef",
+    "GetChunkOutputTypeDef",
     "GetObjectMetadataInputRequestTypeDef",
+    "GetObjectMetadataOutputTypeDef",
     "ListChunksInputRequestTypeDef",
     "ListObjectsInputRequestTypeDef",
     "NotifyObjectCompleteInputRequestTypeDef",
-    "PutChunkInputRequestTypeDef",
-    "PutObjectInputRequestTypeDef",
-    "StartObjectInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetChunkOutputTypeDef",
-    "GetObjectMetadataOutputTypeDef",
-    "ListChunksOutputTypeDef",
-    "ListObjectsOutputTypeDef",
     "NotifyObjectCompleteOutputTypeDef",
+    "PutChunkInputRequestTypeDef",
     "PutChunkOutputTypeDef",
+    "PutObjectInputRequestTypeDef",
     "PutObjectOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartObjectInputRequestTypeDef",
     "StartObjectOutputTypeDef",
+    "ListObjectsOutputTypeDef",
+    "ListChunksOutputTypeDef",
 )
 
 _RequiredBackupObjectTypeDef = TypedDict(
     "_RequiredBackupObjectTypeDef",
     {
         "Name": str,
         "ObjectChecksum": str,
@@ -86,41 +86,60 @@
     "DeleteObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChunkInputRequestTypeDef = TypedDict(
     "GetChunkInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ChunkToken": str,
     },
 )
 
+GetChunkOutputTypeDef = TypedDict(
+    "GetChunkOutputTypeDef",
+    {
+        "Data": StreamingBody,
+        "Length": int,
+        "Checksum": str,
+        "ChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetObjectMetadataInputRequestTypeDef = TypedDict(
     "GetObjectMetadataInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ObjectToken": str,
     },
 )
 
+GetObjectMetadataOutputTypeDef = TypedDict(
+    "GetObjectMetadataOutputTypeDef",
+    {
+        "MetadataString": str,
+        "MetadataBlob": StreamingBody,
+        "MetadataBlobLength": int,
+        "MetadataBlobChecksum": str,
+        "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListChunksInputRequestTypeDef = TypedDict(
     "_RequiredListChunksInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ObjectToken": str,
     },
 )
@@ -185,27 +204,45 @@
 
 class NotifyObjectCompleteInputRequestTypeDef(
     _RequiredNotifyObjectCompleteInputRequestTypeDef,
     _OptionalNotifyObjectCompleteInputRequestTypeDef,
 ):
     pass
 
+NotifyObjectCompleteOutputTypeDef = TypedDict(
+    "NotifyObjectCompleteOutputTypeDef",
+    {
+        "ObjectChecksum": str,
+        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutChunkInputRequestTypeDef = TypedDict(
     "PutChunkInputRequestTypeDef",
     {
         "BackupJobId": str,
         "UploadId": str,
         "ChunkIndex": int,
         "Data": Union[str, bytes, IO[Any], StreamingBody],
         "Length": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
     },
 )
 
+PutChunkOutputTypeDef = TypedDict(
+    "PutChunkOutputTypeDef",
+    {
+        "ChunkChecksum": str,
+        "ChunkChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutObjectInputRequestTypeDef = TypedDict(
     "_RequiredPutObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
     },
 )
@@ -225,14 +262,36 @@
 )
 
 class PutObjectInputRequestTypeDef(
     _RequiredPutObjectInputRequestTypeDef, _OptionalPutObjectInputRequestTypeDef
 ):
     pass
 
+PutObjectOutputTypeDef = TypedDict(
+    "PutObjectOutputTypeDef",
+    {
+        "InlineChunkChecksum": str,
+        "InlineChunkChecksumAlgorithm": Literal["SHA256"],
+        "ObjectChecksum": str,
+        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
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
 _RequiredStartObjectInputRequestTypeDef = TypedDict(
     "_RequiredStartObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
     },
 )
@@ -245,91 +304,32 @@
 )
 
 class StartObjectInputRequestTypeDef(
     _RequiredStartObjectInputRequestTypeDef, _OptionalStartObjectInputRequestTypeDef
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetChunkOutputTypeDef = TypedDict(
-    "GetChunkOutputTypeDef",
-    {
-        "Data": StreamingBody,
-        "Length": int,
-        "Checksum": str,
-        "ChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetObjectMetadataOutputTypeDef = TypedDict(
-    "GetObjectMetadataOutputTypeDef",
-    {
-        "MetadataString": str,
-        "MetadataBlob": StreamingBody,
-        "MetadataBlobLength": int,
-        "MetadataBlobChecksum": str,
-        "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListChunksOutputTypeDef = TypedDict(
-    "ListChunksOutputTypeDef",
+StartObjectOutputTypeDef = TypedDict(
+    "StartObjectOutputTypeDef",
     {
-        "ChunkList": List[ChunkTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "UploadId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListObjectsOutputTypeDef = TypedDict(
     "ListObjectsOutputTypeDef",
     {
         "ObjectList": List[BackupObjectTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-NotifyObjectCompleteOutputTypeDef = TypedDict(
-    "NotifyObjectCompleteOutputTypeDef",
-    {
-        "ObjectChecksum": str,
-        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutChunkOutputTypeDef = TypedDict(
-    "PutChunkOutputTypeDef",
-    {
-        "ChunkChecksum": str,
-        "ChunkChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectOutputTypeDef = TypedDict(
-    "PutObjectOutputTypeDef",
-    {
-        "InlineChunkChecksum": str,
-        "InlineChunkChecksumAlgorithm": Literal["SHA256"],
-        "ObjectChecksum": str,
-        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartObjectOutputTypeDef = TypedDict(
-    "StartObjectOutputTypeDef",
+ListChunksOutputTypeDef = TypedDict(
+    "ListChunksOutputTypeDef",
     {
-        "UploadId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ChunkList": List[ChunkTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage.egg-info/PKG-INFO` & `mypy-boto3-backupstorage-1.27.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-backupstorage
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.BackupStorage 1.26.0 service generated with mypy-boto3-builder 7.11.10
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 backupstorage type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-backupstorage"></a>
 
 # mypy-boto3-backupstorage
 
 [![PyPI - mypy-boto3-backupstorage](https://img.shields.io/pypi/v/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backupstorage?color=blue)](https://pypistats.org/packages/mypy-boto3-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupStorage 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[boto3.BackupStorage 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [mypy-boto3-backupstorage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,74 +269,74 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_backupstorage.type_defs import (
     BackupObjectTypeDef,
     ChunkTypeDef,
     DeleteObjectInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetChunkInputRequestTypeDef,
+    GetChunkOutputTypeDef,
     GetObjectMetadataInputRequestTypeDef,
+    GetObjectMetadataOutputTypeDef,
     ListChunksInputRequestTypeDef,
     ListObjectsInputRequestTypeDef,
     NotifyObjectCompleteInputRequestTypeDef,
-    PutChunkInputRequestTypeDef,
-    PutObjectInputRequestTypeDef,
-    StartObjectInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetChunkOutputTypeDef,
-    GetObjectMetadataOutputTypeDef,
-    ListChunksOutputTypeDef,
-    ListObjectsOutputTypeDef,
     NotifyObjectCompleteOutputTypeDef,
+    PutChunkInputRequestTypeDef,
     PutChunkOutputTypeDef,
+    PutObjectInputRequestTypeDef,
     PutObjectOutputTypeDef,
+    ResponseMetadataTypeDef,
+    StartObjectInputRequestTypeDef,
     StartObjectOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    ListChunksOutputTypeDef,
 )
 
 
 def get_structure() -> BackupObjectTypeDef:
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

### Comparing `mypy-boto3-backupstorage-1.26.0.post1/mypy_boto3_backupstorage.egg-info/SOURCES.txt` & `mypy-boto3-backupstorage-1.27.0/mypy_boto3_backupstorage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.26.0.post1/setup.py` & `mypy-boto3-backupstorage-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-backupstorage.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-backupstorage",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_backupstorage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.BackupStorage 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.BackupStorage 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 backupstorage type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_backupstorage": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_backupstorage": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/",
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


# Comparing `tmp/mypy-boto3-iotsecuretunneling-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-iotsecuretunneling-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotsecuretunneling-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:34 2022, max compression
+gzip compressed data, was "mypy-boto3-iotsecuretunneling-1.27.0.tar", last modified: Mon Jul  3 19:50:55 2023, max compression
```

## Comparing `mypy-boto3-iotsecuretunneling-1.26.0.post1.tar` & `mypy-boto3-iotsecuretunneling-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:34.668830 mypy-boto3-iotsecuretunneling-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:36:16.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13080 2022-11-01 21:43:34.660829 mypy-boto3-iotsecuretunneling-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11595 2022-11-01 21:36:16.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:34.660829 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-11-01 21:36:16.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-11-01 21:36:16.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-11-01 21:36:16.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7989 2022-11-01 21:36:16.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     7975 2022-11-01 21:36:16.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7477 2022-11-01 21:36:16.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7475 2022-11-01 21:36:16.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:36:16.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     6490 2022-11-01 21:36:16.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6483 2022-11-01 21:36:16.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:36:16.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:34.660829 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13080 2022-11-01 21:43:34.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-11-01 21:43:34.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:34.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:34.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:34.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-01 21:43:34.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:34.668830 mypy-boto3-iotsecuretunneling-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-11-01 21:36:16.000000 mypy-boto3-iotsecuretunneling-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:55.183444 mypy-boto3-iotsecuretunneling-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:45.000000 mypy-boto3-iotsecuretunneling-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-07-03 19:50:55.183444 mypy-boto3-iotsecuretunneling-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-07-03 19:39:45.000000 mypy-boto3-iotsecuretunneling-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:55.179443 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-03 19:39:45.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-03 19:39:45.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 19:39:45.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-03 19:39:45.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-07-03 19:39:45.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-07-03 19:39:45.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-03 19:39:45.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:45.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-07-03 19:39:46.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-03 19:39:46.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:45.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:55.183444 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-07-03 19:50:55.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 19:50:55.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:55.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:55.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:55.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 19:50:55.000000 mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:55.183444 mypy-boto3-iotsecuretunneling-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-03 19:39:45.000000 mypy-boto3-iotsecuretunneling-1.27.0/setup.py
```

### Comparing `mypy-boto3-iotsecuretunneling-1.26.0.post1/LICENSE` & `mypy-boto3-iotsecuretunneling-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-iotsecuretunneling-1.26.0.post1/PKG-INFO` & `mypy-boto3-iotsecuretunneling-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsecuretunneling
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IoTSecureTunneling 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTSecureTunneling 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/
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
 
 <a id="mypy-boto3-iotsecuretunneling"></a>
 
 # mypy-boto3-iotsecuretunneling
 
 [![PyPI - mypy-boto3-iotsecuretunneling](https://img.shields.io/pypi/v/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotsecuretunneling?color=blue)](https://pypistats.org/packages/mypy-boto3-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSecureTunneling 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[boto3.IoTSecureTunneling 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [mypy-boto3-iotsecuretunneling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,24 +303,24 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotsecuretunneling.type_defs import (
     CloseTunnelRequestRequestTypeDef,
     ConnectionStateTypeDef,
     DescribeTunnelRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     DestinationConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     ListTunnelsRequestRequestTypeDef,
     TunnelSummaryTypeDef,
     TimeoutConfigTypeDef,
-    UntagResourceRequestRequestTypeDef,
     OpenTunnelResponseTypeDef,
+    ResponseMetadataTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
     RotateTunnelAccessTokenRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListTunnelsResponseTypeDef,
     OpenTunnelRequestRequestTypeDef,
     TunnelTypeDef,
     DescribeTunnelResponseTypeDef,
@@ -333,42 +334,42 @@
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

### Comparing `mypy-boto3-iotsecuretunneling-1.26.0.post1/README.md` & `mypy-boto3-iotsecuretunneling-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iotsecuretunneling"></a>
 
 # mypy-boto3-iotsecuretunneling
 
 [![PyPI - mypy-boto3-iotsecuretunneling](https://img.shields.io/pypi/v/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotsecuretunneling?color=blue)](https://pypistats.org/packages/mypy-boto3-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSecureTunneling 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[boto3.IoTSecureTunneling 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [mypy-boto3-iotsecuretunneling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -271,24 +271,24 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotsecuretunneling.type_defs import (
     CloseTunnelRequestRequestTypeDef,
     ConnectionStateTypeDef,
     DescribeTunnelRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     DestinationConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     ListTunnelsRequestRequestTypeDef,
     TunnelSummaryTypeDef,
     TimeoutConfigTypeDef,
-    UntagResourceRequestRequestTypeDef,
     OpenTunnelResponseTypeDef,
+    ResponseMetadataTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
     RotateTunnelAccessTokenRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListTunnelsResponseTypeDef,
     OpenTunnelRequestRequestTypeDef,
     TunnelTypeDef,
     DescribeTunnelResponseTypeDef,
@@ -302,42 +302,42 @@
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

### Comparing `mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/__main__.py` & `mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTSecureTunneling 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.IoTSecureTunneling 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling\nOther"
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

### Comparing `mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/client.py` & `mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/client.pyi` & `mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/literals.py` & `mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,26 +14,24 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ClientModeType",
     "ConnectionStatusType",
     "TunnelStatusType",
     "IoTSecureTunnelingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ClientModeType = Literal["ALL", "DESTINATION", "SOURCE"]
 ConnectionStatusType = Literal["CONNECTED", "DISCONNECTED"]
 TunnelStatusType = Literal["CLOSED", "OPEN"]
 IoTSecureTunnelingServiceName = Literal["iotsecuretunneling"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -45,23 +43,25 @@
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
@@ -71,30 +71,35 @@
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
@@ -120,14 +125,15 @@
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
@@ -172,51 +178,57 @@
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
@@ -229,14 +241,15 @@
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
@@ -248,28 +261,35 @@
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
@@ -278,14 +298,15 @@
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
@@ -296,55 +317,64 @@
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
@@ -375,14 +405,15 @@
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/literals.pyi` & `mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ClientModeType",
     "ConnectionStatusType",
     "TunnelStatusType",
     "IoTSecureTunnelingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 ClientModeType = Literal["ALL", "DESTINATION", "SOURCE"]
 ConnectionStatusType = Literal["CONNECTED", "DISCONNECTED"]
 TunnelStatusType = Literal["CLOSED", "OPEN"]
 IoTSecureTunnelingServiceName = Literal["iotsecuretunneling"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -43,23 +45,25 @@
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
@@ -69,30 +73,35 @@
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
@@ -118,14 +127,15 @@
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
@@ -170,51 +180,57 @@
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
@@ -227,14 +243,15 @@
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
@@ -246,28 +263,35 @@
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
@@ -276,14 +300,15 @@
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
@@ -294,55 +319,64 @@
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
@@ -373,14 +407,15 @@
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/type_defs.py` & `mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,24 +23,24 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CloseTunnelRequestRequestTypeDef",
     "ConnectionStateTypeDef",
     "DescribeTunnelRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "DestinationConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "ListTunnelsRequestRequestTypeDef",
     "TunnelSummaryTypeDef",
     "TimeoutConfigTypeDef",
-    "UntagResourceRequestRequestTypeDef",
     "OpenTunnelResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "RotateTunnelAccessTokenResponseTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "RotateTunnelAccessTokenRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListTunnelsResponseTypeDef",
     "OpenTunnelRequestRequestTypeDef",
     "TunnelTypeDef",
     "DescribeTunnelResponseTypeDef",
@@ -79,25 +79,14 @@
 DescribeTunnelRequestRequestTypeDef = TypedDict(
     "DescribeTunnelRequestRequestTypeDef",
     {
         "tunnelId": str,
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
 _RequiredDestinationConfigTypeDef = TypedDict(
     "_RequiredDestinationConfigTypeDef",
     {
         "services": List[str],
     },
 )
 _OptionalDestinationConfigTypeDef = TypedDict(
@@ -157,40 +146,51 @@
     "TimeoutConfigTypeDef",
     {
         "maxLifetimeTimeoutMinutes": int,
     },
     total=False,
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
-    },
-)
-
 OpenTunnelResponseTypeDef = TypedDict(
     "OpenTunnelResponseTypeDef",
     {
         "tunnelId": str,
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
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
     },
 )
 
 RotateTunnelAccessTokenResponseTypeDef = TypedDict(
     "RotateTunnelAccessTokenResponseTypeDef",
     {
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
 _RequiredRotateTunnelAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRotateTunnelAccessTokenRequestRequestTypeDef",
     {
         "tunnelId": str,
@@ -213,15 +213,15 @@
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -230,15 +230,15 @@
 )
 
 ListTunnelsResponseTypeDef = TypedDict(
     "ListTunnelsResponseTypeDef",
     {
         "tunnelSummaries": List[TunnelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OpenTunnelRequestRequestTypeDef = TypedDict(
     "OpenTunnelRequestRequestTypeDef",
     {
         "description": str,
@@ -267,10 +267,10 @@
     total=False,
 )
 
 DescribeTunnelResponseTypeDef = TypedDict(
     "DescribeTunnelResponseTypeDef",
     {
         "tunnel": TunnelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling/type_defs.pyi` & `mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -22,24 +22,24 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CloseTunnelRequestRequestTypeDef",
     "ConnectionStateTypeDef",
     "DescribeTunnelRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "DestinationConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "ListTunnelsRequestRequestTypeDef",
     "TunnelSummaryTypeDef",
     "TimeoutConfigTypeDef",
-    "UntagResourceRequestRequestTypeDef",
     "OpenTunnelResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "RotateTunnelAccessTokenResponseTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "RotateTunnelAccessTokenRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListTunnelsResponseTypeDef",
     "OpenTunnelRequestRequestTypeDef",
     "TunnelTypeDef",
     "DescribeTunnelResponseTypeDef",
@@ -76,25 +76,14 @@
 DescribeTunnelRequestRequestTypeDef = TypedDict(
     "DescribeTunnelRequestRequestTypeDef",
     {
         "tunnelId": str,
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
 _RequiredDestinationConfigTypeDef = TypedDict(
     "_RequiredDestinationConfigTypeDef",
     {
         "services": List[str],
     },
 )
 _OptionalDestinationConfigTypeDef = TypedDict(
@@ -152,40 +141,51 @@
     "TimeoutConfigTypeDef",
     {
         "maxLifetimeTimeoutMinutes": int,
     },
     total=False,
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
-    },
-)
-
 OpenTunnelResponseTypeDef = TypedDict(
     "OpenTunnelResponseTypeDef",
     {
         "tunnelId": str,
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
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
     },
 )
 
 RotateTunnelAccessTokenResponseTypeDef = TypedDict(
     "RotateTunnelAccessTokenResponseTypeDef",
     {
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
 _RequiredRotateTunnelAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRotateTunnelAccessTokenRequestRequestTypeDef",
     {
         "tunnelId": str,
@@ -206,15 +206,15 @@
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -223,15 +223,15 @@
 )
 
 ListTunnelsResponseTypeDef = TypedDict(
     "ListTunnelsResponseTypeDef",
     {
         "tunnelSummaries": List[TunnelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OpenTunnelRequestRequestTypeDef = TypedDict(
     "OpenTunnelRequestRequestTypeDef",
     {
         "description": str,
@@ -260,10 +260,10 @@
     total=False,
 )
 
 DescribeTunnelResponseTypeDef = TypedDict(
     "DescribeTunnelResponseTypeDef",
     {
         "tunnel": TunnelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO` & `mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsecuretunneling
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.IoTSecureTunneling 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.IoTSecureTunneling 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/
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
 
 <a id="mypy-boto3-iotsecuretunneling"></a>
 
 # mypy-boto3-iotsecuretunneling
 
 [![PyPI - mypy-boto3-iotsecuretunneling](https://img.shields.io/pypi/v/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotsecuretunneling?color=blue)](https://pypistats.org/packages/mypy-boto3-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSecureTunneling 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[boto3.IoTSecureTunneling 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [mypy-boto3-iotsecuretunneling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,24 +303,24 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotsecuretunneling.type_defs import (
     CloseTunnelRequestRequestTypeDef,
     ConnectionStateTypeDef,
     DescribeTunnelRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     DestinationConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     ListTunnelsRequestRequestTypeDef,
     TunnelSummaryTypeDef,
     TimeoutConfigTypeDef,
-    UntagResourceRequestRequestTypeDef,
     OpenTunnelResponseTypeDef,
+    ResponseMetadataTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
     RotateTunnelAccessTokenRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListTunnelsResponseTypeDef,
     OpenTunnelRequestRequestTypeDef,
     TunnelTypeDef,
     DescribeTunnelResponseTypeDef,
@@ -333,42 +334,42 @@
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

### Comparing `mypy-boto3-iotsecuretunneling-1.26.0.post1/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt` & `mypy-boto3-iotsecuretunneling-1.27.0/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.26.0.post1/setup.py` & `mypy-boto3-iotsecuretunneling-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 """
 Setup script for mypy-boto3-iotsecuretunneling.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotsecuretunneling",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_iotsecuretunneling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTSecureTunneling 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.IoTSecureTunneling 1.27.0 service generated with"
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
     keywords="boto3 iotsecuretunneling type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_iotsecuretunneling": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_iotsecuretunneling": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/"
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


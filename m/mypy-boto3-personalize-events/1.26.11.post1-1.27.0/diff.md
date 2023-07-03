# Comparing `tmp/mypy-boto3-personalize-events-1.26.11.post1.tar.gz` & `tmp/mypy-boto3-personalize-events-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-personalize-events-1.26.11.post1.tar", last modified: Wed Nov 16 20:47:47 2022, max compression
+gzip compressed data, was "mypy-boto3-personalize-events-1.27.0.tar", last modified: Mon Jul  3 19:51:14 2023, max compression
```

## Comparing `mypy-boto3-personalize-events-1.26.11.post1.tar` & `mypy-boto3-personalize-events-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 20:47:47.638882 mypy-boto3-personalize-events-1.26.11.post1/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-16 20:47:08.000000 mypy-boto3-personalize-events-1.26.11.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    12562 2022-11-16 20:47:47.638882 mypy-boto3-personalize-events-1.26.11.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11076 2022-11-16 20:47:08.000000 mypy-boto3-personalize-events-1.26.11.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 20:47:47.630882 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/
--rw-r--r--   0 runner    (1001) docker     (122)      456 2022-11-16 20:47:08.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      455 2022-11-16 20:47:08.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      962 2022-11-16 20:47:08.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4934 2022-11-16 20:47:08.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4925 2022-11-16 20:47:08.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     6948 2022-11-16 20:47:08.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)     6946 2022-11-16 20:47:08.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 20:47:08.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     3297 2022-11-16 20:47:08.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3289 2022-11-16 20:47:08.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       67 2022-11-16 20:47:08.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 20:47:47.638882 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    12562 2022-11-16 20:47:47.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      802 2022-11-16 20:47:47.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-16 20:47:47.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-16 20:47:47.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-16 20:47:47.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2022-11-16 20:47:47.000000 mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-16 20:47:47.638882 mypy-boto3-personalize-events-1.26.11.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2070 2022-11-16 20:47:08.000000 mypy-boto3-personalize-events-1.26.11.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:14.455791 mypy-boto3-personalize-events-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:24.000000 mypy-boto3-personalize-events-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-03 19:51:14.455791 mypy-boto3-personalize-events-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-07-03 19:43:24.000000 mypy-boto3-personalize-events-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:14.447790 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-03 19:43:24.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-03 19:43:24.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-03 19:43:24.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-03 19:43:24.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-03 19:43:24.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-07-03 19:43:24.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-07-03 19:43:24.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:24.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-03 19:43:24.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-03 19:43:24.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:24.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:14.455791 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-03 19:51:14.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 19:51:14.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:14.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:14.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:14.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 19:51:14.000000 mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:14.455791 mypy-boto3-personalize-events-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-03 19:43:23.000000 mypy-boto3-personalize-events-1.27.0/setup.py
```

### Comparing `mypy-boto3-personalize-events-1.26.11.post1/LICENSE` & `mypy-boto3-personalize-events-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-personalize-events-1.26.11.post1/PKG-INFO` & `mypy-boto3-personalize-events-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize-events
-Version: 1.26.11.post1
-Summary: Type annotations for boto3.PersonalizeEvents 1.26.11 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.PersonalizeEvents 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/
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
 
 <a id="mypy-boto3-personalize-events"></a>
 
 # mypy-boto3-personalize-events
 
 [![PyPI - mypy-boto3-personalize-events](https://img.shields.io/pypi/v/mypy-boto3-personalize-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-events)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize-events?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeEvents 1.26.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
+[boto3.PersonalizeEvents 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
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
 [mypy-boto3-personalize-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,65 +296,65 @@
 ### Typed dictionaries
 
 `mypy_boto3_personalize_events.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_personalize_events.type_defs import (
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     MetricAttributionTypeDef,
     ItemTypeDef,
     UserTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     EventTypeDef,
     PutItemsRequestRequestTypeDef,
     PutUsersRequestRequestTypeDef,
     PutEventsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> EmptyResponseMetadataTypeDef:
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

### Comparing `mypy-boto3-personalize-events-1.26.11.post1/README.md` & `mypy-boto3-personalize-events-1.27.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-personalize-events"></a>
 
 # mypy-boto3-personalize-events
 
 [![PyPI - mypy-boto3-personalize-events](https://img.shields.io/pypi/v/mypy-boto3-personalize-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-events)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize-events?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeEvents 1.26.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
+[boto3.PersonalizeEvents 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
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
 [mypy-boto3-personalize-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/).
 
 See how it helps to find and fix potential bugs:
 
@@ -264,65 +264,65 @@
 ### Typed dictionaries
 
 `mypy_boto3_personalize_events.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_personalize_events.type_defs import (
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     MetricAttributionTypeDef,
     ItemTypeDef,
     UserTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     EventTypeDef,
     PutItemsRequestRequestTypeDef,
     PutUsersRequestRequestTypeDef,
     PutEventsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> EmptyResponseMetadataTypeDef:
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

### Comparing `mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/__main__.py` & `mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PersonalizeEvents 1.26.11\nVersion:        "
-        " 1.26.11.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.PersonalizeEvents 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.11.post1")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/client.py` & `mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/client.pyi` & `mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/literals.py` & `mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,23 +34,25 @@
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
@@ -60,30 +62,35 @@
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
@@ -109,14 +116,15 @@
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
@@ -161,51 +169,57 @@
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
@@ -218,14 +232,15 @@
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
@@ -237,28 +252,35 @@
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
@@ -286,57 +308,64 @@
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
     "ssm-contacts",
     "ssm-incidents",
-    "ssmsap",
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

### Comparing `mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/literals.pyi` & `mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -32,23 +32,25 @@
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
@@ -58,30 +60,35 @@
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
@@ -107,14 +114,15 @@
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
@@ -159,51 +167,57 @@
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
@@ -216,14 +230,15 @@
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
@@ -235,28 +250,35 @@
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
@@ -284,57 +306,64 @@
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
     "ssm-contacts",
     "ssm-incidents",
-    "ssmsap",
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

### Comparing `mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/type_defs.py` & `mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,49 +2,45 @@
 Type annotations for personalize-events service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_personalize_events.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_personalize_events.type_defs import EmptyResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: EmptyResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "MetricAttributionTypeDef",
     "ItemTypeDef",
     "UserTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "EventTypeDef",
     "PutItemsRequestRequestTypeDef",
     "PutUsersRequestRequestTypeDef",
     "PutEventsRequestRequestTypeDef",
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
 
 MetricAttributionTypeDef = TypedDict(
     "MetricAttributionTypeDef",
     {
         "eventAttributionSource": str,
@@ -85,18 +81,22 @@
 )
 
 
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredEventTypeDef = TypedDict(
     "_RequiredEventTypeDef",
     {
         "eventType": str,
```

### Comparing `mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events/type_defs.pyi` & `mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,48 +2,44 @@
 Type annotations for personalize-events service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_personalize_events.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_personalize_events.type_defs import EmptyResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: EmptyResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "MetricAttributionTypeDef",
     "ItemTypeDef",
     "UserTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "EventTypeDef",
     "PutItemsRequestRequestTypeDef",
     "PutUsersRequestRequestTypeDef",
     "PutEventsRequestRequestTypeDef",
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
 
 MetricAttributionTypeDef = TypedDict(
     "MetricAttributionTypeDef",
     {
         "eventAttributionSource": str,
@@ -80,18 +76,22 @@
     },
     total=False,
 )
 
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredEventTypeDef = TypedDict(
     "_RequiredEventTypeDef",
     {
         "eventType": str,
```

### Comparing `mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events.egg-info/PKG-INFO` & `mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize-events
-Version: 1.26.11.post1
-Summary: Type annotations for boto3.PersonalizeEvents 1.26.11 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.PersonalizeEvents 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/
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
 
 <a id="mypy-boto3-personalize-events"></a>
 
 # mypy-boto3-personalize-events
 
 [![PyPI - mypy-boto3-personalize-events](https://img.shields.io/pypi/v/mypy-boto3-personalize-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-events)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize-events?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeEvents 1.26.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
+[boto3.PersonalizeEvents 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
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
 [mypy-boto3-personalize-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,65 +296,65 @@
 ### Typed dictionaries
 
 `mypy_boto3_personalize_events.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_personalize_events.type_defs import (
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     MetricAttributionTypeDef,
     ItemTypeDef,
     UserTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     EventTypeDef,
     PutItemsRequestRequestTypeDef,
     PutUsersRequestRequestTypeDef,
     PutEventsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> EmptyResponseMetadataTypeDef:
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

### Comparing `mypy-boto3-personalize-events-1.26.11.post1/mypy_boto3_personalize_events.egg-info/SOURCES.txt` & `mypy-boto3-personalize-events-1.27.0/mypy_boto3_personalize_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-events-1.26.11.post1/setup.py` & `mypy-boto3-personalize-events-1.27.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 """
 Setup script for mypy-boto3-personalize-events.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-personalize-events",
-    version="1.26.11.post1",
+    version="1.27.0",
     packages=["mypy_boto3_personalize_events"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PersonalizeEvents 1.26.11 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.PersonalizeEvents 1.27.0 service generated with"
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
     keywords="boto3 personalize-events type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_personalize_events": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_personalize_events": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/"
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


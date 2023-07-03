# Comparing `tmp/mypy-boto3-amplifybackend-1.26.44.tar.gz` & `tmp/mypy-boto3-amplifybackend-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplifybackend-1.26.44.tar", last modified: Thu Jan  5 20:26:51 2023, max compression
+gzip compressed data, was "mypy-boto3-amplifybackend-1.27.0.tar", last modified: Mon Jul  3 19:50:20 2023, max compression
```

## Comparing `mypy-boto3-amplifybackend-1.26.44.tar` & `mypy-boto3-amplifybackend-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:50.999951 mypy-boto3-amplifybackend-1.26.44/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-05 20:26:13.000000 mypy-boto3-amplifybackend-1.26.44/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-01-05 20:26:50.999951 mypy-boto3-amplifybackend-1.26.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-01-05 20:26:13.000000 mypy-boto3-amplifybackend-1.26.44/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:50.991952 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-01-05 20:26:13.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-01-05 20:26:13.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-01-05 20:26:13.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23022 2023-01-05 20:26:13.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22983 2023-01-05 20:26:13.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-01-05 20:26:14.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-01-05 20:26:14.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-01-05 20:26:14.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-01-05 20:26:14.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:13.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38938 2023-01-05 20:26:14.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38885 2023-01-05 20:26:14.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-05 20:26:13.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:50.995952 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-01-05 20:26:50.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-05 20:26:50.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 20:26:50.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 20:26:50.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-05 20:26:50.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-05 20:26:50.000000 mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 20:26:50.999951 mypy-boto3-amplifybackend-1.26.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-01-05 20:26:13.000000 mypy-boto3-amplifybackend-1.26.44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:20.330781 mypy-boto3-amplifybackend-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:07.000000 mypy-boto3-amplifybackend-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-07-03 19:50:20.330781 mypy-boto3-amplifybackend-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-07-03 19:32:07.000000 mypy-boto3-amplifybackend-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:20.322781 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 19:32:07.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-03 19:32:07.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 19:32:07.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23022 2023-07-03 19:32:07.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22983 2023-07-03 19:32:07.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-03 19:32:08.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-07-03 19:32:08.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-03 19:32:07.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-03 19:32:07.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:07.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    38938 2023-07-03 19:32:09.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38885 2023-07-03 19:32:09.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:07.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:20.330781 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-07-03 19:50:20.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 19:50:20.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:20.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:20.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:20.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:50:20.000000 mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:20.330781 mypy-boto3-amplifybackend-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-03 19:32:07.000000 mypy-boto3-amplifybackend-1.27.0/setup.py
```

### Comparing `mypy-boto3-amplifybackend-1.26.44/LICENSE` & `mypy-boto3-amplifybackend-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-amplifybackend-1.26.44/PKG-INFO` & `mypy-boto3-amplifybackend-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifybackend
-Version: 1.26.44
-Summary: Type annotations for boto3.AmplifyBackend 1.26.44 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.AmplifyBackend 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-amplifybackend"></a>
 
 # mypy-boto3-amplifybackend
 
 [![PyPI - mypy-boto3-amplifybackend](https://img.shields.io/pypi/v/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplifybackend?color=blue)](https://pypistats.org/packages/mypy-boto3-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyBackend 1.26.44](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
+[boto3.AmplifyBackend 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-amplifybackend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -448,42 +448,42 @@
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

### Comparing `mypy-boto3-amplifybackend-1.26.44/README.md` & `mypy-boto3-amplifybackend-1.27.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-amplifybackend"></a>
 
 # mypy-boto3-amplifybackend
 
 [![PyPI - mypy-boto3-amplifybackend](https://img.shields.io/pypi/v/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplifybackend?color=blue)](https://pypistats.org/packages/mypy-boto3-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyBackend 1.26.44](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
+[boto3.AmplifyBackend 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-amplifybackend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -416,42 +416,42 @@
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

### Comparing `mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/__init__.py` & `mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/__init__.pyi` & `mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/__main__.py` & `mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AmplifyBackend 1.26.44\nVersion:         1.26.44\nBuilder"
-        " version: 7.12.2\nDocs:           "
+        "Type annotations for boto3.AmplifyBackend 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.44")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/client.py` & `mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/client.pyi` & `mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/literals.py` & `mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AdditionalConstraintsElementType",
     "AuthResourcesType",
     "AuthenticatedElementType",
     "DeliveryMethodType",
     "ListBackendJobsPaginatorName",
     "MFAModeType",
@@ -40,15 +39,14 @@
     "AmplifyBackendServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdditionalConstraintsElementType = Literal[
     "REQUIRE_DIGIT", "REQUIRE_LOWERCASE", "REQUIRE_SYMBOL", "REQUIRE_UPPERCASE"
 ]
 AuthResourcesType = Literal["IDENTITY_POOL_AND_USER_POOL", "USER_POOL_ONLY"]
 AuthenticatedElementType = Literal["CREATE_AND_UPDATE", "DELETE", "READ"]
 DeliveryMethodType = Literal["EMAIL", "SMS"]
 ListBackendJobsPaginatorName = Literal["list_backend_jobs"]
@@ -96,14 +94,15 @@
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
@@ -124,31 +123,34 @@
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
     "codecatalyst",
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
@@ -227,14 +229,15 @@
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
@@ -245,18 +248,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -287,14 +292,15 @@
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
@@ -313,16 +319,19 @@
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
@@ -402,18 +411,21 @@
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
@@ -441,14 +453,15 @@
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
+    "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
```

### Comparing `mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/literals.pyi` & `mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/literals.py`

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
     "AdditionalConstraintsElementType",
     "AuthResourcesType",
     "AuthenticatedElementType",
     "DeliveryMethodType",
     "ListBackendJobsPaginatorName",
     "MFAModeType",
@@ -39,14 +40,15 @@
     "AmplifyBackendServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AdditionalConstraintsElementType = Literal[
     "REQUIRE_DIGIT", "REQUIRE_LOWERCASE", "REQUIRE_SYMBOL", "REQUIRE_UPPERCASE"
 ]
 AuthResourcesType = Literal["IDENTITY_POOL_AND_USER_POOL", "USER_POOL_ONLY"]
 AuthenticatedElementType = Literal["CREATE_AND_UPDATE", "DELETE", "READ"]
 DeliveryMethodType = Literal["EMAIL", "SMS"]
 ListBackendJobsPaginatorName = Literal["list_backend_jobs"]
@@ -94,14 +96,15 @@
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
@@ -122,31 +125,34 @@
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
     "codecatalyst",
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
@@ -225,14 +231,15 @@
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
@@ -243,18 +250,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -285,14 +294,15 @@
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
@@ -311,16 +321,19 @@
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
@@ -400,18 +413,21 @@
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
@@ -439,14 +455,15 @@
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
+    "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
```

### Comparing `mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/paginator.py` & `mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/paginator.pyi` & `mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/type_defs.py` & `mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend/type_defs.pyi` & `mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend.egg-info/PKG-INFO` & `mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifybackend
-Version: 1.26.44
-Summary: Type annotations for boto3.AmplifyBackend 1.26.44 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.AmplifyBackend 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-amplifybackend"></a>
 
 # mypy-boto3-amplifybackend
 
 [![PyPI - mypy-boto3-amplifybackend](https://img.shields.io/pypi/v/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplifybackend?color=blue)](https://pypistats.org/packages/mypy-boto3-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyBackend 1.26.44](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
+[boto3.AmplifyBackend 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-amplifybackend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -448,42 +448,42 @@
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

### Comparing `mypy-boto3-amplifybackend-1.26.44/mypy_boto3_amplifybackend.egg-info/SOURCES.txt` & `mypy-boto3-amplifybackend-1.27.0/mypy_boto3_amplifybackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.26.44/setup.py` & `mypy-boto3-amplifybackend-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-amplifybackend.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplifybackend",
-    version="1.26.44",
+    version="1.27.0",
     packages=["mypy_boto3_amplifybackend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AmplifyBackend 1.26.44 service generated with"
-        " mypy-boto3-builder 7.12.2"
+        "Type annotations for boto3.AmplifyBackend 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/",
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


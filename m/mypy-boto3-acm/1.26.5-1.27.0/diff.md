# Comparing `tmp/mypy-boto3-acm-1.26.5.tar.gz` & `tmp/mypy-boto3-acm-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-acm-1.26.5.tar", last modified: Tue Nov  8 20:33:28 2022, max compression
+gzip compressed data, was "mypy-boto3-acm-1.27.0.tar", last modified: Mon Jul  3 19:50:17 2023, max compression
```

## Comparing `mypy-boto3-acm-1.26.5.tar` & `mypy-boto3-acm-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 20:33:28.873201 mypy-boto3-acm-1.26.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-08 20:32:18.000000 mypy-boto3-acm-1.26.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14761 2022-11-08 20:33:28.873201 mypy-boto3-acm-1.26.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13342 2022-11-08 20:32:18.000000 mypy-boto3-acm-1.26.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 20:33:28.861201 mypy-boto3-acm-1.26.5/mypy_boto3_acm/
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-11-08 20:32:18.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-11-08 20:32:18.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-11-08 20:32:18.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13747 2022-11-08 20:32:19.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    13723 2022-11-08 20:32:18.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10177 2022-11-08 20:32:19.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    10175 2022-11-08 20:32:19.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-11-08 20:32:19.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2199 2022-11-08 20:32:19.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-08 20:32:18.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    14779 2022-11-08 20:32:19.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    14764 2022-11-08 20:32:19.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-08 20:32:18.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1399 2022-11-08 20:32:19.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-11-08 20:32:19.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 20:33:28.873201 mypy-boto3-acm-1.26.5/mypy_boto3_acm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14761 2022-11-08 20:33:28.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-11-08 20:33:28.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 20:33:28.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 20:33:28.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-08 20:33:28.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-08 20:33:28.000000 mypy-boto3-acm-1.26.5/mypy_boto3_acm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-08 20:33:28.873201 mypy-boto3-acm-1.26.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-11-08 20:32:18.000000 mypy-boto3-acm-1.26.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:17.758734 mypy-boto3-acm-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:31:57.000000 mypy-boto3-acm-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-07-03 19:50:17.754734 mypy-boto3-acm-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-07-03 19:31:57.000000 mypy-boto3-acm-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:17.750733 mypy-boto3-acm-1.27.0/mypy_boto3_acm/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 19:31:57.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-03 19:31:57.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:31:57.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-07-03 19:31:57.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-03 19:31:57.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-07-03 19:31:58.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10933 2023-07-03 19:31:58.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-03 19:31:57.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-03 19:31:57.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:31:57.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-07-03 19:31:58.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-07-03 19:31:58.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:31:57.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-03 19:31:57.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-03 19:31:57.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:17.754734 mypy-boto3-acm-1.27.0/mypy_boto3_acm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-07-03 19:50:17.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 19:50:17.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:17.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:17.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:17.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:17.000000 mypy-boto3-acm-1.27.0/mypy_boto3_acm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:17.758734 mypy-boto3-acm-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:31:57.000000 mypy-boto3-acm-1.27.0/setup.py
```

### Comparing `mypy-boto3-acm-1.26.5/LICENSE` & `mypy-boto3-acm-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-acm-1.26.5/PKG-INFO` & `mypy-boto3-acm-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm
-Version: 1.26.5
-Summary: Type annotations for boto3.ACM 1.26.5 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ACM 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/
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
 
 <a id="mypy-boto3-acm"></a>
 
 # mypy-boto3-acm
 
 [![PyPI - mypy-boto3-acm](https://img.shields.io/pypi/v/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-acm?color=blue)](https://pypistats.org/packages/mypy-boto3-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACM 1.26.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[boto3.ACM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -409,42 +410,42 @@
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

### Comparing `mypy-boto3-acm-1.26.5/README.md` & `mypy-boto3-acm-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-acm"></a>
 
 # mypy-boto3-acm
 
 [![PyPI - mypy-boto3-acm](https://img.shields.io/pypi/v/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-acm?color=blue)](https://pypistats.org/packages/mypy-boto3-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACM 1.26.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[boto3.ACM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -378,42 +378,42 @@
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

### Comparing `mypy-boto3-acm-1.26.5/mypy_boto3_acm/__init__.py` & `mypy-boto3-acm-1.27.0/mypy_boto3_acm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.26.5/mypy_boto3_acm/__init__.pyi` & `mypy-boto3-acm-1.27.0/mypy_boto3_acm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.26.5/mypy_boto3_acm/__main__.py` & `mypy-boto3-acm-1.27.0/mypy_boto3_acm/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ACM 1.26.5\nVersion:         1.26.5\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.ACM 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.5")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-acm-1.26.5/mypy_boto3_acm/client.py` & `mypy-boto3-acm-1.27.0/mypy_boto3_acm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.26.5/mypy_boto3_acm/client.pyi` & `mypy-boto3-acm-1.27.0/mypy_boto3_acm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.26.5/mypy_boto3_acm/literals.py` & `mypy-boto3-acm-1.27.0/mypy_boto3_acm/literals.pyi`

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
     "CertificateStatusType",
     "CertificateTransparencyLoggingPreferenceType",
     "CertificateTypeType",
     "CertificateValidatedWaiterName",
     "DomainStatusType",
     "ExtendedKeyUsageNameType",
@@ -41,15 +40,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 CertificateStatusType = Literal[
     "EXPIRED",
     "FAILED",
     "INACTIVE",
     "ISSUED",
     "PENDING_VALIDATION",
     "REVOKED",
@@ -139,23 +137,25 @@
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
@@ -165,30 +165,35 @@
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
@@ -214,14 +219,15 @@
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
@@ -266,51 +272,57 @@
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
@@ -323,14 +335,15 @@
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
@@ -342,28 +355,35 @@
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
@@ -391,55 +411,64 @@
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
@@ -466,21 +495,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-acm-1.26.5/mypy_boto3_acm/literals.pyi` & `mypy-boto3-acm-1.27.0/mypy_boto3_acm/literals.py`

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
     "CertificateStatusType",
     "CertificateTransparencyLoggingPreferenceType",
     "CertificateTypeType",
     "CertificateValidatedWaiterName",
     "DomainStatusType",
     "ExtendedKeyUsageNameType",
@@ -40,14 +41,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 CertificateStatusType = Literal[
     "EXPIRED",
     "FAILED",
     "INACTIVE",
     "ISSUED",
     "PENDING_VALIDATION",
     "REVOKED",
@@ -137,23 +139,25 @@
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
@@ -163,30 +167,35 @@
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
@@ -212,14 +221,15 @@
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
@@ -264,51 +274,57 @@
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
@@ -321,14 +337,15 @@
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
@@ -340,28 +357,35 @@
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
@@ -389,55 +413,64 @@
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
@@ -464,21 +497,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-acm-1.26.5/mypy_boto3_acm/paginator.py` & `mypy-boto3-acm-1.27.0/mypy_boto3_acm/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.26.5/mypy_boto3_acm/paginator.pyi` & `mypy-boto3-acm-1.27.0/mypy_boto3_acm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.26.5/mypy_boto3_acm/type_defs.py` & `mypy-boto3-acm-1.27.0/mypy_boto3_acm/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.26.5/mypy_boto3_acm/type_defs.pyi` & `mypy-boto3-acm-1.27.0/mypy_boto3_acm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.26.5/mypy_boto3_acm/waiter.py` & `mypy-boto3-acm-1.27.0/mypy_boto3_acm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.26.5/mypy_boto3_acm/waiter.pyi` & `mypy-boto3-acm-1.27.0/mypy_boto3_acm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.26.5/mypy_boto3_acm.egg-info/PKG-INFO` & `mypy-boto3-acm-1.27.0/mypy_boto3_acm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm
-Version: 1.26.5
-Summary: Type annotations for boto3.ACM 1.26.5 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ACM 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/
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
 
 <a id="mypy-boto3-acm"></a>
 
 # mypy-boto3-acm
 
 [![PyPI - mypy-boto3-acm](https://img.shields.io/pypi/v/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-acm?color=blue)](https://pypistats.org/packages/mypy-boto3-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACM 1.26.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[boto3.ACM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -409,42 +410,42 @@
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

### Comparing `mypy-boto3-acm-1.26.5/mypy_boto3_acm.egg-info/SOURCES.txt` & `mypy-boto3-acm-1.27.0/mypy_boto3_acm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.26.5/setup.py` & `mypy-boto3-acm-1.27.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-acm.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-acm",
-    version="1.26.5",
+    version="1.27.0",
     packages=["mypy_boto3_acm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ACM 1.26.5 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.ACM 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 acm type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_acm": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_acm": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/",
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


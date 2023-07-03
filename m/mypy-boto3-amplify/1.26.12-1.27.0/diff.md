# Comparing `tmp/mypy-boto3-amplify-1.26.12.tar.gz` & `tmp/mypy-boto3-amplify-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplify-1.26.12.tar", last modified: Thu Nov 17 20:31:18 2022, max compression
+gzip compressed data, was "mypy-boto3-amplify-1.27.0.tar", last modified: Mon Jul  3 19:50:17 2023, max compression
```

## Comparing `mypy-boto3-amplify-1.26.12.tar` & `mypy-boto3-amplify-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:31:18.600782 mypy-boto3-amplify-1.26.12/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-17 20:29:11.000000 mypy-boto3-amplify-1.26.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16297 2022-11-17 20:31:18.600782 mypy-boto3-amplify-1.26.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14860 2022-11-17 20:29:11.000000 mypy-boto3-amplify-1.26.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:31:18.600782 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-11-17 20:29:11.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-11-17 20:29:11.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-11-17 20:29:11.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27948 2022-11-17 20:29:11.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    27900 2022-11-17 20:29:11.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8448 2022-11-17 20:29:11.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8446 2022-11-17 20:29:11.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4839 2022-11-17 20:29:11.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4833 2022-11-17 20:29:11.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 20:29:11.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    35266 2022-11-17 20:29:13.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    35207 2022-11-17 20:29:12.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-17 20:29:11.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:31:18.600782 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16297 2022-11-17 20:31:18.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-11-17 20:31:18.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 20:31:18.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 20:31:18.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-17 20:31:18.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-17 20:31:18.000000 mypy-boto3-amplify-1.26.12/mypy_boto3_amplify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 20:31:18.600782 mypy-boto3-amplify-1.26.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1964 2022-11-17 20:29:10.000000 mypy-boto3-amplify-1.26.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:17.742733 mypy-boto3-amplify-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:06.000000 mypy-boto3-amplify-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-03 19:50:17.742733 mypy-boto3-amplify-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14837 2023-07-03 19:32:06.000000 mypy-boto3-amplify-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:17.742733 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-03 19:32:06.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-03 19:32:06.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:32:06.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27948 2023-07-03 19:32:06.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27900 2023-07-03 19:32:06.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-07-03 19:32:06.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-07-03 19:32:06.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-03 19:32:06.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-03 19:32:06.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:06.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35266 2023-07-03 19:32:07.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35207 2023-07-03 19:32:06.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:06.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:17.742733 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-03 19:50:17.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-03 19:50:17.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:17.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:17.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:17.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:50:17.000000 mypy-boto3-amplify-1.27.0/mypy_boto3_amplify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:17.758734 mypy-boto3-amplify-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:32:06.000000 mypy-boto3-amplify-1.27.0/setup.py
```

### Comparing `mypy-boto3-amplify-1.26.12/LICENSE` & `mypy-boto3-amplify-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-amplify-1.26.12/PKG-INFO` & `mypy-boto3-amplify-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplify
-Version: 1.26.12
-Summary: Type annotations for boto3.Amplify 1.26.12 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Amplify 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/
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
 
 <a id="mypy-boto3-amplify"></a>
 
 # mypy-boto3-amplify
 
 [![PyPI - mypy-boto3-amplify](https://img.shields.io/pypi/v/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplify?color=blue)](https://pypistats.org/packages/mypy-boto3-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Amplify 1.26.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[boto3.Amplify 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
 See how it helps to find and fix potential bugs:
 
@@ -442,42 +443,42 @@
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

### Comparing `mypy-boto3-amplify-1.26.12/README.md` & `mypy-boto3-amplify-1.27.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-amplify"></a>
 
 # mypy-boto3-amplify
 
 [![PyPI - mypy-boto3-amplify](https://img.shields.io/pypi/v/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplify?color=blue)](https://pypistats.org/packages/mypy-boto3-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Amplify 1.26.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[boto3.Amplify 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
 See how it helps to find and fix potential bugs:
 
@@ -411,42 +411,42 @@
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

### Comparing `mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/__init__.py` & `mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/__init__.pyi` & `mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/__main__.py` & `mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Amplify 1.26.12\nVersion:         1.26.12\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.Amplify 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.12")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/client.py` & `mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/client.pyi` & `mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/literals.py` & `mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DomainStatusType",
     "JobStatusType",
     "JobTypeType",
     "ListAppsPaginatorName",
     "ListBranchesPaginatorName",
     "ListDomainAssociationsPaginatorName",
@@ -33,15 +32,14 @@
     "AmplifyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DomainStatusType = Literal[
     "AVAILABLE",
     "CREATING",
     "FAILED",
     "IN_PROGRESS",
     "PENDING_DEPLOYMENT",
     "PENDING_VERIFICATION",
@@ -71,23 +69,25 @@
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
@@ -97,30 +97,35 @@
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
@@ -146,14 +151,15 @@
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
@@ -198,51 +204,57 @@
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
@@ -255,14 +267,15 @@
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
@@ -274,28 +287,35 @@
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
@@ -323,57 +343,64 @@
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

### Comparing `mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/literals.pyi` & `mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DomainStatusType",
     "JobStatusType",
     "JobTypeType",
     "ListAppsPaginatorName",
     "ListBranchesPaginatorName",
     "ListDomainAssociationsPaginatorName",
@@ -32,14 +33,15 @@
     "AmplifyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DomainStatusType = Literal[
     "AVAILABLE",
     "CREATING",
     "FAILED",
     "IN_PROGRESS",
     "PENDING_DEPLOYMENT",
     "PENDING_VERIFICATION",
@@ -69,23 +71,25 @@
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
@@ -95,30 +99,35 @@
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
@@ -144,14 +153,15 @@
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
@@ -196,51 +206,57 @@
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
@@ -253,14 +269,15 @@
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
@@ -272,28 +289,35 @@
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
@@ -321,57 +345,64 @@
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

### Comparing `mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/paginator.py` & `mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/paginator.pyi` & `mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/type_defs.py` & `mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.26.12/mypy_boto3_amplify/type_defs.pyi` & `mypy-boto3-amplify-1.27.0/mypy_boto3_amplify/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.26.12/mypy_boto3_amplify.egg-info/PKG-INFO` & `mypy-boto3-amplify-1.27.0/mypy_boto3_amplify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplify
-Version: 1.26.12
-Summary: Type annotations for boto3.Amplify 1.26.12 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Amplify 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/
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
 
 <a id="mypy-boto3-amplify"></a>
 
 # mypy-boto3-amplify
 
 [![PyPI - mypy-boto3-amplify](https://img.shields.io/pypi/v/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplify?color=blue)](https://pypistats.org/packages/mypy-boto3-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Amplify 1.26.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[boto3.Amplify 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
 See how it helps to find and fix potential bugs:
 
@@ -442,42 +443,42 @@
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

### Comparing `mypy-boto3-amplify-1.26.12/mypy_boto3_amplify.egg-info/SOURCES.txt` & `mypy-boto3-amplify-1.27.0/mypy_boto3_amplify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.26.12/setup.py` & `mypy-boto3-amplify-1.27.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 """
 Setup script for mypy-boto3-amplify.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplify",
-    version="1.26.12",
+    version="1.27.0",
     packages=["mypy_boto3_amplify"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Amplify 1.26.12 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.Amplify 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 amplify type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_amplify": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_amplify": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/",
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


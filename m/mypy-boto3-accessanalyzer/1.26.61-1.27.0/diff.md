# Comparing `tmp/mypy-boto3-accessanalyzer-1.26.61.tar.gz` & `tmp/mypy-boto3-accessanalyzer-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-accessanalyzer-1.26.61.tar", last modified: Tue Jan 31 20:49:53 2023, max compression
+gzip compressed data, was "mypy-boto3-accessanalyzer-1.27.0.tar", last modified: Mon Jul  3 19:50:17 2023, max compression
```

## Comparing `mypy-boto3-accessanalyzer-1.26.61.tar` & `mypy-boto3-accessanalyzer-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:53.638128 mypy-boto3-accessanalyzer-1.26.61/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-31 20:47:17.000000 mypy-boto3-accessanalyzer-1.26.61/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18857 2023-01-31 20:49:53.630128 mypy-boto3-accessanalyzer-1.26.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17342 2023-01-31 20:47:17.000000 mypy-boto3-accessanalyzer-1.26.61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:53.626128 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-01-31 20:47:17.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-01-31 20:47:17.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-01-31 20:47:17.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24749 2023-01-31 20:47:17.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24706 2023-01-31 20:47:17.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11811 2023-01-31 20:47:17.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-01-31 20:47:17.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-01-31 20:47:17.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-01-31 20:47:17.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:47:17.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42667 2023-01-31 20:47:18.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42588 2023-01-31 20:47:18.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-31 20:47:17.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:53.630128 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18857 2023-01-31 20:49:53.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-31 20:49:53.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:53.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:53.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 20:49:53.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-31 20:49:53.000000 mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 20:49:53.638128 mypy-boto3-accessanalyzer-1.26.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-01-31 20:47:17.000000 mypy-boto3-accessanalyzer-1.26.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:17.762734 mypy-boto3-accessanalyzer-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:31:54.000000 mypy-boto3-accessanalyzer-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18840 2023-07-03 19:50:17.762734 mypy-boto3-accessanalyzer-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-07-03 19:31:54.000000 mypy-boto3-accessanalyzer-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:17.754734 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-03 19:31:54.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-03 19:31:54.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-03 19:31:54.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24748 2023-07-03 19:31:54.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24705 2023-07-03 19:31:54.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-07-03 19:31:55.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-07-03 19:31:54.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-03 19:31:54.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-07-03 19:31:54.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:31:54.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42667 2023-07-03 19:31:56.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42588 2023-07-03 19:31:55.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:31:54.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:17.758734 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18840 2023-07-03 19:50:17.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 19:50:17.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:17.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:17.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:17.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:50:17.000000 mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:17.762734 mypy-boto3-accessanalyzer-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-03 19:31:54.000000 mypy-boto3-accessanalyzer-1.27.0/setup.py
```

### Comparing `mypy-boto3-accessanalyzer-1.26.61/LICENSE` & `mypy-boto3-accessanalyzer-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-accessanalyzer-1.26.61/PKG-INFO` & `mypy-boto3-accessanalyzer-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-accessanalyzer
-Version: 1.26.61
-Summary: Type annotations for boto3.AccessAnalyzer 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.AccessAnalyzer 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-accessanalyzer"></a>
 
 # mypy-boto3-accessanalyzer
 
 [![PyPI - mypy-boto3-accessanalyzer](https://img.shields.io/pypi/v/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-accessanalyzer?color=blue)](https://pypistats.org/packages/mypy-boto3-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AccessAnalyzer 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[boto3.AccessAnalyzer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-accessanalyzer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -496,42 +496,42 @@
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

### Comparing `mypy-boto3-accessanalyzer-1.26.61/README.md` & `mypy-boto3-accessanalyzer-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-accessanalyzer"></a>
 
 # mypy-boto3-accessanalyzer
 
 [![PyPI - mypy-boto3-accessanalyzer](https://img.shields.io/pypi/v/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-accessanalyzer?color=blue)](https://pypistats.org/packages/mypy-boto3-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AccessAnalyzer 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[boto3.AccessAnalyzer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-accessanalyzer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -464,42 +464,42 @@
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

### Comparing `mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/__init__.py` & `mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/__init__.pyi` & `mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/__main__.py` & `mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AccessAnalyzer 1.26.61\nVersion:         1.26.61\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.AccessAnalyzer 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.61")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/client.py` & `mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
         self,
         *,
         jobId: str,
         includeResourcePlaceholders: bool = ...,
         includeServiceLevelTemplate: bool = ...
     ) -> GetGeneratedPolicyResponseTypeDef:
         """
-        Retrieves the policy that was generated using `StartPolicyGeneration` .
+        Retrieves the policy that was generated using `StartPolicyGeneration`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.get_generated_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#get_generated_policy)
         """
 
     def list_access_preview_findings(
         self,
```

### Comparing `mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/client.pyi` & `mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
         self,
         *,
         jobId: str,
         includeResourcePlaceholders: bool = ...,
         includeServiceLevelTemplate: bool = ...
     ) -> GetGeneratedPolicyResponseTypeDef:
         """
-        Retrieves the policy that was generated using `StartPolicyGeneration` .
+        Retrieves the policy that was generated using `StartPolicyGeneration`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client.get_generated_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/client/#get_generated_policy)
         """
     def list_access_preview_findings(
         self,
         *,
```

### Comparing `mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/literals.py` & `mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/literals.pyi`

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
     "AccessPreviewStatusReasonCodeType",
     "AccessPreviewStatusType",
     "AclPermissionType",
     "AnalyzerStatusType",
     "FindingChangeTypeType",
     "FindingSourceTypeType",
@@ -50,15 +49,14 @@
     "AccessAnalyzerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AccessPreviewStatusReasonCodeType = Literal["INTERNAL_ERROR", "INVALID_CONFIGURATION"]
 AccessPreviewStatusType = Literal["COMPLETED", "CREATING", "FAILED"]
 AclPermissionType = Literal["FULL_CONTROL", "READ", "READ_ACP", "WRITE", "WRITE_ACP"]
 AnalyzerStatusType = Literal["ACTIVE", "CREATING", "DISABLED", "FAILED"]
 FindingChangeTypeType = Literal["CHANGED", "NEW", "UNCHANGED"]
 FindingSourceTypeType = Literal[
     "BUCKET_ACL", "POLICY", "S3_ACCESS_POINT", "S3_ACCESS_POINT_ACCOUNT"
@@ -141,14 +139,15 @@
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
@@ -188,14 +187,15 @@
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
@@ -274,14 +274,15 @@
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
@@ -292,14 +293,15 @@
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
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -335,14 +337,15 @@
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
@@ -361,16 +364,19 @@
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
@@ -450,18 +456,21 @@
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

### Comparing `mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/literals.pyi` & `mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/literals.py`

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
     "AccessPreviewStatusReasonCodeType",
     "AccessPreviewStatusType",
     "AclPermissionType",
     "AnalyzerStatusType",
     "FindingChangeTypeType",
     "FindingSourceTypeType",
@@ -49,14 +50,15 @@
     "AccessAnalyzerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AccessPreviewStatusReasonCodeType = Literal["INTERNAL_ERROR", "INVALID_CONFIGURATION"]
 AccessPreviewStatusType = Literal["COMPLETED", "CREATING", "FAILED"]
 AclPermissionType = Literal["FULL_CONTROL", "READ", "READ_ACP", "WRITE", "WRITE_ACP"]
 AnalyzerStatusType = Literal["ACTIVE", "CREATING", "DISABLED", "FAILED"]
 FindingChangeTypeType = Literal["CHANGED", "NEW", "UNCHANGED"]
 FindingSourceTypeType = Literal[
     "BUCKET_ACL", "POLICY", "S3_ACCESS_POINT", "S3_ACCESS_POINT_ACCOUNT"
@@ -139,14 +141,15 @@
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
@@ -186,14 +189,15 @@
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
@@ -272,14 +276,15 @@
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
@@ -290,14 +295,15 @@
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
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -333,14 +339,15 @@
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
@@ -359,16 +366,19 @@
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
@@ -448,18 +458,21 @@
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

### Comparing `mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/paginator.py` & `mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/paginator.pyi` & `mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/type_defs.py` & `mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer/type_defs.pyi` & `mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer.egg-info/PKG-INFO` & `mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-accessanalyzer
-Version: 1.26.61
-Summary: Type annotations for boto3.AccessAnalyzer 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.AccessAnalyzer 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-accessanalyzer"></a>
 
 # mypy-boto3-accessanalyzer
 
 [![PyPI - mypy-boto3-accessanalyzer](https://img.shields.io/pypi/v/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-accessanalyzer?color=blue)](https://pypistats.org/packages/mypy-boto3-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AccessAnalyzer 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[boto3.AccessAnalyzer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-accessanalyzer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -496,42 +496,42 @@
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

### Comparing `mypy-boto3-accessanalyzer-1.26.61/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt` & `mypy-boto3-accessanalyzer-1.27.0/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.26.61/setup.py` & `mypy-boto3-accessanalyzer-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-accessanalyzer.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-accessanalyzer",
-    version="1.26.61",
+    version="1.27.0",
     packages=["mypy_boto3_accessanalyzer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AccessAnalyzer 1.26.61 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.AccessAnalyzer 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/",
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


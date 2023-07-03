# Comparing `tmp/mypy-boto3-cloud9-1.26.51.tar.gz` & `tmp/mypy-boto3-cloud9-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloud9-1.26.51.tar", last modified: Tue Jan 17 20:24:22 2023, max compression
+gzip compressed data, was "mypy-boto3-cloud9-1.27.0.tar", last modified: Mon Jul  3 19:50:29 2023, max compression
```

## Comparing `mypy-boto3-cloud9-1.26.51.tar` & `mypy-boto3-cloud9-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:22.391515 mypy-boto3-cloud9-1.26.51/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-17 20:24:07.000000 mypy-boto3-cloud9-1.26.51/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-01-17 20:24:22.391515 mypy-boto3-cloud9-1.26.51/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-01-17 20:24:07.000000 mypy-boto3-cloud9-1.26.51/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:22.391515 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-17 20:24:07.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-17 20:24:07.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-17 20:24:07.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-01-17 20:24:08.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-01-17 20:24:07.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-01-17 20:24:08.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9188 2023-01-17 20:24:08.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-01-17 20:24:08.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-01-17 20:24:08.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:07.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-01-17 20:24:08.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-01-17 20:24:08.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-17 20:24:07.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:22.391515 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-01-17 20:24:22.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-17 20:24:22.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 20:24:22.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 20:24:22.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-17 20:24:22.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-17 20:24:22.000000 mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 20:24:22.391515 mypy-boto3-cloud9-1.26.51/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-01-17 20:24:07.000000 mypy-boto3-cloud9-1.26.51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.162939 mypy-boto3-cloud9-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:35.000000 mypy-boto3-cloud9-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-07-03 19:50:29.162939 mypy-boto3-cloud9-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-07-03 19:33:35.000000 mypy-boto3-cloud9-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.162939 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-03 19:33:35.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-03 19:33:35.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-03 19:33:35.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-03 19:33:35.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-07-03 19:33:35.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-07-03 19:33:35.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-07-03 19:33:35.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-03 19:33:35.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-03 19:33:35.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:35.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-07-03 19:33:36.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-07-03 19:33:35.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:35.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.162939 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-07-03 19:50:29.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 19:50:29.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:29.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:29.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:29.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 19:50:29.000000 mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:29.162939 mypy-boto3-cloud9-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 19:33:35.000000 mypy-boto3-cloud9-1.27.0/setup.py
```

### Comparing `mypy-boto3-cloud9-1.26.51/LICENSE` & `mypy-boto3-cloud9-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-cloud9-1.26.51/PKG-INFO` & `mypy-boto3-cloud9-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloud9
-Version: 1.26.51
-Summary: Type annotations for boto3.Cloud9 1.26.51 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Cloud9 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-cloud9"></a>
 
 # mypy-boto3-cloud9
 
 [![PyPI - mypy-boto3-cloud9](https://img.shields.io/pypi/v/mypy-boto3-cloud9.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloud9)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloud9.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloud9)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloud9?color=blue)](https://pypistats.org/packages/mypy-boto3-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Cloud9 1.26.51](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
+[boto3.Cloud9 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
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
 [mypy-boto3-cloud9 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,40 +334,40 @@
 
 `mypy_boto3_cloud9.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloud9.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateEnvironmentEC2ResultTypeDef,
     CreateEnvironmentMembershipRequestRequestTypeDef,
     EnvironmentMemberTypeDef,
     DeleteEnvironmentMembershipRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
     DescribeEnvironmentMembershipsRequestRequestTypeDef,
     DescribeEnvironmentStatusRequestRequestTypeDef,
+    DescribeEnvironmentStatusResultTypeDef,
     DescribeEnvironmentsRequestRequestTypeDef,
     EnvironmentLifecycleTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
+    ListEnvironmentsResultTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEnvironmentMembershipRequestRequestTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentEC2RequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateEnvironmentEC2ResultTypeDef,
-    DescribeEnvironmentStatusResultTypeDef,
-    ListEnvironmentsResultTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateEnvironmentMembershipResultTypeDef,
     DescribeEnvironmentMembershipsResultTypeDef,
     UpdateEnvironmentMembershipResultTypeDef,
-    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     EnvironmentTypeDef,
     DescribeEnvironmentsResultTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
@@ -376,42 +376,42 @@
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

### Comparing `mypy-boto3-cloud9-1.26.51/README.md` & `mypy-boto3-cloud9-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cloud9"></a>
 
 # mypy-boto3-cloud9
 
 [![PyPI - mypy-boto3-cloud9](https://img.shields.io/pypi/v/mypy-boto3-cloud9.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloud9)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloud9.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloud9)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloud9?color=blue)](https://pypistats.org/packages/mypy-boto3-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Cloud9 1.26.51](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
+[boto3.Cloud9 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
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
 [mypy-boto3-cloud9 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,40 +302,40 @@
 
 `mypy_boto3_cloud9.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloud9.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateEnvironmentEC2ResultTypeDef,
     CreateEnvironmentMembershipRequestRequestTypeDef,
     EnvironmentMemberTypeDef,
     DeleteEnvironmentMembershipRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
     DescribeEnvironmentMembershipsRequestRequestTypeDef,
     DescribeEnvironmentStatusRequestRequestTypeDef,
+    DescribeEnvironmentStatusResultTypeDef,
     DescribeEnvironmentsRequestRequestTypeDef,
     EnvironmentLifecycleTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
+    ListEnvironmentsResultTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEnvironmentMembershipRequestRequestTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentEC2RequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateEnvironmentEC2ResultTypeDef,
-    DescribeEnvironmentStatusResultTypeDef,
-    ListEnvironmentsResultTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateEnvironmentMembershipResultTypeDef,
     DescribeEnvironmentMembershipsResultTypeDef,
     UpdateEnvironmentMembershipResultTypeDef,
-    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     EnvironmentTypeDef,
     DescribeEnvironmentsResultTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
@@ -344,42 +344,42 @@
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

### Comparing `mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/__init__.py` & `mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/__init__.pyi` & `mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/__main__.py` & `mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Cloud9 1.26.51\nVersion:         1.26.51\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Cloud9 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.51")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/client.py` & `mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/client.pyi` & `mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/literals.py` & `mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
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
@@ -115,21 +116,23 @@
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
@@ -208,14 +211,15 @@
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
@@ -226,14 +230,15 @@
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
@@ -269,14 +274,15 @@
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
@@ -295,16 +301,19 @@
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
@@ -384,18 +393,21 @@
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

### Comparing `mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/literals.pyi` & `mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
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
@@ -113,21 +114,23 @@
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
@@ -206,14 +209,15 @@
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
@@ -224,14 +228,15 @@
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
@@ -267,14 +272,15 @@
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
@@ -293,16 +299,19 @@
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
@@ -382,18 +391,21 @@
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

### Comparing `mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/paginator.py` & `mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,28 +53,28 @@
 
     def paginate(
         self,
         *,
         userArn: str = ...,
         environmentId: str = ...,
         permissions: Sequence[PermissionsType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEnvironmentMembershipsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.DescribeEnvironmentMemberships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/paginators/#describeenvironmentmembershipspaginator)
         """
 
 
 class ListEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.ListEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/paginators/#listenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/paginator.pyi` & `mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -50,27 +50,27 @@
 
     def paginate(
         self,
         *,
         userArn: str = ...,
         environmentId: str = ...,
         permissions: Sequence[PermissionsType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEnvironmentMembershipsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.DescribeEnvironmentMemberships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/paginators/#describeenvironmentmembershipspaginator)
         """
 
 class ListEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.ListEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/paginators/#listenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/type_defs.py` & `mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -27,63 +27,59 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateEnvironmentEC2ResultTypeDef",
     "CreateEnvironmentMembershipRequestRequestTypeDef",
     "EnvironmentMemberTypeDef",
     "DeleteEnvironmentMembershipRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
     "DescribeEnvironmentMembershipsRequestRequestTypeDef",
     "DescribeEnvironmentStatusRequestRequestTypeDef",
+    "DescribeEnvironmentStatusResultTypeDef",
     "DescribeEnvironmentsRequestRequestTypeDef",
     "EnvironmentLifecycleTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
+    "ListEnvironmentsResultTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEnvironmentMembershipRequestRequestTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentEC2RequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateEnvironmentEC2ResultTypeDef",
-    "DescribeEnvironmentStatusResultTypeDef",
-    "ListEnvironmentsResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateEnvironmentMembershipResultTypeDef",
     "DescribeEnvironmentMembershipsResultTypeDef",
     "UpdateEnvironmentMembershipResultTypeDef",
-    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "EnvironmentTypeDef",
     "DescribeEnvironmentsResultTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateEnvironmentEC2ResultTypeDef = TypedDict(
+    "CreateEnvironmentEC2ResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "environmentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEnvironmentMembershipRequestRequestTypeDef = TypedDict(
     "CreateEnvironmentMembershipRequestRequestTypeDef",
     {
         "environmentId": str,
@@ -105,21 +101,19 @@
     "_OptionalEnvironmentMemberTypeDef",
     {
         "lastAccess": datetime,
     },
     total=False,
 )
 
-
 class EnvironmentMemberTypeDef(
     _RequiredEnvironmentMemberTypeDef, _OptionalEnvironmentMemberTypeDef
 ):
     pass
 
-
 DeleteEnvironmentMembershipRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentMembershipRequestRequestTypeDef",
     {
         "environmentId": str,
         "userArn": str,
     },
 )
@@ -127,20 +121,21 @@
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "userArn": str,
+        "environmentId": str,
+        "permissions": Sequence[PermissionsType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeEnvironmentMembershipsRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentMembershipsRequestRequestTypeDef",
     {
@@ -156,14 +151,23 @@
 DescribeEnvironmentStatusRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentStatusRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
+DescribeEnvironmentStatusResultTypeDef = TypedDict(
+    "DescribeEnvironmentStatusResultTypeDef",
+    {
+        "status": EnvironmentStatusType,
+        "message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeEnvironmentsRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentsRequestRequestTypeDef",
     {
         "environmentIds": Sequence[str],
     },
 )
 
@@ -173,30 +177,68 @@
         "status": EnvironmentLifecycleStatusType,
         "reason": str,
         "failureResource": str,
     },
     total=False,
 )
 
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListEnvironmentsResultTypeDef = TypedDict(
+    "ListEnvironmentsResultTypeDef",
+    {
+        "nextToken": str,
+        "environmentIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -222,21 +264,19 @@
         "name": str,
         "description": str,
         "managedCredentialsAction": ManagedCredentialsActionType,
     },
     total=False,
 )
 
-
 class UpdateEnvironmentRequestRequestTypeDef(
     _RequiredUpdateEnvironmentRequestRequestTypeDef, _OptionalUpdateEnvironmentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateEnvironmentEC2RequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentEC2RequestRequestTypeDef",
     {
         "name": str,
         "instanceType": str,
     },
 )
@@ -252,108 +292,61 @@
         "tags": Sequence[TagTypeDef],
         "connectionType": ConnectionTypeType,
         "dryRun": bool,
     },
     total=False,
 )
 
-
 class CreateEnvironmentEC2RequestRequestTypeDef(
     _RequiredCreateEnvironmentEC2RequestRequestTypeDef,
     _OptionalCreateEnvironmentEC2RequestRequestTypeDef,
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-CreateEnvironmentEC2ResultTypeDef = TypedDict(
-    "CreateEnvironmentEC2ResultTypeDef",
-    {
-        "environmentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeEnvironmentStatusResultTypeDef = TypedDict(
-    "DescribeEnvironmentStatusResultTypeDef",
-    {
-        "status": EnvironmentStatusType,
-        "message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListEnvironmentsResultTypeDef = TypedDict(
-    "ListEnvironmentsResultTypeDef",
-    {
-        "nextToken": str,
-        "environmentIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateEnvironmentMembershipResultTypeDef = TypedDict(
     "CreateEnvironmentMembershipResultTypeDef",
     {
         "membership": EnvironmentMemberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEnvironmentMembershipsResultTypeDef = TypedDict(
     "DescribeEnvironmentMembershipsResultTypeDef",
     {
         "memberships": List[EnvironmentMemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEnvironmentMembershipResultTypeDef = TypedDict(
     "UpdateEnvironmentMembershipResultTypeDef",
     {
         "membership": EnvironmentMemberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
-    {
-        "userArn": str,
-        "environmentId": str,
-        "permissions": Sequence[PermissionsType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredEnvironmentTypeDef = TypedDict(
     "_RequiredEnvironmentTypeDef",
     {
         "type": EnvironmentTypeType,
         "arn": str,
         "ownerArn": str,
     },
@@ -367,19 +360,17 @@
         "connectionType": ConnectionTypeType,
         "lifecycle": EnvironmentLifecycleTypeDef,
         "managedCredentialsStatus": ManagedCredentialsStatusType,
     },
     total=False,
 )
 
-
 class EnvironmentTypeDef(_RequiredEnvironmentTypeDef, _OptionalEnvironmentTypeDef):
     pass
 
-
 DescribeEnvironmentsResultTypeDef = TypedDict(
     "DescribeEnvironmentsResultTypeDef",
     {
         "environments": List[EnvironmentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9/type_defs.pyi` & `mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,62 +27,60 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateEnvironmentEC2ResultTypeDef",
     "CreateEnvironmentMembershipRequestRequestTypeDef",
     "EnvironmentMemberTypeDef",
     "DeleteEnvironmentMembershipRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
     "DescribeEnvironmentMembershipsRequestRequestTypeDef",
     "DescribeEnvironmentStatusRequestRequestTypeDef",
+    "DescribeEnvironmentStatusResultTypeDef",
     "DescribeEnvironmentsRequestRequestTypeDef",
     "EnvironmentLifecycleTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
+    "ListEnvironmentsResultTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEnvironmentMembershipRequestRequestTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentEC2RequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "CreateEnvironmentEC2ResultTypeDef",
-    "DescribeEnvironmentStatusResultTypeDef",
-    "ListEnvironmentsResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateEnvironmentMembershipResultTypeDef",
     "DescribeEnvironmentMembershipsResultTypeDef",
     "UpdateEnvironmentMembershipResultTypeDef",
-    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "EnvironmentTypeDef",
     "DescribeEnvironmentsResultTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateEnvironmentEC2ResultTypeDef = TypedDict(
+    "CreateEnvironmentEC2ResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "environmentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEnvironmentMembershipRequestRequestTypeDef = TypedDict(
     "CreateEnvironmentMembershipRequestRequestTypeDef",
     {
         "environmentId": str,
@@ -104,19 +102,21 @@
     "_OptionalEnvironmentMemberTypeDef",
     {
         "lastAccess": datetime,
     },
     total=False,
 )
 
+
 class EnvironmentMemberTypeDef(
     _RequiredEnvironmentMemberTypeDef, _OptionalEnvironmentMemberTypeDef
 ):
     pass
 
+
 DeleteEnvironmentMembershipRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentMembershipRequestRequestTypeDef",
     {
         "environmentId": str,
         "userArn": str,
     },
 )
@@ -124,20 +124,21 @@
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "userArn": str,
+        "environmentId": str,
+        "permissions": Sequence[PermissionsType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeEnvironmentMembershipsRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentMembershipsRequestRequestTypeDef",
     {
@@ -153,14 +154,23 @@
 DescribeEnvironmentStatusRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentStatusRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
+DescribeEnvironmentStatusResultTypeDef = TypedDict(
+    "DescribeEnvironmentStatusResultTypeDef",
+    {
+        "status": EnvironmentStatusType,
+        "message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeEnvironmentsRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentsRequestRequestTypeDef",
     {
         "environmentIds": Sequence[str],
     },
 )
 
@@ -170,30 +180,68 @@
         "status": EnvironmentLifecycleStatusType,
         "reason": str,
         "failureResource": str,
     },
     total=False,
 )
 
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListEnvironmentsResultTypeDef = TypedDict(
+    "ListEnvironmentsResultTypeDef",
+    {
+        "nextToken": str,
+        "environmentIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -219,19 +267,21 @@
         "name": str,
         "description": str,
         "managedCredentialsAction": ManagedCredentialsActionType,
     },
     total=False,
 )
 
+
 class UpdateEnvironmentRequestRequestTypeDef(
     _RequiredUpdateEnvironmentRequestRequestTypeDef, _OptionalUpdateEnvironmentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateEnvironmentEC2RequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentEC2RequestRequestTypeDef",
     {
         "name": str,
         "instanceType": str,
     },
 )
@@ -247,106 +297,63 @@
         "tags": Sequence[TagTypeDef],
         "connectionType": ConnectionTypeType,
         "dryRun": bool,
     },
     total=False,
 )
 
+
 class CreateEnvironmentEC2RequestRequestTypeDef(
     _RequiredCreateEnvironmentEC2RequestRequestTypeDef,
     _OptionalCreateEnvironmentEC2RequestRequestTypeDef,
 ):
     pass
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-CreateEnvironmentEC2ResultTypeDef = TypedDict(
-    "CreateEnvironmentEC2ResultTypeDef",
-    {
-        "environmentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeEnvironmentStatusResultTypeDef = TypedDict(
-    "DescribeEnvironmentStatusResultTypeDef",
-    {
-        "status": EnvironmentStatusType,
-        "message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-ListEnvironmentsResultTypeDef = TypedDict(
-    "ListEnvironmentsResultTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "nextToken": str,
-        "environmentIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreateEnvironmentMembershipResultTypeDef = TypedDict(
     "CreateEnvironmentMembershipResultTypeDef",
     {
         "membership": EnvironmentMemberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEnvironmentMembershipsResultTypeDef = TypedDict(
     "DescribeEnvironmentMembershipsResultTypeDef",
     {
         "memberships": List[EnvironmentMemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateEnvironmentMembershipResultTypeDef = TypedDict(
     "UpdateEnvironmentMembershipResultTypeDef",
     {
         "membership": EnvironmentMemberTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
-    {
-        "userArn": str,
-        "environmentId": str,
-        "permissions": Sequence[PermissionsType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredEnvironmentTypeDef = TypedDict(
     "_RequiredEnvironmentTypeDef",
     {
         "type": EnvironmentTypeType,
         "arn": str,
         "ownerArn": str,
     },
@@ -360,17 +367,19 @@
         "connectionType": ConnectionTypeType,
         "lifecycle": EnvironmentLifecycleTypeDef,
         "managedCredentialsStatus": ManagedCredentialsStatusType,
     },
     total=False,
 )
 
+
 class EnvironmentTypeDef(_RequiredEnvironmentTypeDef, _OptionalEnvironmentTypeDef):
     pass
 
+
 DescribeEnvironmentsResultTypeDef = TypedDict(
     "DescribeEnvironmentsResultTypeDef",
     {
         "environments": List[EnvironmentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9.egg-info/PKG-INFO` & `mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloud9
-Version: 1.26.51
-Summary: Type annotations for boto3.Cloud9 1.26.51 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.Cloud9 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-cloud9"></a>
 
 # mypy-boto3-cloud9
 
 [![PyPI - mypy-boto3-cloud9](https://img.shields.io/pypi/v/mypy-boto3-cloud9.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloud9)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloud9.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloud9)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloud9?color=blue)](https://pypistats.org/packages/mypy-boto3-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Cloud9 1.26.51](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
+[boto3.Cloud9 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
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
 [mypy-boto3-cloud9 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,40 +334,40 @@
 
 `mypy_boto3_cloud9.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloud9.type_defs import (
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateEnvironmentEC2ResultTypeDef,
     CreateEnvironmentMembershipRequestRequestTypeDef,
     EnvironmentMemberTypeDef,
     DeleteEnvironmentMembershipRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
     DescribeEnvironmentMembershipsRequestRequestTypeDef,
     DescribeEnvironmentStatusRequestRequestTypeDef,
+    DescribeEnvironmentStatusResultTypeDef,
     DescribeEnvironmentsRequestRequestTypeDef,
     EnvironmentLifecycleTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
+    ListEnvironmentsResultTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEnvironmentMembershipRequestRequestTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentEC2RequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateEnvironmentEC2ResultTypeDef,
-    DescribeEnvironmentStatusResultTypeDef,
-    ListEnvironmentsResultTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateEnvironmentMembershipResultTypeDef,
     DescribeEnvironmentMembershipsResultTypeDef,
     UpdateEnvironmentMembershipResultTypeDef,
-    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     EnvironmentTypeDef,
     DescribeEnvironmentsResultTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
@@ -376,42 +376,42 @@
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

### Comparing `mypy-boto3-cloud9-1.26.51/mypy_boto3_cloud9.egg-info/SOURCES.txt` & `mypy-boto3-cloud9-1.27.0/mypy_boto3_cloud9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.26.51/setup.py` & `mypy-boto3-cloud9-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-cloud9.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloud9",
-    version="1.26.51",
+    version="1.27.0",
     packages=["mypy_boto3_cloud9"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Cloud9 1.26.51 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.Cloud9 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -44,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/",
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


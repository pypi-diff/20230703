# Comparing `tmp/mypy-boto3-sso-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-sso-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sso-1.26.0.post1.tar", last modified: Tue Nov  1 21:44:03 2022, max compression
+gzip compressed data, was "mypy-boto3-sso-1.27.0.tar", last modified: Mon Jul  3 19:51:31 2023, max compression
```

## Comparing `mypy-boto3-sso-1.26.0.post1.tar` & `mypy-boto3-sso-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:03.528852 mypy-boto3-sso-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12918 2022-11-01 21:44:03.528852 mypy-boto3-sso-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11493 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:03.528852 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6327 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     6314 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7488 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7486 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2809 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     5355 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5346 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:03.528852 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12918 2022-11-01 21:44:03.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-11-01 21:44:03.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:03.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:03.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:44:03.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-01 21:44:03.000000 mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:44:03.528852 mypy-boto3-sso-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-11-01 21:41:51.000000 mypy-boto3-sso-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:31.472064 mypy-boto3-sso-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:43.000000 mypy-boto3-sso-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-07-03 19:51:31.472064 mypy-boto3-sso-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-07-03 19:48:43.000000 mypy-boto3-sso-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:31.460064 mypy-boto3-sso-1.27.0/mypy_boto3_sso/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-03 19:48:43.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-03 19:48:43.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:48:43.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-03 19:48:43.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-03 19:48:43.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-07-03 19:48:43.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-07-03 19:48:43.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-03 19:48:43.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-03 19:48:43.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:43.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-07-03 19:48:44.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-03 19:48:43.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:43.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:31.472064 mypy-boto3-sso-1.27.0/mypy_boto3_sso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-07-03 19:51:31.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:51:31.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:31.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:31.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:31.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:31.000000 mypy-boto3-sso-1.27.0/mypy_boto3_sso.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:31.472064 mypy-boto3-sso-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:48:43.000000 mypy-boto3-sso-1.27.0/setup.py
```

### Comparing `mypy-boto3-sso-1.26.0.post1/LICENSE` & `mypy-boto3-sso-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-sso-1.26.0.post1/PKG-INFO` & `mypy-boto3-sso-1.27.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.SSO 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.SSO 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/
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
 
 <a id="mypy-boto3-sso"></a>
 
 # mypy-boto3-sso
 
 [![PyPI - mypy-boto3-sso](https://img.shields.io/pypi/v/mypy-boto3-sso.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso?color=blue)](https://pypistats.org/packages/mypy-boto3-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSO 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
+[boto3.SSO 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
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
 [mypy-boto3-sso docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/).
 
 See how it helps to find and fix potential bugs:
 
@@ -319,27 +320,27 @@
 
 `mypy_boto3_sso.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sso.type_defs import (
     AccountInfoTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetRoleCredentialsRequestRequestTypeDef,
     RoleCredentialsTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
     ListAccountRolesRequestRequestTypeDef,
     RoleInfoTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountsRequestRequestTypeDef,
     LogoutRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     ListAccountsResponseTypeDef,
     GetRoleCredentialsResponseTypeDef,
-    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountRolesResponseTypeDef,
 )
 
 
 def get_structure() -> AccountInfoTypeDef:
     return {...}
 ```
@@ -347,42 +348,42 @@
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

### Comparing `mypy-boto3-sso-1.26.0.post1/README.md` & `mypy-boto3-sso-1.27.0/mypy_boto3_sso.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-sso
+Version: 1.27.0
+Summary: Type annotations for boto3.SSO 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 sso type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-sso"></a>
 
 # mypy-boto3-sso
 
 [![PyPI - mypy-boto3-sso](https://img.shields.io/pypi/v/mypy-boto3-sso.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso?color=blue)](https://pypistats.org/packages/mypy-boto3-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSO 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
+[boto3.SSO 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
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
 [mypy-boto3-sso docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,27 +320,27 @@
 
 `mypy_boto3_sso.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sso.type_defs import (
     AccountInfoTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetRoleCredentialsRequestRequestTypeDef,
     RoleCredentialsTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
     ListAccountRolesRequestRequestTypeDef,
     RoleInfoTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountsRequestRequestTypeDef,
     LogoutRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     ListAccountsResponseTypeDef,
     GetRoleCredentialsResponseTypeDef,
-    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountRolesResponseTypeDef,
 )
 
 
 def get_structure() -> AccountInfoTypeDef:
     return {...}
 ```
@@ -316,42 +348,42 @@
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

### Comparing `mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/__init__.py` & `mypy-boto3-sso-1.27.0/mypy_boto3_sso/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/__init__.pyi` & `mypy-boto3-sso-1.27.0/mypy_boto3_sso/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/__main__.py` & `mypy-boto3-sso-1.27.0/mypy_boto3_sso/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSO 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.SSO 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO\nOther"
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

### Comparing `mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/client.py` & `mypy-boto3-sso-1.27.0/mypy_boto3_sso/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/client.pyi` & `mypy-boto3-sso-1.27.0/mypy_boto3_sso/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/literals.py` & `mypy-boto3-sso-1.27.0/mypy_boto3_sso/literals.py`

 * *Files 3% similar despite different names*

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
@@ -363,27 +395,30 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_account_roles", "list_accounts"]
 RegionName = Literal[
+    "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
+    "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/literals.pyi` & `mypy-boto3-sso-1.27.0/mypy_boto3_sso/literals.pyi`

 * *Files 2% similar despite different names*

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
@@ -361,27 +393,30 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_account_roles", "list_accounts"]
 RegionName = Literal[
+    "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
+    "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/paginator.py` & `mypy-boto3-sso-1.27.0/mypy_boto3_sso/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -29,46 +29,42 @@
     ListAccountRolesResponseTypeDef,
     ListAccountsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListAccountRolesPaginator", "ListAccountsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListAccountRolesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccountRoles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountrolespaginator)
     """
 
     def paginate(
-        self, *, accessToken: str, accountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, accessToken: str, accountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountRolesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccountRoles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountrolespaginator)
         """
 
-
 class ListAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountspaginator)
     """
 
     def paginate(
-        self, *, accessToken: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, accessToken: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountspaginator)
         """
```

### Comparing `mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/paginator.pyi` & `mypy-boto3-sso-1.27.0/mypy_boto3_sso/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,42 +29,46 @@
     ListAccountRolesResponseTypeDef,
     ListAccountsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListAccountRolesPaginator", "ListAccountsPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListAccountRolesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccountRoles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountrolespaginator)
     """
 
     def paginate(
-        self, *, accessToken: str, accountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, accessToken: str, accountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountRolesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccountRoles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountrolespaginator)
         """
 
+
 class ListAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountspaginator)
     """
 
     def paginate(
-        self, *, accessToken: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, accessToken: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/paginators/#listaccountspaginator)
         """
```

### Comparing `mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/type_defs.py` & `mypy-boto3-sso-1.27.0/mypy_boto3_sso/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -15,51 +15,46 @@
 from typing import Dict, List
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountInfoTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetRoleCredentialsRequestRequestTypeDef",
     "RoleCredentialsTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccountRolesRequestListAccountRolesPaginateTypeDef",
     "ListAccountRolesRequestRequestTypeDef",
     "RoleInfoTypeDef",
+    "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "LogoutRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "ListAccountsResponseTypeDef",
     "GetRoleCredentialsResponseTypeDef",
-    "ListAccountRolesRequestListAccountRolesPaginateTypeDef",
-    "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountRolesResponseTypeDef",
 )
 
 AccountInfoTypeDef = TypedDict(
     "AccountInfoTypeDef",
     {
         "accountId": str,
         "accountName": str,
         "emailAddress": str,
     },
     total=False,
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
 
 GetRoleCredentialsRequestRequestTypeDef = TypedDict(
     "GetRoleCredentialsRequestRequestTypeDef",
     {
         "roleName": str,
@@ -75,24 +70,35 @@
         "secretAccessKey": str,
         "sessionToken": str,
         "expiration": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
+    "_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "accessToken": str,
+        "accountId": str,
+    },
+)
+_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
+    "_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListAccountRolesRequestListAccountRolesPaginateTypeDef(
+    _RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    _OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef,
+):
+    pass
+
 _RequiredListAccountRolesRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountRolesRequestRequestTypeDef",
     {
         "accessToken": str,
         "accountId": str,
     },
 )
@@ -101,30 +107,48 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAccountRolesRequestRequestTypeDef(
     _RequiredListAccountRolesRequestRequestTypeDef, _OptionalListAccountRolesRequestRequestTypeDef
 ):
     pass
 
-
 RoleInfoTypeDef = TypedDict(
     "RoleInfoTypeDef",
     {
         "roleName": str,
         "accountId": str,
     },
     total=False,
 )
 
+_RequiredListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "_RequiredListAccountsRequestListAccountsPaginateTypeDef",
+    {
+        "accessToken": str,
+    },
+)
+_OptionalListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "_OptionalListAccountsRequestListAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListAccountsRequestListAccountsPaginateTypeDef(
+    _RequiredListAccountsRequestListAccountsPaginateTypeDef,
+    _OptionalListAccountsRequestListAccountsPaginateTypeDef,
+):
+    pass
+
 _RequiredListAccountsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountsRequestRequestTypeDef",
     {
         "accessToken": str,
     },
 )
 _OptionalListAccountsRequestRequestTypeDef = TypedDict(
@@ -132,98 +156,65 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAccountsRequestRequestTypeDef(
     _RequiredListAccountsRequestRequestTypeDef, _OptionalListAccountsRequestRequestTypeDef
 ):
     pass
 
-
 LogoutRequestRequestTypeDef = TypedDict(
     "LogoutRequestRequestTypeDef",
     {
         "accessToken": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
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
     },
 )
 
 ListAccountsResponseTypeDef = TypedDict(
     "ListAccountsResponseTypeDef",
     {
         "nextToken": str,
         "accountList": List[AccountInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRoleCredentialsResponseTypeDef = TypedDict(
     "GetRoleCredentialsResponseTypeDef",
     {
         "roleCredentials": RoleCredentialsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
-    "_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef",
-    {
-        "accessToken": str,
-        "accountId": str,
-    },
-)
-_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
-    "_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ListAccountRolesRequestListAccountRolesPaginateTypeDef(
-    _RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef,
-    _OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "_RequiredListAccountsRequestListAccountsPaginateTypeDef",
-    {
-        "accessToken": str,
-    },
-)
-_OptionalListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "_OptionalListAccountsRequestListAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAccountsRequestListAccountsPaginateTypeDef(
-    _RequiredListAccountsRequestListAccountsPaginateTypeDef,
-    _OptionalListAccountsRequestListAccountsPaginateTypeDef,
-):
-    pass
-
-
 ListAccountRolesResponseTypeDef = TypedDict(
     "ListAccountRolesResponseTypeDef",
     {
         "nextToken": str,
         "roleList": List[RoleInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso/type_defs.pyi` & `mypy-boto3-sso-1.27.0/mypy_boto3_sso/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,50 +15,47 @@
 from typing import Dict, List
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountInfoTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetRoleCredentialsRequestRequestTypeDef",
     "RoleCredentialsTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccountRolesRequestListAccountRolesPaginateTypeDef",
     "ListAccountRolesRequestRequestTypeDef",
     "RoleInfoTypeDef",
+    "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "LogoutRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "ListAccountsResponseTypeDef",
     "GetRoleCredentialsResponseTypeDef",
-    "ListAccountRolesRequestListAccountRolesPaginateTypeDef",
-    "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountRolesResponseTypeDef",
 )
 
 AccountInfoTypeDef = TypedDict(
     "AccountInfoTypeDef",
     {
         "accountId": str,
         "accountName": str,
         "emailAddress": str,
     },
     total=False,
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
 
 GetRoleCredentialsRequestRequestTypeDef = TypedDict(
     "GetRoleCredentialsRequestRequestTypeDef",
     {
         "roleName": str,
@@ -74,24 +71,37 @@
         "secretAccessKey": str,
         "sessionToken": str,
         "expiration": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
+    "_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "accessToken": str,
+        "accountId": str,
+    },
+)
+_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
+    "_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListAccountRolesRequestListAccountRolesPaginateTypeDef(
+    _RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    _OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAccountRolesRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountRolesRequestRequestTypeDef",
     {
         "accessToken": str,
         "accountId": str,
     },
 )
@@ -100,28 +110,52 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAccountRolesRequestRequestTypeDef(
     _RequiredListAccountRolesRequestRequestTypeDef, _OptionalListAccountRolesRequestRequestTypeDef
 ):
     pass
 
+
 RoleInfoTypeDef = TypedDict(
     "RoleInfoTypeDef",
     {
         "roleName": str,
         "accountId": str,
     },
     total=False,
 )
 
+_RequiredListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "_RequiredListAccountsRequestListAccountsPaginateTypeDef",
+    {
+        "accessToken": str,
+    },
+)
+_OptionalListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "_OptionalListAccountsRequestListAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListAccountsRequestListAccountsPaginateTypeDef(
+    _RequiredListAccountsRequestListAccountsPaginateTypeDef,
+    _OptionalListAccountsRequestListAccountsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAccountsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountsRequestRequestTypeDef",
     {
         "accessToken": str,
     },
 )
 _OptionalListAccountsRequestRequestTypeDef = TypedDict(
@@ -129,92 +163,67 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAccountsRequestRequestTypeDef(
     _RequiredListAccountsRequestRequestTypeDef, _OptionalListAccountsRequestRequestTypeDef
 ):
     pass
 
+
 LogoutRequestRequestTypeDef = TypedDict(
     "LogoutRequestRequestTypeDef",
     {
         "accessToken": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
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
     },
 )
 
 ListAccountsResponseTypeDef = TypedDict(
     "ListAccountsResponseTypeDef",
     {
         "nextToken": str,
         "accountList": List[AccountInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRoleCredentialsResponseTypeDef = TypedDict(
     "GetRoleCredentialsResponseTypeDef",
     {
         "roleCredentials": RoleCredentialsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
-    "_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef",
-    {
-        "accessToken": str,
-        "accountId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
-    "_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAccountRolesRequestListAccountRolesPaginateTypeDef(
-    _RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef,
-    _OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef,
-):
-    pass
-
-_RequiredListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "_RequiredListAccountsRequestListAccountsPaginateTypeDef",
-    {
-        "accessToken": str,
-    },
-)
-_OptionalListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "_OptionalListAccountsRequestListAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAccountsRequestListAccountsPaginateTypeDef(
-    _RequiredListAccountsRequestListAccountsPaginateTypeDef,
-    _OptionalListAccountsRequestListAccountsPaginateTypeDef,
-):
-    pass
 
 ListAccountRolesResponseTypeDef = TypedDict(
     "ListAccountRolesResponseTypeDef",
     {
         "nextToken": str,
         "roleList": List[RoleInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso.egg-info/PKG-INFO` & `mypy-boto3-sso-1.27.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-sso
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.SSO 1.26.0 service generated with mypy-boto3-builder 7.11.10
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sso type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-sso"></a>
 
 # mypy-boto3-sso
 
 [![PyPI - mypy-boto3-sso](https://img.shields.io/pypi/v/mypy-boto3-sso.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso?color=blue)](https://pypistats.org/packages/mypy-boto3-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSO 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
+[boto3.SSO 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
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
 [mypy-boto3-sso docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/).
 
 See how it helps to find and fix potential bugs:
 
@@ -319,27 +288,27 @@
 
 `mypy_boto3_sso.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sso.type_defs import (
     AccountInfoTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetRoleCredentialsRequestRequestTypeDef,
     RoleCredentialsTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
     ListAccountRolesRequestRequestTypeDef,
     RoleInfoTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountsRequestRequestTypeDef,
     LogoutRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     ListAccountsResponseTypeDef,
     GetRoleCredentialsResponseTypeDef,
-    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountRolesResponseTypeDef,
 )
 
 
 def get_structure() -> AccountInfoTypeDef:
     return {...}
 ```
@@ -347,42 +316,42 @@
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

### Comparing `mypy-boto3-sso-1.26.0.post1/mypy_boto3_sso.egg-info/SOURCES.txt` & `mypy-boto3-sso-1.27.0/mypy_boto3_sso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-1.26.0.post1/setup.py` & `mypy-boto3-sso-1.27.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-sso.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sso",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_sso"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSO 1.26.0 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.SSO 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 sso type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_sso": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_sso": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso/",
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


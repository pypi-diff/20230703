# Comparing `tmp/mypy-boto3-account-1.26.85.tar.gz` & `tmp/mypy-boto3-account-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-account-1.26.85.tar", last modified: Mon Mar  6 20:27:45 2023, max compression
+gzip compressed data, was "mypy-boto3-account-1.27.0.tar", last modified: Mon Jul  3 19:50:17 2023, max compression
```

## Comparing `mypy-boto3-account-1.26.85.tar` & `mypy-boto3-account-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:45.496845 mypy-boto3-account-1.26.85/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-03-06 20:27:45.496845 mypy-boto3-account-1.26.85/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:45.496845 mypy-boto3-account-1.26.85/mypy_boto3_account/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-03-06 20:27:34.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/mypy_boto3_account/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 20:27:45.496845 mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-03-06 20:27:45.000000 mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-06 20:27:45.000000 mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 20:27:45.000000 mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 20:27:45.000000 mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-06 20:27:45.000000 mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-06 20:27:45.000000 mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 20:27:45.496845 mypy-boto3-account-1.26.85/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-06 20:27:33.000000 mypy-boto3-account-1.26.85/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:17.750733 mypy-boto3-account-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:31:56.000000 mypy-boto3-account-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-03 19:50:17.750733 mypy-boto3-account-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-07-03 19:31:56.000000 mypy-boto3-account-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:17.742733 mypy-boto3-account-1.27.0/mypy_boto3_account/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-03 19:31:56.000000 mypy-boto3-account-1.27.0/mypy_boto3_account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-03 19:31:56.000000 mypy-boto3-account-1.27.0/mypy_boto3_account/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:31:56.000000 mypy-boto3-account-1.27.0/mypy_boto3_account/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-03 19:31:56.000000 mypy-boto3-account-1.27.0/mypy_boto3_account/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-07-03 19:31:56.000000 mypy-boto3-account-1.27.0/mypy_boto3_account/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-07-03 19:31:57.000000 mypy-boto3-account-1.27.0/mypy_boto3_account/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-03 19:31:57.000000 mypy-boto3-account-1.27.0/mypy_boto3_account/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-03 19:31:56.000000 mypy-boto3-account-1.27.0/mypy_boto3_account/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-03 19:31:56.000000 mypy-boto3-account-1.27.0/mypy_boto3_account/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:31:56.000000 mypy-boto3-account-1.27.0/mypy_boto3_account/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-03 19:31:57.000000 mypy-boto3-account-1.27.0/mypy_boto3_account/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-07-03 19:31:57.000000 mypy-boto3-account-1.27.0/mypy_boto3_account/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:31:56.000000 mypy-boto3-account-1.27.0/mypy_boto3_account/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:17.750733 mypy-boto3-account-1.27.0/mypy_boto3_account.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-03 19:50:17.000000 mypy-boto3-account-1.27.0/mypy_boto3_account.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-03 19:50:17.000000 mypy-boto3-account-1.27.0/mypy_boto3_account.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:17.000000 mypy-boto3-account-1.27.0/mypy_boto3_account.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:17.000000 mypy-boto3-account-1.27.0/mypy_boto3_account.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:17.000000 mypy-boto3-account-1.27.0/mypy_boto3_account.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:50:17.000000 mypy-boto3-account-1.27.0/mypy_boto3_account.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:17.750733 mypy-boto3-account-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:31:56.000000 mypy-boto3-account-1.27.0/setup.py
```

### Comparing `mypy-boto3-account-1.26.85/LICENSE` & `mypy-boto3-account-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-account-1.26.85/PKG-INFO` & `mypy-boto3-account-1.27.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-account
-Version: 1.26.85
-Summary: Type annotations for boto3.Account 1.26.85 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.Account 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-account"></a>
 
 # mypy-boto3-account
 
 [![PyPI - mypy-boto3-account](https://img.shields.io/pypi/v/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-account?color=blue)](https://pypistats.org/packages/mypy-boto3-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Account 1.26.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
+[boto3.Account 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-account docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/).
 
 See how it helps to find and fix potential bugs:
 
@@ -72,14 +72,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -266,28 +267,50 @@
 from mypy_boto3_account import AccountClient
 
 client: AccountClient = Session().client("account")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_account.paginator` module contains type annotations for all
+paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_account import AccountClient
+from mypy_boto3_account.paginator import ListRegionsPaginator
+
+client: AccountClient = Session().client("account")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+list_regions_paginator: ListRegionsPaginator = client.get_paginator("list_regions")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_account.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_account.literals import (
     AlternateContactTypeType,
+    ListRegionsPaginatorName,
     RegionOptStatusType,
     AccountServiceName,
     ServiceName,
     ResourceServiceName,
+    PaginatorName,
 )
 
 
 def check_value(value: AlternateContactTypeType) -> bool:
     ...
 ```
 
@@ -305,22 +328,24 @@
     DeleteAlternateContactRequestRequestTypeDef,
     DisableRegionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EnableRegionRequestRequestTypeDef,
     GetAlternateContactRequestRequestTypeDef,
     GetContactInformationRequestRequestTypeDef,
     GetRegionOptStatusRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ListRegionsRequestRequestTypeDef,
     RegionTypeDef,
     PutAlternateContactRequestRequestTypeDef,
     PutContactInformationRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAlternateContactResponseTypeDef,
     GetContactInformationResponseTypeDef,
     GetRegionOptStatusResponseTypeDef,
+    ListRegionsRequestListRegionsPaginateTypeDef,
     ListRegionsResponseTypeDef,
 )
 
 
 def get_structure() -> AlternateContactTypeDef:
     return {...}
 ```
@@ -328,42 +353,42 @@
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

### Comparing `mypy-boto3-account-1.26.85/README.md` & `mypy-boto3-account-1.27.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-account"></a>
 
 # mypy-boto3-account
 
 [![PyPI - mypy-boto3-account](https://img.shields.io/pypi/v/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-account?color=blue)](https://pypistats.org/packages/mypy-boto3-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Account 1.26.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
+[boto3.Account 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-account docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/).
 
 See how it helps to find and fix potential bugs:
 
@@ -40,14 +40,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -234,28 +235,50 @@
 from mypy_boto3_account import AccountClient
 
 client: AccountClient = Session().client("account")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_account.paginator` module contains type annotations for all
+paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_account import AccountClient
+from mypy_boto3_account.paginator import ListRegionsPaginator
+
+client: AccountClient = Session().client("account")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+list_regions_paginator: ListRegionsPaginator = client.get_paginator("list_regions")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_account.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_account.literals import (
     AlternateContactTypeType,
+    ListRegionsPaginatorName,
     RegionOptStatusType,
     AccountServiceName,
     ServiceName,
     ResourceServiceName,
+    PaginatorName,
 )
 
 
 def check_value(value: AlternateContactTypeType) -> bool:
     ...
 ```
 
@@ -273,22 +296,24 @@
     DeleteAlternateContactRequestRequestTypeDef,
     DisableRegionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EnableRegionRequestRequestTypeDef,
     GetAlternateContactRequestRequestTypeDef,
     GetContactInformationRequestRequestTypeDef,
     GetRegionOptStatusRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ListRegionsRequestRequestTypeDef,
     RegionTypeDef,
     PutAlternateContactRequestRequestTypeDef,
     PutContactInformationRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAlternateContactResponseTypeDef,
     GetContactInformationResponseTypeDef,
     GetRegionOptStatusResponseTypeDef,
+    ListRegionsRequestListRegionsPaginateTypeDef,
     ListRegionsResponseTypeDef,
 )
 
 
 def get_structure() -> AlternateContactTypeDef:
     return {...}
 ```
@@ -296,42 +321,42 @@
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

### Comparing `mypy-boto3-account-1.26.85/mypy_boto3_account/__main__.py` & `mypy-boto3-account-1.27.0/mypy_boto3_account/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Account 1.26.85\nVersion:         1.26.85\nBuilder version:"
-        " 7.12.5\nDocs:           "
+        "Type annotations for boto3.Account 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.85")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-account-1.26.85/mypy_boto3_account/client.py` & `mypy-boto3-account-1.27.0/mypy_boto3_account/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,36 @@
     from boto3.session import Session
     from mypy_boto3_account.client import AccountClient
 
     session = Session()
     client: AccountClient = session.client("account")
     ```
 """
+import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AlternateContactTypeType, RegionOptStatusType
+from .paginator import ListRegionsPaginator
 from .type_defs import (
     ContactInformationTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAlternateContactResponseTypeDef,
     GetContactInformationResponseTypeDef,
     GetRegionOptStatusResponseTypeDef,
     ListRegionsResponseTypeDef,
 )
 
+if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
+
 __all__ = ("AccountClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -194,7 +202,13 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the primary contact information of an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.put_contact_information)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/client/#put_contact_information)
         """
+
+    def get_paginator(self, operation_name: Literal["list_regions"]) -> ListRegionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-account-1.26.85/mypy_boto3_account/client.pyi` & `mypy-boto3-account-1.27.0/mypy_boto3_account/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,35 @@
     from boto3.session import Session
     from mypy_boto3_account.client import AccountClient
 
     session = Session()
     client: AccountClient = session.client("account")
     ```
 """
+import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AlternateContactTypeType, RegionOptStatusType
+from .paginator import ListRegionsPaginator
 from .type_defs import (
     ContactInformationTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAlternateContactResponseTypeDef,
     GetContactInformationResponseTypeDef,
     GetRegionOptStatusResponseTypeDef,
     ListRegionsResponseTypeDef,
 )
 
+if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 __all__ = ("AccountClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
@@ -179,7 +186,12 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the primary contact information of an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.put_contact_information)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/client/#put_contact_information)
         """
+    def get_paginator(self, operation_name: Literal["list_regions"]) -> ListRegionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-account-1.26.85/mypy_boto3_account/literals.py` & `mypy-boto3-account-1.27.0/mypy_boto3_account/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,25 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AlternateContactTypeType",
+    "ListRegionsPaginatorName",
     "RegionOptStatusType",
     "AccountServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "PaginatorName",
 )
 
 
 AlternateContactTypeType = Literal["BILLING", "OPERATIONS", "SECURITY"]
+ListRegionsPaginatorName = Literal["list_regions"]
 RegionOptStatusType = Literal["DISABLED", "DISABLING", "ENABLED", "ENABLED_BY_DEFAULT", "ENABLING"]
 AccountServiceName = Literal["account"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -42,14 +45,15 @@
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
@@ -89,14 +93,15 @@
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
@@ -194,14 +199,15 @@
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
@@ -237,14 +243,15 @@
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
@@ -263,16 +270,19 @@
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
@@ -356,15 +366,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
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
@@ -382,7 +394,8 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+PaginatorName = Literal["list_regions"]
```

### Comparing `mypy-boto3-account-1.26.85/mypy_boto3_account/literals.pyi` & `mypy-boto3-account-1.27.0/mypy_boto3_account/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,24 @@
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AlternateContactTypeType",
+    "ListRegionsPaginatorName",
     "RegionOptStatusType",
     "AccountServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "PaginatorName",
 )
 
 AlternateContactTypeType = Literal["BILLING", "OPERATIONS", "SECURITY"]
+ListRegionsPaginatorName = Literal["list_regions"]
 RegionOptStatusType = Literal["DISABLED", "DISABLING", "ENABLED", "ENABLED_BY_DEFAULT", "ENABLING"]
 AccountServiceName = Literal["account"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -40,14 +43,15 @@
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
@@ -87,14 +91,15 @@
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
@@ -192,14 +197,15 @@
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
@@ -235,14 +241,15 @@
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
@@ -261,16 +268,19 @@
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
@@ -354,15 +364,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
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
@@ -380,7 +392,8 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+PaginatorName = Literal["list_regions"]
```

### Comparing `mypy-boto3-account-1.26.85/mypy_boto3_account/type_defs.py` & `mypy-boto3-account-1.27.0/mypy_boto3_account/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -17,33 +17,34 @@
 from .literals import AlternateContactTypeType, RegionOptStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AlternateContactTypeDef",
     "ContactInformationTypeDef",
     "DeleteAlternateContactRequestRequestTypeDef",
     "DisableRegionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EnableRegionRequestRequestTypeDef",
     "GetAlternateContactRequestRequestTypeDef",
     "GetContactInformationRequestRequestTypeDef",
     "GetRegionOptStatusRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRegionsRequestRequestTypeDef",
     "RegionTypeDef",
     "PutAlternateContactRequestRequestTypeDef",
     "PutContactInformationRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAlternateContactResponseTypeDef",
     "GetContactInformationResponseTypeDef",
     "GetRegionOptStatusResponseTypeDef",
+    "ListRegionsRequestListRegionsPaginateTypeDef",
     "ListRegionsResponseTypeDef",
 )
 
 AlternateContactTypeDef = TypedDict(
     "AlternateContactTypeDef",
     {
         "AlternateContactType": AlternateContactTypeType,
@@ -75,64 +76,58 @@
         "DistrictOrCounty": str,
         "StateOrRegion": str,
         "WebsiteUrl": str,
     },
     total=False,
 )
 
-
 class ContactInformationTypeDef(
     _RequiredContactInformationTypeDef, _OptionalContactInformationTypeDef
 ):
     pass
 
-
 _RequiredDeleteAlternateContactRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAlternateContactRequestRequestTypeDef",
     {
         "AlternateContactType": AlternateContactTypeType,
     },
 )
 _OptionalDeleteAlternateContactRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAlternateContactRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class DeleteAlternateContactRequestRequestTypeDef(
     _RequiredDeleteAlternateContactRequestRequestTypeDef,
     _OptionalDeleteAlternateContactRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDisableRegionRequestRequestTypeDef = TypedDict(
     "_RequiredDisableRegionRequestRequestTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalDisableRegionRequestRequestTypeDef = TypedDict(
     "_OptionalDisableRegionRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class DisableRegionRequestRequestTypeDef(
     _RequiredDisableRegionRequestRequestTypeDef, _OptionalDisableRegionRequestRequestTypeDef
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -150,43 +145,39 @@
     "_OptionalEnableRegionRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class EnableRegionRequestRequestTypeDef(
     _RequiredEnableRegionRequestRequestTypeDef, _OptionalEnableRegionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetAlternateContactRequestRequestTypeDef = TypedDict(
     "_RequiredGetAlternateContactRequestRequestTypeDef",
     {
         "AlternateContactType": AlternateContactTypeType,
     },
 )
 _OptionalGetAlternateContactRequestRequestTypeDef = TypedDict(
     "_OptionalGetAlternateContactRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class GetAlternateContactRequestRequestTypeDef(
     _RequiredGetAlternateContactRequestRequestTypeDef,
     _OptionalGetAlternateContactRequestRequestTypeDef,
 ):
     pass
 
-
 GetContactInformationRequestRequestTypeDef = TypedDict(
     "GetContactInformationRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
@@ -201,21 +192,29 @@
     "_OptionalGetRegionOptStatusRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class GetRegionOptStatusRequestRequestTypeDef(
     _RequiredGetRegionOptStatusRequestRequestTypeDef,
     _OptionalGetRegionOptStatusRequestRequestTypeDef,
 ):
     pass
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
 
 ListRegionsRequestRequestTypeDef = TypedDict(
     "ListRegionsRequestRequestTypeDef",
     {
         "AccountId": str,
         "MaxResults": int,
         "NextToken": str,
@@ -247,44 +246,40 @@
     "_OptionalPutAlternateContactRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class PutAlternateContactRequestRequestTypeDef(
     _RequiredPutAlternateContactRequestRequestTypeDef,
     _OptionalPutAlternateContactRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutContactInformationRequestRequestTypeDef = TypedDict(
     "_RequiredPutContactInformationRequestRequestTypeDef",
     {
         "ContactInformation": ContactInformationTypeDef,
     },
 )
 _OptionalPutContactInformationRequestRequestTypeDef = TypedDict(
     "_OptionalPutContactInformationRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class PutContactInformationRequestRequestTypeDef(
     _RequiredPutContactInformationRequestRequestTypeDef,
     _OptionalPutContactInformationRequestRequestTypeDef,
 ):
     pass
 
-
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -309,14 +304,24 @@
     {
         "RegionName": str,
         "RegionOptStatus": RegionOptStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListRegionsRequestListRegionsPaginateTypeDef = TypedDict(
+    "ListRegionsRequestListRegionsPaginateTypeDef",
+    {
+        "AccountId": str,
+        "RegionOptStatusContains": Sequence[RegionOptStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListRegionsResponseTypeDef = TypedDict(
     "ListRegionsResponseTypeDef",
     {
         "NextToken": str,
         "Regions": List[RegionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-account-1.26.85/mypy_boto3_account/type_defs.pyi` & `mypy-boto3-account-1.27.0/mypy_boto3_account/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,32 +17,35 @@
 from .literals import AlternateContactTypeType, RegionOptStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AlternateContactTypeDef",
     "ContactInformationTypeDef",
     "DeleteAlternateContactRequestRequestTypeDef",
     "DisableRegionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EnableRegionRequestRequestTypeDef",
     "GetAlternateContactRequestRequestTypeDef",
     "GetContactInformationRequestRequestTypeDef",
     "GetRegionOptStatusRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRegionsRequestRequestTypeDef",
     "RegionTypeDef",
     "PutAlternateContactRequestRequestTypeDef",
     "PutContactInformationRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAlternateContactResponseTypeDef",
     "GetContactInformationResponseTypeDef",
     "GetRegionOptStatusResponseTypeDef",
+    "ListRegionsRequestListRegionsPaginateTypeDef",
     "ListRegionsResponseTypeDef",
 )
 
 AlternateContactTypeDef = TypedDict(
     "AlternateContactTypeDef",
     {
         "AlternateContactType": AlternateContactTypeType,
@@ -74,58 +77,64 @@
         "DistrictOrCounty": str,
         "StateOrRegion": str,
         "WebsiteUrl": str,
     },
     total=False,
 )
 
+
 class ContactInformationTypeDef(
     _RequiredContactInformationTypeDef, _OptionalContactInformationTypeDef
 ):
     pass
 
+
 _RequiredDeleteAlternateContactRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAlternateContactRequestRequestTypeDef",
     {
         "AlternateContactType": AlternateContactTypeType,
     },
 )
 _OptionalDeleteAlternateContactRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAlternateContactRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class DeleteAlternateContactRequestRequestTypeDef(
     _RequiredDeleteAlternateContactRequestRequestTypeDef,
     _OptionalDeleteAlternateContactRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDisableRegionRequestRequestTypeDef = TypedDict(
     "_RequiredDisableRegionRequestRequestTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalDisableRegionRequestRequestTypeDef = TypedDict(
     "_OptionalDisableRegionRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class DisableRegionRequestRequestTypeDef(
     _RequiredDisableRegionRequestRequestTypeDef, _OptionalDisableRegionRequestRequestTypeDef
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -143,39 +152,43 @@
     "_OptionalEnableRegionRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class EnableRegionRequestRequestTypeDef(
     _RequiredEnableRegionRequestRequestTypeDef, _OptionalEnableRegionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetAlternateContactRequestRequestTypeDef = TypedDict(
     "_RequiredGetAlternateContactRequestRequestTypeDef",
     {
         "AlternateContactType": AlternateContactTypeType,
     },
 )
 _OptionalGetAlternateContactRequestRequestTypeDef = TypedDict(
     "_OptionalGetAlternateContactRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class GetAlternateContactRequestRequestTypeDef(
     _RequiredGetAlternateContactRequestRequestTypeDef,
     _OptionalGetAlternateContactRequestRequestTypeDef,
 ):
     pass
 
+
 GetContactInformationRequestRequestTypeDef = TypedDict(
     "GetContactInformationRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
@@ -190,20 +203,32 @@
     "_OptionalGetRegionOptStatusRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class GetRegionOptStatusRequestRequestTypeDef(
     _RequiredGetRegionOptStatusRequestRequestTypeDef,
     _OptionalGetRegionOptStatusRequestRequestTypeDef,
 ):
     pass
 
+
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
 ListRegionsRequestRequestTypeDef = TypedDict(
     "ListRegionsRequestRequestTypeDef",
     {
         "AccountId": str,
         "MaxResults": int,
         "NextToken": str,
         "RegionOptStatusContains": Sequence[RegionOptStatusType],
@@ -234,40 +259,44 @@
     "_OptionalPutAlternateContactRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class PutAlternateContactRequestRequestTypeDef(
     _RequiredPutAlternateContactRequestRequestTypeDef,
     _OptionalPutAlternateContactRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutContactInformationRequestRequestTypeDef = TypedDict(
     "_RequiredPutContactInformationRequestRequestTypeDef",
     {
         "ContactInformation": ContactInformationTypeDef,
     },
 )
 _OptionalPutContactInformationRequestRequestTypeDef = TypedDict(
     "_OptionalPutContactInformationRequestRequestTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class PutContactInformationRequestRequestTypeDef(
     _RequiredPutContactInformationRequestRequestTypeDef,
     _OptionalPutContactInformationRequestRequestTypeDef,
 ):
     pass
 
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -292,14 +321,24 @@
     {
         "RegionName": str,
         "RegionOptStatus": RegionOptStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListRegionsRequestListRegionsPaginateTypeDef = TypedDict(
+    "ListRegionsRequestListRegionsPaginateTypeDef",
+    {
+        "AccountId": str,
+        "RegionOptStatusContains": Sequence[RegionOptStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListRegionsResponseTypeDef = TypedDict(
     "ListRegionsResponseTypeDef",
     {
         "NextToken": str,
         "Regions": List[RegionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/PKG-INFO` & `mypy-boto3-account-1.27.0/mypy_boto3_account.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-account
-Version: 1.26.85
-Summary: Type annotations for boto3.Account 1.26.85 service generated with mypy-boto3-builder 7.12.5
+Version: 1.27.0
+Summary: Type annotations for boto3.Account 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-account"></a>
 
 # mypy-boto3-account
 
 [![PyPI - mypy-boto3-account](https://img.shields.io/pypi/v/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-account?color=blue)](https://pypistats.org/packages/mypy-boto3-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Account 1.26.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
+[boto3.Account 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-account docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/).
 
 See how it helps to find and fix potential bugs:
 
@@ -72,14 +72,15 @@
     - [Emacs](#emacs)
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
+    - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
     - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
@@ -266,28 +267,50 @@
 from mypy_boto3_account import AccountClient
 
 client: AccountClient = Session().client("account")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_account.paginator` module contains type annotations for all
+paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_account import AccountClient
+from mypy_boto3_account.paginator import ListRegionsPaginator
+
+client: AccountClient = Session().client("account")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+list_regions_paginator: ListRegionsPaginator = client.get_paginator("list_regions")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_account.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_account.literals import (
     AlternateContactTypeType,
+    ListRegionsPaginatorName,
     RegionOptStatusType,
     AccountServiceName,
     ServiceName,
     ResourceServiceName,
+    PaginatorName,
 )
 
 
 def check_value(value: AlternateContactTypeType) -> bool:
     ...
 ```
 
@@ -305,22 +328,24 @@
     DeleteAlternateContactRequestRequestTypeDef,
     DisableRegionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EnableRegionRequestRequestTypeDef,
     GetAlternateContactRequestRequestTypeDef,
     GetContactInformationRequestRequestTypeDef,
     GetRegionOptStatusRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ListRegionsRequestRequestTypeDef,
     RegionTypeDef,
     PutAlternateContactRequestRequestTypeDef,
     PutContactInformationRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAlternateContactResponseTypeDef,
     GetContactInformationResponseTypeDef,
     GetRegionOptStatusResponseTypeDef,
+    ListRegionsRequestListRegionsPaginateTypeDef,
     ListRegionsResponseTypeDef,
 )
 
 
 def get_structure() -> AlternateContactTypeDef:
     return {...}
 ```
@@ -328,42 +353,42 @@
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

### Comparing `mypy-boto3-account-1.26.85/mypy_boto3_account.egg-info/SOURCES.txt` & `mypy-boto3-account-1.27.0/mypy_boto3_account.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 mypy_boto3_account/__init__.py
 mypy_boto3_account/__init__.pyi
 mypy_boto3_account/__main__.py
 mypy_boto3_account/client.py
 mypy_boto3_account/client.pyi
 mypy_boto3_account/literals.py
 mypy_boto3_account/literals.pyi
+mypy_boto3_account/paginator.py
+mypy_boto3_account/paginator.pyi
 mypy_boto3_account/py.typed
 mypy_boto3_account/type_defs.py
 mypy_boto3_account/type_defs.pyi
 mypy_boto3_account/version.py
 mypy_boto3_account.egg-info/PKG-INFO
 mypy_boto3_account.egg-info/SOURCES.txt
 mypy_boto3_account.egg-info/dependency_links.txt
```

### Comparing `mypy-boto3-account-1.26.85/setup.py` & `mypy-boto3-account-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 Setup script for mypy-boto3-account.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-account",
-    version="1.26.85",
+    version="1.27.0",
     packages=["mypy_boto3_account"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Account 1.26.85 service generated with mypy-boto3-builder"
-        " 7.12.5"
+        "Type annotations for boto3.Account 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/",
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


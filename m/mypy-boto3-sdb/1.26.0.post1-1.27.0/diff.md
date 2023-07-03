# Comparing `tmp/mypy-boto3-sdb-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-sdb-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sdb-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:58 2022, max compression
+gzip compressed data, was "mypy-boto3-sdb-1.27.0.tar", last modified: Mon Jul  3 19:51:25 2023, max compression
```

## Comparing `mypy-boto3-sdb-1.26.0.post1.tar` & `mypy-boto3-sdb-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:58.880848 mypy-boto3-sdb-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13223 2022-11-01 21:43:58.876848 mypy-boto3-sdb-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11793 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:58.876848 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10495 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    10476 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7227 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7225 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     8632 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8613 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:58.876848 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13223 2022-11-01 21:43:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-11-01 21:43:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-01 21:43:58.000000 mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:58.880848 mypy-boto3-sdb-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-11-01 21:40:58.000000 mypy-boto3-sdb-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:25.783969 mypy-boto3-sdb-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-03 19:51:25.775969 mypy-boto3-sdb-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:25.775969 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-03 19:47:35.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-07-03 19:47:35.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-07-03 19:47:35.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-03 19:47:35.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:25.775969 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-03 19:51:25.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:51:25.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:25.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:25.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:25.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:25.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:25.783969 mypy-boto3-sdb-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/setup.py
```

### Comparing `mypy-boto3-sdb-1.26.0.post1/LICENSE` & `mypy-boto3-sdb-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-sdb-1.26.0.post1/PKG-INFO` & `mypy-boto3-sdb-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sdb
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.SimpleDB 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.SimpleDB 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/
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
 
 <a id="mypy-boto3-sdb"></a>
 
 # mypy-boto3-sdb
 
 [![PyPI - mypy-boto3-sdb](https://img.shields.io/pypi/v/mypy-boto3-sdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-sdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-sdb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sdb?color=blue)](https://pypistats.org/packages/mypy-boto3-sdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimpleDB 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
+[boto3.SimpleDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
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
 [mypy-boto3-sdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,29 +324,29 @@
 ```python
 from mypy_boto3_sdb.type_defs import (
     AttributeTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateConditionTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainMetadataRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DomainMetadataResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetAttributesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListDomainsResultTypeDef,
+    PaginatorConfigTypeDef,
     ReplaceableAttributeTypeDef,
+    ResponseMetadataTypeDef,
     SelectRequestRequestTypeDef,
+    SelectRequestSelectPaginateTypeDef,
     DeletableItemTypeDef,
+    GetAttributesResultTypeDef,
     ItemTypeDef,
     DeleteAttributesRequestRequestTypeDef,
-    DomainMetadataResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAttributesResultTypeDef,
-    ListDomainsResultTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    SelectRequestSelectPaginateTypeDef,
     PutAttributesRequestRequestTypeDef,
     ReplaceableItemTypeDef,
     BatchDeleteAttributesRequestRequestTypeDef,
     SelectResultTypeDef,
     BatchPutAttributesRequestRequestTypeDef,
 )
 
@@ -357,42 +358,42 @@
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

### Comparing `mypy-boto3-sdb-1.26.0.post1/README.md` & `mypy-boto3-sdb-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sdb"></a>
 
 # mypy-boto3-sdb
 
 [![PyPI - mypy-boto3-sdb](https://img.shields.io/pypi/v/mypy-boto3-sdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-sdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-sdb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sdb?color=blue)](https://pypistats.org/packages/mypy-boto3-sdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimpleDB 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
+[boto3.SimpleDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
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
 [mypy-boto3-sdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -292,29 +292,29 @@
 ```python
 from mypy_boto3_sdb.type_defs import (
     AttributeTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateConditionTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainMetadataRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DomainMetadataResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetAttributesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListDomainsResultTypeDef,
+    PaginatorConfigTypeDef,
     ReplaceableAttributeTypeDef,
+    ResponseMetadataTypeDef,
     SelectRequestRequestTypeDef,
+    SelectRequestSelectPaginateTypeDef,
     DeletableItemTypeDef,
+    GetAttributesResultTypeDef,
     ItemTypeDef,
     DeleteAttributesRequestRequestTypeDef,
-    DomainMetadataResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAttributesResultTypeDef,
-    ListDomainsResultTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    SelectRequestSelectPaginateTypeDef,
     PutAttributesRequestRequestTypeDef,
     ReplaceableItemTypeDef,
     BatchDeleteAttributesRequestRequestTypeDef,
     SelectResultTypeDef,
     BatchPutAttributesRequestRequestTypeDef,
 )
 
@@ -326,42 +326,42 @@
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

### Comparing `mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/__init__.py` & `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/__init__.pyi` & `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/client.py` & `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/client.pyi` & `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/literals.py` & `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/literals.py`

 * *Files 2% similar despite different names*

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
```

### Comparing `mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/literals.pyi` & `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/literals.pyi`

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
```

### Comparing `mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/paginator.py` & `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 class ListDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.ListDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/paginators/#listdomainspaginator)
         """
 
 
@@ -62,13 +62,13 @@
     """
 
     def paginate(
         self,
         *,
         SelectExpression: str,
         ConsistentRead: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SelectResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.Select.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/paginators/#selectpaginator)
         """
```

### Comparing `mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/paginator.pyi` & `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 class ListDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.ListDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/paginators/#listdomainspaginator)
         """
 
 class SelectPaginator(Paginator):
@@ -58,13 +58,13 @@
     """
 
     def paginate(
         self,
         *,
         SelectExpression: str,
         ConsistentRead: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SelectResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.Select.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/paginators/#selectpaginator)
         """
```

### Comparing `mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/type_defs.py` & `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,29 +22,29 @@
 
 __all__ = (
     "AttributeTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateConditionTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainMetadataRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DomainMetadataResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetAttributesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
+    "ListDomainsResultTypeDef",
+    "PaginatorConfigTypeDef",
     "ReplaceableAttributeTypeDef",
+    "ResponseMetadataTypeDef",
     "SelectRequestRequestTypeDef",
+    "SelectRequestSelectPaginateTypeDef",
     "DeletableItemTypeDef",
+    "GetAttributesResultTypeDef",
     "ItemTypeDef",
     "DeleteAttributesRequestRequestTypeDef",
-    "DomainMetadataResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAttributesResultTypeDef",
-    "ListDomainsResultTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    "SelectRequestSelectPaginateTypeDef",
     "PutAttributesRequestRequestTypeDef",
     "ReplaceableItemTypeDef",
     "BatchDeleteAttributesRequestRequestTypeDef",
     "SelectResultTypeDef",
     "BatchPutAttributesRequestRequestTypeDef",
 )
 
@@ -96,22 +96,32 @@
 DomainMetadataRequestRequestTypeDef = TypedDict(
     "DomainMetadataRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DomainMetadataResultTypeDef = TypedDict(
+    "DomainMetadataResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ItemCount": int,
+        "ItemNamesSizeBytes": int,
+        "AttributeNameCount": int,
+        "AttributeNamesSizeBytes": int,
+        "AttributeValueCount": int,
+        "AttributeValuesSizeBytes": int,
+        "Timestamp": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -130,33 +140,50 @@
 
 class GetAttributesRequestRequestTypeDef(
     _RequiredGetAttributesRequestRequestTypeDef, _OptionalGetAttributesRequestRequestTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "MaxNumberOfDomains": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListDomainsResultTypeDef = TypedDict(
+    "ListDomainsResultTypeDef",
+    {
+        "DomainNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
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
 _RequiredReplaceableAttributeTypeDef = TypedDict(
     "_RequiredReplaceableAttributeTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -171,14 +198,25 @@
 
 class ReplaceableAttributeTypeDef(
     _RequiredReplaceableAttributeTypeDef, _OptionalReplaceableAttributeTypeDef
 ):
     pass
 
 
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
 _RequiredSelectRequestRequestTypeDef = TypedDict(
     "_RequiredSelectRequestRequestTypeDef",
     {
         "SelectExpression": str,
     },
 )
 _OptionalSelectRequestRequestTypeDef = TypedDict(
@@ -193,14 +231,36 @@
 
 class SelectRequestRequestTypeDef(
     _RequiredSelectRequestRequestTypeDef, _OptionalSelectRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredSelectRequestSelectPaginateTypeDef = TypedDict(
+    "_RequiredSelectRequestSelectPaginateTypeDef",
+    {
+        "SelectExpression": str,
+    },
+)
+_OptionalSelectRequestSelectPaginateTypeDef = TypedDict(
+    "_OptionalSelectRequestSelectPaginateTypeDef",
+    {
+        "ConsistentRead": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class SelectRequestSelectPaginateTypeDef(
+    _RequiredSelectRequestSelectPaginateTypeDef, _OptionalSelectRequestSelectPaginateTypeDef
+):
+    pass
+
+
 _RequiredDeletableItemTypeDef = TypedDict(
     "_RequiredDeletableItemTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDeletableItemTypeDef = TypedDict(
@@ -212,14 +272,22 @@
 )
 
 
 class DeletableItemTypeDef(_RequiredDeletableItemTypeDef, _OptionalDeletableItemTypeDef):
     pass
 
 
+GetAttributesResultTypeDef = TypedDict(
+    "GetAttributesResultTypeDef",
+    {
+        "Attributes": List[AttributeTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredItemTypeDef = TypedDict(
     "_RequiredItemTypeDef",
     {
         "Name": str,
         "Attributes": List[AttributeTypeDef],
     },
 )
@@ -255,82 +323,14 @@
 
 class DeleteAttributesRequestRequestTypeDef(
     _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
 ):
     pass
 
 
-DomainMetadataResultTypeDef = TypedDict(
-    "DomainMetadataResultTypeDef",
-    {
-        "ItemCount": int,
-        "ItemNamesSizeBytes": int,
-        "AttributeNameCount": int,
-        "AttributeNamesSizeBytes": int,
-        "AttributeValueCount": int,
-        "AttributeValuesSizeBytes": int,
-        "Timestamp": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAttributesResultTypeDef = TypedDict(
-    "GetAttributesResultTypeDef",
-    {
-        "Attributes": List[AttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDomainsResultTypeDef = TypedDict(
-    "ListDomainsResultTypeDef",
-    {
-        "DomainNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredSelectRequestSelectPaginateTypeDef = TypedDict(
-    "_RequiredSelectRequestSelectPaginateTypeDef",
-    {
-        "SelectExpression": str,
-    },
-)
-_OptionalSelectRequestSelectPaginateTypeDef = TypedDict(
-    "_OptionalSelectRequestSelectPaginateTypeDef",
-    {
-        "ConsistentRead": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class SelectRequestSelectPaginateTypeDef(
-    _RequiredSelectRequestSelectPaginateTypeDef, _OptionalSelectRequestSelectPaginateTypeDef
-):
-    pass
-
-
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
         "ItemName": str,
         "Attributes": Sequence[ReplaceableAttributeTypeDef],
     },
@@ -367,15 +367,15 @@
 )
 
 SelectResultTypeDef = TypedDict(
     "SelectResultTypeDef",
     {
         "Items": List[ItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutAttributesRequestRequestTypeDef = TypedDict(
     "BatchPutAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
```

### Comparing `mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb/type_defs.pyi` & `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 
 __all__ = (
     "AttributeTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateConditionTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainMetadataRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DomainMetadataResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetAttributesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
+    "ListDomainsResultTypeDef",
+    "PaginatorConfigTypeDef",
     "ReplaceableAttributeTypeDef",
+    "ResponseMetadataTypeDef",
     "SelectRequestRequestTypeDef",
+    "SelectRequestSelectPaginateTypeDef",
     "DeletableItemTypeDef",
+    "GetAttributesResultTypeDef",
     "ItemTypeDef",
     "DeleteAttributesRequestRequestTypeDef",
-    "DomainMetadataResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAttributesResultTypeDef",
-    "ListDomainsResultTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    "SelectRequestSelectPaginateTypeDef",
     "PutAttributesRequestRequestTypeDef",
     "ReplaceableItemTypeDef",
     "BatchDeleteAttributesRequestRequestTypeDef",
     "SelectResultTypeDef",
     "BatchPutAttributesRequestRequestTypeDef",
 )
 
@@ -93,22 +93,32 @@
 DomainMetadataRequestRequestTypeDef = TypedDict(
     "DomainMetadataRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DomainMetadataResultTypeDef = TypedDict(
+    "DomainMetadataResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ItemCount": int,
+        "ItemNamesSizeBytes": int,
+        "AttributeNameCount": int,
+        "AttributeNamesSizeBytes": int,
+        "AttributeValueCount": int,
+        "AttributeValuesSizeBytes": int,
+        "Timestamp": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -125,33 +135,50 @@
 )
 
 class GetAttributesRequestRequestTypeDef(
     _RequiredGetAttributesRequestRequestTypeDef, _OptionalGetAttributesRequestRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "MaxNumberOfDomains": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListDomainsResultTypeDef = TypedDict(
+    "ListDomainsResultTypeDef",
+    {
+        "DomainNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
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
 _RequiredReplaceableAttributeTypeDef = TypedDict(
     "_RequiredReplaceableAttributeTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -164,14 +191,25 @@
 )
 
 class ReplaceableAttributeTypeDef(
     _RequiredReplaceableAttributeTypeDef, _OptionalReplaceableAttributeTypeDef
 ):
     pass
 
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
 _RequiredSelectRequestRequestTypeDef = TypedDict(
     "_RequiredSelectRequestRequestTypeDef",
     {
         "SelectExpression": str,
     },
 )
 _OptionalSelectRequestRequestTypeDef = TypedDict(
@@ -184,14 +222,34 @@
 )
 
 class SelectRequestRequestTypeDef(
     _RequiredSelectRequestRequestTypeDef, _OptionalSelectRequestRequestTypeDef
 ):
     pass
 
+_RequiredSelectRequestSelectPaginateTypeDef = TypedDict(
+    "_RequiredSelectRequestSelectPaginateTypeDef",
+    {
+        "SelectExpression": str,
+    },
+)
+_OptionalSelectRequestSelectPaginateTypeDef = TypedDict(
+    "_OptionalSelectRequestSelectPaginateTypeDef",
+    {
+        "ConsistentRead": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class SelectRequestSelectPaginateTypeDef(
+    _RequiredSelectRequestSelectPaginateTypeDef, _OptionalSelectRequestSelectPaginateTypeDef
+):
+    pass
+
 _RequiredDeletableItemTypeDef = TypedDict(
     "_RequiredDeletableItemTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDeletableItemTypeDef = TypedDict(
@@ -201,14 +259,22 @@
     },
     total=False,
 )
 
 class DeletableItemTypeDef(_RequiredDeletableItemTypeDef, _OptionalDeletableItemTypeDef):
     pass
 
+GetAttributesResultTypeDef = TypedDict(
+    "GetAttributesResultTypeDef",
+    {
+        "Attributes": List[AttributeTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredItemTypeDef = TypedDict(
     "_RequiredItemTypeDef",
     {
         "Name": str,
         "Attributes": List[AttributeTypeDef],
     },
 )
@@ -240,80 +306,14 @@
 )
 
 class DeleteAttributesRequestRequestTypeDef(
     _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
 ):
     pass
 
-DomainMetadataResultTypeDef = TypedDict(
-    "DomainMetadataResultTypeDef",
-    {
-        "ItemCount": int,
-        "ItemNamesSizeBytes": int,
-        "AttributeNameCount": int,
-        "AttributeNamesSizeBytes": int,
-        "AttributeValueCount": int,
-        "AttributeValuesSizeBytes": int,
-        "Timestamp": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAttributesResultTypeDef = TypedDict(
-    "GetAttributesResultTypeDef",
-    {
-        "Attributes": List[AttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDomainsResultTypeDef = TypedDict(
-    "ListDomainsResultTypeDef",
-    {
-        "DomainNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredSelectRequestSelectPaginateTypeDef = TypedDict(
-    "_RequiredSelectRequestSelectPaginateTypeDef",
-    {
-        "SelectExpression": str,
-    },
-)
-_OptionalSelectRequestSelectPaginateTypeDef = TypedDict(
-    "_OptionalSelectRequestSelectPaginateTypeDef",
-    {
-        "ConsistentRead": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class SelectRequestSelectPaginateTypeDef(
-    _RequiredSelectRequestSelectPaginateTypeDef, _OptionalSelectRequestSelectPaginateTypeDef
-):
-    pass
-
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
         "ItemName": str,
         "Attributes": Sequence[ReplaceableAttributeTypeDef],
     },
@@ -348,15 +348,15 @@
 )
 
 SelectResultTypeDef = TypedDict(
     "SelectResultTypeDef",
     {
         "Items": List[ItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutAttributesRequestRequestTypeDef = TypedDict(
     "BatchPutAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
```

### Comparing `mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb.egg-info/PKG-INFO` & `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sdb
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.SimpleDB 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.SimpleDB 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/
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
 
 <a id="mypy-boto3-sdb"></a>
 
 # mypy-boto3-sdb
 
 [![PyPI - mypy-boto3-sdb](https://img.shields.io/pypi/v/mypy-boto3-sdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-sdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-sdb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sdb?color=blue)](https://pypistats.org/packages/mypy-boto3-sdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimpleDB 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
+[boto3.SimpleDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
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
 [mypy-boto3-sdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,29 +324,29 @@
 ```python
 from mypy_boto3_sdb.type_defs import (
     AttributeTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateConditionTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainMetadataRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DomainMetadataResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetAttributesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListDomainsResultTypeDef,
+    PaginatorConfigTypeDef,
     ReplaceableAttributeTypeDef,
+    ResponseMetadataTypeDef,
     SelectRequestRequestTypeDef,
+    SelectRequestSelectPaginateTypeDef,
     DeletableItemTypeDef,
+    GetAttributesResultTypeDef,
     ItemTypeDef,
     DeleteAttributesRequestRequestTypeDef,
-    DomainMetadataResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAttributesResultTypeDef,
-    ListDomainsResultTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    SelectRequestSelectPaginateTypeDef,
     PutAttributesRequestRequestTypeDef,
     ReplaceableItemTypeDef,
     BatchDeleteAttributesRequestRequestTypeDef,
     SelectResultTypeDef,
     BatchPutAttributesRequestRequestTypeDef,
 )
 
@@ -357,42 +358,42 @@
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

### Comparing `mypy-boto3-sdb-1.26.0.post1/mypy_boto3_sdb.egg-info/SOURCES.txt` & `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.26.0.post1/setup.py` & `mypy-boto3-sdb-1.27.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-sdb.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sdb",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_sdb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SimpleDB 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.SimpleDB 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 sdb type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_sdb": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_sdb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/",
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


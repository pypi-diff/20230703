# Comparing `tmp/mypy-boto3-marketplace-catalog-1.26.8.tar.gz` & `tmp/mypy-boto3-marketplace-catalog-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-marketplace-catalog-1.26.8.tar", last modified: Fri Nov 11 21:07:54 2022, max compression
+gzip compressed data, was "mypy-boto3-marketplace-catalog-1.27.0.tar", last modified: Mon Jul  3 19:51:05 2023, max compression
```

## Comparing `mypy-boto3-marketplace-catalog-1.26.8.tar` & `mypy-boto3-marketplace-catalog-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.066122 mypy-boto3-marketplace-catalog-1.26.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13287 2022-11-11 21:07:54.066122 mypy-boto3-marketplace-catalog-1.26.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11805 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.066122 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9814 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     9799 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7238 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7236 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     8466 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8456 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.066122 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13287 2022-11-11 21:07:53.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-11-11 21:07:53.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-11 21:07:53.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-11-11 21:07:53.000000 mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 21:07:54.066122 mypy-boto3-marketplace-catalog-1.26.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-11-11 21:07:30.000000 mypy-boto3-marketplace-catalog-1.26.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:05.571632 mypy-boto3-marketplace-catalog-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:36.000000 mypy-boto3-marketplace-catalog-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14539 2023-07-03 19:51:05.571632 mypy-boto3-marketplace-catalog-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-07-03 19:41:36.000000 mypy-boto3-marketplace-catalog-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:05.571632 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 19:41:36.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-03 19:41:36.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-03 19:41:36.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-07-03 19:41:36.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-07-03 19:41:36.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-07-03 19:41:36.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-07-03 19:41:36.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-03 19:41:36.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-03 19:41:36.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:36.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-03 19:41:37.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-07-03 19:41:36.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:36.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:05.571632 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14539 2023-07-03 19:51:05.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:51:05.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:05.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:05.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:05.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 19:51:05.000000 mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:05.571632 mypy-boto3-marketplace-catalog-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-03 19:41:36.000000 mypy-boto3-marketplace-catalog-1.27.0/setup.py
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.8/LICENSE` & `mypy-boto3-marketplace-catalog-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-marketplace-catalog-1.26.8/PKG-INFO` & `mypy-boto3-marketplace-catalog-1.27.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplace-catalog
-Version: 1.26.8
-Summary: Type annotations for boto3.MarketplaceCatalog 1.26.8 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.MarketplaceCatalog 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/
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
 
 <a id="mypy-boto3-marketplace-catalog"></a>
 
 # mypy-boto3-marketplace-catalog
 
 [![PyPI - mypy-boto3-marketplace-catalog](https://img.shields.io/pypi/v/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-marketplace-catalog?color=blue)](https://pypistats.org/packages/mypy-boto3-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCatalog 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[boto3.MarketplaceCatalog 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
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
 [mypy-boto3-marketplace-catalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -71,14 +72,15 @@
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
@@ -267,29 +269,54 @@
 from mypy_boto3_marketplace_catalog import MarketplaceCatalogClient
 
 client: MarketplaceCatalogClient = Session().client("marketplace-catalog")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_marketplace_catalog.paginator` module contains type annotations for
+all paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_marketplace_catalog import MarketplaceCatalogClient
+from mypy_boto3_marketplace_catalog.paginator import ListChangeSetsPaginator, ListEntitiesPaginator
+
+client: MarketplaceCatalogClient = Session().client("marketplace-catalog")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+list_change_sets_paginator: ListChangeSetsPaginator = client.get_paginator("list_change_sets")
+list_entities_paginator: ListEntitiesPaginator = client.get_paginator("list_entities")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_marketplace_catalog.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.literals import (
     ChangeStatusType,
     FailureCodeType,
+    ListChangeSetsPaginatorName,
+    ListEntitiesPaginatorName,
+    OwnershipTypeType,
     SortOrderType,
     MarketplaceCatalogServiceName,
     ServiceName,
     ResourceServiceName,
+    PaginatorName,
     RegionName,
 )
 
 
 def check_value(value: ChangeStatusType) -> bool:
     ...
 ```
@@ -300,36 +327,43 @@
 
 `mypy_boto3_marketplace_catalog.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelChangeSetResponseTypeDef,
     ChangeSetSummaryListItemTypeDef,
     EntityTypeDef,
     ErrorDetailTypeDef,
     TagTypeDef,
+    DeleteResourcePolicyRequestRequestTypeDef,
     DescribeChangeSetRequestRequestTypeDef,
     DescribeEntityRequestRequestTypeDef,
+    DescribeEntityResponseTypeDef,
     EntitySummaryTypeDef,
     FilterTypeDef,
+    GetResourcePolicyRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
     SortTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CancelChangeSetResponseTypeDef,
-    DescribeEntityResponseTypeDef,
+    PaginatorConfigTypeDef,
+    PutResourcePolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     StartChangeSetResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
     ListChangeSetsResponseTypeDef,
     ChangeSummaryTypeDef,
     ChangeTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEntitiesResponseTypeDef,
+    ListChangeSetsRequestListChangeSetsPaginateTypeDef,
     ListChangeSetsRequestRequestTypeDef,
+    ListEntitiesRequestListEntitiesPaginateTypeDef,
     ListEntitiesRequestRequestTypeDef,
     DescribeChangeSetResponseTypeDef,
     StartChangeSetRequestRequestTypeDef,
 )
 
 
 def get_structure() -> CancelChangeSetRequestRequestTypeDef:
@@ -339,42 +373,42 @@
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

### Comparing `mypy-boto3-marketplace-catalog-1.26.8/README.md` & `mypy-boto3-marketplace-catalog-1.27.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-marketplace-catalog"></a>
 
 # mypy-boto3-marketplace-catalog
 
 [![PyPI - mypy-boto3-marketplace-catalog](https://img.shields.io/pypi/v/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-marketplace-catalog?color=blue)](https://pypistats.org/packages/mypy-boto3-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCatalog 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[boto3.MarketplaceCatalog 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
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
 [mypy-boto3-marketplace-catalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/).
 
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
@@ -236,29 +237,54 @@
 from mypy_boto3_marketplace_catalog import MarketplaceCatalogClient
 
 client: MarketplaceCatalogClient = Session().client("marketplace-catalog")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_marketplace_catalog.paginator` module contains type annotations for
+all paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_marketplace_catalog import MarketplaceCatalogClient
+from mypy_boto3_marketplace_catalog.paginator import ListChangeSetsPaginator, ListEntitiesPaginator
+
+client: MarketplaceCatalogClient = Session().client("marketplace-catalog")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+list_change_sets_paginator: ListChangeSetsPaginator = client.get_paginator("list_change_sets")
+list_entities_paginator: ListEntitiesPaginator = client.get_paginator("list_entities")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_marketplace_catalog.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.literals import (
     ChangeStatusType,
     FailureCodeType,
+    ListChangeSetsPaginatorName,
+    ListEntitiesPaginatorName,
+    OwnershipTypeType,
     SortOrderType,
     MarketplaceCatalogServiceName,
     ServiceName,
     ResourceServiceName,
+    PaginatorName,
     RegionName,
 )
 
 
 def check_value(value: ChangeStatusType) -> bool:
     ...
 ```
@@ -269,36 +295,43 @@
 
 `mypy_boto3_marketplace_catalog.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelChangeSetResponseTypeDef,
     ChangeSetSummaryListItemTypeDef,
     EntityTypeDef,
     ErrorDetailTypeDef,
     TagTypeDef,
+    DeleteResourcePolicyRequestRequestTypeDef,
     DescribeChangeSetRequestRequestTypeDef,
     DescribeEntityRequestRequestTypeDef,
+    DescribeEntityResponseTypeDef,
     EntitySummaryTypeDef,
     FilterTypeDef,
+    GetResourcePolicyRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
     SortTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CancelChangeSetResponseTypeDef,
-    DescribeEntityResponseTypeDef,
+    PaginatorConfigTypeDef,
+    PutResourcePolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     StartChangeSetResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
     ListChangeSetsResponseTypeDef,
     ChangeSummaryTypeDef,
     ChangeTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEntitiesResponseTypeDef,
+    ListChangeSetsRequestListChangeSetsPaginateTypeDef,
     ListChangeSetsRequestRequestTypeDef,
+    ListEntitiesRequestListEntitiesPaginateTypeDef,
     ListEntitiesRequestRequestTypeDef,
     DescribeChangeSetResponseTypeDef,
     StartChangeSetRequestRequestTypeDef,
 )
 
 
 def get_structure() -> CancelChangeSetRequestRequestTypeDef:
@@ -308,42 +341,42 @@
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

### Comparing `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/__main__.py` & `mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MarketplaceCatalog 1.26.8\nVersion:         1.26.8\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.MarketplaceCatalog 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.8")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/client.py` & `mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,32 +9,42 @@
     from boto3.session import Session
     from mypy_boto3_marketplace_catalog.client import MarketplaceCatalogClient
 
     session = Session()
     client: MarketplaceCatalogClient = session.client("marketplace-catalog")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+import sys
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
+from .literals import OwnershipTypeType
+from .paginator import ListChangeSetsPaginator, ListEntitiesPaginator
 from .type_defs import (
     CancelChangeSetResponseTypeDef,
     ChangeTypeDef,
     DescribeChangeSetResponseTypeDef,
     DescribeEntityResponseTypeDef,
     FilterTypeDef,
+    GetResourcePolicyResponseTypeDef,
     ListChangeSetsResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SortTypeDef,
     StartChangeSetResponseTypeDef,
     TagTypeDef,
 )
 
+if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
+
 __all__ = ("MarketplaceCatalogClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -93,14 +103,23 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#close)
         """
 
+    def delete_resource_policy(self, *, ResourceArn: str) -> Dict[str, Any]:
+        """
+        Deletes a resource-based policy on an Entity that is identified by its resource
+        ARN.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.delete_resource_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#delete_resource_policy)
+        """
+
     def describe_change_set(
         self, *, Catalog: str, ChangeSetId: str
     ) -> DescribeChangeSetResponseTypeDef:
         """
         Provides information about a given change set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.describe_change_set)
@@ -125,14 +144,23 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#generate_presigned_url)
         """
 
+    def get_resource_policy(self, *, ResourceArn: str) -> GetResourcePolicyResponseTypeDef:
+        """
+        Gets a resource-based policy of an Entity that is identified by its resource
+        ARN.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.get_resource_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#get_resource_policy)
+        """
+
     def list_change_sets(
         self,
         *,
         Catalog: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         MaxResults: int = ...,
@@ -150,15 +178,16 @@
         self,
         *,
         Catalog: str,
         EntityType: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
+        OwnershipType: OwnershipTypeType = ...
     ) -> ListEntitiesResponseTypeDef:
         """
         Provides the list of entities of a given type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#list_entities)
         """
@@ -171,14 +200,22 @@
         <https://docs.aws.amazon.com/marketplace-catalog/latest/api-
         reference/welcome.html#working-with-change-se...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#list_tags_for_resource)
         """
 
+    def put_resource_policy(self, *, ResourceArn: str, Policy: str) -> Dict[str, Any]:
+        """
+        Attaches a resource-based policy to an Entity.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.put_resource_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#put_resource_policy)
+        """
+
     def start_change_set(
         self,
         *,
         Catalog: str,
         ChangeSet: Sequence[ChangeTypeDef],
         ChangeSetName: str = ...,
         ClientRequestToken: str = ...,
@@ -192,15 +229,15 @@
         """
 
     def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Tags a resource (either an [entity](https://docs.aws.amazon.com/marketplace-
         catalog/latest/api-reference/welcome.html#catalog-api-entities)_ or [change
         set](https://docs.aws.amazon.com/marketplace-catalog/latest/api-
-        reference/welcome.html#working-with-change-sets)_ ).
+        reference/welcome.html#working-with-change-sets)_).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#tag_resource)
         """
 
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
@@ -209,7 +246,21 @@
         reference/welcome.html#catalog-api-entities)_ or [change
         set](https://docs.aws.amazon.com/marketplace-catalog/latest/api-
         reference/welcome.html#working-with-change-sets)...
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#untag_resource)
         """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["list_change_sets"]) -> ListChangeSetsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(self, operation_name: Literal["list_entities"]) -> ListEntitiesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/client.pyi` & `mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/client.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -9,32 +9,41 @@
     from boto3.session import Session
     from mypy_boto3_marketplace_catalog.client import MarketplaceCatalogClient
 
     session = Session()
     client: MarketplaceCatalogClient = session.client("marketplace-catalog")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+import sys
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
+from .literals import OwnershipTypeType
+from .paginator import ListChangeSetsPaginator, ListEntitiesPaginator
 from .type_defs import (
     CancelChangeSetResponseTypeDef,
     ChangeTypeDef,
     DescribeChangeSetResponseTypeDef,
     DescribeEntityResponseTypeDef,
     FilterTypeDef,
+    GetResourcePolicyResponseTypeDef,
     ListChangeSetsResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SortTypeDef,
     StartChangeSetResponseTypeDef,
     TagTypeDef,
 )
 
+if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 __all__ = ("MarketplaceCatalogClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
@@ -86,14 +95,22 @@
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#close)
         """
+    def delete_resource_policy(self, *, ResourceArn: str) -> Dict[str, Any]:
+        """
+        Deletes a resource-based policy on an Entity that is identified by its resource
+        ARN.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.delete_resource_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#delete_resource_policy)
+        """
     def describe_change_set(
         self, *, Catalog: str, ChangeSetId: str
     ) -> DescribeChangeSetResponseTypeDef:
         """
         Provides information about a given change set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.describe_change_set)
@@ -115,14 +132,22 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#generate_presigned_url)
         """
+    def get_resource_policy(self, *, ResourceArn: str) -> GetResourcePolicyResponseTypeDef:
+        """
+        Gets a resource-based policy of an Entity that is identified by its resource
+        ARN.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.get_resource_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#get_resource_policy)
+        """
     def list_change_sets(
         self,
         *,
         Catalog: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         MaxResults: int = ...,
@@ -139,15 +164,16 @@
         self,
         *,
         Catalog: str,
         EntityType: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
+        OwnershipType: OwnershipTypeType = ...
     ) -> ListEntitiesResponseTypeDef:
         """
         Provides the list of entities of a given type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#list_entities)
         """
@@ -158,14 +184,21 @@
         reference/welcome.html#catalog-api-entities)_ or `change set
         <https://docs.aws.amazon.com/marketplace-catalog/latest/api-
         reference/welcome.html#working-with-change-se...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#list_tags_for_resource)
         """
+    def put_resource_policy(self, *, ResourceArn: str, Policy: str) -> Dict[str, Any]:
+        """
+        Attaches a resource-based policy to an Entity.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.put_resource_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#put_resource_policy)
+        """
     def start_change_set(
         self,
         *,
         Catalog: str,
         ChangeSet: Sequence[ChangeTypeDef],
         ChangeSetName: str = ...,
         ClientRequestToken: str = ...,
@@ -178,15 +211,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#start_change_set)
         """
     def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Tags a resource (either an [entity](https://docs.aws.amazon.com/marketplace-
         catalog/latest/api-reference/welcome.html#catalog-api-entities)_ or [change
         set](https://docs.aws.amazon.com/marketplace-catalog/latest/api-
-        reference/welcome.html#working-with-change-sets)_ ).
+        reference/welcome.html#working-with-change-sets)_).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#tag_resource)
         """
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag or list of tags from a resource (either an
@@ -194,7 +227,19 @@
         reference/welcome.html#catalog-api-entities)_ or [change
         set](https://docs.aws.amazon.com/marketplace-catalog/latest/api-
         reference/welcome.html#working-with-change-sets)...
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#untag_resource)
         """
+    @overload
+    def get_paginator(self, operation_name: Literal["list_change_sets"]) -> ListChangeSetsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(self, operation_name: Literal["list_entities"]) -> ListEntitiesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/client/#get_paginator)
+        """
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/literals.py` & `mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/literals.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,24 +18,31 @@
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "ChangeStatusType",
     "FailureCodeType",
+    "ListChangeSetsPaginatorName",
+    "ListEntitiesPaginatorName",
+    "OwnershipTypeType",
     "SortOrderType",
     "MarketplaceCatalogServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "PaginatorName",
     "RegionName",
 )
 
 
 ChangeStatusType = Literal["APPLYING", "CANCELLED", "FAILED", "PREPARING", "SUCCEEDED"]
 FailureCodeType = Literal["CLIENT_ERROR", "SERVER_FAULT"]
+ListChangeSetsPaginatorName = Literal["list_change_sets"]
+ListEntitiesPaginatorName = Literal["list_entities"]
+OwnershipTypeType = Literal["SELF", "SHARED"]
 SortOrderType = Literal["ASCENDING", "DESCENDING"]
 MarketplaceCatalogServiceName = Literal["marketplace-catalog"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -45,23 +52,25 @@
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
@@ -71,30 +80,35 @@
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
@@ -120,14 +134,15 @@
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
@@ -172,51 +187,57 @@
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
@@ -229,14 +250,15 @@
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
@@ -248,28 +270,35 @@
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
@@ -297,56 +326,64 @@
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
@@ -364,8 +401,9 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+PaginatorName = Literal["list_change_sets", "list_entities"]
 RegionName = Literal["us-east-1"]
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/literals.pyi` & `mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/literals.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -17,23 +17,30 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "ChangeStatusType",
     "FailureCodeType",
+    "ListChangeSetsPaginatorName",
+    "ListEntitiesPaginatorName",
+    "OwnershipTypeType",
     "SortOrderType",
     "MarketplaceCatalogServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "PaginatorName",
     "RegionName",
 )
 
 ChangeStatusType = Literal["APPLYING", "CANCELLED", "FAILED", "PREPARING", "SUCCEEDED"]
 FailureCodeType = Literal["CLIENT_ERROR", "SERVER_FAULT"]
+ListChangeSetsPaginatorName = Literal["list_change_sets"]
+ListEntitiesPaginatorName = Literal["list_entities"]
+OwnershipTypeType = Literal["SELF", "SHARED"]
 SortOrderType = Literal["ASCENDING", "DESCENDING"]
 MarketplaceCatalogServiceName = Literal["marketplace-catalog"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -43,23 +50,25 @@
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
@@ -69,30 +78,35 @@
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
@@ -118,14 +132,15 @@
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
@@ -170,51 +185,57 @@
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
@@ -227,14 +248,15 @@
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
@@ -246,28 +268,35 @@
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
@@ -295,56 +324,64 @@
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
@@ -362,8 +399,9 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+PaginatorName = Literal["list_change_sets", "list_entities"]
 RegionName = Literal["us-east-1"]
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/type_defs.py` & `mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/type_defs.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -10,67 +10,71 @@
 
     data: CancelChangeSetRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
-from .literals import ChangeStatusType, FailureCodeType, SortOrderType
+from .literals import ChangeStatusType, FailureCodeType, OwnershipTypeType, SortOrderType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelChangeSetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelChangeSetResponseTypeDef",
     "ChangeSetSummaryListItemTypeDef",
     "EntityTypeDef",
     "ErrorDetailTypeDef",
     "TagTypeDef",
+    "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeChangeSetRequestRequestTypeDef",
     "DescribeEntityRequestRequestTypeDef",
+    "DescribeEntityResponseTypeDef",
     "EntitySummaryTypeDef",
     "FilterTypeDef",
+    "GetResourcePolicyRequestRequestTypeDef",
+    "GetResourcePolicyResponseTypeDef",
     "SortTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "CancelChangeSetResponseTypeDef",
-    "DescribeEntityResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "PutResourcePolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "StartChangeSetResponseTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "ListChangeSetsResponseTypeDef",
     "ChangeSummaryTypeDef",
     "ChangeTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEntitiesResponseTypeDef",
+    "ListChangeSetsRequestListChangeSetsPaginateTypeDef",
     "ListChangeSetsRequestRequestTypeDef",
+    "ListEntitiesRequestListEntitiesPaginateTypeDef",
     "ListEntitiesRequestRequestTypeDef",
     "DescribeChangeSetResponseTypeDef",
     "StartChangeSetRequestRequestTypeDef",
 )
 
 CancelChangeSetRequestRequestTypeDef = TypedDict(
     "CancelChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
         "ChangeSetId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelChangeSetResponseTypeDef = TypedDict(
+    "CancelChangeSetResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ChangeSetId": str,
+        "ChangeSetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeSetSummaryListItemTypeDef = TypedDict(
     "ChangeSetSummaryListItemTypeDef",
     {
         "ChangeSetId": str,
@@ -95,19 +99,17 @@
     "_OptionalEntityTypeDef",
     {
         "Identifier": str,
     },
     total=False,
 )
 
-
 class EntityTypeDef(_RequiredEntityTypeDef, _OptionalEntityTypeDef):
     pass
 
-
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
@@ -117,14 +119,21 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
+    "DeleteResourcePolicyRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+
 DescribeChangeSetRequestRequestTypeDef = TypedDict(
     "DescribeChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
         "ChangeSetId": str,
     },
 )
@@ -133,14 +142,26 @@
     "DescribeEntityRequestRequestTypeDef",
     {
         "Catalog": str,
         "EntityId": str,
     },
 )
 
+DescribeEntityResponseTypeDef = TypedDict(
+    "DescribeEntityResponseTypeDef",
+    {
+        "EntityType": str,
+        "EntityIdentifier": str,
+        "EntityArn": str,
+        "LastModifiedDate": str,
+        "Details": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EntitySummaryTypeDef = TypedDict(
     "EntitySummaryTypeDef",
     {
         "Name": str,
         "EntityType": str,
         "EntityId": str,
         "EntityArn": str,
@@ -155,14 +176,29 @@
     {
         "Name": str,
         "ValueList": Sequence[str],
     },
     total=False,
 )
 
+GetResourcePolicyRequestRequestTypeDef = TypedDict(
+    "GetResourcePolicyRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "SortBy": str,
         "SortOrder": SortOrderType,
     },
     total=False,
@@ -171,58 +207,66 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-CancelChangeSetResponseTypeDef = TypedDict(
-    "CancelChangeSetResponseTypeDef",
+PutResourcePolicyRequestRequestTypeDef = TypedDict(
+    "PutResourcePolicyRequestRequestTypeDef",
     {
-        "ChangeSetId": str,
-        "ChangeSetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "Policy": str,
     },
 )
 
-DescribeEntityResponseTypeDef = TypedDict(
-    "DescribeEntityResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "EntityType": str,
-        "EntityIdentifier": str,
-        "EntityArn": str,
-        "LastModifiedDate": str,
-        "Details": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 StartChangeSetResponseTypeDef = TypedDict(
     "StartChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
 ListChangeSetsResponseTypeDef = TypedDict(
     "ListChangeSetsResponseTypeDef",
     {
         "ChangeSetSummaryList": List[ChangeSetSummaryListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeSummaryTypeDef = TypedDict(
     "ChangeSummaryTypeDef",
     {
         "ChangeType": str,
@@ -247,25 +291,23 @@
     {
         "EntityTags": Sequence[TagTypeDef],
         "ChangeName": str,
     },
     total=False,
 )
 
-
 class ChangeTypeDef(_RequiredChangeTypeDef, _OptionalChangeTypeDef):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -274,17 +316,39 @@
 )
 
 ListEntitiesResponseTypeDef = TypedDict(
     "ListEntitiesResponseTypeDef",
     {
         "EntitySummaryList": List[EntitySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef = TypedDict(
+    "_RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef",
+    {
+        "Catalog": str,
     },
 )
+_OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef = TypedDict(
+    "_OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef",
+    {
+        "FilterList": Sequence[FilterTypeDef],
+        "Sort": SortTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListChangeSetsRequestListChangeSetsPaginateTypeDef(
+    _RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef,
+    _OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef,
+):
+    pass
 
 _RequiredListChangeSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsRequestRequestTypeDef",
     {
         "Catalog": str,
     },
 )
@@ -295,20 +359,42 @@
         "Sort": SortTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListChangeSetsRequestRequestTypeDef(
     _RequiredListChangeSetsRequestRequestTypeDef, _OptionalListChangeSetsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListEntitiesRequestListEntitiesPaginateTypeDef = TypedDict(
+    "_RequiredListEntitiesRequestListEntitiesPaginateTypeDef",
+    {
+        "Catalog": str,
+        "EntityType": str,
+    },
+)
+_OptionalListEntitiesRequestListEntitiesPaginateTypeDef = TypedDict(
+    "_OptionalListEntitiesRequestListEntitiesPaginateTypeDef",
+    {
+        "FilterList": Sequence[FilterTypeDef],
+        "Sort": SortTypeDef,
+        "OwnershipType": OwnershipTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListEntitiesRequestListEntitiesPaginateTypeDef(
+    _RequiredListEntitiesRequestListEntitiesPaginateTypeDef,
+    _OptionalListEntitiesRequestListEntitiesPaginateTypeDef,
+):
+    pass
 
 _RequiredListEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredListEntitiesRequestRequestTypeDef",
     {
         "Catalog": str,
         "EntityType": str,
     },
@@ -316,38 +402,37 @@
 _OptionalListEntitiesRequestRequestTypeDef = TypedDict(
     "_OptionalListEntitiesRequestRequestTypeDef",
     {
         "FilterList": Sequence[FilterTypeDef],
         "Sort": SortTypeDef,
         "NextToken": str,
         "MaxResults": int,
+        "OwnershipType": OwnershipTypeType,
     },
     total=False,
 )
 
-
 class ListEntitiesRequestRequestTypeDef(
     _RequiredListEntitiesRequestRequestTypeDef, _OptionalListEntitiesRequestRequestTypeDef
 ):
     pass
 
-
 DescribeChangeSetResponseTypeDef = TypedDict(
     "DescribeChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
         "ChangeSetName": str,
         "StartTime": str,
         "EndTime": str,
         "Status": ChangeStatusType,
         "FailureCode": FailureCodeType,
         "FailureDescription": str,
         "ChangeSet": List[ChangeSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartChangeSetRequestRequestTypeDef = TypedDict(
     "_RequiredStartChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
@@ -360,12 +445,11 @@
         "ChangeSetName": str,
         "ClientRequestToken": str,
         "ChangeSetTags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartChangeSetRequestRequestTypeDef(
     _RequiredStartChangeSetRequestRequestTypeDef, _OptionalStartChangeSetRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog/type_defs.pyi` & `mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog/type_defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,66 +10,72 @@
 
     data: CancelChangeSetRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
-from .literals import ChangeStatusType, FailureCodeType, SortOrderType
+from .literals import ChangeStatusType, FailureCodeType, OwnershipTypeType, SortOrderType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CancelChangeSetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelChangeSetResponseTypeDef",
     "ChangeSetSummaryListItemTypeDef",
     "EntityTypeDef",
     "ErrorDetailTypeDef",
     "TagTypeDef",
+    "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeChangeSetRequestRequestTypeDef",
     "DescribeEntityRequestRequestTypeDef",
+    "DescribeEntityResponseTypeDef",
     "EntitySummaryTypeDef",
     "FilterTypeDef",
+    "GetResourcePolicyRequestRequestTypeDef",
+    "GetResourcePolicyResponseTypeDef",
     "SortTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "CancelChangeSetResponseTypeDef",
-    "DescribeEntityResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "PutResourcePolicyRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "StartChangeSetResponseTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "ListChangeSetsResponseTypeDef",
     "ChangeSummaryTypeDef",
     "ChangeTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEntitiesResponseTypeDef",
+    "ListChangeSetsRequestListChangeSetsPaginateTypeDef",
     "ListChangeSetsRequestRequestTypeDef",
+    "ListEntitiesRequestListEntitiesPaginateTypeDef",
     "ListEntitiesRequestRequestTypeDef",
     "DescribeChangeSetResponseTypeDef",
     "StartChangeSetRequestRequestTypeDef",
 )
 
 CancelChangeSetRequestRequestTypeDef = TypedDict(
     "CancelChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
         "ChangeSetId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelChangeSetResponseTypeDef = TypedDict(
+    "CancelChangeSetResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ChangeSetId": str,
+        "ChangeSetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeSetSummaryListItemTypeDef = TypedDict(
     "ChangeSetSummaryListItemTypeDef",
     {
         "ChangeSetId": str,
@@ -94,17 +100,19 @@
     "_OptionalEntityTypeDef",
     {
         "Identifier": str,
     },
     total=False,
 )
 
+
 class EntityTypeDef(_RequiredEntityTypeDef, _OptionalEntityTypeDef):
     pass
 
+
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
@@ -114,14 +122,21 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
+    "DeleteResourcePolicyRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+
 DescribeChangeSetRequestRequestTypeDef = TypedDict(
     "DescribeChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
         "ChangeSetId": str,
     },
 )
@@ -130,14 +145,26 @@
     "DescribeEntityRequestRequestTypeDef",
     {
         "Catalog": str,
         "EntityId": str,
     },
 )
 
+DescribeEntityResponseTypeDef = TypedDict(
+    "DescribeEntityResponseTypeDef",
+    {
+        "EntityType": str,
+        "EntityIdentifier": str,
+        "EntityArn": str,
+        "LastModifiedDate": str,
+        "Details": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EntitySummaryTypeDef = TypedDict(
     "EntitySummaryTypeDef",
     {
         "Name": str,
         "EntityType": str,
         "EntityId": str,
         "EntityArn": str,
@@ -152,14 +179,29 @@
     {
         "Name": str,
         "ValueList": Sequence[str],
     },
     total=False,
 )
 
+GetResourcePolicyRequestRequestTypeDef = TypedDict(
+    "GetResourcePolicyRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "SortBy": str,
         "SortOrder": SortOrderType,
     },
     total=False,
@@ -168,58 +210,66 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-CancelChangeSetResponseTypeDef = TypedDict(
-    "CancelChangeSetResponseTypeDef",
+PutResourcePolicyRequestRequestTypeDef = TypedDict(
+    "PutResourcePolicyRequestRequestTypeDef",
     {
-        "ChangeSetId": str,
-        "ChangeSetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "Policy": str,
     },
 )
 
-DescribeEntityResponseTypeDef = TypedDict(
-    "DescribeEntityResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "EntityType": str,
-        "EntityIdentifier": str,
-        "EntityArn": str,
-        "LastModifiedDate": str,
-        "Details": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 StartChangeSetResponseTypeDef = TypedDict(
     "StartChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
 ListChangeSetsResponseTypeDef = TypedDict(
     "ListChangeSetsResponseTypeDef",
     {
         "ChangeSetSummaryList": List[ChangeSetSummaryListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChangeSummaryTypeDef = TypedDict(
     "ChangeSummaryTypeDef",
     {
         "ChangeType": str,
@@ -244,23 +294,25 @@
     {
         "EntityTags": Sequence[TagTypeDef],
         "ChangeName": str,
     },
     total=False,
 )
 
+
 class ChangeTypeDef(_RequiredChangeTypeDef, _OptionalChangeTypeDef):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -269,18 +321,42 @@
 )
 
 ListEntitiesResponseTypeDef = TypedDict(
     "ListEntitiesResponseTypeDef",
     {
         "EntitySummaryList": List[EntitySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef = TypedDict(
+    "_RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef",
+    {
+        "Catalog": str,
+    },
+)
+_OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef = TypedDict(
+    "_OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef",
+    {
+        "FilterList": Sequence[FilterTypeDef],
+        "Sort": SortTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListChangeSetsRequestListChangeSetsPaginateTypeDef(
+    _RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef,
+    _OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListChangeSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsRequestRequestTypeDef",
     {
         "Catalog": str,
     },
 )
 _OptionalListChangeSetsRequestRequestTypeDef = TypedDict(
@@ -290,55 +366,86 @@
         "Sort": SortTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListChangeSetsRequestRequestTypeDef(
     _RequiredListChangeSetsRequestRequestTypeDef, _OptionalListChangeSetsRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredListEntitiesRequestListEntitiesPaginateTypeDef = TypedDict(
+    "_RequiredListEntitiesRequestListEntitiesPaginateTypeDef",
+    {
+        "Catalog": str,
+        "EntityType": str,
+    },
+)
+_OptionalListEntitiesRequestListEntitiesPaginateTypeDef = TypedDict(
+    "_OptionalListEntitiesRequestListEntitiesPaginateTypeDef",
+    {
+        "FilterList": Sequence[FilterTypeDef],
+        "Sort": SortTypeDef,
+        "OwnershipType": OwnershipTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListEntitiesRequestListEntitiesPaginateTypeDef(
+    _RequiredListEntitiesRequestListEntitiesPaginateTypeDef,
+    _OptionalListEntitiesRequestListEntitiesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredListEntitiesRequestRequestTypeDef",
     {
         "Catalog": str,
         "EntityType": str,
     },
 )
 _OptionalListEntitiesRequestRequestTypeDef = TypedDict(
     "_OptionalListEntitiesRequestRequestTypeDef",
     {
         "FilterList": Sequence[FilterTypeDef],
         "Sort": SortTypeDef,
         "NextToken": str,
         "MaxResults": int,
+        "OwnershipType": OwnershipTypeType,
     },
     total=False,
 )
 
+
 class ListEntitiesRequestRequestTypeDef(
     _RequiredListEntitiesRequestRequestTypeDef, _OptionalListEntitiesRequestRequestTypeDef
 ):
     pass
 
+
 DescribeChangeSetResponseTypeDef = TypedDict(
     "DescribeChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
         "ChangeSetName": str,
         "StartTime": str,
         "EndTime": str,
         "Status": ChangeStatusType,
         "FailureCode": FailureCodeType,
         "FailureDescription": str,
         "ChangeSet": List[ChangeSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartChangeSetRequestRequestTypeDef = TypedDict(
     "_RequiredStartChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
@@ -351,11 +458,12 @@
         "ChangeSetName": str,
         "ClientRequestToken": str,
         "ChangeSetTags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartChangeSetRequestRequestTypeDef(
     _RequiredStartChangeSetRequestRequestTypeDef, _OptionalStartChangeSetRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO` & `mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-marketplace-catalog
-Version: 1.26.8
-Summary: Type annotations for boto3.MarketplaceCatalog 1.26.8 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.MarketplaceCatalog 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/
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
 
 <a id="mypy-boto3-marketplace-catalog"></a>
 
 # mypy-boto3-marketplace-catalog
 
 [![PyPI - mypy-boto3-marketplace-catalog](https://img.shields.io/pypi/v/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-marketplace-catalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-marketplace-catalog)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-marketplace-catalog?color=blue)](https://pypistats.org/packages/mypy-boto3-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceCatalog 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[boto3.MarketplaceCatalog 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
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
 [mypy-boto3-marketplace-catalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -71,14 +72,15 @@
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
@@ -267,29 +269,54 @@
 from mypy_boto3_marketplace_catalog import MarketplaceCatalogClient
 
 client: MarketplaceCatalogClient = Session().client("marketplace-catalog")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
+<a id="paginators-annotations"></a>
+
+### Paginators annotations
+
+`mypy_boto3_marketplace_catalog.paginator` module contains type annotations for
+all paginators.
+
+```python
+from boto3.session import Session
+
+from mypy_boto3_marketplace_catalog import MarketplaceCatalogClient
+from mypy_boto3_marketplace_catalog.paginator import ListChangeSetsPaginator, ListEntitiesPaginator
+
+client: MarketplaceCatalogClient = Session().client("marketplace-catalog")
+
+# Explicit type annotations are optional here
+# Types should be correctly discovered by mypy and IDEs
+list_change_sets_paginator: ListChangeSetsPaginator = client.get_paginator("list_change_sets")
+list_entities_paginator: ListEntitiesPaginator = client.get_paginator("list_entities")
+```
+
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_marketplace_catalog.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.literals import (
     ChangeStatusType,
     FailureCodeType,
+    ListChangeSetsPaginatorName,
+    ListEntitiesPaginatorName,
+    OwnershipTypeType,
     SortOrderType,
     MarketplaceCatalogServiceName,
     ServiceName,
     ResourceServiceName,
+    PaginatorName,
     RegionName,
 )
 
 
 def check_value(value: ChangeStatusType) -> bool:
     ...
 ```
@@ -300,36 +327,43 @@
 
 `mypy_boto3_marketplace_catalog.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelChangeSetResponseTypeDef,
     ChangeSetSummaryListItemTypeDef,
     EntityTypeDef,
     ErrorDetailTypeDef,
     TagTypeDef,
+    DeleteResourcePolicyRequestRequestTypeDef,
     DescribeChangeSetRequestRequestTypeDef,
     DescribeEntityRequestRequestTypeDef,
+    DescribeEntityResponseTypeDef,
     EntitySummaryTypeDef,
     FilterTypeDef,
+    GetResourcePolicyRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
     SortTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CancelChangeSetResponseTypeDef,
-    DescribeEntityResponseTypeDef,
+    PaginatorConfigTypeDef,
+    PutResourcePolicyRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     StartChangeSetResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
     ListChangeSetsResponseTypeDef,
     ChangeSummaryTypeDef,
     ChangeTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEntitiesResponseTypeDef,
+    ListChangeSetsRequestListChangeSetsPaginateTypeDef,
     ListChangeSetsRequestRequestTypeDef,
+    ListEntitiesRequestListEntitiesPaginateTypeDef,
     ListEntitiesRequestRequestTypeDef,
     DescribeChangeSetResponseTypeDef,
     StartChangeSetRequestRequestTypeDef,
 )
 
 
 def get_structure() -> CancelChangeSetRequestRequestTypeDef:
@@ -339,42 +373,42 @@
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

### Comparing `mypy-boto3-marketplace-catalog-1.26.8/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt` & `mypy-boto3-marketplace-catalog-1.27.0/mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 mypy_boto3_marketplace_catalog/__init__.py
 mypy_boto3_marketplace_catalog/__init__.pyi
 mypy_boto3_marketplace_catalog/__main__.py
 mypy_boto3_marketplace_catalog/client.py
 mypy_boto3_marketplace_catalog/client.pyi
 mypy_boto3_marketplace_catalog/literals.py
 mypy_boto3_marketplace_catalog/literals.pyi
+mypy_boto3_marketplace_catalog/paginator.py
+mypy_boto3_marketplace_catalog/paginator.pyi
 mypy_boto3_marketplace_catalog/py.typed
 mypy_boto3_marketplace_catalog/type_defs.py
 mypy_boto3_marketplace_catalog/type_defs.pyi
 mypy_boto3_marketplace_catalog/version.py
 mypy_boto3_marketplace_catalog.egg-info/PKG-INFO
 mypy_boto3_marketplace_catalog.egg-info/SOURCES.txt
 mypy_boto3_marketplace_catalog.egg-info/dependency_links.txt
```

### Comparing `mypy-boto3-marketplace-catalog-1.26.8/setup.py` & `mypy-boto3-marketplace-catalog-1.27.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 """
 Setup script for mypy-boto3-marketplace-catalog.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-marketplace-catalog",
-    version="1.26.8",
+    version="1.27.0",
     packages=["mypy_boto3_marketplace_catalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MarketplaceCatalog 1.26.8 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.MarketplaceCatalog 1.27.0 service generated with"
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
     keywords="boto3 marketplace-catalog type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_marketplace_catalog": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_marketplace_catalog": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_marketplace_catalog/"
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


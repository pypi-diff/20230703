# Comparing `tmp/mypy-boto3-route53-recovery-cluster-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-route53-recovery-cluster-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53-recovery-cluster-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:55 2022, max compression
+gzip compressed data, was "mypy-boto3-route53-recovery-cluster-1.27.0.tar", last modified: Mon Jul  3 19:51:21 2023, max compression
```

## Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1.tar` & `mypy-boto3-route53-recovery-cluster-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:55.436845 mypy-boto3-route53-recovery-cluster-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13926 2022-11-01 21:43:55.436845 mypy-boto3-route53-recovery-cluster-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12419 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:55.436845 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7178 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     7166 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7206 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7204 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2117 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4481 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4477 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:55.436845 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13926 2022-11-01 21:43:55.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-11-01 21:43:55.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:55.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:55.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:55.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-01 21:43:55.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:55.436845 mypy-boto3-route53-recovery-cluster-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2022-11-01 21:40:12.000000 mypy-boto3-route53-recovery-cluster-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:21.675903 mypy-boto3-route53-recovery-cluster-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:31.000000 mypy-boto3-route53-recovery-cluster-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-07-03 19:51:21.675903 mypy-boto3-route53-recovery-cluster-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-07-03 19:46:31.000000 mypy-boto3-route53-recovery-cluster-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:21.675903 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-03 19:46:31.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-03 19:46:31.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-03 19:46:31.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-07-03 19:46:31.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-07-03 19:46:31.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-03 19:46:31.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:31.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-03 19:46:32.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:31.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:21.675903 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-03 19:51:21.000000 mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:21.675903 mypy-boto3-route53-recovery-cluster-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-03 19:46:31.000000 mypy-boto3-route53-recovery-cluster-1.27.0/setup.py
```

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/LICENSE` & `mypy-boto3-route53-recovery-cluster-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/PKG-INFO` & `mypy-boto3-route53-recovery-cluster-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-cluster
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Route53RecoveryCluster 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Route53RecoveryCluster 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/
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
 
 <a id="mypy-boto3-route53-recovery-cluster"></a>
 
 # mypy-boto3-route53-recovery-cluster
 
 [![PyPI - mypy-boto3-route53-recovery-cluster](https://img.shields.io/pypi/v/mypy-boto3-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-cluster)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-cluster)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53-recovery-cluster?color=blue)](https://pypistats.org/packages/mypy-boto3-route53-recovery-cluster)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryCluster 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
+[boto3.Route53RecoveryCluster 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
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
 [mypy-boto3-route53-recovery-cluster docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,22 +323,22 @@
 
 `mypy_boto3_route53_recovery_cluster.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53_recovery_cluster.type_defs import (
     GetRoutingControlStateRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
+    GetRoutingControlStateResponseTypeDef,
+    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
     RoutingControlTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UpdateRoutingControlStateEntryTypeDef,
     UpdateRoutingControlStateRequestRequestTypeDef,
-    GetRoutingControlStateResponseTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsResponseTypeDef,
     UpdateRoutingControlStatesRequestRequestTypeDef,
 )
 
 
 def get_structure() -> GetRoutingControlStateRequestRequestTypeDef:
     return {...}
@@ -346,42 +347,42 @@
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

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/README.md` & `mypy-boto3-route53-recovery-cluster-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-route53-recovery-cluster"></a>
 
 # mypy-boto3-route53-recovery-cluster
 
 [![PyPI - mypy-boto3-route53-recovery-cluster](https://img.shields.io/pypi/v/mypy-boto3-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-cluster)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-cluster)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53-recovery-cluster?color=blue)](https://pypistats.org/packages/mypy-boto3-route53-recovery-cluster)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryCluster 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
+[boto3.Route53RecoveryCluster 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
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
 [mypy-boto3-route53-recovery-cluster docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,22 +291,22 @@
 
 `mypy_boto3_route53_recovery_cluster.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53_recovery_cluster.type_defs import (
     GetRoutingControlStateRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
+    GetRoutingControlStateResponseTypeDef,
+    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
     RoutingControlTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UpdateRoutingControlStateEntryTypeDef,
     UpdateRoutingControlStateRequestRequestTypeDef,
-    GetRoutingControlStateResponseTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsResponseTypeDef,
     UpdateRoutingControlStatesRequestRequestTypeDef,
 )
 
 
 def get_structure() -> GetRoutingControlStateRequestRequestTypeDef:
     return {...}
@@ -315,42 +315,42 @@
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

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/__init__.py` & `mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/__init__.pyi` & `mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/__main__.py` & `mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53RecoveryCluster 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.Route53RecoveryCluster 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster\nOther"
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

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/client.py` & `mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/client.pyi` & `mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/literals.py` & `mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,23 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListRoutingControlsPaginatorName",
     "RoutingControlStateType",
     "Route53RecoveryClusterServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ListRoutingControlsPaginatorName = Literal["list_routing_controls"]
 RoutingControlStateType = Literal["Off", "On"]
 Route53RecoveryClusterServiceName = Literal["route53-recovery-cluster"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -43,23 +41,25 @@
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
@@ -69,30 +69,35 @@
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
@@ -118,14 +123,15 @@
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
@@ -170,51 +176,57 @@
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
@@ -227,14 +239,15 @@
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
@@ -246,28 +259,35 @@
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
@@ -276,14 +296,15 @@
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
@@ -294,55 +315,64 @@
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

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/literals.pyi` & `mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListRoutingControlsPaginatorName",
     "RoutingControlStateType",
     "Route53RecoveryClusterServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 ListRoutingControlsPaginatorName = Literal["list_routing_controls"]
 RoutingControlStateType = Literal["Off", "On"]
 Route53RecoveryClusterServiceName = Literal["route53-recovery-cluster"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -41,23 +43,25 @@
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
@@ -67,30 +71,35 @@
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
@@ -116,14 +125,15 @@
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
@@ -168,51 +178,57 @@
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
@@ -225,14 +241,15 @@
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
@@ -244,28 +261,35 @@
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
@@ -274,14 +298,15 @@
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
@@ -292,55 +317,64 @@
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

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/paginator.py` & `mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListRoutingControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Paginator.ListRoutingControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/paginators/#listroutingcontrolspaginator)
     """
 
     def paginate(
-        self, *, ControlPanelArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ControlPanelArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRoutingControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Paginator.ListRoutingControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/paginators/#listroutingcontrolspaginator)
         """
```

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/paginator.pyi` & `mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListRoutingControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Paginator.ListRoutingControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/paginators/#listroutingcontrolspaginator)
     """
 
     def paginate(
-        self, *, ControlPanelArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ControlPanelArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRoutingControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Paginator.ListRoutingControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/paginators/#listroutingcontrolspaginator)
         """
```

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/type_defs.py` & `mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,50 +20,48 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "GetRoutingControlStateRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetRoutingControlStateResponseTypeDef",
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     "ListRoutingControlsRequestRequestTypeDef",
     "RoutingControlTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateRoutingControlStateEntryTypeDef",
     "UpdateRoutingControlStateRequestRequestTypeDef",
-    "GetRoutingControlStateResponseTypeDef",
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     "ListRoutingControlsResponseTypeDef",
     "UpdateRoutingControlStatesRequestRequestTypeDef",
 )
 
 GetRoutingControlStateRequestRequestTypeDef = TypedDict(
     "GetRoutingControlStateRequestRequestTypeDef",
     {
         "RoutingControlArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+GetRoutingControlStateResponseTypeDef = TypedDict(
+    "GetRoutingControlStateResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "RoutingControlArn": str,
+        "RoutingControlState": RoutingControlStateType,
+        "RoutingControlName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ControlPanelArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListRoutingControlsRequestRequestTypeDef = TypedDict(
     "ListRoutingControlsRequestRequestTypeDef",
     {
@@ -82,14 +80,35 @@
         "RoutingControlArn": str,
         "RoutingControlName": str,
         "RoutingControlState": RoutingControlStateType,
     },
     total=False,
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
 UpdateRoutingControlStateEntryTypeDef = TypedDict(
     "UpdateRoutingControlStateEntryTypeDef",
     {
         "RoutingControlArn": str,
         "RoutingControlState": RoutingControlStateType,
     },
 )
@@ -113,39 +132,20 @@
 class UpdateRoutingControlStateRequestRequestTypeDef(
     _RequiredUpdateRoutingControlStateRequestRequestTypeDef,
     _OptionalUpdateRoutingControlStateRequestRequestTypeDef,
 ):
     pass
 
 
-GetRoutingControlStateResponseTypeDef = TypedDict(
-    "GetRoutingControlStateResponseTypeDef",
-    {
-        "RoutingControlArn": str,
-        "RoutingControlState": RoutingControlStateType,
-        "RoutingControlName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
-    {
-        "ControlPanelArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListRoutingControlsResponseTypeDef = TypedDict(
     "ListRoutingControlsResponseTypeDef",
     {
         "RoutingControls": List[RoutingControlTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateRoutingControlStatesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRoutingControlStatesRequestRequestTypeDef",
     {
         "UpdateRoutingControlStateEntries": Sequence[UpdateRoutingControlStateEntryTypeDef],
```

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster/type_defs.pyi` & `mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -19,50 +19,48 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "GetRoutingControlStateRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetRoutingControlStateResponseTypeDef",
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     "ListRoutingControlsRequestRequestTypeDef",
     "RoutingControlTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateRoutingControlStateEntryTypeDef",
     "UpdateRoutingControlStateRequestRequestTypeDef",
-    "GetRoutingControlStateResponseTypeDef",
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     "ListRoutingControlsResponseTypeDef",
     "UpdateRoutingControlStatesRequestRequestTypeDef",
 )
 
 GetRoutingControlStateRequestRequestTypeDef = TypedDict(
     "GetRoutingControlStateRequestRequestTypeDef",
     {
         "RoutingControlArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+GetRoutingControlStateResponseTypeDef = TypedDict(
+    "GetRoutingControlStateResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "RoutingControlArn": str,
+        "RoutingControlState": RoutingControlStateType,
+        "RoutingControlName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ControlPanelArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListRoutingControlsRequestRequestTypeDef = TypedDict(
     "ListRoutingControlsRequestRequestTypeDef",
     {
@@ -81,14 +79,35 @@
         "RoutingControlArn": str,
         "RoutingControlName": str,
         "RoutingControlState": RoutingControlStateType,
     },
     total=False,
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
 UpdateRoutingControlStateEntryTypeDef = TypedDict(
     "UpdateRoutingControlStateEntryTypeDef",
     {
         "RoutingControlArn": str,
         "RoutingControlState": RoutingControlStateType,
     },
 )
@@ -110,39 +129,20 @@
 
 class UpdateRoutingControlStateRequestRequestTypeDef(
     _RequiredUpdateRoutingControlStateRequestRequestTypeDef,
     _OptionalUpdateRoutingControlStateRequestRequestTypeDef,
 ):
     pass
 
-GetRoutingControlStateResponseTypeDef = TypedDict(
-    "GetRoutingControlStateResponseTypeDef",
-    {
-        "RoutingControlArn": str,
-        "RoutingControlState": RoutingControlStateType,
-        "RoutingControlName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
-    {
-        "ControlPanelArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListRoutingControlsResponseTypeDef = TypedDict(
     "ListRoutingControlsResponseTypeDef",
     {
         "RoutingControls": List[RoutingControlTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateRoutingControlStatesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRoutingControlStatesRequestRequestTypeDef",
     {
         "UpdateRoutingControlStateEntries": Sequence[UpdateRoutingControlStateEntryTypeDef],
```

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster.egg-info/PKG-INFO` & `mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-cluster
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Route53RecoveryCluster 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Route53RecoveryCluster 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/
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
 
 <a id="mypy-boto3-route53-recovery-cluster"></a>
 
 # mypy-boto3-route53-recovery-cluster
 
 [![PyPI - mypy-boto3-route53-recovery-cluster](https://img.shields.io/pypi/v/mypy-boto3-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-cluster)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-cluster)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53-recovery-cluster?color=blue)](https://pypistats.org/packages/mypy-boto3-route53-recovery-cluster)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryCluster 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
+[boto3.Route53RecoveryCluster 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
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
 [mypy-boto3-route53-recovery-cluster docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,22 +323,22 @@
 
 `mypy_boto3_route53_recovery_cluster.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53_recovery_cluster.type_defs import (
     GetRoutingControlStateRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
+    GetRoutingControlStateResponseTypeDef,
+    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
     RoutingControlTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     UpdateRoutingControlStateEntryTypeDef,
     UpdateRoutingControlStateRequestRequestTypeDef,
-    GetRoutingControlStateResponseTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsResponseTypeDef,
     UpdateRoutingControlStatesRequestRequestTypeDef,
 )
 
 
 def get_structure() -> GetRoutingControlStateRequestRequestTypeDef:
     return {...}
@@ -346,42 +347,42 @@
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

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/mypy_boto3_route53_recovery_cluster.egg-info/SOURCES.txt` & `mypy-boto3-route53-recovery-cluster-1.27.0/mypy_boto3_route53_recovery_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-cluster-1.26.0.post1/setup.py` & `mypy-boto3-route53-recovery-cluster-1.27.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 """
 Setup script for mypy-boto3-route53-recovery-cluster.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53-recovery-cluster",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_route53_recovery_cluster"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53RecoveryCluster 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.Route53RecoveryCluster 1.27.0 service generated with"
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
     keywords=(
         "boto3 route53-recovery-cluster type-annotations boto3-stubs mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_route53_recovery_cluster": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_route53_recovery_cluster": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_cluster/"
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


# Comparing `tmp/mypy-boto3-dax-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-dax-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dax-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:19 2022, max compression
+gzip compressed data, was "mypy-boto3-dax-1.27.0.tar", last modified: Mon Jul  3 19:50:38 2023, max compression
```

## Comparing `mypy-boto3-dax-1.26.0.post1.tar` & `mypy-boto3-dax-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:19.948823 mypy-boto3-dax-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:32:42.000000 mypy-boto3-dax-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16081 2022-11-01 21:43:19.948823 mypy-boto3-dax-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14656 2022-11-01 21:32:42.000000 mypy-boto3-dax-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:19.944823 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/
--rw-r--r--   0 runner    (1001) docker     (121)     1872 2022-11-01 21:32:42.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-11-01 21:32:42.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-11-01 21:32:42.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20424 2022-11-01 21:32:42.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    20389 2022-11-01 21:32:42.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8559 2022-11-01 21:32:42.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8557 2022-11-01 21:32:42.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8586 2022-11-01 21:32:42.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     8577 2022-11-01 21:32:42.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:32:42.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    22331 2022-11-01 21:32:43.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    22308 2022-11-01 21:32:42.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:32:42.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:19.948823 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16081 2022-11-01 21:43:19.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-11-01 21:43:19.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:19.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:19.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:19.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-01 21:43:19.000000 mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:19.952823 mypy-boto3-dax-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-11-01 21:32:41.000000 mypy-boto3-dax-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.547107 mypy-boto3-dax-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:23.000000 mypy-boto3-dax-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16099 2023-07-03 19:50:38.547107 mypy-boto3-dax-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14630 2023-07-03 19:35:23.000000 mypy-boto3-dax-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.547107 mypy-boto3-dax-1.27.0/mypy_boto3_dax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-03 19:35:23.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-03 19:35:23.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:35:23.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-07-03 19:35:23.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20389 2023-07-03 19:35:23.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-07-03 19:35:23.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-03 19:35:23.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-03 19:35:23.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-07-03 19:35:23.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:23.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22387 2023-07-03 19:35:25.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-07-03 19:35:24.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:23.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.547107 mypy-boto3-dax-1.27.0/mypy_boto3_dax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16099 2023-07-03 19:50:38.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:50:38.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:38.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:38.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:38.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:38.000000 mypy-boto3-dax-1.27.0/mypy_boto3_dax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:38.547107 mypy-boto3-dax-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:35:23.000000 mypy-boto3-dax-1.27.0/setup.py
```

### Comparing `mypy-boto3-dax-1.26.0.post1/LICENSE` & `mypy-boto3-dax-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-dax-1.26.0.post1/PKG-INFO` & `mypy-boto3-dax-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dax
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.DAX 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.DAX 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/
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
 
 <a id="mypy-boto3-dax"></a>
 
 # mypy-boto3-dax
 
 [![PyPI - mypy-boto3-dax](https://img.shields.io/pypi/v/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dax?color=blue)](https://pypistats.org/packages/mypy-boto3-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DAX 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[boto3.DAX 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
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
 [mypy-boto3-dax docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,57 +358,57 @@
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     ParameterGroupStatusTypeDef,
     SSEDescriptionTypeDef,
     SecurityGroupMembershipTypeDef,
     SSESpecificationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     CreateParameterGroupRequestRequestTypeDef,
     ParameterGroupTypeDef,
     CreateSubnetGroupRequestRequestTypeDef,
     DecreaseReplicationFactorRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteParameterGroupRequestRequestTypeDef,
+    DeleteParameterGroupResponseTypeDef,
     DeleteSubnetGroupRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DeleteSubnetGroupResponseTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeClustersRequestRequestTypeDef,
+    DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
     DescribeDefaultParametersRequestRequestTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     EventTypeDef,
+    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
+    DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
+    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     IncreaseReplicationFactorRequestRequestTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
     NodeTypeSpecificValueTypeDef,
+    PaginatorConfigTypeDef,
     ParameterNameValueTypeDef,
     RebootNodeRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SubnetTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateSubnetGroupRequestRequestTypeDef,
     NodeTypeDef,
     CreateClusterRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    DeleteParameterGroupResponseTypeDef,
-    DeleteSubnetGroupResponseTypeDef,
     ListTagsResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     TagResourceResponseTypeDef,
     UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
-    DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
-    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
-    DescribeParametersRequestDescribeParametersPaginateTypeDef,
-    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     DescribeEventsResponseTypeDef,
     ParameterTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     SubnetGroupTypeDef,
     ClusterTypeDef,
     DescribeDefaultParametersResponseTypeDef,
     DescribeParametersResponseTypeDef,
@@ -431,42 +432,42 @@
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

### Comparing `mypy-boto3-dax-1.26.0.post1/README.md` & `mypy-boto3-dax-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-dax"></a>
 
 # mypy-boto3-dax
 
 [![PyPI - mypy-boto3-dax](https://img.shields.io/pypi/v/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dax?color=blue)](https://pypistats.org/packages/mypy-boto3-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DAX 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[boto3.DAX 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
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
 [mypy-boto3-dax docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,57 +326,57 @@
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     ParameterGroupStatusTypeDef,
     SSEDescriptionTypeDef,
     SecurityGroupMembershipTypeDef,
     SSESpecificationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     CreateParameterGroupRequestRequestTypeDef,
     ParameterGroupTypeDef,
     CreateSubnetGroupRequestRequestTypeDef,
     DecreaseReplicationFactorRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteParameterGroupRequestRequestTypeDef,
+    DeleteParameterGroupResponseTypeDef,
     DeleteSubnetGroupRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DeleteSubnetGroupResponseTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeClustersRequestRequestTypeDef,
+    DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
     DescribeDefaultParametersRequestRequestTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     EventTypeDef,
+    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
+    DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
+    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     IncreaseReplicationFactorRequestRequestTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
     NodeTypeSpecificValueTypeDef,
+    PaginatorConfigTypeDef,
     ParameterNameValueTypeDef,
     RebootNodeRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SubnetTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateSubnetGroupRequestRequestTypeDef,
     NodeTypeDef,
     CreateClusterRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    DeleteParameterGroupResponseTypeDef,
-    DeleteSubnetGroupResponseTypeDef,
     ListTagsResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     TagResourceResponseTypeDef,
     UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
-    DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
-    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
-    DescribeParametersRequestDescribeParametersPaginateTypeDef,
-    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     DescribeEventsResponseTypeDef,
     ParameterTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     SubnetGroupTypeDef,
     ClusterTypeDef,
     DescribeDefaultParametersResponseTypeDef,
     DescribeParametersResponseTypeDef,
@@ -400,42 +400,42 @@
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

### Comparing `mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/__init__.py` & `mypy-boto3-dax-1.27.0/mypy_boto3_dax/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/__init__.pyi` & `mypy-boto3-dax-1.27.0/mypy_boto3_dax/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/__main__.py` & `mypy-boto3-dax-1.27.0/mypy_boto3_dax/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DAX 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.DAX 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX\nOther"
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

### Comparing `mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/client.py` & `mypy-boto3-dax-1.27.0/mypy_boto3_dax/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/client.pyi` & `mypy-boto3-dax-1.27.0/mypy_boto3_dax/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/literals.py` & `mypy-boto3-dax-1.27.0/mypy_boto3_dax/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,23 +66,25 @@
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
@@ -92,30 +94,35 @@
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
@@ -141,14 +148,15 @@
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
@@ -193,51 +201,57 @@
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
@@ -250,14 +264,15 @@
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
@@ -269,28 +284,35 @@
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
@@ -299,14 +321,15 @@
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
@@ -317,55 +340,64 @@
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

### Comparing `mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/literals.pyi` & `mypy-boto3-dax-1.27.0/mypy_boto3_dax/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -64,23 +64,25 @@
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
@@ -90,30 +92,35 @@
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
@@ -139,14 +146,15 @@
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
@@ -191,51 +199,57 @@
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
@@ -248,14 +262,15 @@
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
@@ -267,28 +282,35 @@
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
@@ -297,14 +319,15 @@
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
@@ -315,55 +338,64 @@
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

### Comparing `mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/paginator.py` & `mypy-boto3-dax-1.27.0/mypy_boto3_dax/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,30 +72,30 @@
 class DescribeClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeclusterspaginator)
     """
 
     def paginate(
-        self, *, ClusterNames: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterNames: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeclusterspaginator)
         """
 
 
 class DescribeDefaultParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeDefaultParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describedefaultparameterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDefaultParametersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeDefaultParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describedefaultparameterspaginator)
         """
 
 
@@ -109,15 +109,15 @@
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeeventspaginator)
         """
 
 
@@ -127,15 +127,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeparametergroupspaginator)
     """
 
     def paginate(
         self,
         *,
         ParameterGroupNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeParameterGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeparametergroupspaginator)
         """
 
 
@@ -146,15 +146,15 @@
     """
 
     def paginate(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeParametersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeparameterspaginator)
         """
 
 
@@ -164,28 +164,28 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describesubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         SubnetGroupNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describesubnetgroupspaginator)
         """
 
 
 class ListTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.ListTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#listtagspaginator)
     """
 
     def paginate(
-        self, *, ResourceName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.ListTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#listtagspaginator)
         """
```

### Comparing `mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/paginator.pyi` & `mypy-boto3-dax-1.27.0/mypy_boto3_dax/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -69,29 +69,29 @@
 class DescribeClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeclusterspaginator)
     """
 
     def paginate(
-        self, *, ClusterNames: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ClusterNames: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeclusterspaginator)
         """
 
 class DescribeDefaultParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeDefaultParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describedefaultparameterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDefaultParametersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeDefaultParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describedefaultparameterspaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
@@ -104,15 +104,15 @@
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeeventspaginator)
         """
 
 class DescribeParameterGroupsPaginator(Paginator):
@@ -121,15 +121,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeparametergroupspaginator)
     """
 
     def paginate(
         self,
         *,
         ParameterGroupNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeParameterGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeparametergroupspaginator)
         """
 
 class DescribeParametersPaginator(Paginator):
@@ -139,15 +139,15 @@
     """
 
     def paginate(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeParametersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeparameterspaginator)
         """
 
 class DescribeSubnetGroupsPaginator(Paginator):
@@ -156,27 +156,27 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describesubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         SubnetGroupNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describesubnetgroupspaginator)
         """
 
 class ListTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.ListTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#listtagspaginator)
     """
 
     def paginate(
-        self, *, ResourceName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.ListTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#listtagspaginator)
         """
```

### Comparing `mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/type_defs.py` & `mypy-boto3-dax-1.27.0/mypy_boto3_dax/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -25,66 +25,65 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "EndpointTypeDef",
     "NotificationConfigurationTypeDef",
     "ParameterGroupStatusTypeDef",
     "SSEDescriptionTypeDef",
     "SecurityGroupMembershipTypeDef",
     "SSESpecificationTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateParameterGroupRequestRequestTypeDef",
     "ParameterGroupTypeDef",
     "CreateSubnetGroupRequestRequestTypeDef",
     "DecreaseReplicationFactorRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteParameterGroupRequestRequestTypeDef",
+    "DeleteParameterGroupResponseTypeDef",
     "DeleteSubnetGroupRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DeleteSubnetGroupResponseTypeDef",
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
     "DescribeClustersRequestRequestTypeDef",
+    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
     "DescribeDefaultParametersRequestRequestTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "EventTypeDef",
+    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     "DescribeParameterGroupsRequestRequestTypeDef",
+    "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeParametersRequestRequestTypeDef",
+    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "DescribeSubnetGroupsRequestRequestTypeDef",
     "IncreaseReplicationFactorRequestRequestTypeDef",
+    "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
     "NodeTypeSpecificValueTypeDef",
+    "PaginatorConfigTypeDef",
     "ParameterNameValueTypeDef",
     "RebootNodeRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SubnetTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "UpdateSubnetGroupRequestRequestTypeDef",
     "NodeTypeDef",
     "CreateClusterRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "DeleteParameterGroupResponseTypeDef",
-    "DeleteSubnetGroupResponseTypeDef",
     "ListTagsResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "TagResourceResponseTypeDef",
     "UntagResourceResponseTypeDef",
     "CreateParameterGroupResponseTypeDef",
     "DescribeParameterGroupsResponseTypeDef",
     "UpdateParameterGroupResponseTypeDef",
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
-    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
-    "DescribeParametersRequestDescribeParametersPaginateTypeDef",
-    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
-    "ListTagsRequestListTagsPaginateTypeDef",
     "DescribeEventsResponseTypeDef",
     "ParameterTypeDef",
     "UpdateParameterGroupRequestRequestTypeDef",
     "SubnetGroupTypeDef",
     "ClusterTypeDef",
     "DescribeDefaultParametersResponseTypeDef",
     "DescribeParametersResponseTypeDef",
@@ -158,47 +157,34 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredCreateParameterGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateParameterGroupRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalCreateParameterGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateParameterGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateParameterGroupRequestRequestTypeDef(
     _RequiredCreateParameterGroupRequestRequestTypeDef,
     _OptionalCreateParameterGroupRequestRequestTypeDef,
 ):
     pass
 
-
 ParameterGroupTypeDef = TypedDict(
     "ParameterGroupTypeDef",
     {
         "ParameterGroupName": str,
         "Description": str,
     },
     total=False,
@@ -215,21 +201,19 @@
     "_OptionalCreateSubnetGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateSubnetGroupRequestRequestTypeDef(
     _RequiredCreateSubnetGroupRequestRequestTypeDef, _OptionalCreateSubnetGroupRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDecreaseReplicationFactorRequestRequestTypeDef = TypedDict(
     "_RequiredDecreaseReplicationFactorRequestRequestTypeDef",
     {
         "ClusterName": str,
         "NewReplicationFactor": int,
     },
 )
@@ -238,72 +222,106 @@
     {
         "AvailabilityZones": Sequence[str],
         "NodeIdsToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class DecreaseReplicationFactorRequestRequestTypeDef(
     _RequiredDecreaseReplicationFactorRequestRequestTypeDef,
     _OptionalDecreaseReplicationFactorRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteClusterRequestRequestTypeDef = TypedDict(
     "DeleteClusterRequestRequestTypeDef",
     {
         "ClusterName": str,
     },
 )
 
 DeleteParameterGroupRequestRequestTypeDef = TypedDict(
     "DeleteParameterGroupRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 
+DeleteParameterGroupResponseTypeDef = TypedDict(
+    "DeleteParameterGroupResponseTypeDef",
+    {
+        "DeletionMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSubnetGroupRequestRequestTypeDef = TypedDict(
     "DeleteSubnetGroupRequestRequestTypeDef",
     {
         "SubnetGroupName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DeleteSubnetGroupResponseTypeDef = TypedDict(
+    "DeleteSubnetGroupResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DeletionMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    {
+        "ClusterNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeClustersRequestRequestTypeDef = TypedDict(
     "DescribeClustersRequestRequestTypeDef",
     {
         "ClusterNames": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef = TypedDict(
+    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeDefaultParametersRequestRequestTypeDef = TypedDict(
     "DescribeDefaultParametersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "SourceName": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventsRequestRequestTypeDef = TypedDict(
     "DescribeEventsRequestRequestTypeDef",
     {
         "SourceName": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -321,24 +339,54 @@
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
     },
     total=False,
 )
 
+DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
+    {
+        "ParameterGroupNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeParameterGroupsRequestRequestTypeDef = TypedDict(
     "DescribeParameterGroupsRequestRequestTypeDef",
     {
         "ParameterGroupNames": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+    },
+)
+_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeParametersRequestDescribeParametersPaginateTypeDef(
+    _RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef,
+    _OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeParametersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeParametersRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalDescribeParametersRequestRequestTypeDef = TypedDict(
@@ -347,21 +395,28 @@
         "Source": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeParametersRequestRequestTypeDef(
     _RequiredDescribeParametersRequestRequestTypeDef,
     _OptionalDescribeParametersRequestRequestTypeDef,
 ):
     pass
 
+DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
+    {
+        "SubnetGroupNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 DescribeSubnetGroupsRequestRequestTypeDef = TypedDict(
     "DescribeSubnetGroupsRequestRequestTypeDef",
     {
         "SubnetGroupNames": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
@@ -380,21 +435,38 @@
     "_OptionalIncreaseReplicationFactorRequestRequestTypeDef",
     {
         "AvailabilityZones": Sequence[str],
     },
     total=False,
 )
 
-
 class IncreaseReplicationFactorRequestRequestTypeDef(
     _RequiredIncreaseReplicationFactorRequestRequestTypeDef,
     _OptionalIncreaseReplicationFactorRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_RequiredListTagsRequestListTagsPaginateTypeDef",
+    {
+        "ResourceName": str,
+    },
+)
+_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_OptionalListTagsRequestListTagsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTagsRequestListTagsPaginateTypeDef(
+    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
+):
+    pass
 
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceName": str,
     },
 )
@@ -402,30 +474,38 @@
     "_OptionalListTagsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
-
 NodeTypeSpecificValueTypeDef = TypedDict(
     "NodeTypeSpecificValueTypeDef",
     {
         "NodeType": str,
         "Value": str,
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
 ParameterNameValueTypeDef = TypedDict(
     "ParameterNameValueTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
     total=False,
@@ -435,14 +515,25 @@
     "RebootNodeRequestRequestTypeDef",
     {
         "ClusterName": str,
         "NodeId": str,
     },
 )
 
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
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": str,
     },
     total=False,
@@ -471,21 +562,19 @@
         "NotificationTopicStatus": str,
         "ParameterGroupName": str,
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateSubnetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubnetGroupRequestRequestTypeDef",
     {
         "SubnetGroupName": str,
     },
 )
 _OptionalUpdateSubnetGroupRequestRequestTypeDef = TypedDict(
@@ -493,21 +582,19 @@
     {
         "Description": str,
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateSubnetGroupRequestRequestTypeDef(
     _RequiredUpdateSubnetGroupRequestRequestTypeDef, _OptionalUpdateSubnetGroupRequestRequestTypeDef
 ):
     pass
 
-
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "NodeId": str,
         "Endpoint": EndpointTypeDef,
         "NodeCreateTime": datetime,
         "AvailabilityZone": str,
@@ -539,193 +626,83 @@
         "Tags": Sequence[TagTypeDef],
         "SSESpecification": SSESpecificationTypeDef,
         "ClusterEndpointEncryptionType": ClusterEndpointEncryptionTypeType,
     },
     total=False,
 )
 
-
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceName": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-DeleteParameterGroupResponseTypeDef = TypedDict(
-    "DeleteParameterGroupResponseTypeDef",
-    {
-        "DeletionMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSubnetGroupResponseTypeDef = TypedDict(
-    "DeleteSubnetGroupResponseTypeDef",
-    {
-        "DeletionMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 TagResourceResponseTypeDef = TypedDict(
     "TagResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UntagResourceResponseTypeDef = TypedDict(
     "UntagResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateParameterGroupResponseTypeDef = TypedDict(
     "CreateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeParameterGroupsResponseTypeDef = TypedDict(
     "DescribeParameterGroupsResponseTypeDef",
     {
         "NextToken": str,
         "ParameterGroups": List[ParameterGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateParameterGroupResponseTypeDef = TypedDict(
     "UpdateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
-    {
-        "ClusterNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef = TypedDict(
-    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "SourceName": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
-    {
-        "ParameterGroupNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-    },
-)
-_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeParametersRequestDescribeParametersPaginateTypeDef(
-    _RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef,
-    _OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef,
-):
-    pass
-
-
-DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
-    {
-        "SubnetGroupNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_RequiredListTagsRequestListTagsPaginateTypeDef",
-    {
-        "ResourceName": str,
-    },
-)
-_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_OptionalListTagsRequestListTagsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTagsRequestListTagsPaginateTypeDef(
-    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
-):
-    pass
-
-
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "NextToken": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "ParameterName": str,
@@ -787,101 +764,101 @@
 )
 
 DescribeDefaultParametersResponseTypeDef = TypedDict(
     "DescribeDefaultParametersResponseTypeDef",
     {
         "NextToken": str,
         "Parameters": List[ParameterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeParametersResponseTypeDef = TypedDict(
     "DescribeParametersResponseTypeDef",
     {
         "NextToken": str,
         "Parameters": List[ParameterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSubnetGroupResponseTypeDef = TypedDict(
     "CreateSubnetGroupResponseTypeDef",
     {
         "SubnetGroup": SubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSubnetGroupsResponseTypeDef = TypedDict(
     "DescribeSubnetGroupsResponseTypeDef",
     {
         "NextToken": str,
         "SubnetGroups": List[SubnetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSubnetGroupResponseTypeDef = TypedDict(
     "UpdateSubnetGroupResponseTypeDef",
     {
         "SubnetGroup": SubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DecreaseReplicationFactorResponseTypeDef = TypedDict(
     "DecreaseReplicationFactorResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "NextToken": str,
         "Clusters": List[ClusterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IncreaseReplicationFactorResponseTypeDef = TypedDict(
     "IncreaseReplicationFactorResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootNodeResponseTypeDef = TypedDict(
     "RebootNodeResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterResponseTypeDef = TypedDict(
     "UpdateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax/type_defs.pyi` & `mypy-boto3-dax-1.27.0/mypy_boto3_dax/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,65 +25,66 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "EndpointTypeDef",
     "NotificationConfigurationTypeDef",
     "ParameterGroupStatusTypeDef",
     "SSEDescriptionTypeDef",
     "SecurityGroupMembershipTypeDef",
     "SSESpecificationTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateParameterGroupRequestRequestTypeDef",
     "ParameterGroupTypeDef",
     "CreateSubnetGroupRequestRequestTypeDef",
     "DecreaseReplicationFactorRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteParameterGroupRequestRequestTypeDef",
+    "DeleteParameterGroupResponseTypeDef",
     "DeleteSubnetGroupRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DeleteSubnetGroupResponseTypeDef",
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
     "DescribeClustersRequestRequestTypeDef",
+    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
     "DescribeDefaultParametersRequestRequestTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "EventTypeDef",
+    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     "DescribeParameterGroupsRequestRequestTypeDef",
+    "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeParametersRequestRequestTypeDef",
+    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "DescribeSubnetGroupsRequestRequestTypeDef",
     "IncreaseReplicationFactorRequestRequestTypeDef",
+    "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
     "NodeTypeSpecificValueTypeDef",
+    "PaginatorConfigTypeDef",
     "ParameterNameValueTypeDef",
     "RebootNodeRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SubnetTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "UpdateSubnetGroupRequestRequestTypeDef",
     "NodeTypeDef",
     "CreateClusterRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "DeleteParameterGroupResponseTypeDef",
-    "DeleteSubnetGroupResponseTypeDef",
     "ListTagsResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "TagResourceResponseTypeDef",
     "UntagResourceResponseTypeDef",
     "CreateParameterGroupResponseTypeDef",
     "DescribeParameterGroupsResponseTypeDef",
     "UpdateParameterGroupResponseTypeDef",
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
-    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
-    "DescribeParametersRequestDescribeParametersPaginateTypeDef",
-    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
-    "ListTagsRequestListTagsPaginateTypeDef",
     "DescribeEventsResponseTypeDef",
     "ParameterTypeDef",
     "UpdateParameterGroupRequestRequestTypeDef",
     "SubnetGroupTypeDef",
     "ClusterTypeDef",
     "DescribeDefaultParametersResponseTypeDef",
     "DescribeParametersResponseTypeDef",
@@ -157,45 +158,36 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredCreateParameterGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateParameterGroupRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalCreateParameterGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateParameterGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateParameterGroupRequestRequestTypeDef(
     _RequiredCreateParameterGroupRequestRequestTypeDef,
     _OptionalCreateParameterGroupRequestRequestTypeDef,
 ):
     pass
 
+
 ParameterGroupTypeDef = TypedDict(
     "ParameterGroupTypeDef",
     {
         "ParameterGroupName": str,
         "Description": str,
     },
     total=False,
@@ -212,19 +204,21 @@
     "_OptionalCreateSubnetGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateSubnetGroupRequestRequestTypeDef(
     _RequiredCreateSubnetGroupRequestRequestTypeDef, _OptionalCreateSubnetGroupRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDecreaseReplicationFactorRequestRequestTypeDef = TypedDict(
     "_RequiredDecreaseReplicationFactorRequestRequestTypeDef",
     {
         "ClusterName": str,
         "NewReplicationFactor": int,
     },
 )
@@ -233,70 +227,108 @@
     {
         "AvailabilityZones": Sequence[str],
         "NodeIdsToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class DecreaseReplicationFactorRequestRequestTypeDef(
     _RequiredDecreaseReplicationFactorRequestRequestTypeDef,
     _OptionalDecreaseReplicationFactorRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteClusterRequestRequestTypeDef = TypedDict(
     "DeleteClusterRequestRequestTypeDef",
     {
         "ClusterName": str,
     },
 )
 
 DeleteParameterGroupRequestRequestTypeDef = TypedDict(
     "DeleteParameterGroupRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 
+DeleteParameterGroupResponseTypeDef = TypedDict(
+    "DeleteParameterGroupResponseTypeDef",
+    {
+        "DeletionMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSubnetGroupRequestRequestTypeDef = TypedDict(
     "DeleteSubnetGroupRequestRequestTypeDef",
     {
         "SubnetGroupName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DeleteSubnetGroupResponseTypeDef = TypedDict(
+    "DeleteSubnetGroupResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DeletionMessage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    {
+        "ClusterNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeClustersRequestRequestTypeDef = TypedDict(
     "DescribeClustersRequestRequestTypeDef",
     {
         "ClusterNames": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef = TypedDict(
+    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeDefaultParametersRequestRequestTypeDef = TypedDict(
     "DescribeDefaultParametersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "SourceName": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventsRequestRequestTypeDef = TypedDict(
     "DescribeEventsRequestRequestTypeDef",
     {
         "SourceName": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -314,24 +346,56 @@
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
     },
     total=False,
 )
 
+DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
+    {
+        "ParameterGroupNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeParameterGroupsRequestRequestTypeDef = TypedDict(
     "DescribeParameterGroupsRequestRequestTypeDef",
     {
         "ParameterGroupNames": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+    },
+)
+_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeParametersRequestDescribeParametersPaginateTypeDef(
+    _RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef,
+    _OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeParametersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeParametersRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalDescribeParametersRequestRequestTypeDef = TypedDict(
@@ -340,20 +404,31 @@
         "Source": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeParametersRequestRequestTypeDef(
     _RequiredDescribeParametersRequestRequestTypeDef,
     _OptionalDescribeParametersRequestRequestTypeDef,
 ):
     pass
 
+
+DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
+    {
+        "SubnetGroupNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeSubnetGroupsRequestRequestTypeDef = TypedDict(
     "DescribeSubnetGroupsRequestRequestTypeDef",
     {
         "SubnetGroupNames": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -371,48 +446,83 @@
     "_OptionalIncreaseReplicationFactorRequestRequestTypeDef",
     {
         "AvailabilityZones": Sequence[str],
     },
     total=False,
 )
 
+
 class IncreaseReplicationFactorRequestRequestTypeDef(
     _RequiredIncreaseReplicationFactorRequestRequestTypeDef,
     _OptionalIncreaseReplicationFactorRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_RequiredListTagsRequestListTagsPaginateTypeDef",
+    {
+        "ResourceName": str,
+    },
+)
+_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_OptionalListTagsRequestListTagsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTagsRequestListTagsPaginateTypeDef(
+    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
+):
+    pass
+
+
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceName": str,
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
     "_OptionalListTagsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
+
 NodeTypeSpecificValueTypeDef = TypedDict(
     "NodeTypeSpecificValueTypeDef",
     {
         "NodeType": str,
         "Value": str,
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
 ParameterNameValueTypeDef = TypedDict(
     "ParameterNameValueTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
     total=False,
@@ -422,14 +532,25 @@
     "RebootNodeRequestRequestTypeDef",
     {
         "ClusterName": str,
         "NodeId": str,
     },
 )
 
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
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": str,
     },
     total=False,
@@ -458,19 +579,21 @@
         "NotificationTopicStatus": str,
         "ParameterGroupName": str,
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateSubnetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubnetGroupRequestRequestTypeDef",
     {
         "SubnetGroupName": str,
     },
 )
 _OptionalUpdateSubnetGroupRequestRequestTypeDef = TypedDict(
@@ -478,19 +601,21 @@
     {
         "Description": str,
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateSubnetGroupRequestRequestTypeDef(
     _RequiredUpdateSubnetGroupRequestRequestTypeDef, _OptionalUpdateSubnetGroupRequestRequestTypeDef
 ):
     pass
 
+
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "NodeId": str,
         "Endpoint": EndpointTypeDef,
         "NodeCreateTime": datetime,
         "AvailabilityZone": str,
@@ -522,187 +647,85 @@
         "Tags": Sequence[TagTypeDef],
         "SSESpecification": SSESpecificationTypeDef,
         "ClusterEndpointEncryptionType": ClusterEndpointEncryptionTypeType,
     },
     total=False,
 )
 
+
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceName": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-DeleteParameterGroupResponseTypeDef = TypedDict(
-    "DeleteParameterGroupResponseTypeDef",
-    {
-        "DeletionMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSubnetGroupResponseTypeDef = TypedDict(
-    "DeleteSubnetGroupResponseTypeDef",
-    {
-        "DeletionMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 ListTagsResponseTypeDef = TypedDict(
     "ListTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceName": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 TagResourceResponseTypeDef = TypedDict(
     "TagResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UntagResourceResponseTypeDef = TypedDict(
     "UntagResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateParameterGroupResponseTypeDef = TypedDict(
     "CreateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeParameterGroupsResponseTypeDef = TypedDict(
     "DescribeParameterGroupsResponseTypeDef",
     {
         "NextToken": str,
         "ParameterGroups": List[ParameterGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateParameterGroupResponseTypeDef = TypedDict(
     "UpdateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
-    {
-        "ClusterNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef = TypedDict(
-    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "SourceName": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
-    {
-        "ParameterGroupNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-    },
-)
-_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeParametersRequestDescribeParametersPaginateTypeDef(
-    _RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef,
-    _OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef,
-):
-    pass
-
-DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
-    {
-        "SubnetGroupNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_RequiredListTagsRequestListTagsPaginateTypeDef",
-    {
-        "ResourceName": str,
-    },
-)
-_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_OptionalListTagsRequestListTagsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTagsRequestListTagsPaginateTypeDef(
-    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
-):
-    pass
-
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "NextToken": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "ParameterName": str,
@@ -764,101 +787,101 @@
 )
 
 DescribeDefaultParametersResponseTypeDef = TypedDict(
     "DescribeDefaultParametersResponseTypeDef",
     {
         "NextToken": str,
         "Parameters": List[ParameterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeParametersResponseTypeDef = TypedDict(
     "DescribeParametersResponseTypeDef",
     {
         "NextToken": str,
         "Parameters": List[ParameterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSubnetGroupResponseTypeDef = TypedDict(
     "CreateSubnetGroupResponseTypeDef",
     {
         "SubnetGroup": SubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSubnetGroupsResponseTypeDef = TypedDict(
     "DescribeSubnetGroupsResponseTypeDef",
     {
         "NextToken": str,
         "SubnetGroups": List[SubnetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSubnetGroupResponseTypeDef = TypedDict(
     "UpdateSubnetGroupResponseTypeDef",
     {
         "SubnetGroup": SubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DecreaseReplicationFactorResponseTypeDef = TypedDict(
     "DecreaseReplicationFactorResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "NextToken": str,
         "Clusters": List[ClusterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IncreaseReplicationFactorResponseTypeDef = TypedDict(
     "IncreaseReplicationFactorResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootNodeResponseTypeDef = TypedDict(
     "RebootNodeResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterResponseTypeDef = TypedDict(
     "UpdateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax.egg-info/PKG-INFO` & `mypy-boto3-dax-1.27.0/mypy_boto3_dax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dax
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.DAX 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.DAX 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/
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
 
 <a id="mypy-boto3-dax"></a>
 
 # mypy-boto3-dax
 
 [![PyPI - mypy-boto3-dax](https://img.shields.io/pypi/v/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dax?color=blue)](https://pypistats.org/packages/mypy-boto3-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DAX 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[boto3.DAX 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
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
 [mypy-boto3-dax docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,57 +358,57 @@
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     ParameterGroupStatusTypeDef,
     SSEDescriptionTypeDef,
     SecurityGroupMembershipTypeDef,
     SSESpecificationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     CreateParameterGroupRequestRequestTypeDef,
     ParameterGroupTypeDef,
     CreateSubnetGroupRequestRequestTypeDef,
     DecreaseReplicationFactorRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteParameterGroupRequestRequestTypeDef,
+    DeleteParameterGroupResponseTypeDef,
     DeleteSubnetGroupRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DeleteSubnetGroupResponseTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeClustersRequestRequestTypeDef,
+    DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
     DescribeDefaultParametersRequestRequestTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     EventTypeDef,
+    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
+    DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
+    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     IncreaseReplicationFactorRequestRequestTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
     NodeTypeSpecificValueTypeDef,
+    PaginatorConfigTypeDef,
     ParameterNameValueTypeDef,
     RebootNodeRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SubnetTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateSubnetGroupRequestRequestTypeDef,
     NodeTypeDef,
     CreateClusterRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    DeleteParameterGroupResponseTypeDef,
-    DeleteSubnetGroupResponseTypeDef,
     ListTagsResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     TagResourceResponseTypeDef,
     UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
-    DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
-    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
-    DescribeParametersRequestDescribeParametersPaginateTypeDef,
-    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     DescribeEventsResponseTypeDef,
     ParameterTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     SubnetGroupTypeDef,
     ClusterTypeDef,
     DescribeDefaultParametersResponseTypeDef,
     DescribeParametersResponseTypeDef,
@@ -431,42 +432,42 @@
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

### Comparing `mypy-boto3-dax-1.26.0.post1/mypy_boto3_dax.egg-info/SOURCES.txt` & `mypy-boto3-dax-1.27.0/mypy_boto3_dax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.26.0.post1/setup.py` & `mypy-boto3-dax-1.27.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-dax.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dax",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_dax"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DAX 1.26.0 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.DAX 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 dax type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_dax": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_dax": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/",
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


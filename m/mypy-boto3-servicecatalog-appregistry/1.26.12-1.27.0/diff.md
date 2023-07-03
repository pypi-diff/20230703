# Comparing `tmp/mypy-boto3-servicecatalog-appregistry-1.26.12.tar.gz` & `tmp/mypy-boto3-servicecatalog-appregistry-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-servicecatalog-appregistry-1.26.12.tar", last modified: Thu Nov 17 20:31:23 2022, max compression
+gzip compressed data, was "mypy-boto3-servicecatalog-appregistry-1.27.0.tar", last modified: Mon Jul  3 19:51:27 2023, max compression
```

## Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12.tar` & `mypy-boto3-servicecatalog-appregistry-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:31:23.988786 mypy-boto3-servicecatalog-appregistry-1.26.12/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-17 20:31:00.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    17111 2022-11-17 20:31:23.984786 mypy-boto3-servicecatalog-appregistry-1.26.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15613 2022-11-17 20:31:00.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:31:23.972786 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/
--rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-11-17 20:31:00.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-11-17 20:31:00.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-11-17 20:31:00.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21034 2022-11-17 20:31:00.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    20998 2022-11-17 20:31:00.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8603 2022-11-17 20:31:00.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8601 2022-11-17 20:31:00.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7076 2022-11-17 20:31:00.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7069 2022-11-17 20:31:00.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 20:31:00.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    21590 2022-11-17 20:31:01.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    21569 2022-11-17 20:31:00.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-17 20:31:00.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:31:23.972786 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17111 2022-11-17 20:31:23.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-11-17 20:31:23.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 20:31:23.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 20:31:23.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-17 20:31:23.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 20:31:23.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 20:31:23.988786 mypy-boto3-servicecatalog-appregistry-1.26.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-11-17 20:30:59.000000 mypy-boto3-servicecatalog-appregistry-1.26.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:26.999990 mypy-boto3-servicecatalog-appregistry-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:01.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17155 2023-07-03 19:51:26.991990 mypy-boto3-servicecatalog-appregistry-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15609 2023-07-03 19:48:01.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:26.991990 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-03 19:48:01.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-03 19:48:01.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-03 19:48:01.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-07-03 19:48:02.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21071 2023-07-03 19:48:01.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-07-03 19:48:02.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-03 19:48:02.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-07-03 19:48:02.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-07-03 19:48:02.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:01.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21722 2023-07-03 19:48:02.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-07-03 19:48:02.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:01.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:26.991990 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17155 2023-07-03 19:51:26.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-03 19:51:26.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:26.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:26.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:26.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:26.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:26.999990 mypy-boto3-servicecatalog-appregistry-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-03 19:48:01.000000 mypy-boto3-servicecatalog-appregistry-1.27.0/setup.py
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/LICENSE` & `mypy-boto3-servicecatalog-appregistry-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/PKG-INFO` & `mypy-boto3-servicecatalog-appregistry-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog-appregistry
-Version: 1.26.12
-Summary: Type annotations for boto3.AppRegistry 1.26.12 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.AppRegistry 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/
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
 
 <a id="mypy-boto3-servicecatalog-appregistry"></a>
 
 # mypy-boto3-servicecatalog-appregistry
 
 [![PyPI - mypy-boto3-servicecatalog-appregistry](https://img.shields.io/pypi/v/mypy-boto3-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog-appregistry)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog-appregistry)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicecatalog-appregistry?color=blue)](https://pypistats.org/packages/mypy-boto3-servicecatalog-appregistry)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRegistry 1.26.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
+[boto3.AppRegistry 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
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
 [mypy-boto3-servicecatalog-appregistry docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,68 +349,68 @@
 
 ```python
 from mypy_boto3_servicecatalog_appregistry.type_defs import (
     TagQueryConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     AssociateAttributeGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateAttributeGroupResponseTypeDef,
     AssociateResourceRequestRequestTypeDef,
+    AssociateResourceResponseTypeDef,
     AttributeGroupDetailsTypeDef,
     AttributeGroupSummaryTypeDef,
     AttributeGroupTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateAttributeGroupRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteAttributeGroupRequestRequestTypeDef,
     DisassociateAttributeGroupRequestRequestTypeDef,
+    DisassociateAttributeGroupResponseTypeDef,
     DisassociateResourceRequestRequestTypeDef,
+    DisassociateResourceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetAssociatedResourceRequestRequestTypeDef,
     GetAttributeGroupRequestRequestTypeDef,
+    GetAttributeGroupResponseTypeDef,
     ResourceGroupTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
     ListAssociatedAttributeGroupsRequestRequestTypeDef,
+    ListAssociatedAttributeGroupsResponseTypeDef,
+    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
     ListAssociatedResourcesRequestRequestTypeDef,
+    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
     ListAttributeGroupsForApplicationRequestRequestTypeDef,
+    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ListAttributeGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     ResourceDetailsTypeDef,
+    ResponseMetadataTypeDef,
     SyncResourceRequestRequestTypeDef,
+    SyncResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateAttributeGroupRequestRequestTypeDef,
     AppRegistryConfigurationTypeDef,
-    AssociateAttributeGroupResponseTypeDef,
-    AssociateResourceResponseTypeDef,
-    CreateApplicationResponseTypeDef,
     DeleteApplicationResponseTypeDef,
-    DisassociateAttributeGroupResponseTypeDef,
-    DisassociateResourceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAttributeGroupResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListAssociatedAttributeGroupsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SyncResourceResponseTypeDef,
+    CreateApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     ListAttributeGroupsForApplicationResponseTypeDef,
     DeleteAttributeGroupResponseTypeDef,
     ListAttributeGroupsResponseTypeDef,
     CreateAttributeGroupResponseTypeDef,
     UpdateAttributeGroupResponseTypeDef,
     IntegrationsTypeDef,
     ResourceIntegrationsTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ResourceInfoTypeDef,
     GetConfigurationResponseTypeDef,
     PutConfigurationRequestRequestTypeDef,
     GetApplicationResponseTypeDef,
     ResourceTypeDef,
     ListAssociatedResourcesResponseTypeDef,
     GetAssociatedResourceResponseTypeDef,
@@ -423,42 +424,42 @@
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

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/README.md` & `mypy-boto3-servicecatalog-appregistry-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-servicecatalog-appregistry"></a>
 
 # mypy-boto3-servicecatalog-appregistry
 
 [![PyPI - mypy-boto3-servicecatalog-appregistry](https://img.shields.io/pypi/v/mypy-boto3-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog-appregistry)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog-appregistry)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicecatalog-appregistry?color=blue)](https://pypistats.org/packages/mypy-boto3-servicecatalog-appregistry)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRegistry 1.26.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
+[boto3.AppRegistry 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
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
 [mypy-boto3-servicecatalog-appregistry docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,68 +317,68 @@
 
 ```python
 from mypy_boto3_servicecatalog_appregistry.type_defs import (
     TagQueryConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     AssociateAttributeGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateAttributeGroupResponseTypeDef,
     AssociateResourceRequestRequestTypeDef,
+    AssociateResourceResponseTypeDef,
     AttributeGroupDetailsTypeDef,
     AttributeGroupSummaryTypeDef,
     AttributeGroupTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateAttributeGroupRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteAttributeGroupRequestRequestTypeDef,
     DisassociateAttributeGroupRequestRequestTypeDef,
+    DisassociateAttributeGroupResponseTypeDef,
     DisassociateResourceRequestRequestTypeDef,
+    DisassociateResourceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetAssociatedResourceRequestRequestTypeDef,
     GetAttributeGroupRequestRequestTypeDef,
+    GetAttributeGroupResponseTypeDef,
     ResourceGroupTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
     ListAssociatedAttributeGroupsRequestRequestTypeDef,
+    ListAssociatedAttributeGroupsResponseTypeDef,
+    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
     ListAssociatedResourcesRequestRequestTypeDef,
+    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
     ListAttributeGroupsForApplicationRequestRequestTypeDef,
+    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ListAttributeGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     ResourceDetailsTypeDef,
+    ResponseMetadataTypeDef,
     SyncResourceRequestRequestTypeDef,
+    SyncResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateAttributeGroupRequestRequestTypeDef,
     AppRegistryConfigurationTypeDef,
-    AssociateAttributeGroupResponseTypeDef,
-    AssociateResourceResponseTypeDef,
-    CreateApplicationResponseTypeDef,
     DeleteApplicationResponseTypeDef,
-    DisassociateAttributeGroupResponseTypeDef,
-    DisassociateResourceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAttributeGroupResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListAssociatedAttributeGroupsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SyncResourceResponseTypeDef,
+    CreateApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     ListAttributeGroupsForApplicationResponseTypeDef,
     DeleteAttributeGroupResponseTypeDef,
     ListAttributeGroupsResponseTypeDef,
     CreateAttributeGroupResponseTypeDef,
     UpdateAttributeGroupResponseTypeDef,
     IntegrationsTypeDef,
     ResourceIntegrationsTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ResourceInfoTypeDef,
     GetConfigurationResponseTypeDef,
     PutConfigurationRequestRequestTypeDef,
     GetApplicationResponseTypeDef,
     ResourceTypeDef,
     ListAssociatedResourcesResponseTypeDef,
     GetAssociatedResourceResponseTypeDef,
@@ -392,42 +392,42 @@
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

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/__init__.py` & `mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/__init__.pyi` & `mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/__main__.py` & `mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppRegistry 1.26.12\nVersion:         1.26.12\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.AppRegistry 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry\nOther"
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

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/client.py` & `mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
+    ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 
 class AppRegistryClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/client/)
@@ -157,23 +158,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.create_attribute_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/client/#create_attribute_group)
         """
 
     def delete_application(self, *, application: str) -> DeleteApplicationResponseTypeDef:
         """
-        Deletes an application that is specified either by its application ID or name.
+        Deletes an application that is specified either by its application ID, name, or
+        ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/client/#delete_application)
         """
 
     def delete_attribute_group(self, *, attributeGroup: str) -> DeleteAttributeGroupResponseTypeDef:
         """
-        Deletes an attribute group, specified either by its attribute group ID or name.
+        Deletes an attribute group, specified either by its attribute group ID, name, or
+        ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.delete_attribute_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/client/#delete_attribute_group)
         """
 
     def disassociate_attribute_group(
         self, *, application: str, attributeGroup: str
@@ -226,15 +229,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.get_associated_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/client/#get_associated_resource)
         """
 
     def get_attribute_group(self, *, attributeGroup: str) -> GetAttributeGroupResponseTypeDef:
         """
-        Retrieves an attribute group, either by its name or its ID.
+        Retrieves an attribute group by its ARN, ID, or name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.get_attribute_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/client/#get_attribute_group)
         """
 
     def get_configuration(self) -> GetConfigurationResponseTypeDef:
         """
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/client.pyi` & `mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
+    ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 class AppRegistryClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/client/)
     """
@@ -146,22 +147,24 @@
         Creates a new attribute group as a container for user-defined attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.create_attribute_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/client/#create_attribute_group)
         """
     def delete_application(self, *, application: str) -> DeleteApplicationResponseTypeDef:
         """
-        Deletes an application that is specified either by its application ID or name.
+        Deletes an application that is specified either by its application ID, name, or
+        ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/client/#delete_application)
         """
     def delete_attribute_group(self, *, attributeGroup: str) -> DeleteAttributeGroupResponseTypeDef:
         """
-        Deletes an attribute group, specified either by its attribute group ID or name.
+        Deletes an attribute group, specified either by its attribute group ID, name, or
+        ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.delete_attribute_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/client/#delete_attribute_group)
         """
     def disassociate_attribute_group(
         self, *, application: str, attributeGroup: str
     ) -> DisassociateAttributeGroupResponseTypeDef:
@@ -208,15 +211,15 @@
         Gets the resource associated with the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.get_associated_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/client/#get_associated_resource)
         """
     def get_attribute_group(self, *, attributeGroup: str) -> GetAttributeGroupResponseTypeDef:
         """
-        Retrieves an attribute group, either by its name or its ID.
+        Retrieves an attribute group by its ARN, ID, or name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Client.get_attribute_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/client/#get_attribute_group)
         """
     def get_configuration(self) -> GetConfigurationResponseTypeDef:
         """
         Retrieves a `TagKey` configuration from an account.
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/literals.py` & `mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/literals.pyi`

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
     "ListApplicationsPaginatorName",
     "ListAssociatedAttributeGroupsPaginatorName",
     "ListAssociatedResourcesPaginatorName",
     "ListAttributeGroupsForApplicationPaginatorName",
     "ListAttributeGroupsPaginatorName",
     "ResourceGroupStateType",
@@ -31,15 +30,14 @@
     "AppRegistryServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListAssociatedAttributeGroupsPaginatorName = Literal["list_associated_attribute_groups"]
 ListAssociatedResourcesPaginatorName = Literal["list_associated_resources"]
 ListAttributeGroupsForApplicationPaginatorName = Literal["list_attribute_groups_for_application"]
 ListAttributeGroupsPaginatorName = Literal["list_attribute_groups"]
 ResourceGroupStateType = Literal[
     "CREATE_COMPLETE", "CREATE_FAILED", "CREATING", "UPDATE_COMPLETE", "UPDATE_FAILED", "UPDATING"
@@ -58,23 +56,25 @@
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
@@ -84,30 +84,35 @@
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
@@ -133,14 +138,15 @@
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
@@ -185,51 +191,57 @@
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
@@ -242,14 +254,15 @@
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
@@ -261,28 +274,35 @@
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
@@ -310,57 +330,64 @@
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
@@ -402,14 +429,15 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/literals.pyi` & `mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/literals.py`

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
     "ListApplicationsPaginatorName",
     "ListAssociatedAttributeGroupsPaginatorName",
     "ListAssociatedResourcesPaginatorName",
     "ListAttributeGroupsForApplicationPaginatorName",
     "ListAttributeGroupsPaginatorName",
     "ResourceGroupStateType",
@@ -30,14 +31,15 @@
     "AppRegistryServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ListApplicationsPaginatorName = Literal["list_applications"]
 ListAssociatedAttributeGroupsPaginatorName = Literal["list_associated_attribute_groups"]
 ListAssociatedResourcesPaginatorName = Literal["list_associated_resources"]
 ListAttributeGroupsForApplicationPaginatorName = Literal["list_attribute_groups_for_application"]
 ListAttributeGroupsPaginatorName = Literal["list_attribute_groups"]
 ResourceGroupStateType = Literal[
     "CREATE_COMPLETE", "CREATE_FAILED", "CREATING", "UPDATE_COMPLETE", "UPDATE_FAILED", "UPDATING"
@@ -56,23 +58,25 @@
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
@@ -82,30 +86,35 @@
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
@@ -131,14 +140,15 @@
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
@@ -183,51 +193,57 @@
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
@@ -240,14 +256,15 @@
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
@@ -259,28 +276,35 @@
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
@@ -308,57 +332,64 @@
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
@@ -400,14 +431,15 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/paginator.py` & `mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,73 +62,73 @@
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listapplicationspaginator)
         """
 
 
 class ListAssociatedAttributeGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedAttributeGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedattributegroupspaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociatedAttributeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedAttributeGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedattributegroupspaginator)
         """
 
 
 class ListAssociatedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedresourcespaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociatedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedresourcespaginator)
         """
 
 
 class ListAttributeGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAttributeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupspaginator)
         """
 
 
 class ListAttributeGroupsForApplicationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroupsForApplication)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupsforapplicationpaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAttributeGroupsForApplicationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroupsForApplication.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupsforapplicationpaginator)
         """
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/paginator.pyi` & `mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -59,69 +59,69 @@
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listapplicationspaginator)
         """
 
 class ListAssociatedAttributeGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedAttributeGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedattributegroupspaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociatedAttributeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedAttributeGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedattributegroupspaginator)
         """
 
 class ListAssociatedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedresourcespaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssociatedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedresourcespaginator)
         """
 
 class ListAttributeGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAttributeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupspaginator)
         """
 
 class ListAttributeGroupsForApplicationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroupsForApplication)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupsforapplicationpaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAttributeGroupsForApplicationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroupsForApplication.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupsforapplicationpaginator)
         """
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/type_defs.py` & `mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,68 +24,68 @@
 
 
 __all__ = (
     "TagQueryConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
     "AssociateAttributeGroupRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateAttributeGroupResponseTypeDef",
     "AssociateResourceRequestRequestTypeDef",
+    "AssociateResourceResponseTypeDef",
     "AttributeGroupDetailsTypeDef",
     "AttributeGroupSummaryTypeDef",
     "AttributeGroupTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateAttributeGroupRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteAttributeGroupRequestRequestTypeDef",
     "DisassociateAttributeGroupRequestRequestTypeDef",
+    "DisassociateAttributeGroupResponseTypeDef",
     "DisassociateResourceRequestRequestTypeDef",
+    "DisassociateResourceResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetAssociatedResourceRequestRequestTypeDef",
     "GetAttributeGroupRequestRequestTypeDef",
+    "GetAttributeGroupResponseTypeDef",
     "ResourceGroupTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
+    "ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
     "ListAssociatedAttributeGroupsRequestRequestTypeDef",
+    "ListAssociatedAttributeGroupsResponseTypeDef",
+    "ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
     "ListAssociatedResourcesRequestRequestTypeDef",
+    "ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
     "ListAttributeGroupsForApplicationRequestRequestTypeDef",
+    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
     "ListAttributeGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "ResourceDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "SyncResourceRequestRequestTypeDef",
+    "SyncResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateAttributeGroupRequestRequestTypeDef",
     "AppRegistryConfigurationTypeDef",
-    "AssociateAttributeGroupResponseTypeDef",
-    "AssociateResourceResponseTypeDef",
-    "CreateApplicationResponseTypeDef",
     "DeleteApplicationResponseTypeDef",
-    "DisassociateAttributeGroupResponseTypeDef",
-    "DisassociateResourceResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAttributeGroupResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "ListAssociatedAttributeGroupsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "SyncResourceResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "ListAttributeGroupsForApplicationResponseTypeDef",
     "DeleteAttributeGroupResponseTypeDef",
     "ListAttributeGroupsResponseTypeDef",
     "CreateAttributeGroupResponseTypeDef",
     "UpdateAttributeGroupResponseTypeDef",
     "IntegrationsTypeDef",
     "ResourceIntegrationsTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    "ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
-    "ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
-    "ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
-    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
     "ResourceInfoTypeDef",
     "GetConfigurationResponseTypeDef",
     "PutConfigurationRequestRequestTypeDef",
     "GetApplicationResponseTypeDef",
     "ResourceTypeDef",
     "ListAssociatedResourcesResponseTypeDef",
     "GetAssociatedResourceResponseTypeDef",
@@ -130,53 +130,62 @@
     "AssociateAttributeGroupRequestRequestTypeDef",
     {
         "application": str,
         "attributeGroup": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateAttributeGroupResponseTypeDef = TypedDict(
+    "AssociateAttributeGroupResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "applicationArn": str,
+        "attributeGroupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateResourceRequestRequestTypeDef = TypedDict(
     "AssociateResourceRequestRequestTypeDef",
     {
         "application": str,
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
+AssociateResourceResponseTypeDef = TypedDict(
+    "AssociateResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AttributeGroupDetailsTypeDef = TypedDict(
     "AttributeGroupDetailsTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
+        "createdBy": str,
     },
     total=False,
 )
 
 AttributeGroupSummaryTypeDef = TypedDict(
     "AttributeGroupSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
+        "createdBy": str,
     },
     total=False,
 )
 
 AttributeGroupTypeDef = TypedDict(
     "AttributeGroupTypeDef",
     {
@@ -257,23 +266,48 @@
     "DisassociateAttributeGroupRequestRequestTypeDef",
     {
         "application": str,
         "attributeGroup": str,
     },
 )
 
+DisassociateAttributeGroupResponseTypeDef = TypedDict(
+    "DisassociateAttributeGroupResponseTypeDef",
+    {
+        "applicationArn": str,
+        "attributeGroupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateResourceRequestRequestTypeDef = TypedDict(
     "DisassociateResourceRequestRequestTypeDef",
     {
         "application": str,
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
+DisassociateResourceResponseTypeDef = TypedDict(
+    "DisassociateResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetApplicationRequestRequestTypeDef = TypedDict(
     "GetApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 
@@ -289,43 +323,83 @@
 GetAttributeGroupRequestRequestTypeDef = TypedDict(
     "GetAttributeGroupRequestRequestTypeDef",
     {
         "attributeGroup": str,
     },
 )
 
+GetAttributeGroupResponseTypeDef = TypedDict(
+    "GetAttributeGroupResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "attributes": str,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "tags": Dict[str, str],
+        "createdBy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ResourceGroupTypeDef = TypedDict(
     "ResourceGroupTypeDef",
     {
         "state": ResourceGroupStateType,
         "arn": str,
         "errorMessage": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+        {
+            "application": str,
+        },
+    )
+)
+_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+        {
+            "PaginationConfig": "PaginatorConfigTypeDef",
+        },
+        total=False,
+    )
+)
+
+
+class ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef(
+    _RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+    _OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAssociatedAttributeGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedAttributeGroupsRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAssociatedAttributeGroupsRequestRequestTypeDef = TypedDict(
@@ -341,14 +415,45 @@
 class ListAssociatedAttributeGroupsRequestRequestTypeDef(
     _RequiredListAssociatedAttributeGroupsRequestRequestTypeDef,
     _OptionalListAssociatedAttributeGroupsRequestRequestTypeDef,
 ):
     pass
 
 
+ListAssociatedAttributeGroupsResponseTypeDef = TypedDict(
+    "ListAssociatedAttributeGroupsResponseTypeDef",
+    {
+        "attributeGroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    {
+        "application": str,
+    },
+)
+_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef(
+    _RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+    _OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAssociatedResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedResourcesRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAssociatedResourcesRequestRequestTypeDef = TypedDict(
@@ -364,14 +469,36 @@
 class ListAssociatedResourcesRequestRequestTypeDef(
     _RequiredListAssociatedResourcesRequestRequestTypeDef,
     _OptionalListAssociatedResourcesRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
+    "_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    {
+        "application": str,
+    },
+)
+_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
+    "_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef(
+    _RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+    _OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAttributeGroupsForApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredListAttributeGroupsForApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAttributeGroupsForApplicationRequestRequestTypeDef = TypedDict(
@@ -387,14 +514,22 @@
 class ListAttributeGroupsForApplicationRequestRequestTypeDef(
     _RequiredListAttributeGroupsForApplicationRequestRequestTypeDef,
     _OptionalListAttributeGroupsForApplicationRequestRequestTypeDef,
 ):
     pass
 
 
+ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef = TypedDict(
+    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListAttributeGroupsRequestRequestTypeDef = TypedDict(
     "ListAttributeGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -403,30 +538,69 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
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
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "tagValue": str,
     },
     total=False,
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
 SyncResourceRequestRequestTypeDef = TypedDict(
     "SyncResourceRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
+SyncResourceResponseTypeDef = TypedDict(
+    "SyncResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "actionTaken": SyncActionType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -489,171 +663,86 @@
     "AppRegistryConfigurationTypeDef",
     {
         "tagQueryConfiguration": TagQueryConfigurationTypeDef,
     },
     total=False,
 )
 
-AssociateAttributeGroupResponseTypeDef = TypedDict(
-    "AssociateAttributeGroupResponseTypeDef",
-    {
-        "applicationArn": str,
-        "attributeGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateResourceResponseTypeDef = TypedDict(
-    "AssociateResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "application": ApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeleteApplicationResponseTypeDef = TypedDict(
     "DeleteApplicationResponseTypeDef",
     {
         "application": ApplicationSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateAttributeGroupResponseTypeDef = TypedDict(
-    "DisassociateAttributeGroupResponseTypeDef",
-    {
-        "applicationArn": str,
-        "attributeGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateResourceResponseTypeDef = TypedDict(
-    "DisassociateResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
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
-GetAttributeGroupResponseTypeDef = TypedDict(
-    "GetAttributeGroupResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "attributes": str,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAssociatedAttributeGroupsResponseTypeDef = TypedDict(
-    "ListAssociatedAttributeGroupsResponseTypeDef",
-    {
-        "attributeGroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SyncResourceResponseTypeDef = TypedDict(
-    "SyncResourceResponseTypeDef",
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
     {
-        "applicationArn": str,
-        "resourceArn": str,
-        "actionTaken": SyncActionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "application": ApplicationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAttributeGroupsForApplicationResponseTypeDef = TypedDict(
     "ListAttributeGroupsForApplicationResponseTypeDef",
     {
         "attributeGroupsDetails": List[AttributeGroupDetailsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAttributeGroupResponseTypeDef = TypedDict(
     "DeleteAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAttributeGroupsResponseTypeDef = TypedDict(
     "ListAttributeGroupsResponseTypeDef",
     {
         "attributeGroups": List[AttributeGroupSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAttributeGroupResponseTypeDef = TypedDict(
     "CreateAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAttributeGroupResponseTypeDef = TypedDict(
     "UpdateAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IntegrationsTypeDef = TypedDict(
     "IntegrationsTypeDef",
     {
         "resourceGroup": ResourceGroupTypeDef,
@@ -665,100 +754,14 @@
     "ResourceIntegrationsTypeDef",
     {
         "resourceGroup": ResourceGroupTypeDef,
     },
     total=False,
 )
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
-        {
-            "application": str,
-        },
-    )
-)
-_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
-        {
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-
-class ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef(
-    _RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-    _OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
-    {
-        "application": str,
-    },
-)
-_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef(
-    _RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-    _OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
-    "_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
-    {
-        "application": str,
-    },
-)
-_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
-    "_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef(
-    _RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-    _OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-):
-    pass
-
-
-ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef = TypedDict(
-    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ResourceInfoTypeDef = TypedDict(
     "ResourceInfoTypeDef",
     {
         "name": str,
         "arn": str,
         "resourceType": ResourceTypeType,
         "resourceDetails": ResourceDetailsTypeDef,
@@ -766,15 +769,15 @@
     total=False,
 )
 
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
         "configuration": AppRegistryConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutConfigurationRequestRequestTypeDef = TypedDict(
     "PutConfigurationRequestRequestTypeDef",
     {
         "configuration": AppRegistryConfigurationTypeDef,
@@ -789,15 +792,15 @@
         "name": str,
         "description": str,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "associatedResourceCount": int,
         "tags": Dict[str, str],
         "integrations": IntegrationsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "name": str,
@@ -809,18 +812,18 @@
 )
 
 ListAssociatedResourcesResponseTypeDef = TypedDict(
     "ListAssociatedResourcesResponseTypeDef",
     {
         "resources": List[ResourceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAssociatedResourceResponseTypeDef = TypedDict(
     "GetAssociatedResourceResponseTypeDef",
     {
         "resource": ResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry/type_defs.pyi` & `mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,68 +23,68 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagQueryConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
     "AssociateAttributeGroupRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateAttributeGroupResponseTypeDef",
     "AssociateResourceRequestRequestTypeDef",
+    "AssociateResourceResponseTypeDef",
     "AttributeGroupDetailsTypeDef",
     "AttributeGroupSummaryTypeDef",
     "AttributeGroupTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateAttributeGroupRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteAttributeGroupRequestRequestTypeDef",
     "DisassociateAttributeGroupRequestRequestTypeDef",
+    "DisassociateAttributeGroupResponseTypeDef",
     "DisassociateResourceRequestRequestTypeDef",
+    "DisassociateResourceResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetAssociatedResourceRequestRequestTypeDef",
     "GetAttributeGroupRequestRequestTypeDef",
+    "GetAttributeGroupResponseTypeDef",
     "ResourceGroupTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
+    "ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
     "ListAssociatedAttributeGroupsRequestRequestTypeDef",
+    "ListAssociatedAttributeGroupsResponseTypeDef",
+    "ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
     "ListAssociatedResourcesRequestRequestTypeDef",
+    "ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
     "ListAttributeGroupsForApplicationRequestRequestTypeDef",
+    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
     "ListAttributeGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "ResourceDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "SyncResourceRequestRequestTypeDef",
+    "SyncResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateAttributeGroupRequestRequestTypeDef",
     "AppRegistryConfigurationTypeDef",
-    "AssociateAttributeGroupResponseTypeDef",
-    "AssociateResourceResponseTypeDef",
-    "CreateApplicationResponseTypeDef",
     "DeleteApplicationResponseTypeDef",
-    "DisassociateAttributeGroupResponseTypeDef",
-    "DisassociateResourceResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAttributeGroupResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "ListAssociatedAttributeGroupsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "SyncResourceResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "ListAttributeGroupsForApplicationResponseTypeDef",
     "DeleteAttributeGroupResponseTypeDef",
     "ListAttributeGroupsResponseTypeDef",
     "CreateAttributeGroupResponseTypeDef",
     "UpdateAttributeGroupResponseTypeDef",
     "IntegrationsTypeDef",
     "ResourceIntegrationsTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    "ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
-    "ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
-    "ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
-    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
     "ResourceInfoTypeDef",
     "GetConfigurationResponseTypeDef",
     "PutConfigurationRequestRequestTypeDef",
     "GetApplicationResponseTypeDef",
     "ResourceTypeDef",
     "ListAssociatedResourcesResponseTypeDef",
     "GetAssociatedResourceResponseTypeDef",
@@ -129,53 +129,62 @@
     "AssociateAttributeGroupRequestRequestTypeDef",
     {
         "application": str,
         "attributeGroup": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateAttributeGroupResponseTypeDef = TypedDict(
+    "AssociateAttributeGroupResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "applicationArn": str,
+        "attributeGroupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateResourceRequestRequestTypeDef = TypedDict(
     "AssociateResourceRequestRequestTypeDef",
     {
         "application": str,
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
+AssociateResourceResponseTypeDef = TypedDict(
+    "AssociateResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AttributeGroupDetailsTypeDef = TypedDict(
     "AttributeGroupDetailsTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
+        "createdBy": str,
     },
     total=False,
 )
 
 AttributeGroupSummaryTypeDef = TypedDict(
     "AttributeGroupSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
+        "createdBy": str,
     },
     total=False,
 )
 
 AttributeGroupTypeDef = TypedDict(
     "AttributeGroupTypeDef",
     {
@@ -252,23 +261,48 @@
     "DisassociateAttributeGroupRequestRequestTypeDef",
     {
         "application": str,
         "attributeGroup": str,
     },
 )
 
+DisassociateAttributeGroupResponseTypeDef = TypedDict(
+    "DisassociateAttributeGroupResponseTypeDef",
+    {
+        "applicationArn": str,
+        "attributeGroupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateResourceRequestRequestTypeDef = TypedDict(
     "DisassociateResourceRequestRequestTypeDef",
     {
         "application": str,
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
+DisassociateResourceResponseTypeDef = TypedDict(
+    "DisassociateResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetApplicationRequestRequestTypeDef = TypedDict(
     "GetApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 
@@ -284,43 +318,81 @@
 GetAttributeGroupRequestRequestTypeDef = TypedDict(
     "GetAttributeGroupRequestRequestTypeDef",
     {
         "attributeGroup": str,
     },
 )
 
+GetAttributeGroupResponseTypeDef = TypedDict(
+    "GetAttributeGroupResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "attributes": str,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "tags": Dict[str, str],
+        "createdBy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ResourceGroupTypeDef = TypedDict(
     "ResourceGroupTypeDef",
     {
         "state": ResourceGroupStateType,
         "arn": str,
         "errorMessage": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+        {
+            "application": str,
+        },
+    )
+)
+_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+        {
+            "PaginationConfig": "PaginatorConfigTypeDef",
+        },
+        total=False,
+    )
+)
+
+class ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef(
+    _RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+    _OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+):
+    pass
+
 _RequiredListAssociatedAttributeGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedAttributeGroupsRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAssociatedAttributeGroupsRequestRequestTypeDef = TypedDict(
@@ -334,14 +406,43 @@
 
 class ListAssociatedAttributeGroupsRequestRequestTypeDef(
     _RequiredListAssociatedAttributeGroupsRequestRequestTypeDef,
     _OptionalListAssociatedAttributeGroupsRequestRequestTypeDef,
 ):
     pass
 
+ListAssociatedAttributeGroupsResponseTypeDef = TypedDict(
+    "ListAssociatedAttributeGroupsResponseTypeDef",
+    {
+        "attributeGroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    {
+        "application": str,
+    },
+)
+_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef(
+    _RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+    _OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+):
+    pass
+
 _RequiredListAssociatedResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedResourcesRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAssociatedResourcesRequestRequestTypeDef = TypedDict(
@@ -355,14 +456,34 @@
 
 class ListAssociatedResourcesRequestRequestTypeDef(
     _RequiredListAssociatedResourcesRequestRequestTypeDef,
     _OptionalListAssociatedResourcesRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
+    "_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    {
+        "application": str,
+    },
+)
+_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
+    "_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef(
+    _RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+    _OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+):
+    pass
+
 _RequiredListAttributeGroupsForApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredListAttributeGroupsForApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAttributeGroupsForApplicationRequestRequestTypeDef = TypedDict(
@@ -376,14 +497,22 @@
 
 class ListAttributeGroupsForApplicationRequestRequestTypeDef(
     _RequiredListAttributeGroupsForApplicationRequestRequestTypeDef,
     _OptionalListAttributeGroupsForApplicationRequestRequestTypeDef,
 ):
     pass
 
+ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef = TypedDict(
+    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListAttributeGroupsRequestRequestTypeDef = TypedDict(
     "ListAttributeGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -392,30 +521,69 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
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
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "tagValue": str,
     },
     total=False,
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
 SyncResourceRequestRequestTypeDef = TypedDict(
     "SyncResourceRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
+SyncResourceResponseTypeDef = TypedDict(
+    "SyncResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "actionTaken": SyncActionType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -474,171 +642,86 @@
     "AppRegistryConfigurationTypeDef",
     {
         "tagQueryConfiguration": TagQueryConfigurationTypeDef,
     },
     total=False,
 )
 
-AssociateAttributeGroupResponseTypeDef = TypedDict(
-    "AssociateAttributeGroupResponseTypeDef",
-    {
-        "applicationArn": str,
-        "attributeGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociateResourceResponseTypeDef = TypedDict(
-    "AssociateResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "application": ApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeleteApplicationResponseTypeDef = TypedDict(
     "DeleteApplicationResponseTypeDef",
     {
         "application": ApplicationSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateAttributeGroupResponseTypeDef = TypedDict(
-    "DisassociateAttributeGroupResponseTypeDef",
-    {
-        "applicationArn": str,
-        "attributeGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateResourceResponseTypeDef = TypedDict(
-    "DisassociateResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
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
-GetAttributeGroupResponseTypeDef = TypedDict(
-    "GetAttributeGroupResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "attributes": str,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAssociatedAttributeGroupsResponseTypeDef = TypedDict(
-    "ListAssociatedAttributeGroupsResponseTypeDef",
-    {
-        "attributeGroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SyncResourceResponseTypeDef = TypedDict(
-    "SyncResourceResponseTypeDef",
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
     {
-        "applicationArn": str,
-        "resourceArn": str,
-        "actionTaken": SyncActionType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "application": ApplicationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAttributeGroupsForApplicationResponseTypeDef = TypedDict(
     "ListAttributeGroupsForApplicationResponseTypeDef",
     {
         "attributeGroupsDetails": List[AttributeGroupDetailsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAttributeGroupResponseTypeDef = TypedDict(
     "DeleteAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAttributeGroupsResponseTypeDef = TypedDict(
     "ListAttributeGroupsResponseTypeDef",
     {
         "attributeGroups": List[AttributeGroupSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAttributeGroupResponseTypeDef = TypedDict(
     "CreateAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAttributeGroupResponseTypeDef = TypedDict(
     "UpdateAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IntegrationsTypeDef = TypedDict(
     "IntegrationsTypeDef",
     {
         "resourceGroup": ResourceGroupTypeDef,
@@ -650,94 +733,14 @@
     "ResourceIntegrationsTypeDef",
     {
         "resourceGroup": ResourceGroupTypeDef,
     },
     total=False,
 )
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
-        {
-            "application": str,
-        },
-    )
-)
-_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
-        {
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-class ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef(
-    _RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-    _OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-):
-    pass
-
-_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
-    {
-        "application": str,
-    },
-)
-_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef(
-    _RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-    _OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-):
-    pass
-
-_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
-    "_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
-    {
-        "application": str,
-    },
-)
-_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
-    "_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef(
-    _RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-    _OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-):
-    pass
-
-ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef = TypedDict(
-    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ResourceInfoTypeDef = TypedDict(
     "ResourceInfoTypeDef",
     {
         "name": str,
         "arn": str,
         "resourceType": ResourceTypeType,
         "resourceDetails": ResourceDetailsTypeDef,
@@ -745,15 +748,15 @@
     total=False,
 )
 
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
         "configuration": AppRegistryConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutConfigurationRequestRequestTypeDef = TypedDict(
     "PutConfigurationRequestRequestTypeDef",
     {
         "configuration": AppRegistryConfigurationTypeDef,
@@ -768,15 +771,15 @@
         "name": str,
         "description": str,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "associatedResourceCount": int,
         "tags": Dict[str, str],
         "integrations": IntegrationsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "name": str,
@@ -788,18 +791,18 @@
 )
 
 ListAssociatedResourcesResponseTypeDef = TypedDict(
     "ListAssociatedResourcesResponseTypeDef",
     {
         "resources": List[ResourceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAssociatedResourceResponseTypeDef = TypedDict(
     "GetAssociatedResourceResponseTypeDef",
     {
         "resource": ResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO` & `mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog-appregistry
-Version: 1.26.12
-Summary: Type annotations for boto3.AppRegistry 1.26.12 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.AppRegistry 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/
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
 
 <a id="mypy-boto3-servicecatalog-appregistry"></a>
 
 # mypy-boto3-servicecatalog-appregistry
 
 [![PyPI - mypy-boto3-servicecatalog-appregistry](https://img.shields.io/pypi/v/mypy-boto3-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog-appregistry)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog-appregistry)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicecatalog-appregistry?color=blue)](https://pypistats.org/packages/mypy-boto3-servicecatalog-appregistry)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRegistry 1.26.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
+[boto3.AppRegistry 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
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
 [mypy-boto3-servicecatalog-appregistry docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,68 +349,68 @@
 
 ```python
 from mypy_boto3_servicecatalog_appregistry.type_defs import (
     TagQueryConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     AssociateAttributeGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateAttributeGroupResponseTypeDef,
     AssociateResourceRequestRequestTypeDef,
+    AssociateResourceResponseTypeDef,
     AttributeGroupDetailsTypeDef,
     AttributeGroupSummaryTypeDef,
     AttributeGroupTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateAttributeGroupRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteAttributeGroupRequestRequestTypeDef,
     DisassociateAttributeGroupRequestRequestTypeDef,
+    DisassociateAttributeGroupResponseTypeDef,
     DisassociateResourceRequestRequestTypeDef,
+    DisassociateResourceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetAssociatedResourceRequestRequestTypeDef,
     GetAttributeGroupRequestRequestTypeDef,
+    GetAttributeGroupResponseTypeDef,
     ResourceGroupTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
     ListAssociatedAttributeGroupsRequestRequestTypeDef,
+    ListAssociatedAttributeGroupsResponseTypeDef,
+    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
     ListAssociatedResourcesRequestRequestTypeDef,
+    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
     ListAttributeGroupsForApplicationRequestRequestTypeDef,
+    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ListAttributeGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     ResourceDetailsTypeDef,
+    ResponseMetadataTypeDef,
     SyncResourceRequestRequestTypeDef,
+    SyncResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateAttributeGroupRequestRequestTypeDef,
     AppRegistryConfigurationTypeDef,
-    AssociateAttributeGroupResponseTypeDef,
-    AssociateResourceResponseTypeDef,
-    CreateApplicationResponseTypeDef,
     DeleteApplicationResponseTypeDef,
-    DisassociateAttributeGroupResponseTypeDef,
-    DisassociateResourceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAttributeGroupResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListAssociatedAttributeGroupsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SyncResourceResponseTypeDef,
+    CreateApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     ListAttributeGroupsForApplicationResponseTypeDef,
     DeleteAttributeGroupResponseTypeDef,
     ListAttributeGroupsResponseTypeDef,
     CreateAttributeGroupResponseTypeDef,
     UpdateAttributeGroupResponseTypeDef,
     IntegrationsTypeDef,
     ResourceIntegrationsTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ResourceInfoTypeDef,
     GetConfigurationResponseTypeDef,
     PutConfigurationRequestRequestTypeDef,
     GetApplicationResponseTypeDef,
     ResourceTypeDef,
     ListAssociatedResourcesResponseTypeDef,
     GetAssociatedResourceResponseTypeDef,
@@ -423,42 +424,42 @@
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

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt` & `mypy-boto3-servicecatalog-appregistry-1.27.0/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.26.12/setup.py` & `mypy-boto3-servicecatalog-appregistry-1.27.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 """
 Setup script for mypy-boto3-servicecatalog-appregistry.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-servicecatalog-appregistry",
-    version="1.26.12",
+    version="1.27.0",
     packages=["mypy_boto3_servicecatalog_appregistry"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppRegistry 1.26.12 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.AppRegistry 1.27.0 service generated with mypy-boto3-builder"
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
     keywords=(
         "boto3 servicecatalog-appregistry type-annotations boto3-stubs mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_servicecatalog_appregistry": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_servicecatalog_appregistry": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/"
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


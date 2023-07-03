# Comparing `tmp/mypy-boto3-appintegrations-1.26.90.tar.gz` & `tmp/mypy-boto3-appintegrations-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appintegrations-1.26.90.tar", last modified: Mon Mar 13 19:32:22 2023, max compression
+gzip compressed data, was "mypy-boto3-appintegrations-1.27.0.tar", last modified: Mon Jul  3 19:50:22 2023, max compression
```

## Comparing `mypy-boto3-appintegrations-1.26.90.tar` & `mypy-boto3-appintegrations-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:22.883339 mypy-boto3-appintegrations-1.26.90/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-13 19:32:02.000000 mypy-boto3-appintegrations-1.26.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-03-13 19:32:22.883339 mypy-boto3-appintegrations-1.26.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-03-13 19:32:02.000000 mypy-boto3-appintegrations-1.26.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:22.871339 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-13 19:32:02.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-13 19:32:02.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-13 19:32:02.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-03-13 19:32:02.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-03-13 19:32:02.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-03-13 19:32:02.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-03-13 19:32:02.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:02.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-03-13 19:32:02.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-03-13 19:32:02.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-13 19:32:02.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:22.883339 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-03-13 19:32:22.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-13 19:32:22.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 19:32:22.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 19:32:22.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-13 19:32:22.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-13 19:32:22.000000 mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 19:32:22.883339 mypy-boto3-appintegrations-1.26.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-03-13 19:32:02.000000 mypy-boto3-appintegrations-1.26.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.526822 mypy-boto3-appintegrations-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:30.000000 mypy-boto3-appintegrations-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-07-03 19:50:22.526822 mypy-boto3-appintegrations-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-07-03 19:32:30.000000 mypy-boto3-appintegrations-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.522822 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-03 19:32:30.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-03 19:32:30.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-03 19:32:30.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-03 19:32:30.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-07-03 19:32:30.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-07-03 19:32:30.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-07-03 19:32:30.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:30.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-03 19:32:30.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-07-03 19:32:30.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:30.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.526822 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-07-03 19:50:22.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-03 19:50:22.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:22.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 19:50:22.000000 mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:22.526822 mypy-boto3-appintegrations-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-03 19:32:30.000000 mypy-boto3-appintegrations-1.27.0/setup.py
```

### Comparing `mypy-boto3-appintegrations-1.26.90/LICENSE` & `mypy-boto3-appintegrations-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-appintegrations-1.26.90/PKG-INFO` & `mypy-boto3-appintegrations-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appintegrations
-Version: 1.26.90
-Summary: Type annotations for boto3.AppIntegrationsService 1.26.90 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.AppIntegrationsService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-appintegrations"></a>
 
 # mypy-boto3-appintegrations
 
 [![PyPI - mypy-boto3-appintegrations](https://img.shields.io/pypi/v/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appintegrations?color=blue)](https://pypistats.org/packages/mypy-boto3-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppIntegrationsService 1.26.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[boto3.AppIntegrationsService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appintegrations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,37 +299,37 @@
 `mypy_boto3_appintegrations.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appintegrations.type_defs import (
     FileConfigurationTypeDef,
     ScheduleConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     EventFilterTypeDef,
+    CreateEventIntegrationResponseTypeDef,
     DataIntegrationAssociationSummaryTypeDef,
     DataIntegrationSummaryTypeDef,
     DeleteDataIntegrationRequestRequestTypeDef,
     DeleteEventIntegrationRequestRequestTypeDef,
     EventIntegrationAssociationTypeDef,
     GetDataIntegrationRequestRequestTypeDef,
     GetEventIntegrationRequestRequestTypeDef,
     ListDataIntegrationAssociationsRequestRequestTypeDef,
     ListDataIntegrationsRequestRequestTypeDef,
     ListEventIntegrationAssociationsRequestRequestTypeDef,
     ListEventIntegrationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDataIntegrationRequestRequestTypeDef,
     UpdateEventIntegrationRequestRequestTypeDef,
     CreateDataIntegrationRequestRequestTypeDef,
     CreateDataIntegrationResponseTypeDef,
-    CreateEventIntegrationResponseTypeDef,
     GetDataIntegrationResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateEventIntegrationRequestRequestTypeDef,
     EventIntegrationTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
@@ -343,42 +343,42 @@
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

### Comparing `mypy-boto3-appintegrations-1.26.90/README.md` & `mypy-boto3-appintegrations-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-appintegrations"></a>
 
 # mypy-boto3-appintegrations
 
 [![PyPI - mypy-boto3-appintegrations](https://img.shields.io/pypi/v/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appintegrations?color=blue)](https://pypistats.org/packages/mypy-boto3-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppIntegrationsService 1.26.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[boto3.AppIntegrationsService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appintegrations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,37 +267,37 @@
 `mypy_boto3_appintegrations.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appintegrations.type_defs import (
     FileConfigurationTypeDef,
     ScheduleConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     EventFilterTypeDef,
+    CreateEventIntegrationResponseTypeDef,
     DataIntegrationAssociationSummaryTypeDef,
     DataIntegrationSummaryTypeDef,
     DeleteDataIntegrationRequestRequestTypeDef,
     DeleteEventIntegrationRequestRequestTypeDef,
     EventIntegrationAssociationTypeDef,
     GetDataIntegrationRequestRequestTypeDef,
     GetEventIntegrationRequestRequestTypeDef,
     ListDataIntegrationAssociationsRequestRequestTypeDef,
     ListDataIntegrationsRequestRequestTypeDef,
     ListEventIntegrationAssociationsRequestRequestTypeDef,
     ListEventIntegrationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDataIntegrationRequestRequestTypeDef,
     UpdateEventIntegrationRequestRequestTypeDef,
     CreateDataIntegrationRequestRequestTypeDef,
     CreateDataIntegrationResponseTypeDef,
-    CreateEventIntegrationResponseTypeDef,
     GetDataIntegrationResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateEventIntegrationRequestRequestTypeDef,
     EventIntegrationTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
@@ -311,42 +311,42 @@
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

### Comparing `mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/__main__.py` & `mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppIntegrationsService 1.26.90\nVersion:        "
-        " 1.26.90\nBuilder version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.AppIntegrationsService 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.90")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/client.py` & `mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/client.pyi` & `mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/literals.py` & `mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
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
@@ -81,14 +82,15 @@
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
@@ -186,14 +188,15 @@
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
@@ -229,14 +232,15 @@
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
@@ -255,16 +259,19 @@
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
@@ -348,15 +355,17 @@
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
```

### Comparing `mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/literals.pyi` & `mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
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
@@ -79,14 +80,15 @@
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
@@ -184,14 +186,15 @@
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
@@ -227,14 +230,15 @@
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
@@ -253,16 +257,19 @@
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
@@ -346,15 +353,17 @@
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
```

### Comparing `mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/type_defs.py` & `mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,37 +19,37 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "FileConfigurationTypeDef",
     "ScheduleConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
     "EventFilterTypeDef",
+    "CreateEventIntegrationResponseTypeDef",
     "DataIntegrationAssociationSummaryTypeDef",
     "DataIntegrationSummaryTypeDef",
     "DeleteDataIntegrationRequestRequestTypeDef",
     "DeleteEventIntegrationRequestRequestTypeDef",
     "EventIntegrationAssociationTypeDef",
     "GetDataIntegrationRequestRequestTypeDef",
     "GetEventIntegrationRequestRequestTypeDef",
     "ListDataIntegrationAssociationsRequestRequestTypeDef",
     "ListDataIntegrationsRequestRequestTypeDef",
     "ListEventIntegrationAssociationsRequestRequestTypeDef",
     "ListEventIntegrationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDataIntegrationRequestRequestTypeDef",
     "UpdateEventIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationResponseTypeDef",
-    "CreateEventIntegrationResponseTypeDef",
     "GetDataIntegrationResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "CreateEventIntegrationRequestRequestTypeDef",
     "EventIntegrationTypeDef",
     "GetEventIntegrationResponseTypeDef",
     "ListDataIntegrationAssociationsResponseTypeDef",
     "ListDataIntegrationsResponseTypeDef",
     "ListEventIntegrationAssociationsResponseTypeDef",
     "ListEventIntegrationsResponseTypeDef",
@@ -94,29 +94,26 @@
 
 class ScheduleConfigurationTypeDef(
     _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EventFilterTypeDef = TypedDict(
+    "EventFilterTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Source": str,
     },
 )
 
-EventFilterTypeDef = TypedDict(
-    "EventFilterTypeDef",
+CreateEventIntegrationResponseTypeDef = TypedDict(
+    "CreateEventIntegrationResponseTypeDef",
     {
-        "Source": str,
+        "EventIntegrationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataIntegrationAssociationSummaryTypeDef = TypedDict(
     "DataIntegrationAssociationSummaryTypeDef",
     {
         "DataIntegrationAssociationArn": str,
@@ -244,14 +241,33 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -348,23 +364,15 @@
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
         "ClientToken": str,
         "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEventIntegrationResponseTypeDef = TypedDict(
-    "CreateEventIntegrationResponseTypeDef",
-    {
-        "EventIntegrationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDataIntegrationResponseTypeDef = TypedDict(
     "GetDataIntegrationResponseTypeDef",
     {
         "Arn": str,
@@ -373,23 +381,15 @@
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
         "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
@@ -433,46 +433,46 @@
     {
         "Name": str,
         "Description": str,
         "EventIntegrationArn": str,
         "EventBridgeBus": str,
         "EventFilter": EventFilterTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDataIntegrationAssociationsResponseTypeDef = TypedDict(
     "ListDataIntegrationAssociationsResponseTypeDef",
     {
         "DataIntegrationAssociations": List[DataIntegrationAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDataIntegrationsResponseTypeDef = TypedDict(
     "ListDataIntegrationsResponseTypeDef",
     {
         "DataIntegrations": List[DataIntegrationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventIntegrationAssociationsResponseTypeDef = TypedDict(
     "ListEventIntegrationAssociationsResponseTypeDef",
     {
         "EventIntegrationAssociations": List[EventIntegrationAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventIntegrationsResponseTypeDef = TypedDict(
     "ListEventIntegrationsResponseTypeDef",
     {
         "EventIntegrations": List[EventIntegrationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations/type_defs.pyi` & `mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,37 +18,37 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "FileConfigurationTypeDef",
     "ScheduleConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
     "EventFilterTypeDef",
+    "CreateEventIntegrationResponseTypeDef",
     "DataIntegrationAssociationSummaryTypeDef",
     "DataIntegrationSummaryTypeDef",
     "DeleteDataIntegrationRequestRequestTypeDef",
     "DeleteEventIntegrationRequestRequestTypeDef",
     "EventIntegrationAssociationTypeDef",
     "GetDataIntegrationRequestRequestTypeDef",
     "GetEventIntegrationRequestRequestTypeDef",
     "ListDataIntegrationAssociationsRequestRequestTypeDef",
     "ListDataIntegrationsRequestRequestTypeDef",
     "ListEventIntegrationAssociationsRequestRequestTypeDef",
     "ListEventIntegrationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDataIntegrationRequestRequestTypeDef",
     "UpdateEventIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationResponseTypeDef",
-    "CreateEventIntegrationResponseTypeDef",
     "GetDataIntegrationResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "CreateEventIntegrationRequestRequestTypeDef",
     "EventIntegrationTypeDef",
     "GetEventIntegrationResponseTypeDef",
     "ListDataIntegrationAssociationsResponseTypeDef",
     "ListDataIntegrationsResponseTypeDef",
     "ListEventIntegrationAssociationsResponseTypeDef",
     "ListEventIntegrationsResponseTypeDef",
@@ -89,29 +89,26 @@
 )
 
 class ScheduleConfigurationTypeDef(
     _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EventFilterTypeDef = TypedDict(
+    "EventFilterTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Source": str,
     },
 )
 
-EventFilterTypeDef = TypedDict(
-    "EventFilterTypeDef",
+CreateEventIntegrationResponseTypeDef = TypedDict(
+    "CreateEventIntegrationResponseTypeDef",
     {
-        "Source": str,
+        "EventIntegrationArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataIntegrationAssociationSummaryTypeDef = TypedDict(
     "DataIntegrationAssociationSummaryTypeDef",
     {
         "DataIntegrationAssociationArn": str,
@@ -235,14 +232,33 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -333,23 +349,15 @@
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
         "ClientToken": str,
         "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEventIntegrationResponseTypeDef = TypedDict(
-    "CreateEventIntegrationResponseTypeDef",
-    {
-        "EventIntegrationArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDataIntegrationResponseTypeDef = TypedDict(
     "GetDataIntegrationResponseTypeDef",
     {
         "Arn": str,
@@ -358,23 +366,15 @@
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
         "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
@@ -416,46 +416,46 @@
     {
         "Name": str,
         "Description": str,
         "EventIntegrationArn": str,
         "EventBridgeBus": str,
         "EventFilter": EventFilterTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDataIntegrationAssociationsResponseTypeDef = TypedDict(
     "ListDataIntegrationAssociationsResponseTypeDef",
     {
         "DataIntegrationAssociations": List[DataIntegrationAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDataIntegrationsResponseTypeDef = TypedDict(
     "ListDataIntegrationsResponseTypeDef",
     {
         "DataIntegrations": List[DataIntegrationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventIntegrationAssociationsResponseTypeDef = TypedDict(
     "ListEventIntegrationAssociationsResponseTypeDef",
     {
         "EventIntegrationAssociations": List[EventIntegrationAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventIntegrationsResponseTypeDef = TypedDict(
     "ListEventIntegrationsResponseTypeDef",
     {
         "EventIntegrations": List[EventIntegrationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations.egg-info/PKG-INFO` & `mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appintegrations
-Version: 1.26.90
-Summary: Type annotations for boto3.AppIntegrationsService 1.26.90 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.AppIntegrationsService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-appintegrations"></a>
 
 # mypy-boto3-appintegrations
 
 [![PyPI - mypy-boto3-appintegrations](https://img.shields.io/pypi/v/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appintegrations?color=blue)](https://pypistats.org/packages/mypy-boto3-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppIntegrationsService 1.26.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[boto3.AppIntegrationsService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appintegrations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,37 +299,37 @@
 `mypy_boto3_appintegrations.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appintegrations.type_defs import (
     FileConfigurationTypeDef,
     ScheduleConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     EventFilterTypeDef,
+    CreateEventIntegrationResponseTypeDef,
     DataIntegrationAssociationSummaryTypeDef,
     DataIntegrationSummaryTypeDef,
     DeleteDataIntegrationRequestRequestTypeDef,
     DeleteEventIntegrationRequestRequestTypeDef,
     EventIntegrationAssociationTypeDef,
     GetDataIntegrationRequestRequestTypeDef,
     GetEventIntegrationRequestRequestTypeDef,
     ListDataIntegrationAssociationsRequestRequestTypeDef,
     ListDataIntegrationsRequestRequestTypeDef,
     ListEventIntegrationAssociationsRequestRequestTypeDef,
     ListEventIntegrationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDataIntegrationRequestRequestTypeDef,
     UpdateEventIntegrationRequestRequestTypeDef,
     CreateDataIntegrationRequestRequestTypeDef,
     CreateDataIntegrationResponseTypeDef,
-    CreateEventIntegrationResponseTypeDef,
     GetDataIntegrationResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateEventIntegrationRequestRequestTypeDef,
     EventIntegrationTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
@@ -343,42 +343,42 @@
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

### Comparing `mypy-boto3-appintegrations-1.26.90/mypy_boto3_appintegrations.egg-info/SOURCES.txt` & `mypy-boto3-appintegrations-1.27.0/mypy_boto3_appintegrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.26.90/setup.py` & `mypy-boto3-appintegrations-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-appintegrations.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appintegrations",
-    version="1.26.90",
+    version="1.27.0",
     packages=["mypy_boto3_appintegrations"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppIntegrationsService 1.26.90 service generated with"
-        " mypy-boto3-builder 7.13.0"
+        "Type annotations for boto3.AppIntegrationsService 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/",
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


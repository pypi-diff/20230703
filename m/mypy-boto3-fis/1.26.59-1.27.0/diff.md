# Comparing `tmp/mypy-boto3-fis-1.26.59.tar.gz` & `tmp/mypy-boto3-fis-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fis-1.26.59.tar", last modified: Fri Jan 27 20:32:50 2023, max compression
+gzip compressed data, was "mypy-boto3-fis-1.27.0.tar", last modified: Mon Jul  3 19:50:47 2023, max compression
```

## Comparing `mypy-boto3-fis-1.26.59.tar` & `mypy-boto3-fis-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.584096 mypy-boto3-fis-1.26.59/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-27 20:32:05.000000 mypy-boto3-fis-1.26.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14518 2023-01-27 20:32:50.576096 mypy-boto3-fis-1.26.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-01-27 20:32:05.000000 mypy-boto3-fis-1.26.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.576096 mypy-boto3-fis-1.26.59/mypy_boto3_fis/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-01-27 20:32:05.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-01-27 20:32:05.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-01-27 20:32:05.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-01-27 20:32:06.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-01-27 20:32:05.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-01-27 20:32:06.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-01-27 20:32:06.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:05.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-01-27 20:32:07.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23848 2023-01-27 20:32:06.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-27 20:32:05.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.576096 mypy-boto3-fis-1.26.59/mypy_boto3_fis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14518 2023-01-27 20:32:50.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-01-27 20:32:50.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:50.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:50.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-27 20:32:50.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-27 20:32:50.000000 mypy-boto3-fis-1.26.59/mypy_boto3_fis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 20:32:50.584096 mypy-boto3-fis-1.26.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-01-27 20:32:05.000000 mypy-boto3-fis-1.26.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.055261 mypy-boto3-fis-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:49.000000 mypy-boto3-fis-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14490 2023-07-03 19:50:47.055261 mypy-boto3-fis-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-07-03 19:37:49.000000 mypy-boto3-fis-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.051261 mypy-boto3-fis-1.27.0/mypy_boto3_fis/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-03 19:37:49.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-03 19:37:49.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:37:49.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-07-03 19:37:50.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-07-03 19:37:50.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-07-03 19:37:50.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-07-03 19:37:50.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:49.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23899 2023-07-03 19:37:51.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23876 2023-07-03 19:37:50.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:49.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.055261 mypy-boto3-fis-1.27.0/mypy_boto3_fis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14490 2023-07-03 19:50:46.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-03 19:50:46.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:46.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:46.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:46.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:46.000000 mypy-boto3-fis-1.27.0/mypy_boto3_fis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:47.055261 mypy-boto3-fis-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:37:49.000000 mypy-boto3-fis-1.27.0/setup.py
```

### Comparing `mypy-boto3-fis-1.26.59/LICENSE` & `mypy-boto3-fis-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-fis-1.26.59/PKG-INFO` & `mypy-boto3-fis-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fis
-Version: 1.26.59
-Summary: Type annotations for boto3.FIS 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.FIS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-fis"></a>
 
 # mypy-boto3-fis
 
 [![PyPI - mypy-boto3-fis](https://img.shields.io/pypi/v/mypy-boto3-fis.svg?color=blue)](https://pypi.org/project/mypy-boto3-fis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fis.svg?color=blue)](https://pypi.org/project/mypy-boto3-fis)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fis?color=blue)](https://pypistats.org/packages/mypy-boto3-fis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FIS 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
+[boto3.FIS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
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
 [mypy-boto3-fis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,15 +302,14 @@
 from mypy_boto3_fis.type_defs import (
     ActionParameterTypeDef,
     ActionTargetTypeDef,
     CreateExperimentTemplateActionInputTypeDef,
     ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef,
     ExperimentTemplateS3LogConfigurationInputTypeDef,
     CreateExperimentTemplateStopConditionInputTypeDef,
-    ResponseMetadataTypeDef,
     ExperimentTemplateTargetInputFilterTypeDef,
     DeleteExperimentTemplateRequestRequestTypeDef,
     ExperimentActionStateTypeDef,
     ExperimentCloudWatchLogsLogConfigurationTypeDef,
     ExperimentS3LogConfigurationTypeDef,
     ExperimentStateTypeDef,
     ExperimentStopConditionTypeDef,
@@ -325,28 +324,29 @@
     GetExperimentRequestRequestTypeDef,
     GetExperimentTemplateRequestRequestTypeDef,
     GetTargetResourceTypeRequestRequestTypeDef,
     ListActionsRequestRequestTypeDef,
     ListExperimentTemplatesRequestRequestTypeDef,
     ListExperimentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTargetResourceTypesRequestRequestTypeDef,
     TargetResourceTypeSummaryTypeDef,
+    ResponseMetadataTypeDef,
     StartExperimentRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TargetResourceTypeParameterTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateExperimentTemplateActionInputItemTypeDef,
     UpdateExperimentTemplateStopConditionInputTypeDef,
     ActionSummaryTypeDef,
     ActionTypeDef,
     CreateExperimentTemplateLogConfigurationInputTypeDef,
     UpdateExperimentTemplateLogConfigurationInputTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateExperimentTemplateTargetInputTypeDef,
     UpdateExperimentTemplateTargetInputTypeDef,
     ExperimentActionTypeDef,
     ExperimentLogConfigurationTypeDef,
     ExperimentSummaryTypeDef,
     ExperimentTargetTypeDef,
     ExperimentTemplateLogConfigurationTypeDef,
@@ -379,42 +379,42 @@
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

### Comparing `mypy-boto3-fis-1.26.59/README.md` & `mypy-boto3-fis-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-fis"></a>
 
 # mypy-boto3-fis
 
 [![PyPI - mypy-boto3-fis](https://img.shields.io/pypi/v/mypy-boto3-fis.svg?color=blue)](https://pypi.org/project/mypy-boto3-fis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fis.svg?color=blue)](https://pypi.org/project/mypy-boto3-fis)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fis?color=blue)](https://pypistats.org/packages/mypy-boto3-fis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FIS 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
+[boto3.FIS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
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
 [mypy-boto3-fis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -270,15 +270,14 @@
 from mypy_boto3_fis.type_defs import (
     ActionParameterTypeDef,
     ActionTargetTypeDef,
     CreateExperimentTemplateActionInputTypeDef,
     ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef,
     ExperimentTemplateS3LogConfigurationInputTypeDef,
     CreateExperimentTemplateStopConditionInputTypeDef,
-    ResponseMetadataTypeDef,
     ExperimentTemplateTargetInputFilterTypeDef,
     DeleteExperimentTemplateRequestRequestTypeDef,
     ExperimentActionStateTypeDef,
     ExperimentCloudWatchLogsLogConfigurationTypeDef,
     ExperimentS3LogConfigurationTypeDef,
     ExperimentStateTypeDef,
     ExperimentStopConditionTypeDef,
@@ -293,28 +292,29 @@
     GetExperimentRequestRequestTypeDef,
     GetExperimentTemplateRequestRequestTypeDef,
     GetTargetResourceTypeRequestRequestTypeDef,
     ListActionsRequestRequestTypeDef,
     ListExperimentTemplatesRequestRequestTypeDef,
     ListExperimentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTargetResourceTypesRequestRequestTypeDef,
     TargetResourceTypeSummaryTypeDef,
+    ResponseMetadataTypeDef,
     StartExperimentRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TargetResourceTypeParameterTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateExperimentTemplateActionInputItemTypeDef,
     UpdateExperimentTemplateStopConditionInputTypeDef,
     ActionSummaryTypeDef,
     ActionTypeDef,
     CreateExperimentTemplateLogConfigurationInputTypeDef,
     UpdateExperimentTemplateLogConfigurationInputTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateExperimentTemplateTargetInputTypeDef,
     UpdateExperimentTemplateTargetInputTypeDef,
     ExperimentActionTypeDef,
     ExperimentLogConfigurationTypeDef,
     ExperimentSummaryTypeDef,
     ExperimentTargetTypeDef,
     ExperimentTemplateLogConfigurationTypeDef,
@@ -347,42 +347,42 @@
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

### Comparing `mypy-boto3-fis-1.26.59/mypy_boto3_fis/__main__.py` & `mypy-boto3-fis-1.27.0/mypy_boto3_fis/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FIS 1.26.59\nVersion:         1.26.59\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.FIS 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.59")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-fis-1.26.59/mypy_boto3_fis/client.py` & `mypy-boto3-fis-1.27.0/mypy_boto3_fis/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.26.59/mypy_boto3_fis/client.pyi` & `mypy-boto3-fis-1.27.0/mypy_boto3_fis/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.26.59/mypy_boto3_fis/literals.py` & `mypy-boto3-fis-1.27.0/mypy_boto3_fis/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
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
@@ -85,21 +86,23 @@
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
@@ -178,14 +181,15 @@
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
@@ -196,14 +200,15 @@
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
@@ -239,14 +244,15 @@
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
@@ -265,16 +271,19 @@
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
@@ -354,18 +363,21 @@
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

### Comparing `mypy-boto3-fis-1.26.59/mypy_boto3_fis/literals.pyi` & `mypy-boto3-fis-1.27.0/mypy_boto3_fis/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
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
@@ -83,21 +84,23 @@
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
@@ -176,14 +179,15 @@
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
@@ -194,14 +198,15 @@
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
@@ -237,14 +242,15 @@
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
@@ -263,16 +269,19 @@
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
@@ -352,18 +361,21 @@
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

### Comparing `mypy-boto3-fis-1.26.59/mypy_boto3_fis/type_defs.py` & `mypy-boto3-fis-1.27.0/mypy_boto3_fis/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 __all__ = (
     "ActionParameterTypeDef",
     "ActionTargetTypeDef",
     "CreateExperimentTemplateActionInputTypeDef",
     "ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef",
     "ExperimentTemplateS3LogConfigurationInputTypeDef",
     "CreateExperimentTemplateStopConditionInputTypeDef",
-    "ResponseMetadataTypeDef",
     "ExperimentTemplateTargetInputFilterTypeDef",
     "DeleteExperimentTemplateRequestRequestTypeDef",
     "ExperimentActionStateTypeDef",
     "ExperimentCloudWatchLogsLogConfigurationTypeDef",
     "ExperimentS3LogConfigurationTypeDef",
     "ExperimentStateTypeDef",
     "ExperimentStopConditionTypeDef",
@@ -49,28 +48,29 @@
     "GetExperimentRequestRequestTypeDef",
     "GetExperimentTemplateRequestRequestTypeDef",
     "GetTargetResourceTypeRequestRequestTypeDef",
     "ListActionsRequestRequestTypeDef",
     "ListExperimentTemplatesRequestRequestTypeDef",
     "ListExperimentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTargetResourceTypesRequestRequestTypeDef",
     "TargetResourceTypeSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "StartExperimentRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TargetResourceTypeParameterTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateExperimentTemplateActionInputItemTypeDef",
     "UpdateExperimentTemplateStopConditionInputTypeDef",
     "ActionSummaryTypeDef",
     "ActionTypeDef",
     "CreateExperimentTemplateLogConfigurationInputTypeDef",
     "UpdateExperimentTemplateLogConfigurationInputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "CreateExperimentTemplateTargetInputTypeDef",
     "UpdateExperimentTemplateTargetInputTypeDef",
     "ExperimentActionTypeDef",
     "ExperimentLogConfigurationTypeDef",
     "ExperimentSummaryTypeDef",
     "ExperimentTargetTypeDef",
     "ExperimentTemplateLogConfigurationTypeDef",
@@ -184,25 +184,14 @@
 class CreateExperimentTemplateStopConditionInputTypeDef(
     _RequiredCreateExperimentTemplateStopConditionInputTypeDef,
     _OptionalCreateExperimentTemplateStopConditionInputTypeDef,
 ):
     pass
 
 
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
 ExperimentTemplateTargetInputFilterTypeDef = TypedDict(
     "ExperimentTemplateTargetInputFilterTypeDef",
     {
         "path": str,
         "values": Sequence[str],
     },
 )
@@ -384,14 +373,22 @@
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
 ListTargetResourceTypesRequestRequestTypeDef = TypedDict(
     "ListTargetResourceTypesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -402,14 +399,25 @@
     {
         "resourceType": str,
         "description": str,
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
 _RequiredStartExperimentRequestRequestTypeDef = TypedDict(
     "_RequiredStartExperimentRequestRequestTypeDef",
     {
         "clientToken": str,
         "experimentTemplateId": str,
     },
 )
@@ -559,22 +567,14 @@
         "cloudWatchLogsConfiguration": ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef,
         "s3Configuration": ExperimentTemplateS3LogConfigurationInputTypeDef,
         "logSchemaVersion": int,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateExperimentTemplateTargetInputTypeDef = TypedDict(
     "_RequiredCreateExperimentTemplateTargetInputTypeDef",
     {
         "resourceType": str,
         "selectionMode": str,
     },
 )
@@ -684,15 +684,15 @@
 )
 
 ListExperimentTemplatesResponseTypeDef = TypedDict(
     "ListExperimentTemplatesResponseTypeDef",
     {
         "experimentTemplates": List[ExperimentTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExperimentTemplateTargetTypeDef = TypedDict(
     "ExperimentTemplateTargetTypeDef",
     {
         "resourceType": str,
@@ -706,15 +706,15 @@
 )
 
 ListTargetResourceTypesResponseTypeDef = TypedDict(
     "ListTargetResourceTypesResponseTypeDef",
     {
         "targetResourceTypes": List[TargetResourceTypeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TargetResourceTypeTypeDef = TypedDict(
     "TargetResourceTypeTypeDef",
     {
         "resourceType": str,
@@ -725,23 +725,23 @@
 )
 
 ListActionsResponseTypeDef = TypedDict(
     "ListActionsResponseTypeDef",
     {
         "actions": List[ActionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetActionResponseTypeDef = TypedDict(
     "GetActionResponseTypeDef",
     {
         "action": ActionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateExperimentTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperimentTemplateRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -797,15 +797,15 @@
 
 
 ListExperimentsResponseTypeDef = TypedDict(
     "ListExperimentsResponseTypeDef",
     {
         "experiments": List[ExperimentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExperimentTypeDef = TypedDict(
     "ExperimentTypeDef",
     {
         "id": str,
@@ -841,66 +841,66 @@
     total=False,
 )
 
 GetTargetResourceTypeResponseTypeDef = TypedDict(
     "GetTargetResourceTypeResponseTypeDef",
     {
         "targetResourceType": TargetResourceTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExperimentResponseTypeDef = TypedDict(
     "GetExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartExperimentResponseTypeDef = TypedDict(
     "StartExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopExperimentResponseTypeDef = TypedDict(
     "StopExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateExperimentTemplateResponseTypeDef = TypedDict(
     "CreateExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteExperimentTemplateResponseTypeDef = TypedDict(
     "DeleteExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExperimentTemplateResponseTypeDef = TypedDict(
     "GetExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateExperimentTemplateResponseTypeDef = TypedDict(
     "UpdateExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-fis-1.26.59/mypy_boto3_fis/type_defs.pyi` & `mypy-boto3-fis-1.27.0/mypy_boto3_fis/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 __all__ = (
     "ActionParameterTypeDef",
     "ActionTargetTypeDef",
     "CreateExperimentTemplateActionInputTypeDef",
     "ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef",
     "ExperimentTemplateS3LogConfigurationInputTypeDef",
     "CreateExperimentTemplateStopConditionInputTypeDef",
-    "ResponseMetadataTypeDef",
     "ExperimentTemplateTargetInputFilterTypeDef",
     "DeleteExperimentTemplateRequestRequestTypeDef",
     "ExperimentActionStateTypeDef",
     "ExperimentCloudWatchLogsLogConfigurationTypeDef",
     "ExperimentS3LogConfigurationTypeDef",
     "ExperimentStateTypeDef",
     "ExperimentStopConditionTypeDef",
@@ -48,28 +47,29 @@
     "GetExperimentRequestRequestTypeDef",
     "GetExperimentTemplateRequestRequestTypeDef",
     "GetTargetResourceTypeRequestRequestTypeDef",
     "ListActionsRequestRequestTypeDef",
     "ListExperimentTemplatesRequestRequestTypeDef",
     "ListExperimentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTargetResourceTypesRequestRequestTypeDef",
     "TargetResourceTypeSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "StartExperimentRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TargetResourceTypeParameterTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateExperimentTemplateActionInputItemTypeDef",
     "UpdateExperimentTemplateStopConditionInputTypeDef",
     "ActionSummaryTypeDef",
     "ActionTypeDef",
     "CreateExperimentTemplateLogConfigurationInputTypeDef",
     "UpdateExperimentTemplateLogConfigurationInputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "CreateExperimentTemplateTargetInputTypeDef",
     "UpdateExperimentTemplateTargetInputTypeDef",
     "ExperimentActionTypeDef",
     "ExperimentLogConfigurationTypeDef",
     "ExperimentSummaryTypeDef",
     "ExperimentTargetTypeDef",
     "ExperimentTemplateLogConfigurationTypeDef",
@@ -177,25 +177,14 @@
 
 class CreateExperimentTemplateStopConditionInputTypeDef(
     _RequiredCreateExperimentTemplateStopConditionInputTypeDef,
     _OptionalCreateExperimentTemplateStopConditionInputTypeDef,
 ):
     pass
 
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
 ExperimentTemplateTargetInputFilterTypeDef = TypedDict(
     "ExperimentTemplateTargetInputFilterTypeDef",
     {
         "path": str,
         "values": Sequence[str],
     },
 )
@@ -377,14 +366,22 @@
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
 ListTargetResourceTypesRequestRequestTypeDef = TypedDict(
     "ListTargetResourceTypesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -395,14 +392,25 @@
     {
         "resourceType": str,
         "description": str,
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
 _RequiredStartExperimentRequestRequestTypeDef = TypedDict(
     "_RequiredStartExperimentRequestRequestTypeDef",
     {
         "clientToken": str,
         "experimentTemplateId": str,
     },
 )
@@ -544,22 +552,14 @@
         "cloudWatchLogsConfiguration": ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef,
         "s3Configuration": ExperimentTemplateS3LogConfigurationInputTypeDef,
         "logSchemaVersion": int,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateExperimentTemplateTargetInputTypeDef = TypedDict(
     "_RequiredCreateExperimentTemplateTargetInputTypeDef",
     {
         "resourceType": str,
         "selectionMode": str,
     },
 )
@@ -665,15 +665,15 @@
 )
 
 ListExperimentTemplatesResponseTypeDef = TypedDict(
     "ListExperimentTemplatesResponseTypeDef",
     {
         "experimentTemplates": List[ExperimentTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExperimentTemplateTargetTypeDef = TypedDict(
     "ExperimentTemplateTargetTypeDef",
     {
         "resourceType": str,
@@ -687,15 +687,15 @@
 )
 
 ListTargetResourceTypesResponseTypeDef = TypedDict(
     "ListTargetResourceTypesResponseTypeDef",
     {
         "targetResourceTypes": List[TargetResourceTypeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TargetResourceTypeTypeDef = TypedDict(
     "TargetResourceTypeTypeDef",
     {
         "resourceType": str,
@@ -706,23 +706,23 @@
 )
 
 ListActionsResponseTypeDef = TypedDict(
     "ListActionsResponseTypeDef",
     {
         "actions": List[ActionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetActionResponseTypeDef = TypedDict(
     "GetActionResponseTypeDef",
     {
         "action": ActionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateExperimentTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperimentTemplateRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -774,15 +774,15 @@
     pass
 
 ListExperimentsResponseTypeDef = TypedDict(
     "ListExperimentsResponseTypeDef",
     {
         "experiments": List[ExperimentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExperimentTypeDef = TypedDict(
     "ExperimentTypeDef",
     {
         "id": str,
@@ -818,66 +818,66 @@
     total=False,
 )
 
 GetTargetResourceTypeResponseTypeDef = TypedDict(
     "GetTargetResourceTypeResponseTypeDef",
     {
         "targetResourceType": TargetResourceTypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExperimentResponseTypeDef = TypedDict(
     "GetExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartExperimentResponseTypeDef = TypedDict(
     "StartExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopExperimentResponseTypeDef = TypedDict(
     "StopExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateExperimentTemplateResponseTypeDef = TypedDict(
     "CreateExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteExperimentTemplateResponseTypeDef = TypedDict(
     "DeleteExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExperimentTemplateResponseTypeDef = TypedDict(
     "GetExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateExperimentTemplateResponseTypeDef = TypedDict(
     "UpdateExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-fis-1.26.59/mypy_boto3_fis.egg-info/PKG-INFO` & `mypy-boto3-fis-1.27.0/mypy_boto3_fis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fis
-Version: 1.26.59
-Summary: Type annotations for boto3.FIS 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.FIS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-fis"></a>
 
 # mypy-boto3-fis
 
 [![PyPI - mypy-boto3-fis](https://img.shields.io/pypi/v/mypy-boto3-fis.svg?color=blue)](https://pypi.org/project/mypy-boto3-fis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fis.svg?color=blue)](https://pypi.org/project/mypy-boto3-fis)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fis?color=blue)](https://pypistats.org/packages/mypy-boto3-fis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FIS 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
+[boto3.FIS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
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
 [mypy-boto3-fis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,15 +302,14 @@
 from mypy_boto3_fis.type_defs import (
     ActionParameterTypeDef,
     ActionTargetTypeDef,
     CreateExperimentTemplateActionInputTypeDef,
     ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef,
     ExperimentTemplateS3LogConfigurationInputTypeDef,
     CreateExperimentTemplateStopConditionInputTypeDef,
-    ResponseMetadataTypeDef,
     ExperimentTemplateTargetInputFilterTypeDef,
     DeleteExperimentTemplateRequestRequestTypeDef,
     ExperimentActionStateTypeDef,
     ExperimentCloudWatchLogsLogConfigurationTypeDef,
     ExperimentS3LogConfigurationTypeDef,
     ExperimentStateTypeDef,
     ExperimentStopConditionTypeDef,
@@ -325,28 +324,29 @@
     GetExperimentRequestRequestTypeDef,
     GetExperimentTemplateRequestRequestTypeDef,
     GetTargetResourceTypeRequestRequestTypeDef,
     ListActionsRequestRequestTypeDef,
     ListExperimentTemplatesRequestRequestTypeDef,
     ListExperimentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTargetResourceTypesRequestRequestTypeDef,
     TargetResourceTypeSummaryTypeDef,
+    ResponseMetadataTypeDef,
     StartExperimentRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TargetResourceTypeParameterTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateExperimentTemplateActionInputItemTypeDef,
     UpdateExperimentTemplateStopConditionInputTypeDef,
     ActionSummaryTypeDef,
     ActionTypeDef,
     CreateExperimentTemplateLogConfigurationInputTypeDef,
     UpdateExperimentTemplateLogConfigurationInputTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateExperimentTemplateTargetInputTypeDef,
     UpdateExperimentTemplateTargetInputTypeDef,
     ExperimentActionTypeDef,
     ExperimentLogConfigurationTypeDef,
     ExperimentSummaryTypeDef,
     ExperimentTargetTypeDef,
     ExperimentTemplateLogConfigurationTypeDef,
@@ -379,42 +379,42 @@
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

### Comparing `mypy-boto3-fis-1.26.59/mypy_boto3_fis.egg-info/SOURCES.txt` & `mypy-boto3-fis-1.27.0/mypy_boto3_fis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.26.59/setup.py` & `mypy-boto3-fis-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-fis.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-fis",
-    version="1.26.59",
+    version="1.27.0",
     packages=["mypy_boto3_fis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FIS 1.26.59 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.FIS 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/",
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


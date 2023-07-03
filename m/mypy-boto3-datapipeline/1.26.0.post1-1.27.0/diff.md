# Comparing `tmp/mypy-boto3-datapipeline-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-datapipeline-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-datapipeline-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:18 2022, max compression
+gzip compressed data, was "mypy-boto3-datapipeline-1.27.0.tar", last modified: Mon Jul  3 19:50:38 2023, max compression
```

## Comparing `mypy-boto3-datapipeline-1.26.0.post1.tar` & `mypy-boto3-datapipeline-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:18.452821 mypy-boto3-datapipeline-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:32:38.000000 mypy-boto3-datapipeline-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14916 2022-11-01 21:43:18.452821 mypy-boto3-datapipeline-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13455 2022-11-01 21:32:38.000000 mypy-boto3-datapipeline-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:18.452821 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-11-01 21:32:38.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-11-01 21:32:38.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-01 21:32:38.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16581 2022-11-01 21:32:38.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    16552 2022-11-01 21:32:38.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7521 2022-11-01 21:32:39.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7519 2022-11-01 21:32:38.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4174 2022-11-01 21:32:38.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4169 2022-11-01 21:32:38.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:32:38.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    17873 2022-11-01 21:32:39.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    17841 2022-11-01 21:32:39.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:32:38.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:18.452821 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14916 2022-11-01 21:43:18.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-11-01 21:43:18.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:18.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:18.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:18.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-01 21:43:18.000000 mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:18.452821 mypy-boto3-datapipeline-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-11-01 21:32:38.000000 mypy-boto3-datapipeline-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.239102 mypy-boto3-datapipeline-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:18.000000 mypy-boto3-datapipeline-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-07-03 19:50:38.239102 mypy-boto3-datapipeline-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13438 2023-07-03 19:35:18.000000 mypy-boto3-datapipeline-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.235102 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-03 19:35:18.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-03 19:35:18.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:35:18.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-07-03 19:35:18.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-07-03 19:35:18.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-07-03 19:35:19.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-03 19:35:19.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-03 19:35:18.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-03 19:35:18.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:18.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-07-03 19:35:19.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17873 2023-07-03 19:35:19.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:18.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:38.239102 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-07-03 19:50:38.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:50:38.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:38.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:38.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:38.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:38.000000 mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:38.239102 mypy-boto3-datapipeline-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:35:18.000000 mypy-boto3-datapipeline-1.27.0/setup.py
```

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/LICENSE` & `mypy-boto3-datapipeline-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/PKG-INFO` & `mypy-boto3-datapipeline-1.27.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datapipeline
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.DataPipeline 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.DataPipeline 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/
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
 
 <a id="mypy-boto3-datapipeline"></a>
 
 # mypy-boto3-datapipeline
 
 [![PyPI - mypy-boto3-datapipeline](https://img.shields.io/pypi/v/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-datapipeline?color=blue)](https://pypistats.org/packages/mypy-boto3-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataPipeline 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[boto3.DataPipeline 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
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
 [mypy-boto3-datapipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,45 +331,45 @@
 `mypy_boto3_datapipeline.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_datapipeline.type_defs import (
     ParameterValueTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreatePipelineOutputTypeDef,
     DeactivatePipelineInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeObjectsInputDescribeObjectsPaginateTypeDef,
     DescribeObjectsInputRequestTypeDef,
     DescribePipelinesInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EvaluateExpressionInputRequestTypeDef,
+    EvaluateExpressionOutputTypeDef,
     FieldTypeDef,
     GetPipelineDefinitionInputRequestTypeDef,
     InstanceIdentityTypeDef,
+    ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineIdNameTypeDef,
     OperatorTypeDef,
+    PaginatorConfigTypeDef,
     ParameterAttributeTypeDef,
     ValidationErrorTypeDef,
     ValidationWarningTypeDef,
+    QueryObjectsOutputTypeDef,
     RemoveTagsInputRequestTypeDef,
+    ReportTaskProgressOutputTypeDef,
     ReportTaskRunnerHeartbeatInputRequestTypeDef,
+    ReportTaskRunnerHeartbeatOutputTypeDef,
+    ResponseMetadataTypeDef,
     SetStatusInputRequestTypeDef,
     SetTaskStatusInputRequestTypeDef,
     ActivatePipelineInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
     CreatePipelineInputRequestTypeDef,
-    CreatePipelineOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EvaluateExpressionOutputTypeDef,
-    QueryObjectsOutputTypeDef,
-    ReportTaskProgressOutputTypeDef,
-    ReportTaskRunnerHeartbeatOutputTypeDef,
-    DescribeObjectsInputDescribeObjectsPaginateTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
     PipelineDescriptionTypeDef,
     PipelineObjectTypeDef,
     ReportTaskProgressInputRequestTypeDef,
     PollForTaskInputRequestTypeDef,
     ListPipelinesOutputTypeDef,
     SelectorTypeDef,
     ParameterObjectTypeDef,
@@ -394,42 +395,42 @@
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

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/README.md` & `mypy-boto3-datapipeline-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-datapipeline"></a>
 
 # mypy-boto3-datapipeline
 
 [![PyPI - mypy-boto3-datapipeline](https://img.shields.io/pypi/v/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-datapipeline?color=blue)](https://pypistats.org/packages/mypy-boto3-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataPipeline 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[boto3.DataPipeline 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
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
 [mypy-boto3-datapipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,45 +299,45 @@
 `mypy_boto3_datapipeline.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_datapipeline.type_defs import (
     ParameterValueTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreatePipelineOutputTypeDef,
     DeactivatePipelineInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeObjectsInputDescribeObjectsPaginateTypeDef,
     DescribeObjectsInputRequestTypeDef,
     DescribePipelinesInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EvaluateExpressionInputRequestTypeDef,
+    EvaluateExpressionOutputTypeDef,
     FieldTypeDef,
     GetPipelineDefinitionInputRequestTypeDef,
     InstanceIdentityTypeDef,
+    ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineIdNameTypeDef,
     OperatorTypeDef,
+    PaginatorConfigTypeDef,
     ParameterAttributeTypeDef,
     ValidationErrorTypeDef,
     ValidationWarningTypeDef,
+    QueryObjectsOutputTypeDef,
     RemoveTagsInputRequestTypeDef,
+    ReportTaskProgressOutputTypeDef,
     ReportTaskRunnerHeartbeatInputRequestTypeDef,
+    ReportTaskRunnerHeartbeatOutputTypeDef,
+    ResponseMetadataTypeDef,
     SetStatusInputRequestTypeDef,
     SetTaskStatusInputRequestTypeDef,
     ActivatePipelineInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
     CreatePipelineInputRequestTypeDef,
-    CreatePipelineOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EvaluateExpressionOutputTypeDef,
-    QueryObjectsOutputTypeDef,
-    ReportTaskProgressOutputTypeDef,
-    ReportTaskRunnerHeartbeatOutputTypeDef,
-    DescribeObjectsInputDescribeObjectsPaginateTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
     PipelineDescriptionTypeDef,
     PipelineObjectTypeDef,
     ReportTaskProgressInputRequestTypeDef,
     PollForTaskInputRequestTypeDef,
     ListPipelinesOutputTypeDef,
     SelectorTypeDef,
     ParameterObjectTypeDef,
@@ -363,42 +363,42 @@
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

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/__init__.py` & `mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/__init__.pyi` & `mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/__main__.py` & `mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataPipeline 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.DataPipeline 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline\nOther"
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

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/client.py` & `mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/client.pyi` & `mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/literals.py` & `mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/literals.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeObjectsPaginatorName",
     "ListPipelinesPaginatorName",
     "OperatorTypeType",
     "QueryObjectsPaginatorName",
     "TaskStatusType",
     "DataPipelineServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeObjectsPaginatorName = Literal["describe_objects"]
 ListPipelinesPaginatorName = Literal["list_pipelines"]
 OperatorTypeType = Literal["BETWEEN", "EQ", "GE", "LE", "REF_EQ"]
 QueryObjectsPaginatorName = Literal["query_objects"]
 TaskStatusType = Literal["FAILED", "FALSE", "FINISHED"]
 DataPipelineServiceName = Literal["datapipeline"]
 ServiceName = Literal[
@@ -50,23 +48,25 @@
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
@@ -76,30 +76,35 @@
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
@@ -125,14 +130,15 @@
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
@@ -177,51 +183,57 @@
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
@@ -234,14 +246,15 @@
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
@@ -253,28 +266,35 @@
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
@@ -283,14 +303,15 @@
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
@@ -301,55 +322,64 @@
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

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/literals.pyi` & `mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/literals.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DescribeObjectsPaginatorName",
     "ListPipelinesPaginatorName",
     "OperatorTypeType",
     "QueryObjectsPaginatorName",
     "TaskStatusType",
     "DataPipelineServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DescribeObjectsPaginatorName = Literal["describe_objects"]
 ListPipelinesPaginatorName = Literal["list_pipelines"]
 OperatorTypeType = Literal["BETWEEN", "EQ", "GE", "LE", "REF_EQ"]
 QueryObjectsPaginatorName = Literal["query_objects"]
 TaskStatusType = Literal["FAILED", "FALSE", "FINISHED"]
 DataPipelineServiceName = Literal["datapipeline"]
 ServiceName = Literal[
@@ -48,23 +50,25 @@
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
@@ -74,30 +78,35 @@
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
@@ -123,14 +132,15 @@
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
@@ -175,51 +185,57 @@
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
@@ -232,14 +248,15 @@
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
@@ -251,28 +268,35 @@
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
@@ -281,14 +305,15 @@
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
@@ -299,55 +324,64 @@
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

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/paginator.py` & `mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,30 +56,30 @@
 
     def paginate(
         self,
         *,
         pipelineId: str,
         objectIds: Sequence[str],
         evaluateExpressions: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.DescribeObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#describeobjectspaginator)
         """
 
 
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPipelinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#listpipelinespaginator)
         """
 
 
@@ -91,13 +91,13 @@
 
     def paginate(
         self,
         *,
         pipelineId: str,
         sphere: str,
         query: QueryTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[QueryObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.QueryObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#queryobjectspaginator)
         """
```

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/paginator.pyi` & `mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,29 +53,29 @@
 
     def paginate(
         self,
         *,
         pipelineId: str,
         objectIds: Sequence[str],
         evaluateExpressions: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.DescribeObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#describeobjectspaginator)
         """
 
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPipelinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#listpipelinespaginator)
         """
 
 class QueryObjectsPaginator(Paginator):
@@ -86,13 +86,13 @@
 
     def paginate(
         self,
         *,
         pipelineId: str,
         sphere: str,
         query: QueryTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[QueryObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.QueryObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#queryobjectspaginator)
         """
```

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/type_defs.py` & `mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,45 +22,45 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ParameterValueTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreatePipelineOutputTypeDef",
     "DeactivatePipelineInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeObjectsInputDescribeObjectsPaginateTypeDef",
     "DescribeObjectsInputRequestTypeDef",
     "DescribePipelinesInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EvaluateExpressionInputRequestTypeDef",
+    "EvaluateExpressionOutputTypeDef",
     "FieldTypeDef",
     "GetPipelineDefinitionInputRequestTypeDef",
     "InstanceIdentityTypeDef",
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListPipelinesInputRequestTypeDef",
     "PipelineIdNameTypeDef",
     "OperatorTypeDef",
+    "PaginatorConfigTypeDef",
     "ParameterAttributeTypeDef",
     "ValidationErrorTypeDef",
     "ValidationWarningTypeDef",
+    "QueryObjectsOutputTypeDef",
     "RemoveTagsInputRequestTypeDef",
+    "ReportTaskProgressOutputTypeDef",
     "ReportTaskRunnerHeartbeatInputRequestTypeDef",
+    "ReportTaskRunnerHeartbeatOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "SetStatusInputRequestTypeDef",
     "SetTaskStatusInputRequestTypeDef",
     "ActivatePipelineInputRequestTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreatePipelineInputRequestTypeDef",
-    "CreatePipelineOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EvaluateExpressionOutputTypeDef",
-    "QueryObjectsOutputTypeDef",
-    "ReportTaskProgressOutputTypeDef",
-    "ReportTaskRunnerHeartbeatOutputTypeDef",
-    "DescribeObjectsInputDescribeObjectsPaginateTypeDef",
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
     "PipelineDescriptionTypeDef",
     "PipelineObjectTypeDef",
     "ReportTaskProgressInputRequestTypeDef",
     "PollForTaskInputRequestTypeDef",
     "ListPipelinesOutputTypeDef",
     "SelectorTypeDef",
     "ParameterObjectTypeDef",
@@ -90,22 +90,19 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreatePipelineOutputTypeDef = TypedDict(
+    "CreatePipelineOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "pipelineId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeactivatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredDeactivatePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
@@ -129,24 +126,38 @@
 DeletePipelineInputRequestTypeDef = TypedDict(
     "DeletePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "pipelineId": str,
+        "objectIds": Sequence[str],
+    },
+)
+_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef",
+    {
+        "evaluateExpressions": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class DescribeObjectsInputDescribeObjectsPaginateTypeDef(
+    _RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef,
+    _OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeObjectsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeObjectsInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectIds": Sequence[str],
     },
 )
@@ -169,23 +180,38 @@
 DescribePipelinesInputRequestTypeDef = TypedDict(
     "DescribePipelinesInputRequestTypeDef",
     {
         "pipelineIds": Sequence[str],
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EvaluateExpressionInputRequestTypeDef = TypedDict(
     "EvaluateExpressionInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectId": str,
         "expression": str,
     },
 )
 
+EvaluateExpressionOutputTypeDef = TypedDict(
+    "EvaluateExpressionOutputTypeDef",
+    {
+        "evaluatedExpression": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFieldTypeDef = TypedDict(
     "_RequiredFieldTypeDef",
     {
         "key": str,
     },
 )
 _OptionalFieldTypeDef = TypedDict(
@@ -229,14 +255,22 @@
     {
         "document": str,
         "signature": str,
     },
     total=False,
 )
 
+ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPipelinesInputRequestTypeDef = TypedDict(
     "ListPipelinesInputRequestTypeDef",
     {
         "marker": str,
     },
     total=False,
 )
@@ -255,14 +289,24 @@
     {
         "type": OperatorTypeType,
         "values": Sequence[str],
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
 ParameterAttributeTypeDef = TypedDict(
     "ParameterAttributeTypeDef",
     {
         "key": str,
         "stringValue": str,
     },
 )
@@ -281,22 +325,40 @@
     {
         "id": str,
         "warnings": List[str],
     },
     total=False,
 )
 
+QueryObjectsOutputTypeDef = TypedDict(
+    "QueryObjectsOutputTypeDef",
+    {
+        "ids": List[str],
+        "marker": str,
+        "hasMoreResults": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveTagsInputRequestTypeDef = TypedDict(
     "RemoveTagsInputRequestTypeDef",
     {
         "pipelineId": str,
         "tagKeys": Sequence[str],
     },
 )
 
+ReportTaskProgressOutputTypeDef = TypedDict(
+    "ReportTaskProgressOutputTypeDef",
+    {
+        "canceled": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredReportTaskRunnerHeartbeatInputRequestTypeDef = TypedDict(
     "_RequiredReportTaskRunnerHeartbeatInputRequestTypeDef",
     {
         "taskrunnerId": str,
     },
 )
 _OptionalReportTaskRunnerHeartbeatInputRequestTypeDef = TypedDict(
@@ -312,14 +374,33 @@
 class ReportTaskRunnerHeartbeatInputRequestTypeDef(
     _RequiredReportTaskRunnerHeartbeatInputRequestTypeDef,
     _OptionalReportTaskRunnerHeartbeatInputRequestTypeDef,
 ):
     pass
 
 
+ReportTaskRunnerHeartbeatOutputTypeDef = TypedDict(
+    "ReportTaskRunnerHeartbeatOutputTypeDef",
+    {
+        "terminate": bool,
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
 SetStatusInputRequestTypeDef = TypedDict(
     "SetStatusInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectIds": Sequence[str],
         "status": str,
     },
@@ -398,95 +479,14 @@
 
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
 
-CreatePipelineOutputTypeDef = TypedDict(
-    "CreatePipelineOutputTypeDef",
-    {
-        "pipelineId": str,
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
-EvaluateExpressionOutputTypeDef = TypedDict(
-    "EvaluateExpressionOutputTypeDef",
-    {
-        "evaluatedExpression": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-QueryObjectsOutputTypeDef = TypedDict(
-    "QueryObjectsOutputTypeDef",
-    {
-        "ids": List[str],
-        "marker": str,
-        "hasMoreResults": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReportTaskProgressOutputTypeDef = TypedDict(
-    "ReportTaskProgressOutputTypeDef",
-    {
-        "canceled": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReportTaskRunnerHeartbeatOutputTypeDef = TypedDict(
-    "ReportTaskRunnerHeartbeatOutputTypeDef",
-    {
-        "terminate": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef",
-    {
-        "pipelineId": str,
-        "objectIds": Sequence[str],
-    },
-)
-_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef",
-    {
-        "evaluateExpressions": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeObjectsInputDescribeObjectsPaginateTypeDef(
-    _RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef,
-    _OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef,
-):
-    pass
-
-
-ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredPipelineDescriptionTypeDef = TypedDict(
     "_RequiredPipelineDescriptionTypeDef",
     {
         "pipelineId": str,
         "name": str,
         "fields": List[FieldTypeDef],
     },
@@ -561,15 +561,15 @@
 
 ListPipelinesOutputTypeDef = TypedDict(
     "ListPipelinesOutputTypeDef",
     {
         "pipelineIdList": List[PipelineIdNameTypeDef],
         "marker": str,
         "hasMoreResults": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SelectorTypeDef = TypedDict(
     "SelectorTypeDef",
     {
         "fieldName": str,
@@ -588,43 +588,43 @@
 
 PutPipelineDefinitionOutputTypeDef = TypedDict(
     "PutPipelineDefinitionOutputTypeDef",
     {
         "validationErrors": List[ValidationErrorTypeDef],
         "validationWarnings": List[ValidationWarningTypeDef],
         "errored": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ValidatePipelineDefinitionOutputTypeDef = TypedDict(
     "ValidatePipelineDefinitionOutputTypeDef",
     {
         "validationErrors": List[ValidationErrorTypeDef],
         "validationWarnings": List[ValidationWarningTypeDef],
         "errored": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePipelinesOutputTypeDef = TypedDict(
     "DescribePipelinesOutputTypeDef",
     {
         "pipelineDescriptionList": List[PipelineDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeObjectsOutputTypeDef = TypedDict(
     "DescribeObjectsOutputTypeDef",
     {
         "pipelineObjects": List[PipelineObjectTypeDef],
         "marker": str,
         "hasMoreResults": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TaskObjectTypeDef = TypedDict(
     "TaskObjectTypeDef",
     {
         "taskId": str,
@@ -645,15 +645,15 @@
 
 GetPipelineDefinitionOutputTypeDef = TypedDict(
     "GetPipelineDefinitionOutputTypeDef",
     {
         "pipelineObjects": List[PipelineObjectTypeDef],
         "parameterObjects": List[ParameterObjectTypeDef],
         "parameterValues": List[ParameterValueTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredPutPipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
@@ -701,30 +701,30 @@
     pass
 
 
 PollForTaskOutputTypeDef = TypedDict(
     "PollForTaskOutputTypeDef",
     {
         "taskObject": TaskObjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredQueryObjectsInputQueryObjectsPaginateTypeDef = TypedDict(
     "_RequiredQueryObjectsInputQueryObjectsPaginateTypeDef",
     {
         "pipelineId": str,
         "sphere": str,
     },
 )
 _OptionalQueryObjectsInputQueryObjectsPaginateTypeDef = TypedDict(
     "_OptionalQueryObjectsInputQueryObjectsPaginateTypeDef",
     {
         "query": QueryTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class QueryObjectsInputQueryObjectsPaginateTypeDef(
     _RequiredQueryObjectsInputQueryObjectsPaginateTypeDef,
```

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline/type_defs.pyi` & `mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -21,45 +21,45 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ParameterValueTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreatePipelineOutputTypeDef",
     "DeactivatePipelineInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeObjectsInputDescribeObjectsPaginateTypeDef",
     "DescribeObjectsInputRequestTypeDef",
     "DescribePipelinesInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EvaluateExpressionInputRequestTypeDef",
+    "EvaluateExpressionOutputTypeDef",
     "FieldTypeDef",
     "GetPipelineDefinitionInputRequestTypeDef",
     "InstanceIdentityTypeDef",
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListPipelinesInputRequestTypeDef",
     "PipelineIdNameTypeDef",
     "OperatorTypeDef",
+    "PaginatorConfigTypeDef",
     "ParameterAttributeTypeDef",
     "ValidationErrorTypeDef",
     "ValidationWarningTypeDef",
+    "QueryObjectsOutputTypeDef",
     "RemoveTagsInputRequestTypeDef",
+    "ReportTaskProgressOutputTypeDef",
     "ReportTaskRunnerHeartbeatInputRequestTypeDef",
+    "ReportTaskRunnerHeartbeatOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "SetStatusInputRequestTypeDef",
     "SetTaskStatusInputRequestTypeDef",
     "ActivatePipelineInputRequestTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreatePipelineInputRequestTypeDef",
-    "CreatePipelineOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EvaluateExpressionOutputTypeDef",
-    "QueryObjectsOutputTypeDef",
-    "ReportTaskProgressOutputTypeDef",
-    "ReportTaskRunnerHeartbeatOutputTypeDef",
-    "DescribeObjectsInputDescribeObjectsPaginateTypeDef",
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
     "PipelineDescriptionTypeDef",
     "PipelineObjectTypeDef",
     "ReportTaskProgressInputRequestTypeDef",
     "PollForTaskInputRequestTypeDef",
     "ListPipelinesOutputTypeDef",
     "SelectorTypeDef",
     "ParameterObjectTypeDef",
@@ -89,22 +89,19 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreatePipelineOutputTypeDef = TypedDict(
+    "CreatePipelineOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "pipelineId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeactivatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredDeactivatePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
@@ -126,24 +123,36 @@
 DeletePipelineInputRequestTypeDef = TypedDict(
     "DeletePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "pipelineId": str,
+        "objectIds": Sequence[str],
+    },
+)
+_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef",
+    {
+        "evaluateExpressions": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class DescribeObjectsInputDescribeObjectsPaginateTypeDef(
+    _RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef,
+    _OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeObjectsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeObjectsInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectIds": Sequence[str],
     },
 )
@@ -164,23 +173,38 @@
 DescribePipelinesInputRequestTypeDef = TypedDict(
     "DescribePipelinesInputRequestTypeDef",
     {
         "pipelineIds": Sequence[str],
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EvaluateExpressionInputRequestTypeDef = TypedDict(
     "EvaluateExpressionInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectId": str,
         "expression": str,
     },
 )
 
+EvaluateExpressionOutputTypeDef = TypedDict(
+    "EvaluateExpressionOutputTypeDef",
+    {
+        "evaluatedExpression": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFieldTypeDef = TypedDict(
     "_RequiredFieldTypeDef",
     {
         "key": str,
     },
 )
 _OptionalFieldTypeDef = TypedDict(
@@ -220,14 +244,22 @@
     {
         "document": str,
         "signature": str,
     },
     total=False,
 )
 
+ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPipelinesInputRequestTypeDef = TypedDict(
     "ListPipelinesInputRequestTypeDef",
     {
         "marker": str,
     },
     total=False,
 )
@@ -246,14 +278,24 @@
     {
         "type": OperatorTypeType,
         "values": Sequence[str],
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
 ParameterAttributeTypeDef = TypedDict(
     "ParameterAttributeTypeDef",
     {
         "key": str,
         "stringValue": str,
     },
 )
@@ -272,22 +314,40 @@
     {
         "id": str,
         "warnings": List[str],
     },
     total=False,
 )
 
+QueryObjectsOutputTypeDef = TypedDict(
+    "QueryObjectsOutputTypeDef",
+    {
+        "ids": List[str],
+        "marker": str,
+        "hasMoreResults": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveTagsInputRequestTypeDef = TypedDict(
     "RemoveTagsInputRequestTypeDef",
     {
         "pipelineId": str,
         "tagKeys": Sequence[str],
     },
 )
 
+ReportTaskProgressOutputTypeDef = TypedDict(
+    "ReportTaskProgressOutputTypeDef",
+    {
+        "canceled": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredReportTaskRunnerHeartbeatInputRequestTypeDef = TypedDict(
     "_RequiredReportTaskRunnerHeartbeatInputRequestTypeDef",
     {
         "taskrunnerId": str,
     },
 )
 _OptionalReportTaskRunnerHeartbeatInputRequestTypeDef = TypedDict(
@@ -301,14 +361,33 @@
 
 class ReportTaskRunnerHeartbeatInputRequestTypeDef(
     _RequiredReportTaskRunnerHeartbeatInputRequestTypeDef,
     _OptionalReportTaskRunnerHeartbeatInputRequestTypeDef,
 ):
     pass
 
+ReportTaskRunnerHeartbeatOutputTypeDef = TypedDict(
+    "ReportTaskRunnerHeartbeatOutputTypeDef",
+    {
+        "terminate": bool,
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
 SetStatusInputRequestTypeDef = TypedDict(
     "SetStatusInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectIds": Sequence[str],
         "status": str,
     },
@@ -381,93 +460,14 @@
 )
 
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
-CreatePipelineOutputTypeDef = TypedDict(
-    "CreatePipelineOutputTypeDef",
-    {
-        "pipelineId": str,
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
-EvaluateExpressionOutputTypeDef = TypedDict(
-    "EvaluateExpressionOutputTypeDef",
-    {
-        "evaluatedExpression": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-QueryObjectsOutputTypeDef = TypedDict(
-    "QueryObjectsOutputTypeDef",
-    {
-        "ids": List[str],
-        "marker": str,
-        "hasMoreResults": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReportTaskProgressOutputTypeDef = TypedDict(
-    "ReportTaskProgressOutputTypeDef",
-    {
-        "canceled": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReportTaskRunnerHeartbeatOutputTypeDef = TypedDict(
-    "ReportTaskRunnerHeartbeatOutputTypeDef",
-    {
-        "terminate": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef",
-    {
-        "pipelineId": str,
-        "objectIds": Sequence[str],
-    },
-)
-_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef",
-    {
-        "evaluateExpressions": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeObjectsInputDescribeObjectsPaginateTypeDef(
-    _RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef,
-    _OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef,
-):
-    pass
-
-ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredPipelineDescriptionTypeDef = TypedDict(
     "_RequiredPipelineDescriptionTypeDef",
     {
         "pipelineId": str,
         "name": str,
         "fields": List[FieldTypeDef],
     },
@@ -536,15 +536,15 @@
 
 ListPipelinesOutputTypeDef = TypedDict(
     "ListPipelinesOutputTypeDef",
     {
         "pipelineIdList": List[PipelineIdNameTypeDef],
         "marker": str,
         "hasMoreResults": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SelectorTypeDef = TypedDict(
     "SelectorTypeDef",
     {
         "fieldName": str,
@@ -563,43 +563,43 @@
 
 PutPipelineDefinitionOutputTypeDef = TypedDict(
     "PutPipelineDefinitionOutputTypeDef",
     {
         "validationErrors": List[ValidationErrorTypeDef],
         "validationWarnings": List[ValidationWarningTypeDef],
         "errored": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ValidatePipelineDefinitionOutputTypeDef = TypedDict(
     "ValidatePipelineDefinitionOutputTypeDef",
     {
         "validationErrors": List[ValidationErrorTypeDef],
         "validationWarnings": List[ValidationWarningTypeDef],
         "errored": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePipelinesOutputTypeDef = TypedDict(
     "DescribePipelinesOutputTypeDef",
     {
         "pipelineDescriptionList": List[PipelineDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeObjectsOutputTypeDef = TypedDict(
     "DescribeObjectsOutputTypeDef",
     {
         "pipelineObjects": List[PipelineObjectTypeDef],
         "marker": str,
         "hasMoreResults": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TaskObjectTypeDef = TypedDict(
     "TaskObjectTypeDef",
     {
         "taskId": str,
@@ -620,15 +620,15 @@
 
 GetPipelineDefinitionOutputTypeDef = TypedDict(
     "GetPipelineDefinitionOutputTypeDef",
     {
         "pipelineObjects": List[PipelineObjectTypeDef],
         "parameterObjects": List[ParameterObjectTypeDef],
         "parameterValues": List[ParameterValueTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredPutPipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
@@ -672,30 +672,30 @@
 ):
     pass
 
 PollForTaskOutputTypeDef = TypedDict(
     "PollForTaskOutputTypeDef",
     {
         "taskObject": TaskObjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredQueryObjectsInputQueryObjectsPaginateTypeDef = TypedDict(
     "_RequiredQueryObjectsInputQueryObjectsPaginateTypeDef",
     {
         "pipelineId": str,
         "sphere": str,
     },
 )
 _OptionalQueryObjectsInputQueryObjectsPaginateTypeDef = TypedDict(
     "_OptionalQueryObjectsInputQueryObjectsPaginateTypeDef",
     {
         "query": QueryTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class QueryObjectsInputQueryObjectsPaginateTypeDef(
     _RequiredQueryObjectsInputQueryObjectsPaginateTypeDef,
     _OptionalQueryObjectsInputQueryObjectsPaginateTypeDef,
```

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline.egg-info/PKG-INFO` & `mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datapipeline
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.DataPipeline 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.DataPipeline 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/
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
 
 <a id="mypy-boto3-datapipeline"></a>
 
 # mypy-boto3-datapipeline
 
 [![PyPI - mypy-boto3-datapipeline](https://img.shields.io/pypi/v/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-datapipeline?color=blue)](https://pypistats.org/packages/mypy-boto3-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataPipeline 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[boto3.DataPipeline 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
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
 [mypy-boto3-datapipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,45 +331,45 @@
 `mypy_boto3_datapipeline.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_datapipeline.type_defs import (
     ParameterValueTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
+    CreatePipelineOutputTypeDef,
     DeactivatePipelineInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeObjectsInputDescribeObjectsPaginateTypeDef,
     DescribeObjectsInputRequestTypeDef,
     DescribePipelinesInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     EvaluateExpressionInputRequestTypeDef,
+    EvaluateExpressionOutputTypeDef,
     FieldTypeDef,
     GetPipelineDefinitionInputRequestTypeDef,
     InstanceIdentityTypeDef,
+    ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineIdNameTypeDef,
     OperatorTypeDef,
+    PaginatorConfigTypeDef,
     ParameterAttributeTypeDef,
     ValidationErrorTypeDef,
     ValidationWarningTypeDef,
+    QueryObjectsOutputTypeDef,
     RemoveTagsInputRequestTypeDef,
+    ReportTaskProgressOutputTypeDef,
     ReportTaskRunnerHeartbeatInputRequestTypeDef,
+    ReportTaskRunnerHeartbeatOutputTypeDef,
+    ResponseMetadataTypeDef,
     SetStatusInputRequestTypeDef,
     SetTaskStatusInputRequestTypeDef,
     ActivatePipelineInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
     CreatePipelineInputRequestTypeDef,
-    CreatePipelineOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EvaluateExpressionOutputTypeDef,
-    QueryObjectsOutputTypeDef,
-    ReportTaskProgressOutputTypeDef,
-    ReportTaskRunnerHeartbeatOutputTypeDef,
-    DescribeObjectsInputDescribeObjectsPaginateTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
     PipelineDescriptionTypeDef,
     PipelineObjectTypeDef,
     ReportTaskProgressInputRequestTypeDef,
     PollForTaskInputRequestTypeDef,
     ListPipelinesOutputTypeDef,
     SelectorTypeDef,
     ParameterObjectTypeDef,
@@ -394,42 +395,42 @@
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

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/mypy_boto3_datapipeline.egg-info/SOURCES.txt` & `mypy-boto3-datapipeline-1.27.0/mypy_boto3_datapipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.26.0.post1/setup.py` & `mypy-boto3-datapipeline-1.27.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-datapipeline.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-datapipeline",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_datapipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DataPipeline 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.DataPipeline 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 datapipeline type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_datapipeline": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_datapipeline": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/",
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


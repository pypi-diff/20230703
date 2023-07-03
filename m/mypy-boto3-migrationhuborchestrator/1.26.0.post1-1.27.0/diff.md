# Comparing `tmp/mypy-boto3-migrationhuborchestrator-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-migrationhuborchestrator-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migrationhuborchestrator-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:45 2022, max compression
+gzip compressed data, was "mypy-boto3-migrationhuborchestrator-1.27.0.tar", last modified: Mon Jul  3 19:51:08 2023, max compression
```

## Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1.tar` & `mypy-boto3-migrationhuborchestrator-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:45.868836 mypy-boto3-migrationhuborchestrator-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:38:23.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    18010 2022-11-01 21:43:45.864837 mypy-boto3-migrationhuborchestrator-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16501 2022-11-01 21:38:23.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:45.864837 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/
--rw-r--r--   0 runner    (1001) docker     (121)     1992 2022-11-01 21:38:23.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-11-01 21:38:23.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-11-01 21:38:23.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25168 2022-11-01 21:38:23.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    25126 2022-11-01 21:38:23.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9278 2022-11-01 21:38:23.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9276 2022-11-01 21:38:23.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9366 2022-11-01 21:38:23.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9357 2022-11-01 21:38:23.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:38:23.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    31820 2022-11-01 21:38:24.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    31792 2022-11-01 21:38:24.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:38:23.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:45.864837 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18010 2022-11-01 21:43:45.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-11-01 21:43:45.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:45.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:45.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:45.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-01 21:43:45.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:45.868836 mypy-boto3-migrationhuborchestrator-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2127 2022-11-01 21:38:23.000000 mypy-boto3-migrationhuborchestrator-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.735690 mypy-boto3-migrationhuborchestrator-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:25.000000 mypy-boto3-migrationhuborchestrator-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-07-03 19:51:08.731690 mypy-boto3-migrationhuborchestrator-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-07-03 19:42:25.000000 mypy-boto3-migrationhuborchestrator-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.731690 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-03 19:42:25.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-03 19:42:25.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-03 19:42:25.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25168 2023-07-03 19:42:25.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-07-03 19:42:25.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-07-03 19:42:26.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-07-03 19:42:25.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-07-03 19:42:25.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-07-03 19:42:25.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:25.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31882 2023-07-03 19:42:26.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31854 2023-07-03 19:42:26.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:25.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:08.731690 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-07-03 19:51:08.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-03 19:51:08.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:08.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:08.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:08.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-03 19:51:08.000000 mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:08.735690 mypy-boto3-migrationhuborchestrator-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-03 19:42:25.000000 mypy-boto3-migrationhuborchestrator-1.27.0/setup.py
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/LICENSE` & `mypy-boto3-migrationhuborchestrator-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/PKG-INFO` & `mypy-boto3-migrationhuborchestrator-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhuborchestrator
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.MigrationHubOrchestrator 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.MigrationHubOrchestrator 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/
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
 
 <a id="mypy-boto3-migrationhuborchestrator"></a>
 
 # mypy-boto3-migrationhuborchestrator
 
 [![PyPI - mypy-boto3-migrationhuborchestrator](https://img.shields.io/pypi/v/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migrationhuborchestrator?color=blue)](https://pypistats.org/packages/mypy-boto3-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubOrchestrator 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[boto3.MigrationHubOrchestrator 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
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
 [mypy-boto3-migrationhuborchestrator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,77 +359,77 @@
 
 `mypy_boto3_migrationhuborchestrator.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhuborchestrator.type_defs import (
     StepInputTypeDef,
-    ResponseMetadataTypeDef,
     CreateWorkflowStepGroupRequestRequestTypeDef,
     ToolTypeDef,
+    CreateWorkflowStepResponseTypeDef,
     DeleteMigrationWorkflowRequestRequestTypeDef,
+    DeleteMigrationWorkflowResponseTypeDef,
     DeleteWorkflowStepGroupRequestRequestTypeDef,
     DeleteWorkflowStepRequestRequestTypeDef,
     GetMigrationWorkflowRequestRequestTypeDef,
     GetMigrationWorkflowTemplateRequestRequestTypeDef,
     TemplateInputTypeDef,
     GetTemplateStepGroupRequestRequestTypeDef,
     GetTemplateStepRequestRequestTypeDef,
     StepOutputTypeDef,
     GetWorkflowStepGroupRequestRequestTypeDef,
     GetWorkflowStepRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
     ListMigrationWorkflowTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
+    ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListMigrationWorkflowsRequestRequestTypeDef,
     MigrationWorkflowSummaryTypeDef,
+    ListPluginsRequestListPluginsPaginateTypeDef,
     ListPluginsRequestRequestTypeDef,
     PluginSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
     ListTemplateStepGroupsRequestRequestTypeDef,
     TemplateStepGroupSummaryTypeDef,
+    ListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
     ListTemplateStepsRequestRequestTypeDef,
     TemplateStepSummaryTypeDef,
+    ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
     ListWorkflowStepGroupsRequestRequestTypeDef,
     WorkflowStepGroupSummaryTypeDef,
+    ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
     ListWorkflowStepsRequestRequestTypeDef,
     WorkflowStepSummaryTypeDef,
+    PaginatorConfigTypeDef,
     PlatformCommandTypeDef,
     PlatformScriptKeyTypeDef,
+    ResponseMetadataTypeDef,
     RetryWorkflowStepRequestRequestTypeDef,
+    RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowRequestRequestTypeDef,
+    StartMigrationWorkflowResponseTypeDef,
     StopMigrationWorkflowRequestRequestTypeDef,
+    StopMigrationWorkflowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWorkflowStepGroupRequestRequestTypeDef,
+    UpdateWorkflowStepResponseTypeDef,
     WorkflowStepOutputUnionTypeDef,
     CreateMigrationWorkflowRequestRequestTypeDef,
-    UpdateMigrationWorkflowRequestRequestTypeDef,
     CreateMigrationWorkflowResponseTypeDef,
-    CreateWorkflowStepResponseTypeDef,
-    DeleteMigrationWorkflowResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RetryWorkflowStepResponseTypeDef,
-    StartMigrationWorkflowResponseTypeDef,
-    StopMigrationWorkflowResponseTypeDef,
+    UpdateMigrationWorkflowRequestRequestTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
-    UpdateWorkflowStepResponseTypeDef,
     CreateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowResponseTypeDef,
     GetTemplateStepGroupResponseTypeDef,
     GetWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowTemplateResponseTypeDef,
-    ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
-    ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef,
-    ListPluginsRequestListPluginsPaginateTypeDef,
-    ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
-    ListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
-    ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
-    ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
     ListMigrationWorkflowTemplatesResponseTypeDef,
     ListMigrationWorkflowsResponseTypeDef,
     ListPluginsResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
@@ -449,42 +450,42 @@
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

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/README.md` & `mypy-boto3-migrationhuborchestrator-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-migrationhuborchestrator"></a>
 
 # mypy-boto3-migrationhuborchestrator
 
 [![PyPI - mypy-boto3-migrationhuborchestrator](https://img.shields.io/pypi/v/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migrationhuborchestrator?color=blue)](https://pypistats.org/packages/mypy-boto3-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubOrchestrator 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[boto3.MigrationHubOrchestrator 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
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
 [mypy-boto3-migrationhuborchestrator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,77 +327,77 @@
 
 `mypy_boto3_migrationhuborchestrator.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhuborchestrator.type_defs import (
     StepInputTypeDef,
-    ResponseMetadataTypeDef,
     CreateWorkflowStepGroupRequestRequestTypeDef,
     ToolTypeDef,
+    CreateWorkflowStepResponseTypeDef,
     DeleteMigrationWorkflowRequestRequestTypeDef,
+    DeleteMigrationWorkflowResponseTypeDef,
     DeleteWorkflowStepGroupRequestRequestTypeDef,
     DeleteWorkflowStepRequestRequestTypeDef,
     GetMigrationWorkflowRequestRequestTypeDef,
     GetMigrationWorkflowTemplateRequestRequestTypeDef,
     TemplateInputTypeDef,
     GetTemplateStepGroupRequestRequestTypeDef,
     GetTemplateStepRequestRequestTypeDef,
     StepOutputTypeDef,
     GetWorkflowStepGroupRequestRequestTypeDef,
     GetWorkflowStepRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
     ListMigrationWorkflowTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
+    ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListMigrationWorkflowsRequestRequestTypeDef,
     MigrationWorkflowSummaryTypeDef,
+    ListPluginsRequestListPluginsPaginateTypeDef,
     ListPluginsRequestRequestTypeDef,
     PluginSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
     ListTemplateStepGroupsRequestRequestTypeDef,
     TemplateStepGroupSummaryTypeDef,
+    ListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
     ListTemplateStepsRequestRequestTypeDef,
     TemplateStepSummaryTypeDef,
+    ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
     ListWorkflowStepGroupsRequestRequestTypeDef,
     WorkflowStepGroupSummaryTypeDef,
+    ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
     ListWorkflowStepsRequestRequestTypeDef,
     WorkflowStepSummaryTypeDef,
+    PaginatorConfigTypeDef,
     PlatformCommandTypeDef,
     PlatformScriptKeyTypeDef,
+    ResponseMetadataTypeDef,
     RetryWorkflowStepRequestRequestTypeDef,
+    RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowRequestRequestTypeDef,
+    StartMigrationWorkflowResponseTypeDef,
     StopMigrationWorkflowRequestRequestTypeDef,
+    StopMigrationWorkflowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWorkflowStepGroupRequestRequestTypeDef,
+    UpdateWorkflowStepResponseTypeDef,
     WorkflowStepOutputUnionTypeDef,
     CreateMigrationWorkflowRequestRequestTypeDef,
-    UpdateMigrationWorkflowRequestRequestTypeDef,
     CreateMigrationWorkflowResponseTypeDef,
-    CreateWorkflowStepResponseTypeDef,
-    DeleteMigrationWorkflowResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RetryWorkflowStepResponseTypeDef,
-    StartMigrationWorkflowResponseTypeDef,
-    StopMigrationWorkflowResponseTypeDef,
+    UpdateMigrationWorkflowRequestRequestTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
-    UpdateWorkflowStepResponseTypeDef,
     CreateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowResponseTypeDef,
     GetTemplateStepGroupResponseTypeDef,
     GetWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowTemplateResponseTypeDef,
-    ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
-    ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef,
-    ListPluginsRequestListPluginsPaginateTypeDef,
-    ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
-    ListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
-    ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
-    ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
     ListMigrationWorkflowTemplatesResponseTypeDef,
     ListMigrationWorkflowsResponseTypeDef,
     ListPluginsResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
@@ -418,42 +418,42 @@
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

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/__init__.py` & `mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/__init__.pyi` & `mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/__main__.py` & `mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHubOrchestrator 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.MigrationHubOrchestrator 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator\nOther"
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

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/client.py` & `mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/client.pyi` & `mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/literals.py` & `mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DataTypeType",
     "ListPluginsPaginatorName",
     "ListTemplateStepGroupsPaginatorName",
     "ListTemplateStepsPaginatorName",
     "ListTemplatesPaginatorName",
     "ListWorkflowStepGroupsPaginatorName",
@@ -40,15 +39,14 @@
     "MigrationHubOrchestratorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DataTypeType = Literal["INTEGER", "STRING", "STRINGLIST", "STRINGMAP"]
 ListPluginsPaginatorName = Literal["list_plugins"]
 ListTemplateStepGroupsPaginatorName = Literal["list_template_step_groups"]
 ListTemplateStepsPaginatorName = Literal["list_template_steps"]
 ListTemplatesPaginatorName = Literal["list_templates"]
 ListWorkflowStepGroupsPaginatorName = Literal["list_workflow_step_groups"]
 ListWorkflowStepsPaginatorName = Literal["list_workflow_steps"]
@@ -106,23 +104,25 @@
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
@@ -132,30 +132,35 @@
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
@@ -181,14 +186,15 @@
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
@@ -233,51 +239,57 @@
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
@@ -290,14 +302,15 @@
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
@@ -309,28 +322,35 @@
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
@@ -339,14 +359,15 @@
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
@@ -357,55 +378,64 @@
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

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/literals.pyi` & `mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DataTypeType",
     "ListPluginsPaginatorName",
     "ListTemplateStepGroupsPaginatorName",
     "ListTemplateStepsPaginatorName",
     "ListTemplatesPaginatorName",
     "ListWorkflowStepGroupsPaginatorName",
@@ -39,14 +40,15 @@
     "MigrationHubOrchestratorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DataTypeType = Literal["INTEGER", "STRING", "STRINGLIST", "STRINGMAP"]
 ListPluginsPaginatorName = Literal["list_plugins"]
 ListTemplateStepGroupsPaginatorName = Literal["list_template_step_groups"]
 ListTemplateStepsPaginatorName = Literal["list_template_steps"]
 ListTemplatesPaginatorName = Literal["list_templates"]
 ListWorkflowStepGroupsPaginatorName = Literal["list_workflow_step_groups"]
 ListWorkflowStepsPaginatorName = Literal["list_workflow_steps"]
@@ -104,23 +106,25 @@
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
@@ -130,30 +134,35 @@
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
@@ -179,14 +188,15 @@
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
@@ -231,51 +241,57 @@
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
@@ -288,14 +304,15 @@
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
@@ -307,28 +324,35 @@
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
@@ -337,14 +361,15 @@
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
@@ -355,55 +380,64 @@
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

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/paginator.py` & `mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,90 +71,90 @@
 class ListPluginsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListPlugins)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listpluginspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPluginsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListPlugins.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listpluginspaginator)
         """
 
 
 class ListTemplateStepGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateStepGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepgroupspaginator)
     """
 
     def paginate(
-        self, *, templateId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, templateId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTemplateStepGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateStepGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepgroupspaginator)
         """
 
 
 class ListTemplateStepsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateSteps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepspaginator)
     """
 
     def paginate(
-        self, *, templateId: str, stepGroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, templateId: str, stepGroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTemplateStepsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateSteps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepspaginator)
         """
 
 
 class ListTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatespaginator)
     """
 
     def paginate(
-        self, *, name: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, name: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMigrationWorkflowTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatespaginator)
         """
 
 
 class ListWorkflowStepGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowStepGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepgroupspaginator)
     """
 
     def paginate(
-        self, *, workflowId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, workflowId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkflowStepGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowStepGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepgroupspaginator)
         """
 
 
 class ListWorkflowStepsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowSteps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepspaginator)
     """
 
     def paginate(
-        self, *, workflowId: str, stepGroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, workflowId: str, stepGroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkflowStepsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowSteps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepspaginator)
         """
 
 
@@ -167,13 +167,13 @@
     def paginate(
         self,
         *,
         templateId: str = ...,
         adsApplicationConfigurationName: str = ...,
         status: MigrationWorkflowStatusEnumType = ...,
         name: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMigrationWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowspaginator)
         """
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/paginator.pyi` & `mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -68,85 +68,85 @@
 class ListPluginsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListPlugins)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listpluginspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPluginsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListPlugins.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listpluginspaginator)
         """
 
 class ListTemplateStepGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateStepGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepgroupspaginator)
     """
 
     def paginate(
-        self, *, templateId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, templateId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTemplateStepGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateStepGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepgroupspaginator)
         """
 
 class ListTemplateStepsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateSteps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepspaginator)
     """
 
     def paginate(
-        self, *, templateId: str, stepGroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, templateId: str, stepGroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTemplateStepsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateSteps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepspaginator)
         """
 
 class ListTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatespaginator)
     """
 
     def paginate(
-        self, *, name: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, name: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMigrationWorkflowTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatespaginator)
         """
 
 class ListWorkflowStepGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowStepGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepgroupspaginator)
     """
 
     def paginate(
-        self, *, workflowId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, workflowId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkflowStepGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowStepGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepgroupspaginator)
         """
 
 class ListWorkflowStepsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowSteps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepspaginator)
     """
 
     def paginate(
-        self, *, workflowId: str, stepGroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, workflowId: str, stepGroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorkflowStepsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowSteps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepspaginator)
         """
 
 class ListWorkflowsPaginator(Paginator):
@@ -158,13 +158,13 @@
     def paginate(
         self,
         *,
         templateId: str = ...,
         adsApplicationConfigurationName: str = ...,
         status: MigrationWorkflowStatusEnumType = ...,
         name: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListMigrationWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowspaginator)
         """
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/type_defs.py` & `mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,77 +35,77 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "StepInputTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateWorkflowStepGroupRequestRequestTypeDef",
     "ToolTypeDef",
+    "CreateWorkflowStepResponseTypeDef",
     "DeleteMigrationWorkflowRequestRequestTypeDef",
+    "DeleteMigrationWorkflowResponseTypeDef",
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     "DeleteWorkflowStepRequestRequestTypeDef",
     "GetMigrationWorkflowRequestRequestTypeDef",
     "GetMigrationWorkflowTemplateRequestRequestTypeDef",
     "TemplateInputTypeDef",
     "GetTemplateStepGroupRequestRequestTypeDef",
     "GetTemplateStepRequestRequestTypeDef",
     "StepOutputTypeDef",
     "GetWorkflowStepGroupRequestRequestTypeDef",
     "GetWorkflowStepRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
     "ListMigrationWorkflowTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
+    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListMigrationWorkflowsRequestRequestTypeDef",
     "MigrationWorkflowSummaryTypeDef",
+    "ListPluginsRequestListPluginsPaginateTypeDef",
     "ListPluginsRequestRequestTypeDef",
     "PluginSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
     "ListTemplateStepGroupsRequestRequestTypeDef",
     "TemplateStepGroupSummaryTypeDef",
+    "ListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
     "ListTemplateStepsRequestRequestTypeDef",
     "TemplateStepSummaryTypeDef",
+    "ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
     "ListWorkflowStepGroupsRequestRequestTypeDef",
     "WorkflowStepGroupSummaryTypeDef",
+    "ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
     "ListWorkflowStepsRequestRequestTypeDef",
     "WorkflowStepSummaryTypeDef",
+    "PaginatorConfigTypeDef",
     "PlatformCommandTypeDef",
     "PlatformScriptKeyTypeDef",
+    "ResponseMetadataTypeDef",
     "RetryWorkflowStepRequestRequestTypeDef",
+    "RetryWorkflowStepResponseTypeDef",
     "StartMigrationWorkflowRequestRequestTypeDef",
+    "StartMigrationWorkflowResponseTypeDef",
     "StopMigrationWorkflowRequestRequestTypeDef",
+    "StopMigrationWorkflowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkflowStepGroupRequestRequestTypeDef",
+    "UpdateWorkflowStepResponseTypeDef",
     "WorkflowStepOutputUnionTypeDef",
     "CreateMigrationWorkflowRequestRequestTypeDef",
-    "UpdateMigrationWorkflowRequestRequestTypeDef",
     "CreateMigrationWorkflowResponseTypeDef",
-    "CreateWorkflowStepResponseTypeDef",
-    "DeleteMigrationWorkflowResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RetryWorkflowStepResponseTypeDef",
-    "StartMigrationWorkflowResponseTypeDef",
-    "StopMigrationWorkflowResponseTypeDef",
+    "UpdateMigrationWorkflowRequestRequestTypeDef",
     "UpdateMigrationWorkflowResponseTypeDef",
-    "UpdateWorkflowStepResponseTypeDef",
     "CreateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowResponseTypeDef",
     "GetTemplateStepGroupResponseTypeDef",
     "GetWorkflowStepGroupResponseTypeDef",
     "UpdateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowTemplateResponseTypeDef",
-    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
-    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
-    "ListPluginsRequestListPluginsPaginateTypeDef",
-    "ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
-    "ListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
-    "ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
-    "ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
     "ListMigrationWorkflowTemplatesResponseTypeDef",
     "ListMigrationWorkflowsResponseTypeDef",
     "ListPluginsResponseTypeDef",
     "ListTemplateStepGroupsResponseTypeDef",
     "ListTemplateStepsResponseTypeDef",
     "ListWorkflowStepGroupsResponseTypeDef",
     "ListWorkflowStepsResponseTypeDef",
@@ -125,25 +125,14 @@
         "stringValue": str,
         "listOfStringsValue": Sequence[str],
         "mapOfStringValue": Mapping[str, str],
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
 _RequiredCreateWorkflowStepGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowStepGroupRequestRequestTypeDef",
     {
         "workflowId": str,
         "name": str,
     },
 )
@@ -170,21 +159,42 @@
     {
         "name": str,
         "url": str,
     },
     total=False,
 )
 
+CreateWorkflowStepResponseTypeDef = TypedDict(
+    "CreateWorkflowStepResponseTypeDef",
+    {
+        "id": str,
+        "stepGroupId": str,
+        "workflowId": str,
+        "name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+DeleteMigrationWorkflowResponseTypeDef = TypedDict(
+    "DeleteMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "status": MigrationWorkflowStatusEnumType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteWorkflowStepGroupRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     {
         "workflowId": str,
         "id": str,
     },
 )
@@ -262,20 +272,19 @@
     {
         "workflowId": str,
         "stepGroupId": str,
         "id": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
+    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "name": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListMigrationWorkflowTemplatesRequestRequestTypeDef = TypedDict(
     "ListMigrationWorkflowTemplatesRequestRequestTypeDef",
     {
@@ -293,14 +302,26 @@
         "name": str,
         "arn": str,
         "description": str,
     },
     total=False,
 )
 
+ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
+    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
+    {
+        "templateId": str,
+        "adsApplicationConfigurationName": str,
+        "status": MigrationWorkflowStatusEnumType,
+        "name": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMigrationWorkflowsRequestRequestTypeDef = TypedDict(
     "ListMigrationWorkflowsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "templateId": str,
         "adsApplicationConfigurationName": str,
@@ -323,14 +344,22 @@
         "statusMessage": str,
         "completedSteps": int,
         "totalSteps": int,
     },
     total=False,
 )
 
+ListPluginsRequestListPluginsPaginateTypeDef = TypedDict(
+    "ListPluginsRequestListPluginsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPluginsRequestRequestTypeDef = TypedDict(
     "ListPluginsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -352,14 +381,44 @@
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
+_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
+    {
+        "templateId": str,
+    },
+)
+_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef(
+    _RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
+    _OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTemplateStepGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplateStepGroupsRequestRequestTypeDef",
     {
         "templateId": str,
     },
 )
 _OptionalListTemplateStepGroupsRequestRequestTypeDef = TypedDict(
@@ -386,14 +445,37 @@
         "name": str,
         "previous": List[str],
         "next": List[str],
     },
     total=False,
 )
 
+_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
+    "_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
+    {
+        "templateId": str,
+        "stepGroupId": str,
+    },
+)
+_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
+    "_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTemplateStepsRequestListTemplateStepsPaginateTypeDef(
+    _RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
+    _OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTemplateStepsRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplateStepsRequestRequestTypeDef",
     {
         "templateId": str,
         "stepGroupId": str,
     },
 )
@@ -425,14 +507,36 @@
         "owner": OwnerType,
         "previous": List[str],
         "next": List[str],
     },
     total=False,
 )
 
+_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
+    {
+        "workflowId": str,
+    },
+)
+_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef(
+    _RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
+    _OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListWorkflowStepGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkflowStepGroupsRequestRequestTypeDef",
     {
         "workflowId": str,
     },
 )
 _OptionalListWorkflowStepGroupsRequestRequestTypeDef = TypedDict(
@@ -461,14 +565,37 @@
         "status": StepGroupStatusType,
         "previous": List[str],
         "next": List[str],
     },
     total=False,
 )
 
+_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
+    "_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
+    {
+        "workflowId": str,
+        "stepGroupId": str,
+    },
+)
+_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
+    "_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef(
+    _RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
+    _OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListWorkflowStepsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkflowStepsRequestRequestTypeDef",
     {
         "workflowId": str,
         "stepGroupId": str,
     },
 )
@@ -504,14 +631,24 @@
         "totalNoOfSrv": int,
         "description": str,
         "scriptLocation": str,
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
 PlatformCommandTypeDef = TypedDict(
     "PlatformCommandTypeDef",
     {
         "linux": str,
         "windows": str,
     },
     total=False,
@@ -522,37 +659,83 @@
     {
         "linux": str,
         "windows": str,
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
 RetryWorkflowStepRequestRequestTypeDef = TypedDict(
     "RetryWorkflowStepRequestRequestTypeDef",
     {
         "workflowId": str,
         "stepGroupId": str,
         "id": str,
     },
 )
 
+RetryWorkflowStepResponseTypeDef = TypedDict(
+    "RetryWorkflowStepResponseTypeDef",
+    {
+        "stepGroupId": str,
+        "workflowId": str,
+        "id": str,
+        "status": StepStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StartMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+StartMigrationWorkflowResponseTypeDef = TypedDict(
+    "StartMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "status": MigrationWorkflowStatusEnumType,
+        "statusMessage": str,
+        "lastStartTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StopMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+StopMigrationWorkflowResponseTypeDef = TypedDict(
+    "StopMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "status": MigrationWorkflowStatusEnumType,
+        "statusMessage": str,
+        "lastStopTime": datetime,
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
@@ -587,14 +770,25 @@
 class UpdateWorkflowStepGroupRequestRequestTypeDef(
     _RequiredUpdateWorkflowStepGroupRequestRequestTypeDef,
     _OptionalUpdateWorkflowStepGroupRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateWorkflowStepResponseTypeDef = TypedDict(
+    "UpdateWorkflowStepResponseTypeDef",
+    {
+        "id": str,
+        "stepGroupId": str,
+        "workflowId": str,
+        "name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WorkflowStepOutputUnionTypeDef = TypedDict(
     "WorkflowStepOutputUnionTypeDef",
     {
         "integerValue": int,
         "stringValue": str,
         "listOfStringValue": Sequence[str],
     },
@@ -624,120 +818,56 @@
 class CreateMigrationWorkflowRequestRequestTypeDef(
     _RequiredCreateMigrationWorkflowRequestRequestTypeDef,
     _OptionalCreateMigrationWorkflowRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "inputParameters": Mapping[str, StepInputTypeDef],
-        "stepTargets": Sequence[str],
-    },
-    total=False,
-)
-
-
-class UpdateMigrationWorkflowRequestRequestTypeDef(
-    _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
-    _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
-):
-    pass
-
-
 CreateMigrationWorkflowResponseTypeDef = TypedDict(
     "CreateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
         "templateId": str,
         "adsApplicationConfigurationId": str,
         "workflowInputs": Dict[str, StepInputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkflowStepResponseTypeDef = TypedDict(
-    "CreateWorkflowStepResponseTypeDef",
-    {
-        "id": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteMigrationWorkflowResponseTypeDef = TypedDict(
-    "DeleteMigrationWorkflowResponseTypeDef",
+_RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
-        "arn": str,
-        "status": MigrationWorkflowStatusEnumType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMigrationWorkflowRequestRequestTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "name": str,
+        "description": str,
+        "inputParameters": Mapping[str, StepInputTypeDef],
+        "stepTargets": Sequence[str],
     },
+    total=False,
 )
 
-RetryWorkflowStepResponseTypeDef = TypedDict(
-    "RetryWorkflowStepResponseTypeDef",
-    {
-        "stepGroupId": str,
-        "workflowId": str,
-        "id": str,
-        "status": StepStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-StartMigrationWorkflowResponseTypeDef = TypedDict(
-    "StartMigrationWorkflowResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "status": MigrationWorkflowStatusEnumType,
-        "statusMessage": str,
-        "lastStartTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UpdateMigrationWorkflowRequestRequestTypeDef(
+    _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
+    _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
+):
+    pass
 
-StopMigrationWorkflowResponseTypeDef = TypedDict(
-    "StopMigrationWorkflowResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "status": MigrationWorkflowStatusEnumType,
-        "statusMessage": str,
-        "lastStopTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 UpdateMigrationWorkflowResponseTypeDef = TypedDict(
     "UpdateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
@@ -746,41 +876,30 @@
         "adsApplicationConfigurationId": str,
         "workflowInputs": Dict[str, StepInputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
         "lastModifiedTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateWorkflowStepResponseTypeDef = TypedDict(
-    "UpdateWorkflowStepResponseTypeDef",
-    {
-        "id": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateWorkflowStepGroupResponseTypeDef = TypedDict(
     "CreateWorkflowStepGroupResponseTypeDef",
     {
         "workflowId": str,
         "name": str,
         "id": str,
         "description": str,
         "tools": List[ToolTypeDef],
         "next": List[str],
         "previous": List[str],
         "creationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMigrationWorkflowResponseTypeDef = TypedDict(
     "GetMigrationWorkflowResponseTypeDef",
     {
         "id": str,
@@ -799,15 +918,15 @@
         "endTime": datetime,
         "tools": List[ToolTypeDef],
         "totalSteps": int,
         "completedSteps": int,
         "workflowInputs": Dict[str, StepInputTypeDef],
         "tags": Dict[str, str],
         "workflowBucket": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTemplateStepGroupResponseTypeDef = TypedDict(
     "GetTemplateStepGroupResponseTypeDef",
     {
         "templateId": str,
@@ -816,15 +935,15 @@
         "description": str,
         "status": StepGroupStatusType,
         "creationTime": datetime,
         "lastModifiedTime": datetime,
         "tools": List[ToolTypeDef],
         "previous": List[str],
         "next": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWorkflowStepGroupResponseTypeDef = TypedDict(
     "GetWorkflowStepGroupResponseTypeDef",
     {
         "id": str,
@@ -835,226 +954,107 @@
         "owner": OwnerType,
         "creationTime": datetime,
         "lastModifiedTime": datetime,
         "endTime": datetime,
         "tools": List[ToolTypeDef],
         "previous": List[str],
         "next": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateWorkflowStepGroupResponseTypeDef = TypedDict(
     "UpdateWorkflowStepGroupResponseTypeDef",
     {
         "workflowId": str,
         "name": str,
         "id": str,
         "description": str,
         "tools": List[ToolTypeDef],
         "next": List[str],
         "previous": List[str],
         "lastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMigrationWorkflowTemplateResponseTypeDef = TypedDict(
     "GetMigrationWorkflowTemplateResponseTypeDef",
     {
         "id": str,
         "name": str,
         "description": str,
         "inputs": List[TemplateInputTypeDef],
         "tools": List[ToolTypeDef],
         "status": Literal["CREATED"],
         "creationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
-    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
-    {
-        "name": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
-    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
-    {
-        "templateId": str,
-        "adsApplicationConfigurationName": str,
-        "status": MigrationWorkflowStatusEnumType,
-        "name": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPluginsRequestListPluginsPaginateTypeDef = TypedDict(
-    "ListPluginsRequestListPluginsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
-    {
-        "templateId": str,
-    },
-)
-_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef(
-    _RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
-    _OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
-    "_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
-    {
-        "templateId": str,
-        "stepGroupId": str,
-    },
-)
-_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
-    "_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTemplateStepsRequestListTemplateStepsPaginateTypeDef(
-    _RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
-    _OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
-    {
-        "workflowId": str,
-    },
-)
-_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef(
-    _RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
-    _OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
-    "_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
-    {
-        "workflowId": str,
-        "stepGroupId": str,
-    },
-)
-_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
-    "_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef(
-    _RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
-    _OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
-):
-    pass
-
-
 ListMigrationWorkflowTemplatesResponseTypeDef = TypedDict(
     "ListMigrationWorkflowTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "templateSummary": List[TemplateSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMigrationWorkflowsResponseTypeDef = TypedDict(
     "ListMigrationWorkflowsResponseTypeDef",
     {
         "nextToken": str,
         "migrationWorkflowSummary": List[MigrationWorkflowSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPluginsResponseTypeDef = TypedDict(
     "ListPluginsResponseTypeDef",
     {
         "nextToken": str,
         "plugins": List[PluginSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTemplateStepGroupsResponseTypeDef = TypedDict(
     "ListTemplateStepGroupsResponseTypeDef",
     {
         "nextToken": str,
         "templateStepGroupSummary": List[TemplateStepGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTemplateStepsResponseTypeDef = TypedDict(
     "ListTemplateStepsResponseTypeDef",
     {
         "nextToken": str,
         "templateStepSummaryList": List[TemplateStepSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkflowStepGroupsResponseTypeDef = TypedDict(
     "ListWorkflowStepGroupsResponseTypeDef",
     {
         "nextToken": str,
         "workflowStepGroupsSummary": List[WorkflowStepGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkflowStepsResponseTypeDef = TypedDict(
     "ListWorkflowStepsResponseTypeDef",
     {
         "nextToken": str,
         "workflowStepsSummary": List[WorkflowStepSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StepAutomationConfigurationTypeDef = TypedDict(
     "StepAutomationConfigurationTypeDef",
     {
         "scriptLocationS3Bucket": str,
@@ -1099,15 +1099,15 @@
         "description": str,
         "stepActionType": StepActionTypeType,
         "creationTime": str,
         "previous": List[str],
         "next": List[str],
         "outputs": List[StepOutputTypeDef],
         "stepAutomationConfiguration": StepAutomationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateWorkflowStepRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowStepRequestRequestTypeDef",
     {
         "name": str,
@@ -1157,15 +1157,15 @@
         "scriptOutputLocation": str,
         "creationTime": datetime,
         "lastStartTime": datetime,
         "endTime": datetime,
         "noOfSrvCompleted": int,
         "noOfSrvFailed": int,
         "totalNoOfSrv": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateWorkflowStepRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkflowStepRequestRequestTypeDef",
     {
         "id": str,
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator/type_defs.pyi` & `mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -34,77 +34,77 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "StepInputTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateWorkflowStepGroupRequestRequestTypeDef",
     "ToolTypeDef",
+    "CreateWorkflowStepResponseTypeDef",
     "DeleteMigrationWorkflowRequestRequestTypeDef",
+    "DeleteMigrationWorkflowResponseTypeDef",
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     "DeleteWorkflowStepRequestRequestTypeDef",
     "GetMigrationWorkflowRequestRequestTypeDef",
     "GetMigrationWorkflowTemplateRequestRequestTypeDef",
     "TemplateInputTypeDef",
     "GetTemplateStepGroupRequestRequestTypeDef",
     "GetTemplateStepRequestRequestTypeDef",
     "StepOutputTypeDef",
     "GetWorkflowStepGroupRequestRequestTypeDef",
     "GetWorkflowStepRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
     "ListMigrationWorkflowTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
+    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListMigrationWorkflowsRequestRequestTypeDef",
     "MigrationWorkflowSummaryTypeDef",
+    "ListPluginsRequestListPluginsPaginateTypeDef",
     "ListPluginsRequestRequestTypeDef",
     "PluginSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
     "ListTemplateStepGroupsRequestRequestTypeDef",
     "TemplateStepGroupSummaryTypeDef",
+    "ListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
     "ListTemplateStepsRequestRequestTypeDef",
     "TemplateStepSummaryTypeDef",
+    "ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
     "ListWorkflowStepGroupsRequestRequestTypeDef",
     "WorkflowStepGroupSummaryTypeDef",
+    "ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
     "ListWorkflowStepsRequestRequestTypeDef",
     "WorkflowStepSummaryTypeDef",
+    "PaginatorConfigTypeDef",
     "PlatformCommandTypeDef",
     "PlatformScriptKeyTypeDef",
+    "ResponseMetadataTypeDef",
     "RetryWorkflowStepRequestRequestTypeDef",
+    "RetryWorkflowStepResponseTypeDef",
     "StartMigrationWorkflowRequestRequestTypeDef",
+    "StartMigrationWorkflowResponseTypeDef",
     "StopMigrationWorkflowRequestRequestTypeDef",
+    "StopMigrationWorkflowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkflowStepGroupRequestRequestTypeDef",
+    "UpdateWorkflowStepResponseTypeDef",
     "WorkflowStepOutputUnionTypeDef",
     "CreateMigrationWorkflowRequestRequestTypeDef",
-    "UpdateMigrationWorkflowRequestRequestTypeDef",
     "CreateMigrationWorkflowResponseTypeDef",
-    "CreateWorkflowStepResponseTypeDef",
-    "DeleteMigrationWorkflowResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RetryWorkflowStepResponseTypeDef",
-    "StartMigrationWorkflowResponseTypeDef",
-    "StopMigrationWorkflowResponseTypeDef",
+    "UpdateMigrationWorkflowRequestRequestTypeDef",
     "UpdateMigrationWorkflowResponseTypeDef",
-    "UpdateWorkflowStepResponseTypeDef",
     "CreateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowResponseTypeDef",
     "GetTemplateStepGroupResponseTypeDef",
     "GetWorkflowStepGroupResponseTypeDef",
     "UpdateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowTemplateResponseTypeDef",
-    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
-    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
-    "ListPluginsRequestListPluginsPaginateTypeDef",
-    "ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
-    "ListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
-    "ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
-    "ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
     "ListMigrationWorkflowTemplatesResponseTypeDef",
     "ListMigrationWorkflowsResponseTypeDef",
     "ListPluginsResponseTypeDef",
     "ListTemplateStepGroupsResponseTypeDef",
     "ListTemplateStepsResponseTypeDef",
     "ListWorkflowStepGroupsResponseTypeDef",
     "ListWorkflowStepsResponseTypeDef",
@@ -124,25 +124,14 @@
         "stringValue": str,
         "listOfStringsValue": Sequence[str],
         "mapOfStringValue": Mapping[str, str],
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
 _RequiredCreateWorkflowStepGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowStepGroupRequestRequestTypeDef",
     {
         "workflowId": str,
         "name": str,
     },
 )
@@ -167,21 +156,42 @@
     {
         "name": str,
         "url": str,
     },
     total=False,
 )
 
+CreateWorkflowStepResponseTypeDef = TypedDict(
+    "CreateWorkflowStepResponseTypeDef",
+    {
+        "id": str,
+        "stepGroupId": str,
+        "workflowId": str,
+        "name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+DeleteMigrationWorkflowResponseTypeDef = TypedDict(
+    "DeleteMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "status": MigrationWorkflowStatusEnumType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteWorkflowStepGroupRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     {
         "workflowId": str,
         "id": str,
     },
 )
@@ -259,20 +269,19 @@
     {
         "workflowId": str,
         "stepGroupId": str,
         "id": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
+    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "name": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListMigrationWorkflowTemplatesRequestRequestTypeDef = TypedDict(
     "ListMigrationWorkflowTemplatesRequestRequestTypeDef",
     {
@@ -290,14 +299,26 @@
         "name": str,
         "arn": str,
         "description": str,
     },
     total=False,
 )
 
+ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
+    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
+    {
+        "templateId": str,
+        "adsApplicationConfigurationName": str,
+        "status": MigrationWorkflowStatusEnumType,
+        "name": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListMigrationWorkflowsRequestRequestTypeDef = TypedDict(
     "ListMigrationWorkflowsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "templateId": str,
         "adsApplicationConfigurationName": str,
@@ -320,14 +341,22 @@
         "statusMessage": str,
         "completedSteps": int,
         "totalSteps": int,
     },
     total=False,
 )
 
+ListPluginsRequestListPluginsPaginateTypeDef = TypedDict(
+    "ListPluginsRequestListPluginsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPluginsRequestRequestTypeDef = TypedDict(
     "ListPluginsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -349,14 +378,42 @@
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
+_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
+    {
+        "templateId": str,
+    },
+)
+_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef(
+    _RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
+    _OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
+):
+    pass
+
 _RequiredListTemplateStepGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplateStepGroupsRequestRequestTypeDef",
     {
         "templateId": str,
     },
 )
 _OptionalListTemplateStepGroupsRequestRequestTypeDef = TypedDict(
@@ -381,14 +438,35 @@
         "name": str,
         "previous": List[str],
         "next": List[str],
     },
     total=False,
 )
 
+_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
+    "_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
+    {
+        "templateId": str,
+        "stepGroupId": str,
+    },
+)
+_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
+    "_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTemplateStepsRequestListTemplateStepsPaginateTypeDef(
+    _RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
+    _OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
+):
+    pass
+
 _RequiredListTemplateStepsRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplateStepsRequestRequestTypeDef",
     {
         "templateId": str,
         "stepGroupId": str,
     },
 )
@@ -418,14 +496,34 @@
         "owner": OwnerType,
         "previous": List[str],
         "next": List[str],
     },
     total=False,
 )
 
+_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
+    {
+        "workflowId": str,
+    },
+)
+_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef(
+    _RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
+    _OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
+):
+    pass
+
 _RequiredListWorkflowStepGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkflowStepGroupsRequestRequestTypeDef",
     {
         "workflowId": str,
     },
 )
 _OptionalListWorkflowStepGroupsRequestRequestTypeDef = TypedDict(
@@ -452,14 +550,35 @@
         "status": StepGroupStatusType,
         "previous": List[str],
         "next": List[str],
     },
     total=False,
 )
 
+_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
+    "_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
+    {
+        "workflowId": str,
+        "stepGroupId": str,
+    },
+)
+_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
+    "_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef(
+    _RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
+    _OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
+):
+    pass
+
 _RequiredListWorkflowStepsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkflowStepsRequestRequestTypeDef",
     {
         "workflowId": str,
         "stepGroupId": str,
     },
 )
@@ -493,14 +612,24 @@
         "totalNoOfSrv": int,
         "description": str,
         "scriptLocation": str,
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
 PlatformCommandTypeDef = TypedDict(
     "PlatformCommandTypeDef",
     {
         "linux": str,
         "windows": str,
     },
     total=False,
@@ -511,37 +640,83 @@
     {
         "linux": str,
         "windows": str,
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
 RetryWorkflowStepRequestRequestTypeDef = TypedDict(
     "RetryWorkflowStepRequestRequestTypeDef",
     {
         "workflowId": str,
         "stepGroupId": str,
         "id": str,
     },
 )
 
+RetryWorkflowStepResponseTypeDef = TypedDict(
+    "RetryWorkflowStepResponseTypeDef",
+    {
+        "stepGroupId": str,
+        "workflowId": str,
+        "id": str,
+        "status": StepStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StartMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+StartMigrationWorkflowResponseTypeDef = TypedDict(
+    "StartMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "status": MigrationWorkflowStatusEnumType,
+        "statusMessage": str,
+        "lastStartTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StopMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+StopMigrationWorkflowResponseTypeDef = TypedDict(
+    "StopMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "status": MigrationWorkflowStatusEnumType,
+        "statusMessage": str,
+        "lastStopTime": datetime,
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
@@ -574,14 +749,25 @@
 
 class UpdateWorkflowStepGroupRequestRequestTypeDef(
     _RequiredUpdateWorkflowStepGroupRequestRequestTypeDef,
     _OptionalUpdateWorkflowStepGroupRequestRequestTypeDef,
 ):
     pass
 
+UpdateWorkflowStepResponseTypeDef = TypedDict(
+    "UpdateWorkflowStepResponseTypeDef",
+    {
+        "id": str,
+        "stepGroupId": str,
+        "workflowId": str,
+        "name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WorkflowStepOutputUnionTypeDef = TypedDict(
     "WorkflowStepOutputUnionTypeDef",
     {
         "integerValue": int,
         "stringValue": str,
         "listOfStringValue": Sequence[str],
     },
@@ -609,118 +795,54 @@
 
 class CreateMigrationWorkflowRequestRequestTypeDef(
     _RequiredCreateMigrationWorkflowRequestRequestTypeDef,
     _OptionalCreateMigrationWorkflowRequestRequestTypeDef,
 ):
     pass
 
-_RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "inputParameters": Mapping[str, StepInputTypeDef],
-        "stepTargets": Sequence[str],
-    },
-    total=False,
-)
-
-class UpdateMigrationWorkflowRequestRequestTypeDef(
-    _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
-    _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
-):
-    pass
-
 CreateMigrationWorkflowResponseTypeDef = TypedDict(
     "CreateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
         "templateId": str,
         "adsApplicationConfigurationId": str,
         "workflowInputs": Dict[str, StepInputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkflowStepResponseTypeDef = TypedDict(
-    "CreateWorkflowStepResponseTypeDef",
-    {
-        "id": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteMigrationWorkflowResponseTypeDef = TypedDict(
-    "DeleteMigrationWorkflowResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "status": MigrationWorkflowStatusEnumType,
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
 
-RetryWorkflowStepResponseTypeDef = TypedDict(
-    "RetryWorkflowStepResponseTypeDef",
+_RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
     {
-        "stepGroupId": str,
-        "workflowId": str,
         "id": str,
-        "status": StepStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-StartMigrationWorkflowResponseTypeDef = TypedDict(
-    "StartMigrationWorkflowResponseTypeDef",
+_OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMigrationWorkflowRequestRequestTypeDef",
     {
-        "id": str,
-        "arn": str,
-        "status": MigrationWorkflowStatusEnumType,
-        "statusMessage": str,
-        "lastStartTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "name": str,
+        "description": str,
+        "inputParameters": Mapping[str, StepInputTypeDef],
+        "stepTargets": Sequence[str],
     },
+    total=False,
 )
 
-StopMigrationWorkflowResponseTypeDef = TypedDict(
-    "StopMigrationWorkflowResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "status": MigrationWorkflowStatusEnumType,
-        "statusMessage": str,
-        "lastStopTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UpdateMigrationWorkflowRequestRequestTypeDef(
+    _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
+    _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
+):
+    pass
 
 UpdateMigrationWorkflowResponseTypeDef = TypedDict(
     "UpdateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
@@ -729,41 +851,30 @@
         "adsApplicationConfigurationId": str,
         "workflowInputs": Dict[str, StepInputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
         "lastModifiedTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateWorkflowStepResponseTypeDef = TypedDict(
-    "UpdateWorkflowStepResponseTypeDef",
-    {
-        "id": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateWorkflowStepGroupResponseTypeDef = TypedDict(
     "CreateWorkflowStepGroupResponseTypeDef",
     {
         "workflowId": str,
         "name": str,
         "id": str,
         "description": str,
         "tools": List[ToolTypeDef],
         "next": List[str],
         "previous": List[str],
         "creationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMigrationWorkflowResponseTypeDef = TypedDict(
     "GetMigrationWorkflowResponseTypeDef",
     {
         "id": str,
@@ -782,15 +893,15 @@
         "endTime": datetime,
         "tools": List[ToolTypeDef],
         "totalSteps": int,
         "completedSteps": int,
         "workflowInputs": Dict[str, StepInputTypeDef],
         "tags": Dict[str, str],
         "workflowBucket": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTemplateStepGroupResponseTypeDef = TypedDict(
     "GetTemplateStepGroupResponseTypeDef",
     {
         "templateId": str,
@@ -799,15 +910,15 @@
         "description": str,
         "status": StepGroupStatusType,
         "creationTime": datetime,
         "lastModifiedTime": datetime,
         "tools": List[ToolTypeDef],
         "previous": List[str],
         "next": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWorkflowStepGroupResponseTypeDef = TypedDict(
     "GetWorkflowStepGroupResponseTypeDef",
     {
         "id": str,
@@ -818,218 +929,107 @@
         "owner": OwnerType,
         "creationTime": datetime,
         "lastModifiedTime": datetime,
         "endTime": datetime,
         "tools": List[ToolTypeDef],
         "previous": List[str],
         "next": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateWorkflowStepGroupResponseTypeDef = TypedDict(
     "UpdateWorkflowStepGroupResponseTypeDef",
     {
         "workflowId": str,
         "name": str,
         "id": str,
         "description": str,
         "tools": List[ToolTypeDef],
         "next": List[str],
         "previous": List[str],
         "lastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMigrationWorkflowTemplateResponseTypeDef = TypedDict(
     "GetMigrationWorkflowTemplateResponseTypeDef",
     {
         "id": str,
         "name": str,
         "description": str,
         "inputs": List[TemplateInputTypeDef],
         "tools": List[ToolTypeDef],
         "status": Literal["CREATED"],
         "creationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
-    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
-    {
-        "name": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
-    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
-    {
-        "templateId": str,
-        "adsApplicationConfigurationName": str,
-        "status": MigrationWorkflowStatusEnumType,
-        "name": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ListPluginsRequestListPluginsPaginateTypeDef = TypedDict(
-    "ListPluginsRequestListPluginsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
-    {
-        "templateId": str,
-    },
-)
-_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef(
-    _RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
-    _OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
-):
-    pass
-
-_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
-    "_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
-    {
-        "templateId": str,
-        "stepGroupId": str,
-    },
-)
-_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
-    "_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTemplateStepsRequestListTemplateStepsPaginateTypeDef(
-    _RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
-    _OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
-):
-    pass
-
-_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
-    {
-        "workflowId": str,
-    },
-)
-_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef(
-    _RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
-    _OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
-):
-    pass
-
-_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
-    "_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
-    {
-        "workflowId": str,
-        "stepGroupId": str,
-    },
-)
-_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
-    "_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef(
-    _RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
-    _OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
-):
-    pass
-
 ListMigrationWorkflowTemplatesResponseTypeDef = TypedDict(
     "ListMigrationWorkflowTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "templateSummary": List[TemplateSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMigrationWorkflowsResponseTypeDef = TypedDict(
     "ListMigrationWorkflowsResponseTypeDef",
     {
         "nextToken": str,
         "migrationWorkflowSummary": List[MigrationWorkflowSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPluginsResponseTypeDef = TypedDict(
     "ListPluginsResponseTypeDef",
     {
         "nextToken": str,
         "plugins": List[PluginSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTemplateStepGroupsResponseTypeDef = TypedDict(
     "ListTemplateStepGroupsResponseTypeDef",
     {
         "nextToken": str,
         "templateStepGroupSummary": List[TemplateStepGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTemplateStepsResponseTypeDef = TypedDict(
     "ListTemplateStepsResponseTypeDef",
     {
         "nextToken": str,
         "templateStepSummaryList": List[TemplateStepSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkflowStepGroupsResponseTypeDef = TypedDict(
     "ListWorkflowStepGroupsResponseTypeDef",
     {
         "nextToken": str,
         "workflowStepGroupsSummary": List[WorkflowStepGroupSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorkflowStepsResponseTypeDef = TypedDict(
     "ListWorkflowStepsResponseTypeDef",
     {
         "nextToken": str,
         "workflowStepsSummary": List[WorkflowStepSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StepAutomationConfigurationTypeDef = TypedDict(
     "StepAutomationConfigurationTypeDef",
     {
         "scriptLocationS3Bucket": str,
@@ -1074,15 +1074,15 @@
         "description": str,
         "stepActionType": StepActionTypeType,
         "creationTime": str,
         "previous": List[str],
         "next": List[str],
         "outputs": List[StepOutputTypeDef],
         "stepAutomationConfiguration": StepAutomationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateWorkflowStepRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowStepRequestRequestTypeDef",
     {
         "name": str,
@@ -1130,15 +1130,15 @@
         "scriptOutputLocation": str,
         "creationTime": datetime,
         "lastStartTime": datetime,
         "endTime": datetime,
         "noOfSrvCompleted": int,
         "noOfSrvFailed": int,
         "totalNoOfSrv": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateWorkflowStepRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkflowStepRequestRequestTypeDef",
     {
         "id": str,
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO` & `mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhuborchestrator
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.MigrationHubOrchestrator 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.MigrationHubOrchestrator 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/
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
 
 <a id="mypy-boto3-migrationhuborchestrator"></a>
 
 # mypy-boto3-migrationhuborchestrator
 
 [![PyPI - mypy-boto3-migrationhuborchestrator](https://img.shields.io/pypi/v/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migrationhuborchestrator?color=blue)](https://pypistats.org/packages/mypy-boto3-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubOrchestrator 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[boto3.MigrationHubOrchestrator 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
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
 [mypy-boto3-migrationhuborchestrator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,77 +359,77 @@
 
 `mypy_boto3_migrationhuborchestrator.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhuborchestrator.type_defs import (
     StepInputTypeDef,
-    ResponseMetadataTypeDef,
     CreateWorkflowStepGroupRequestRequestTypeDef,
     ToolTypeDef,
+    CreateWorkflowStepResponseTypeDef,
     DeleteMigrationWorkflowRequestRequestTypeDef,
+    DeleteMigrationWorkflowResponseTypeDef,
     DeleteWorkflowStepGroupRequestRequestTypeDef,
     DeleteWorkflowStepRequestRequestTypeDef,
     GetMigrationWorkflowRequestRequestTypeDef,
     GetMigrationWorkflowTemplateRequestRequestTypeDef,
     TemplateInputTypeDef,
     GetTemplateStepGroupRequestRequestTypeDef,
     GetTemplateStepRequestRequestTypeDef,
     StepOutputTypeDef,
     GetWorkflowStepGroupRequestRequestTypeDef,
     GetWorkflowStepRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
     ListMigrationWorkflowTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
+    ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListMigrationWorkflowsRequestRequestTypeDef,
     MigrationWorkflowSummaryTypeDef,
+    ListPluginsRequestListPluginsPaginateTypeDef,
     ListPluginsRequestRequestTypeDef,
     PluginSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
     ListTemplateStepGroupsRequestRequestTypeDef,
     TemplateStepGroupSummaryTypeDef,
+    ListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
     ListTemplateStepsRequestRequestTypeDef,
     TemplateStepSummaryTypeDef,
+    ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
     ListWorkflowStepGroupsRequestRequestTypeDef,
     WorkflowStepGroupSummaryTypeDef,
+    ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
     ListWorkflowStepsRequestRequestTypeDef,
     WorkflowStepSummaryTypeDef,
+    PaginatorConfigTypeDef,
     PlatformCommandTypeDef,
     PlatformScriptKeyTypeDef,
+    ResponseMetadataTypeDef,
     RetryWorkflowStepRequestRequestTypeDef,
+    RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowRequestRequestTypeDef,
+    StartMigrationWorkflowResponseTypeDef,
     StopMigrationWorkflowRequestRequestTypeDef,
+    StopMigrationWorkflowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWorkflowStepGroupRequestRequestTypeDef,
+    UpdateWorkflowStepResponseTypeDef,
     WorkflowStepOutputUnionTypeDef,
     CreateMigrationWorkflowRequestRequestTypeDef,
-    UpdateMigrationWorkflowRequestRequestTypeDef,
     CreateMigrationWorkflowResponseTypeDef,
-    CreateWorkflowStepResponseTypeDef,
-    DeleteMigrationWorkflowResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RetryWorkflowStepResponseTypeDef,
-    StartMigrationWorkflowResponseTypeDef,
-    StopMigrationWorkflowResponseTypeDef,
+    UpdateMigrationWorkflowRequestRequestTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
-    UpdateWorkflowStepResponseTypeDef,
     CreateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowResponseTypeDef,
     GetTemplateStepGroupResponseTypeDef,
     GetWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowTemplateResponseTypeDef,
-    ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
-    ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef,
-    ListPluginsRequestListPluginsPaginateTypeDef,
-    ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
-    ListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
-    ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
-    ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
     ListMigrationWorkflowTemplatesResponseTypeDef,
     ListMigrationWorkflowsResponseTypeDef,
     ListPluginsResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
@@ -449,42 +450,42 @@
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

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt` & `mypy-boto3-migrationhuborchestrator-1.27.0/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.26.0.post1/setup.py` & `mypy-boto3-migrationhuborchestrator-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 """
 Setup script for mypy-boto3-migrationhuborchestrator.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migrationhuborchestrator",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_migrationhuborchestrator"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubOrchestrator 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.MigrationHubOrchestrator 1.27.0 service generated with"
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
         "boto3 migrationhuborchestrator type-annotations boto3-stubs mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_migrationhuborchestrator": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_migrationhuborchestrator": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/"
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


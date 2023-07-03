# Comparing `tmp/mypy-boto3-databrew-1.26.56.tar.gz` & `tmp/mypy-boto3-databrew-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-databrew-1.26.56.tar", last modified: Tue Jan 24 20:25:10 2023, max compression
+gzip compressed data, was "mypy-boto3-databrew-1.27.0.tar", last modified: Mon Jul  3 19:50:37 2023, max compression
```

## Comparing `mypy-boto3-databrew-1.26.56.tar` & `mypy-boto3-databrew-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:25:10.920532 mypy-boto3-databrew-1.26.56/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-24 20:24:56.000000 mypy-boto3-databrew-1.26.56/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19013 2023-01-24 20:25:10.920532 mypy-boto3-databrew-1.26.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-01-24 20:24:56.000000 mypy-boto3-databrew-1.26.56/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:25:10.920532 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-01-24 20:24:56.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-01-24 20:24:56.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-24 20:24:56.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33794 2023-01-24 20:24:56.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33735 2023-01-24 20:24:56.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-01-24 20:24:56.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-01-24 20:24:56.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-01-24 20:24:56.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-01-24 20:24:56.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:24:56.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54072 2023-01-24 20:24:58.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53974 2023-01-24 20:24:57.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-24 20:24:56.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:25:10.920532 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19013 2023-01-24 20:25:10.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-01-24 20:25:10.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 20:25:10.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 20:25:10.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-24 20:25:10.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-24 20:25:10.000000 mypy-boto3-databrew-1.26.56/mypy_boto3_databrew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 20:25:10.920532 mypy-boto3-databrew-1.26.56/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-01-24 20:24:56.000000 mypy-boto3-databrew-1.26.56/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:37.943096 mypy-boto3-databrew-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:13.000000 mypy-boto3-databrew-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-07-03 19:50:37.943096 mypy-boto3-databrew-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-07-03 19:35:13.000000 mypy-boto3-databrew-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:37.943096 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-03 19:35:13.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-03 19:35:13.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:35:13.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-07-03 19:35:14.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33726 2023-07-03 19:35:14.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-07-03 19:35:14.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-07-03 19:35:14.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-03 19:35:14.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-07-03 19:35:14.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:13.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54172 2023-07-03 19:35:15.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54074 2023-07-03 19:35:14.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:13.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:37.943096 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-07-03 19:50:37.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 19:50:37.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:37.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:37.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:37.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:50:37.000000 mypy-boto3-databrew-1.27.0/mypy_boto3_databrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:37.943096 mypy-boto3-databrew-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-03 19:35:13.000000 mypy-boto3-databrew-1.27.0/setup.py
```

### Comparing `mypy-boto3-databrew-1.26.56/LICENSE` & `mypy-boto3-databrew-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-databrew-1.26.56/PKG-INFO` & `mypy-boto3-databrew-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-databrew
-Version: 1.26.56
-Summary: Type annotations for boto3.GlueDataBrew 1.26.56 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.GlueDataBrew 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-databrew"></a>
 
 # mypy-boto3-databrew
 
 [![PyPI - mypy-boto3-databrew](https://img.shields.io/pypi/v/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-databrew?color=blue)](https://pypistats.org/packages/mypy-boto3-databrew)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlueDataBrew 1.26.56](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
+[boto3.GlueDataBrew 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
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
 [mypy-boto3-databrew docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,115 +365,115 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_databrew.type_defs import (
     AllowedStatisticsTypeDef,
     BatchDeleteRecipeVersionRequestRequestTypeDef,
     RecipeVersionErrorDetailTypeDef,
-    ResponseMetadataTypeDef,
     ColumnSelectorTypeDef,
     ConditionExpressionTypeDef,
+    CreateDatasetResponseTypeDef,
     JobSampleTypeDef,
     S3LocationTypeDef,
     ValidationConfigurationTypeDef,
+    CreateProfileJobResponseTypeDef,
     SampleTypeDef,
+    CreateProjectResponseTypeDef,
     RecipeReferenceTypeDef,
+    CreateRecipeJobResponseTypeDef,
+    CreateRecipeResponseTypeDef,
+    CreateRulesetResponseTypeDef,
     CreateScheduleRequestRequestTypeDef,
+    CreateScheduleResponseTypeDef,
     CsvOptionsTypeDef,
     CsvOutputOptionsTypeDef,
     DatetimeOptionsTypeDef,
     FilterExpressionTypeDef,
     DeleteDatasetRequestRequestTypeDef,
+    DeleteDatasetResponseTypeDef,
     DeleteJobRequestRequestTypeDef,
+    DeleteJobResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
+    DeleteProjectResponseTypeDef,
     DeleteRecipeVersionRequestRequestTypeDef,
+    DeleteRecipeVersionResponseTypeDef,
     DeleteRulesetRequestRequestTypeDef,
+    DeleteRulesetResponseTypeDef,
     DeleteScheduleRequestRequestTypeDef,
+    DeleteScheduleResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DescribeRecipeRequestRequestTypeDef,
     DescribeRulesetRequestRequestTypeDef,
     DescribeScheduleRequestRequestTypeDef,
+    DescribeScheduleResponseTypeDef,
     ExcelOptionsTypeDef,
     FilesLimitTypeDef,
     JsonOptionsTypeDef,
     MetadataTypeDef,
-    PaginatorConfigTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
+    ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
     ListRecipeVersionsRequestRequestTypeDef,
+    ListRecipesRequestListRecipesPaginateTypeDef,
     ListRecipesRequestRequestTypeDef,
+    ListRulesetsRequestListRulesetsPaginateTypeDef,
     ListRulesetsRequestRequestTypeDef,
     RulesetItemTypeDef,
+    ListSchedulesRequestListSchedulesPaginateTypeDef,
     ListSchedulesRequestRequestTypeDef,
     ScheduleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PublishRecipeRequestRequestTypeDef,
+    PublishRecipeResponseTypeDef,
     RecipeActionTypeDef,
+    ResponseMetadataTypeDef,
     ThresholdTypeDef,
     ViewFrameTypeDef,
+    SendProjectSessionActionResponseTypeDef,
     StartJobRunRequestRequestTypeDef,
+    StartJobRunResponseTypeDef,
     StartProjectSessionRequestRequestTypeDef,
+    StartProjectSessionResponseTypeDef,
     StatisticOverrideTypeDef,
     StopJobRunRequestRequestTypeDef,
+    StopJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateScheduleRequestRequestTypeDef,
-    EntityDetectorConfigurationTypeDef,
-    BatchDeleteRecipeVersionResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateProfileJobResponseTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateRecipeJobResponseTypeDef,
-    CreateRecipeResponseTypeDef,
-    CreateRulesetResponseTypeDef,
-    CreateScheduleResponseTypeDef,
-    DeleteDatasetResponseTypeDef,
-    DeleteJobResponseTypeDef,
-    DeleteProjectResponseTypeDef,
-    DeleteRecipeVersionResponseTypeDef,
-    DeleteRulesetResponseTypeDef,
-    DeleteScheduleResponseTypeDef,
-    DescribeScheduleResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PublishRecipeResponseTypeDef,
-    SendProjectSessionActionResponseTypeDef,
-    StartJobRunResponseTypeDef,
-    StartProjectSessionResponseTypeDef,
-    StopJobRunResponseTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdateProfileJobResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateRecipeJobResponseTypeDef,
     UpdateRecipeResponseTypeDef,
     UpdateRulesetResponseTypeDef,
+    UpdateScheduleRequestRequestTypeDef,
     UpdateScheduleResponseTypeDef,
+    EntityDetectorConfigurationTypeDef,
+    BatchDeleteRecipeVersionResponseTypeDef,
     DataCatalogInputDefinitionTypeDef,
     DatabaseInputDefinitionTypeDef,
     DatabaseTableOutputOptionsTypeDef,
     S3TableOutputOptionsTypeDef,
     CreateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
     ProjectTypeDef,
     UpdateProjectRequestRequestTypeDef,
     OutputFormatOptionsTypeDef,
     DatasetParameterTypeDef,
     FormatOptionsTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
-    ListRecipesRequestListRecipesPaginateTypeDef,
-    ListRulesetsRequestListRulesetsPaginateTypeDef,
-    ListSchedulesRequestListSchedulesPaginateTypeDef,
     ListRulesetsResponseTypeDef,
     ListSchedulesResponseTypeDef,
     RecipeStepTypeDef,
     RuleTypeDef,
     StatisticsConfigurationTypeDef,
     InputTypeDef,
     DatabaseOutputTypeDef,
@@ -518,42 +518,42 @@
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

### Comparing `mypy-boto3-databrew-1.26.56/README.md` & `mypy-boto3-databrew-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-databrew"></a>
 
 # mypy-boto3-databrew
 
 [![PyPI - mypy-boto3-databrew](https://img.shields.io/pypi/v/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-databrew?color=blue)](https://pypistats.org/packages/mypy-boto3-databrew)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlueDataBrew 1.26.56](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
+[boto3.GlueDataBrew 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
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
 [mypy-boto3-databrew docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,115 +333,115 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_databrew.type_defs import (
     AllowedStatisticsTypeDef,
     BatchDeleteRecipeVersionRequestRequestTypeDef,
     RecipeVersionErrorDetailTypeDef,
-    ResponseMetadataTypeDef,
     ColumnSelectorTypeDef,
     ConditionExpressionTypeDef,
+    CreateDatasetResponseTypeDef,
     JobSampleTypeDef,
     S3LocationTypeDef,
     ValidationConfigurationTypeDef,
+    CreateProfileJobResponseTypeDef,
     SampleTypeDef,
+    CreateProjectResponseTypeDef,
     RecipeReferenceTypeDef,
+    CreateRecipeJobResponseTypeDef,
+    CreateRecipeResponseTypeDef,
+    CreateRulesetResponseTypeDef,
     CreateScheduleRequestRequestTypeDef,
+    CreateScheduleResponseTypeDef,
     CsvOptionsTypeDef,
     CsvOutputOptionsTypeDef,
     DatetimeOptionsTypeDef,
     FilterExpressionTypeDef,
     DeleteDatasetRequestRequestTypeDef,
+    DeleteDatasetResponseTypeDef,
     DeleteJobRequestRequestTypeDef,
+    DeleteJobResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
+    DeleteProjectResponseTypeDef,
     DeleteRecipeVersionRequestRequestTypeDef,
+    DeleteRecipeVersionResponseTypeDef,
     DeleteRulesetRequestRequestTypeDef,
+    DeleteRulesetResponseTypeDef,
     DeleteScheduleRequestRequestTypeDef,
+    DeleteScheduleResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DescribeRecipeRequestRequestTypeDef,
     DescribeRulesetRequestRequestTypeDef,
     DescribeScheduleRequestRequestTypeDef,
+    DescribeScheduleResponseTypeDef,
     ExcelOptionsTypeDef,
     FilesLimitTypeDef,
     JsonOptionsTypeDef,
     MetadataTypeDef,
-    PaginatorConfigTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
+    ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
     ListRecipeVersionsRequestRequestTypeDef,
+    ListRecipesRequestListRecipesPaginateTypeDef,
     ListRecipesRequestRequestTypeDef,
+    ListRulesetsRequestListRulesetsPaginateTypeDef,
     ListRulesetsRequestRequestTypeDef,
     RulesetItemTypeDef,
+    ListSchedulesRequestListSchedulesPaginateTypeDef,
     ListSchedulesRequestRequestTypeDef,
     ScheduleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PublishRecipeRequestRequestTypeDef,
+    PublishRecipeResponseTypeDef,
     RecipeActionTypeDef,
+    ResponseMetadataTypeDef,
     ThresholdTypeDef,
     ViewFrameTypeDef,
+    SendProjectSessionActionResponseTypeDef,
     StartJobRunRequestRequestTypeDef,
+    StartJobRunResponseTypeDef,
     StartProjectSessionRequestRequestTypeDef,
+    StartProjectSessionResponseTypeDef,
     StatisticOverrideTypeDef,
     StopJobRunRequestRequestTypeDef,
+    StopJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateScheduleRequestRequestTypeDef,
-    EntityDetectorConfigurationTypeDef,
-    BatchDeleteRecipeVersionResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateProfileJobResponseTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateRecipeJobResponseTypeDef,
-    CreateRecipeResponseTypeDef,
-    CreateRulesetResponseTypeDef,
-    CreateScheduleResponseTypeDef,
-    DeleteDatasetResponseTypeDef,
-    DeleteJobResponseTypeDef,
-    DeleteProjectResponseTypeDef,
-    DeleteRecipeVersionResponseTypeDef,
-    DeleteRulesetResponseTypeDef,
-    DeleteScheduleResponseTypeDef,
-    DescribeScheduleResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PublishRecipeResponseTypeDef,
-    SendProjectSessionActionResponseTypeDef,
-    StartJobRunResponseTypeDef,
-    StartProjectSessionResponseTypeDef,
-    StopJobRunResponseTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdateProfileJobResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateRecipeJobResponseTypeDef,
     UpdateRecipeResponseTypeDef,
     UpdateRulesetResponseTypeDef,
+    UpdateScheduleRequestRequestTypeDef,
     UpdateScheduleResponseTypeDef,
+    EntityDetectorConfigurationTypeDef,
+    BatchDeleteRecipeVersionResponseTypeDef,
     DataCatalogInputDefinitionTypeDef,
     DatabaseInputDefinitionTypeDef,
     DatabaseTableOutputOptionsTypeDef,
     S3TableOutputOptionsTypeDef,
     CreateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
     ProjectTypeDef,
     UpdateProjectRequestRequestTypeDef,
     OutputFormatOptionsTypeDef,
     DatasetParameterTypeDef,
     FormatOptionsTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
-    ListRecipesRequestListRecipesPaginateTypeDef,
-    ListRulesetsRequestListRulesetsPaginateTypeDef,
-    ListSchedulesRequestListSchedulesPaginateTypeDef,
     ListRulesetsResponseTypeDef,
     ListSchedulesResponseTypeDef,
     RecipeStepTypeDef,
     RuleTypeDef,
     StatisticsConfigurationTypeDef,
     InputTypeDef,
     DatabaseOutputTypeDef,
@@ -486,42 +486,42 @@
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

### Comparing `mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/__init__.py` & `mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/__init__.pyi` & `mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/__main__.py` & `mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GlueDataBrew 1.26.56\nVersion:         1.26.56\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.GlueDataBrew 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.56")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/client.py` & `mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,16 +461,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#list_projects)
         """
 
     def list_recipe_versions(
         self, *, Name: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListRecipeVersionsResponseTypeDef:
         """
-        Lists the versions of a particular DataBrew recipe, except for `LATEST_WORKING`
-        .
+        Lists the versions of a particular DataBrew recipe, except for `LATEST_WORKING`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.list_recipe_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#list_recipe_versions)
         """
 
     def list_recipes(
         self, *, MaxResults: int = ..., NextToken: str = ..., RecipeVersion: str = ...
```

### Comparing `mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/client.pyi` & `mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -428,16 +428,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.list_projects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#list_projects)
         """
     def list_recipe_versions(
         self, *, Name: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListRecipeVersionsResponseTypeDef:
         """
-        Lists the versions of a particular DataBrew recipe, except for `LATEST_WORKING`
-        .
+        Lists the versions of a particular DataBrew recipe, except for `LATEST_WORKING`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.list_recipe_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#list_recipe_versions)
         """
     def list_recipes(
         self, *, MaxResults: int = ..., NextToken: str = ..., RecipeVersion: str = ...
     ) -> ListRecipesResponseTypeDef:
```

### Comparing `mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/literals.py` & `mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
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
@@ -152,21 +153,23 @@
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
@@ -245,14 +248,15 @@
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
@@ -263,14 +267,15 @@
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
@@ -306,14 +311,15 @@
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
@@ -332,16 +338,19 @@
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
@@ -421,18 +430,21 @@
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

### Comparing `mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/literals.pyi` & `mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
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
@@ -150,21 +151,23 @@
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
@@ -243,14 +246,15 @@
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
@@ -261,14 +265,15 @@
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
@@ -304,14 +309,15 @@
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
@@ -330,16 +336,19 @@
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
@@ -419,18 +428,21 @@
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

### Comparing `mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/paginator.py` & `mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,30 +74,30 @@
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listdatasetspaginator)
         """
 
 
 class ListJobRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listjobrunspaginator)
     """
 
     def paginate(
-        self, *, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listjobrunspaginator)
         """
 
 
@@ -108,88 +108,88 @@
     """
 
     def paginate(
         self,
         *,
         DatasetName: str = ...,
         ProjectName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listjobspaginator)
         """
 
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listprojectspaginator)
         """
 
 
 class ListRecipeVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipeVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipeversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecipeVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipeVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipeversionspaginator)
         """
 
 
 class ListRecipesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipespaginator)
     """
 
     def paginate(
-        self, *, RecipeVersion: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, RecipeVersion: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipespaginator)
         """
 
 
 class ListRulesetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRulesets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrulesetspaginator)
     """
 
     def paginate(
-        self, *, TargetArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TargetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRulesetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRulesets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrulesetspaginator)
         """
 
 
 class ListSchedulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListSchedules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listschedulespaginator)
     """
 
     def paginate(
-        self, *, JobName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, JobName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchedulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listschedulespaginator)
         """
```

### Comparing `mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/paginator.pyi` & `mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -71,29 +71,29 @@
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listdatasetspaginator)
         """
 
 class ListJobRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listjobrunspaginator)
     """
 
     def paginate(
-        self, *, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listjobrunspaginator)
         """
 
 class ListJobsPaginator(Paginator):
@@ -103,83 +103,83 @@
     """
 
     def paginate(
         self,
         *,
         DatasetName: str = ...,
         ProjectName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listjobspaginator)
         """
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listprojectspaginator)
         """
 
 class ListRecipeVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipeVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipeversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecipeVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipeVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipeversionspaginator)
         """
 
 class ListRecipesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipespaginator)
     """
 
     def paginate(
-        self, *, RecipeVersion: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, RecipeVersion: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRecipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipespaginator)
         """
 
 class ListRulesetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRulesets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrulesetspaginator)
     """
 
     def paginate(
-        self, *, TargetArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, TargetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRulesetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRulesets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrulesetspaginator)
         """
 
 class ListSchedulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListSchedules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listschedulespaginator)
     """
 
     def paginate(
-        self, *, JobName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, JobName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchedulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listschedulespaginator)
         """
```

### Comparing `mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/type_defs.py` & `mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,115 +44,115 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AllowedStatisticsTypeDef",
     "BatchDeleteRecipeVersionRequestRequestTypeDef",
     "RecipeVersionErrorDetailTypeDef",
-    "ResponseMetadataTypeDef",
     "ColumnSelectorTypeDef",
     "ConditionExpressionTypeDef",
+    "CreateDatasetResponseTypeDef",
     "JobSampleTypeDef",
     "S3LocationTypeDef",
     "ValidationConfigurationTypeDef",
+    "CreateProfileJobResponseTypeDef",
     "SampleTypeDef",
+    "CreateProjectResponseTypeDef",
     "RecipeReferenceTypeDef",
+    "CreateRecipeJobResponseTypeDef",
+    "CreateRecipeResponseTypeDef",
+    "CreateRulesetResponseTypeDef",
     "CreateScheduleRequestRequestTypeDef",
+    "CreateScheduleResponseTypeDef",
     "CsvOptionsTypeDef",
     "CsvOutputOptionsTypeDef",
     "DatetimeOptionsTypeDef",
     "FilterExpressionTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
+    "DeleteDatasetResponseTypeDef",
     "DeleteJobRequestRequestTypeDef",
+    "DeleteJobResponseTypeDef",
     "DeleteProjectRequestRequestTypeDef",
+    "DeleteProjectResponseTypeDef",
     "DeleteRecipeVersionRequestRequestTypeDef",
+    "DeleteRecipeVersionResponseTypeDef",
     "DeleteRulesetRequestRequestTypeDef",
+    "DeleteRulesetResponseTypeDef",
     "DeleteScheduleRequestRequestTypeDef",
+    "DeleteScheduleResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DescribeRecipeRequestRequestTypeDef",
     "DescribeRulesetRequestRequestTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
+    "DescribeScheduleResponseTypeDef",
     "ExcelOptionsTypeDef",
     "FilesLimitTypeDef",
     "JsonOptionsTypeDef",
     "MetadataTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
+    "ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     "ListRecipeVersionsRequestRequestTypeDef",
+    "ListRecipesRequestListRecipesPaginateTypeDef",
     "ListRecipesRequestRequestTypeDef",
+    "ListRulesetsRequestListRulesetsPaginateTypeDef",
     "ListRulesetsRequestRequestTypeDef",
     "RulesetItemTypeDef",
+    "ListSchedulesRequestListSchedulesPaginateTypeDef",
     "ListSchedulesRequestRequestTypeDef",
     "ScheduleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PublishRecipeRequestRequestTypeDef",
+    "PublishRecipeResponseTypeDef",
     "RecipeActionTypeDef",
+    "ResponseMetadataTypeDef",
     "ThresholdTypeDef",
     "ViewFrameTypeDef",
+    "SendProjectSessionActionResponseTypeDef",
     "StartJobRunRequestRequestTypeDef",
+    "StartJobRunResponseTypeDef",
     "StartProjectSessionRequestRequestTypeDef",
+    "StartProjectSessionResponseTypeDef",
     "StatisticOverrideTypeDef",
     "StopJobRunRequestRequestTypeDef",
+    "StopJobRunResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateScheduleRequestRequestTypeDef",
-    "EntityDetectorConfigurationTypeDef",
-    "BatchDeleteRecipeVersionResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateProfileJobResponseTypeDef",
-    "CreateProjectResponseTypeDef",
-    "CreateRecipeJobResponseTypeDef",
-    "CreateRecipeResponseTypeDef",
-    "CreateRulesetResponseTypeDef",
-    "CreateScheduleResponseTypeDef",
-    "DeleteDatasetResponseTypeDef",
-    "DeleteJobResponseTypeDef",
-    "DeleteProjectResponseTypeDef",
-    "DeleteRecipeVersionResponseTypeDef",
-    "DeleteRulesetResponseTypeDef",
-    "DeleteScheduleResponseTypeDef",
-    "DescribeScheduleResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PublishRecipeResponseTypeDef",
-    "SendProjectSessionActionResponseTypeDef",
-    "StartJobRunResponseTypeDef",
-    "StartProjectSessionResponseTypeDef",
-    "StopJobRunResponseTypeDef",
     "UpdateDatasetResponseTypeDef",
     "UpdateProfileJobResponseTypeDef",
     "UpdateProjectResponseTypeDef",
     "UpdateRecipeJobResponseTypeDef",
     "UpdateRecipeResponseTypeDef",
     "UpdateRulesetResponseTypeDef",
+    "UpdateScheduleRequestRequestTypeDef",
     "UpdateScheduleResponseTypeDef",
+    "EntityDetectorConfigurationTypeDef",
+    "BatchDeleteRecipeVersionResponseTypeDef",
     "DataCatalogInputDefinitionTypeDef",
     "DatabaseInputDefinitionTypeDef",
     "DatabaseTableOutputOptionsTypeDef",
     "S3TableOutputOptionsTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
     "ProjectTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "OutputFormatOptionsTypeDef",
     "DatasetParameterTypeDef",
     "FormatOptionsTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    "ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
-    "ListRecipesRequestListRecipesPaginateTypeDef",
-    "ListRulesetsRequestListRulesetsPaginateTypeDef",
-    "ListSchedulesRequestListSchedulesPaginateTypeDef",
     "ListRulesetsResponseTypeDef",
     "ListSchedulesResponseTypeDef",
     "RecipeStepTypeDef",
     "RuleTypeDef",
     "StatisticsConfigurationTypeDef",
     "InputTypeDef",
     "DatabaseOutputTypeDef",
@@ -210,25 +210,14 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "RecipeVersion": str,
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
 ColumnSelectorTypeDef = TypedDict(
     "ColumnSelectorTypeDef",
     {
         "Regex": str,
         "Name": str,
     },
     total=False,
@@ -252,14 +241,22 @@
 
 class ConditionExpressionTypeDef(
     _RequiredConditionExpressionTypeDef, _OptionalConditionExpressionTypeDef
 ):
     pass
 
 
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 JobSampleTypeDef = TypedDict(
     "JobSampleTypeDef",
     {
         "Mode": SampleModeType,
         "Size": int,
     },
     total=False,
@@ -302,14 +299,22 @@
 
 class ValidationConfigurationTypeDef(
     _RequiredValidationConfigurationTypeDef, _OptionalValidationConfigurationTypeDef
 ):
     pass
 
 
+CreateProfileJobResponseTypeDef = TypedDict(
+    "CreateProfileJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSampleTypeDef = TypedDict(
     "_RequiredSampleTypeDef",
     {
         "Type": SampleTypeType,
     },
 )
 _OptionalSampleTypeDef = TypedDict(
@@ -321,14 +326,22 @@
 )
 
 
 class SampleTypeDef(_RequiredSampleTypeDef, _OptionalSampleTypeDef):
     pass
 
 
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRecipeReferenceTypeDef = TypedDict(
     "_RequiredRecipeReferenceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalRecipeReferenceTypeDef = TypedDict(
@@ -340,14 +353,38 @@
 )
 
 
 class RecipeReferenceTypeDef(_RequiredRecipeReferenceTypeDef, _OptionalRecipeReferenceTypeDef):
     pass
 
 
+CreateRecipeJobResponseTypeDef = TypedDict(
+    "CreateRecipeJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateRecipeResponseTypeDef = TypedDict(
+    "CreateRecipeResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateRulesetResponseTypeDef = TypedDict(
+    "CreateRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScheduleRequestRequestTypeDef",
     {
         "CronExpression": str,
         "Name": str,
     },
 )
@@ -363,14 +400,22 @@
 
 class CreateScheduleRequestRequestTypeDef(
     _RequiredCreateScheduleRequestRequestTypeDef, _OptionalCreateScheduleRequestRequestTypeDef
 ):
     pass
 
 
+CreateScheduleResponseTypeDef = TypedDict(
+    "CreateScheduleResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
         "HeaderRow": bool,
     },
     total=False,
@@ -415,50 +460,99 @@
 DeleteDatasetRequestRequestTypeDef = TypedDict(
     "DeleteDatasetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteDatasetResponseTypeDef = TypedDict(
+    "DeleteDatasetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteJobRequestRequestTypeDef = TypedDict(
     "DeleteJobRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteJobResponseTypeDef = TypedDict(
+    "DeleteJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRecipeVersionRequestRequestTypeDef = TypedDict(
     "DeleteRecipeVersionRequestRequestTypeDef",
     {
         "Name": str,
         "RecipeVersion": str,
     },
 )
 
+DeleteRecipeVersionResponseTypeDef = TypedDict(
+    "DeleteRecipeVersionResponseTypeDef",
+    {
+        "Name": str,
+        "RecipeVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRulesetRequestRequestTypeDef = TypedDict(
     "DeleteRulesetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteRulesetResponseTypeDef = TypedDict(
+    "DeleteRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteScheduleRequestRequestTypeDef = TypedDict(
     "DeleteScheduleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteScheduleResponseTypeDef = TypedDict(
+    "DeleteScheduleResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -515,14 +609,30 @@
 DescribeScheduleRequestRequestTypeDef = TypedDict(
     "DescribeScheduleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DescribeScheduleResponseTypeDef = TypedDict(
+    "DescribeScheduleResponseTypeDef",
+    {
+        "CreateDate": datetime,
+        "CreatedBy": str,
+        "JobNames": List[str],
+        "LastModifiedBy": str,
+        "LastModifiedDate": datetime,
+        "ResourceArn": str,
+        "CronExpression": str,
+        "Tags": Dict[str, str],
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExcelOptionsTypeDef = TypedDict(
     "ExcelOptionsTypeDef",
     {
         "SheetNames": Sequence[str],
         "SheetIndexes": Sequence[int],
         "HeaderRow": bool,
     },
@@ -561,33 +671,53 @@
     "MetadataTypeDef",
     {
         "SourceArn": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListJobRunsRequestListJobRunsPaginateTypeDef(
+    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
+    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -602,34 +732,74 @@
 
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
 
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "DatasetName": str,
+        "ProjectName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "DatasetName": str,
         "MaxResults": int,
         "NextToken": str,
         "ProjectName": str,
     },
     total=False,
 )
 
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef(
+    _RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
+    _OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRecipeVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecipeVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListRecipeVersionsRequestRequestTypeDef = TypedDict(
@@ -645,24 +815,42 @@
 class ListRecipeVersionsRequestRequestTypeDef(
     _RequiredListRecipeVersionsRequestRequestTypeDef,
     _OptionalListRecipeVersionsRequestRequestTypeDef,
 ):
     pass
 
 
+ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
+    "ListRecipesRequestListRecipesPaginateTypeDef",
+    {
+        "RecipeVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRecipesRequestRequestTypeDef = TypedDict(
     "ListRecipesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "RecipeVersion": str,
     },
     total=False,
 )
 
+ListRulesetsRequestListRulesetsPaginateTypeDef = TypedDict(
+    "ListRulesetsRequestListRulesetsPaginateTypeDef",
+    {
+        "TargetArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRulesetsRequestRequestTypeDef = TypedDict(
     "ListRulesetsRequestRequestTypeDef",
     {
         "TargetArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -693,14 +881,23 @@
 )
 
 
 class RulesetItemTypeDef(_RequiredRulesetItemTypeDef, _OptionalRulesetItemTypeDef):
     pass
 
 
+ListSchedulesRequestListSchedulesPaginateTypeDef = TypedDict(
+    "ListSchedulesRequestListSchedulesPaginateTypeDef",
+    {
+        "JobName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSchedulesRequestRequestTypeDef = TypedDict(
     "ListSchedulesRequestRequestTypeDef",
     {
         "JobName": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -737,14 +934,32 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
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
 _RequiredPublishRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredPublishRecipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalPublishRecipeRequestRequestTypeDef = TypedDict(
@@ -758,14 +973,22 @@
 
 class PublishRecipeRequestRequestTypeDef(
     _RequiredPublishRecipeRequestRequestTypeDef, _OptionalPublishRecipeRequestRequestTypeDef
 ):
     pass
 
 
+PublishRecipeResponseTypeDef = TypedDict(
+    "PublishRecipeResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRecipeActionTypeDef = TypedDict(
     "_RequiredRecipeActionTypeDef",
     {
         "Operation": str,
     },
 )
 _OptionalRecipeActionTypeDef = TypedDict(
@@ -777,14 +1000,25 @@
 )
 
 
 class RecipeActionTypeDef(_RequiredRecipeActionTypeDef, _OptionalRecipeActionTypeDef):
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
 _RequiredThresholdTypeDef = TypedDict(
     "_RequiredThresholdTypeDef",
     {
         "Value": float,
     },
 )
 _OptionalThresholdTypeDef = TypedDict(
@@ -820,21 +1054,39 @@
 )
 
 
 class ViewFrameTypeDef(_RequiredViewFrameTypeDef, _OptionalViewFrameTypeDef):
     pass
 
 
+SendProjectSessionActionResponseTypeDef = TypedDict(
+    "SendProjectSessionActionResponseTypeDef",
+    {
+        "Result": str,
+        "Name": str,
+        "ActionId": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartJobRunRequestRequestTypeDef = TypedDict(
     "StartJobRunRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartProjectSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartProjectSessionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalStartProjectSessionRequestRequestTypeDef = TypedDict(
@@ -849,14 +1101,23 @@
 class StartProjectSessionRequestRequestTypeDef(
     _RequiredStartProjectSessionRequestRequestTypeDef,
     _OptionalStartProjectSessionRequestRequestTypeDef,
 ):
     pass
 
 
+StartProjectSessionResponseTypeDef = TypedDict(
+    "StartProjectSessionResponseTypeDef",
+    {
+        "Name": str,
+        "ClientSessionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StatisticOverrideTypeDef = TypedDict(
     "StatisticOverrideTypeDef",
     {
         "Statistic": str,
         "Parameters": Mapping[str, str],
     },
 )
@@ -865,14 +1126,22 @@
     "StopJobRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
 
+StopJobRunResponseTypeDef = TypedDict(
+    "StopJobRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -881,292 +1150,120 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredUpdateScheduleRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateScheduleRequestRequestTypeDef",
-    {
-        "CronExpression": str,
-        "Name": str,
-    },
-)
-_OptionalUpdateScheduleRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateScheduleRequestRequestTypeDef",
-    {
-        "JobNames": Sequence[str],
-    },
-    total=False,
-)
-
-
-class UpdateScheduleRequestRequestTypeDef(
-    _RequiredUpdateScheduleRequestRequestTypeDef, _OptionalUpdateScheduleRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredEntityDetectorConfigurationTypeDef = TypedDict(
-    "_RequiredEntityDetectorConfigurationTypeDef",
-    {
-        "EntityTypes": Sequence[str],
-    },
-)
-_OptionalEntityDetectorConfigurationTypeDef = TypedDict(
-    "_OptionalEntityDetectorConfigurationTypeDef",
-    {
-        "AllowedStatistics": Sequence[AllowedStatisticsTypeDef],
-    },
-    total=False,
-)
-
-
-class EntityDetectorConfigurationTypeDef(
-    _RequiredEntityDetectorConfigurationTypeDef, _OptionalEntityDetectorConfigurationTypeDef
-):
-    pass
-
-
-BatchDeleteRecipeVersionResponseTypeDef = TypedDict(
-    "BatchDeleteRecipeVersionResponseTypeDef",
-    {
-        "Name": str,
-        "Errors": List[RecipeVersionErrorDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProfileJobResponseTypeDef = TypedDict(
-    "CreateProfileJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRecipeJobResponseTypeDef = TypedDict(
-    "CreateRecipeJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRecipeResponseTypeDef = TypedDict(
-    "CreateRecipeResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRulesetResponseTypeDef = TypedDict(
-    "CreateRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateScheduleResponseTypeDef = TypedDict(
-    "CreateScheduleResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDatasetResponseTypeDef = TypedDict(
-    "DeleteDatasetResponseTypeDef",
+UpdateDatasetResponseTypeDef = TypedDict(
+    "UpdateDatasetResponseTypeDef",
     {
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteJobResponseTypeDef = TypedDict(
-    "DeleteJobResponseTypeDef",
+UpdateProfileJobResponseTypeDef = TypedDict(
+    "UpdateProfileJobResponseTypeDef",
     {
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
+UpdateProjectResponseTypeDef = TypedDict(
+    "UpdateProjectResponseTypeDef",
     {
+        "LastModifiedDate": datetime,
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRecipeVersionResponseTypeDef = TypedDict(
-    "DeleteRecipeVersionResponseTypeDef",
+UpdateRecipeJobResponseTypeDef = TypedDict(
+    "UpdateRecipeJobResponseTypeDef",
     {
         "Name": str,
-        "RecipeVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRulesetResponseTypeDef = TypedDict(
-    "DeleteRulesetResponseTypeDef",
+UpdateRecipeResponseTypeDef = TypedDict(
+    "UpdateRecipeResponseTypeDef",
     {
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteScheduleResponseTypeDef = TypedDict(
-    "DeleteScheduleResponseTypeDef",
+UpdateRulesetResponseTypeDef = TypedDict(
+    "UpdateRulesetResponseTypeDef",
     {
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeScheduleResponseTypeDef = TypedDict(
-    "DescribeScheduleResponseTypeDef",
+_RequiredUpdateScheduleRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateScheduleRequestRequestTypeDef",
     {
-        "CreateDate": datetime,
-        "CreatedBy": str,
-        "JobNames": List[str],
-        "LastModifiedBy": str,
-        "LastModifiedDate": datetime,
-        "ResourceArn": str,
         "CronExpression": str,
-        "Tags": Dict[str, str],
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PublishRecipeResponseTypeDef = TypedDict(
-    "PublishRecipeResponseTypeDef",
-    {
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-SendProjectSessionActionResponseTypeDef = TypedDict(
-    "SendProjectSessionActionResponseTypeDef",
+_OptionalUpdateScheduleRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateScheduleRequestRequestTypeDef",
     {
-        "Result": str,
-        "Name": str,
-        "ActionId": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobNames": Sequence[str],
     },
+    total=False,
 )
 
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-StartProjectSessionResponseTypeDef = TypedDict(
-    "StartProjectSessionResponseTypeDef",
-    {
-        "Name": str,
-        "ClientSessionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UpdateScheduleRequestRequestTypeDef(
+    _RequiredUpdateScheduleRequestRequestTypeDef, _OptionalUpdateScheduleRequestRequestTypeDef
+):
+    pass
 
-StopJobRunResponseTypeDef = TypedDict(
-    "StopJobRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpdateDatasetResponseTypeDef = TypedDict(
-    "UpdateDatasetResponseTypeDef",
+UpdateScheduleResponseTypeDef = TypedDict(
+    "UpdateScheduleResponseTypeDef",
     {
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateProfileJobResponseTypeDef = TypedDict(
-    "UpdateProfileJobResponseTypeDef",
+_RequiredEntityDetectorConfigurationTypeDef = TypedDict(
+    "_RequiredEntityDetectorConfigurationTypeDef",
     {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "EntityTypes": Sequence[str],
     },
 )
-
-UpdateProjectResponseTypeDef = TypedDict(
-    "UpdateProjectResponseTypeDef",
+_OptionalEntityDetectorConfigurationTypeDef = TypedDict(
+    "_OptionalEntityDetectorConfigurationTypeDef",
     {
-        "LastModifiedDate": datetime,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AllowedStatistics": Sequence[AllowedStatisticsTypeDef],
     },
+    total=False,
 )
 
-UpdateRecipeJobResponseTypeDef = TypedDict(
-    "UpdateRecipeJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpdateRecipeResponseTypeDef = TypedDict(
-    "UpdateRecipeResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class EntityDetectorConfigurationTypeDef(
+    _RequiredEntityDetectorConfigurationTypeDef, _OptionalEntityDetectorConfigurationTypeDef
+):
+    pass
 
-UpdateRulesetResponseTypeDef = TypedDict(
-    "UpdateRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpdateScheduleResponseTypeDef = TypedDict(
-    "UpdateScheduleResponseTypeDef",
+BatchDeleteRecipeVersionResponseTypeDef = TypedDict(
+    "BatchDeleteRecipeVersionResponseTypeDef",
     {
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Errors": List[RecipeVersionErrorDetailTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDataCatalogInputDefinitionTypeDef = TypedDict(
     "_RequiredDataCatalogInputDefinitionTypeDef",
     {
         "DatabaseName": str,
@@ -1278,15 +1375,15 @@
         "ResourceArn": str,
         "Sample": SampleTypeDef,
         "RoleArn": str,
         "Tags": Dict[str, str],
         "SessionStatus": SessionStatusType,
         "OpenedBy": str,
         "OpenDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredProjectTypeDef = TypedDict(
     "_RequiredProjectTypeDef",
     {
         "Name": str,
@@ -1375,126 +1472,29 @@
         "Json": JsonOptionsTypeDef,
         "Excel": ExcelOptionsTypeDef,
         "Csv": CsvOptionsTypeDef,
     },
     total=False,
 )
 
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListJobRunsRequestListJobRunsPaginateTypeDef(
-    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
-    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
-):
-    pass
-
-
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "DatasetName": str,
-        "ProjectName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef(
-    _RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
-    _OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
-    "ListRecipesRequestListRecipesPaginateTypeDef",
-    {
-        "RecipeVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRulesetsRequestListRulesetsPaginateTypeDef = TypedDict(
-    "ListRulesetsRequestListRulesetsPaginateTypeDef",
-    {
-        "TargetArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSchedulesRequestListSchedulesPaginateTypeDef = TypedDict(
-    "ListSchedulesRequestListSchedulesPaginateTypeDef",
-    {
-        "JobName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListRulesetsResponseTypeDef = TypedDict(
     "ListRulesetsResponseTypeDef",
     {
         "Rulesets": List[RulesetItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSchedulesResponseTypeDef = TypedDict(
     "ListSchedulesResponseTypeDef",
     {
         "Schedules": List[ScheduleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRecipeStepTypeDef = TypedDict(
     "_RequiredRecipeStepTypeDef",
     {
         "Action": RecipeActionTypeDef,
@@ -1602,15 +1602,15 @@
 
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "Projects": List[ProjectTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredOutputTypeDef = TypedDict(
     "_RequiredOutputTypeDef",
     {
         "Location": S3LocationTypeDef,
@@ -1679,15 +1679,15 @@
         "PublishedDate": datetime,
         "Description": str,
         "Name": str,
         "Steps": List[RecipeStepTypeDef],
         "Tags": Dict[str, str],
         "ResourceArn": str,
         "RecipeVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRecipeTypeDef = TypedDict(
     "_RequiredRecipeTypeDef",
     {
         "Name": str,
@@ -1798,15 +1798,15 @@
         "Rules": List[RuleTypeDef],
         "CreateDate": datetime,
         "CreatedBy": str,
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
         "ResourceArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRulesetRequestRequestTypeDef",
     {
         "Name": str,
@@ -2045,15 +2045,15 @@
         "Input": InputTypeDef,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "Source": SourceType,
         "PathOptions": PathOptionsTypeDef,
         "Tags": Dict[str, str],
         "ResourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "Name": str,
@@ -2078,24 +2078,24 @@
 
 
 ListRecipeVersionsResponseTypeDef = TypedDict(
     "ListRecipeVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Recipes": List[RecipeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecipesResponseTypeDef = TypedDict(
     "ListRecipesResponseTypeDef",
     {
         "Recipes": List[RecipeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProfileConfigurationTypeDef = TypedDict(
     "ProfileConfigurationTypeDef",
     {
         "DatasetStatisticsConfiguration": StatisticsConfigurationTypeDef,
@@ -2107,33 +2107,33 @@
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "JobRuns": List[JobRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateProfileJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfileJobRequestRequestTypeDef",
     {
         "DatasetName": str,
@@ -2189,15 +2189,15 @@
         "ValidationConfigurations": List[ValidationConfigurationTypeDef],
         "RecipeReference": RecipeReferenceTypeDef,
         "ResourceArn": str,
         "RoleArn": str,
         "Tags": Dict[str, str],
         "Timeout": int,
         "JobSample": JobSampleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeJobRunResponseTypeDef = TypedDict(
     "DescribeJobRunResponseTypeDef",
     {
         "Attempt": int,
@@ -2215,15 +2215,15 @@
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
         "RecipeReference": RecipeReferenceTypeDef,
         "StartedBy": str,
         "StartedOn": datetime,
         "JobSample": JobSampleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateProfileJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProfileJobRequestRequestTypeDef",
     {
         "Name": str,
```

### Comparing `mypy-boto3-databrew-1.26.56/mypy_boto3_databrew/type_defs.pyi` & `mypy-boto3-databrew-1.27.0/mypy_boto3_databrew/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -43,115 +43,115 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AllowedStatisticsTypeDef",
     "BatchDeleteRecipeVersionRequestRequestTypeDef",
     "RecipeVersionErrorDetailTypeDef",
-    "ResponseMetadataTypeDef",
     "ColumnSelectorTypeDef",
     "ConditionExpressionTypeDef",
+    "CreateDatasetResponseTypeDef",
     "JobSampleTypeDef",
     "S3LocationTypeDef",
     "ValidationConfigurationTypeDef",
+    "CreateProfileJobResponseTypeDef",
     "SampleTypeDef",
+    "CreateProjectResponseTypeDef",
     "RecipeReferenceTypeDef",
+    "CreateRecipeJobResponseTypeDef",
+    "CreateRecipeResponseTypeDef",
+    "CreateRulesetResponseTypeDef",
     "CreateScheduleRequestRequestTypeDef",
+    "CreateScheduleResponseTypeDef",
     "CsvOptionsTypeDef",
     "CsvOutputOptionsTypeDef",
     "DatetimeOptionsTypeDef",
     "FilterExpressionTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
+    "DeleteDatasetResponseTypeDef",
     "DeleteJobRequestRequestTypeDef",
+    "DeleteJobResponseTypeDef",
     "DeleteProjectRequestRequestTypeDef",
+    "DeleteProjectResponseTypeDef",
     "DeleteRecipeVersionRequestRequestTypeDef",
+    "DeleteRecipeVersionResponseTypeDef",
     "DeleteRulesetRequestRequestTypeDef",
+    "DeleteRulesetResponseTypeDef",
     "DeleteScheduleRequestRequestTypeDef",
+    "DeleteScheduleResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DescribeRecipeRequestRequestTypeDef",
     "DescribeRulesetRequestRequestTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
+    "DescribeScheduleResponseTypeDef",
     "ExcelOptionsTypeDef",
     "FilesLimitTypeDef",
     "JsonOptionsTypeDef",
     "MetadataTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
+    "ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     "ListRecipeVersionsRequestRequestTypeDef",
+    "ListRecipesRequestListRecipesPaginateTypeDef",
     "ListRecipesRequestRequestTypeDef",
+    "ListRulesetsRequestListRulesetsPaginateTypeDef",
     "ListRulesetsRequestRequestTypeDef",
     "RulesetItemTypeDef",
+    "ListSchedulesRequestListSchedulesPaginateTypeDef",
     "ListSchedulesRequestRequestTypeDef",
     "ScheduleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PublishRecipeRequestRequestTypeDef",
+    "PublishRecipeResponseTypeDef",
     "RecipeActionTypeDef",
+    "ResponseMetadataTypeDef",
     "ThresholdTypeDef",
     "ViewFrameTypeDef",
+    "SendProjectSessionActionResponseTypeDef",
     "StartJobRunRequestRequestTypeDef",
+    "StartJobRunResponseTypeDef",
     "StartProjectSessionRequestRequestTypeDef",
+    "StartProjectSessionResponseTypeDef",
     "StatisticOverrideTypeDef",
     "StopJobRunRequestRequestTypeDef",
+    "StopJobRunResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateScheduleRequestRequestTypeDef",
-    "EntityDetectorConfigurationTypeDef",
-    "BatchDeleteRecipeVersionResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateProfileJobResponseTypeDef",
-    "CreateProjectResponseTypeDef",
-    "CreateRecipeJobResponseTypeDef",
-    "CreateRecipeResponseTypeDef",
-    "CreateRulesetResponseTypeDef",
-    "CreateScheduleResponseTypeDef",
-    "DeleteDatasetResponseTypeDef",
-    "DeleteJobResponseTypeDef",
-    "DeleteProjectResponseTypeDef",
-    "DeleteRecipeVersionResponseTypeDef",
-    "DeleteRulesetResponseTypeDef",
-    "DeleteScheduleResponseTypeDef",
-    "DescribeScheduleResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PublishRecipeResponseTypeDef",
-    "SendProjectSessionActionResponseTypeDef",
-    "StartJobRunResponseTypeDef",
-    "StartProjectSessionResponseTypeDef",
-    "StopJobRunResponseTypeDef",
     "UpdateDatasetResponseTypeDef",
     "UpdateProfileJobResponseTypeDef",
     "UpdateProjectResponseTypeDef",
     "UpdateRecipeJobResponseTypeDef",
     "UpdateRecipeResponseTypeDef",
     "UpdateRulesetResponseTypeDef",
+    "UpdateScheduleRequestRequestTypeDef",
     "UpdateScheduleResponseTypeDef",
+    "EntityDetectorConfigurationTypeDef",
+    "BatchDeleteRecipeVersionResponseTypeDef",
     "DataCatalogInputDefinitionTypeDef",
     "DatabaseInputDefinitionTypeDef",
     "DatabaseTableOutputOptionsTypeDef",
     "S3TableOutputOptionsTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
     "ProjectTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "OutputFormatOptionsTypeDef",
     "DatasetParameterTypeDef",
     "FormatOptionsTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    "ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
-    "ListRecipesRequestListRecipesPaginateTypeDef",
-    "ListRulesetsRequestListRulesetsPaginateTypeDef",
-    "ListSchedulesRequestListSchedulesPaginateTypeDef",
     "ListRulesetsResponseTypeDef",
     "ListSchedulesResponseTypeDef",
     "RecipeStepTypeDef",
     "RuleTypeDef",
     "StatisticsConfigurationTypeDef",
     "InputTypeDef",
     "DatabaseOutputTypeDef",
@@ -209,25 +209,14 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "RecipeVersion": str,
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
 ColumnSelectorTypeDef = TypedDict(
     "ColumnSelectorTypeDef",
     {
         "Regex": str,
         "Name": str,
     },
     total=False,
@@ -249,14 +238,22 @@
 )
 
 class ConditionExpressionTypeDef(
     _RequiredConditionExpressionTypeDef, _OptionalConditionExpressionTypeDef
 ):
     pass
 
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 JobSampleTypeDef = TypedDict(
     "JobSampleTypeDef",
     {
         "Mode": SampleModeType,
         "Size": int,
     },
     total=False,
@@ -295,14 +292,22 @@
 )
 
 class ValidationConfigurationTypeDef(
     _RequiredValidationConfigurationTypeDef, _OptionalValidationConfigurationTypeDef
 ):
     pass
 
+CreateProfileJobResponseTypeDef = TypedDict(
+    "CreateProfileJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSampleTypeDef = TypedDict(
     "_RequiredSampleTypeDef",
     {
         "Type": SampleTypeType,
     },
 )
 _OptionalSampleTypeDef = TypedDict(
@@ -312,14 +317,22 @@
     },
     total=False,
 )
 
 class SampleTypeDef(_RequiredSampleTypeDef, _OptionalSampleTypeDef):
     pass
 
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRecipeReferenceTypeDef = TypedDict(
     "_RequiredRecipeReferenceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalRecipeReferenceTypeDef = TypedDict(
@@ -329,14 +342,38 @@
     },
     total=False,
 )
 
 class RecipeReferenceTypeDef(_RequiredRecipeReferenceTypeDef, _OptionalRecipeReferenceTypeDef):
     pass
 
+CreateRecipeJobResponseTypeDef = TypedDict(
+    "CreateRecipeJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateRecipeResponseTypeDef = TypedDict(
+    "CreateRecipeResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateRulesetResponseTypeDef = TypedDict(
+    "CreateRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScheduleRequestRequestTypeDef",
     {
         "CronExpression": str,
         "Name": str,
     },
 )
@@ -350,14 +387,22 @@
 )
 
 class CreateScheduleRequestRequestTypeDef(
     _RequiredCreateScheduleRequestRequestTypeDef, _OptionalCreateScheduleRequestRequestTypeDef
 ):
     pass
 
+CreateScheduleResponseTypeDef = TypedDict(
+    "CreateScheduleResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
         "HeaderRow": bool,
     },
     total=False,
@@ -400,50 +445,99 @@
 DeleteDatasetRequestRequestTypeDef = TypedDict(
     "DeleteDatasetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteDatasetResponseTypeDef = TypedDict(
+    "DeleteDatasetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteJobRequestRequestTypeDef = TypedDict(
     "DeleteJobRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteJobResponseTypeDef = TypedDict(
+    "DeleteJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRecipeVersionRequestRequestTypeDef = TypedDict(
     "DeleteRecipeVersionRequestRequestTypeDef",
     {
         "Name": str,
         "RecipeVersion": str,
     },
 )
 
+DeleteRecipeVersionResponseTypeDef = TypedDict(
+    "DeleteRecipeVersionResponseTypeDef",
+    {
+        "Name": str,
+        "RecipeVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteRulesetRequestRequestTypeDef = TypedDict(
     "DeleteRulesetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteRulesetResponseTypeDef = TypedDict(
+    "DeleteRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteScheduleRequestRequestTypeDef = TypedDict(
     "DeleteScheduleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteScheduleResponseTypeDef = TypedDict(
+    "DeleteScheduleResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -498,14 +592,30 @@
 DescribeScheduleRequestRequestTypeDef = TypedDict(
     "DescribeScheduleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DescribeScheduleResponseTypeDef = TypedDict(
+    "DescribeScheduleResponseTypeDef",
+    {
+        "CreateDate": datetime,
+        "CreatedBy": str,
+        "JobNames": List[str],
+        "LastModifiedBy": str,
+        "LastModifiedDate": datetime,
+        "ResourceArn": str,
+        "CronExpression": str,
+        "Tags": Dict[str, str],
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExcelOptionsTypeDef = TypedDict(
     "ExcelOptionsTypeDef",
     {
         "SheetNames": Sequence[str],
         "SheetIndexes": Sequence[int],
         "HeaderRow": bool,
     },
@@ -542,33 +652,51 @@
     "MetadataTypeDef",
     {
         "SourceArn": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListJobRunsRequestListJobRunsPaginateTypeDef(
+    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
+    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
+):
+    pass
+
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -581,34 +709,72 @@
 )
 
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "DatasetName": str,
+        "ProjectName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "DatasetName": str,
         "MaxResults": int,
         "NextToken": str,
         "ProjectName": str,
     },
     total=False,
 )
 
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef(
+    _RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
+    _OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListRecipeVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecipeVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListRecipeVersionsRequestRequestTypeDef = TypedDict(
@@ -622,24 +788,42 @@
 
 class ListRecipeVersionsRequestRequestTypeDef(
     _RequiredListRecipeVersionsRequestRequestTypeDef,
     _OptionalListRecipeVersionsRequestRequestTypeDef,
 ):
     pass
 
+ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
+    "ListRecipesRequestListRecipesPaginateTypeDef",
+    {
+        "RecipeVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRecipesRequestRequestTypeDef = TypedDict(
     "ListRecipesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "RecipeVersion": str,
     },
     total=False,
 )
 
+ListRulesetsRequestListRulesetsPaginateTypeDef = TypedDict(
+    "ListRulesetsRequestListRulesetsPaginateTypeDef",
+    {
+        "TargetArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRulesetsRequestRequestTypeDef = TypedDict(
     "ListRulesetsRequestRequestTypeDef",
     {
         "TargetArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -668,14 +852,23 @@
     },
     total=False,
 )
 
 class RulesetItemTypeDef(_RequiredRulesetItemTypeDef, _OptionalRulesetItemTypeDef):
     pass
 
+ListSchedulesRequestListSchedulesPaginateTypeDef = TypedDict(
+    "ListSchedulesRequestListSchedulesPaginateTypeDef",
+    {
+        "JobName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSchedulesRequestRequestTypeDef = TypedDict(
     "ListSchedulesRequestRequestTypeDef",
     {
         "JobName": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -710,14 +903,32 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
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
 _RequiredPublishRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredPublishRecipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalPublishRecipeRequestRequestTypeDef = TypedDict(
@@ -729,14 +940,22 @@
 )
 
 class PublishRecipeRequestRequestTypeDef(
     _RequiredPublishRecipeRequestRequestTypeDef, _OptionalPublishRecipeRequestRequestTypeDef
 ):
     pass
 
+PublishRecipeResponseTypeDef = TypedDict(
+    "PublishRecipeResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRecipeActionTypeDef = TypedDict(
     "_RequiredRecipeActionTypeDef",
     {
         "Operation": str,
     },
 )
 _OptionalRecipeActionTypeDef = TypedDict(
@@ -746,14 +965,25 @@
     },
     total=False,
 )
 
 class RecipeActionTypeDef(_RequiredRecipeActionTypeDef, _OptionalRecipeActionTypeDef):
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
 _RequiredThresholdTypeDef = TypedDict(
     "_RequiredThresholdTypeDef",
     {
         "Value": float,
     },
 )
 _OptionalThresholdTypeDef = TypedDict(
@@ -785,21 +1015,39 @@
     },
     total=False,
 )
 
 class ViewFrameTypeDef(_RequiredViewFrameTypeDef, _OptionalViewFrameTypeDef):
     pass
 
+SendProjectSessionActionResponseTypeDef = TypedDict(
+    "SendProjectSessionActionResponseTypeDef",
+    {
+        "Result": str,
+        "Name": str,
+        "ActionId": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartJobRunRequestRequestTypeDef = TypedDict(
     "StartJobRunRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartProjectSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartProjectSessionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalStartProjectSessionRequestRequestTypeDef = TypedDict(
@@ -812,14 +1060,23 @@
 
 class StartProjectSessionRequestRequestTypeDef(
     _RequiredStartProjectSessionRequestRequestTypeDef,
     _OptionalStartProjectSessionRequestRequestTypeDef,
 ):
     pass
 
+StartProjectSessionResponseTypeDef = TypedDict(
+    "StartProjectSessionResponseTypeDef",
+    {
+        "Name": str,
+        "ClientSessionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StatisticOverrideTypeDef = TypedDict(
     "StatisticOverrideTypeDef",
     {
         "Statistic": str,
         "Parameters": Mapping[str, str],
     },
 )
@@ -828,14 +1085,22 @@
     "StopJobRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
 
+StopJobRunResponseTypeDef = TypedDict(
+    "StopJobRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -844,288 +1109,116 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredUpdateScheduleRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateScheduleRequestRequestTypeDef",
-    {
-        "CronExpression": str,
-        "Name": str,
-    },
-)
-_OptionalUpdateScheduleRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateScheduleRequestRequestTypeDef",
-    {
-        "JobNames": Sequence[str],
-    },
-    total=False,
-)
-
-class UpdateScheduleRequestRequestTypeDef(
-    _RequiredUpdateScheduleRequestRequestTypeDef, _OptionalUpdateScheduleRequestRequestTypeDef
-):
-    pass
-
-_RequiredEntityDetectorConfigurationTypeDef = TypedDict(
-    "_RequiredEntityDetectorConfigurationTypeDef",
-    {
-        "EntityTypes": Sequence[str],
-    },
-)
-_OptionalEntityDetectorConfigurationTypeDef = TypedDict(
-    "_OptionalEntityDetectorConfigurationTypeDef",
-    {
-        "AllowedStatistics": Sequence[AllowedStatisticsTypeDef],
-    },
-    total=False,
-)
-
-class EntityDetectorConfigurationTypeDef(
-    _RequiredEntityDetectorConfigurationTypeDef, _OptionalEntityDetectorConfigurationTypeDef
-):
-    pass
-
-BatchDeleteRecipeVersionResponseTypeDef = TypedDict(
-    "BatchDeleteRecipeVersionResponseTypeDef",
-    {
-        "Name": str,
-        "Errors": List[RecipeVersionErrorDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProfileJobResponseTypeDef = TypedDict(
-    "CreateProfileJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRecipeJobResponseTypeDef = TypedDict(
-    "CreateRecipeJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRecipeResponseTypeDef = TypedDict(
-    "CreateRecipeResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRulesetResponseTypeDef = TypedDict(
-    "CreateRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateScheduleResponseTypeDef = TypedDict(
-    "CreateScheduleResponseTypeDef",
+UpdateDatasetResponseTypeDef = TypedDict(
+    "UpdateDatasetResponseTypeDef",
     {
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteDatasetResponseTypeDef = TypedDict(
-    "DeleteDatasetResponseTypeDef",
+UpdateProfileJobResponseTypeDef = TypedDict(
+    "UpdateProfileJobResponseTypeDef",
     {
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteJobResponseTypeDef = TypedDict(
-    "DeleteJobResponseTypeDef",
+UpdateProjectResponseTypeDef = TypedDict(
+    "UpdateProjectResponseTypeDef",
     {
+        "LastModifiedDate": datetime,
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
+UpdateRecipeJobResponseTypeDef = TypedDict(
+    "UpdateRecipeJobResponseTypeDef",
     {
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteRecipeVersionResponseTypeDef = TypedDict(
-    "DeleteRecipeVersionResponseTypeDef",
-    {
-        "Name": str,
-        "RecipeVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteRulesetResponseTypeDef = TypedDict(
-    "DeleteRulesetResponseTypeDef",
+UpdateRecipeResponseTypeDef = TypedDict(
+    "UpdateRecipeResponseTypeDef",
     {
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteScheduleResponseTypeDef = TypedDict(
-    "DeleteScheduleResponseTypeDef",
+UpdateRulesetResponseTypeDef = TypedDict(
+    "UpdateRulesetResponseTypeDef",
     {
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeScheduleResponseTypeDef = TypedDict(
-    "DescribeScheduleResponseTypeDef",
+_RequiredUpdateScheduleRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateScheduleRequestRequestTypeDef",
     {
-        "CreateDate": datetime,
-        "CreatedBy": str,
-        "JobNames": List[str],
-        "LastModifiedBy": str,
-        "LastModifiedDate": datetime,
-        "ResourceArn": str,
         "CronExpression": str,
-        "Tags": Dict[str, str],
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PublishRecipeResponseTypeDef = TypedDict(
-    "PublishRecipeResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendProjectSessionActionResponseTypeDef = TypedDict(
-    "SendProjectSessionActionResponseTypeDef",
-    {
-        "Result": str,
-        "Name": str,
-        "ActionId": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartProjectSessionResponseTypeDef = TypedDict(
-    "StartProjectSessionResponseTypeDef",
-    {
-        "Name": str,
-        "ClientSessionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopJobRunResponseTypeDef = TypedDict(
-    "StopJobRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateDatasetResponseTypeDef = TypedDict(
-    "UpdateDatasetResponseTypeDef",
+_OptionalUpdateScheduleRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateScheduleRequestRequestTypeDef",
     {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobNames": Sequence[str],
     },
+    total=False,
 )
 
-UpdateProfileJobResponseTypeDef = TypedDict(
-    "UpdateProfileJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class UpdateScheduleRequestRequestTypeDef(
+    _RequiredUpdateScheduleRequestRequestTypeDef, _OptionalUpdateScheduleRequestRequestTypeDef
+):
+    pass
 
-UpdateProjectResponseTypeDef = TypedDict(
-    "UpdateProjectResponseTypeDef",
+UpdateScheduleResponseTypeDef = TypedDict(
+    "UpdateScheduleResponseTypeDef",
     {
-        "LastModifiedDate": datetime,
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRecipeJobResponseTypeDef = TypedDict(
-    "UpdateRecipeJobResponseTypeDef",
+_RequiredEntityDetectorConfigurationTypeDef = TypedDict(
+    "_RequiredEntityDetectorConfigurationTypeDef",
     {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "EntityTypes": Sequence[str],
     },
 )
-
-UpdateRecipeResponseTypeDef = TypedDict(
-    "UpdateRecipeResponseTypeDef",
+_OptionalEntityDetectorConfigurationTypeDef = TypedDict(
+    "_OptionalEntityDetectorConfigurationTypeDef",
     {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AllowedStatistics": Sequence[AllowedStatisticsTypeDef],
     },
+    total=False,
 )
 
-UpdateRulesetResponseTypeDef = TypedDict(
-    "UpdateRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class EntityDetectorConfigurationTypeDef(
+    _RequiredEntityDetectorConfigurationTypeDef, _OptionalEntityDetectorConfigurationTypeDef
+):
+    pass
 
-UpdateScheduleResponseTypeDef = TypedDict(
-    "UpdateScheduleResponseTypeDef",
+BatchDeleteRecipeVersionResponseTypeDef = TypedDict(
+    "BatchDeleteRecipeVersionResponseTypeDef",
     {
         "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Errors": List[RecipeVersionErrorDetailTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDataCatalogInputDefinitionTypeDef = TypedDict(
     "_RequiredDataCatalogInputDefinitionTypeDef",
     {
         "DatabaseName": str,
@@ -1229,15 +1322,15 @@
         "ResourceArn": str,
         "Sample": SampleTypeDef,
         "RoleArn": str,
         "Tags": Dict[str, str],
         "SessionStatus": SessionStatusType,
         "OpenedBy": str,
         "OpenDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredProjectTypeDef = TypedDict(
     "_RequiredProjectTypeDef",
     {
         "Name": str,
@@ -1320,122 +1413,29 @@
         "Json": JsonOptionsTypeDef,
         "Excel": ExcelOptionsTypeDef,
         "Csv": CsvOptionsTypeDef,
     },
     total=False,
 )
 
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListJobRunsRequestListJobRunsPaginateTypeDef(
-    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
-    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
-):
-    pass
-
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "DatasetName": str,
-        "ProjectName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef(
-    _RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
-    _OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
-):
-    pass
-
-ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
-    "ListRecipesRequestListRecipesPaginateTypeDef",
-    {
-        "RecipeVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListRulesetsRequestListRulesetsPaginateTypeDef = TypedDict(
-    "ListRulesetsRequestListRulesetsPaginateTypeDef",
-    {
-        "TargetArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSchedulesRequestListSchedulesPaginateTypeDef = TypedDict(
-    "ListSchedulesRequestListSchedulesPaginateTypeDef",
-    {
-        "JobName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListRulesetsResponseTypeDef = TypedDict(
     "ListRulesetsResponseTypeDef",
     {
         "Rulesets": List[RulesetItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSchedulesResponseTypeDef = TypedDict(
     "ListSchedulesResponseTypeDef",
     {
         "Schedules": List[ScheduleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRecipeStepTypeDef = TypedDict(
     "_RequiredRecipeStepTypeDef",
     {
         "Action": RecipeActionTypeDef,
@@ -1535,15 +1535,15 @@
     pass
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "Projects": List[ProjectTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredOutputTypeDef = TypedDict(
     "_RequiredOutputTypeDef",
     {
         "Location": S3LocationTypeDef,
@@ -1608,15 +1608,15 @@
         "PublishedDate": datetime,
         "Description": str,
         "Name": str,
         "Steps": List[RecipeStepTypeDef],
         "Tags": Dict[str, str],
         "ResourceArn": str,
         "RecipeVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRecipeTypeDef = TypedDict(
     "_RequiredRecipeTypeDef",
     {
         "Name": str,
@@ -1719,15 +1719,15 @@
         "Rules": List[RuleTypeDef],
         "CreateDate": datetime,
         "CreatedBy": str,
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
         "ResourceArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRulesetRequestRequestTypeDef",
     {
         "Name": str,
@@ -1952,15 +1952,15 @@
         "Input": InputTypeDef,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "Source": SourceType,
         "PathOptions": PathOptionsTypeDef,
         "Tags": Dict[str, str],
         "ResourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "Name": str,
@@ -1983,24 +1983,24 @@
     pass
 
 ListRecipeVersionsResponseTypeDef = TypedDict(
     "ListRecipeVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Recipes": List[RecipeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecipesResponseTypeDef = TypedDict(
     "ListRecipesResponseTypeDef",
     {
         "Recipes": List[RecipeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProfileConfigurationTypeDef = TypedDict(
     "ProfileConfigurationTypeDef",
     {
         "DatasetStatisticsConfiguration": StatisticsConfigurationTypeDef,
@@ -2012,33 +2012,33 @@
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "JobRuns": List[JobRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateProfileJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfileJobRequestRequestTypeDef",
     {
         "DatasetName": str,
@@ -2092,15 +2092,15 @@
         "ValidationConfigurations": List[ValidationConfigurationTypeDef],
         "RecipeReference": RecipeReferenceTypeDef,
         "ResourceArn": str,
         "RoleArn": str,
         "Tags": Dict[str, str],
         "Timeout": int,
         "JobSample": JobSampleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeJobRunResponseTypeDef = TypedDict(
     "DescribeJobRunResponseTypeDef",
     {
         "Attempt": int,
@@ -2118,15 +2118,15 @@
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
         "RecipeReference": RecipeReferenceTypeDef,
         "StartedBy": str,
         "StartedOn": datetime,
         "JobSample": JobSampleTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateProfileJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProfileJobRequestRequestTypeDef",
     {
         "Name": str,
```

### Comparing `mypy-boto3-databrew-1.26.56/mypy_boto3_databrew.egg-info/PKG-INFO` & `mypy-boto3-databrew-1.27.0/mypy_boto3_databrew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-databrew
-Version: 1.26.56
-Summary: Type annotations for boto3.GlueDataBrew 1.26.56 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.GlueDataBrew 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-databrew"></a>
 
 # mypy-boto3-databrew
 
 [![PyPI - mypy-boto3-databrew](https://img.shields.io/pypi/v/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-databrew?color=blue)](https://pypistats.org/packages/mypy-boto3-databrew)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlueDataBrew 1.26.56](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
+[boto3.GlueDataBrew 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
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
 [mypy-boto3-databrew docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,115 +365,115 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_databrew.type_defs import (
     AllowedStatisticsTypeDef,
     BatchDeleteRecipeVersionRequestRequestTypeDef,
     RecipeVersionErrorDetailTypeDef,
-    ResponseMetadataTypeDef,
     ColumnSelectorTypeDef,
     ConditionExpressionTypeDef,
+    CreateDatasetResponseTypeDef,
     JobSampleTypeDef,
     S3LocationTypeDef,
     ValidationConfigurationTypeDef,
+    CreateProfileJobResponseTypeDef,
     SampleTypeDef,
+    CreateProjectResponseTypeDef,
     RecipeReferenceTypeDef,
+    CreateRecipeJobResponseTypeDef,
+    CreateRecipeResponseTypeDef,
+    CreateRulesetResponseTypeDef,
     CreateScheduleRequestRequestTypeDef,
+    CreateScheduleResponseTypeDef,
     CsvOptionsTypeDef,
     CsvOutputOptionsTypeDef,
     DatetimeOptionsTypeDef,
     FilterExpressionTypeDef,
     DeleteDatasetRequestRequestTypeDef,
+    DeleteDatasetResponseTypeDef,
     DeleteJobRequestRequestTypeDef,
+    DeleteJobResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
+    DeleteProjectResponseTypeDef,
     DeleteRecipeVersionRequestRequestTypeDef,
+    DeleteRecipeVersionResponseTypeDef,
     DeleteRulesetRequestRequestTypeDef,
+    DeleteRulesetResponseTypeDef,
     DeleteScheduleRequestRequestTypeDef,
+    DeleteScheduleResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DescribeRecipeRequestRequestTypeDef,
     DescribeRulesetRequestRequestTypeDef,
     DescribeScheduleRequestRequestTypeDef,
+    DescribeScheduleResponseTypeDef,
     ExcelOptionsTypeDef,
     FilesLimitTypeDef,
     JsonOptionsTypeDef,
     MetadataTypeDef,
-    PaginatorConfigTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
+    ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
     ListRecipeVersionsRequestRequestTypeDef,
+    ListRecipesRequestListRecipesPaginateTypeDef,
     ListRecipesRequestRequestTypeDef,
+    ListRulesetsRequestListRulesetsPaginateTypeDef,
     ListRulesetsRequestRequestTypeDef,
     RulesetItemTypeDef,
+    ListSchedulesRequestListSchedulesPaginateTypeDef,
     ListSchedulesRequestRequestTypeDef,
     ScheduleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PublishRecipeRequestRequestTypeDef,
+    PublishRecipeResponseTypeDef,
     RecipeActionTypeDef,
+    ResponseMetadataTypeDef,
     ThresholdTypeDef,
     ViewFrameTypeDef,
+    SendProjectSessionActionResponseTypeDef,
     StartJobRunRequestRequestTypeDef,
+    StartJobRunResponseTypeDef,
     StartProjectSessionRequestRequestTypeDef,
+    StartProjectSessionResponseTypeDef,
     StatisticOverrideTypeDef,
     StopJobRunRequestRequestTypeDef,
+    StopJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateScheduleRequestRequestTypeDef,
-    EntityDetectorConfigurationTypeDef,
-    BatchDeleteRecipeVersionResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateProfileJobResponseTypeDef,
-    CreateProjectResponseTypeDef,
-    CreateRecipeJobResponseTypeDef,
-    CreateRecipeResponseTypeDef,
-    CreateRulesetResponseTypeDef,
-    CreateScheduleResponseTypeDef,
-    DeleteDatasetResponseTypeDef,
-    DeleteJobResponseTypeDef,
-    DeleteProjectResponseTypeDef,
-    DeleteRecipeVersionResponseTypeDef,
-    DeleteRulesetResponseTypeDef,
-    DeleteScheduleResponseTypeDef,
-    DescribeScheduleResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PublishRecipeResponseTypeDef,
-    SendProjectSessionActionResponseTypeDef,
-    StartJobRunResponseTypeDef,
-    StartProjectSessionResponseTypeDef,
-    StopJobRunResponseTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdateProfileJobResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateRecipeJobResponseTypeDef,
     UpdateRecipeResponseTypeDef,
     UpdateRulesetResponseTypeDef,
+    UpdateScheduleRequestRequestTypeDef,
     UpdateScheduleResponseTypeDef,
+    EntityDetectorConfigurationTypeDef,
+    BatchDeleteRecipeVersionResponseTypeDef,
     DataCatalogInputDefinitionTypeDef,
     DatabaseInputDefinitionTypeDef,
     DatabaseTableOutputOptionsTypeDef,
     S3TableOutputOptionsTypeDef,
     CreateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
     ProjectTypeDef,
     UpdateProjectRequestRequestTypeDef,
     OutputFormatOptionsTypeDef,
     DatasetParameterTypeDef,
     FormatOptionsTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
-    ListRecipesRequestListRecipesPaginateTypeDef,
-    ListRulesetsRequestListRulesetsPaginateTypeDef,
-    ListSchedulesRequestListSchedulesPaginateTypeDef,
     ListRulesetsResponseTypeDef,
     ListSchedulesResponseTypeDef,
     RecipeStepTypeDef,
     RuleTypeDef,
     StatisticsConfigurationTypeDef,
     InputTypeDef,
     DatabaseOutputTypeDef,
@@ -518,42 +518,42 @@
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

### Comparing `mypy-boto3-databrew-1.26.56/mypy_boto3_databrew.egg-info/SOURCES.txt` & `mypy-boto3-databrew-1.27.0/mypy_boto3_databrew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.26.56/setup.py` & `mypy-boto3-databrew-1.27.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-databrew.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-databrew",
-    version="1.26.56",
+    version="1.27.0",
     packages=["mypy_boto3_databrew"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GlueDataBrew 1.26.56 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.GlueDataBrew 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/",
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


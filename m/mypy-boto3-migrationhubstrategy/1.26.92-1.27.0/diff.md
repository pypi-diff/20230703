# Comparing `tmp/mypy-boto3-migrationhubstrategy-1.26.92.tar.gz` & `tmp/mypy-boto3-migrationhubstrategy-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migrationhubstrategy-1.26.92.tar", last modified: Wed Mar 15 19:32:09 2023, max compression
+gzip compressed data, was "mypy-boto3-migrationhubstrategy-1.27.0.tar", last modified: Mon Jul  3 19:51:09 2023, max compression
```

## Comparing `mypy-boto3-migrationhubstrategy-1.26.92.tar` & `mypy-boto3-migrationhubstrategy-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 19:32:09.731555 mypy-boto3-migrationhubstrategy-1.26.92/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-15 19:31:55.000000 mypy-boto3-migrationhubstrategy-1.26.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-03-15 19:32:09.731555 mypy-boto3-migrationhubstrategy-1.26.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17310 2023-03-15 19:31:55.000000 mypy-boto3-migrationhubstrategy-1.26.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 19:32:09.731555 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-15 19:31:55.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-03-15 19:31:55.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-15 19:31:55.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-03-15 19:31:55.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20755 2023-03-15 19:31:55.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-03-15 19:31:56.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15456 2023-03-15 19:31:55.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-03-15 19:31:55.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-03-15 19:31:55.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 19:31:55.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31710 2023-03-15 19:31:56.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31699 2023-03-15 19:31:56.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-15 19:31:55.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 19:32:09.731555 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-03-15 19:32:09.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-15 19:32:09.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 19:32:09.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 19:32:09.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-15 19:32:09.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-15 19:32:09.000000 mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 19:32:09.731555 mypy-boto3-migrationhubstrategy-1.26.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-03-15 19:31:55.000000 mypy-boto3-migrationhubstrategy-1.26.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:09.871711 mypy-boto3-migrationhubstrategy-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:28.000000 mypy-boto3-migrationhubstrategy-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18853 2023-07-03 19:51:09.871711 mypy-boto3-migrationhubstrategy-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17301 2023-07-03 19:42:28.000000 mypy-boto3-migrationhubstrategy-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:09.871711 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-03 19:42:28.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-03 19:42:28.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-03 19:42:28.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-07-03 19:42:28.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20755 2023-07-03 19:42:28.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-07-03 19:42:29.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-07-03 19:42:29.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-07-03 19:42:28.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-03 19:42:28.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:28.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31754 2023-07-03 19:42:29.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31743 2023-07-03 19:42:29.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:28.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:09.871711 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18853 2023-07-03 19:51:09.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 19:51:09.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:09.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:09.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:09.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 19:51:09.000000 mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:09.871711 mypy-boto3-migrationhubstrategy-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-03 19:42:28.000000 mypy-boto3-migrationhubstrategy-1.27.0/setup.py
```

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/LICENSE` & `mypy-boto3-migrationhubstrategy-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/PKG-INFO` & `mypy-boto3-migrationhubstrategy-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhubstrategy
-Version: 1.26.92
-Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.26.92 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-migrationhubstrategy"></a>
 
 # mypy-boto3-migrationhubstrategy
 
 [![PyPI - mypy-boto3-migrationhubstrategy](https://img.shields.io/pypi/v/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migrationhubstrategy?color=blue)](https://pypistats.org/packages/mypy-boto3-migrationhubstrategy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubStrategyRecommendations 1.26.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
+[boto3.MigrationHubStrategyRecommendations 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
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
 [mypy-boto3-migrationhubstrategy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -408,52 +408,52 @@
     VcenterBasedRemoteInfoTypeDef,
     VersionControlInfoTypeDef,
     DataCollectionDetailsTypeDef,
     HeterogeneousTypeDef,
     HomogeneousTypeDef,
     NoDatabaseMigrationPreferenceTypeDef,
     GetApplicationComponentDetailsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     GetApplicationComponentStrategiesRequestRequestTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetImportFileTaskRequestRequestTypeDef,
+    GetImportFileTaskResponseTypeDef,
+    GetLatestAssessmentIdResponseTypeDef,
     GetRecommendationReportDetailsRequestRequestTypeDef,
     RecommendationReportDetailsTypeDef,
-    PaginatorConfigTypeDef,
+    GetServerDetailsRequestGetServerDetailsPaginateTypeDef,
     GetServerDetailsRequestRequestTypeDef,
     GetServerStrategiesRequestRequestTypeDef,
     GroupTypeDef,
     ImportFileTaskInformationTypeDef,
+    ListCollectorsRequestListCollectorsPaginateTypeDef,
     ListCollectorsRequestRequestTypeDef,
+    ListImportFileTaskRequestListImportFileTaskPaginateTypeDef,
     ListImportFileTaskRequestRequestTypeDef,
     NoManagementPreferenceTypeDef,
     SelfManageResourcesTypeDef,
     NetworkInfoTypeDef,
     OSInfoTypeDef,
+    PaginatorConfigTypeDef,
     TransformationToolTypeDef,
+    ResponseMetadataTypeDef,
     ServerErrorTypeDef,
     SourceCodeTypeDef,
+    StartAssessmentResponseTypeDef,
+    StartImportFileTaskResponseTypeDef,
+    StartRecommendationReportGenerationResponseTypeDef,
     StopAssessmentRequestRequestTypeDef,
     StrategyOptionTypeDef,
     AntipatternReportResultTypeDef,
     AssessmentSummaryTypeDef,
     StartAssessmentRequestRequestTypeDef,
     PrioritizeBusinessGoalsTypeDef,
     ConfigurationSummaryTypeDef,
-    DatabaseMigrationPreferenceTypeDef,
     GetAssessmentResponseTypeDef,
-    GetImportFileTaskResponseTypeDef,
-    GetLatestAssessmentIdResponseTypeDef,
-    StartAssessmentResponseTypeDef,
-    StartImportFileTaskResponseTypeDef,
-    StartRecommendationReportGenerationResponseTypeDef,
+    DatabaseMigrationPreferenceTypeDef,
     GetRecommendationReportDetailsResponseTypeDef,
-    GetServerDetailsRequestGetServerDetailsPaginateTypeDef,
-    ListCollectorsRequestListCollectorsPaginateTypeDef,
-    ListImportFileTaskRequestListImportFileTaskPaginateTypeDef,
     ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef,
     ListApplicationComponentsRequestRequestTypeDef,
     ListServersRequestListServersPaginateTypeDef,
     ListServersRequestRequestTypeDef,
     StartImportFileTaskRequestRequestTypeDef,
     StartRecommendationReportGenerationRequestRequestTypeDef,
     ListImportFileTaskResponseTypeDef,
@@ -490,42 +490,42 @@
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

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/README.md` & `mypy-boto3-migrationhubstrategy-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-migrationhubstrategy"></a>
 
 # mypy-boto3-migrationhubstrategy
 
 [![PyPI - mypy-boto3-migrationhubstrategy](https://img.shields.io/pypi/v/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migrationhubstrategy?color=blue)](https://pypistats.org/packages/mypy-boto3-migrationhubstrategy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubStrategyRecommendations 1.26.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
+[boto3.MigrationHubStrategyRecommendations 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
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
 [mypy-boto3-migrationhubstrategy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -376,52 +376,52 @@
     VcenterBasedRemoteInfoTypeDef,
     VersionControlInfoTypeDef,
     DataCollectionDetailsTypeDef,
     HeterogeneousTypeDef,
     HomogeneousTypeDef,
     NoDatabaseMigrationPreferenceTypeDef,
     GetApplicationComponentDetailsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     GetApplicationComponentStrategiesRequestRequestTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetImportFileTaskRequestRequestTypeDef,
+    GetImportFileTaskResponseTypeDef,
+    GetLatestAssessmentIdResponseTypeDef,
     GetRecommendationReportDetailsRequestRequestTypeDef,
     RecommendationReportDetailsTypeDef,
-    PaginatorConfigTypeDef,
+    GetServerDetailsRequestGetServerDetailsPaginateTypeDef,
     GetServerDetailsRequestRequestTypeDef,
     GetServerStrategiesRequestRequestTypeDef,
     GroupTypeDef,
     ImportFileTaskInformationTypeDef,
+    ListCollectorsRequestListCollectorsPaginateTypeDef,
     ListCollectorsRequestRequestTypeDef,
+    ListImportFileTaskRequestListImportFileTaskPaginateTypeDef,
     ListImportFileTaskRequestRequestTypeDef,
     NoManagementPreferenceTypeDef,
     SelfManageResourcesTypeDef,
     NetworkInfoTypeDef,
     OSInfoTypeDef,
+    PaginatorConfigTypeDef,
     TransformationToolTypeDef,
+    ResponseMetadataTypeDef,
     ServerErrorTypeDef,
     SourceCodeTypeDef,
+    StartAssessmentResponseTypeDef,
+    StartImportFileTaskResponseTypeDef,
+    StartRecommendationReportGenerationResponseTypeDef,
     StopAssessmentRequestRequestTypeDef,
     StrategyOptionTypeDef,
     AntipatternReportResultTypeDef,
     AssessmentSummaryTypeDef,
     StartAssessmentRequestRequestTypeDef,
     PrioritizeBusinessGoalsTypeDef,
     ConfigurationSummaryTypeDef,
-    DatabaseMigrationPreferenceTypeDef,
     GetAssessmentResponseTypeDef,
-    GetImportFileTaskResponseTypeDef,
-    GetLatestAssessmentIdResponseTypeDef,
-    StartAssessmentResponseTypeDef,
-    StartImportFileTaskResponseTypeDef,
-    StartRecommendationReportGenerationResponseTypeDef,
+    DatabaseMigrationPreferenceTypeDef,
     GetRecommendationReportDetailsResponseTypeDef,
-    GetServerDetailsRequestGetServerDetailsPaginateTypeDef,
-    ListCollectorsRequestListCollectorsPaginateTypeDef,
-    ListImportFileTaskRequestListImportFileTaskPaginateTypeDef,
     ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef,
     ListApplicationComponentsRequestRequestTypeDef,
     ListServersRequestListServersPaginateTypeDef,
     ListServersRequestRequestTypeDef,
     StartImportFileTaskRequestRequestTypeDef,
     StartRecommendationReportGenerationRequestRequestTypeDef,
     ListImportFileTaskResponseTypeDef,
@@ -458,42 +458,42 @@
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

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/__init__.py` & `mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/__init__.pyi` & `mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/__main__.py` & `mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.26.92\nVersion:        "
-        " 1.26.92\nBuilder version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.92")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/client.py` & `mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/client.pyi` & `mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/literals.py` & `mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AnalysisTypeType",
     "AntipatternReportStatusType",
     "AppTypeType",
     "AppUnitErrorCategoryType",
     "ApplicationComponentCriteriaType",
     "ApplicationModeType",
@@ -71,15 +70,14 @@
     "MigrationHubStrategyRecommendationsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AnalysisTypeType = Literal[
     "BINARY_ANALYSIS", "DATABASE_ANALYSIS", "RUNTIME_ANALYSIS", "SOURCE_CODE_ANALYSIS"
 ]
 AntipatternReportStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
 AppTypeType = Literal[
     "Cassandra",
     "DB2",
@@ -281,14 +279,15 @@
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
@@ -328,14 +327,15 @@
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
@@ -433,14 +433,15 @@
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
@@ -476,14 +477,15 @@
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
@@ -502,16 +504,19 @@
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
@@ -595,15 +600,17 @@
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

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/literals.pyi` & `mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AnalysisTypeType",
     "AntipatternReportStatusType",
     "AppTypeType",
     "AppUnitErrorCategoryType",
     "ApplicationComponentCriteriaType",
     "ApplicationModeType",
@@ -70,14 +71,15 @@
     "MigrationHubStrategyRecommendationsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AnalysisTypeType = Literal[
     "BINARY_ANALYSIS", "DATABASE_ANALYSIS", "RUNTIME_ANALYSIS", "SOURCE_CODE_ANALYSIS"
 ]
 AntipatternReportStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
 AppTypeType = Literal[
     "Cassandra",
     "DB2",
@@ -279,14 +281,15 @@
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
@@ -326,14 +329,15 @@
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
@@ -431,14 +435,15 @@
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
@@ -474,14 +479,15 @@
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
@@ -500,16 +506,19 @@
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
@@ -593,15 +602,17 @@
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

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/paginator.py` & `mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 class GetServerDetailsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.GetServerDetails)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#getserverdetailspaginator)
     """
 
     def paginate(
-        self, *, serverId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, serverId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetServerDetailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.GetServerDetails.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#getserverdetailspaginator)
         """
 
 
@@ -85,45 +85,45 @@
     def paginate(
         self,
         *,
         applicationComponentCriteria: ApplicationComponentCriteriaType = ...,
         filterValue: str = ...,
         groupIdFilter: Sequence[GroupTypeDef] = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListApplicationComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listapplicationcomponentspaginator)
         """
 
 
 class ListCollectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListCollectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listcollectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCollectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListCollectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listcollectorspaginator)
         """
 
 
 class ListImportFileTaskPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListImportFileTask)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listimportfiletaskpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListImportFileTaskResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListImportFileTask.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listimportfiletaskpaginator)
         """
 
 
@@ -136,13 +136,13 @@
     def paginate(
         self,
         *,
         filterValue: str = ...,
         groupIdFilter: Sequence[GroupTypeDef] = ...,
         serverCriteria: ServerCriteriaType = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listserverspaginator)
         """
```

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/paginator.pyi` & `mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 class GetServerDetailsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.GetServerDetails)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#getserverdetailspaginator)
     """
 
     def paginate(
-        self, *, serverId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, serverId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetServerDetailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.GetServerDetails.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#getserverdetailspaginator)
         """
 
 class ListApplicationComponentsPaginator(Paginator):
@@ -81,43 +81,43 @@
     def paginate(
         self,
         *,
         applicationComponentCriteria: ApplicationComponentCriteriaType = ...,
         filterValue: str = ...,
         groupIdFilter: Sequence[GroupTypeDef] = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListApplicationComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listapplicationcomponentspaginator)
         """
 
 class ListCollectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListCollectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listcollectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCollectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListCollectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listcollectorspaginator)
         """
 
 class ListImportFileTaskPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListImportFileTask)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listimportfiletaskpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListImportFileTaskResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListImportFileTask.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listimportfiletaskpaginator)
         """
 
 class ListServersPaginator(Paginator):
@@ -129,13 +129,13 @@
     def paginate(
         self,
         *,
         filterValue: str = ...,
         groupIdFilter: Sequence[GroupTypeDef] = ...,
         serverCriteria: ServerCriteriaType = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listserverspaginator)
         """
```

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/type_defs.py` & `mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,52 +92,52 @@
     "VcenterBasedRemoteInfoTypeDef",
     "VersionControlInfoTypeDef",
     "DataCollectionDetailsTypeDef",
     "HeterogeneousTypeDef",
     "HomogeneousTypeDef",
     "NoDatabaseMigrationPreferenceTypeDef",
     "GetApplicationComponentDetailsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "GetApplicationComponentStrategiesRequestRequestTypeDef",
     "GetAssessmentRequestRequestTypeDef",
     "GetImportFileTaskRequestRequestTypeDef",
+    "GetImportFileTaskResponseTypeDef",
+    "GetLatestAssessmentIdResponseTypeDef",
     "GetRecommendationReportDetailsRequestRequestTypeDef",
     "RecommendationReportDetailsTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetServerDetailsRequestGetServerDetailsPaginateTypeDef",
     "GetServerDetailsRequestRequestTypeDef",
     "GetServerStrategiesRequestRequestTypeDef",
     "GroupTypeDef",
     "ImportFileTaskInformationTypeDef",
+    "ListCollectorsRequestListCollectorsPaginateTypeDef",
     "ListCollectorsRequestRequestTypeDef",
+    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
     "ListImportFileTaskRequestRequestTypeDef",
     "NoManagementPreferenceTypeDef",
     "SelfManageResourcesTypeDef",
     "NetworkInfoTypeDef",
     "OSInfoTypeDef",
+    "PaginatorConfigTypeDef",
     "TransformationToolTypeDef",
+    "ResponseMetadataTypeDef",
     "ServerErrorTypeDef",
     "SourceCodeTypeDef",
+    "StartAssessmentResponseTypeDef",
+    "StartImportFileTaskResponseTypeDef",
+    "StartRecommendationReportGenerationResponseTypeDef",
     "StopAssessmentRequestRequestTypeDef",
     "StrategyOptionTypeDef",
     "AntipatternReportResultTypeDef",
     "AssessmentSummaryTypeDef",
     "StartAssessmentRequestRequestTypeDef",
     "PrioritizeBusinessGoalsTypeDef",
     "ConfigurationSummaryTypeDef",
-    "DatabaseMigrationPreferenceTypeDef",
     "GetAssessmentResponseTypeDef",
-    "GetImportFileTaskResponseTypeDef",
-    "GetLatestAssessmentIdResponseTypeDef",
-    "StartAssessmentResponseTypeDef",
-    "StartImportFileTaskResponseTypeDef",
-    "StartRecommendationReportGenerationResponseTypeDef",
+    "DatabaseMigrationPreferenceTypeDef",
     "GetRecommendationReportDetailsResponseTypeDef",
-    "GetServerDetailsRequestGetServerDetailsPaginateTypeDef",
-    "ListCollectorsRequestListCollectorsPaginateTypeDef",
-    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
     "ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef",
     "ListApplicationComponentsRequestRequestTypeDef",
     "ListServersRequestListServersPaginateTypeDef",
     "ListServersRequestRequestTypeDef",
     "StartImportFileTaskRequestRequestTypeDef",
     "StartRecommendationReportGenerationRequestRequestTypeDef",
     "ListImportFileTaskResponseTypeDef",
@@ -396,25 +396,14 @@
 GetApplicationComponentDetailsRequestRequestTypeDef = TypedDict(
     "GetApplicationComponentDetailsRequestRequestTypeDef",
     {
         "applicationComponentId": str,
     },
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
 GetApplicationComponentStrategiesRequestRequestTypeDef = TypedDict(
     "GetApplicationComponentStrategiesRequestRequestTypeDef",
     {
         "applicationComponentId": str,
     },
 )
 
@@ -428,14 +417,40 @@
 GetImportFileTaskRequestRequestTypeDef = TypedDict(
     "GetImportFileTaskRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+GetImportFileTaskResponseTypeDef = TypedDict(
+    "GetImportFileTaskResponseTypeDef",
+    {
+        "completionTime": datetime,
+        "id": str,
+        "importName": str,
+        "inputS3Bucket": str,
+        "inputS3Key": str,
+        "numberOfRecordsFailed": int,
+        "numberOfRecordsSuccess": int,
+        "startTime": datetime,
+        "status": ImportFileTaskStatusType,
+        "statusReportS3Bucket": str,
+        "statusReportS3Key": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetLatestAssessmentIdResponseTypeDef = TypedDict(
+    "GetLatestAssessmentIdResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetRecommendationReportDetailsRequestRequestTypeDef = TypedDict(
     "GetRecommendationReportDetailsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -448,24 +463,36 @@
         "startTime": datetime,
         "status": RecommendationReportStatusType,
         "statusMessage": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
+    "_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "serverId": str,
+    },
+)
+_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
+    "_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class GetServerDetailsRequestGetServerDetailsPaginateTypeDef(
+    _RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
+    _OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetServerDetailsRequestRequestTypeDef = TypedDict(
     "_RequiredGetServerDetailsRequestRequestTypeDef",
     {
         "serverId": str,
     },
 )
 _OptionalGetServerDetailsRequestRequestTypeDef = TypedDict(
@@ -514,23 +541,39 @@
         "status": ImportFileTaskStatusType,
         "statusReportS3Bucket": str,
         "statusReportS3Key": str,
     },
     total=False,
 )
 
+ListCollectorsRequestListCollectorsPaginateTypeDef = TypedDict(
+    "ListCollectorsRequestListCollectorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCollectorsRequestRequestTypeDef = TypedDict(
     "ListCollectorsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListImportFileTaskRequestListImportFileTaskPaginateTypeDef = TypedDict(
+    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListImportFileTaskRequestRequestTypeDef = TypedDict(
     "ListImportFileTaskRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -565,24 +608,45 @@
     {
         "type": OSTypeType,
         "version": str,
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
 TransformationToolTypeDef = TypedDict(
     "TransformationToolTypeDef",
     {
         "description": str,
         "name": TransformationToolNameType,
         "tranformationToolInstallationLink": str,
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
 ServerErrorTypeDef = TypedDict(
     "ServerErrorTypeDef",
     {
         "serverErrorCategory": ServerErrorCategoryType,
     },
     total=False,
 )
@@ -594,14 +658,38 @@
         "projectName": str,
         "sourceVersion": str,
         "versionControl": VersionControlType,
     },
     total=False,
 )
 
+StartAssessmentResponseTypeDef = TypedDict(
+    "StartAssessmentResponseTypeDef",
+    {
+        "assessmentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartImportFileTaskResponseTypeDef = TypedDict(
+    "StartImportFileTaskResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartRecommendationReportGenerationResponseTypeDef = TypedDict(
+    "StartRecommendationReportGenerationResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopAssessmentRequestRequestTypeDef = TypedDict(
     "StopAssessmentRequestRequestTypeDef",
     {
         "assessmentId": str,
     },
 )
 
@@ -671,139 +759,51 @@
         "remoteSourceCodeAnalysisServerInfo": RemoteSourceCodeAnalysisServerInfoTypeDef,
         "vcenterBasedRemoteInfoList": List[VcenterBasedRemoteInfoTypeDef],
         "versionControlInfoList": List[VersionControlInfoTypeDef],
     },
     total=False,
 )
 
-DatabaseMigrationPreferenceTypeDef = TypedDict(
-    "DatabaseMigrationPreferenceTypeDef",
-    {
-        "heterogeneous": HeterogeneousTypeDef,
-        "homogeneous": HomogeneousTypeDef,
-        "noPreference": NoDatabaseMigrationPreferenceTypeDef,
-    },
-    total=False,
-)
-
 GetAssessmentResponseTypeDef = TypedDict(
     "GetAssessmentResponseTypeDef",
     {
         "assessmentTargets": List[AssessmentTargetTypeDef],
         "dataCollectionDetails": DataCollectionDetailsTypeDef,
         "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetImportFileTaskResponseTypeDef = TypedDict(
-    "GetImportFileTaskResponseTypeDef",
-    {
-        "completionTime": datetime,
-        "id": str,
-        "importName": str,
-        "inputS3Bucket": str,
-        "inputS3Key": str,
-        "numberOfRecordsFailed": int,
-        "numberOfRecordsSuccess": int,
-        "startTime": datetime,
-        "status": ImportFileTaskStatusType,
-        "statusReportS3Bucket": str,
-        "statusReportS3Key": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLatestAssessmentIdResponseTypeDef = TypedDict(
-    "GetLatestAssessmentIdResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartAssessmentResponseTypeDef = TypedDict(
-    "StartAssessmentResponseTypeDef",
-    {
-        "assessmentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartImportFileTaskResponseTypeDef = TypedDict(
-    "StartImportFileTaskResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartRecommendationReportGenerationResponseTypeDef = TypedDict(
-    "StartRecommendationReportGenerationResponseTypeDef",
+DatabaseMigrationPreferenceTypeDef = TypedDict(
+    "DatabaseMigrationPreferenceTypeDef",
     {
-        "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "heterogeneous": HeterogeneousTypeDef,
+        "homogeneous": HomogeneousTypeDef,
+        "noPreference": NoDatabaseMigrationPreferenceTypeDef,
     },
+    total=False,
 )
 
 GetRecommendationReportDetailsResponseTypeDef = TypedDict(
     "GetRecommendationReportDetailsResponseTypeDef",
     {
         "id": str,
         "recommendationReportDetails": RecommendationReportDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
-    "_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
-    {
-        "serverId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
-    "_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetServerDetailsRequestGetServerDetailsPaginateTypeDef(
-    _RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
-    _OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
-):
-    pass
-
-
-ListCollectorsRequestListCollectorsPaginateTypeDef = TypedDict(
-    "ListCollectorsRequestListCollectorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListImportFileTaskRequestListImportFileTaskPaginateTypeDef = TypedDict(
-    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
 ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef = TypedDict(
     "ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef",
     {
         "applicationComponentCriteria": ApplicationComponentCriteriaType,
         "filterValue": str,
         "groupIdFilter": Sequence[GroupTypeDef],
         "sort": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationComponentsRequestRequestTypeDef = TypedDict(
     "ListApplicationComponentsRequestRequestTypeDef",
     {
@@ -820,15 +820,15 @@
 ListServersRequestListServersPaginateTypeDef = TypedDict(
     "ListServersRequestListServersPaginateTypeDef",
     {
         "filterValue": str,
         "groupIdFilter": Sequence[GroupTypeDef],
         "serverCriteria": ServerCriteriaType,
         "sort": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListServersRequestRequestTypeDef = TypedDict(
     "ListServersRequestRequestTypeDef",
     {
@@ -878,15 +878,15 @@
 )
 
 ListImportFileTaskResponseTypeDef = TypedDict(
     "ListImportFileTaskResponseTypeDef",
     {
         "nextToken": str,
         "taskInfos": List[ImportFileTaskInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ManagementPreferenceTypeDef = TypedDict(
     "ManagementPreferenceTypeDef",
     {
         "awsManagedResources": AwsManagedResourcesTypeDef,
@@ -977,15 +977,15 @@
     total=False,
 )
 
 GetPortfolioSummaryResponseTypeDef = TypedDict(
     "GetPortfolioSummaryResponseTypeDef",
     {
         "assessmentSummary": AssessmentSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CollectorTypeDef = TypedDict(
     "CollectorTypeDef",
     {
         "collectorHealth": CollectorHealthType,
@@ -1090,26 +1090,26 @@
 )
 
 ListCollectorsResponseTypeDef = TypedDict(
     "ListCollectorsResponseTypeDef",
     {
         "Collectors": List[CollectorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPortfolioPreferencesResponseTypeDef = TypedDict(
     "GetPortfolioPreferencesResponseTypeDef",
     {
         "applicationMode": ApplicationModeType,
         "applicationPreferences": ApplicationPreferencesTypeDef,
         "databasePreferences": DatabasePreferencesTypeDef,
         "prioritizeBusinessGoals": PrioritizeBusinessGoalsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutPortfolioPreferencesRequestRequestTypeDef = TypedDict(
     "PutPortfolioPreferencesRequestRequestTypeDef",
     {
         "applicationMode": ApplicationModeType,
@@ -1120,57 +1120,57 @@
     total=False,
 )
 
 GetApplicationComponentStrategiesResponseTypeDef = TypedDict(
     "GetApplicationComponentStrategiesResponseTypeDef",
     {
         "applicationComponentStrategies": List[ApplicationComponentStrategyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServerDetailsResponseTypeDef = TypedDict(
     "GetServerDetailsResponseTypeDef",
     {
         "associatedApplications": List[AssociatedApplicationTypeDef],
         "nextToken": str,
         "serverDetail": ServerDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServersResponseTypeDef = TypedDict(
     "ListServersResponseTypeDef",
     {
         "nextToken": str,
         "serverInfos": List[ServerDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServerStrategiesResponseTypeDef = TypedDict(
     "GetServerStrategiesResponseTypeDef",
     {
         "serverStrategies": List[ServerStrategyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationComponentDetailsResponseTypeDef = TypedDict(
     "GetApplicationComponentDetailsResponseTypeDef",
     {
         "applicationComponentDetail": ApplicationComponentDetailTypeDef,
         "associatedApplications": List[AssociatedApplicationTypeDef],
         "associatedServerIds": List[str],
         "moreApplicationResource": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApplicationComponentsResponseTypeDef = TypedDict(
     "ListApplicationComponentsResponseTypeDef",
     {
         "applicationComponentInfos": List[ApplicationComponentDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy/type_defs.pyi` & `mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -91,52 +91,52 @@
     "VcenterBasedRemoteInfoTypeDef",
     "VersionControlInfoTypeDef",
     "DataCollectionDetailsTypeDef",
     "HeterogeneousTypeDef",
     "HomogeneousTypeDef",
     "NoDatabaseMigrationPreferenceTypeDef",
     "GetApplicationComponentDetailsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "GetApplicationComponentStrategiesRequestRequestTypeDef",
     "GetAssessmentRequestRequestTypeDef",
     "GetImportFileTaskRequestRequestTypeDef",
+    "GetImportFileTaskResponseTypeDef",
+    "GetLatestAssessmentIdResponseTypeDef",
     "GetRecommendationReportDetailsRequestRequestTypeDef",
     "RecommendationReportDetailsTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetServerDetailsRequestGetServerDetailsPaginateTypeDef",
     "GetServerDetailsRequestRequestTypeDef",
     "GetServerStrategiesRequestRequestTypeDef",
     "GroupTypeDef",
     "ImportFileTaskInformationTypeDef",
+    "ListCollectorsRequestListCollectorsPaginateTypeDef",
     "ListCollectorsRequestRequestTypeDef",
+    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
     "ListImportFileTaskRequestRequestTypeDef",
     "NoManagementPreferenceTypeDef",
     "SelfManageResourcesTypeDef",
     "NetworkInfoTypeDef",
     "OSInfoTypeDef",
+    "PaginatorConfigTypeDef",
     "TransformationToolTypeDef",
+    "ResponseMetadataTypeDef",
     "ServerErrorTypeDef",
     "SourceCodeTypeDef",
+    "StartAssessmentResponseTypeDef",
+    "StartImportFileTaskResponseTypeDef",
+    "StartRecommendationReportGenerationResponseTypeDef",
     "StopAssessmentRequestRequestTypeDef",
     "StrategyOptionTypeDef",
     "AntipatternReportResultTypeDef",
     "AssessmentSummaryTypeDef",
     "StartAssessmentRequestRequestTypeDef",
     "PrioritizeBusinessGoalsTypeDef",
     "ConfigurationSummaryTypeDef",
-    "DatabaseMigrationPreferenceTypeDef",
     "GetAssessmentResponseTypeDef",
-    "GetImportFileTaskResponseTypeDef",
-    "GetLatestAssessmentIdResponseTypeDef",
-    "StartAssessmentResponseTypeDef",
-    "StartImportFileTaskResponseTypeDef",
-    "StartRecommendationReportGenerationResponseTypeDef",
+    "DatabaseMigrationPreferenceTypeDef",
     "GetRecommendationReportDetailsResponseTypeDef",
-    "GetServerDetailsRequestGetServerDetailsPaginateTypeDef",
-    "ListCollectorsRequestListCollectorsPaginateTypeDef",
-    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
     "ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef",
     "ListApplicationComponentsRequestRequestTypeDef",
     "ListServersRequestListServersPaginateTypeDef",
     "ListServersRequestRequestTypeDef",
     "StartImportFileTaskRequestRequestTypeDef",
     "StartRecommendationReportGenerationRequestRequestTypeDef",
     "ListImportFileTaskResponseTypeDef",
@@ -395,25 +395,14 @@
 GetApplicationComponentDetailsRequestRequestTypeDef = TypedDict(
     "GetApplicationComponentDetailsRequestRequestTypeDef",
     {
         "applicationComponentId": str,
     },
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
 GetApplicationComponentStrategiesRequestRequestTypeDef = TypedDict(
     "GetApplicationComponentStrategiesRequestRequestTypeDef",
     {
         "applicationComponentId": str,
     },
 )
 
@@ -427,14 +416,40 @@
 GetImportFileTaskRequestRequestTypeDef = TypedDict(
     "GetImportFileTaskRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+GetImportFileTaskResponseTypeDef = TypedDict(
+    "GetImportFileTaskResponseTypeDef",
+    {
+        "completionTime": datetime,
+        "id": str,
+        "importName": str,
+        "inputS3Bucket": str,
+        "inputS3Key": str,
+        "numberOfRecordsFailed": int,
+        "numberOfRecordsSuccess": int,
+        "startTime": datetime,
+        "status": ImportFileTaskStatusType,
+        "statusReportS3Bucket": str,
+        "statusReportS3Key": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetLatestAssessmentIdResponseTypeDef = TypedDict(
+    "GetLatestAssessmentIdResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetRecommendationReportDetailsRequestRequestTypeDef = TypedDict(
     "GetRecommendationReportDetailsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -447,24 +462,34 @@
         "startTime": datetime,
         "status": RecommendationReportStatusType,
         "statusMessage": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
+    "_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "serverId": str,
+    },
+)
+_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
+    "_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class GetServerDetailsRequestGetServerDetailsPaginateTypeDef(
+    _RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
+    _OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetServerDetailsRequestRequestTypeDef = TypedDict(
     "_RequiredGetServerDetailsRequestRequestTypeDef",
     {
         "serverId": str,
     },
 )
 _OptionalGetServerDetailsRequestRequestTypeDef = TypedDict(
@@ -511,23 +536,39 @@
         "status": ImportFileTaskStatusType,
         "statusReportS3Bucket": str,
         "statusReportS3Key": str,
     },
     total=False,
 )
 
+ListCollectorsRequestListCollectorsPaginateTypeDef = TypedDict(
+    "ListCollectorsRequestListCollectorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCollectorsRequestRequestTypeDef = TypedDict(
     "ListCollectorsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListImportFileTaskRequestListImportFileTaskPaginateTypeDef = TypedDict(
+    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListImportFileTaskRequestRequestTypeDef = TypedDict(
     "ListImportFileTaskRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -562,24 +603,45 @@
     {
         "type": OSTypeType,
         "version": str,
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
 TransformationToolTypeDef = TypedDict(
     "TransformationToolTypeDef",
     {
         "description": str,
         "name": TransformationToolNameType,
         "tranformationToolInstallationLink": str,
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
 ServerErrorTypeDef = TypedDict(
     "ServerErrorTypeDef",
     {
         "serverErrorCategory": ServerErrorCategoryType,
     },
     total=False,
 )
@@ -591,14 +653,38 @@
         "projectName": str,
         "sourceVersion": str,
         "versionControl": VersionControlType,
     },
     total=False,
 )
 
+StartAssessmentResponseTypeDef = TypedDict(
+    "StartAssessmentResponseTypeDef",
+    {
+        "assessmentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartImportFileTaskResponseTypeDef = TypedDict(
+    "StartImportFileTaskResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartRecommendationReportGenerationResponseTypeDef = TypedDict(
+    "StartRecommendationReportGenerationResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopAssessmentRequestRequestTypeDef = TypedDict(
     "StopAssessmentRequestRequestTypeDef",
     {
         "assessmentId": str,
     },
 )
 
@@ -668,137 +754,51 @@
         "remoteSourceCodeAnalysisServerInfo": RemoteSourceCodeAnalysisServerInfoTypeDef,
         "vcenterBasedRemoteInfoList": List[VcenterBasedRemoteInfoTypeDef],
         "versionControlInfoList": List[VersionControlInfoTypeDef],
     },
     total=False,
 )
 
-DatabaseMigrationPreferenceTypeDef = TypedDict(
-    "DatabaseMigrationPreferenceTypeDef",
-    {
-        "heterogeneous": HeterogeneousTypeDef,
-        "homogeneous": HomogeneousTypeDef,
-        "noPreference": NoDatabaseMigrationPreferenceTypeDef,
-    },
-    total=False,
-)
-
 GetAssessmentResponseTypeDef = TypedDict(
     "GetAssessmentResponseTypeDef",
     {
         "assessmentTargets": List[AssessmentTargetTypeDef],
         "dataCollectionDetails": DataCollectionDetailsTypeDef,
         "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetImportFileTaskResponseTypeDef = TypedDict(
-    "GetImportFileTaskResponseTypeDef",
-    {
-        "completionTime": datetime,
-        "id": str,
-        "importName": str,
-        "inputS3Bucket": str,
-        "inputS3Key": str,
-        "numberOfRecordsFailed": int,
-        "numberOfRecordsSuccess": int,
-        "startTime": datetime,
-        "status": ImportFileTaskStatusType,
-        "statusReportS3Bucket": str,
-        "statusReportS3Key": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLatestAssessmentIdResponseTypeDef = TypedDict(
-    "GetLatestAssessmentIdResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartAssessmentResponseTypeDef = TypedDict(
-    "StartAssessmentResponseTypeDef",
-    {
-        "assessmentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartImportFileTaskResponseTypeDef = TypedDict(
-    "StartImportFileTaskResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartRecommendationReportGenerationResponseTypeDef = TypedDict(
-    "StartRecommendationReportGenerationResponseTypeDef",
+DatabaseMigrationPreferenceTypeDef = TypedDict(
+    "DatabaseMigrationPreferenceTypeDef",
     {
-        "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "heterogeneous": HeterogeneousTypeDef,
+        "homogeneous": HomogeneousTypeDef,
+        "noPreference": NoDatabaseMigrationPreferenceTypeDef,
     },
+    total=False,
 )
 
 GetRecommendationReportDetailsResponseTypeDef = TypedDict(
     "GetRecommendationReportDetailsResponseTypeDef",
     {
         "id": str,
         "recommendationReportDetails": RecommendationReportDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
-    "_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
-    {
-        "serverId": str,
-    },
-)
-_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
-    "_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetServerDetailsRequestGetServerDetailsPaginateTypeDef(
-    _RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
-    _OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
-):
-    pass
-
-ListCollectorsRequestListCollectorsPaginateTypeDef = TypedDict(
-    "ListCollectorsRequestListCollectorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListImportFileTaskRequestListImportFileTaskPaginateTypeDef = TypedDict(
-    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef = TypedDict(
     "ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef",
     {
         "applicationComponentCriteria": ApplicationComponentCriteriaType,
         "filterValue": str,
         "groupIdFilter": Sequence[GroupTypeDef],
         "sort": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationComponentsRequestRequestTypeDef = TypedDict(
     "ListApplicationComponentsRequestRequestTypeDef",
     {
@@ -815,15 +815,15 @@
 ListServersRequestListServersPaginateTypeDef = TypedDict(
     "ListServersRequestListServersPaginateTypeDef",
     {
         "filterValue": str,
         "groupIdFilter": Sequence[GroupTypeDef],
         "serverCriteria": ServerCriteriaType,
         "sort": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListServersRequestRequestTypeDef = TypedDict(
     "ListServersRequestRequestTypeDef",
     {
@@ -871,15 +871,15 @@
 )
 
 ListImportFileTaskResponseTypeDef = TypedDict(
     "ListImportFileTaskResponseTypeDef",
     {
         "nextToken": str,
         "taskInfos": List[ImportFileTaskInformationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ManagementPreferenceTypeDef = TypedDict(
     "ManagementPreferenceTypeDef",
     {
         "awsManagedResources": AwsManagedResourcesTypeDef,
@@ -966,15 +966,15 @@
     total=False,
 )
 
 GetPortfolioSummaryResponseTypeDef = TypedDict(
     "GetPortfolioSummaryResponseTypeDef",
     {
         "assessmentSummary": AssessmentSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CollectorTypeDef = TypedDict(
     "CollectorTypeDef",
     {
         "collectorHealth": CollectorHealthType,
@@ -1079,26 +1079,26 @@
 )
 
 ListCollectorsResponseTypeDef = TypedDict(
     "ListCollectorsResponseTypeDef",
     {
         "Collectors": List[CollectorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPortfolioPreferencesResponseTypeDef = TypedDict(
     "GetPortfolioPreferencesResponseTypeDef",
     {
         "applicationMode": ApplicationModeType,
         "applicationPreferences": ApplicationPreferencesTypeDef,
         "databasePreferences": DatabasePreferencesTypeDef,
         "prioritizeBusinessGoals": PrioritizeBusinessGoalsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutPortfolioPreferencesRequestRequestTypeDef = TypedDict(
     "PutPortfolioPreferencesRequestRequestTypeDef",
     {
         "applicationMode": ApplicationModeType,
@@ -1109,57 +1109,57 @@
     total=False,
 )
 
 GetApplicationComponentStrategiesResponseTypeDef = TypedDict(
     "GetApplicationComponentStrategiesResponseTypeDef",
     {
         "applicationComponentStrategies": List[ApplicationComponentStrategyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServerDetailsResponseTypeDef = TypedDict(
     "GetServerDetailsResponseTypeDef",
     {
         "associatedApplications": List[AssociatedApplicationTypeDef],
         "nextToken": str,
         "serverDetail": ServerDetailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServersResponseTypeDef = TypedDict(
     "ListServersResponseTypeDef",
     {
         "nextToken": str,
         "serverInfos": List[ServerDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetServerStrategiesResponseTypeDef = TypedDict(
     "GetServerStrategiesResponseTypeDef",
     {
         "serverStrategies": List[ServerStrategyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetApplicationComponentDetailsResponseTypeDef = TypedDict(
     "GetApplicationComponentDetailsResponseTypeDef",
     {
         "applicationComponentDetail": ApplicationComponentDetailTypeDef,
         "associatedApplications": List[AssociatedApplicationTypeDef],
         "associatedServerIds": List[str],
         "moreApplicationResource": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApplicationComponentsResponseTypeDef = TypedDict(
     "ListApplicationComponentsResponseTypeDef",
     {
         "applicationComponentInfos": List[ApplicationComponentDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO` & `mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhubstrategy
-Version: 1.26.92
-Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.26.92 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-migrationhubstrategy"></a>
 
 # mypy-boto3-migrationhubstrategy
 
 [![PyPI - mypy-boto3-migrationhubstrategy](https://img.shields.io/pypi/v/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migrationhubstrategy?color=blue)](https://pypistats.org/packages/mypy-boto3-migrationhubstrategy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubStrategyRecommendations 1.26.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
+[boto3.MigrationHubStrategyRecommendations 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
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
 [mypy-boto3-migrationhubstrategy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -408,52 +408,52 @@
     VcenterBasedRemoteInfoTypeDef,
     VersionControlInfoTypeDef,
     DataCollectionDetailsTypeDef,
     HeterogeneousTypeDef,
     HomogeneousTypeDef,
     NoDatabaseMigrationPreferenceTypeDef,
     GetApplicationComponentDetailsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     GetApplicationComponentStrategiesRequestRequestTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetImportFileTaskRequestRequestTypeDef,
+    GetImportFileTaskResponseTypeDef,
+    GetLatestAssessmentIdResponseTypeDef,
     GetRecommendationReportDetailsRequestRequestTypeDef,
     RecommendationReportDetailsTypeDef,
-    PaginatorConfigTypeDef,
+    GetServerDetailsRequestGetServerDetailsPaginateTypeDef,
     GetServerDetailsRequestRequestTypeDef,
     GetServerStrategiesRequestRequestTypeDef,
     GroupTypeDef,
     ImportFileTaskInformationTypeDef,
+    ListCollectorsRequestListCollectorsPaginateTypeDef,
     ListCollectorsRequestRequestTypeDef,
+    ListImportFileTaskRequestListImportFileTaskPaginateTypeDef,
     ListImportFileTaskRequestRequestTypeDef,
     NoManagementPreferenceTypeDef,
     SelfManageResourcesTypeDef,
     NetworkInfoTypeDef,
     OSInfoTypeDef,
+    PaginatorConfigTypeDef,
     TransformationToolTypeDef,
+    ResponseMetadataTypeDef,
     ServerErrorTypeDef,
     SourceCodeTypeDef,
+    StartAssessmentResponseTypeDef,
+    StartImportFileTaskResponseTypeDef,
+    StartRecommendationReportGenerationResponseTypeDef,
     StopAssessmentRequestRequestTypeDef,
     StrategyOptionTypeDef,
     AntipatternReportResultTypeDef,
     AssessmentSummaryTypeDef,
     StartAssessmentRequestRequestTypeDef,
     PrioritizeBusinessGoalsTypeDef,
     ConfigurationSummaryTypeDef,
-    DatabaseMigrationPreferenceTypeDef,
     GetAssessmentResponseTypeDef,
-    GetImportFileTaskResponseTypeDef,
-    GetLatestAssessmentIdResponseTypeDef,
-    StartAssessmentResponseTypeDef,
-    StartImportFileTaskResponseTypeDef,
-    StartRecommendationReportGenerationResponseTypeDef,
+    DatabaseMigrationPreferenceTypeDef,
     GetRecommendationReportDetailsResponseTypeDef,
-    GetServerDetailsRequestGetServerDetailsPaginateTypeDef,
-    ListCollectorsRequestListCollectorsPaginateTypeDef,
-    ListImportFileTaskRequestListImportFileTaskPaginateTypeDef,
     ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef,
     ListApplicationComponentsRequestRequestTypeDef,
     ListServersRequestListServersPaginateTypeDef,
     ListServersRequestRequestTypeDef,
     StartImportFileTaskRequestRequestTypeDef,
     StartRecommendationReportGenerationRequestRequestTypeDef,
     ListImportFileTaskResponseTypeDef,
@@ -490,42 +490,42 @@
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

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt` & `mypy-boto3-migrationhubstrategy-1.27.0/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.26.92/setup.py` & `mypy-boto3-migrationhubstrategy-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-migrationhubstrategy.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migrationhubstrategy",
-    version="1.26.92",
+    version="1.27.0",
     packages=["mypy_boto3_migrationhubstrategy"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.26.92 service generated"
-        " with mypy-boto3-builder 7.13.0"
+        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.27.0 service generated"
+        " with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -47,11 +47,11 @@
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/"
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


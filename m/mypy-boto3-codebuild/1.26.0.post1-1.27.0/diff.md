# Comparing `tmp/mypy-boto3-codebuild-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-codebuild-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codebuild-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:14 2022, max compression
+gzip compressed data, was "mypy-boto3-codebuild-1.27.0.tar", last modified: Mon Jul  3 19:50:31 2023, max compression
```

## Comparing `mypy-boto3-codebuild-1.26.0.post1.tar` & `mypy-boto3-codebuild-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.000818 mypy-boto3-codebuild-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:31:45.000000 mypy-boto3-codebuild-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    21044 2022-11-01 21:43:13.996818 mypy-boto3-codebuild-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    19595 2022-11-01 21:31:45.000000 mypy-boto3-codebuild-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:13.992818 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/
--rw-r--r--   0 runner    (1001) docker     (121)     3014 2022-11-01 21:31:45.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3013 2022-11-01 21:31:45.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-11-01 21:31:45.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    41432 2022-11-01 21:31:46.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    41368 2022-11-01 21:31:45.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13300 2022-11-01 21:31:46.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    13298 2022-11-01 21:31:46.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    15290 2022-11-01 21:31:46.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    15276 2022-11-01 21:31:46.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:31:45.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    57179 2022-11-01 21:31:47.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    57120 2022-11-01 21:31:47.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:31:45.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:13.996818 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    21044 2022-11-01 21:43:13.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-11-01 21:43:13.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:13.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:13.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:13.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-01 21:43:13.000000 mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:14.000818 mypy-boto3-codebuild-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-11-01 21:31:45.000000 mypy-boto3-codebuild-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.758984 mypy-boto3-codebuild-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:09.000000 mypy-boto3-codebuild-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-07-03 19:50:31.758984 mypy-boto3-codebuild-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-03 19:34:09.000000 mypy-boto3-codebuild-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.754984 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-03 19:34:09.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-03 19:34:09.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:34:09.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41431 2023-07-03 19:34:09.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41367 2023-07-03 19:34:09.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-07-03 19:34:09.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-07-03 19:34:09.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-07-03 19:34:09.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15324 2023-07-03 19:34:09.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:09.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57281 2023-07-03 19:34:11.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57222 2023-07-03 19:34:11.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:09.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.758984 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-07-03 19:50:31.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 19:50:31.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:31.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:50:31.000000 mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:31.758984 mypy-boto3-codebuild-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:34:09.000000 mypy-boto3-codebuild-1.27.0/setup.py
```

### Comparing `mypy-boto3-codebuild-1.26.0.post1/LICENSE` & `mypy-boto3-codebuild-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-codebuild-1.26.0.post1/PKG-INFO` & `mypy-boto3-codebuild-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codebuild
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodeBuild 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeBuild 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/
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
 
 <a id="mypy-boto3-codebuild"></a>
 
 # mypy-boto3-codebuild
 
 [![PyPI - mypy-boto3-codebuild](https://img.shields.io/pypi/v/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codebuild?color=blue)](https://pypistats.org/packages/mypy-boto3-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeBuild 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[boto3.CodeBuild 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [mypy-boto3-codebuild docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/).
 
 See how it helps to find and fix potential bugs:
 
@@ -406,15 +407,14 @@
 `mypy_boto3_codebuild.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codebuild.type_defs import (
     BatchDeleteBuildsInputRequestTypeDef,
     BuildNotDeletedTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetBuildBatchesInputRequestTypeDef,
     BatchGetBuildsInputRequestTypeDef,
     BatchGetProjectsInputRequestTypeDef,
     BatchGetReportGroupsInputRequestTypeDef,
     BatchGetReportsInputRequestTypeDef,
     BatchRestrictionsTypeDef,
     BuildArtifactsTypeDef,
@@ -437,84 +437,85 @@
     WebhookFilterTypeDef,
     DeleteBuildBatchInputRequestTypeDef,
     DeleteProjectInputRequestTypeDef,
     DeleteReportGroupInputRequestTypeDef,
     DeleteReportInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteSourceCredentialsInputRequestTypeDef,
+    DeleteSourceCredentialsOutputTypeDef,
     DeleteWebhookInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
     DescribeCodeCoveragesInputRequestTypeDef,
     TestCaseFilterTypeDef,
     TestCaseTypeDef,
     EnvironmentImageTypeDef,
     EnvironmentVariableTypeDef,
     GetReportGroupTrendInputRequestTypeDef,
     ReportGroupTrendStatsTypeDef,
     ReportWithRawDataTypeDef,
     GetResourcePolicyInputRequestTypeDef,
+    GetResourcePolicyOutputTypeDef,
     GitSubmodulesConfigTypeDef,
     ImportSourceCredentialsInputRequestTypeDef,
+    ImportSourceCredentialsOutputTypeDef,
     InvalidateProjectCacheInputRequestTypeDef,
+    ListBuildBatchesForProjectOutputTypeDef,
+    ListBuildBatchesOutputTypeDef,
+    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
     ListBuildsForProjectInputRequestTypeDef,
+    ListBuildsForProjectOutputTypeDef,
+    ListBuildsInputListBuildsPaginateTypeDef,
     ListBuildsInputRequestTypeDef,
+    ListBuildsOutputTypeDef,
+    ListProjectsInputListProjectsPaginateTypeDef,
     ListProjectsInputRequestTypeDef,
+    ListProjectsOutputTypeDef,
+    ListReportGroupsInputListReportGroupsPaginateTypeDef,
     ListReportGroupsInputRequestTypeDef,
+    ListReportGroupsOutputTypeDef,
     ReportFilterTypeDef,
+    ListReportsForReportGroupOutputTypeDef,
+    ListReportsOutputTypeDef,
+    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
     ListSharedProjectsInputRequestTypeDef,
+    ListSharedProjectsOutputTypeDef,
+    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     ListSharedReportGroupsInputRequestTypeDef,
+    ListSharedReportGroupsOutputTypeDef,
     SourceCredentialsInfoTypeDef,
     S3LogsConfigTypeDef,
+    PaginatorConfigTypeDef,
     ProjectBadgeTypeDef,
     RegistryCredentialTypeDef,
     SourceAuthTypeDef,
     PutResourcePolicyInputRequestTypeDef,
+    PutResourcePolicyOutputTypeDef,
     S3ReportExportConfigTypeDef,
     TestReportSummaryTypeDef,
+    ResponseMetadataTypeDef,
     RetryBuildBatchInputRequestTypeDef,
     RetryBuildInputRequestTypeDef,
     StopBuildBatchInputRequestTypeDef,
     StopBuildInputRequestTypeDef,
     UpdateProjectVisibilityInputRequestTypeDef,
+    UpdateProjectVisibilityOutputTypeDef,
     BatchDeleteBuildsOutputTypeDef,
     DeleteBuildBatchOutputTypeDef,
-    DeleteSourceCredentialsOutputTypeDef,
-    GetResourcePolicyOutputTypeDef,
-    ImportSourceCredentialsOutputTypeDef,
-    ListBuildBatchesForProjectOutputTypeDef,
-    ListBuildBatchesOutputTypeDef,
-    ListBuildsForProjectOutputTypeDef,
-    ListBuildsOutputTypeDef,
-    ListProjectsOutputTypeDef,
-    ListReportGroupsOutputTypeDef,
-    ListReportsForReportGroupOutputTypeDef,
-    ListReportsOutputTypeDef,
-    ListSharedProjectsOutputTypeDef,
-    ListSharedReportGroupsOutputTypeDef,
-    PutResourcePolicyOutputTypeDef,
-    UpdateProjectVisibilityOutputTypeDef,
     ProjectBuildBatchConfigTypeDef,
+    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
     ListBuildBatchesForProjectInputRequestTypeDef,
+    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
     ListBuildBatchesInputRequestTypeDef,
     BuildBatchPhaseTypeDef,
     BuildPhaseTypeDef,
     BuildSummaryTypeDef,
     DescribeCodeCoveragesOutputTypeDef,
     CreateWebhookInputRequestTypeDef,
     UpdateWebhookInputRequestTypeDef,
     WebhookTypeDef,
-    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
-    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
-    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
-    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
-    ListBuildsInputListBuildsPaginateTypeDef,
-    ListProjectsInputListProjectsPaginateTypeDef,
-    ListReportGroupsInputListReportGroupsPaginateTypeDef,
-    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
-    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     DescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     DescribeTestCasesInputRequestTypeDef,
     DescribeTestCasesOutputTypeDef,
     EnvironmentLanguageTypeDef,
     GetReportGroupTrendOutputTypeDef,
     ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     ListReportsForReportGroupInputRequestTypeDef,
@@ -567,42 +568,42 @@
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

### Comparing `mypy-boto3-codebuild-1.26.0.post1/README.md` & `mypy-boto3-codebuild-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codebuild"></a>
 
 # mypy-boto3-codebuild
 
 [![PyPI - mypy-boto3-codebuild](https://img.shields.io/pypi/v/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codebuild?color=blue)](https://pypistats.org/packages/mypy-boto3-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeBuild 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[boto3.CodeBuild 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [mypy-boto3-codebuild docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/).
 
 See how it helps to find and fix potential bugs:
 
@@ -375,15 +375,14 @@
 `mypy_boto3_codebuild.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codebuild.type_defs import (
     BatchDeleteBuildsInputRequestTypeDef,
     BuildNotDeletedTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetBuildBatchesInputRequestTypeDef,
     BatchGetBuildsInputRequestTypeDef,
     BatchGetProjectsInputRequestTypeDef,
     BatchGetReportGroupsInputRequestTypeDef,
     BatchGetReportsInputRequestTypeDef,
     BatchRestrictionsTypeDef,
     BuildArtifactsTypeDef,
@@ -406,84 +405,85 @@
     WebhookFilterTypeDef,
     DeleteBuildBatchInputRequestTypeDef,
     DeleteProjectInputRequestTypeDef,
     DeleteReportGroupInputRequestTypeDef,
     DeleteReportInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteSourceCredentialsInputRequestTypeDef,
+    DeleteSourceCredentialsOutputTypeDef,
     DeleteWebhookInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
     DescribeCodeCoveragesInputRequestTypeDef,
     TestCaseFilterTypeDef,
     TestCaseTypeDef,
     EnvironmentImageTypeDef,
     EnvironmentVariableTypeDef,
     GetReportGroupTrendInputRequestTypeDef,
     ReportGroupTrendStatsTypeDef,
     ReportWithRawDataTypeDef,
     GetResourcePolicyInputRequestTypeDef,
+    GetResourcePolicyOutputTypeDef,
     GitSubmodulesConfigTypeDef,
     ImportSourceCredentialsInputRequestTypeDef,
+    ImportSourceCredentialsOutputTypeDef,
     InvalidateProjectCacheInputRequestTypeDef,
+    ListBuildBatchesForProjectOutputTypeDef,
+    ListBuildBatchesOutputTypeDef,
+    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
     ListBuildsForProjectInputRequestTypeDef,
+    ListBuildsForProjectOutputTypeDef,
+    ListBuildsInputListBuildsPaginateTypeDef,
     ListBuildsInputRequestTypeDef,
+    ListBuildsOutputTypeDef,
+    ListProjectsInputListProjectsPaginateTypeDef,
     ListProjectsInputRequestTypeDef,
+    ListProjectsOutputTypeDef,
+    ListReportGroupsInputListReportGroupsPaginateTypeDef,
     ListReportGroupsInputRequestTypeDef,
+    ListReportGroupsOutputTypeDef,
     ReportFilterTypeDef,
+    ListReportsForReportGroupOutputTypeDef,
+    ListReportsOutputTypeDef,
+    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
     ListSharedProjectsInputRequestTypeDef,
+    ListSharedProjectsOutputTypeDef,
+    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     ListSharedReportGroupsInputRequestTypeDef,
+    ListSharedReportGroupsOutputTypeDef,
     SourceCredentialsInfoTypeDef,
     S3LogsConfigTypeDef,
+    PaginatorConfigTypeDef,
     ProjectBadgeTypeDef,
     RegistryCredentialTypeDef,
     SourceAuthTypeDef,
     PutResourcePolicyInputRequestTypeDef,
+    PutResourcePolicyOutputTypeDef,
     S3ReportExportConfigTypeDef,
     TestReportSummaryTypeDef,
+    ResponseMetadataTypeDef,
     RetryBuildBatchInputRequestTypeDef,
     RetryBuildInputRequestTypeDef,
     StopBuildBatchInputRequestTypeDef,
     StopBuildInputRequestTypeDef,
     UpdateProjectVisibilityInputRequestTypeDef,
+    UpdateProjectVisibilityOutputTypeDef,
     BatchDeleteBuildsOutputTypeDef,
     DeleteBuildBatchOutputTypeDef,
-    DeleteSourceCredentialsOutputTypeDef,
-    GetResourcePolicyOutputTypeDef,
-    ImportSourceCredentialsOutputTypeDef,
-    ListBuildBatchesForProjectOutputTypeDef,
-    ListBuildBatchesOutputTypeDef,
-    ListBuildsForProjectOutputTypeDef,
-    ListBuildsOutputTypeDef,
-    ListProjectsOutputTypeDef,
-    ListReportGroupsOutputTypeDef,
-    ListReportsForReportGroupOutputTypeDef,
-    ListReportsOutputTypeDef,
-    ListSharedProjectsOutputTypeDef,
-    ListSharedReportGroupsOutputTypeDef,
-    PutResourcePolicyOutputTypeDef,
-    UpdateProjectVisibilityOutputTypeDef,
     ProjectBuildBatchConfigTypeDef,
+    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
     ListBuildBatchesForProjectInputRequestTypeDef,
+    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
     ListBuildBatchesInputRequestTypeDef,
     BuildBatchPhaseTypeDef,
     BuildPhaseTypeDef,
     BuildSummaryTypeDef,
     DescribeCodeCoveragesOutputTypeDef,
     CreateWebhookInputRequestTypeDef,
     UpdateWebhookInputRequestTypeDef,
     WebhookTypeDef,
-    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
-    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
-    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
-    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
-    ListBuildsInputListBuildsPaginateTypeDef,
-    ListProjectsInputListProjectsPaginateTypeDef,
-    ListReportGroupsInputListReportGroupsPaginateTypeDef,
-    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
-    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     DescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     DescribeTestCasesInputRequestTypeDef,
     DescribeTestCasesOutputTypeDef,
     EnvironmentLanguageTypeDef,
     GetReportGroupTrendOutputTypeDef,
     ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     ListReportsForReportGroupInputRequestTypeDef,
@@ -536,42 +536,42 @@
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

### Comparing `mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/__init__.py` & `mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/__init__.pyi` & `mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/__main__.py` & `mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeBuild 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.CodeBuild 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild\nOther"
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

### Comparing `mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/client.py` & `mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -550,15 +550,15 @@
         reportGroupArn: str,
         nextToken: str = ...,
         sortOrder: SortOrderTypeType = ...,
         maxResults: int = ...,
         filter: ReportFilterTypeDef = ...
     ) -> ListReportsForReportGroupOutputTypeDef:
         """
-        Returns a list of ARNs for the reports that belong to a `ReportGroup` .
+        Returns a list of ARNs for the reports that belong to a `ReportGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_reports_for_report_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/client/#list_reports_for_report_group)
         """
 
     def list_shared_projects(
         self,
```

### Comparing `mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/client.pyi` & `mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -512,15 +512,15 @@
         reportGroupArn: str,
         nextToken: str = ...,
         sortOrder: SortOrderTypeType = ...,
         maxResults: int = ...,
         filter: ReportFilterTypeDef = ...
     ) -> ListReportsForReportGroupOutputTypeDef:
         """
-        Returns a list of ARNs for the reports that belong to a `ReportGroup` .
+        Returns a list of ARNs for the reports that belong to a `ReportGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.list_reports_for_report_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/client/#list_reports_for_report_group)
         """
     def list_shared_projects(
         self,
         *,
```

### Comparing `mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/literals.py` & `mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,23 +187,25 @@
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
@@ -213,30 +215,35 @@
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
@@ -262,14 +269,15 @@
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
@@ -314,51 +322,57 @@
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
@@ -371,14 +385,15 @@
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
@@ -390,28 +405,35 @@
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
@@ -420,14 +442,15 @@
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
@@ -438,55 +461,64 @@
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
@@ -525,24 +557,29 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
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

### Comparing `mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/literals.pyi` & `mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -185,23 +185,25 @@
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
@@ -211,30 +213,35 @@
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
@@ -260,14 +267,15 @@
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
@@ -312,51 +320,57 @@
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
@@ -369,14 +383,15 @@
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
@@ -388,28 +403,35 @@
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
@@ -418,14 +440,15 @@
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
@@ -436,55 +459,64 @@
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
@@ -523,24 +555,29 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
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

### Comparing `mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/paginator.py` & `mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         self,
         *,
         reportArn: str,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportCodeCoverageSortByTypeType = ...,
         minLineCoveragePercentage: float = ...,
         maxLineCoveragePercentage: float = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeCodeCoveragesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeCodeCoverages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#describecodecoveragespaginator)
         """
 
 
@@ -126,15 +126,15 @@
     """
 
     def paginate(
         self,
         *,
         reportArn: str,
         filter: TestCaseFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTestCasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeTestCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#describetestcasespaginator)
         """
 
 
@@ -145,15 +145,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBuildBatchesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildbatchespaginator)
         """
 
 
@@ -165,30 +165,33 @@
 
     def paginate(
         self,
         *,
         projectName: str = ...,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBuildBatchesForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatchesForProject.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildbatchesforprojectpaginator)
         """
 
 
 class ListBuildsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuilds)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildspaginator)
     """
 
     def paginate(
-        self, *, sortOrder: SortOrderTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        sortOrder: SortOrderTypeType = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBuildsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuilds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildspaginator)
         """
 
 
@@ -199,15 +202,15 @@
     """
 
     def paginate(
         self,
         *,
         projectName: str,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBuildsForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildsForProject.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildsforprojectpaginator)
         """
 
 
@@ -218,15 +221,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: ProjectSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listprojectspaginator)
         """
 
 
@@ -237,15 +240,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportGroupSortByTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listreportgroupspaginator)
         """
 
 
@@ -256,15 +259,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listreportspaginator)
         """
 
 
@@ -276,15 +279,15 @@
 
     def paginate(
         self,
         *,
         reportGroupArn: str,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReportsForReportGroupOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportsForReportGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listreportsforreportgrouppaginator)
         """
 
 
@@ -295,15 +298,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: SharedResourceSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSharedProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listsharedprojectspaginator)
         """
 
 
@@ -314,13 +317,13 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: SharedResourceSortByTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSharedReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedReportGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listsharedreportgroupspaginator)
         """
```

### Comparing `mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/paginator.pyi` & `mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         self,
         *,
         reportArn: str,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportCodeCoverageSortByTypeType = ...,
         minLineCoveragePercentage: float = ...,
         maxLineCoveragePercentage: float = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeCodeCoveragesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeCodeCoverages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#describecodecoveragespaginator)
         """
 
 class DescribeTestCasesPaginator(Paginator):
@@ -122,15 +122,15 @@
     """
 
     def paginate(
         self,
         *,
         reportArn: str,
         filter: TestCaseFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTestCasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeTestCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#describetestcasespaginator)
         """
 
 class ListBuildBatchesPaginator(Paginator):
@@ -140,15 +140,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBuildBatchesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildbatchespaginator)
         """
 
 class ListBuildBatchesForProjectPaginator(Paginator):
@@ -159,29 +159,32 @@
 
     def paginate(
         self,
         *,
         projectName: str = ...,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBuildBatchesForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatchesForProject.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildbatchesforprojectpaginator)
         """
 
 class ListBuildsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuilds)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildspaginator)
     """
 
     def paginate(
-        self, *, sortOrder: SortOrderTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        sortOrder: SortOrderTypeType = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBuildsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuilds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildspaginator)
         """
 
 class ListBuildsForProjectPaginator(Paginator):
@@ -191,15 +194,15 @@
     """
 
     def paginate(
         self,
         *,
         projectName: str,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBuildsForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildsForProject.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listbuildsforprojectpaginator)
         """
 
 class ListProjectsPaginator(Paginator):
@@ -209,15 +212,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: ProjectSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listprojectspaginator)
         """
 
 class ListReportGroupsPaginator(Paginator):
@@ -227,15 +230,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportGroupSortByTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listreportgroupspaginator)
         """
 
 class ListReportsPaginator(Paginator):
@@ -245,15 +248,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listreportspaginator)
         """
 
 class ListReportsForReportGroupPaginator(Paginator):
@@ -264,15 +267,15 @@
 
     def paginate(
         self,
         *,
         reportGroupArn: str,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReportsForReportGroupOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportsForReportGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listreportsforreportgrouppaginator)
         """
 
 class ListSharedProjectsPaginator(Paginator):
@@ -282,15 +285,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: SharedResourceSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSharedProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listsharedprojectspaginator)
         """
 
 class ListSharedReportGroupsPaginator(Paginator):
@@ -300,13 +303,13 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: SharedResourceSortByTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSharedReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedReportGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/paginators/#listsharedreportgroupspaginator)
         """
```

### Comparing `mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/type_defs.py` & `mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BatchDeleteBuildsInputRequestTypeDef",
     "BuildNotDeletedTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchGetBuildBatchesInputRequestTypeDef",
     "BatchGetBuildsInputRequestTypeDef",
     "BatchGetProjectsInputRequestTypeDef",
     "BatchGetReportGroupsInputRequestTypeDef",
     "BatchGetReportsInputRequestTypeDef",
     "BatchRestrictionsTypeDef",
     "BuildArtifactsTypeDef",
@@ -93,84 +92,85 @@
     "WebhookFilterTypeDef",
     "DeleteBuildBatchInputRequestTypeDef",
     "DeleteProjectInputRequestTypeDef",
     "DeleteReportGroupInputRequestTypeDef",
     "DeleteReportInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteSourceCredentialsInputRequestTypeDef",
+    "DeleteSourceCredentialsOutputTypeDef",
     "DeleteWebhookInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
     "DescribeCodeCoveragesInputRequestTypeDef",
     "TestCaseFilterTypeDef",
     "TestCaseTypeDef",
     "EnvironmentImageTypeDef",
     "EnvironmentVariableTypeDef",
     "GetReportGroupTrendInputRequestTypeDef",
     "ReportGroupTrendStatsTypeDef",
     "ReportWithRawDataTypeDef",
     "GetResourcePolicyInputRequestTypeDef",
+    "GetResourcePolicyOutputTypeDef",
     "GitSubmodulesConfigTypeDef",
     "ImportSourceCredentialsInputRequestTypeDef",
+    "ImportSourceCredentialsOutputTypeDef",
     "InvalidateProjectCacheInputRequestTypeDef",
+    "ListBuildBatchesForProjectOutputTypeDef",
+    "ListBuildBatchesOutputTypeDef",
+    "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
     "ListBuildsForProjectInputRequestTypeDef",
+    "ListBuildsForProjectOutputTypeDef",
+    "ListBuildsInputListBuildsPaginateTypeDef",
     "ListBuildsInputRequestTypeDef",
+    "ListBuildsOutputTypeDef",
+    "ListProjectsInputListProjectsPaginateTypeDef",
     "ListProjectsInputRequestTypeDef",
+    "ListProjectsOutputTypeDef",
+    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
     "ListReportGroupsInputRequestTypeDef",
+    "ListReportGroupsOutputTypeDef",
     "ReportFilterTypeDef",
+    "ListReportsForReportGroupOutputTypeDef",
+    "ListReportsOutputTypeDef",
+    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
     "ListSharedProjectsInputRequestTypeDef",
+    "ListSharedProjectsOutputTypeDef",
+    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
     "ListSharedReportGroupsInputRequestTypeDef",
+    "ListSharedReportGroupsOutputTypeDef",
     "SourceCredentialsInfoTypeDef",
     "S3LogsConfigTypeDef",
+    "PaginatorConfigTypeDef",
     "ProjectBadgeTypeDef",
     "RegistryCredentialTypeDef",
     "SourceAuthTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
+    "PutResourcePolicyOutputTypeDef",
     "S3ReportExportConfigTypeDef",
     "TestReportSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "RetryBuildBatchInputRequestTypeDef",
     "RetryBuildInputRequestTypeDef",
     "StopBuildBatchInputRequestTypeDef",
     "StopBuildInputRequestTypeDef",
     "UpdateProjectVisibilityInputRequestTypeDef",
+    "UpdateProjectVisibilityOutputTypeDef",
     "BatchDeleteBuildsOutputTypeDef",
     "DeleteBuildBatchOutputTypeDef",
-    "DeleteSourceCredentialsOutputTypeDef",
-    "GetResourcePolicyOutputTypeDef",
-    "ImportSourceCredentialsOutputTypeDef",
-    "ListBuildBatchesForProjectOutputTypeDef",
-    "ListBuildBatchesOutputTypeDef",
-    "ListBuildsForProjectOutputTypeDef",
-    "ListBuildsOutputTypeDef",
-    "ListProjectsOutputTypeDef",
-    "ListReportGroupsOutputTypeDef",
-    "ListReportsForReportGroupOutputTypeDef",
-    "ListReportsOutputTypeDef",
-    "ListSharedProjectsOutputTypeDef",
-    "ListSharedReportGroupsOutputTypeDef",
-    "PutResourcePolicyOutputTypeDef",
-    "UpdateProjectVisibilityOutputTypeDef",
     "ProjectBuildBatchConfigTypeDef",
+    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
     "ListBuildBatchesForProjectInputRequestTypeDef",
+    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
     "ListBuildBatchesInputRequestTypeDef",
     "BuildBatchPhaseTypeDef",
     "BuildPhaseTypeDef",
     "BuildSummaryTypeDef",
     "DescribeCodeCoveragesOutputTypeDef",
     "CreateWebhookInputRequestTypeDef",
     "UpdateWebhookInputRequestTypeDef",
     "WebhookTypeDef",
-    "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
-    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
-    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
-    "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
-    "ListBuildsInputListBuildsPaginateTypeDef",
-    "ListProjectsInputListProjectsPaginateTypeDef",
-    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
-    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
-    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
     "DescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     "DescribeTestCasesInputRequestTypeDef",
     "DescribeTestCasesOutputTypeDef",
     "EnvironmentLanguageTypeDef",
     "GetReportGroupTrendOutputTypeDef",
     "ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     "ListReportsForReportGroupInputRequestTypeDef",
@@ -227,25 +227,14 @@
     {
         "id": str,
         "statusCode": str,
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
 BatchGetBuildBatchesInputRequestTypeDef = TypedDict(
     "BatchGetBuildBatchesInputRequestTypeDef",
     {
         "ids": Sequence[str],
     },
 )
 
@@ -573,31 +562,55 @@
 DeleteSourceCredentialsInputRequestTypeDef = TypedDict(
     "DeleteSourceCredentialsInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+DeleteSourceCredentialsOutputTypeDef = TypedDict(
+    "DeleteSourceCredentialsOutputTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteWebhookInputRequestTypeDef = TypedDict(
     "DeleteWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "reportArn": str,
+    },
+)
+_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": ReportCodeCoverageSortByTypeType,
+        "minLineCoveragePercentage": float,
+        "maxLineCoveragePercentage": float,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef(
+    _RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    _OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeCodeCoveragesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeCodeCoveragesInputRequestTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeCodeCoveragesInputRequestTypeDef = TypedDict(
@@ -721,14 +734,22 @@
 GetResourcePolicyInputRequestTypeDef = TypedDict(
     "GetResourcePolicyInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+GetResourcePolicyOutputTypeDef = TypedDict(
+    "GetResourcePolicyOutputTypeDef",
+    {
+        "policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GitSubmodulesConfigTypeDef = TypedDict(
     "GitSubmodulesConfigTypeDef",
     {
         "fetchSubmodules": bool,
     },
 )
 
@@ -753,21 +774,70 @@
 class ImportSourceCredentialsInputRequestTypeDef(
     _RequiredImportSourceCredentialsInputRequestTypeDef,
     _OptionalImportSourceCredentialsInputRequestTypeDef,
 ):
     pass
 
 
+ImportSourceCredentialsOutputTypeDef = TypedDict(
+    "ImportSourceCredentialsOutputTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InvalidateProjectCacheInputRequestTypeDef = TypedDict(
     "InvalidateProjectCacheInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
+ListBuildBatchesForProjectOutputTypeDef = TypedDict(
+    "ListBuildBatchesForProjectOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBuildBatchesOutputTypeDef = TypedDict(
+    "ListBuildBatchesOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
+    "_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    {
+        "projectName": str,
+    },
+)
+_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
+    "_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef(
+    _RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+    _OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListBuildsForProjectInputRequestTypeDef = TypedDict(
     "_RequiredListBuildsForProjectInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalListBuildsForProjectInputRequestTypeDef = TypedDict(
@@ -783,74 +853,195 @@
 class ListBuildsForProjectInputRequestTypeDef(
     _RequiredListBuildsForProjectInputRequestTypeDef,
     _OptionalListBuildsForProjectInputRequestTypeDef,
 ):
     pass
 
 
+ListBuildsForProjectOutputTypeDef = TypedDict(
+    "ListBuildsForProjectOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBuildsInputListBuildsPaginateTypeDef = TypedDict(
+    "ListBuildsInputListBuildsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBuildsInputRequestTypeDef = TypedDict(
     "ListBuildsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
+ListBuildsOutputTypeDef = TypedDict(
+    "ListBuildsOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListProjectsInputListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsInputListProjectsPaginateTypeDef",
+    {
+        "sortBy": ProjectSortByTypeType,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProjectsInputRequestTypeDef = TypedDict(
     "ListProjectsInputRequestTypeDef",
     {
         "sortBy": ProjectSortByTypeType,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
+ListProjectsOutputTypeDef = TypedDict(
+    "ListProjectsOutputTypeDef",
+    {
+        "nextToken": str,
+        "projects": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListReportGroupsInputListReportGroupsPaginateTypeDef = TypedDict(
+    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": ReportGroupSortByTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReportGroupsInputRequestTypeDef = TypedDict(
     "ListReportGroupsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "sortBy": ReportGroupSortByTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListReportGroupsOutputTypeDef = TypedDict(
+    "ListReportGroupsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reportGroups": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ReportFilterTypeDef = TypedDict(
     "ReportFilterTypeDef",
     {
         "status": ReportStatusTypeType,
     },
     total=False,
 )
 
+ListReportsForReportGroupOutputTypeDef = TypedDict(
+    "ListReportsForReportGroupOutputTypeDef",
+    {
+        "nextToken": str,
+        "reports": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListReportsOutputTypeDef = TypedDict(
+    "ListReportsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reports": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSharedProjectsInputListSharedProjectsPaginateTypeDef = TypedDict(
+    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
+    {
+        "sortBy": SharedResourceSortByTypeType,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSharedProjectsInputRequestTypeDef = TypedDict(
     "ListSharedProjectsInputRequestTypeDef",
     {
         "sortBy": SharedResourceSortByTypeType,
         "sortOrder": SortOrderTypeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListSharedProjectsOutputTypeDef = TypedDict(
+    "ListSharedProjectsOutputTypeDef",
+    {
+        "nextToken": str,
+        "projects": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef = TypedDict(
+    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": SharedResourceSortByTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSharedReportGroupsInputRequestTypeDef = TypedDict(
     "ListSharedReportGroupsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "sortBy": SharedResourceSortByTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListSharedReportGroupsOutputTypeDef = TypedDict(
+    "ListSharedReportGroupsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reportGroups": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SourceCredentialsInfoTypeDef = TypedDict(
     "SourceCredentialsInfoTypeDef",
     {
         "arn": str,
         "serverType": ServerTypeType,
         "authType": AuthTypeType,
     },
@@ -874,14 +1065,24 @@
 )
 
 
 class S3LogsConfigTypeDef(_RequiredS3LogsConfigTypeDef, _OptionalS3LogsConfigTypeDef):
     pass
 
 
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
 ProjectBadgeTypeDef = TypedDict(
     "ProjectBadgeTypeDef",
     {
         "badgeEnabled": bool,
         "badgeRequestUrl": str,
     },
     total=False,
@@ -918,14 +1119,22 @@
     "PutResourcePolicyInputRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
     },
 )
 
+PutResourcePolicyOutputTypeDef = TypedDict(
+    "PutResourcePolicyOutputTypeDef",
+    {
+        "resourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 S3ReportExportConfigTypeDef = TypedDict(
     "S3ReportExportConfigTypeDef",
     {
         "bucket": str,
         "bucketOwner": str,
         "path": str,
         "packaging": ReportPackagingTypeType,
@@ -940,14 +1149,25 @@
     {
         "total": int,
         "statusCounts": Dict[str, int],
         "durationInNanoSeconds": int,
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
 RetryBuildBatchInputRequestTypeDef = TypedDict(
     "RetryBuildBatchInputRequestTypeDef",
     {
         "id": str,
         "idempotencyToken": str,
         "retryType": RetryBuildBatchTypeType,
     },
@@ -996,162 +1216,40 @@
 class UpdateProjectVisibilityInputRequestTypeDef(
     _RequiredUpdateProjectVisibilityInputRequestTypeDef,
     _OptionalUpdateProjectVisibilityInputRequestTypeDef,
 ):
     pass
 
 
+UpdateProjectVisibilityOutputTypeDef = TypedDict(
+    "UpdateProjectVisibilityOutputTypeDef",
+    {
+        "projectArn": str,
+        "publicProjectAlias": str,
+        "projectVisibility": ProjectVisibilityTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchDeleteBuildsOutputTypeDef = TypedDict(
     "BatchDeleteBuildsOutputTypeDef",
     {
         "buildsDeleted": List[str],
         "buildsNotDeleted": List[BuildNotDeletedTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteBuildBatchOutputTypeDef = TypedDict(
     "DeleteBuildBatchOutputTypeDef",
     {
         "statusCode": str,
         "buildsDeleted": List[str],
         "buildsNotDeleted": List[BuildNotDeletedTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSourceCredentialsOutputTypeDef = TypedDict(
-    "DeleteSourceCredentialsOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetResourcePolicyOutputTypeDef = TypedDict(
-    "GetResourcePolicyOutputTypeDef",
-    {
-        "policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ImportSourceCredentialsOutputTypeDef = TypedDict(
-    "ImportSourceCredentialsOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBuildBatchesForProjectOutputTypeDef = TypedDict(
-    "ListBuildBatchesForProjectOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBuildBatchesOutputTypeDef = TypedDict(
-    "ListBuildBatchesOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBuildsForProjectOutputTypeDef = TypedDict(
-    "ListBuildsForProjectOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBuildsOutputTypeDef = TypedDict(
-    "ListBuildsOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListProjectsOutputTypeDef = TypedDict(
-    "ListProjectsOutputTypeDef",
-    {
-        "nextToken": str,
-        "projects": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListReportGroupsOutputTypeDef = TypedDict(
-    "ListReportGroupsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reportGroups": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListReportsForReportGroupOutputTypeDef = TypedDict(
-    "ListReportsForReportGroupOutputTypeDef",
-    {
-        "nextToken": str,
-        "reports": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListReportsOutputTypeDef = TypedDict(
-    "ListReportsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reports": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListSharedProjectsOutputTypeDef = TypedDict(
-    "ListSharedProjectsOutputTypeDef",
-    {
-        "nextToken": str,
-        "projects": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListSharedReportGroupsOutputTypeDef = TypedDict(
-    "ListSharedReportGroupsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reportGroups": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutResourcePolicyOutputTypeDef = TypedDict(
-    "PutResourcePolicyOutputTypeDef",
-    {
-        "resourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateProjectVisibilityOutputTypeDef = TypedDict(
-    "UpdateProjectVisibilityOutputTypeDef",
-    {
-        "projectArn": str,
-        "publicProjectAlias": str,
-        "projectVisibility": ProjectVisibilityTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProjectBuildBatchConfigTypeDef = TypedDict(
     "ProjectBuildBatchConfigTypeDef",
     {
         "serviceRole": str,
@@ -1159,26 +1257,47 @@
         "restrictions": BatchRestrictionsTypeDef,
         "timeoutInMins": int,
         "batchReportMode": BatchReportModeTypeType,
     },
     total=False,
 )
 
+ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef = TypedDict(
+    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
+    {
+        "projectName": str,
+        "filter": BuildBatchFilterTypeDef,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBuildBatchesForProjectInputRequestTypeDef = TypedDict(
     "ListBuildBatchesForProjectInputRequestTypeDef",
     {
         "projectName": str,
         "filter": BuildBatchFilterTypeDef,
         "maxResults": int,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
+ListBuildBatchesInputListBuildBatchesPaginateTypeDef = TypedDict(
+    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
+    {
+        "filter": BuildBatchFilterTypeDef,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBuildBatchesInputRequestTypeDef = TypedDict(
     "ListBuildBatchesInputRequestTypeDef",
     {
         "filter": BuildBatchFilterTypeDef,
         "maxResults": int,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
@@ -1225,15 +1344,15 @@
 )
 
 DescribeCodeCoveragesOutputTypeDef = TypedDict(
     "DescribeCodeCoveragesOutputTypeDef",
     {
         "nextToken": str,
         "codeCoverages": List[CodeCoverageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateWebhookInputRequestTypeDef = TypedDict(
     "_RequiredCreateWebhookInputRequestTypeDef",
     {
         "projectName": str,
@@ -1290,144 +1409,25 @@
         "filterGroups": List[List[WebhookFilterTypeDef]],
         "buildType": WebhookBuildTypeType,
         "lastModifiedSecret": datetime,
     },
     total=False,
 )
 
-_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
-    {
-        "reportArn": str,
-    },
-)
-_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": ReportCodeCoverageSortByTypeType,
-        "minLineCoveragePercentage": float,
-        "maxLineCoveragePercentage": float,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef(
-    _RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
-    _OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
-):
-    pass
-
-
-ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef = TypedDict(
-    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
-    {
-        "projectName": str,
-        "filter": BuildBatchFilterTypeDef,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListBuildBatchesInputListBuildBatchesPaginateTypeDef = TypedDict(
-    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
-    {
-        "filter": BuildBatchFilterTypeDef,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
-    "_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
-    {
-        "projectName": str,
-    },
-)
-_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
-    "_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef(
-    _RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
-    _OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
-):
-    pass
-
-
-ListBuildsInputListBuildsPaginateTypeDef = TypedDict(
-    "ListBuildsInputListBuildsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListProjectsInputListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsInputListProjectsPaginateTypeDef",
-    {
-        "sortBy": ProjectSortByTypeType,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListReportGroupsInputListReportGroupsPaginateTypeDef = TypedDict(
-    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": ReportGroupSortByTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSharedProjectsInputListSharedProjectsPaginateTypeDef = TypedDict(
-    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
-    {
-        "sortBy": SharedResourceSortByTypeType,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef = TypedDict(
-    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": SharedResourceSortByTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
     "_RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
     "_OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     {
         "filter": TestCaseFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeTestCasesInputDescribeTestCasesPaginateTypeDef(
     _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
@@ -1460,15 +1460,15 @@
 
 
 DescribeTestCasesOutputTypeDef = TypedDict(
     "DescribeTestCasesOutputTypeDef",
     {
         "nextToken": str,
         "testCases": List[TestCaseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentLanguageTypeDef = TypedDict(
     "EnvironmentLanguageTypeDef",
     {
         "language": LanguageTypeType,
@@ -1478,30 +1478,30 @@
 )
 
 GetReportGroupTrendOutputTypeDef = TypedDict(
     "GetReportGroupTrendOutputTypeDef",
     {
         "stats": ReportGroupTrendStatsTypeDef,
         "rawData": List[ReportWithRawDataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef = TypedDict(
     "_RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     {
         "reportGroupArn": str,
     },
 )
 _OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef = TypedDict(
     "_OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef(
     _RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
@@ -1536,15 +1536,15 @@
 
 
 ListReportsInputListReportsPaginateTypeDef = TypedDict(
     "ListReportsInputListReportsPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListReportsInputRequestTypeDef = TypedDict(
     "ListReportsInputRequestTypeDef",
     {
@@ -1556,15 +1556,15 @@
     total=False,
 )
 
 ListSourceCredentialsOutputTypeDef = TypedDict(
     "ListSourceCredentialsOutputTypeDef",
     {
         "sourceCredentialsInfos": List[SourceCredentialsInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LogsConfigTypeDef = TypedDict(
     "LogsConfigTypeDef",
     {
         "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
@@ -1663,23 +1663,23 @@
     total=False,
 )
 
 CreateWebhookOutputTypeDef = TypedDict(
     "CreateWebhookOutputTypeDef",
     {
         "webhook": WebhookTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateWebhookOutputTypeDef = TypedDict(
     "UpdateWebhookOutputTypeDef",
     {
         "webhook": WebhookTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentPlatformTypeDef = TypedDict(
     "EnvironmentPlatformTypeDef",
     {
         "platform": PlatformTypeType,
@@ -2058,135 +2058,135 @@
     total=False,
 )
 
 ListCuratedEnvironmentImagesOutputTypeDef = TypedDict(
     "ListCuratedEnvironmentImagesOutputTypeDef",
     {
         "platforms": List[EnvironmentPlatformTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetBuildsOutputTypeDef = TypedDict(
     "BatchGetBuildsOutputTypeDef",
     {
         "builds": List[BuildTypeDef],
         "buildsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RetryBuildOutputTypeDef = TypedDict(
     "RetryBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartBuildOutputTypeDef = TypedDict(
     "StartBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopBuildOutputTypeDef = TypedDict(
     "StopBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetProjectsOutputTypeDef = TypedDict(
     "BatchGetProjectsOutputTypeDef",
     {
         "projects": List[ProjectTypeDef],
         "projectsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateProjectOutputTypeDef = TypedDict(
     "CreateProjectOutputTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateProjectOutputTypeDef = TypedDict(
     "UpdateProjectOutputTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetReportGroupsOutputTypeDef = TypedDict(
     "BatchGetReportGroupsOutputTypeDef",
     {
         "reportGroups": List[ReportGroupTypeDef],
         "reportGroupsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateReportGroupOutputTypeDef = TypedDict(
     "CreateReportGroupOutputTypeDef",
     {
         "reportGroup": ReportGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateReportGroupOutputTypeDef = TypedDict(
     "UpdateReportGroupOutputTypeDef",
     {
         "reportGroup": ReportGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetReportsOutputTypeDef = TypedDict(
     "BatchGetReportsOutputTypeDef",
     {
         "reports": List[ReportTypeDef],
         "reportsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetBuildBatchesOutputTypeDef = TypedDict(
     "BatchGetBuildBatchesOutputTypeDef",
     {
         "buildBatches": List[BuildBatchTypeDef],
         "buildBatchesNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RetryBuildBatchOutputTypeDef = TypedDict(
     "RetryBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartBuildBatchOutputTypeDef = TypedDict(
     "StartBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopBuildBatchOutputTypeDef = TypedDict(
     "StopBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild/type_defs.pyi` & `mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BatchDeleteBuildsInputRequestTypeDef",
     "BuildNotDeletedTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchGetBuildBatchesInputRequestTypeDef",
     "BatchGetBuildsInputRequestTypeDef",
     "BatchGetProjectsInputRequestTypeDef",
     "BatchGetReportGroupsInputRequestTypeDef",
     "BatchGetReportsInputRequestTypeDef",
     "BatchRestrictionsTypeDef",
     "BuildArtifactsTypeDef",
@@ -92,84 +91,85 @@
     "WebhookFilterTypeDef",
     "DeleteBuildBatchInputRequestTypeDef",
     "DeleteProjectInputRequestTypeDef",
     "DeleteReportGroupInputRequestTypeDef",
     "DeleteReportInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteSourceCredentialsInputRequestTypeDef",
+    "DeleteSourceCredentialsOutputTypeDef",
     "DeleteWebhookInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
     "DescribeCodeCoveragesInputRequestTypeDef",
     "TestCaseFilterTypeDef",
     "TestCaseTypeDef",
     "EnvironmentImageTypeDef",
     "EnvironmentVariableTypeDef",
     "GetReportGroupTrendInputRequestTypeDef",
     "ReportGroupTrendStatsTypeDef",
     "ReportWithRawDataTypeDef",
     "GetResourcePolicyInputRequestTypeDef",
+    "GetResourcePolicyOutputTypeDef",
     "GitSubmodulesConfigTypeDef",
     "ImportSourceCredentialsInputRequestTypeDef",
+    "ImportSourceCredentialsOutputTypeDef",
     "InvalidateProjectCacheInputRequestTypeDef",
+    "ListBuildBatchesForProjectOutputTypeDef",
+    "ListBuildBatchesOutputTypeDef",
+    "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
     "ListBuildsForProjectInputRequestTypeDef",
+    "ListBuildsForProjectOutputTypeDef",
+    "ListBuildsInputListBuildsPaginateTypeDef",
     "ListBuildsInputRequestTypeDef",
+    "ListBuildsOutputTypeDef",
+    "ListProjectsInputListProjectsPaginateTypeDef",
     "ListProjectsInputRequestTypeDef",
+    "ListProjectsOutputTypeDef",
+    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
     "ListReportGroupsInputRequestTypeDef",
+    "ListReportGroupsOutputTypeDef",
     "ReportFilterTypeDef",
+    "ListReportsForReportGroupOutputTypeDef",
+    "ListReportsOutputTypeDef",
+    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
     "ListSharedProjectsInputRequestTypeDef",
+    "ListSharedProjectsOutputTypeDef",
+    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
     "ListSharedReportGroupsInputRequestTypeDef",
+    "ListSharedReportGroupsOutputTypeDef",
     "SourceCredentialsInfoTypeDef",
     "S3LogsConfigTypeDef",
+    "PaginatorConfigTypeDef",
     "ProjectBadgeTypeDef",
     "RegistryCredentialTypeDef",
     "SourceAuthTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
+    "PutResourcePolicyOutputTypeDef",
     "S3ReportExportConfigTypeDef",
     "TestReportSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "RetryBuildBatchInputRequestTypeDef",
     "RetryBuildInputRequestTypeDef",
     "StopBuildBatchInputRequestTypeDef",
     "StopBuildInputRequestTypeDef",
     "UpdateProjectVisibilityInputRequestTypeDef",
+    "UpdateProjectVisibilityOutputTypeDef",
     "BatchDeleteBuildsOutputTypeDef",
     "DeleteBuildBatchOutputTypeDef",
-    "DeleteSourceCredentialsOutputTypeDef",
-    "GetResourcePolicyOutputTypeDef",
-    "ImportSourceCredentialsOutputTypeDef",
-    "ListBuildBatchesForProjectOutputTypeDef",
-    "ListBuildBatchesOutputTypeDef",
-    "ListBuildsForProjectOutputTypeDef",
-    "ListBuildsOutputTypeDef",
-    "ListProjectsOutputTypeDef",
-    "ListReportGroupsOutputTypeDef",
-    "ListReportsForReportGroupOutputTypeDef",
-    "ListReportsOutputTypeDef",
-    "ListSharedProjectsOutputTypeDef",
-    "ListSharedReportGroupsOutputTypeDef",
-    "PutResourcePolicyOutputTypeDef",
-    "UpdateProjectVisibilityOutputTypeDef",
     "ProjectBuildBatchConfigTypeDef",
+    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
     "ListBuildBatchesForProjectInputRequestTypeDef",
+    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
     "ListBuildBatchesInputRequestTypeDef",
     "BuildBatchPhaseTypeDef",
     "BuildPhaseTypeDef",
     "BuildSummaryTypeDef",
     "DescribeCodeCoveragesOutputTypeDef",
     "CreateWebhookInputRequestTypeDef",
     "UpdateWebhookInputRequestTypeDef",
     "WebhookTypeDef",
-    "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
-    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
-    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
-    "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
-    "ListBuildsInputListBuildsPaginateTypeDef",
-    "ListProjectsInputListProjectsPaginateTypeDef",
-    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
-    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
-    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
     "DescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     "DescribeTestCasesInputRequestTypeDef",
     "DescribeTestCasesOutputTypeDef",
     "EnvironmentLanguageTypeDef",
     "GetReportGroupTrendOutputTypeDef",
     "ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     "ListReportsForReportGroupInputRequestTypeDef",
@@ -226,25 +226,14 @@
     {
         "id": str,
         "statusCode": str,
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
 BatchGetBuildBatchesInputRequestTypeDef = TypedDict(
     "BatchGetBuildBatchesInputRequestTypeDef",
     {
         "ids": Sequence[str],
     },
 )
 
@@ -562,31 +551,53 @@
 DeleteSourceCredentialsInputRequestTypeDef = TypedDict(
     "DeleteSourceCredentialsInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+DeleteSourceCredentialsOutputTypeDef = TypedDict(
+    "DeleteSourceCredentialsOutputTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteWebhookInputRequestTypeDef = TypedDict(
     "DeleteWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "reportArn": str,
+    },
+)
+_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": ReportCodeCoverageSortByTypeType,
+        "minLineCoveragePercentage": float,
+        "maxLineCoveragePercentage": float,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef(
+    _RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    _OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeCodeCoveragesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeCodeCoveragesInputRequestTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeCodeCoveragesInputRequestTypeDef = TypedDict(
@@ -704,14 +715,22 @@
 GetResourcePolicyInputRequestTypeDef = TypedDict(
     "GetResourcePolicyInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+GetResourcePolicyOutputTypeDef = TypedDict(
+    "GetResourcePolicyOutputTypeDef",
+    {
+        "policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GitSubmodulesConfigTypeDef = TypedDict(
     "GitSubmodulesConfigTypeDef",
     {
         "fetchSubmodules": bool,
     },
 )
 
@@ -734,21 +753,68 @@
 
 class ImportSourceCredentialsInputRequestTypeDef(
     _RequiredImportSourceCredentialsInputRequestTypeDef,
     _OptionalImportSourceCredentialsInputRequestTypeDef,
 ):
     pass
 
+ImportSourceCredentialsOutputTypeDef = TypedDict(
+    "ImportSourceCredentialsOutputTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InvalidateProjectCacheInputRequestTypeDef = TypedDict(
     "InvalidateProjectCacheInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
+ListBuildBatchesForProjectOutputTypeDef = TypedDict(
+    "ListBuildBatchesForProjectOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBuildBatchesOutputTypeDef = TypedDict(
+    "ListBuildBatchesOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
+    "_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    {
+        "projectName": str,
+    },
+)
+_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
+    "_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef(
+    _RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+    _OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+):
+    pass
+
 _RequiredListBuildsForProjectInputRequestTypeDef = TypedDict(
     "_RequiredListBuildsForProjectInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalListBuildsForProjectInputRequestTypeDef = TypedDict(
@@ -762,74 +828,195 @@
 
 class ListBuildsForProjectInputRequestTypeDef(
     _RequiredListBuildsForProjectInputRequestTypeDef,
     _OptionalListBuildsForProjectInputRequestTypeDef,
 ):
     pass
 
+ListBuildsForProjectOutputTypeDef = TypedDict(
+    "ListBuildsForProjectOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBuildsInputListBuildsPaginateTypeDef = TypedDict(
+    "ListBuildsInputListBuildsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBuildsInputRequestTypeDef = TypedDict(
     "ListBuildsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
+ListBuildsOutputTypeDef = TypedDict(
+    "ListBuildsOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListProjectsInputListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsInputListProjectsPaginateTypeDef",
+    {
+        "sortBy": ProjectSortByTypeType,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListProjectsInputRequestTypeDef = TypedDict(
     "ListProjectsInputRequestTypeDef",
     {
         "sortBy": ProjectSortByTypeType,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
+ListProjectsOutputTypeDef = TypedDict(
+    "ListProjectsOutputTypeDef",
+    {
+        "nextToken": str,
+        "projects": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListReportGroupsInputListReportGroupsPaginateTypeDef = TypedDict(
+    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": ReportGroupSortByTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReportGroupsInputRequestTypeDef = TypedDict(
     "ListReportGroupsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "sortBy": ReportGroupSortByTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListReportGroupsOutputTypeDef = TypedDict(
+    "ListReportGroupsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reportGroups": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ReportFilterTypeDef = TypedDict(
     "ReportFilterTypeDef",
     {
         "status": ReportStatusTypeType,
     },
     total=False,
 )
 
+ListReportsForReportGroupOutputTypeDef = TypedDict(
+    "ListReportsForReportGroupOutputTypeDef",
+    {
+        "nextToken": str,
+        "reports": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListReportsOutputTypeDef = TypedDict(
+    "ListReportsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reports": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSharedProjectsInputListSharedProjectsPaginateTypeDef = TypedDict(
+    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
+    {
+        "sortBy": SharedResourceSortByTypeType,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSharedProjectsInputRequestTypeDef = TypedDict(
     "ListSharedProjectsInputRequestTypeDef",
     {
         "sortBy": SharedResourceSortByTypeType,
         "sortOrder": SortOrderTypeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListSharedProjectsOutputTypeDef = TypedDict(
+    "ListSharedProjectsOutputTypeDef",
+    {
+        "nextToken": str,
+        "projects": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef = TypedDict(
+    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": SharedResourceSortByTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSharedReportGroupsInputRequestTypeDef = TypedDict(
     "ListSharedReportGroupsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "sortBy": SharedResourceSortByTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListSharedReportGroupsOutputTypeDef = TypedDict(
+    "ListSharedReportGroupsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reportGroups": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SourceCredentialsInfoTypeDef = TypedDict(
     "SourceCredentialsInfoTypeDef",
     {
         "arn": str,
         "serverType": ServerTypeType,
         "authType": AuthTypeType,
     },
@@ -851,14 +1038,24 @@
     },
     total=False,
 )
 
 class S3LogsConfigTypeDef(_RequiredS3LogsConfigTypeDef, _OptionalS3LogsConfigTypeDef):
     pass
 
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
 ProjectBadgeTypeDef = TypedDict(
     "ProjectBadgeTypeDef",
     {
         "badgeEnabled": bool,
         "badgeRequestUrl": str,
     },
     total=False,
@@ -893,14 +1090,22 @@
     "PutResourcePolicyInputRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
     },
 )
 
+PutResourcePolicyOutputTypeDef = TypedDict(
+    "PutResourcePolicyOutputTypeDef",
+    {
+        "resourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 S3ReportExportConfigTypeDef = TypedDict(
     "S3ReportExportConfigTypeDef",
     {
         "bucket": str,
         "bucketOwner": str,
         "path": str,
         "packaging": ReportPackagingTypeType,
@@ -915,14 +1120,25 @@
     {
         "total": int,
         "statusCounts": Dict[str, int],
         "durationInNanoSeconds": int,
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
 RetryBuildBatchInputRequestTypeDef = TypedDict(
     "RetryBuildBatchInputRequestTypeDef",
     {
         "id": str,
         "idempotencyToken": str,
         "retryType": RetryBuildBatchTypeType,
     },
@@ -969,162 +1185,40 @@
 
 class UpdateProjectVisibilityInputRequestTypeDef(
     _RequiredUpdateProjectVisibilityInputRequestTypeDef,
     _OptionalUpdateProjectVisibilityInputRequestTypeDef,
 ):
     pass
 
+UpdateProjectVisibilityOutputTypeDef = TypedDict(
+    "UpdateProjectVisibilityOutputTypeDef",
+    {
+        "projectArn": str,
+        "publicProjectAlias": str,
+        "projectVisibility": ProjectVisibilityTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchDeleteBuildsOutputTypeDef = TypedDict(
     "BatchDeleteBuildsOutputTypeDef",
     {
         "buildsDeleted": List[str],
         "buildsNotDeleted": List[BuildNotDeletedTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteBuildBatchOutputTypeDef = TypedDict(
     "DeleteBuildBatchOutputTypeDef",
     {
         "statusCode": str,
         "buildsDeleted": List[str],
         "buildsNotDeleted": List[BuildNotDeletedTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSourceCredentialsOutputTypeDef = TypedDict(
-    "DeleteSourceCredentialsOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetResourcePolicyOutputTypeDef = TypedDict(
-    "GetResourcePolicyOutputTypeDef",
-    {
-        "policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ImportSourceCredentialsOutputTypeDef = TypedDict(
-    "ImportSourceCredentialsOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBuildBatchesForProjectOutputTypeDef = TypedDict(
-    "ListBuildBatchesForProjectOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBuildBatchesOutputTypeDef = TypedDict(
-    "ListBuildBatchesOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBuildsForProjectOutputTypeDef = TypedDict(
-    "ListBuildsForProjectOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBuildsOutputTypeDef = TypedDict(
-    "ListBuildsOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListProjectsOutputTypeDef = TypedDict(
-    "ListProjectsOutputTypeDef",
-    {
-        "nextToken": str,
-        "projects": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListReportGroupsOutputTypeDef = TypedDict(
-    "ListReportGroupsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reportGroups": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListReportsForReportGroupOutputTypeDef = TypedDict(
-    "ListReportsForReportGroupOutputTypeDef",
-    {
-        "nextToken": str,
-        "reports": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListReportsOutputTypeDef = TypedDict(
-    "ListReportsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reports": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListSharedProjectsOutputTypeDef = TypedDict(
-    "ListSharedProjectsOutputTypeDef",
-    {
-        "nextToken": str,
-        "projects": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListSharedReportGroupsOutputTypeDef = TypedDict(
-    "ListSharedReportGroupsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reportGroups": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutResourcePolicyOutputTypeDef = TypedDict(
-    "PutResourcePolicyOutputTypeDef",
-    {
-        "resourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateProjectVisibilityOutputTypeDef = TypedDict(
-    "UpdateProjectVisibilityOutputTypeDef",
-    {
-        "projectArn": str,
-        "publicProjectAlias": str,
-        "projectVisibility": ProjectVisibilityTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ProjectBuildBatchConfigTypeDef = TypedDict(
     "ProjectBuildBatchConfigTypeDef",
     {
         "serviceRole": str,
@@ -1132,26 +1226,47 @@
         "restrictions": BatchRestrictionsTypeDef,
         "timeoutInMins": int,
         "batchReportMode": BatchReportModeTypeType,
     },
     total=False,
 )
 
+ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef = TypedDict(
+    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
+    {
+        "projectName": str,
+        "filter": BuildBatchFilterTypeDef,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBuildBatchesForProjectInputRequestTypeDef = TypedDict(
     "ListBuildBatchesForProjectInputRequestTypeDef",
     {
         "projectName": str,
         "filter": BuildBatchFilterTypeDef,
         "maxResults": int,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
+ListBuildBatchesInputListBuildBatchesPaginateTypeDef = TypedDict(
+    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
+    {
+        "filter": BuildBatchFilterTypeDef,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListBuildBatchesInputRequestTypeDef = TypedDict(
     "ListBuildBatchesInputRequestTypeDef",
     {
         "filter": BuildBatchFilterTypeDef,
         "maxResults": int,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
@@ -1198,15 +1313,15 @@
 )
 
 DescribeCodeCoveragesOutputTypeDef = TypedDict(
     "DescribeCodeCoveragesOutputTypeDef",
     {
         "nextToken": str,
         "codeCoverages": List[CodeCoverageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateWebhookInputRequestTypeDef = TypedDict(
     "_RequiredCreateWebhookInputRequestTypeDef",
     {
         "projectName": str,
@@ -1259,140 +1374,25 @@
         "filterGroups": List[List[WebhookFilterTypeDef]],
         "buildType": WebhookBuildTypeType,
         "lastModifiedSecret": datetime,
     },
     total=False,
 )
 
-_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
-    {
-        "reportArn": str,
-    },
-)
-_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": ReportCodeCoverageSortByTypeType,
-        "minLineCoveragePercentage": float,
-        "maxLineCoveragePercentage": float,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef(
-    _RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
-    _OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
-):
-    pass
-
-ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef = TypedDict(
-    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
-    {
-        "projectName": str,
-        "filter": BuildBatchFilterTypeDef,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListBuildBatchesInputListBuildBatchesPaginateTypeDef = TypedDict(
-    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
-    {
-        "filter": BuildBatchFilterTypeDef,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
-    "_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
-    {
-        "projectName": str,
-    },
-)
-_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
-    "_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef(
-    _RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
-    _OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
-):
-    pass
-
-ListBuildsInputListBuildsPaginateTypeDef = TypedDict(
-    "ListBuildsInputListBuildsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListProjectsInputListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsInputListProjectsPaginateTypeDef",
-    {
-        "sortBy": ProjectSortByTypeType,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListReportGroupsInputListReportGroupsPaginateTypeDef = TypedDict(
-    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": ReportGroupSortByTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSharedProjectsInputListSharedProjectsPaginateTypeDef = TypedDict(
-    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
-    {
-        "sortBy": SharedResourceSortByTypeType,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef = TypedDict(
-    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": SharedResourceSortByTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
     "_RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
     "_OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     {
         "filter": TestCaseFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeTestCasesInputDescribeTestCasesPaginateTypeDef(
     _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     _OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
@@ -1421,15 +1421,15 @@
     pass
 
 DescribeTestCasesOutputTypeDef = TypedDict(
     "DescribeTestCasesOutputTypeDef",
     {
         "nextToken": str,
         "testCases": List[TestCaseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentLanguageTypeDef = TypedDict(
     "EnvironmentLanguageTypeDef",
     {
         "language": LanguageTypeType,
@@ -1439,30 +1439,30 @@
 )
 
 GetReportGroupTrendOutputTypeDef = TypedDict(
     "GetReportGroupTrendOutputTypeDef",
     {
         "stats": ReportGroupTrendStatsTypeDef,
         "rawData": List[ReportWithRawDataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef = TypedDict(
     "_RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     {
         "reportGroupArn": str,
     },
 )
 _OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef = TypedDict(
     "_OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef(
     _RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     _OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
@@ -1493,15 +1493,15 @@
     pass
 
 ListReportsInputListReportsPaginateTypeDef = TypedDict(
     "ListReportsInputListReportsPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListReportsInputRequestTypeDef = TypedDict(
     "ListReportsInputRequestTypeDef",
     {
@@ -1513,15 +1513,15 @@
     total=False,
 )
 
 ListSourceCredentialsOutputTypeDef = TypedDict(
     "ListSourceCredentialsOutputTypeDef",
     {
         "sourceCredentialsInfos": List[SourceCredentialsInfoTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LogsConfigTypeDef = TypedDict(
     "LogsConfigTypeDef",
     {
         "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
@@ -1616,23 +1616,23 @@
     total=False,
 )
 
 CreateWebhookOutputTypeDef = TypedDict(
     "CreateWebhookOutputTypeDef",
     {
         "webhook": WebhookTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateWebhookOutputTypeDef = TypedDict(
     "UpdateWebhookOutputTypeDef",
     {
         "webhook": WebhookTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentPlatformTypeDef = TypedDict(
     "EnvironmentPlatformTypeDef",
     {
         "platform": PlatformTypeType,
@@ -1999,135 +1999,135 @@
     total=False,
 )
 
 ListCuratedEnvironmentImagesOutputTypeDef = TypedDict(
     "ListCuratedEnvironmentImagesOutputTypeDef",
     {
         "platforms": List[EnvironmentPlatformTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetBuildsOutputTypeDef = TypedDict(
     "BatchGetBuildsOutputTypeDef",
     {
         "builds": List[BuildTypeDef],
         "buildsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RetryBuildOutputTypeDef = TypedDict(
     "RetryBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartBuildOutputTypeDef = TypedDict(
     "StartBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopBuildOutputTypeDef = TypedDict(
     "StopBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetProjectsOutputTypeDef = TypedDict(
     "BatchGetProjectsOutputTypeDef",
     {
         "projects": List[ProjectTypeDef],
         "projectsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateProjectOutputTypeDef = TypedDict(
     "CreateProjectOutputTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateProjectOutputTypeDef = TypedDict(
     "UpdateProjectOutputTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetReportGroupsOutputTypeDef = TypedDict(
     "BatchGetReportGroupsOutputTypeDef",
     {
         "reportGroups": List[ReportGroupTypeDef],
         "reportGroupsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateReportGroupOutputTypeDef = TypedDict(
     "CreateReportGroupOutputTypeDef",
     {
         "reportGroup": ReportGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateReportGroupOutputTypeDef = TypedDict(
     "UpdateReportGroupOutputTypeDef",
     {
         "reportGroup": ReportGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetReportsOutputTypeDef = TypedDict(
     "BatchGetReportsOutputTypeDef",
     {
         "reports": List[ReportTypeDef],
         "reportsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetBuildBatchesOutputTypeDef = TypedDict(
     "BatchGetBuildBatchesOutputTypeDef",
     {
         "buildBatches": List[BuildBatchTypeDef],
         "buildBatchesNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RetryBuildBatchOutputTypeDef = TypedDict(
     "RetryBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartBuildBatchOutputTypeDef = TypedDict(
     "StartBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopBuildBatchOutputTypeDef = TypedDict(
     "StopBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild.egg-info/PKG-INFO` & `mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codebuild
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodeBuild 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeBuild 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/
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
 
 <a id="mypy-boto3-codebuild"></a>
 
 # mypy-boto3-codebuild
 
 [![PyPI - mypy-boto3-codebuild](https://img.shields.io/pypi/v/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codebuild?color=blue)](https://pypistats.org/packages/mypy-boto3-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeBuild 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[boto3.CodeBuild 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [mypy-boto3-codebuild docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/).
 
 See how it helps to find and fix potential bugs:
 
@@ -406,15 +407,14 @@
 `mypy_boto3_codebuild.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codebuild.type_defs import (
     BatchDeleteBuildsInputRequestTypeDef,
     BuildNotDeletedTypeDef,
-    ResponseMetadataTypeDef,
     BatchGetBuildBatchesInputRequestTypeDef,
     BatchGetBuildsInputRequestTypeDef,
     BatchGetProjectsInputRequestTypeDef,
     BatchGetReportGroupsInputRequestTypeDef,
     BatchGetReportsInputRequestTypeDef,
     BatchRestrictionsTypeDef,
     BuildArtifactsTypeDef,
@@ -437,84 +437,85 @@
     WebhookFilterTypeDef,
     DeleteBuildBatchInputRequestTypeDef,
     DeleteProjectInputRequestTypeDef,
     DeleteReportGroupInputRequestTypeDef,
     DeleteReportInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteSourceCredentialsInputRequestTypeDef,
+    DeleteSourceCredentialsOutputTypeDef,
     DeleteWebhookInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
     DescribeCodeCoveragesInputRequestTypeDef,
     TestCaseFilterTypeDef,
     TestCaseTypeDef,
     EnvironmentImageTypeDef,
     EnvironmentVariableTypeDef,
     GetReportGroupTrendInputRequestTypeDef,
     ReportGroupTrendStatsTypeDef,
     ReportWithRawDataTypeDef,
     GetResourcePolicyInputRequestTypeDef,
+    GetResourcePolicyOutputTypeDef,
     GitSubmodulesConfigTypeDef,
     ImportSourceCredentialsInputRequestTypeDef,
+    ImportSourceCredentialsOutputTypeDef,
     InvalidateProjectCacheInputRequestTypeDef,
+    ListBuildBatchesForProjectOutputTypeDef,
+    ListBuildBatchesOutputTypeDef,
+    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
     ListBuildsForProjectInputRequestTypeDef,
+    ListBuildsForProjectOutputTypeDef,
+    ListBuildsInputListBuildsPaginateTypeDef,
     ListBuildsInputRequestTypeDef,
+    ListBuildsOutputTypeDef,
+    ListProjectsInputListProjectsPaginateTypeDef,
     ListProjectsInputRequestTypeDef,
+    ListProjectsOutputTypeDef,
+    ListReportGroupsInputListReportGroupsPaginateTypeDef,
     ListReportGroupsInputRequestTypeDef,
+    ListReportGroupsOutputTypeDef,
     ReportFilterTypeDef,
+    ListReportsForReportGroupOutputTypeDef,
+    ListReportsOutputTypeDef,
+    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
     ListSharedProjectsInputRequestTypeDef,
+    ListSharedProjectsOutputTypeDef,
+    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     ListSharedReportGroupsInputRequestTypeDef,
+    ListSharedReportGroupsOutputTypeDef,
     SourceCredentialsInfoTypeDef,
     S3LogsConfigTypeDef,
+    PaginatorConfigTypeDef,
     ProjectBadgeTypeDef,
     RegistryCredentialTypeDef,
     SourceAuthTypeDef,
     PutResourcePolicyInputRequestTypeDef,
+    PutResourcePolicyOutputTypeDef,
     S3ReportExportConfigTypeDef,
     TestReportSummaryTypeDef,
+    ResponseMetadataTypeDef,
     RetryBuildBatchInputRequestTypeDef,
     RetryBuildInputRequestTypeDef,
     StopBuildBatchInputRequestTypeDef,
     StopBuildInputRequestTypeDef,
     UpdateProjectVisibilityInputRequestTypeDef,
+    UpdateProjectVisibilityOutputTypeDef,
     BatchDeleteBuildsOutputTypeDef,
     DeleteBuildBatchOutputTypeDef,
-    DeleteSourceCredentialsOutputTypeDef,
-    GetResourcePolicyOutputTypeDef,
-    ImportSourceCredentialsOutputTypeDef,
-    ListBuildBatchesForProjectOutputTypeDef,
-    ListBuildBatchesOutputTypeDef,
-    ListBuildsForProjectOutputTypeDef,
-    ListBuildsOutputTypeDef,
-    ListProjectsOutputTypeDef,
-    ListReportGroupsOutputTypeDef,
-    ListReportsForReportGroupOutputTypeDef,
-    ListReportsOutputTypeDef,
-    ListSharedProjectsOutputTypeDef,
-    ListSharedReportGroupsOutputTypeDef,
-    PutResourcePolicyOutputTypeDef,
-    UpdateProjectVisibilityOutputTypeDef,
     ProjectBuildBatchConfigTypeDef,
+    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
     ListBuildBatchesForProjectInputRequestTypeDef,
+    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
     ListBuildBatchesInputRequestTypeDef,
     BuildBatchPhaseTypeDef,
     BuildPhaseTypeDef,
     BuildSummaryTypeDef,
     DescribeCodeCoveragesOutputTypeDef,
     CreateWebhookInputRequestTypeDef,
     UpdateWebhookInputRequestTypeDef,
     WebhookTypeDef,
-    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
-    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
-    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
-    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
-    ListBuildsInputListBuildsPaginateTypeDef,
-    ListProjectsInputListProjectsPaginateTypeDef,
-    ListReportGroupsInputListReportGroupsPaginateTypeDef,
-    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
-    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     DescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     DescribeTestCasesInputRequestTypeDef,
     DescribeTestCasesOutputTypeDef,
     EnvironmentLanguageTypeDef,
     GetReportGroupTrendOutputTypeDef,
     ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     ListReportsForReportGroupInputRequestTypeDef,
@@ -567,42 +568,42 @@
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

### Comparing `mypy-boto3-codebuild-1.26.0.post1/mypy_boto3_codebuild.egg-info/SOURCES.txt` & `mypy-boto3-codebuild-1.27.0/mypy_boto3_codebuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.26.0.post1/setup.py` & `mypy-boto3-codebuild-1.27.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-codebuild.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codebuild",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_codebuild"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeBuild 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.CodeBuild 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 codebuild type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_codebuild": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_codebuild": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/",
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


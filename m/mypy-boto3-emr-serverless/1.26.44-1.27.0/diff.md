# Comparing `tmp/mypy-boto3-emr-serverless-1.26.44.tar.gz` & `tmp/mypy-boto3-emr-serverless-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-serverless-1.26.44.tar", last modified: Thu Jan  5 20:26:50 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-serverless-1.27.0.tar", last modified: Mon Jul  3 19:50:45 2023, max compression
```

## Comparing `mypy-boto3-emr-serverless-1.26.44.tar` & `mypy-boto3-emr-serverless-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:50.939952 mypy-boto3-emr-serverless-1.26.44/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-01-05 20:26:50.935952 mypy-boto3-emr-serverless-1.26.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:50.931952 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14120 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-01-05 20:26:25.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19515 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:50.935952 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-01-05 20:26:50.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-05 20:26:50.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 20:26:50.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 20:26:50.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-05 20:26:50.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-05 20:26:50.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 20:26:50.939952 mypy-boto3-emr-serverless-1.26.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.527234 mypy-boto3-emr-serverless-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:32.000000 mypy-boto3-emr-serverless-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-07-03 19:50:45.527234 mypy-boto3-emr-serverless-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-07-03 19:37:32.000000 mypy-boto3-emr-serverless-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.519234 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-03 19:37:32.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-03 19:37:32.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:37:32.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14177 2023-07-03 19:37:32.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-07-03 19:37:32.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-07-03 19:37:33.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-07-03 19:37:33.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-03 19:37:33.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-03 19:37:32.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:32.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19961 2023-07-03 19:37:33.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-07-03 19:37:33.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:32.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.527234 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-07-03 19:50:45.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 19:50:45.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:45.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:45.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:45.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:50:45.000000 mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:45.527234 mypy-boto3-emr-serverless-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-03 19:37:32.000000 mypy-boto3-emr-serverless-1.27.0/setup.py
```

### Comparing `mypy-boto3-emr-serverless-1.26.44/LICENSE` & `mypy-boto3-emr-serverless-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-emr-serverless-1.26.44/PKG-INFO` & `mypy-boto3-emr-serverless-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.26.44
-Summary: Type annotations for boto3.EMRServerless 1.26.44 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.EMRServerless 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-emr-serverless"></a>
 
 # mypy-boto3-emr-serverless
 
 [![PyPI - mypy-boto3-emr-serverless](https://img.shields.io/pypi/v/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.26.44](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,49 +332,50 @@
     ApplicationSummaryTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     ImageConfigurationTypeDef,
     MaximumAllowedResourcesTypeDef,
     NetworkConfigurationTypeDef,
     CancelJobRunRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJobRunResponseTypeDef,
     ConfigurationTypeDef,
     ImageConfigurationInputTypeDef,
+    CreateApplicationResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
+    GetDashboardForJobRunResponseTypeDef,
     GetJobRunRequestRequestTypeDef,
     HiveTypeDef,
     WorkerResourceConfigTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
+    ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
     S3MonitoringConfigurationTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
+    StartJobRunResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    WorkerTypeSpecificationTypeDef,
-    CancelJobRunResponseTypeDef,
-    CreateApplicationResponseTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartJobRunResponseTypeDef,
+    WorkerTypeSpecificationTypeDef,
     WorkerTypeSpecificationInputTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     ConfigurationOverridesTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
@@ -391,42 +392,42 @@
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

### Comparing `mypy-boto3-emr-serverless-1.26.44/README.md` & `mypy-boto3-emr-serverless-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-emr-serverless"></a>
 
 # mypy-boto3-emr-serverless
 
 [![PyPI - mypy-boto3-emr-serverless](https://img.shields.io/pypi/v/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.26.44](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,49 +300,50 @@
     ApplicationSummaryTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     ImageConfigurationTypeDef,
     MaximumAllowedResourcesTypeDef,
     NetworkConfigurationTypeDef,
     CancelJobRunRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJobRunResponseTypeDef,
     ConfigurationTypeDef,
     ImageConfigurationInputTypeDef,
+    CreateApplicationResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
+    GetDashboardForJobRunResponseTypeDef,
     GetJobRunRequestRequestTypeDef,
     HiveTypeDef,
     WorkerResourceConfigTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
+    ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
     S3MonitoringConfigurationTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
+    StartJobRunResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    WorkerTypeSpecificationTypeDef,
-    CancelJobRunResponseTypeDef,
-    CreateApplicationResponseTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartJobRunResponseTypeDef,
+    WorkerTypeSpecificationTypeDef,
     WorkerTypeSpecificationInputTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     ConfigurationOverridesTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
@@ -359,42 +360,42 @@
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

### Comparing `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/__init__.py` & `mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/__init__.pyi` & `mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/__main__.py` & `mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRServerless 1.26.44\nVersion:         1.26.44\nBuilder"
-        " version: 7.12.2\nDocs:           "
+        "Type annotations for boto3.EMRServerless 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.44")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/client.py` & `mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,16 @@
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
-        workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
+        workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
+        releaseLabel: str = ...
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#update_application)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/client.pyi` & `mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,16 @@
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
-        workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
+        workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
+        releaseLabel: str = ...
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#update_application)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/literals.py` & `mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
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
@@ -82,31 +83,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -185,14 +189,15 @@
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
@@ -203,18 +208,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -245,14 +252,15 @@
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
@@ -271,16 +279,19 @@
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
@@ -360,18 +371,21 @@
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
@@ -391,24 +405,26 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_applications", "list_job_runs"]
 RegionName = Literal[
+    "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/literals.pyi` & `mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,15 @@
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
@@ -80,31 +81,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -183,14 +187,15 @@
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
@@ -201,18 +206,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -243,14 +250,15 @@
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
@@ -269,16 +277,19 @@
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
@@ -358,18 +369,21 @@
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
@@ -389,24 +403,26 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_applications", "list_job_runs"]
 RegionName = Literal[
+    "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/paginator.py` & `mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         states: Sequence[ApplicationStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
         """
 
 
@@ -73,13 +73,13 @@
     def paginate(
         self,
         *,
         applicationId: str,
         createdAtAfter: Union[datetime, str] = ...,
         createdAtBefore: Union[datetime, str] = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/paginator.pyi` & `mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         states: Sequence[ApplicationStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
         """
 
 class ListJobRunsPaginator(Paginator):
@@ -69,13 +69,13 @@
     def paginate(
         self,
         *,
         applicationId: str,
         createdAtAfter: Union[datetime, str] = ...,
         createdAtBefore: Union[datetime, str] = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/type_defs.py` & `mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,49 +27,50 @@
     "ApplicationSummaryTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
     "ImageConfigurationTypeDef",
     "MaximumAllowedResourcesTypeDef",
     "NetworkConfigurationTypeDef",
     "CancelJobRunRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelJobRunResponseTypeDef",
     "ConfigurationTypeDef",
     "ImageConfigurationInputTypeDef",
+    "CreateApplicationResponseTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
+    "GetDashboardForJobRunResponseTypeDef",
     "GetJobRunRequestRequestTypeDef",
     "HiveTypeDef",
     "WorkerResourceConfigTypeDef",
     "SparkSubmitTypeDef",
     "JobRunSummaryTypeDef",
+    "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     "S3MonitoringConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
+    "StartJobRunResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "WorkerTypeSpecificationTypeDef",
-    "CancelJobRunResponseTypeDef",
-    "CreateApplicationResponseTypeDef",
-    "GetDashboardForJobRunResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartJobRunResponseTypeDef",
+    "WorkerTypeSpecificationTypeDef",
     "WorkerTypeSpecificationInputTypeDef",
     "InitialCapacityConfigTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "ConfigurationOverridesTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
@@ -180,22 +181,20 @@
     "CancelJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelJobRunResponseTypeDef = TypedDict(
+    "CancelJobRunResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "applicationId": str,
+        "jobRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
@@ -219,14 +218,24 @@
     "ImageConfigurationInputTypeDef",
     {
         "imageUri": str,
     },
     total=False,
 )
 
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "applicationId": str,
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -241,14 +250,22 @@
     "GetDashboardForJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
+GetDashboardForJobRunResponseTypeDef = TypedDict(
+    "GetDashboardForJobRunResponseTypeDef",
+    {
+        "url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetJobRunRequestRequestTypeDef = TypedDict(
     "GetJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
@@ -340,44 +357,78 @@
 )
 
 
 class JobRunSummaryTypeDef(_RequiredJobRunSummaryTypeDef, _OptionalJobRunSummaryTypeDef):
     pass
 
 
+ResourceUtilizationTypeDef = TypedDict(
+    "ResourceUtilizationTypeDef",
+    {
+        "vCPUHour": float,
+        "memoryGBHour": float,
+        "storageGBHour": float,
+    },
+    total=False,
+)
+
 TotalResourceUtilizationTypeDef = TypedDict(
     "TotalResourceUtilizationTypeDef",
     {
         "vCPUHour": float,
         "memoryGBHour": float,
         "storageGBHour": float,
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
+        "states": Sequence[ApplicationStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "states": Sequence[ApplicationStateType],
     },
     total=False,
 )
 
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "createdAtAfter": Union[datetime, str],
+        "createdAtBefore": Union[datetime, str],
+        "states": Sequence[JobRunStateType],
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
         "applicationId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -402,14 +453,22 @@
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
 ManagedPersistenceMonitoringConfigurationTypeDef = TypedDict(
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     {
         "enabled": bool,
         "encryptionKeyArn": str,
     },
     total=False,
@@ -420,21 +479,52 @@
     {
         "logUri": str,
         "encryptionKeyArn": str,
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
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
+    {
+        "applicationId": str,
+        "jobRunId": str,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopApplicationRequestRequestTypeDef = TypedDict(
     "StopApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -450,74 +540,29 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-WorkerTypeSpecificationTypeDef = TypedDict(
-    "WorkerTypeSpecificationTypeDef",
-    {
-        "imageConfiguration": ImageConfigurationTypeDef,
-    },
-    total=False,
-)
-
-CancelJobRunResponseTypeDef = TypedDict(
-    "CancelJobRunResponseTypeDef",
-    {
-        "applicationId": str,
-        "jobRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "applicationId": str,
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDashboardForJobRunResponseTypeDef = TypedDict(
-    "GetDashboardForJobRunResponseTypeDef",
-    {
-        "url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
+WorkerTypeSpecificationTypeDef = TypedDict(
+    "WorkerTypeSpecificationTypeDef",
     {
-        "applicationId": str,
-        "jobRunId": str,
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "imageConfiguration": ImageConfigurationTypeDef,
     },
+    total=False,
 )
 
 WorkerTypeSpecificationInputTypeDef = TypedDict(
     "WorkerTypeSpecificationInputTypeDef",
     {
         "imageConfiguration": ImageConfigurationInputTypeDef,
     },
@@ -555,57 +600,25 @@
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "jobRuns": List[JobRunSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "states": Sequence[ApplicationStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
-        "states": Sequence[JobRunStateType],
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
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
-        "managedPersistenceMonitoringConfiguration": ManagedPersistenceMonitoringConfigurationTypeDef,
+        "managedPersistenceMonitoringConfiguration": (
+            ManagedPersistenceMonitoringConfigurationTypeDef
+        ),
     },
     total=False,
 )
 
 _RequiredApplicationTypeDef = TypedDict(
     "_RequiredApplicationTypeDef",
     {
@@ -687,14 +700,15 @@
         "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "autoStartConfiguration": AutoStartConfigTypeDef,
         "autoStopConfiguration": AutoStopConfigTypeDef,
         "networkConfiguration": NetworkConfigurationTypeDef,
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationInputTypeDef,
         "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
+        "releaseLabel": str,
     },
     total=False,
 )
 
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
@@ -711,23 +725,23 @@
     total=False,
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
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
 
 _RequiredJobRunTypeDef = TypedDict(
     "_RequiredJobRunTypeDef",
     {
         "applicationId": str,
@@ -748,14 +762,16 @@
     {
         "name": str,
         "configurationOverrides": ConfigurationOverridesTypeDef,
         "tags": Dict[str, str],
         "totalResourceUtilization": TotalResourceUtilizationTypeDef,
         "networkConfiguration": NetworkConfigurationTypeDef,
         "totalExecutionDurationSeconds": int,
+        "executionTimeoutMinutes": int,
+        "billedResourceUtilization": ResourceUtilizationTypeDef,
     },
     total=False,
 )
 
 
 class JobRunTypeDef(_RequiredJobRunTypeDef, _OptionalJobRunTypeDef):
     pass
@@ -788,10 +804,10 @@
     pass
 
 
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "jobRun": JobRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/type_defs.pyi` & `mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -26,49 +26,50 @@
     "ApplicationSummaryTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
     "ImageConfigurationTypeDef",
     "MaximumAllowedResourcesTypeDef",
     "NetworkConfigurationTypeDef",
     "CancelJobRunRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelJobRunResponseTypeDef",
     "ConfigurationTypeDef",
     "ImageConfigurationInputTypeDef",
+    "CreateApplicationResponseTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
+    "GetDashboardForJobRunResponseTypeDef",
     "GetJobRunRequestRequestTypeDef",
     "HiveTypeDef",
     "WorkerResourceConfigTypeDef",
     "SparkSubmitTypeDef",
     "JobRunSummaryTypeDef",
+    "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     "S3MonitoringConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
+    "StartJobRunResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "WorkerTypeSpecificationTypeDef",
-    "CancelJobRunResponseTypeDef",
-    "CreateApplicationResponseTypeDef",
-    "GetDashboardForJobRunResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartJobRunResponseTypeDef",
+    "WorkerTypeSpecificationTypeDef",
     "WorkerTypeSpecificationInputTypeDef",
     "InitialCapacityConfigTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "ConfigurationOverridesTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
@@ -173,22 +174,20 @@
     "CancelJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelJobRunResponseTypeDef = TypedDict(
+    "CancelJobRunResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "applicationId": str,
+        "jobRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
@@ -210,14 +209,24 @@
     "ImageConfigurationInputTypeDef",
     {
         "imageUri": str,
     },
     total=False,
 )
 
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "applicationId": str,
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -232,14 +241,22 @@
     "GetDashboardForJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
+GetDashboardForJobRunResponseTypeDef = TypedDict(
+    "GetDashboardForJobRunResponseTypeDef",
+    {
+        "url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetJobRunRequestRequestTypeDef = TypedDict(
     "GetJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
@@ -323,44 +340,76 @@
     },
     total=False,
 )
 
 class JobRunSummaryTypeDef(_RequiredJobRunSummaryTypeDef, _OptionalJobRunSummaryTypeDef):
     pass
 
+ResourceUtilizationTypeDef = TypedDict(
+    "ResourceUtilizationTypeDef",
+    {
+        "vCPUHour": float,
+        "memoryGBHour": float,
+        "storageGBHour": float,
+    },
+    total=False,
+)
+
 TotalResourceUtilizationTypeDef = TypedDict(
     "TotalResourceUtilizationTypeDef",
     {
         "vCPUHour": float,
         "memoryGBHour": float,
         "storageGBHour": float,
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
+        "states": Sequence[ApplicationStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "states": Sequence[ApplicationStateType],
     },
     total=False,
 )
 
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "createdAtAfter": Union[datetime, str],
+        "createdAtBefore": Union[datetime, str],
+        "states": Sequence[JobRunStateType],
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
         "applicationId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -383,14 +432,22 @@
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
 ManagedPersistenceMonitoringConfigurationTypeDef = TypedDict(
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     {
         "enabled": bool,
         "encryptionKeyArn": str,
     },
     total=False,
@@ -401,21 +458,52 @@
     {
         "logUri": str,
         "encryptionKeyArn": str,
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
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
+    {
+        "applicationId": str,
+        "jobRunId": str,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopApplicationRequestRequestTypeDef = TypedDict(
     "StopApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -431,74 +519,29 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-WorkerTypeSpecificationTypeDef = TypedDict(
-    "WorkerTypeSpecificationTypeDef",
-    {
-        "imageConfiguration": ImageConfigurationTypeDef,
-    },
-    total=False,
-)
-
-CancelJobRunResponseTypeDef = TypedDict(
-    "CancelJobRunResponseTypeDef",
-    {
-        "applicationId": str,
-        "jobRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "applicationId": str,
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDashboardForJobRunResponseTypeDef = TypedDict(
-    "GetDashboardForJobRunResponseTypeDef",
-    {
-        "url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
+WorkerTypeSpecificationTypeDef = TypedDict(
+    "WorkerTypeSpecificationTypeDef",
     {
-        "applicationId": str,
-        "jobRunId": str,
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "imageConfiguration": ImageConfigurationTypeDef,
     },
+    total=False,
 )
 
 WorkerTypeSpecificationInputTypeDef = TypedDict(
     "WorkerTypeSpecificationInputTypeDef",
     {
         "imageConfiguration": ImageConfigurationInputTypeDef,
     },
@@ -534,55 +577,25 @@
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "jobRuns": List[JobRunSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "states": Sequence[ApplicationStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
-        "states": Sequence[JobRunStateType],
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
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
-        "managedPersistenceMonitoringConfiguration": ManagedPersistenceMonitoringConfigurationTypeDef,
+        "managedPersistenceMonitoringConfiguration": (
+            ManagedPersistenceMonitoringConfigurationTypeDef
+        ),
     },
     total=False,
 )
 
 _RequiredApplicationTypeDef = TypedDict(
     "_RequiredApplicationTypeDef",
     {
@@ -660,14 +673,15 @@
         "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "autoStartConfiguration": AutoStartConfigTypeDef,
         "autoStopConfiguration": AutoStopConfigTypeDef,
         "networkConfiguration": NetworkConfigurationTypeDef,
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationInputTypeDef,
         "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
+        "releaseLabel": str,
     },
     total=False,
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
@@ -682,23 +696,23 @@
     total=False,
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
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
 
 _RequiredJobRunTypeDef = TypedDict(
     "_RequiredJobRunTypeDef",
     {
         "applicationId": str,
@@ -719,14 +733,16 @@
     {
         "name": str,
         "configurationOverrides": ConfigurationOverridesTypeDef,
         "tags": Dict[str, str],
         "totalResourceUtilization": TotalResourceUtilizationTypeDef,
         "networkConfiguration": NetworkConfigurationTypeDef,
         "totalExecutionDurationSeconds": int,
+        "executionTimeoutMinutes": int,
+        "billedResourceUtilization": ResourceUtilizationTypeDef,
     },
     total=False,
 )
 
 class JobRunTypeDef(_RequiredJobRunTypeDef, _OptionalJobRunTypeDef):
     pass
 
@@ -755,10 +771,10 @@
 ):
     pass
 
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "jobRun": JobRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/PKG-INFO` & `mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.26.44
-Summary: Type annotations for boto3.EMRServerless 1.26.44 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.EMRServerless 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-emr-serverless"></a>
 
 # mypy-boto3-emr-serverless
 
 [![PyPI - mypy-boto3-emr-serverless](https://img.shields.io/pypi/v/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.26.44](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,49 +332,50 @@
     ApplicationSummaryTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     ImageConfigurationTypeDef,
     MaximumAllowedResourcesTypeDef,
     NetworkConfigurationTypeDef,
     CancelJobRunRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJobRunResponseTypeDef,
     ConfigurationTypeDef,
     ImageConfigurationInputTypeDef,
+    CreateApplicationResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
+    GetDashboardForJobRunResponseTypeDef,
     GetJobRunRequestRequestTypeDef,
     HiveTypeDef,
     WorkerResourceConfigTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
+    ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
-    PaginatorConfigTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
     S3MonitoringConfigurationTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
+    StartJobRunResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    WorkerTypeSpecificationTypeDef,
-    CancelJobRunResponseTypeDef,
-    CreateApplicationResponseTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartJobRunResponseTypeDef,
+    WorkerTypeSpecificationTypeDef,
     WorkerTypeSpecificationInputTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     ConfigurationOverridesTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
@@ -391,42 +392,42 @@
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

### Comparing `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/SOURCES.txt` & `mypy-boto3-emr-serverless-1.27.0/mypy_boto3_emr_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.26.44/setup.py` & `mypy-boto3-emr-serverless-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-emr-serverless.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr-serverless",
-    version="1.26.44",
+    version="1.27.0",
     packages=["mypy_boto3_emr_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMRServerless 1.26.44 service generated with mypy-boto3-builder"
-        " 7.12.2"
+        "Type annotations for boto3.EMRServerless 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/",
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


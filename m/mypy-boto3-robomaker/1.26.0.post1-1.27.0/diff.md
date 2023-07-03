# Comparing `tmp/mypy-boto3-robomaker-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-robomaker-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-robomaker-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:54 2022, max compression
+gzip compressed data, was "mypy-boto3-robomaker-1.27.0.tar", last modified: Mon Jul  3 19:51:20 2023, max compression
```

## Comparing `mypy-boto3-robomaker-1.26.0.post1.tar` & `mypy-boto3-robomaker-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:54.828845 mypy-boto3-robomaker-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:40:05.000000 mypy-boto3-robomaker-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    21727 2022-11-01 21:43:54.828845 mypy-boto3-robomaker-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    20278 2022-11-01 21:40:05.000000 mypy-boto3-robomaker-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:54.820845 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2022-11-01 21:40:05.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2797 2022-11-01 21:40:05.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-11-01 21:40:05.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    42165 2022-11-01 21:40:05.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    42090 2022-11-01 21:40:05.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13136 2022-11-01 21:40:06.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    13134 2022-11-01 21:40:05.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13390 2022-11-01 21:40:05.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    13377 2022-11-01 21:40:05.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:40:05.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    63499 2022-11-01 21:40:09.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    63444 2022-11-01 21:40:08.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:40:05.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:54.828845 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    21727 2022-11-01 21:43:54.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-11-01 21:43:54.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:54.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:54.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:54.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-01 21:43:54.000000 mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:54.828845 mypy-boto3-robomaker-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-11-01 21:40:05.000000 mypy-boto3-robomaker-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:20.419889 mypy-boto3-robomaker-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:23.000000 mypy-boto3-robomaker-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21751 2023-07-03 19:51:20.419889 mypy-boto3-robomaker-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20258 2023-07-03 19:46:23.000000 mypy-boto3-robomaker-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:20.419889 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-03 19:46:23.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-03 19:46:23.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:46:23.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42233 2023-07-03 19:46:23.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42158 2023-07-03 19:46:23.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-03 19:46:24.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-07-03 19:46:23.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-07-03 19:46:23.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13399 2023-07-03 19:46:23.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:23.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63609 2023-07-03 19:46:25.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63554 2023-07-03 19:46:24.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:23.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:20.419889 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21751 2023-07-03 19:51:20.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 19:51:20.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:20.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:20.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:20.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:51:20.000000 mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:20.419889 mypy-boto3-robomaker-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:46:23.000000 mypy-boto3-robomaker-1.27.0/setup.py
```

### Comparing `mypy-boto3-robomaker-1.26.0.post1/LICENSE` & `mypy-boto3-robomaker-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-robomaker-1.26.0.post1/PKG-INFO` & `mypy-boto3-robomaker-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-robomaker
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.RoboMaker 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.RoboMaker 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/
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
 
 <a id="mypy-boto3-robomaker"></a>
 
 # mypy-boto3-robomaker
 
 [![PyPI - mypy-boto3-robomaker](https://img.shields.io/pypi/v/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-robomaker?color=blue)](https://pypistats.org/packages/mypy-boto3-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RoboMaker 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[boto3.RoboMaker 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [mypy-boto3-robomaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -388,95 +389,96 @@
 
 `mypy_boto3_robomaker.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_robomaker.type_defs import (
     BatchDeleteWorldsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    BatchDeleteWorldsResponseTypeDef,
     BatchDescribeSimulationJobRequestRequestTypeDef,
     BatchPolicyTypeDef,
     CancelDeploymentJobRequestRequestTypeDef,
     CancelSimulationJobBatchRequestRequestTypeDef,
     CancelSimulationJobRequestRequestTypeDef,
     CancelWorldExportJobRequestRequestTypeDef,
     CancelWorldGenerationJobRequestRequestTypeDef,
     ComputeResponseTypeDef,
     ComputeTypeDef,
     CreateFleetRequestRequestTypeDef,
+    CreateFleetResponseTypeDef,
     EnvironmentTypeDef,
     RobotSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
+    CreateRobotResponseTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
     DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
     TemplateLocationTypeDef,
+    CreateWorldTemplateResponseTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
     DeploymentLaunchConfigTypeDef,
     S3ObjectTypeDef,
     DeregisterRobotRequestRequestTypeDef,
+    DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobRequestRequestTypeDef,
     DescribeFleetRequestRequestTypeDef,
     RobotTypeDef,
     DescribeRobotApplicationRequestRequestTypeDef,
     DescribeRobotRequestRequestTypeDef,
+    DescribeRobotResponseTypeDef,
     DescribeSimulationApplicationRequestRequestTypeDef,
     DescribeSimulationJobBatchRequestRequestTypeDef,
     SimulationJobSummaryTypeDef,
     DescribeSimulationJobRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     DescribeWorldExportJobRequestRequestTypeDef,
     DescribeWorldGenerationJobRequestRequestTypeDef,
     DescribeWorldRequestRequestTypeDef,
+    DescribeWorldResponseTypeDef,
     DescribeWorldTemplateRequestRequestTypeDef,
+    DescribeWorldTemplateResponseTypeDef,
     WorldFailureTypeDef,
     FilterTypeDef,
     FleetTypeDef,
     GetWorldTemplateBodyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetWorldTemplateBodyResponseTypeDef,
     SimulationJobBatchSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
     ListWorldTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     WorldSummaryTypeDef,
+    PaginatorConfigTypeDef,
     PortMappingTypeDef,
     ProgressDetailTypeDef,
     RegisterRobotRequestRequestTypeDef,
+    RegisterRobotResponseTypeDef,
+    ResponseMetadataTypeDef,
     RestartSimulationJobRequestRequestTypeDef,
     ToolTypeDef,
     UploadConfigurationTypeDef,
     WorldConfigTypeDef,
     SyncDeploymentJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    BatchDeleteWorldsResponseTypeDef,
-    CreateFleetResponseTypeDef,
-    CreateRobotResponseTypeDef,
-    CreateWorldTemplateResponseTypeDef,
-    DeregisterRobotResponseTypeDef,
-    DescribeRobotResponseTypeDef,
-    DescribeWorldResponseTypeDef,
-    DescribeWorldTemplateResponseTypeDef,
-    GetWorldTemplateBodyResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RegisterRobotResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
     RobotApplicationSummaryTypeDef,
     CreateRobotApplicationRequestRequestTypeDef,
     UpdateRobotApplicationRequestRequestTypeDef,
     CreateRobotApplicationResponseTypeDef,
     CreateRobotApplicationVersionResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
@@ -500,36 +502,35 @@
     DataSourceTypeDef,
     DeploymentApplicationConfigTypeDef,
     DeploymentConfigTypeDef,
     DescribeFleetResponseTypeDef,
     ListRobotsResponseTypeDef,
     ListSimulationJobsResponseTypeDef,
     FailureSummaryTypeDef,
+    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
     ListDeploymentJobsRequestRequestTypeDef,
+    ListFleetsRequestListFleetsPaginateTypeDef,
     ListFleetsRequestRequestTypeDef,
+    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
     ListRobotApplicationsRequestRequestTypeDef,
+    ListRobotsRequestListRobotsPaginateTypeDef,
     ListRobotsRequestRequestTypeDef,
+    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
     ListSimulationApplicationsRequestRequestTypeDef,
+    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
     ListSimulationJobBatchesRequestRequestTypeDef,
+    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
     ListSimulationJobsRequestRequestTypeDef,
+    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
     ListWorldExportJobsRequestRequestTypeDef,
+    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
     ListWorldGenerationJobsRequestRequestTypeDef,
+    ListWorldsRequestListWorldsPaginateTypeDef,
     ListWorldsRequestRequestTypeDef,
     ListFleetsResponseTypeDef,
-    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
-    ListFleetsRequestListFleetsPaginateTypeDef,
-    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
-    ListRobotsRequestListRobotsPaginateTypeDef,
-    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
-    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
-    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
-    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
-    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
-    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
-    ListWorldsRequestListWorldsPaginateTypeDef,
     ListSimulationJobBatchesResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     ListWorldsResponseTypeDef,
     PortForwardingConfigTypeDef,
     RobotDeploymentTypeDef,
     ListRobotApplicationsResponseTypeDef,
     ListSimulationApplicationsResponseTypeDef,
@@ -566,42 +567,42 @@
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

### Comparing `mypy-boto3-robomaker-1.26.0.post1/README.md` & `mypy-boto3-robomaker-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-robomaker"></a>
 
 # mypy-boto3-robomaker
 
 [![PyPI - mypy-boto3-robomaker](https://img.shields.io/pypi/v/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-robomaker?color=blue)](https://pypistats.org/packages/mypy-boto3-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RoboMaker 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[boto3.RoboMaker 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [mypy-boto3-robomaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,95 +357,96 @@
 
 `mypy_boto3_robomaker.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_robomaker.type_defs import (
     BatchDeleteWorldsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    BatchDeleteWorldsResponseTypeDef,
     BatchDescribeSimulationJobRequestRequestTypeDef,
     BatchPolicyTypeDef,
     CancelDeploymentJobRequestRequestTypeDef,
     CancelSimulationJobBatchRequestRequestTypeDef,
     CancelSimulationJobRequestRequestTypeDef,
     CancelWorldExportJobRequestRequestTypeDef,
     CancelWorldGenerationJobRequestRequestTypeDef,
     ComputeResponseTypeDef,
     ComputeTypeDef,
     CreateFleetRequestRequestTypeDef,
+    CreateFleetResponseTypeDef,
     EnvironmentTypeDef,
     RobotSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
+    CreateRobotResponseTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
     DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
     TemplateLocationTypeDef,
+    CreateWorldTemplateResponseTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
     DeploymentLaunchConfigTypeDef,
     S3ObjectTypeDef,
     DeregisterRobotRequestRequestTypeDef,
+    DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobRequestRequestTypeDef,
     DescribeFleetRequestRequestTypeDef,
     RobotTypeDef,
     DescribeRobotApplicationRequestRequestTypeDef,
     DescribeRobotRequestRequestTypeDef,
+    DescribeRobotResponseTypeDef,
     DescribeSimulationApplicationRequestRequestTypeDef,
     DescribeSimulationJobBatchRequestRequestTypeDef,
     SimulationJobSummaryTypeDef,
     DescribeSimulationJobRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     DescribeWorldExportJobRequestRequestTypeDef,
     DescribeWorldGenerationJobRequestRequestTypeDef,
     DescribeWorldRequestRequestTypeDef,
+    DescribeWorldResponseTypeDef,
     DescribeWorldTemplateRequestRequestTypeDef,
+    DescribeWorldTemplateResponseTypeDef,
     WorldFailureTypeDef,
     FilterTypeDef,
     FleetTypeDef,
     GetWorldTemplateBodyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetWorldTemplateBodyResponseTypeDef,
     SimulationJobBatchSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
     ListWorldTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     WorldSummaryTypeDef,
+    PaginatorConfigTypeDef,
     PortMappingTypeDef,
     ProgressDetailTypeDef,
     RegisterRobotRequestRequestTypeDef,
+    RegisterRobotResponseTypeDef,
+    ResponseMetadataTypeDef,
     RestartSimulationJobRequestRequestTypeDef,
     ToolTypeDef,
     UploadConfigurationTypeDef,
     WorldConfigTypeDef,
     SyncDeploymentJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    BatchDeleteWorldsResponseTypeDef,
-    CreateFleetResponseTypeDef,
-    CreateRobotResponseTypeDef,
-    CreateWorldTemplateResponseTypeDef,
-    DeregisterRobotResponseTypeDef,
-    DescribeRobotResponseTypeDef,
-    DescribeWorldResponseTypeDef,
-    DescribeWorldTemplateResponseTypeDef,
-    GetWorldTemplateBodyResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RegisterRobotResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
     RobotApplicationSummaryTypeDef,
     CreateRobotApplicationRequestRequestTypeDef,
     UpdateRobotApplicationRequestRequestTypeDef,
     CreateRobotApplicationResponseTypeDef,
     CreateRobotApplicationVersionResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
@@ -469,36 +470,35 @@
     DataSourceTypeDef,
     DeploymentApplicationConfigTypeDef,
     DeploymentConfigTypeDef,
     DescribeFleetResponseTypeDef,
     ListRobotsResponseTypeDef,
     ListSimulationJobsResponseTypeDef,
     FailureSummaryTypeDef,
+    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
     ListDeploymentJobsRequestRequestTypeDef,
+    ListFleetsRequestListFleetsPaginateTypeDef,
     ListFleetsRequestRequestTypeDef,
+    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
     ListRobotApplicationsRequestRequestTypeDef,
+    ListRobotsRequestListRobotsPaginateTypeDef,
     ListRobotsRequestRequestTypeDef,
+    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
     ListSimulationApplicationsRequestRequestTypeDef,
+    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
     ListSimulationJobBatchesRequestRequestTypeDef,
+    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
     ListSimulationJobsRequestRequestTypeDef,
+    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
     ListWorldExportJobsRequestRequestTypeDef,
+    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
     ListWorldGenerationJobsRequestRequestTypeDef,
+    ListWorldsRequestListWorldsPaginateTypeDef,
     ListWorldsRequestRequestTypeDef,
     ListFleetsResponseTypeDef,
-    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
-    ListFleetsRequestListFleetsPaginateTypeDef,
-    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
-    ListRobotsRequestListRobotsPaginateTypeDef,
-    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
-    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
-    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
-    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
-    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
-    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
-    ListWorldsRequestListWorldsPaginateTypeDef,
     ListSimulationJobBatchesResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     ListWorldsResponseTypeDef,
     PortForwardingConfigTypeDef,
     RobotDeploymentTypeDef,
     ListRobotApplicationsResponseTypeDef,
     ListSimulationApplicationsResponseTypeDef,
@@ -535,42 +535,42 @@
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

### Comparing `mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/__init__.py` & `mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/__init__.pyi` & `mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/__main__.py` & `mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RoboMaker 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.RoboMaker 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker\nOther"
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

### Comparing `mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/client.py` & `mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -742,15 +742,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/client/#tag_resource)
         """
 
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        .
+        Removes the specified tags from the specified AWS RoboMaker resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/client/#untag_resource)
         """
 
     def update_robot_application(
         self,
```

### Comparing `mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/client.pyi` & `mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -681,15 +681,15 @@
         Adds or edits tags for a AWS RoboMaker resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/client/#tag_resource)
         """
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        .
+        Removes the specified tags from the specified AWS RoboMaker resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/client/#untag_resource)
         """
     def update_robot_application(
         self,
         *,
```

### Comparing `mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/literals.py` & `mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,23 +214,25 @@
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
@@ -240,30 +242,35 @@
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
@@ -289,14 +296,15 @@
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
@@ -341,51 +349,57 @@
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
@@ -398,14 +412,15 @@
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
@@ -417,28 +432,35 @@
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
@@ -447,14 +469,15 @@
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
@@ -465,55 +488,64 @@
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

### Comparing `mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/literals.pyi` & `mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -212,23 +212,25 @@
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
@@ -238,30 +240,35 @@
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
@@ -287,14 +294,15 @@
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
@@ -339,51 +347,57 @@
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
@@ -396,14 +410,15 @@
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
@@ -415,28 +430,35 @@
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
@@ -445,14 +467,15 @@
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
@@ -463,55 +486,64 @@
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

### Comparing `mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/paginator.py` & `mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listdeploymentjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListDeploymentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listdeploymentjobspaginator)
         """
 
 
@@ -108,15 +108,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listfleetspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listfleetspaginator)
         """
 
 
@@ -127,15 +127,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRobotApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobotApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listrobotapplicationspaginator)
         """
 
 
@@ -145,15 +145,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listrobotspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRobotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listrobotspaginator)
         """
 
 
@@ -164,15 +164,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSimulationApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationapplicationspaginator)
         """
 
 
@@ -182,15 +182,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobbatchespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSimulationJobBatchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobBatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobbatchespaginator)
         """
 
 
@@ -200,15 +200,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSimulationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobspaginator)
         """
 
 
@@ -218,15 +218,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorldExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldexportjobspaginator)
         """
 
 
@@ -236,30 +236,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldgenerationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorldGenerationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldGenerationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldgenerationjobspaginator)
         """
 
 
 class ListWorldTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorldTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldtemplatespaginator)
         """
 
 
@@ -269,13 +269,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorldsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorlds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldspaginator)
         """
```

### Comparing `mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/paginator.pyi` & `mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listdeploymentjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListDeploymentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listdeploymentjobspaginator)
         """
 
 class ListFleetsPaginator(Paginator):
@@ -104,15 +104,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listfleetspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listfleetspaginator)
         """
 
 class ListRobotApplicationsPaginator(Paginator):
@@ -122,15 +122,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRobotApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobotApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listrobotapplicationspaginator)
         """
 
 class ListRobotsPaginator(Paginator):
@@ -139,15 +139,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listrobotspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRobotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listrobotspaginator)
         """
 
 class ListSimulationApplicationsPaginator(Paginator):
@@ -157,15 +157,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSimulationApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationapplicationspaginator)
         """
 
 class ListSimulationJobBatchesPaginator(Paginator):
@@ -174,15 +174,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobbatchespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSimulationJobBatchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobBatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobbatchespaginator)
         """
 
 class ListSimulationJobsPaginator(Paginator):
@@ -191,15 +191,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSimulationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobspaginator)
         """
 
 class ListWorldExportJobsPaginator(Paginator):
@@ -208,15 +208,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorldExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldexportjobspaginator)
         """
 
 class ListWorldGenerationJobsPaginator(Paginator):
@@ -225,29 +225,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldgenerationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorldGenerationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldGenerationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldgenerationjobspaginator)
         """
 
 class ListWorldTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorldTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldtemplatespaginator)
         """
 
 class ListWorldsPaginator(Paginator):
@@ -256,13 +256,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListWorldsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorlds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldspaginator)
         """
```

### Comparing `mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/type_defs.py` & `mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,95 +46,96 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BatchDeleteWorldsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "BatchDeleteWorldsResponseTypeDef",
     "BatchDescribeSimulationJobRequestRequestTypeDef",
     "BatchPolicyTypeDef",
     "CancelDeploymentJobRequestRequestTypeDef",
     "CancelSimulationJobBatchRequestRequestTypeDef",
     "CancelSimulationJobRequestRequestTypeDef",
     "CancelWorldExportJobRequestRequestTypeDef",
     "CancelWorldGenerationJobRequestRequestTypeDef",
     "ComputeResponseTypeDef",
     "ComputeTypeDef",
     "CreateFleetRequestRequestTypeDef",
+    "CreateFleetResponseTypeDef",
     "EnvironmentTypeDef",
     "RobotSoftwareSuiteTypeDef",
     "SourceConfigTypeDef",
     "SourceTypeDef",
     "CreateRobotApplicationVersionRequestRequestTypeDef",
     "CreateRobotRequestRequestTypeDef",
+    "CreateRobotResponseTypeDef",
     "RenderingEngineTypeDef",
     "SimulationSoftwareSuiteTypeDef",
     "CreateSimulationApplicationVersionRequestRequestTypeDef",
     "DataSourceConfigTypeDef",
     "LoggingConfigTypeDef",
     "OutputLocationTypeDef",
     "VPCConfigTypeDef",
     "VPCConfigResponseTypeDef",
     "WorldCountTypeDef",
     "TemplateLocationTypeDef",
+    "CreateWorldTemplateResponseTypeDef",
     "S3KeyOutputTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteRobotApplicationRequestRequestTypeDef",
     "DeleteRobotRequestRequestTypeDef",
     "DeleteSimulationApplicationRequestRequestTypeDef",
     "DeleteWorldTemplateRequestRequestTypeDef",
     "DeploymentLaunchConfigTypeDef",
     "S3ObjectTypeDef",
     "DeregisterRobotRequestRequestTypeDef",
+    "DeregisterRobotResponseTypeDef",
     "DescribeDeploymentJobRequestRequestTypeDef",
     "DescribeFleetRequestRequestTypeDef",
     "RobotTypeDef",
     "DescribeRobotApplicationRequestRequestTypeDef",
     "DescribeRobotRequestRequestTypeDef",
+    "DescribeRobotResponseTypeDef",
     "DescribeSimulationApplicationRequestRequestTypeDef",
     "DescribeSimulationJobBatchRequestRequestTypeDef",
     "SimulationJobSummaryTypeDef",
     "DescribeSimulationJobRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeWorldExportJobRequestRequestTypeDef",
     "DescribeWorldGenerationJobRequestRequestTypeDef",
     "DescribeWorldRequestRequestTypeDef",
+    "DescribeWorldResponseTypeDef",
     "DescribeWorldTemplateRequestRequestTypeDef",
+    "DescribeWorldTemplateResponseTypeDef",
     "WorldFailureTypeDef",
     "FilterTypeDef",
     "FleetTypeDef",
     "GetWorldTemplateBodyRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetWorldTemplateBodyResponseTypeDef",
     "SimulationJobBatchSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
     "ListWorldTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "WorldSummaryTypeDef",
+    "PaginatorConfigTypeDef",
     "PortMappingTypeDef",
     "ProgressDetailTypeDef",
     "RegisterRobotRequestRequestTypeDef",
+    "RegisterRobotResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "RestartSimulationJobRequestRequestTypeDef",
     "ToolTypeDef",
     "UploadConfigurationTypeDef",
     "WorldConfigTypeDef",
     "SyncDeploymentJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "BatchDeleteWorldsResponseTypeDef",
-    "CreateFleetResponseTypeDef",
-    "CreateRobotResponseTypeDef",
-    "CreateWorldTemplateResponseTypeDef",
-    "DeregisterRobotResponseTypeDef",
-    "DescribeRobotResponseTypeDef",
-    "DescribeWorldResponseTypeDef",
-    "DescribeWorldTemplateResponseTypeDef",
-    "GetWorldTemplateBodyResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RegisterRobotResponseTypeDef",
     "UpdateWorldTemplateResponseTypeDef",
     "RobotApplicationSummaryTypeDef",
     "CreateRobotApplicationRequestRequestTypeDef",
     "UpdateRobotApplicationRequestRequestTypeDef",
     "CreateRobotApplicationResponseTypeDef",
     "CreateRobotApplicationVersionResponseTypeDef",
     "DescribeRobotApplicationResponseTypeDef",
@@ -158,36 +159,35 @@
     "DataSourceTypeDef",
     "DeploymentApplicationConfigTypeDef",
     "DeploymentConfigTypeDef",
     "DescribeFleetResponseTypeDef",
     "ListRobotsResponseTypeDef",
     "ListSimulationJobsResponseTypeDef",
     "FailureSummaryTypeDef",
+    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
     "ListDeploymentJobsRequestRequestTypeDef",
+    "ListFleetsRequestListFleetsPaginateTypeDef",
     "ListFleetsRequestRequestTypeDef",
+    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
     "ListRobotApplicationsRequestRequestTypeDef",
+    "ListRobotsRequestListRobotsPaginateTypeDef",
     "ListRobotsRequestRequestTypeDef",
+    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
     "ListSimulationApplicationsRequestRequestTypeDef",
+    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
     "ListSimulationJobBatchesRequestRequestTypeDef",
+    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
     "ListSimulationJobsRequestRequestTypeDef",
+    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
     "ListWorldExportJobsRequestRequestTypeDef",
+    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
     "ListWorldGenerationJobsRequestRequestTypeDef",
+    "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListWorldsRequestRequestTypeDef",
     "ListFleetsResponseTypeDef",
-    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
-    "ListFleetsRequestListFleetsPaginateTypeDef",
-    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
-    "ListRobotsRequestListRobotsPaginateTypeDef",
-    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
-    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
-    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
-    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
-    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
-    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
-    "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListSimulationJobBatchesResponseTypeDef",
     "ListWorldTemplatesResponseTypeDef",
     "ListWorldsResponseTypeDef",
     "PortForwardingConfigTypeDef",
     "RobotDeploymentTypeDef",
     "ListRobotApplicationsResponseTypeDef",
     "ListSimulationApplicationsResponseTypeDef",
@@ -219,22 +219,19 @@
 BatchDeleteWorldsRequestRequestTypeDef = TypedDict(
     "BatchDeleteWorldsRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+BatchDeleteWorldsResponseTypeDef = TypedDict(
+    "BatchDeleteWorldsResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "unprocessedWorlds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDescribeSimulationJobRequestRequestTypeDef = TypedDict(
     "BatchDescribeSimulationJobRequestRequestTypeDef",
     {
         "jobs": Sequence[str],
@@ -322,14 +319,25 @@
 
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
 
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "createdAt": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "uri": str,
     },
     total=False,
 )
@@ -407,14 +415,27 @@
 
 class CreateRobotRequestRequestTypeDef(
     _RequiredCreateRobotRequestRequestTypeDef, _OptionalCreateRobotRequestRequestTypeDef
 ):
     pass
 
 
+CreateRobotResponseTypeDef = TypedDict(
+    "CreateRobotResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "createdAt": datetime,
+        "greengrassGroupId": str,
+        "architecture": ArchitectureType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RenderingEngineTypeDef = TypedDict(
     "RenderingEngineTypeDef",
     {
         "name": Literal["OGRE"],
         "version": str,
     },
     total=False,
@@ -536,14 +557,26 @@
     "TemplateLocationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
 
+CreateWorldTemplateResponseTypeDef = TypedDict(
+    "CreateWorldTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "clientRequestToken": str,
+        "createdAt": datetime,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 S3KeyOutputTypeDef = TypedDict(
     "S3KeyOutputTypeDef",
     {
         "s3Key": str,
         "etag": str,
     },
     total=False,
@@ -662,14 +695,23 @@
     "DeregisterRobotRequestRequestTypeDef",
     {
         "fleet": str,
         "robot": str,
     },
 )
 
+DeregisterRobotResponseTypeDef = TypedDict(
+    "DeregisterRobotResponseTypeDef",
+    {
+        "fleet": str,
+        "robot": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDeploymentJobRequestRequestTypeDef = TypedDict(
     "DescribeDeploymentJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
@@ -721,14 +763,31 @@
 DescribeRobotRequestRequestTypeDef = TypedDict(
     "DescribeRobotRequestRequestTypeDef",
     {
         "robot": str,
     },
 )
 
+DescribeRobotResponseTypeDef = TypedDict(
+    "DescribeRobotResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "fleetArn": str,
+        "status": RobotStatusType,
+        "greengrassGroupId": str,
+        "createdAt": datetime,
+        "architecture": ArchitectureType,
+        "lastDeploymentJob": str,
+        "lastDeploymentTime": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeSimulationApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSimulationApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalDescribeSimulationApplicationRequestRequestTypeDef = TypedDict(
@@ -803,21 +862,48 @@
 DescribeWorldRequestRequestTypeDef = TypedDict(
     "DescribeWorldRequestRequestTypeDef",
     {
         "world": str,
     },
 )
 
+DescribeWorldResponseTypeDef = TypedDict(
+    "DescribeWorldResponseTypeDef",
+    {
+        "arn": str,
+        "generationJob": str,
+        "template": str,
+        "createdAt": datetime,
+        "tags": Dict[str, str],
+        "worldDescriptionBody": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeWorldTemplateRequestRequestTypeDef = TypedDict(
     "DescribeWorldTemplateRequestRequestTypeDef",
     {
         "template": str,
     },
 )
 
+DescribeWorldTemplateResponseTypeDef = TypedDict(
+    "DescribeWorldTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "clientRequestToken": str,
+        "name": str,
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "tags": Dict[str, str],
+        "version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WorldFailureTypeDef = TypedDict(
     "WorldFailureTypeDef",
     {
         "failureCode": WorldGenerationJobErrorCodeType,
         "sampleFailureReason": str,
         "failureCount": int,
     },
@@ -851,22 +937,20 @@
     {
         "template": str,
         "generationJob": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetWorldTemplateBodyResponseTypeDef = TypedDict(
+    "GetWorldTemplateBodyResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "templateBody": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 SimulationJobBatchSummaryTypeDef = TypedDict(
     "SimulationJobBatchSummaryTypeDef",
     {
         "arn": str,
         "lastUpdatedAt": datetime,
@@ -882,14 +966,30 @@
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
+ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef = TypedDict(
+    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListWorldTemplatesRequestRequestTypeDef = TypedDict(
     "ListWorldTemplatesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -914,14 +1014,24 @@
         "createdAt": datetime,
         "generationJob": str,
         "template": str,
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
 _RequiredPortMappingTypeDef = TypedDict(
     "_RequiredPortMappingTypeDef",
     {
         "jobPort": int,
         "applicationPort": int,
     },
 )
@@ -953,14 +1063,34 @@
     "RegisterRobotRequestRequestTypeDef",
     {
         "fleet": str,
         "robot": str,
     },
 )
 
+RegisterRobotResponseTypeDef = TypedDict(
+    "RegisterRobotResponseTypeDef",
+    {
+        "fleet": str,
+        "robot": str,
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
 RestartSimulationJobRequestRequestTypeDef = TypedDict(
     "RestartSimulationJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
@@ -1023,144 +1153,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-BatchDeleteWorldsResponseTypeDef = TypedDict(
-    "BatchDeleteWorldsResponseTypeDef",
-    {
-        "unprocessedWorlds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "createdAt": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRobotResponseTypeDef = TypedDict(
-    "CreateRobotResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "createdAt": datetime,
-        "greengrassGroupId": str,
-        "architecture": ArchitectureType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorldTemplateResponseTypeDef = TypedDict(
-    "CreateWorldTemplateResponseTypeDef",
-    {
-        "arn": str,
-        "clientRequestToken": str,
-        "createdAt": datetime,
-        "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeregisterRobotResponseTypeDef = TypedDict(
-    "DeregisterRobotResponseTypeDef",
-    {
-        "fleet": str,
-        "robot": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRobotResponseTypeDef = TypedDict(
-    "DescribeRobotResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "fleetArn": str,
-        "status": RobotStatusType,
-        "greengrassGroupId": str,
-        "createdAt": datetime,
-        "architecture": ArchitectureType,
-        "lastDeploymentJob": str,
-        "lastDeploymentTime": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeWorldResponseTypeDef = TypedDict(
-    "DescribeWorldResponseTypeDef",
-    {
-        "arn": str,
-        "generationJob": str,
-        "template": str,
-        "createdAt": datetime,
-        "tags": Dict[str, str],
-        "worldDescriptionBody": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeWorldTemplateResponseTypeDef = TypedDict(
-    "DescribeWorldTemplateResponseTypeDef",
-    {
-        "arn": str,
-        "clientRequestToken": str,
-        "name": str,
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "tags": Dict[str, str],
-        "version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetWorldTemplateBodyResponseTypeDef = TypedDict(
-    "GetWorldTemplateBodyResponseTypeDef",
-    {
-        "templateBody": str,
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
-RegisterRobotResponseTypeDef = TypedDict(
-    "RegisterRobotResponseTypeDef",
-    {
-        "fleet": str,
-        "robot": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateWorldTemplateResponseTypeDef = TypedDict(
     "UpdateWorldTemplateResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RobotApplicationSummaryTypeDef = TypedDict(
     "RobotApplicationSummaryTypeDef",
     {
         "name": str,
@@ -1230,30 +1238,30 @@
         "version": str,
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRobotApplicationVersionResponseTypeDef = TypedDict(
     "CreateRobotApplicationVersionResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRobotApplicationResponseTypeDef = TypedDict(
     "DescribeRobotApplicationResponseTypeDef",
     {
         "arn": str,
@@ -1262,30 +1270,30 @@
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
         "imageDigest": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRobotApplicationResponseTypeDef = TypedDict(
     "UpdateRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSimulationApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSimulationApplicationRequestRequestTypeDef",
     {
         "name": str,
@@ -1322,15 +1330,15 @@
         "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSimulationApplicationVersionResponseTypeDef = TypedDict(
     "CreateSimulationApplicationVersionResponseTypeDef",
     {
         "arn": str,
@@ -1339,15 +1347,15 @@
         "sources": List[SourceTypeDef],
         "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSimulationApplicationResponseTypeDef = TypedDict(
     "DescribeSimulationApplicationResponseTypeDef",
     {
         "arn": str,
@@ -1358,15 +1366,15 @@
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
         "imageDigest": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SimulationApplicationSummaryTypeDef = TypedDict(
     "SimulationApplicationSummaryTypeDef",
     {
         "name": str,
@@ -1415,15 +1423,15 @@
         "sources": List[SourceTypeDef],
         "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateWorldExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorldExportJobRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
@@ -1455,15 +1463,15 @@
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldExportJobErrorCodeType,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorldExportJobResponseTypeDef = TypedDict(
     "DescribeWorldExportJobResponseTypeDef",
     {
         "arn": str,
@@ -1472,15 +1480,15 @@
         "failureCode": WorldExportJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
         "worlds": List[str],
         "outputLocation": OutputLocationTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorldExportJobSummaryTypeDef = TypedDict(
     "WorldExportJobSummaryTypeDef",
     {
         "arn": str,
@@ -1525,15 +1533,15 @@
         "createdAt": datetime,
         "failureCode": WorldGenerationJobErrorCodeType,
         "clientRequestToken": str,
         "template": str,
         "worldCount": WorldCountTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorldGenerationJobSummaryTypeDef = TypedDict(
     "WorldGenerationJobSummaryTypeDef",
     {
         "arn": str,
@@ -1622,280 +1630,272 @@
         "arn": str,
         "robots": List[RobotTypeDef],
         "createdAt": datetime,
         "lastDeploymentStatus": DeploymentStatusType,
         "lastDeploymentJob": str,
         "lastDeploymentTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRobotsResponseTypeDef = TypedDict(
     "ListRobotsResponseTypeDef",
     {
         "robots": List[RobotTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSimulationJobsResponseTypeDef = TypedDict(
     "ListSimulationJobsResponseTypeDef",
     {
         "simulationJobSummaries": List[SimulationJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FailureSummaryTypeDef = TypedDict(
     "FailureSummaryTypeDef",
     {
         "totalFailureCount": int,
         "failures": List[WorldFailureTypeDef],
     },
     total=False,
 )
 
-ListDeploymentJobsRequestRequestTypeDef = TypedDict(
-    "ListDeploymentJobsRequestRequestTypeDef",
+ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef = TypedDict(
+    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListFleetsRequestRequestTypeDef = TypedDict(
-    "ListFleetsRequestRequestTypeDef",
+ListDeploymentJobsRequestRequestTypeDef = TypedDict(
+    "ListDeploymentJobsRequestRequestTypeDef",
     {
+        "filters": Sequence[FilterTypeDef],
         "nextToken": str,
         "maxResults": int,
-        "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListRobotApplicationsRequestRequestTypeDef = TypedDict(
-    "ListRobotApplicationsRequestRequestTypeDef",
+ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
+    "ListFleetsRequestListFleetsPaginateTypeDef",
     {
-        "versionQualifier": str,
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListRobotsRequestRequestTypeDef = TypedDict(
-    "ListRobotsRequestRequestTypeDef",
+ListFleetsRequestRequestTypeDef = TypedDict(
+    "ListFleetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListSimulationApplicationsRequestRequestTypeDef = TypedDict(
-    "ListSimulationApplicationsRequestRequestTypeDef",
+ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef = TypedDict(
+    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
     {
         "versionQualifier": str,
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListSimulationJobBatchesRequestRequestTypeDef = TypedDict(
-    "ListSimulationJobBatchesRequestRequestTypeDef",
+ListRobotApplicationsRequestRequestTypeDef = TypedDict(
+    "ListRobotApplicationsRequestRequestTypeDef",
     {
+        "versionQualifier": str,
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListSimulationJobsRequestRequestTypeDef = TypedDict(
-    "ListSimulationJobsRequestRequestTypeDef",
+ListRobotsRequestListRobotsPaginateTypeDef = TypedDict(
+    "ListRobotsRequestListRobotsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListWorldExportJobsRequestRequestTypeDef = TypedDict(
-    "ListWorldExportJobsRequestRequestTypeDef",
+ListRobotsRequestRequestTypeDef = TypedDict(
+    "ListRobotsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListWorldGenerationJobsRequestRequestTypeDef = TypedDict(
-    "ListWorldGenerationJobsRequestRequestTypeDef",
+ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef = TypedDict(
+    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "versionQualifier": str,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListWorldsRequestRequestTypeDef = TypedDict(
-    "ListWorldsRequestRequestTypeDef",
+ListSimulationApplicationsRequestRequestTypeDef = TypedDict(
+    "ListSimulationApplicationsRequestRequestTypeDef",
     {
+        "versionQualifier": str,
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListFleetsResponseTypeDef = TypedDict(
-    "ListFleetsResponseTypeDef",
-    {
-        "fleetDetails": List[FleetTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef = TypedDict(
-    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
+ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef = TypedDict(
+    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
-    "ListFleetsRequestListFleetsPaginateTypeDef",
+ListSimulationJobBatchesRequestRequestTypeDef = TypedDict(
+    "ListSimulationJobBatchesRequestRequestTypeDef",
     {
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef = TypedDict(
-    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
+ListSimulationJobsRequestListSimulationJobsPaginateTypeDef = TypedDict(
+    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
     {
-        "versionQualifier": str,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListRobotsRequestListRobotsPaginateTypeDef = TypedDict(
-    "ListRobotsRequestListRobotsPaginateTypeDef",
+ListSimulationJobsRequestRequestTypeDef = TypedDict(
+    "ListSimulationJobsRequestRequestTypeDef",
     {
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef = TypedDict(
-    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
+ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef = TypedDict(
+    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
     {
-        "versionQualifier": str,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef = TypedDict(
-    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
+ListWorldExportJobsRequestRequestTypeDef = TypedDict(
+    "ListWorldExportJobsRequestRequestTypeDef",
     {
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationJobsRequestListSimulationJobsPaginateTypeDef = TypedDict(
-    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
+ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef = TypedDict(
+    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef = TypedDict(
-    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
+ListWorldGenerationJobsRequestRequestTypeDef = TypedDict(
+    "ListWorldGenerationJobsRequestRequestTypeDef",
     {
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef = TypedDict(
-    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
+ListWorldsRequestListWorldsPaginateTypeDef = TypedDict(
+    "ListWorldsRequestListWorldsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef = TypedDict(
-    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
+ListWorldsRequestRequestTypeDef = TypedDict(
+    "ListWorldsRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "nextToken": str,
+        "maxResults": int,
+        "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListWorldsRequestListWorldsPaginateTypeDef = TypedDict(
-    "ListWorldsRequestListWorldsPaginateTypeDef",
+ListFleetsResponseTypeDef = TypedDict(
+    "ListFleetsResponseTypeDef",
     {
-        "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "fleetDetails": List[FleetTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ListSimulationJobBatchesResponseTypeDef = TypedDict(
     "ListSimulationJobBatchesResponseTypeDef",
     {
         "simulationJobBatchSummaries": List[SimulationJobBatchSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorldTemplatesResponseTypeDef = TypedDict(
     "ListWorldTemplatesResponseTypeDef",
     {
         "templateSummaries": List[TemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorldsResponseTypeDef = TypedDict(
     "ListWorldsResponseTypeDef",
     {
         "worldSummaries": List[WorldSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PortForwardingConfigTypeDef = TypedDict(
     "PortForwardingConfigTypeDef",
     {
         "portMappings": List[PortMappingTypeDef],
@@ -1918,42 +1918,42 @@
 )
 
 ListRobotApplicationsResponseTypeDef = TypedDict(
     "ListRobotApplicationsResponseTypeDef",
     {
         "robotApplicationSummaries": List[RobotApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSimulationApplicationsResponseTypeDef = TypedDict(
     "ListSimulationApplicationsResponseTypeDef",
     {
         "simulationApplicationSummaries": List[SimulationApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorldExportJobsResponseTypeDef = TypedDict(
     "ListWorldExportJobsResponseTypeDef",
     {
         "worldExportJobSummaries": List[WorldExportJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorldGenerationJobsResponseTypeDef = TypedDict(
     "ListWorldGenerationJobsResponseTypeDef",
     {
         "worldGenerationJobSummaries": List[WorldGenerationJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
@@ -1986,15 +1986,15 @@
         "status": DeploymentStatusType,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "deploymentConfig": DeploymentConfigTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentJobTypeDef = TypedDict(
     "DeploymentJobTypeDef",
     {
         "arn": str,
@@ -2016,15 +2016,15 @@
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentConfig": DeploymentConfigTypeDef,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FinishedWorldsSummaryTypeDef = TypedDict(
     "FinishedWorldsSummaryTypeDef",
     {
         "finishedCount": int,
@@ -2056,24 +2056,24 @@
         "deploymentConfig": DeploymentConfigTypeDef,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "robotDeploymentSummary": List[RobotDeploymentTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeploymentJobsResponseTypeDef = TypedDict(
     "ListDeploymentJobsResponseTypeDef",
     {
         "deploymentJobs": List[DeploymentJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorldGenerationJobResponseTypeDef = TypedDict(
     "DescribeWorldGenerationJobResponseTypeDef",
     {
         "arn": str,
@@ -2083,15 +2083,15 @@
         "failureReason": str,
         "clientRequestToken": str,
         "template": str,
         "worldCount": WorldCountTypeDef,
         "finishedWorldsSummary": FinishedWorldsSummaryTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRobotApplicationConfigTypeDef = TypedDict(
     "_RequiredRobotApplicationConfigTypeDef",
     {
         "application": str,
@@ -2193,15 +2193,15 @@
         "iamRole": str,
         "robotApplications": List[RobotApplicationConfigTypeDef],
         "simulationApplications": List[SimulationApplicationConfigTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "compute": ComputeResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSimulationJobResponseTypeDef = TypedDict(
     "DescribeSimulationJobResponseTypeDef",
     {
         "arn": str,
@@ -2221,15 +2221,15 @@
         "robotApplications": List[RobotApplicationConfigTypeDef],
         "simulationApplications": List[SimulationApplicationConfigTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSimulationJobRequestTypeDef = TypedDict(
     "_RequiredSimulationJobRequestTypeDef",
     {
         "maxJobDurationInSeconds": int,
@@ -2324,15 +2324,15 @@
 
 
 BatchDescribeSimulationJobResponseTypeDef = TypedDict(
     "BatchDescribeSimulationJobResponseTypeDef",
     {
         "jobs": List[SimulationJobTypeDef],
         "unprocessedJobs": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSimulationJobBatchResponseTypeDef = TypedDict(
     "DescribeSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
@@ -2343,15 +2343,15 @@
         "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
         "pendingRequests": List[SimulationJobRequestTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartSimulationJobBatchResponseTypeDef = TypedDict(
     "StartSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
@@ -2361,10 +2361,10 @@
         "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
         "pendingRequests": List[SimulationJobRequestTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker/type_defs.pyi` & `mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -45,95 +45,96 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BatchDeleteWorldsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "BatchDeleteWorldsResponseTypeDef",
     "BatchDescribeSimulationJobRequestRequestTypeDef",
     "BatchPolicyTypeDef",
     "CancelDeploymentJobRequestRequestTypeDef",
     "CancelSimulationJobBatchRequestRequestTypeDef",
     "CancelSimulationJobRequestRequestTypeDef",
     "CancelWorldExportJobRequestRequestTypeDef",
     "CancelWorldGenerationJobRequestRequestTypeDef",
     "ComputeResponseTypeDef",
     "ComputeTypeDef",
     "CreateFleetRequestRequestTypeDef",
+    "CreateFleetResponseTypeDef",
     "EnvironmentTypeDef",
     "RobotSoftwareSuiteTypeDef",
     "SourceConfigTypeDef",
     "SourceTypeDef",
     "CreateRobotApplicationVersionRequestRequestTypeDef",
     "CreateRobotRequestRequestTypeDef",
+    "CreateRobotResponseTypeDef",
     "RenderingEngineTypeDef",
     "SimulationSoftwareSuiteTypeDef",
     "CreateSimulationApplicationVersionRequestRequestTypeDef",
     "DataSourceConfigTypeDef",
     "LoggingConfigTypeDef",
     "OutputLocationTypeDef",
     "VPCConfigTypeDef",
     "VPCConfigResponseTypeDef",
     "WorldCountTypeDef",
     "TemplateLocationTypeDef",
+    "CreateWorldTemplateResponseTypeDef",
     "S3KeyOutputTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteRobotApplicationRequestRequestTypeDef",
     "DeleteRobotRequestRequestTypeDef",
     "DeleteSimulationApplicationRequestRequestTypeDef",
     "DeleteWorldTemplateRequestRequestTypeDef",
     "DeploymentLaunchConfigTypeDef",
     "S3ObjectTypeDef",
     "DeregisterRobotRequestRequestTypeDef",
+    "DeregisterRobotResponseTypeDef",
     "DescribeDeploymentJobRequestRequestTypeDef",
     "DescribeFleetRequestRequestTypeDef",
     "RobotTypeDef",
     "DescribeRobotApplicationRequestRequestTypeDef",
     "DescribeRobotRequestRequestTypeDef",
+    "DescribeRobotResponseTypeDef",
     "DescribeSimulationApplicationRequestRequestTypeDef",
     "DescribeSimulationJobBatchRequestRequestTypeDef",
     "SimulationJobSummaryTypeDef",
     "DescribeSimulationJobRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeWorldExportJobRequestRequestTypeDef",
     "DescribeWorldGenerationJobRequestRequestTypeDef",
     "DescribeWorldRequestRequestTypeDef",
+    "DescribeWorldResponseTypeDef",
     "DescribeWorldTemplateRequestRequestTypeDef",
+    "DescribeWorldTemplateResponseTypeDef",
     "WorldFailureTypeDef",
     "FilterTypeDef",
     "FleetTypeDef",
     "GetWorldTemplateBodyRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetWorldTemplateBodyResponseTypeDef",
     "SimulationJobBatchSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
     "ListWorldTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "WorldSummaryTypeDef",
+    "PaginatorConfigTypeDef",
     "PortMappingTypeDef",
     "ProgressDetailTypeDef",
     "RegisterRobotRequestRequestTypeDef",
+    "RegisterRobotResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "RestartSimulationJobRequestRequestTypeDef",
     "ToolTypeDef",
     "UploadConfigurationTypeDef",
     "WorldConfigTypeDef",
     "SyncDeploymentJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "BatchDeleteWorldsResponseTypeDef",
-    "CreateFleetResponseTypeDef",
-    "CreateRobotResponseTypeDef",
-    "CreateWorldTemplateResponseTypeDef",
-    "DeregisterRobotResponseTypeDef",
-    "DescribeRobotResponseTypeDef",
-    "DescribeWorldResponseTypeDef",
-    "DescribeWorldTemplateResponseTypeDef",
-    "GetWorldTemplateBodyResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RegisterRobotResponseTypeDef",
     "UpdateWorldTemplateResponseTypeDef",
     "RobotApplicationSummaryTypeDef",
     "CreateRobotApplicationRequestRequestTypeDef",
     "UpdateRobotApplicationRequestRequestTypeDef",
     "CreateRobotApplicationResponseTypeDef",
     "CreateRobotApplicationVersionResponseTypeDef",
     "DescribeRobotApplicationResponseTypeDef",
@@ -157,36 +158,35 @@
     "DataSourceTypeDef",
     "DeploymentApplicationConfigTypeDef",
     "DeploymentConfigTypeDef",
     "DescribeFleetResponseTypeDef",
     "ListRobotsResponseTypeDef",
     "ListSimulationJobsResponseTypeDef",
     "FailureSummaryTypeDef",
+    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
     "ListDeploymentJobsRequestRequestTypeDef",
+    "ListFleetsRequestListFleetsPaginateTypeDef",
     "ListFleetsRequestRequestTypeDef",
+    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
     "ListRobotApplicationsRequestRequestTypeDef",
+    "ListRobotsRequestListRobotsPaginateTypeDef",
     "ListRobotsRequestRequestTypeDef",
+    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
     "ListSimulationApplicationsRequestRequestTypeDef",
+    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
     "ListSimulationJobBatchesRequestRequestTypeDef",
+    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
     "ListSimulationJobsRequestRequestTypeDef",
+    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
     "ListWorldExportJobsRequestRequestTypeDef",
+    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
     "ListWorldGenerationJobsRequestRequestTypeDef",
+    "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListWorldsRequestRequestTypeDef",
     "ListFleetsResponseTypeDef",
-    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
-    "ListFleetsRequestListFleetsPaginateTypeDef",
-    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
-    "ListRobotsRequestListRobotsPaginateTypeDef",
-    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
-    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
-    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
-    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
-    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
-    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
-    "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListSimulationJobBatchesResponseTypeDef",
     "ListWorldTemplatesResponseTypeDef",
     "ListWorldsResponseTypeDef",
     "PortForwardingConfigTypeDef",
     "RobotDeploymentTypeDef",
     "ListRobotApplicationsResponseTypeDef",
     "ListSimulationApplicationsResponseTypeDef",
@@ -218,22 +218,19 @@
 BatchDeleteWorldsRequestRequestTypeDef = TypedDict(
     "BatchDeleteWorldsRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+BatchDeleteWorldsResponseTypeDef = TypedDict(
+    "BatchDeleteWorldsResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "unprocessedWorlds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDescribeSimulationJobRequestRequestTypeDef = TypedDict(
     "BatchDescribeSimulationJobRequestRequestTypeDef",
     {
         "jobs": Sequence[str],
@@ -319,14 +316,25 @@
 )
 
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "createdAt": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "uri": str,
     },
     total=False,
 )
@@ -400,14 +408,27 @@
 )
 
 class CreateRobotRequestRequestTypeDef(
     _RequiredCreateRobotRequestRequestTypeDef, _OptionalCreateRobotRequestRequestTypeDef
 ):
     pass
 
+CreateRobotResponseTypeDef = TypedDict(
+    "CreateRobotResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "createdAt": datetime,
+        "greengrassGroupId": str,
+        "architecture": ArchitectureType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RenderingEngineTypeDef = TypedDict(
     "RenderingEngineTypeDef",
     {
         "name": Literal["OGRE"],
         "version": str,
     },
     total=False,
@@ -523,14 +544,26 @@
     "TemplateLocationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
 
+CreateWorldTemplateResponseTypeDef = TypedDict(
+    "CreateWorldTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "clientRequestToken": str,
+        "createdAt": datetime,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 S3KeyOutputTypeDef = TypedDict(
     "S3KeyOutputTypeDef",
     {
         "s3Key": str,
         "etag": str,
     },
     total=False,
@@ -641,14 +674,23 @@
     "DeregisterRobotRequestRequestTypeDef",
     {
         "fleet": str,
         "robot": str,
     },
 )
 
+DeregisterRobotResponseTypeDef = TypedDict(
+    "DeregisterRobotResponseTypeDef",
+    {
+        "fleet": str,
+        "robot": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDeploymentJobRequestRequestTypeDef = TypedDict(
     "DescribeDeploymentJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
@@ -698,14 +740,31 @@
 DescribeRobotRequestRequestTypeDef = TypedDict(
     "DescribeRobotRequestRequestTypeDef",
     {
         "robot": str,
     },
 )
 
+DescribeRobotResponseTypeDef = TypedDict(
+    "DescribeRobotResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "fleetArn": str,
+        "status": RobotStatusType,
+        "greengrassGroupId": str,
+        "createdAt": datetime,
+        "architecture": ArchitectureType,
+        "lastDeploymentJob": str,
+        "lastDeploymentTime": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeSimulationApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSimulationApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalDescribeSimulationApplicationRequestRequestTypeDef = TypedDict(
@@ -778,21 +837,48 @@
 DescribeWorldRequestRequestTypeDef = TypedDict(
     "DescribeWorldRequestRequestTypeDef",
     {
         "world": str,
     },
 )
 
+DescribeWorldResponseTypeDef = TypedDict(
+    "DescribeWorldResponseTypeDef",
+    {
+        "arn": str,
+        "generationJob": str,
+        "template": str,
+        "createdAt": datetime,
+        "tags": Dict[str, str],
+        "worldDescriptionBody": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeWorldTemplateRequestRequestTypeDef = TypedDict(
     "DescribeWorldTemplateRequestRequestTypeDef",
     {
         "template": str,
     },
 )
 
+DescribeWorldTemplateResponseTypeDef = TypedDict(
+    "DescribeWorldTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "clientRequestToken": str,
+        "name": str,
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "tags": Dict[str, str],
+        "version": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WorldFailureTypeDef = TypedDict(
     "WorldFailureTypeDef",
     {
         "failureCode": WorldGenerationJobErrorCodeType,
         "sampleFailureReason": str,
         "failureCount": int,
     },
@@ -826,22 +912,20 @@
     {
         "template": str,
         "generationJob": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetWorldTemplateBodyResponseTypeDef = TypedDict(
+    "GetWorldTemplateBodyResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "templateBody": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 SimulationJobBatchSummaryTypeDef = TypedDict(
     "SimulationJobBatchSummaryTypeDef",
     {
         "arn": str,
         "lastUpdatedAt": datetime,
@@ -857,14 +941,30 @@
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
+ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef = TypedDict(
+    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListWorldTemplatesRequestRequestTypeDef = TypedDict(
     "ListWorldTemplatesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -889,14 +989,24 @@
         "createdAt": datetime,
         "generationJob": str,
         "template": str,
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
 _RequiredPortMappingTypeDef = TypedDict(
     "_RequiredPortMappingTypeDef",
     {
         "jobPort": int,
         "applicationPort": int,
     },
 )
@@ -926,14 +1036,34 @@
     "RegisterRobotRequestRequestTypeDef",
     {
         "fleet": str,
         "robot": str,
     },
 )
 
+RegisterRobotResponseTypeDef = TypedDict(
+    "RegisterRobotResponseTypeDef",
+    {
+        "fleet": str,
+        "robot": str,
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
 RestartSimulationJobRequestRequestTypeDef = TypedDict(
     "RestartSimulationJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
@@ -994,144 +1124,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-BatchDeleteWorldsResponseTypeDef = TypedDict(
-    "BatchDeleteWorldsResponseTypeDef",
-    {
-        "unprocessedWorlds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "createdAt": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRobotResponseTypeDef = TypedDict(
-    "CreateRobotResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "createdAt": datetime,
-        "greengrassGroupId": str,
-        "architecture": ArchitectureType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorldTemplateResponseTypeDef = TypedDict(
-    "CreateWorldTemplateResponseTypeDef",
-    {
-        "arn": str,
-        "clientRequestToken": str,
-        "createdAt": datetime,
-        "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeregisterRobotResponseTypeDef = TypedDict(
-    "DeregisterRobotResponseTypeDef",
-    {
-        "fleet": str,
-        "robot": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRobotResponseTypeDef = TypedDict(
-    "DescribeRobotResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "fleetArn": str,
-        "status": RobotStatusType,
-        "greengrassGroupId": str,
-        "createdAt": datetime,
-        "architecture": ArchitectureType,
-        "lastDeploymentJob": str,
-        "lastDeploymentTime": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeWorldResponseTypeDef = TypedDict(
-    "DescribeWorldResponseTypeDef",
-    {
-        "arn": str,
-        "generationJob": str,
-        "template": str,
-        "createdAt": datetime,
-        "tags": Dict[str, str],
-        "worldDescriptionBody": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeWorldTemplateResponseTypeDef = TypedDict(
-    "DescribeWorldTemplateResponseTypeDef",
-    {
-        "arn": str,
-        "clientRequestToken": str,
-        "name": str,
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "tags": Dict[str, str],
-        "version": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetWorldTemplateBodyResponseTypeDef = TypedDict(
-    "GetWorldTemplateBodyResponseTypeDef",
-    {
-        "templateBody": str,
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
-RegisterRobotResponseTypeDef = TypedDict(
-    "RegisterRobotResponseTypeDef",
-    {
-        "fleet": str,
-        "robot": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateWorldTemplateResponseTypeDef = TypedDict(
     "UpdateWorldTemplateResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RobotApplicationSummaryTypeDef = TypedDict(
     "RobotApplicationSummaryTypeDef",
     {
         "name": str,
@@ -1197,30 +1205,30 @@
         "version": str,
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRobotApplicationVersionResponseTypeDef = TypedDict(
     "CreateRobotApplicationVersionResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRobotApplicationResponseTypeDef = TypedDict(
     "DescribeRobotApplicationResponseTypeDef",
     {
         "arn": str,
@@ -1229,30 +1237,30 @@
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
         "imageDigest": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateRobotApplicationResponseTypeDef = TypedDict(
     "UpdateRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateSimulationApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSimulationApplicationRequestRequestTypeDef",
     {
         "name": str,
@@ -1287,15 +1295,15 @@
         "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSimulationApplicationVersionResponseTypeDef = TypedDict(
     "CreateSimulationApplicationVersionResponseTypeDef",
     {
         "arn": str,
@@ -1304,15 +1312,15 @@
         "sources": List[SourceTypeDef],
         "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSimulationApplicationResponseTypeDef = TypedDict(
     "DescribeSimulationApplicationResponseTypeDef",
     {
         "arn": str,
@@ -1323,15 +1331,15 @@
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
         "imageDigest": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SimulationApplicationSummaryTypeDef = TypedDict(
     "SimulationApplicationSummaryTypeDef",
     {
         "name": str,
@@ -1378,15 +1386,15 @@
         "sources": List[SourceTypeDef],
         "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateWorldExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorldExportJobRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
@@ -1416,15 +1424,15 @@
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldExportJobErrorCodeType,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorldExportJobResponseTypeDef = TypedDict(
     "DescribeWorldExportJobResponseTypeDef",
     {
         "arn": str,
@@ -1433,15 +1441,15 @@
         "failureCode": WorldExportJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
         "worlds": List[str],
         "outputLocation": OutputLocationTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorldExportJobSummaryTypeDef = TypedDict(
     "WorldExportJobSummaryTypeDef",
     {
         "arn": str,
@@ -1484,15 +1492,15 @@
         "createdAt": datetime,
         "failureCode": WorldGenerationJobErrorCodeType,
         "clientRequestToken": str,
         "template": str,
         "worldCount": WorldCountTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorldGenerationJobSummaryTypeDef = TypedDict(
     "WorldGenerationJobSummaryTypeDef",
     {
         "arn": str,
@@ -1579,280 +1587,272 @@
         "arn": str,
         "robots": List[RobotTypeDef],
         "createdAt": datetime,
         "lastDeploymentStatus": DeploymentStatusType,
         "lastDeploymentJob": str,
         "lastDeploymentTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRobotsResponseTypeDef = TypedDict(
     "ListRobotsResponseTypeDef",
     {
         "robots": List[RobotTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSimulationJobsResponseTypeDef = TypedDict(
     "ListSimulationJobsResponseTypeDef",
     {
         "simulationJobSummaries": List[SimulationJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FailureSummaryTypeDef = TypedDict(
     "FailureSummaryTypeDef",
     {
         "totalFailureCount": int,
         "failures": List[WorldFailureTypeDef],
     },
     total=False,
 )
 
-ListDeploymentJobsRequestRequestTypeDef = TypedDict(
-    "ListDeploymentJobsRequestRequestTypeDef",
+ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef = TypedDict(
+    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListFleetsRequestRequestTypeDef = TypedDict(
-    "ListFleetsRequestRequestTypeDef",
+ListDeploymentJobsRequestRequestTypeDef = TypedDict(
+    "ListDeploymentJobsRequestRequestTypeDef",
     {
+        "filters": Sequence[FilterTypeDef],
         "nextToken": str,
         "maxResults": int,
-        "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListRobotApplicationsRequestRequestTypeDef = TypedDict(
-    "ListRobotApplicationsRequestRequestTypeDef",
+ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
+    "ListFleetsRequestListFleetsPaginateTypeDef",
     {
-        "versionQualifier": str,
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListRobotsRequestRequestTypeDef = TypedDict(
-    "ListRobotsRequestRequestTypeDef",
+ListFleetsRequestRequestTypeDef = TypedDict(
+    "ListFleetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListSimulationApplicationsRequestRequestTypeDef = TypedDict(
-    "ListSimulationApplicationsRequestRequestTypeDef",
+ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef = TypedDict(
+    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
     {
         "versionQualifier": str,
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListSimulationJobBatchesRequestRequestTypeDef = TypedDict(
-    "ListSimulationJobBatchesRequestRequestTypeDef",
+ListRobotApplicationsRequestRequestTypeDef = TypedDict(
+    "ListRobotApplicationsRequestRequestTypeDef",
     {
+        "versionQualifier": str,
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListSimulationJobsRequestRequestTypeDef = TypedDict(
-    "ListSimulationJobsRequestRequestTypeDef",
+ListRobotsRequestListRobotsPaginateTypeDef = TypedDict(
+    "ListRobotsRequestListRobotsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListWorldExportJobsRequestRequestTypeDef = TypedDict(
-    "ListWorldExportJobsRequestRequestTypeDef",
+ListRobotsRequestRequestTypeDef = TypedDict(
+    "ListRobotsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListWorldGenerationJobsRequestRequestTypeDef = TypedDict(
-    "ListWorldGenerationJobsRequestRequestTypeDef",
+ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef = TypedDict(
+    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "versionQualifier": str,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListWorldsRequestRequestTypeDef = TypedDict(
-    "ListWorldsRequestRequestTypeDef",
+ListSimulationApplicationsRequestRequestTypeDef = TypedDict(
+    "ListSimulationApplicationsRequestRequestTypeDef",
     {
+        "versionQualifier": str,
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListFleetsResponseTypeDef = TypedDict(
-    "ListFleetsResponseTypeDef",
-    {
-        "fleetDetails": List[FleetTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef = TypedDict(
-    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
+ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef = TypedDict(
+    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
-    "ListFleetsRequestListFleetsPaginateTypeDef",
+ListSimulationJobBatchesRequestRequestTypeDef = TypedDict(
+    "ListSimulationJobBatchesRequestRequestTypeDef",
     {
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef = TypedDict(
-    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
+ListSimulationJobsRequestListSimulationJobsPaginateTypeDef = TypedDict(
+    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
     {
-        "versionQualifier": str,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListRobotsRequestListRobotsPaginateTypeDef = TypedDict(
-    "ListRobotsRequestListRobotsPaginateTypeDef",
+ListSimulationJobsRequestRequestTypeDef = TypedDict(
+    "ListSimulationJobsRequestRequestTypeDef",
     {
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef = TypedDict(
-    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
+ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef = TypedDict(
+    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
     {
-        "versionQualifier": str,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef = TypedDict(
-    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
+ListWorldExportJobsRequestRequestTypeDef = TypedDict(
+    "ListWorldExportJobsRequestRequestTypeDef",
     {
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationJobsRequestListSimulationJobsPaginateTypeDef = TypedDict(
-    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
+ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef = TypedDict(
+    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef = TypedDict(
-    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
+ListWorldGenerationJobsRequestRequestTypeDef = TypedDict(
+    "ListWorldGenerationJobsRequestRequestTypeDef",
     {
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef = TypedDict(
-    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
+ListWorldsRequestListWorldsPaginateTypeDef = TypedDict(
+    "ListWorldsRequestListWorldsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef = TypedDict(
-    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
+ListWorldsRequestRequestTypeDef = TypedDict(
+    "ListWorldsRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "nextToken": str,
+        "maxResults": int,
+        "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListWorldsRequestListWorldsPaginateTypeDef = TypedDict(
-    "ListWorldsRequestListWorldsPaginateTypeDef",
+ListFleetsResponseTypeDef = TypedDict(
+    "ListFleetsResponseTypeDef",
     {
-        "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "fleetDetails": List[FleetTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 ListSimulationJobBatchesResponseTypeDef = TypedDict(
     "ListSimulationJobBatchesResponseTypeDef",
     {
         "simulationJobBatchSummaries": List[SimulationJobBatchSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorldTemplatesResponseTypeDef = TypedDict(
     "ListWorldTemplatesResponseTypeDef",
     {
         "templateSummaries": List[TemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorldsResponseTypeDef = TypedDict(
     "ListWorldsResponseTypeDef",
     {
         "worldSummaries": List[WorldSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PortForwardingConfigTypeDef = TypedDict(
     "PortForwardingConfigTypeDef",
     {
         "portMappings": List[PortMappingTypeDef],
@@ -1875,42 +1875,42 @@
 )
 
 ListRobotApplicationsResponseTypeDef = TypedDict(
     "ListRobotApplicationsResponseTypeDef",
     {
         "robotApplicationSummaries": List[RobotApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSimulationApplicationsResponseTypeDef = TypedDict(
     "ListSimulationApplicationsResponseTypeDef",
     {
         "simulationApplicationSummaries": List[SimulationApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorldExportJobsResponseTypeDef = TypedDict(
     "ListWorldExportJobsResponseTypeDef",
     {
         "worldExportJobSummaries": List[WorldExportJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListWorldGenerationJobsResponseTypeDef = TypedDict(
     "ListWorldGenerationJobsResponseTypeDef",
     {
         "worldGenerationJobSummaries": List[WorldGenerationJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
@@ -1941,15 +1941,15 @@
         "status": DeploymentStatusType,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "deploymentConfig": DeploymentConfigTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentJobTypeDef = TypedDict(
     "DeploymentJobTypeDef",
     {
         "arn": str,
@@ -1971,15 +1971,15 @@
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentConfig": DeploymentConfigTypeDef,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FinishedWorldsSummaryTypeDef = TypedDict(
     "FinishedWorldsSummaryTypeDef",
     {
         "finishedCount": int,
@@ -2011,24 +2011,24 @@
         "deploymentConfig": DeploymentConfigTypeDef,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "robotDeploymentSummary": List[RobotDeploymentTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeploymentJobsResponseTypeDef = TypedDict(
     "ListDeploymentJobsResponseTypeDef",
     {
         "deploymentJobs": List[DeploymentJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorldGenerationJobResponseTypeDef = TypedDict(
     "DescribeWorldGenerationJobResponseTypeDef",
     {
         "arn": str,
@@ -2038,15 +2038,15 @@
         "failureReason": str,
         "clientRequestToken": str,
         "template": str,
         "worldCount": WorldCountTypeDef,
         "finishedWorldsSummary": FinishedWorldsSummaryTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRobotApplicationConfigTypeDef = TypedDict(
     "_RequiredRobotApplicationConfigTypeDef",
     {
         "application": str,
@@ -2142,15 +2142,15 @@
         "iamRole": str,
         "robotApplications": List[RobotApplicationConfigTypeDef],
         "simulationApplications": List[SimulationApplicationConfigTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "compute": ComputeResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSimulationJobResponseTypeDef = TypedDict(
     "DescribeSimulationJobResponseTypeDef",
     {
         "arn": str,
@@ -2170,15 +2170,15 @@
         "robotApplications": List[RobotApplicationConfigTypeDef],
         "simulationApplications": List[SimulationApplicationConfigTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSimulationJobRequestTypeDef = TypedDict(
     "_RequiredSimulationJobRequestTypeDef",
     {
         "maxJobDurationInSeconds": int,
@@ -2269,15 +2269,15 @@
     pass
 
 BatchDescribeSimulationJobResponseTypeDef = TypedDict(
     "BatchDescribeSimulationJobResponseTypeDef",
     {
         "jobs": List[SimulationJobTypeDef],
         "unprocessedJobs": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSimulationJobBatchResponseTypeDef = TypedDict(
     "DescribeSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
@@ -2288,15 +2288,15 @@
         "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
         "pendingRequests": List[SimulationJobRequestTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartSimulationJobBatchResponseTypeDef = TypedDict(
     "StartSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
@@ -2306,10 +2306,10 @@
         "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
         "pendingRequests": List[SimulationJobRequestTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker.egg-info/PKG-INFO` & `mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-robomaker
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.RoboMaker 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.RoboMaker 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/
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
 
 <a id="mypy-boto3-robomaker"></a>
 
 # mypy-boto3-robomaker
 
 [![PyPI - mypy-boto3-robomaker](https://img.shields.io/pypi/v/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-robomaker?color=blue)](https://pypistats.org/packages/mypy-boto3-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RoboMaker 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[boto3.RoboMaker 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [mypy-boto3-robomaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -388,95 +389,96 @@
 
 `mypy_boto3_robomaker.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_robomaker.type_defs import (
     BatchDeleteWorldsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    BatchDeleteWorldsResponseTypeDef,
     BatchDescribeSimulationJobRequestRequestTypeDef,
     BatchPolicyTypeDef,
     CancelDeploymentJobRequestRequestTypeDef,
     CancelSimulationJobBatchRequestRequestTypeDef,
     CancelSimulationJobRequestRequestTypeDef,
     CancelWorldExportJobRequestRequestTypeDef,
     CancelWorldGenerationJobRequestRequestTypeDef,
     ComputeResponseTypeDef,
     ComputeTypeDef,
     CreateFleetRequestRequestTypeDef,
+    CreateFleetResponseTypeDef,
     EnvironmentTypeDef,
     RobotSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
+    CreateRobotResponseTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
     DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
     TemplateLocationTypeDef,
+    CreateWorldTemplateResponseTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
     DeploymentLaunchConfigTypeDef,
     S3ObjectTypeDef,
     DeregisterRobotRequestRequestTypeDef,
+    DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobRequestRequestTypeDef,
     DescribeFleetRequestRequestTypeDef,
     RobotTypeDef,
     DescribeRobotApplicationRequestRequestTypeDef,
     DescribeRobotRequestRequestTypeDef,
+    DescribeRobotResponseTypeDef,
     DescribeSimulationApplicationRequestRequestTypeDef,
     DescribeSimulationJobBatchRequestRequestTypeDef,
     SimulationJobSummaryTypeDef,
     DescribeSimulationJobRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     DescribeWorldExportJobRequestRequestTypeDef,
     DescribeWorldGenerationJobRequestRequestTypeDef,
     DescribeWorldRequestRequestTypeDef,
+    DescribeWorldResponseTypeDef,
     DescribeWorldTemplateRequestRequestTypeDef,
+    DescribeWorldTemplateResponseTypeDef,
     WorldFailureTypeDef,
     FilterTypeDef,
     FleetTypeDef,
     GetWorldTemplateBodyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetWorldTemplateBodyResponseTypeDef,
     SimulationJobBatchSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
     ListWorldTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     WorldSummaryTypeDef,
+    PaginatorConfigTypeDef,
     PortMappingTypeDef,
     ProgressDetailTypeDef,
     RegisterRobotRequestRequestTypeDef,
+    RegisterRobotResponseTypeDef,
+    ResponseMetadataTypeDef,
     RestartSimulationJobRequestRequestTypeDef,
     ToolTypeDef,
     UploadConfigurationTypeDef,
     WorldConfigTypeDef,
     SyncDeploymentJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    BatchDeleteWorldsResponseTypeDef,
-    CreateFleetResponseTypeDef,
-    CreateRobotResponseTypeDef,
-    CreateWorldTemplateResponseTypeDef,
-    DeregisterRobotResponseTypeDef,
-    DescribeRobotResponseTypeDef,
-    DescribeWorldResponseTypeDef,
-    DescribeWorldTemplateResponseTypeDef,
-    GetWorldTemplateBodyResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RegisterRobotResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
     RobotApplicationSummaryTypeDef,
     CreateRobotApplicationRequestRequestTypeDef,
     UpdateRobotApplicationRequestRequestTypeDef,
     CreateRobotApplicationResponseTypeDef,
     CreateRobotApplicationVersionResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
@@ -500,36 +502,35 @@
     DataSourceTypeDef,
     DeploymentApplicationConfigTypeDef,
     DeploymentConfigTypeDef,
     DescribeFleetResponseTypeDef,
     ListRobotsResponseTypeDef,
     ListSimulationJobsResponseTypeDef,
     FailureSummaryTypeDef,
+    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
     ListDeploymentJobsRequestRequestTypeDef,
+    ListFleetsRequestListFleetsPaginateTypeDef,
     ListFleetsRequestRequestTypeDef,
+    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
     ListRobotApplicationsRequestRequestTypeDef,
+    ListRobotsRequestListRobotsPaginateTypeDef,
     ListRobotsRequestRequestTypeDef,
+    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
     ListSimulationApplicationsRequestRequestTypeDef,
+    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
     ListSimulationJobBatchesRequestRequestTypeDef,
+    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
     ListSimulationJobsRequestRequestTypeDef,
+    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
     ListWorldExportJobsRequestRequestTypeDef,
+    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
     ListWorldGenerationJobsRequestRequestTypeDef,
+    ListWorldsRequestListWorldsPaginateTypeDef,
     ListWorldsRequestRequestTypeDef,
     ListFleetsResponseTypeDef,
-    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
-    ListFleetsRequestListFleetsPaginateTypeDef,
-    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
-    ListRobotsRequestListRobotsPaginateTypeDef,
-    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
-    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
-    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
-    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
-    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
-    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
-    ListWorldsRequestListWorldsPaginateTypeDef,
     ListSimulationJobBatchesResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     ListWorldsResponseTypeDef,
     PortForwardingConfigTypeDef,
     RobotDeploymentTypeDef,
     ListRobotApplicationsResponseTypeDef,
     ListSimulationApplicationsResponseTypeDef,
@@ -566,42 +567,42 @@
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

### Comparing `mypy-boto3-robomaker-1.26.0.post1/mypy_boto3_robomaker.egg-info/SOURCES.txt` & `mypy-boto3-robomaker-1.27.0/mypy_boto3_robomaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.26.0.post1/setup.py` & `mypy-boto3-robomaker-1.27.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-robomaker.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-robomaker",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_robomaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RoboMaker 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.RoboMaker 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 robomaker type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_robomaker": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_robomaker": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/",
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


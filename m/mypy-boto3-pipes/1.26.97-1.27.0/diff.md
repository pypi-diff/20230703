# Comparing `tmp/mypy-boto3-pipes-1.26.97.tar.gz` & `tmp/mypy-boto3-pipes-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pipes-1.26.97.tar", last modified: Wed Mar 22 19:32:31 2023, max compression
+gzip compressed data, was "mypy-boto3-pipes-1.27.0.tar", last modified: Mon Jul  3 19:51:15 2023, max compression
```

## Comparing `mypy-boto3-pipes-1.26.97.tar` & `mypy-boto3-pipes-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.369775 mypy-boto3-pipes-1.26.97/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-22 19:32:09.000000 mypy-boto3-pipes-1.26.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16101 2023-03-22 19:32:31.365775 mypy-boto3-pipes-1.26.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-03-22 19:32:09.000000 mypy-boto3-pipes-1.26.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.365775 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-22 19:32:09.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-22 19:32:09.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-03-22 19:32:09.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-03-22 19:32:09.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-03-22 19:32:09.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-03-22 19:32:10.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-03-22 19:32:10.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-22 19:32:09.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-03-22 19:32:09.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:09.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31863 2023-03-22 19:32:10.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31833 2023-03-22 19:32:10.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-22 19:32:09.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.365775 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16101 2023-03-22 19:32:31.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-22 19:32:31.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:32:31.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:32:31.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-22 19:32:31.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-22 19:32:31.000000 mypy-boto3-pipes-1.26.97/mypy_boto3_pipes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 19:32:31.369775 mypy-boto3-pipes-1.26.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-22 19:32:09.000000 mypy-boto3-pipes-1.26.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:15.523808 mypy-boto3-pipes-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:43.000000 mypy-boto3-pipes-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-03 19:51:15.523808 mypy-boto3-pipes-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-07-03 19:43:43.000000 mypy-boto3-pipes-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:15.523808 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-03 19:43:43.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-03 19:43:43.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-03 19:43:43.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-07-03 19:43:43.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-07-03 19:43:43.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-07-03 19:43:44.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-07-03 19:43:43.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-03 19:43:43.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-03 19:43:43.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:43.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31881 2023-07-03 19:43:44.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31851 2023-07-03 19:43:44.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:43.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:15.523808 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-03 19:51:15.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 19:51:15.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:15.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:15.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:15.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 19:51:15.000000 mypy-boto3-pipes-1.27.0/mypy_boto3_pipes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:15.523808 mypy-boto3-pipes-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-03 19:43:43.000000 mypy-boto3-pipes-1.27.0/setup.py
```

### Comparing `mypy-boto3-pipes-1.26.97/LICENSE` & `mypy-boto3-pipes-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-pipes-1.26.97/PKG-INFO` & `mypy-boto3-pipes-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pipes
-Version: 1.26.97
-Summary: Type annotations for boto3.EventBridgePipes 1.26.97 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.EventBridgePipes 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-pipes"></a>
 
 # mypy-boto3-pipes
 
 [![PyPI - mypy-boto3-pipes](https://img.shields.io/pypi/v/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pipes?color=blue)](https://pypistats.org/packages/mypy-boto3-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgePipes 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[boto3.EventBridgePipes 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,30 +343,33 @@
     AwsVpcConfigurationTypeDef,
     BatchArrayPropertiesTypeDef,
     BatchEnvironmentVariableTypeDef,
     BatchResourceRequirementTypeDef,
     BatchJobDependencyTypeDef,
     BatchRetryStrategyTypeDef,
     CapacityProviderStrategyItemTypeDef,
-    ResponseMetadataTypeDef,
+    CreatePipeResponseTypeDef,
     DeadLetterConfigTypeDef,
     DeletePipeRequestRequestTypeDef,
+    DeletePipeResponseTypeDef,
     DescribePipeRequestRequestTypeDef,
     EcsEnvironmentFileTypeDef,
     EcsEnvironmentVariableTypeDef,
     EcsResourceRequirementTypeDef,
     EcsEphemeralStorageTypeDef,
     EcsInferenceAcceleratorOverrideTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
+    ListPipesRequestListPipesPaginateTypeDef,
     ListPipesRequestRequestTypeDef,
     PipeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MQBrokerAccessCredentialsTypeDef,
     MSKAccessCredentialsTypeDef,
+    PaginatorConfigTypeDef,
     PipeEnrichmentHttpParametersTypeDef,
     PipeSourceSqsQueueParametersTypeDef,
     SelfManagedKafkaAccessConfigurationCredentialsTypeDef,
     SelfManagedKafkaAccessConfigurationVpcTypeDef,
     PipeTargetCloudWatchLogsParametersTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
@@ -375,34 +378,31 @@
     PipeTargetHttpParametersTypeDef,
     PipeTargetKinesisStreamParametersTypeDef,
     PipeTargetLambdaFunctionParametersTypeDef,
     PipeTargetRedshiftDataParametersTypeDef,
     PipeTargetSqsQueueParametersTypeDef,
     PipeTargetStateMachineParametersTypeDef,
     SageMakerPipelineParameterTypeDef,
+    ResponseMetadataTypeDef,
     StartPipeRequestRequestTypeDef,
+    StartPipeResponseTypeDef,
     StopPipeRequestRequestTypeDef,
+    StopPipeResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdatePipeResponseTypeDef,
     UpdatePipeSourceSqsQueueParametersTypeDef,
     NetworkConfigurationTypeDef,
     BatchContainerOverridesTypeDef,
-    CreatePipeResponseTypeDef,
-    DeletePipeResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartPipeResponseTypeDef,
-    StopPipeResponseTypeDef,
-    UpdatePipeResponseTypeDef,
     PipeSourceDynamoDBStreamParametersTypeDef,
     PipeSourceKinesisStreamParametersTypeDef,
     UpdatePipeSourceDynamoDBStreamParametersTypeDef,
     UpdatePipeSourceKinesisStreamParametersTypeDef,
     EcsContainerOverrideTypeDef,
     FilterCriteriaTypeDef,
-    ListPipesRequestListPipesPaginateTypeDef,
     ListPipesResponseTypeDef,
     PipeSourceActiveMQBrokerParametersTypeDef,
     PipeSourceRabbitMQBrokerParametersTypeDef,
     UpdatePipeSourceActiveMQBrokerParametersTypeDef,
     UpdatePipeSourceRabbitMQBrokerParametersTypeDef,
     PipeSourceManagedStreamingKafkaParametersTypeDef,
     UpdatePipeSourceManagedStreamingKafkaParametersTypeDef,
@@ -429,42 +429,42 @@
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

### Comparing `mypy-boto3-pipes-1.26.97/README.md` & `mypy-boto3-pipes-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-pipes"></a>
 
 # mypy-boto3-pipes
 
 [![PyPI - mypy-boto3-pipes](https://img.shields.io/pypi/v/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pipes?color=blue)](https://pypistats.org/packages/mypy-boto3-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgePipes 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[boto3.EventBridgePipes 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,30 +311,33 @@
     AwsVpcConfigurationTypeDef,
     BatchArrayPropertiesTypeDef,
     BatchEnvironmentVariableTypeDef,
     BatchResourceRequirementTypeDef,
     BatchJobDependencyTypeDef,
     BatchRetryStrategyTypeDef,
     CapacityProviderStrategyItemTypeDef,
-    ResponseMetadataTypeDef,
+    CreatePipeResponseTypeDef,
     DeadLetterConfigTypeDef,
     DeletePipeRequestRequestTypeDef,
+    DeletePipeResponseTypeDef,
     DescribePipeRequestRequestTypeDef,
     EcsEnvironmentFileTypeDef,
     EcsEnvironmentVariableTypeDef,
     EcsResourceRequirementTypeDef,
     EcsEphemeralStorageTypeDef,
     EcsInferenceAcceleratorOverrideTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
+    ListPipesRequestListPipesPaginateTypeDef,
     ListPipesRequestRequestTypeDef,
     PipeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MQBrokerAccessCredentialsTypeDef,
     MSKAccessCredentialsTypeDef,
+    PaginatorConfigTypeDef,
     PipeEnrichmentHttpParametersTypeDef,
     PipeSourceSqsQueueParametersTypeDef,
     SelfManagedKafkaAccessConfigurationCredentialsTypeDef,
     SelfManagedKafkaAccessConfigurationVpcTypeDef,
     PipeTargetCloudWatchLogsParametersTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
@@ -343,34 +346,31 @@
     PipeTargetHttpParametersTypeDef,
     PipeTargetKinesisStreamParametersTypeDef,
     PipeTargetLambdaFunctionParametersTypeDef,
     PipeTargetRedshiftDataParametersTypeDef,
     PipeTargetSqsQueueParametersTypeDef,
     PipeTargetStateMachineParametersTypeDef,
     SageMakerPipelineParameterTypeDef,
+    ResponseMetadataTypeDef,
     StartPipeRequestRequestTypeDef,
+    StartPipeResponseTypeDef,
     StopPipeRequestRequestTypeDef,
+    StopPipeResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdatePipeResponseTypeDef,
     UpdatePipeSourceSqsQueueParametersTypeDef,
     NetworkConfigurationTypeDef,
     BatchContainerOverridesTypeDef,
-    CreatePipeResponseTypeDef,
-    DeletePipeResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartPipeResponseTypeDef,
-    StopPipeResponseTypeDef,
-    UpdatePipeResponseTypeDef,
     PipeSourceDynamoDBStreamParametersTypeDef,
     PipeSourceKinesisStreamParametersTypeDef,
     UpdatePipeSourceDynamoDBStreamParametersTypeDef,
     UpdatePipeSourceKinesisStreamParametersTypeDef,
     EcsContainerOverrideTypeDef,
     FilterCriteriaTypeDef,
-    ListPipesRequestListPipesPaginateTypeDef,
     ListPipesResponseTypeDef,
     PipeSourceActiveMQBrokerParametersTypeDef,
     PipeSourceRabbitMQBrokerParametersTypeDef,
     UpdatePipeSourceActiveMQBrokerParametersTypeDef,
     UpdatePipeSourceRabbitMQBrokerParametersTypeDef,
     PipeSourceManagedStreamingKafkaParametersTypeDef,
     UpdatePipeSourceManagedStreamingKafkaParametersTypeDef,
@@ -397,42 +397,42 @@
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

### Comparing `mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/__init__.py` & `mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/__init__.pyi` & `mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/__main__.py` & `mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridgePipes 1.26.97\nVersion:         1.26.97\nBuilder"
-        " version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.EventBridgePipes 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.97")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/client.py` & `mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/client.pyi` & `mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/literals.py` & `mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
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
@@ -137,14 +138,15 @@
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
@@ -242,14 +244,15 @@
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
@@ -285,14 +288,15 @@
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
@@ -311,16 +315,19 @@
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
@@ -404,15 +411,17 @@
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

### Comparing `mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/literals.pyi` & `mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
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
@@ -135,14 +136,15 @@
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
@@ -240,14 +242,15 @@
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
@@ -283,14 +286,15 @@
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
@@ -309,16 +313,19 @@
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
@@ -402,15 +409,17 @@
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

### Comparing `mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/paginator.py` & `mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -24,38 +24,35 @@
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import PipeStateType, RequestedPipeStateType
 from .type_defs import ListPipesResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListPipesPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListPipesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Paginator.ListPipes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/paginators/#listpipespaginator)
     """
 
     def paginate(
         self,
         *,
         CurrentState: PipeStateType = ...,
         DesiredState: RequestedPipeStateType = ...,
         NamePrefix: str = ...,
         SourcePrefix: str = ...,
         TargetPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Paginator.ListPipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/paginators/#listpipespaginator)
         """
```

### Comparing `mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/paginator.pyi` & `mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,35 +24,38 @@
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import PipeStateType, RequestedPipeStateType
 from .type_defs import ListPipesResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListPipesPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListPipesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Paginator.ListPipes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/paginators/#listpipespaginator)
     """
 
     def paginate(
         self,
         *,
         CurrentState: PipeStateType = ...,
         DesiredState: RequestedPipeStateType = ...,
         NamePrefix: str = ...,
         SourcePrefix: str = ...,
         TargetPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Paginator.ListPipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/paginators/#listpipespaginator)
         """
```

### Comparing `mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/type_defs.py` & `mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,30 +47,33 @@
     "AwsVpcConfigurationTypeDef",
     "BatchArrayPropertiesTypeDef",
     "BatchEnvironmentVariableTypeDef",
     "BatchResourceRequirementTypeDef",
     "BatchJobDependencyTypeDef",
     "BatchRetryStrategyTypeDef",
     "CapacityProviderStrategyItemTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreatePipeResponseTypeDef",
     "DeadLetterConfigTypeDef",
     "DeletePipeRequestRequestTypeDef",
+    "DeletePipeResponseTypeDef",
     "DescribePipeRequestRequestTypeDef",
     "EcsEnvironmentFileTypeDef",
     "EcsEnvironmentVariableTypeDef",
     "EcsResourceRequirementTypeDef",
     "EcsEphemeralStorageTypeDef",
     "EcsInferenceAcceleratorOverrideTypeDef",
     "FilterTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListPipesRequestListPipesPaginateTypeDef",
     "ListPipesRequestRequestTypeDef",
     "PipeTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "MQBrokerAccessCredentialsTypeDef",
     "MSKAccessCredentialsTypeDef",
+    "PaginatorConfigTypeDef",
     "PipeEnrichmentHttpParametersTypeDef",
     "PipeSourceSqsQueueParametersTypeDef",
     "SelfManagedKafkaAccessConfigurationCredentialsTypeDef",
     "SelfManagedKafkaAccessConfigurationVpcTypeDef",
     "PipeTargetCloudWatchLogsParametersTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
@@ -79,34 +82,31 @@
     "PipeTargetHttpParametersTypeDef",
     "PipeTargetKinesisStreamParametersTypeDef",
     "PipeTargetLambdaFunctionParametersTypeDef",
     "PipeTargetRedshiftDataParametersTypeDef",
     "PipeTargetSqsQueueParametersTypeDef",
     "PipeTargetStateMachineParametersTypeDef",
     "SageMakerPipelineParameterTypeDef",
+    "ResponseMetadataTypeDef",
     "StartPipeRequestRequestTypeDef",
+    "StartPipeResponseTypeDef",
     "StopPipeRequestRequestTypeDef",
+    "StopPipeResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdatePipeResponseTypeDef",
     "UpdatePipeSourceSqsQueueParametersTypeDef",
     "NetworkConfigurationTypeDef",
     "BatchContainerOverridesTypeDef",
-    "CreatePipeResponseTypeDef",
-    "DeletePipeResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartPipeResponseTypeDef",
-    "StopPipeResponseTypeDef",
-    "UpdatePipeResponseTypeDef",
     "PipeSourceDynamoDBStreamParametersTypeDef",
     "PipeSourceKinesisStreamParametersTypeDef",
     "UpdatePipeSourceDynamoDBStreamParametersTypeDef",
     "UpdatePipeSourceKinesisStreamParametersTypeDef",
     "EcsContainerOverrideTypeDef",
     "FilterCriteriaTypeDef",
-    "ListPipesRequestListPipesPaginateTypeDef",
     "ListPipesResponseTypeDef",
     "PipeSourceActiveMQBrokerParametersTypeDef",
     "PipeSourceRabbitMQBrokerParametersTypeDef",
     "UpdatePipeSourceActiveMQBrokerParametersTypeDef",
     "UpdatePipeSourceRabbitMQBrokerParametersTypeDef",
     "PipeSourceManagedStreamingKafkaParametersTypeDef",
     "UpdatePipeSourceManagedStreamingKafkaParametersTypeDef",
@@ -207,22 +207,24 @@
 
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreatePipeResponseTypeDef = TypedDict(
+    "CreatePipeResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "CreationTime": datetime,
+        "CurrentState": PipeStateType,
+        "DesiredState": RequestedPipeStateType,
+        "LastModifiedTime": datetime,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
@@ -233,14 +235,27 @@
 DeletePipeRequestRequestTypeDef = TypedDict(
     "DeletePipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeletePipeResponseTypeDef = TypedDict(
+    "DeletePipeResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "CurrentState": PipeStateType,
+        "DesiredState": RequestedPipeStateDescribeResponseType,
+        "LastModifiedTime": datetime,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribePipeRequestRequestTypeDef = TypedDict(
     "DescribePipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -289,20 +304,23 @@
     "FilterTypeDef",
     {
         "Pattern": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListPipesRequestListPipesPaginateTypeDef = TypedDict(
+    "ListPipesRequestListPipesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "CurrentState": PipeStateType,
+        "DesiredState": RequestedPipeStateType,
+        "NamePrefix": str,
+        "SourcePrefix": str,
+        "TargetPrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPipesRequestRequestTypeDef = TypedDict(
     "ListPipesRequestRequestTypeDef",
     {
@@ -337,14 +355,22 @@
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
 MQBrokerAccessCredentialsTypeDef = TypedDict(
     "MQBrokerAccessCredentialsTypeDef",
     {
         "BasicAuth": str,
     },
     total=False,
 )
@@ -354,14 +380,24 @@
     {
         "ClientCertificateTlsAuth": str,
         "SaslScram512Auth": str,
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
 PipeEnrichmentHttpParametersTypeDef = TypedDict(
     "PipeEnrichmentHttpParametersTypeDef",
     {
         "HeaderParameters": Mapping[str, str],
         "PathParameterValues": Sequence[str],
         "QueryStringParameters": Mapping[str, str],
     },
@@ -516,28 +552,65 @@
     "SageMakerPipelineParameterTypeDef",
     {
         "Name": str,
         "Value": str,
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
 StartPipeRequestRequestTypeDef = TypedDict(
     "StartPipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+StartPipeResponseTypeDef = TypedDict(
+    "StartPipeResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "CurrentState": PipeStateType,
+        "DesiredState": RequestedPipeStateType,
+        "LastModifiedTime": datetime,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopPipeRequestRequestTypeDef = TypedDict(
     "StopPipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+StopPipeResponseTypeDef = TypedDict(
+    "StopPipeResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "CurrentState": PipeStateType,
+        "DesiredState": RequestedPipeStateType,
+        "LastModifiedTime": datetime,
+        "Name": str,
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
@@ -546,14 +619,27 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdatePipeResponseTypeDef = TypedDict(
+    "UpdatePipeResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "CurrentState": PipeStateType,
+        "DesiredState": RequestedPipeStateType,
+        "LastModifiedTime": datetime,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdatePipeSourceSqsQueueParametersTypeDef = TypedDict(
     "UpdatePipeSourceSqsQueueParametersTypeDef",
     {
         "BatchSize": int,
         "MaximumBatchingWindowInSeconds": int,
     },
     total=False,
@@ -574,87 +660,14 @@
         "Environment": Sequence[BatchEnvironmentVariableTypeDef],
         "InstanceType": str,
         "ResourceRequirements": Sequence[BatchResourceRequirementTypeDef],
     },
     total=False,
 )
 
-CreatePipeResponseTypeDef = TypedDict(
-    "CreatePipeResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "CurrentState": PipeStateType,
-        "DesiredState": RequestedPipeStateType,
-        "LastModifiedTime": datetime,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePipeResponseTypeDef = TypedDict(
-    "DeletePipeResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "CurrentState": PipeStateType,
-        "DesiredState": RequestedPipeStateDescribeResponseType,
-        "LastModifiedTime": datetime,
-        "Name": str,
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
-StartPipeResponseTypeDef = TypedDict(
-    "StartPipeResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "CurrentState": PipeStateType,
-        "DesiredState": RequestedPipeStateType,
-        "LastModifiedTime": datetime,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopPipeResponseTypeDef = TypedDict(
-    "StopPipeResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "CurrentState": PipeStateType,
-        "DesiredState": RequestedPipeStateType,
-        "LastModifiedTime": datetime,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePipeResponseTypeDef = TypedDict(
-    "UpdatePipeResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "CurrentState": PipeStateType,
-        "DesiredState": RequestedPipeStateType,
-        "LastModifiedTime": datetime,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredPipeSourceDynamoDBStreamParametersTypeDef = TypedDict(
     "_RequiredPipeSourceDynamoDBStreamParametersTypeDef",
     {
         "StartingPosition": DynamoDBStreamStartPositionType,
     },
 )
 _OptionalPipeSourceDynamoDBStreamParametersTypeDef = TypedDict(
@@ -755,33 +768,20 @@
     "FilterCriteriaTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListPipesRequestListPipesPaginateTypeDef = TypedDict(
-    "ListPipesRequestListPipesPaginateTypeDef",
-    {
-        "CurrentState": PipeStateType,
-        "DesiredState": RequestedPipeStateType,
-        "NamePrefix": str,
-        "SourcePrefix": str,
-        "TargetPrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListPipesResponseTypeDef = TypedDict(
     "ListPipesResponseTypeDef",
     {
         "NextToken": str,
         "Pipes": List[PipeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPipeSourceActiveMQBrokerParametersTypeDef = TypedDict(
     "_RequiredPipeSourceActiveMQBrokerParametersTypeDef",
     {
         "Credentials": MQBrokerAccessCredentialsTypeDef,
@@ -1138,15 +1138,15 @@
         "RoleArn": str,
         "Source": str,
         "SourceParameters": PipeSourceParametersTypeDef,
         "StateReason": str,
         "Tags": Dict[str, str],
         "Target": str,
         "TargetParameters": PipeTargetParametersTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdatePipeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipeRequestRequestTypeDef",
     {
         "Name": str,
```

### Comparing `mypy-boto3-pipes-1.26.97/mypy_boto3_pipes/type_defs.pyi` & `mypy-boto3-pipes-1.27.0/mypy_boto3_pipes/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -46,30 +46,33 @@
     "AwsVpcConfigurationTypeDef",
     "BatchArrayPropertiesTypeDef",
     "BatchEnvironmentVariableTypeDef",
     "BatchResourceRequirementTypeDef",
     "BatchJobDependencyTypeDef",
     "BatchRetryStrategyTypeDef",
     "CapacityProviderStrategyItemTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreatePipeResponseTypeDef",
     "DeadLetterConfigTypeDef",
     "DeletePipeRequestRequestTypeDef",
+    "DeletePipeResponseTypeDef",
     "DescribePipeRequestRequestTypeDef",
     "EcsEnvironmentFileTypeDef",
     "EcsEnvironmentVariableTypeDef",
     "EcsResourceRequirementTypeDef",
     "EcsEphemeralStorageTypeDef",
     "EcsInferenceAcceleratorOverrideTypeDef",
     "FilterTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListPipesRequestListPipesPaginateTypeDef",
     "ListPipesRequestRequestTypeDef",
     "PipeTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "MQBrokerAccessCredentialsTypeDef",
     "MSKAccessCredentialsTypeDef",
+    "PaginatorConfigTypeDef",
     "PipeEnrichmentHttpParametersTypeDef",
     "PipeSourceSqsQueueParametersTypeDef",
     "SelfManagedKafkaAccessConfigurationCredentialsTypeDef",
     "SelfManagedKafkaAccessConfigurationVpcTypeDef",
     "PipeTargetCloudWatchLogsParametersTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
@@ -78,34 +81,31 @@
     "PipeTargetHttpParametersTypeDef",
     "PipeTargetKinesisStreamParametersTypeDef",
     "PipeTargetLambdaFunctionParametersTypeDef",
     "PipeTargetRedshiftDataParametersTypeDef",
     "PipeTargetSqsQueueParametersTypeDef",
     "PipeTargetStateMachineParametersTypeDef",
     "SageMakerPipelineParameterTypeDef",
+    "ResponseMetadataTypeDef",
     "StartPipeRequestRequestTypeDef",
+    "StartPipeResponseTypeDef",
     "StopPipeRequestRequestTypeDef",
+    "StopPipeResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdatePipeResponseTypeDef",
     "UpdatePipeSourceSqsQueueParametersTypeDef",
     "NetworkConfigurationTypeDef",
     "BatchContainerOverridesTypeDef",
-    "CreatePipeResponseTypeDef",
-    "DeletePipeResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartPipeResponseTypeDef",
-    "StopPipeResponseTypeDef",
-    "UpdatePipeResponseTypeDef",
     "PipeSourceDynamoDBStreamParametersTypeDef",
     "PipeSourceKinesisStreamParametersTypeDef",
     "UpdatePipeSourceDynamoDBStreamParametersTypeDef",
     "UpdatePipeSourceKinesisStreamParametersTypeDef",
     "EcsContainerOverrideTypeDef",
     "FilterCriteriaTypeDef",
-    "ListPipesRequestListPipesPaginateTypeDef",
     "ListPipesResponseTypeDef",
     "PipeSourceActiveMQBrokerParametersTypeDef",
     "PipeSourceRabbitMQBrokerParametersTypeDef",
     "UpdatePipeSourceActiveMQBrokerParametersTypeDef",
     "UpdatePipeSourceRabbitMQBrokerParametersTypeDef",
     "PipeSourceManagedStreamingKafkaParametersTypeDef",
     "UpdatePipeSourceManagedStreamingKafkaParametersTypeDef",
@@ -202,22 +202,24 @@
 )
 
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreatePipeResponseTypeDef = TypedDict(
+    "CreatePipeResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "CreationTime": datetime,
+        "CurrentState": PipeStateType,
+        "DesiredState": RequestedPipeStateType,
+        "LastModifiedTime": datetime,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
@@ -228,14 +230,27 @@
 DeletePipeRequestRequestTypeDef = TypedDict(
     "DeletePipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeletePipeResponseTypeDef = TypedDict(
+    "DeletePipeResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "CurrentState": PipeStateType,
+        "DesiredState": RequestedPipeStateDescribeResponseType,
+        "LastModifiedTime": datetime,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribePipeRequestRequestTypeDef = TypedDict(
     "DescribePipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -284,20 +299,23 @@
     "FilterTypeDef",
     {
         "Pattern": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListPipesRequestListPipesPaginateTypeDef = TypedDict(
+    "ListPipesRequestListPipesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "CurrentState": PipeStateType,
+        "DesiredState": RequestedPipeStateType,
+        "NamePrefix": str,
+        "SourcePrefix": str,
+        "TargetPrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPipesRequestRequestTypeDef = TypedDict(
     "ListPipesRequestRequestTypeDef",
     {
@@ -332,14 +350,22 @@
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
 MQBrokerAccessCredentialsTypeDef = TypedDict(
     "MQBrokerAccessCredentialsTypeDef",
     {
         "BasicAuth": str,
     },
     total=False,
 )
@@ -349,14 +375,24 @@
     {
         "ClientCertificateTlsAuth": str,
         "SaslScram512Auth": str,
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
 PipeEnrichmentHttpParametersTypeDef = TypedDict(
     "PipeEnrichmentHttpParametersTypeDef",
     {
         "HeaderParameters": Mapping[str, str],
         "PathParameterValues": Sequence[str],
         "QueryStringParameters": Mapping[str, str],
     },
@@ -509,28 +545,65 @@
     "SageMakerPipelineParameterTypeDef",
     {
         "Name": str,
         "Value": str,
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
 StartPipeRequestRequestTypeDef = TypedDict(
     "StartPipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+StartPipeResponseTypeDef = TypedDict(
+    "StartPipeResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "CurrentState": PipeStateType,
+        "DesiredState": RequestedPipeStateType,
+        "LastModifiedTime": datetime,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopPipeRequestRequestTypeDef = TypedDict(
     "StopPipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+StopPipeResponseTypeDef = TypedDict(
+    "StopPipeResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "CurrentState": PipeStateType,
+        "DesiredState": RequestedPipeStateType,
+        "LastModifiedTime": datetime,
+        "Name": str,
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
@@ -539,14 +612,27 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdatePipeResponseTypeDef = TypedDict(
+    "UpdatePipeResponseTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "CurrentState": PipeStateType,
+        "DesiredState": RequestedPipeStateType,
+        "LastModifiedTime": datetime,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdatePipeSourceSqsQueueParametersTypeDef = TypedDict(
     "UpdatePipeSourceSqsQueueParametersTypeDef",
     {
         "BatchSize": int,
         "MaximumBatchingWindowInSeconds": int,
     },
     total=False,
@@ -567,87 +653,14 @@
         "Environment": Sequence[BatchEnvironmentVariableTypeDef],
         "InstanceType": str,
         "ResourceRequirements": Sequence[BatchResourceRequirementTypeDef],
     },
     total=False,
 )
 
-CreatePipeResponseTypeDef = TypedDict(
-    "CreatePipeResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "CurrentState": PipeStateType,
-        "DesiredState": RequestedPipeStateType,
-        "LastModifiedTime": datetime,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePipeResponseTypeDef = TypedDict(
-    "DeletePipeResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "CurrentState": PipeStateType,
-        "DesiredState": RequestedPipeStateDescribeResponseType,
-        "LastModifiedTime": datetime,
-        "Name": str,
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
-StartPipeResponseTypeDef = TypedDict(
-    "StartPipeResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "CurrentState": PipeStateType,
-        "DesiredState": RequestedPipeStateType,
-        "LastModifiedTime": datetime,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopPipeResponseTypeDef = TypedDict(
-    "StopPipeResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "CurrentState": PipeStateType,
-        "DesiredState": RequestedPipeStateType,
-        "LastModifiedTime": datetime,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePipeResponseTypeDef = TypedDict(
-    "UpdatePipeResponseTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "CurrentState": PipeStateType,
-        "DesiredState": RequestedPipeStateType,
-        "LastModifiedTime": datetime,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredPipeSourceDynamoDBStreamParametersTypeDef = TypedDict(
     "_RequiredPipeSourceDynamoDBStreamParametersTypeDef",
     {
         "StartingPosition": DynamoDBStreamStartPositionType,
     },
 )
 _OptionalPipeSourceDynamoDBStreamParametersTypeDef = TypedDict(
@@ -744,33 +757,20 @@
     "FilterCriteriaTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListPipesRequestListPipesPaginateTypeDef = TypedDict(
-    "ListPipesRequestListPipesPaginateTypeDef",
-    {
-        "CurrentState": PipeStateType,
-        "DesiredState": RequestedPipeStateType,
-        "NamePrefix": str,
-        "SourcePrefix": str,
-        "TargetPrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListPipesResponseTypeDef = TypedDict(
     "ListPipesResponseTypeDef",
     {
         "NextToken": str,
         "Pipes": List[PipeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPipeSourceActiveMQBrokerParametersTypeDef = TypedDict(
     "_RequiredPipeSourceActiveMQBrokerParametersTypeDef",
     {
         "Credentials": MQBrokerAccessCredentialsTypeDef,
@@ -1109,15 +1109,15 @@
         "RoleArn": str,
         "Source": str,
         "SourceParameters": PipeSourceParametersTypeDef,
         "StateReason": str,
         "Tags": Dict[str, str],
         "Target": str,
         "TargetParameters": PipeTargetParametersTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdatePipeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipeRequestRequestTypeDef",
     {
         "Name": str,
```

### Comparing `mypy-boto3-pipes-1.26.97/mypy_boto3_pipes.egg-info/PKG-INFO` & `mypy-boto3-pipes-1.27.0/mypy_boto3_pipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pipes
-Version: 1.26.97
-Summary: Type annotations for boto3.EventBridgePipes 1.26.97 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.EventBridgePipes 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-pipes"></a>
 
 # mypy-boto3-pipes
 
 [![PyPI - mypy-boto3-pipes](https://img.shields.io/pypi/v/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pipes?color=blue)](https://pypistats.org/packages/mypy-boto3-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgePipes 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[boto3.EventBridgePipes 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,30 +343,33 @@
     AwsVpcConfigurationTypeDef,
     BatchArrayPropertiesTypeDef,
     BatchEnvironmentVariableTypeDef,
     BatchResourceRequirementTypeDef,
     BatchJobDependencyTypeDef,
     BatchRetryStrategyTypeDef,
     CapacityProviderStrategyItemTypeDef,
-    ResponseMetadataTypeDef,
+    CreatePipeResponseTypeDef,
     DeadLetterConfigTypeDef,
     DeletePipeRequestRequestTypeDef,
+    DeletePipeResponseTypeDef,
     DescribePipeRequestRequestTypeDef,
     EcsEnvironmentFileTypeDef,
     EcsEnvironmentVariableTypeDef,
     EcsResourceRequirementTypeDef,
     EcsEphemeralStorageTypeDef,
     EcsInferenceAcceleratorOverrideTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
+    ListPipesRequestListPipesPaginateTypeDef,
     ListPipesRequestRequestTypeDef,
     PipeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MQBrokerAccessCredentialsTypeDef,
     MSKAccessCredentialsTypeDef,
+    PaginatorConfigTypeDef,
     PipeEnrichmentHttpParametersTypeDef,
     PipeSourceSqsQueueParametersTypeDef,
     SelfManagedKafkaAccessConfigurationCredentialsTypeDef,
     SelfManagedKafkaAccessConfigurationVpcTypeDef,
     PipeTargetCloudWatchLogsParametersTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
@@ -375,34 +378,31 @@
     PipeTargetHttpParametersTypeDef,
     PipeTargetKinesisStreamParametersTypeDef,
     PipeTargetLambdaFunctionParametersTypeDef,
     PipeTargetRedshiftDataParametersTypeDef,
     PipeTargetSqsQueueParametersTypeDef,
     PipeTargetStateMachineParametersTypeDef,
     SageMakerPipelineParameterTypeDef,
+    ResponseMetadataTypeDef,
     StartPipeRequestRequestTypeDef,
+    StartPipeResponseTypeDef,
     StopPipeRequestRequestTypeDef,
+    StopPipeResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdatePipeResponseTypeDef,
     UpdatePipeSourceSqsQueueParametersTypeDef,
     NetworkConfigurationTypeDef,
     BatchContainerOverridesTypeDef,
-    CreatePipeResponseTypeDef,
-    DeletePipeResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartPipeResponseTypeDef,
-    StopPipeResponseTypeDef,
-    UpdatePipeResponseTypeDef,
     PipeSourceDynamoDBStreamParametersTypeDef,
     PipeSourceKinesisStreamParametersTypeDef,
     UpdatePipeSourceDynamoDBStreamParametersTypeDef,
     UpdatePipeSourceKinesisStreamParametersTypeDef,
     EcsContainerOverrideTypeDef,
     FilterCriteriaTypeDef,
-    ListPipesRequestListPipesPaginateTypeDef,
     ListPipesResponseTypeDef,
     PipeSourceActiveMQBrokerParametersTypeDef,
     PipeSourceRabbitMQBrokerParametersTypeDef,
     UpdatePipeSourceActiveMQBrokerParametersTypeDef,
     UpdatePipeSourceRabbitMQBrokerParametersTypeDef,
     PipeSourceManagedStreamingKafkaParametersTypeDef,
     UpdatePipeSourceManagedStreamingKafkaParametersTypeDef,
@@ -429,42 +429,42 @@
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

### Comparing `mypy-boto3-pipes-1.26.97/mypy_boto3_pipes.egg-info/SOURCES.txt` & `mypy-boto3-pipes-1.27.0/mypy_boto3_pipes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.26.97/setup.py` & `mypy-boto3-pipes-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-pipes.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pipes",
-    version="1.26.97",
+    version="1.27.0",
     packages=["mypy_boto3_pipes"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EventBridgePipes 1.26.97 service generated with"
-        " mypy-boto3-builder 7.13.0"
+        "Type annotations for boto3.EventBridgePipes 1.27.0 service generated with"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/",
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


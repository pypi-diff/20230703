# Comparing `tmp/mypy-boto3-emr-containers-1.26.68.tar.gz` & `tmp/mypy-boto3-emr-containers-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-containers-1.26.68.tar", last modified: Thu Feb  9 20:26:50 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-containers-1.27.0.tar", last modified: Mon Jul  3 19:50:45 2023, max compression
```

## Comparing `mypy-boto3-emr-containers-1.26.68.tar` & `mypy-boto3-emr-containers-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.994837 mypy-boto3-emr-containers-1.26.68/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-02-09 20:26:49.994837 mypy-boto3-emr-containers-1.26.68/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.990837 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-02-09 20:26:12.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24266 2023-02-09 20:26:12.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-02-09 20:26:12.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 20:26:49.994837 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-02-09 20:26:49.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-09 20:26:49.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 20:26:49.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-09 20:26:49.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-09 20:26:49.000000 mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 20:26:49.994837 mypy-boto3-emr-containers-1.26.68/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-02-09 20:26:11.000000 mypy-boto3-emr-containers-1.26.68/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.371231 mypy-boto3-emr-containers-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:30.000000 mypy-boto3-emr-containers-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-07-03 19:50:45.367231 mypy-boto3-emr-containers-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-07-03 19:37:30.000000 mypy-boto3-emr-containers-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.367231 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-03 19:37:30.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-03 19:37:30.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:37:30.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18379 2023-07-03 19:37:30.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-07-03 19:37:30.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-03 19:37:30.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-07-03 19:37:30.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-03 19:37:30.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-07-03 19:37:30.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:30.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25981 2023-07-03 19:37:32.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25950 2023-07-03 19:37:32.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:30.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.367231 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-07-03 19:50:45.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 19:50:45.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:45.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:45.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:45.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:50:45.000000 mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:45.371231 mypy-boto3-emr-containers-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-03 19:37:30.000000 mypy-boto3-emr-containers-1.27.0/setup.py
```

### Comparing `mypy-boto3-emr-containers-1.26.68/LICENSE` & `mypy-boto3-emr-containers-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-emr-containers-1.26.68/PKG-INFO` & `mypy-boto3-emr-containers-1.27.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-containers
-Version: 1.26.68
-Summary: Type annotations for boto3.EMRContainers 1.26.68 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.EMRContainers 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-emr-containers"></a>
 
 # mypy-boto3-emr-containers
 
 [![PyPI - mypy-boto3-emr-containers](https://img.shields.io/pypi/v/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-containers?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
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
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,57 +343,61 @@
 
 `mypy_boto3_emr_containers.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_containers.type_defs import (
     CancelJobRunRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJobRunResponseTypeDef,
     CertificateTypeDef,
     CloudWatchMonitoringConfigurationTypeDef,
     ConfigurationTypeDef,
     EksInfoTypeDef,
+    ContainerLogRotationConfigurationTypeDef,
+    CreateJobTemplateResponseTypeDef,
+    CreateManagedEndpointResponseTypeDef,
+    CreateVirtualClusterResponseTypeDef,
+    CredentialsTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
+    DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointRequestRequestTypeDef,
+    DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterRequestRequestTypeDef,
+    DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
     DescribeManagedEndpointRequestRequestTypeDef,
     DescribeVirtualClusterRequestRequestTypeDef,
+    GetManagedEndpointSessionCredentialsRequestRequestTypeDef,
     SparkSqlJobDriverTypeDef,
     SparkSubmitJobDriverTypeDef,
     RetryPolicyConfigurationTypeDef,
     RetryPolicyExecutionTypeDef,
     TemplateParameterConfigurationTypeDef,
-    PaginatorConfigTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
+    ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     ListManagedEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
     ListVirtualClustersRequestRequestTypeDef,
     S3MonitoringConfigurationTypeDef,
+    PaginatorConfigTypeDef,
     ParametricCloudWatchMonitoringConfigurationTypeDef,
     ParametricS3MonitoringConfigurationTypeDef,
+    ResponseMetadataTypeDef,
+    StartJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
-    CreateJobTemplateResponseTypeDef,
-    CreateManagedEndpointResponseTypeDef,
-    CreateVirtualClusterResponseTypeDef,
-    DeleteJobTemplateResponseTypeDef,
-    DeleteManagedEndpointResponseTypeDef,
-    DeleteVirtualClusterResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartJobRunResponseTypeDef,
     ContainerInfoTypeDef,
+    GetManagedEndpointSessionCredentialsResponseTypeDef,
     JobDriverTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
-    ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
-    ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
     MonitoringConfigurationTypeDef,
     ParametricMonitoringConfigurationTypeDef,
     ContainerProviderTypeDef,
     ConfigurationOverridesTypeDef,
     ParametricConfigurationOverridesTypeDef,
     CreateVirtualClusterRequestRequestTypeDef,
     VirtualClusterTypeDef,
@@ -422,42 +426,42 @@
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

### Comparing `mypy-boto3-emr-containers-1.26.68/README.md` & `mypy-boto3-emr-containers-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-emr-containers"></a>
 
 # mypy-boto3-emr-containers
 
 [![PyPI - mypy-boto3-emr-containers](https://img.shields.io/pypi/v/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-containers?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
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
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,57 +311,61 @@
 
 `mypy_boto3_emr_containers.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_containers.type_defs import (
     CancelJobRunRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJobRunResponseTypeDef,
     CertificateTypeDef,
     CloudWatchMonitoringConfigurationTypeDef,
     ConfigurationTypeDef,
     EksInfoTypeDef,
+    ContainerLogRotationConfigurationTypeDef,
+    CreateJobTemplateResponseTypeDef,
+    CreateManagedEndpointResponseTypeDef,
+    CreateVirtualClusterResponseTypeDef,
+    CredentialsTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
+    DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointRequestRequestTypeDef,
+    DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterRequestRequestTypeDef,
+    DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
     DescribeManagedEndpointRequestRequestTypeDef,
     DescribeVirtualClusterRequestRequestTypeDef,
+    GetManagedEndpointSessionCredentialsRequestRequestTypeDef,
     SparkSqlJobDriverTypeDef,
     SparkSubmitJobDriverTypeDef,
     RetryPolicyConfigurationTypeDef,
     RetryPolicyExecutionTypeDef,
     TemplateParameterConfigurationTypeDef,
-    PaginatorConfigTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
+    ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     ListManagedEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
     ListVirtualClustersRequestRequestTypeDef,
     S3MonitoringConfigurationTypeDef,
+    PaginatorConfigTypeDef,
     ParametricCloudWatchMonitoringConfigurationTypeDef,
     ParametricS3MonitoringConfigurationTypeDef,
+    ResponseMetadataTypeDef,
+    StartJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
-    CreateJobTemplateResponseTypeDef,
-    CreateManagedEndpointResponseTypeDef,
-    CreateVirtualClusterResponseTypeDef,
-    DeleteJobTemplateResponseTypeDef,
-    DeleteManagedEndpointResponseTypeDef,
-    DeleteVirtualClusterResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartJobRunResponseTypeDef,
     ContainerInfoTypeDef,
+    GetManagedEndpointSessionCredentialsResponseTypeDef,
     JobDriverTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
-    ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
-    ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
     MonitoringConfigurationTypeDef,
     ParametricMonitoringConfigurationTypeDef,
     ContainerProviderTypeDef,
     ConfigurationOverridesTypeDef,
     ParametricConfigurationOverridesTypeDef,
     CreateVirtualClusterRequestRequestTypeDef,
     VirtualClusterTypeDef,
@@ -390,42 +394,42 @@
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

### Comparing `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/__init__.py` & `mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/__init__.pyi` & `mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/__main__.py` & `mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRContainers 1.26.68\nVersion:         1.26.68\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.EMRContainers 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.68")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/client.py` & `mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeJobTemplateResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
     DescribeVirtualClusterResponseTypeDef,
+    GetManagedEndpointSessionCredentialsResponseTypeDef,
     JobDriverTypeDef,
     JobTemplateDataTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
@@ -67,14 +68,15 @@
         self.response: Dict[str, Any]
         self.operation_name: str
 
 
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
+    RequestThrottledException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 
 class EMRContainersClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client)
@@ -237,14 +239,32 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#generate_presigned_url)
         """
 
+    def get_managed_endpoint_session_credentials(
+        self,
+        *,
+        endpointIdentifier: str,
+        virtualClusterIdentifier: str,
+        executionRoleArn: str,
+        credentialType: str,
+        durationInSeconds: int = ...,
+        logContext: str = ...,
+        clientToken: str = ...
+    ) -> GetManagedEndpointSessionCredentialsResponseTypeDef:
+        """
+        Generate a session token to connect to a managed endpoint.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_managed_endpoint_session_credentials)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#get_managed_endpoint_session_credentials)
+        """
+
     def list_job_runs(
         self,
         *,
         virtualClusterId: str,
         createdBefore: Union[datetime, str] = ...,
         createdAfter: Union[datetime, str] = ...,
         name: str = ...,
```

### Comparing `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/client.pyi` & `mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeJobTemplateResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
     DescribeVirtualClusterResponseTypeDef,
+    GetManagedEndpointSessionCredentialsResponseTypeDef,
     JobDriverTypeDef,
     JobTemplateDataTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
@@ -64,14 +65,15 @@
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
+    RequestThrottledException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 class EMRContainersClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/)
@@ -218,14 +220,31 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#generate_presigned_url)
         """
+    def get_managed_endpoint_session_credentials(
+        self,
+        *,
+        endpointIdentifier: str,
+        virtualClusterIdentifier: str,
+        executionRoleArn: str,
+        credentialType: str,
+        durationInSeconds: int = ...,
+        logContext: str = ...,
+        clientToken: str = ...
+    ) -> GetManagedEndpointSessionCredentialsResponseTypeDef:
+        """
+        Generate a session token to connect to a managed endpoint.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_managed_endpoint_session_credentials)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#get_managed_endpoint_session_credentials)
+        """
     def list_job_runs(
         self,
         *,
         virtualClusterId: str,
         createdBefore: Union[datetime, str] = ...,
         createdAfter: Union[datetime, str] = ...,
         name: str = ...,
```

### Comparing `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/literals.py` & `mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
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
@@ -115,14 +116,15 @@
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
@@ -201,14 +203,15 @@
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
@@ -219,14 +222,15 @@
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
@@ -262,14 +266,15 @@
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
@@ -288,16 +293,19 @@
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
@@ -377,18 +385,21 @@
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
@@ -410,24 +421,26 @@
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_job_runs", "list_job_templates", "list_managed_endpoints", "list_virtual_clusters"
 ]
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

### Comparing `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/literals.pyi` & `mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
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
@@ -113,14 +114,15 @@
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
@@ -199,14 +201,15 @@
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
@@ -217,14 +220,15 @@
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
@@ -260,14 +264,15 @@
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
@@ -286,16 +291,19 @@
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
@@ -375,18 +383,21 @@
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
@@ -408,24 +419,26 @@
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_job_runs", "list_job_templates", "list_managed_endpoints", "list_virtual_clusters"
 ]
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

### Comparing `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/paginator.py` & `mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -41,109 +41,102 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListJobRunsPaginator",
     "ListJobTemplatesPaginator",
     "ListManagedEndpointsPaginator",
     "ListVirtualClustersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListJobRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobrunspaginator)
     """
 
     def paginate(
         self,
         *,
         virtualClusterId: str,
         createdBefore: Union[datetime, str] = ...,
         createdAfter: Union[datetime, str] = ...,
         name: str = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobrunspaginator)
         """
 
-
 class ListJobTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         createdAfter: Union[datetime, str] = ...,
         createdBefore: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobtemplatespaginator)
         """
 
-
 class ListManagedEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listmanagedendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         virtualClusterId: str,
         createdBefore: Union[datetime, str] = ...,
         createdAfter: Union[datetime, str] = ...,
         types: Sequence[str] = ...,
         states: Sequence[EndpointStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListManagedEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listmanagedendpointspaginator)
         """
 
-
 class ListVirtualClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listvirtualclusterspaginator)
     """
 
     def paginate(
         self,
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
         createdAfter: Union[datetime, str] = ...,
         createdBefore: Union[datetime, str] = ...,
         states: Sequence[VirtualClusterStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVirtualClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listvirtualclusterspaginator)
         """
```

### Comparing `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/paginator.pyi` & `mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,102 +41,109 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListJobRunsPaginator",
     "ListJobTemplatesPaginator",
     "ListManagedEndpointsPaginator",
     "ListVirtualClustersPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListJobRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobrunspaginator)
     """
 
     def paginate(
         self,
         *,
         virtualClusterId: str,
         createdBefore: Union[datetime, str] = ...,
         createdAfter: Union[datetime, str] = ...,
         name: str = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobrunspaginator)
         """
 
+
 class ListJobTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         createdAfter: Union[datetime, str] = ...,
         createdBefore: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobtemplatespaginator)
         """
 
+
 class ListManagedEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listmanagedendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         virtualClusterId: str,
         createdBefore: Union[datetime, str] = ...,
         createdAfter: Union[datetime, str] = ...,
         types: Sequence[str] = ...,
         states: Sequence[EndpointStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListManagedEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listmanagedendpointspaginator)
         """
 
+
 class ListVirtualClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listvirtualclusterspaginator)
     """
 
     def paginate(
         self,
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
         createdAfter: Union[datetime, str] = ...,
         createdBefore: Union[datetime, str] = ...,
         states: Sequence[VirtualClusterStateType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVirtualClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listvirtualclusterspaginator)
         """
```

### Comparing `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/type_defs.py` & `mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,57 +32,61 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelJobRunRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelJobRunResponseTypeDef",
     "CertificateTypeDef",
     "CloudWatchMonitoringConfigurationTypeDef",
     "ConfigurationTypeDef",
     "EksInfoTypeDef",
+    "ContainerLogRotationConfigurationTypeDef",
+    "CreateJobTemplateResponseTypeDef",
+    "CreateManagedEndpointResponseTypeDef",
+    "CreateVirtualClusterResponseTypeDef",
+    "CredentialsTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
+    "DeleteJobTemplateResponseTypeDef",
     "DeleteManagedEndpointRequestRequestTypeDef",
+    "DeleteManagedEndpointResponseTypeDef",
     "DeleteVirtualClusterRequestRequestTypeDef",
+    "DeleteVirtualClusterResponseTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
     "DescribeManagedEndpointRequestRequestTypeDef",
     "DescribeVirtualClusterRequestRequestTypeDef",
+    "GetManagedEndpointSessionCredentialsRequestRequestTypeDef",
     "SparkSqlJobDriverTypeDef",
     "SparkSubmitJobDriverTypeDef",
     "RetryPolicyConfigurationTypeDef",
     "RetryPolicyExecutionTypeDef",
     "TemplateParameterConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
+    "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     "ListManagedEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     "ListVirtualClustersRequestRequestTypeDef",
     "S3MonitoringConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
     "ParametricCloudWatchMonitoringConfigurationTypeDef",
     "ParametricS3MonitoringConfigurationTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartJobRunResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "CancelJobRunResponseTypeDef",
-    "CreateJobTemplateResponseTypeDef",
-    "CreateManagedEndpointResponseTypeDef",
-    "CreateVirtualClusterResponseTypeDef",
-    "DeleteJobTemplateResponseTypeDef",
-    "DeleteManagedEndpointResponseTypeDef",
-    "DeleteVirtualClusterResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartJobRunResponseTypeDef",
     "ContainerInfoTypeDef",
+    "GetManagedEndpointSessionCredentialsResponseTypeDef",
     "JobDriverTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
-    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParametricMonitoringConfigurationTypeDef",
     "ContainerProviderTypeDef",
     "ConfigurationOverridesTypeDef",
     "ParametricConfigurationOverridesTypeDef",
     "CreateVirtualClusterRequestRequestTypeDef",
     "VirtualClusterTypeDef",
@@ -107,22 +111,20 @@
     "CancelJobRunRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
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
+        "id": str,
+        "virtualClusterId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "certificateArn": str,
@@ -177,36 +179,109 @@
     "EksInfoTypeDef",
     {
         "namespace": str,
     },
     total=False,
 )
 
+ContainerLogRotationConfigurationTypeDef = TypedDict(
+    "ContainerLogRotationConfigurationTypeDef",
+    {
+        "rotationSize": str,
+        "maxFilesToKeep": int,
+    },
+)
+
+CreateJobTemplateResponseTypeDef = TypedDict(
+    "CreateJobTemplateResponseTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "arn": str,
+        "createdAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateManagedEndpointResponseTypeDef = TypedDict(
+    "CreateManagedEndpointResponseTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "arn": str,
+        "virtualClusterId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateVirtualClusterResponseTypeDef = TypedDict(
+    "CreateVirtualClusterResponseTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CredentialsTypeDef = TypedDict(
+    "CredentialsTypeDef",
+    {
+        "token": str,
+    },
+    total=False,
+)
+
 DeleteJobTemplateRequestRequestTypeDef = TypedDict(
     "DeleteJobTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+DeleteJobTemplateResponseTypeDef = TypedDict(
+    "DeleteJobTemplateResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteManagedEndpointRequestRequestTypeDef = TypedDict(
     "DeleteManagedEndpointRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
     },
 )
 
+DeleteManagedEndpointResponseTypeDef = TypedDict(
+    "DeleteManagedEndpointResponseTypeDef",
+    {
+        "id": str,
+        "virtualClusterId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteVirtualClusterRequestRequestTypeDef = TypedDict(
     "DeleteVirtualClusterRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+DeleteVirtualClusterResponseTypeDef = TypedDict(
+    "DeleteVirtualClusterResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeJobRunRequestRequestTypeDef = TypedDict(
     "DescribeJobRunRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
     },
 )
@@ -229,14 +304,41 @@
 DescribeVirtualClusterRequestRequestTypeDef = TypedDict(
     "DescribeVirtualClusterRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+_RequiredGetManagedEndpointSessionCredentialsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetManagedEndpointSessionCredentialsRequestRequestTypeDef",
+    {
+        "endpointIdentifier": str,
+        "virtualClusterIdentifier": str,
+        "executionRoleArn": str,
+        "credentialType": str,
+    },
+)
+_OptionalGetManagedEndpointSessionCredentialsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetManagedEndpointSessionCredentialsRequestRequestTypeDef",
+    {
+        "durationInSeconds": int,
+        "logContext": str,
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class GetManagedEndpointSessionCredentialsRequestRequestTypeDef(
+    _RequiredGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
+    _OptionalGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
+):
+    pass
+
+
 SparkSqlJobDriverTypeDef = TypedDict(
     "SparkSqlJobDriverTypeDef",
     {
         "entryPoint": str,
         "sparkSqlParameters": str,
     },
     total=False,
@@ -283,24 +385,40 @@
     {
         "type": TemplateParameterDataTypeType,
         "defaultValue": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "virtualClusterId": str,
+    },
+)
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "createdBefore": Union[datetime, str],
+        "createdAfter": Union[datetime, str],
+        "name": str,
+        "states": Sequence[JobRunStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
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
         "virtualClusterId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -319,25 +437,61 @@
 
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
 
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    {
+        "createdAfter": Union[datetime, str],
+        "createdBefore": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
+    "_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
+    {
+        "virtualClusterId": str,
+    },
+)
+_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
+    "_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
+    {
+        "createdBefore": Union[datetime, str],
+        "createdAfter": Union[datetime, str],
+        "types": Sequence[str],
+        "states": Sequence[EndpointStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
+    _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
+    _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListManagedEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListManagedEndpointsRequestRequestTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListManagedEndpointsRequestRequestTypeDef = TypedDict(
@@ -364,14 +518,35 @@
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
+ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
+    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
+    {
+        "containerProviderId": str,
+        "containerProviderType": Literal["EKS"],
+        "createdAfter": Union[datetime, str],
+        "createdBefore": Union[datetime, str],
+        "states": Sequence[VirtualClusterStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListVirtualClustersRequestRequestTypeDef = TypedDict(
     "ListVirtualClustersRequestRequestTypeDef",
     {
         "containerProviderId": str,
         "containerProviderType": Literal["EKS"],
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
@@ -385,14 +560,24 @@
 S3MonitoringConfigurationTypeDef = TypedDict(
     "S3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
     },
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
 ParametricCloudWatchMonitoringConfigurationTypeDef = TypedDict(
     "ParametricCloudWatchMonitoringConfigurationTypeDef",
     {
         "logGroupName": str,
         "logStreamNamePrefix": str,
     },
     total=False,
@@ -402,213 +587,86 @@
     "ParametricS3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
     },
     total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Mapping[str, str],
-    },
-)
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
-    },
-)
-
-CancelJobRunResponseTypeDef = TypedDict(
-    "CancelJobRunResponseTypeDef",
-    {
-        "id": str,
-        "virtualClusterId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobTemplateResponseTypeDef = TypedDict(
-    "CreateJobTemplateResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "id": str,
-        "name": str,
-        "arn": str,
-        "createdAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-CreateManagedEndpointResponseTypeDef = TypedDict(
-    "CreateManagedEndpointResponseTypeDef",
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "virtualClusterId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateVirtualClusterResponseTypeDef = TypedDict(
-    "CreateVirtualClusterResponseTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteJobTemplateResponseTypeDef = TypedDict(
-    "DeleteJobTemplateResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteManagedEndpointResponseTypeDef = TypedDict(
-    "DeleteManagedEndpointResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "id": str,
-        "virtualClusterId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tags": Mapping[str, str],
     },
 )
 
-DeleteVirtualClusterResponseTypeDef = TypedDict(
-    "DeleteVirtualClusterResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ContainerInfoTypeDef = TypedDict(
+    "ContainerInfoTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "eksInfo": EksInfoTypeDef,
     },
+    total=False,
 )
 
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
+GetManagedEndpointSessionCredentialsResponseTypeDef = TypedDict(
+    "GetManagedEndpointSessionCredentialsResponseTypeDef",
     {
         "id": str,
-        "name": str,
-        "arn": str,
-        "virtualClusterId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "credentials": CredentialsTypeDef,
+        "expiresAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ContainerInfoTypeDef = TypedDict(
-    "ContainerInfoTypeDef",
-    {
-        "eksInfo": EksInfoTypeDef,
-    },
-    total=False,
-)
-
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmitJobDriver": SparkSubmitJobDriverTypeDef,
         "sparkSqlJobDriver": SparkSqlJobDriverTypeDef,
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "virtualClusterId": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
-        "name": str,
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
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
-    "_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
-    {
-        "virtualClusterId": str,
-    },
-)
-_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
-    "_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
-    {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
-        "types": Sequence[str],
-        "states": Sequence[EndpointStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
-    _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
-    _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
-):
-    pass
-
-
-ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
-    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
-    {
-        "containerProviderId": str,
-        "containerProviderType": Literal["EKS"],
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "states": Sequence[VirtualClusterStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "persistentAppUI": PersistentAppUIType,
         "cloudWatchMonitoringConfiguration": CloudWatchMonitoringConfigurationTypeDef,
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
+        "containerLogRotationConfiguration": ContainerLogRotationConfigurationTypeDef,
     },
     total=False,
 )
 
 ParametricMonitoringConfigurationTypeDef = TypedDict(
     "ParametricMonitoringConfigurationTypeDef",
     {
@@ -829,58 +887,58 @@
     pass
 
 
 DescribeVirtualClusterResponseTypeDef = TypedDict(
     "DescribeVirtualClusterResponseTypeDef",
     {
         "virtualCluster": VirtualClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVirtualClustersResponseTypeDef = TypedDict(
     "ListVirtualClustersResponseTypeDef",
     {
         "virtualClusters": List[VirtualClusterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeManagedEndpointResponseTypeDef = TypedDict(
     "DescribeManagedEndpointResponseTypeDef",
     {
         "endpoint": EndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListManagedEndpointsResponseTypeDef = TypedDict(
     "ListManagedEndpointsResponseTypeDef",
     {
         "endpoints": List[EndpointTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeJobRunResponseTypeDef = TypedDict(
     "DescribeJobRunResponseTypeDef",
     {
         "jobRun": JobRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "jobRuns": List[JobRunTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobTemplateRequestRequestTypeDef",
     {
         "name": str,
@@ -930,19 +988,19 @@
     pass
 
 
 DescribeJobTemplateResponseTypeDef = TypedDict(
     "DescribeJobTemplateResponseTypeDef",
     {
         "jobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "templates": List[JobTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers/type_defs.pyi` & `mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -31,57 +31,61 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelJobRunRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelJobRunResponseTypeDef",
     "CertificateTypeDef",
     "CloudWatchMonitoringConfigurationTypeDef",
     "ConfigurationTypeDef",
     "EksInfoTypeDef",
+    "ContainerLogRotationConfigurationTypeDef",
+    "CreateJobTemplateResponseTypeDef",
+    "CreateManagedEndpointResponseTypeDef",
+    "CreateVirtualClusterResponseTypeDef",
+    "CredentialsTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
+    "DeleteJobTemplateResponseTypeDef",
     "DeleteManagedEndpointRequestRequestTypeDef",
+    "DeleteManagedEndpointResponseTypeDef",
     "DeleteVirtualClusterRequestRequestTypeDef",
+    "DeleteVirtualClusterResponseTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
     "DescribeManagedEndpointRequestRequestTypeDef",
     "DescribeVirtualClusterRequestRequestTypeDef",
+    "GetManagedEndpointSessionCredentialsRequestRequestTypeDef",
     "SparkSqlJobDriverTypeDef",
     "SparkSubmitJobDriverTypeDef",
     "RetryPolicyConfigurationTypeDef",
     "RetryPolicyExecutionTypeDef",
     "TemplateParameterConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
+    "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     "ListManagedEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     "ListVirtualClustersRequestRequestTypeDef",
     "S3MonitoringConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
     "ParametricCloudWatchMonitoringConfigurationTypeDef",
     "ParametricS3MonitoringConfigurationTypeDef",
+    "ResponseMetadataTypeDef",
+    "StartJobRunResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "CancelJobRunResponseTypeDef",
-    "CreateJobTemplateResponseTypeDef",
-    "CreateManagedEndpointResponseTypeDef",
-    "CreateVirtualClusterResponseTypeDef",
-    "DeleteJobTemplateResponseTypeDef",
-    "DeleteManagedEndpointResponseTypeDef",
-    "DeleteVirtualClusterResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartJobRunResponseTypeDef",
     "ContainerInfoTypeDef",
+    "GetManagedEndpointSessionCredentialsResponseTypeDef",
     "JobDriverTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
-    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParametricMonitoringConfigurationTypeDef",
     "ContainerProviderTypeDef",
     "ConfigurationOverridesTypeDef",
     "ParametricConfigurationOverridesTypeDef",
     "CreateVirtualClusterRequestRequestTypeDef",
     "VirtualClusterTypeDef",
@@ -106,22 +110,20 @@
     "CancelJobRunRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
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
+        "id": str,
+        "virtualClusterId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "certificateArn": str,
@@ -172,36 +174,109 @@
     "EksInfoTypeDef",
     {
         "namespace": str,
     },
     total=False,
 )
 
+ContainerLogRotationConfigurationTypeDef = TypedDict(
+    "ContainerLogRotationConfigurationTypeDef",
+    {
+        "rotationSize": str,
+        "maxFilesToKeep": int,
+    },
+)
+
+CreateJobTemplateResponseTypeDef = TypedDict(
+    "CreateJobTemplateResponseTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "arn": str,
+        "createdAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateManagedEndpointResponseTypeDef = TypedDict(
+    "CreateManagedEndpointResponseTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "arn": str,
+        "virtualClusterId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateVirtualClusterResponseTypeDef = TypedDict(
+    "CreateVirtualClusterResponseTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CredentialsTypeDef = TypedDict(
+    "CredentialsTypeDef",
+    {
+        "token": str,
+    },
+    total=False,
+)
+
 DeleteJobTemplateRequestRequestTypeDef = TypedDict(
     "DeleteJobTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+DeleteJobTemplateResponseTypeDef = TypedDict(
+    "DeleteJobTemplateResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteManagedEndpointRequestRequestTypeDef = TypedDict(
     "DeleteManagedEndpointRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
     },
 )
 
+DeleteManagedEndpointResponseTypeDef = TypedDict(
+    "DeleteManagedEndpointResponseTypeDef",
+    {
+        "id": str,
+        "virtualClusterId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteVirtualClusterRequestRequestTypeDef = TypedDict(
     "DeleteVirtualClusterRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+DeleteVirtualClusterResponseTypeDef = TypedDict(
+    "DeleteVirtualClusterResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeJobRunRequestRequestTypeDef = TypedDict(
     "DescribeJobRunRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
     },
 )
@@ -224,14 +299,39 @@
 DescribeVirtualClusterRequestRequestTypeDef = TypedDict(
     "DescribeVirtualClusterRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+_RequiredGetManagedEndpointSessionCredentialsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetManagedEndpointSessionCredentialsRequestRequestTypeDef",
+    {
+        "endpointIdentifier": str,
+        "virtualClusterIdentifier": str,
+        "executionRoleArn": str,
+        "credentialType": str,
+    },
+)
+_OptionalGetManagedEndpointSessionCredentialsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetManagedEndpointSessionCredentialsRequestRequestTypeDef",
+    {
+        "durationInSeconds": int,
+        "logContext": str,
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class GetManagedEndpointSessionCredentialsRequestRequestTypeDef(
+    _RequiredGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
+    _OptionalGetManagedEndpointSessionCredentialsRequestRequestTypeDef,
+):
+    pass
+
 SparkSqlJobDriverTypeDef = TypedDict(
     "SparkSqlJobDriverTypeDef",
     {
         "entryPoint": str,
         "sparkSqlParameters": str,
     },
     total=False,
@@ -276,24 +376,38 @@
     {
         "type": TemplateParameterDataTypeType,
         "defaultValue": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "virtualClusterId": str,
+    },
+)
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "createdBefore": Union[datetime, str],
+        "createdAfter": Union[datetime, str],
+        "name": str,
+        "states": Sequence[JobRunStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListJobRunsRequestListJobRunsPaginateTypeDef(
+    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
+    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
+):
+    pass
+
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -310,25 +424,59 @@
 )
 
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    {
+        "createdAfter": Union[datetime, str],
+        "createdBefore": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
+    "_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
+    {
+        "virtualClusterId": str,
+    },
+)
+_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
+    "_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
+    {
+        "createdBefore": Union[datetime, str],
+        "createdAfter": Union[datetime, str],
+        "types": Sequence[str],
+        "states": Sequence[EndpointStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
+    _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
+    _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
+):
+    pass
+
 _RequiredListManagedEndpointsRequestRequestTypeDef = TypedDict(
     "_RequiredListManagedEndpointsRequestRequestTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListManagedEndpointsRequestRequestTypeDef = TypedDict(
@@ -353,14 +501,35 @@
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
+ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
+    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
+    {
+        "containerProviderId": str,
+        "containerProviderType": Literal["EKS"],
+        "createdAfter": Union[datetime, str],
+        "createdBefore": Union[datetime, str],
+        "states": Sequence[VirtualClusterStateType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListVirtualClustersRequestRequestTypeDef = TypedDict(
     "ListVirtualClustersRequestRequestTypeDef",
     {
         "containerProviderId": str,
         "containerProviderType": Literal["EKS"],
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
@@ -374,14 +543,24 @@
 S3MonitoringConfigurationTypeDef = TypedDict(
     "S3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
     },
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
 ParametricCloudWatchMonitoringConfigurationTypeDef = TypedDict(
     "ParametricCloudWatchMonitoringConfigurationTypeDef",
     {
         "logGroupName": str,
         "logStreamNamePrefix": str,
     },
     total=False,
@@ -391,209 +570,86 @@
     "ParametricS3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
     },
     total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Mapping[str, str],
-    },
-)
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
-    },
-)
-
-CancelJobRunResponseTypeDef = TypedDict(
-    "CancelJobRunResponseTypeDef",
-    {
-        "id": str,
-        "virtualClusterId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobTemplateResponseTypeDef = TypedDict(
-    "CreateJobTemplateResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "id": str,
-        "name": str,
-        "arn": str,
-        "createdAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-CreateManagedEndpointResponseTypeDef = TypedDict(
-    "CreateManagedEndpointResponseTypeDef",
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "virtualClusterId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateVirtualClusterResponseTypeDef = TypedDict(
-    "CreateVirtualClusterResponseTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteJobTemplateResponseTypeDef = TypedDict(
-    "DeleteJobTemplateResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteManagedEndpointResponseTypeDef = TypedDict(
-    "DeleteManagedEndpointResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "id": str,
-        "virtualClusterId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tags": Mapping[str, str],
     },
 )
 
-DeleteVirtualClusterResponseTypeDef = TypedDict(
-    "DeleteVirtualClusterResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ContainerInfoTypeDef = TypedDict(
+    "ContainerInfoTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "eksInfo": EksInfoTypeDef,
     },
+    total=False,
 )
 
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
+GetManagedEndpointSessionCredentialsResponseTypeDef = TypedDict(
+    "GetManagedEndpointSessionCredentialsResponseTypeDef",
     {
         "id": str,
-        "name": str,
-        "arn": str,
-        "virtualClusterId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "credentials": CredentialsTypeDef,
+        "expiresAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ContainerInfoTypeDef = TypedDict(
-    "ContainerInfoTypeDef",
-    {
-        "eksInfo": EksInfoTypeDef,
-    },
-    total=False,
-)
-
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmitJobDriver": SparkSubmitJobDriverTypeDef,
         "sparkSqlJobDriver": SparkSqlJobDriverTypeDef,
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "virtualClusterId": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
-        "name": str,
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
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
-    "_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
-    {
-        "virtualClusterId": str,
-    },
-)
-_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
-    "_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
-    {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
-        "types": Sequence[str],
-        "states": Sequence[EndpointStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
-    _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
-    _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
-):
-    pass
-
-ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
-    "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
-    {
-        "containerProviderId": str,
-        "containerProviderType": Literal["EKS"],
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "states": Sequence[VirtualClusterStateType],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "persistentAppUI": PersistentAppUIType,
         "cloudWatchMonitoringConfiguration": CloudWatchMonitoringConfigurationTypeDef,
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
+        "containerLogRotationConfiguration": ContainerLogRotationConfigurationTypeDef,
     },
     total=False,
 )
 
 ParametricMonitoringConfigurationTypeDef = TypedDict(
     "ParametricMonitoringConfigurationTypeDef",
     {
@@ -804,58 +860,58 @@
 class JobTemplateDataTypeDef(_RequiredJobTemplateDataTypeDef, _OptionalJobTemplateDataTypeDef):
     pass
 
 DescribeVirtualClusterResponseTypeDef = TypedDict(
     "DescribeVirtualClusterResponseTypeDef",
     {
         "virtualCluster": VirtualClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVirtualClustersResponseTypeDef = TypedDict(
     "ListVirtualClustersResponseTypeDef",
     {
         "virtualClusters": List[VirtualClusterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeManagedEndpointResponseTypeDef = TypedDict(
     "DescribeManagedEndpointResponseTypeDef",
     {
         "endpoint": EndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListManagedEndpointsResponseTypeDef = TypedDict(
     "ListManagedEndpointsResponseTypeDef",
     {
         "endpoints": List[EndpointTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeJobRunResponseTypeDef = TypedDict(
     "DescribeJobRunResponseTypeDef",
     {
         "jobRun": JobRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "jobRuns": List[JobRunTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobTemplateRequestRequestTypeDef",
     {
         "name": str,
@@ -901,19 +957,19 @@
 class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
     pass
 
 DescribeJobTemplateResponseTypeDef = TypedDict(
     "DescribeJobTemplateResponseTypeDef",
     {
         "jobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "templates": List[JobTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/PKG-INFO` & `mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-containers
-Version: 1.26.68
-Summary: Type annotations for boto3.EMRContainers 1.26.68 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.EMRContainers 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-emr-containers"></a>
 
 # mypy-boto3-emr-containers
 
 [![PyPI - mypy-boto3-emr-containers](https://img.shields.io/pypi/v/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-containers?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.26.68](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
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
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,57 +343,61 @@
 
 `mypy_boto3_emr_containers.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_containers.type_defs import (
     CancelJobRunRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelJobRunResponseTypeDef,
     CertificateTypeDef,
     CloudWatchMonitoringConfigurationTypeDef,
     ConfigurationTypeDef,
     EksInfoTypeDef,
+    ContainerLogRotationConfigurationTypeDef,
+    CreateJobTemplateResponseTypeDef,
+    CreateManagedEndpointResponseTypeDef,
+    CreateVirtualClusterResponseTypeDef,
+    CredentialsTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
+    DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointRequestRequestTypeDef,
+    DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterRequestRequestTypeDef,
+    DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
     DescribeManagedEndpointRequestRequestTypeDef,
     DescribeVirtualClusterRequestRequestTypeDef,
+    GetManagedEndpointSessionCredentialsRequestRequestTypeDef,
     SparkSqlJobDriverTypeDef,
     SparkSubmitJobDriverTypeDef,
     RetryPolicyConfigurationTypeDef,
     RetryPolicyExecutionTypeDef,
     TemplateParameterConfigurationTypeDef,
-    PaginatorConfigTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
+    ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     ListManagedEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
     ListVirtualClustersRequestRequestTypeDef,
     S3MonitoringConfigurationTypeDef,
+    PaginatorConfigTypeDef,
     ParametricCloudWatchMonitoringConfigurationTypeDef,
     ParametricS3MonitoringConfigurationTypeDef,
+    ResponseMetadataTypeDef,
+    StartJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
-    CreateJobTemplateResponseTypeDef,
-    CreateManagedEndpointResponseTypeDef,
-    CreateVirtualClusterResponseTypeDef,
-    DeleteJobTemplateResponseTypeDef,
-    DeleteManagedEndpointResponseTypeDef,
-    DeleteVirtualClusterResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartJobRunResponseTypeDef,
     ContainerInfoTypeDef,
+    GetManagedEndpointSessionCredentialsResponseTypeDef,
     JobDriverTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
-    ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
-    ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
     MonitoringConfigurationTypeDef,
     ParametricMonitoringConfigurationTypeDef,
     ContainerProviderTypeDef,
     ConfigurationOverridesTypeDef,
     ParametricConfigurationOverridesTypeDef,
     CreateVirtualClusterRequestRequestTypeDef,
     VirtualClusterTypeDef,
@@ -422,42 +426,42 @@
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

### Comparing `mypy-boto3-emr-containers-1.26.68/mypy_boto3_emr_containers.egg-info/SOURCES.txt` & `mypy-boto3-emr-containers-1.27.0/mypy_boto3_emr_containers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.26.68/setup.py` & `mypy-boto3-emr-containers-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-emr-containers.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr-containers",
-    version="1.26.68",
+    version="1.27.0",
     packages=["mypy_boto3_emr_containers"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMRContainers 1.26.68 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.EMRContainers 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/",
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


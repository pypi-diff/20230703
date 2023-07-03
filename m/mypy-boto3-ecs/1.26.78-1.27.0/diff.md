# Comparing `tmp/mypy-boto3-ecs-1.26.78.tar.gz` & `tmp/mypy-boto3-ecs-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecs-1.26.78.tar", last modified: Thu Feb 23 20:34:57 2023, max compression
+gzip compressed data, was "mypy-boto3-ecs-1.27.0.tar", last modified: Mon Jul  3 19:50:43 2023, max compression
```

## Comparing `mypy-boto3-ecs-1.26.78.tar` & `mypy-boto3-ecs-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.324421 mypy-boto3-ecs-1.26.78/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24442 2023-02-23 20:34:57.324421 mypy-boto3-ecs-1.26.78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22971 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.320421 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49990 2023-02-23 20:34:24.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49914 2023-02-23 20:34:24.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15403 2023-02-23 20:34:25.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-02-23 20:34:25.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-02-23 20:34:24.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-02-23 20:34:24.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    85416 2023-02-23 20:34:27.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85315 2023-02-23 20:34:25.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-02-23 20:34:24.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-02-23 20:34:24.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.324421 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24442 2023-02-23 20:34:57.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-02-23 20:34:57.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 20:34:57.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-23 20:34:57.000000 mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 20:34:57.324421 mypy-boto3-ecs-1.26.78/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-23 20:34:23.000000 mypy-boto3-ecs-1.26.78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.123190 mypy-boto3-ecs-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:00.000000 mypy-boto3-ecs-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24414 2023-07-03 19:50:43.123190 mypy-boto3-ecs-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22945 2023-07-03 19:37:00.000000 mypy-boto3-ecs-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.115190 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-03 19:37:00.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-03 19:37:00.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:37:00.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49990 2023-07-03 19:37:02.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49914 2023-07-03 19:37:02.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-07-03 19:37:02.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15682 2023-07-03 19:37:02.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-07-03 19:37:02.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-07-03 19:37:02.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:00.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    85580 2023-07-03 19:37:04.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85479 2023-07-03 19:37:03.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:00.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-03 19:37:02.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-03 19:37:02.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:43.123190 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24414 2023-07-03 19:50:42.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 19:50:42.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:42.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:42.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:42.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:42.000000 mypy-boto3-ecs-1.27.0/mypy_boto3_ecs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:43.123190 mypy-boto3-ecs-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:37:00.000000 mypy-boto3-ecs-1.27.0/setup.py
```

### Comparing `mypy-boto3-ecs-1.26.78/LICENSE` & `mypy-boto3-ecs-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-ecs-1.26.78/PKG-INFO` & `mypy-boto3-ecs-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecs
-Version: 1.26.78
-Summary: Type annotations for boto3.ECS 1.26.78 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.ECS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ecs"></a>
 
 # mypy-boto3-ecs
 
 [![PyPI - mypy-boto3-ecs](https://img.shields.io/pypi/v/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecs?color=blue)](https://pypistats.org/packages/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -473,15 +473,14 @@
     VolumeFromTypeDef,
     InstanceHealthCheckResultTypeDef,
     ResourceTypeDef,
     VersionInfoTypeDef,
     NetworkBindingTypeDef,
     ManagedAgentTypeDef,
     NetworkInterfaceTypeDef,
-    ResponseMetadataTypeDef,
     DeploymentControllerTypeDef,
     LoadBalancerTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     ServiceRegistryTypeDef,
     ScaleTypeDef,
     DeleteAccountSettingRequestRequestTypeDef,
@@ -503,85 +502,95 @@
     DescribeServicesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTaskDefinitionRequestRequestTypeDef,
     DescribeTaskSetsRequestRequestTypeDef,
     DescribeTasksRequestRequestTypeDef,
     DeviceTypeDef,
     DiscoverPollEndpointRequestRequestTypeDef,
+    DiscoverPollEndpointResponseTypeDef,
     DockerVolumeConfigurationTypeDef,
     EFSAuthorizationConfigTypeDef,
     EphemeralStorageTypeDef,
     ExecuteCommandLogConfigurationTypeDef,
     ExecuteCommandRequestRequestTypeDef,
     SessionTypeDef,
     FSxWindowsFileServerAuthorizationConfigTypeDef,
     GetTaskProtectionRequestRequestTypeDef,
     ProtectedTaskTypeDef,
     HostVolumePropertiesTypeDef,
     InferenceAcceleratorOverrideTypeDef,
     InferenceAcceleratorTypeDef,
     KernelCapabilitiesTypeDef,
     TmpfsTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
     ListAccountSettingsRequestRequestTypeDef,
+    ListAttributesRequestListAttributesPaginateTypeDef,
     ListAttributesRequestRequestTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListClustersResponseTypeDef,
+    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
     ListContainerInstancesRequestRequestTypeDef,
+    ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     ListServicesByNamespaceRequestRequestTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
+    ListServicesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
     ListTaskDefinitionFamiliesRequestRequestTypeDef,
+    ListTaskDefinitionFamiliesResponseTypeDef,
+    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
+    ListTaskDefinitionsResponseTypeDef,
+    ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
+    ListTasksResponseTypeDef,
     ManagedAgentStateChangeTypeDef,
+    PaginatorConfigTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
+    ResponseMetadataTypeDef,
     ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
     StopTaskRequestRequestTypeDef,
+    SubmitAttachmentStateChangesResponseTypeDef,
+    SubmitContainerStateChangeResponseTypeDef,
+    SubmitTaskStateChangeResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
     SubmitAttachmentStateChangesRequestRequestTypeDef,
     AttachmentTypeDef,
     ProxyConfigurationTypeDef,
     DeleteAttributesRequestRequestTypeDef,
+    DeleteAttributesResponseTypeDef,
+    ListAttributesResponseTypeDef,
     PutAttributesRequestRequestTypeDef,
+    PutAttributesResponseTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     NetworkConfigurationTypeDef,
     PutClusterCapacityProvidersRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UpdateClusterSettingsRequestRequestTypeDef,
     ContainerOverrideTypeDef,
     LogConfigurationTypeDef,
     ContainerInstanceHealthStatusTypeDef,
     ContainerStateChangeTypeDef,
     SubmitContainerStateChangeRequestRequestTypeDef,
     ContainerTypeDef,
-    DeleteAttributesResponseTypeDef,
-    DiscoverPollEndpointResponseTypeDef,
-    ListAttributesResponseTypeDef,
-    ListClustersResponseTypeDef,
-    ListContainerInstancesResponseTypeDef,
-    ListServicesByNamespaceResponseTypeDef,
-    ListServicesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTaskDefinitionFamiliesResponseTypeDef,
-    ListTaskDefinitionsResponseTypeDef,
-    ListTasksResponseTypeDef,
-    PutAttributesResponseTypeDef,
-    SubmitAttachmentStateChangesResponseTypeDef,
-    SubmitContainerStateChangeResponseTypeDef,
-    SubmitTaskStateChangeResponseTypeDef,
     UpdateTaskSetRequestRequestTypeDef,
     DeleteAccountSettingResponseTypeDef,
     ListAccountSettingsResponseTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
     DeploymentConfigurationTypeDef,
     DescribeServicesRequestServicesInactiveWaitTypeDef,
@@ -591,23 +600,14 @@
     EFSVolumeConfigurationTypeDef,
     ExecuteCommandConfigurationTypeDef,
     ExecuteCommandResponseTypeDef,
     FSxWindowsFileServerVolumeConfigurationTypeDef,
     GetTaskProtectionResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     LinuxParametersTypeDef,
-    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
-    ListAttributesRequestListAttributesPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
-    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
-    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
-    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
-    ListTasksRequestListTasksPaginateTypeDef,
     RegisterContainerInstanceRequestRequestTypeDef,
     ServiceConnectServiceTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
     CreateTaskSetRequestRequestTypeDef,
     TaskSetTypeDef,
@@ -672,42 +672,42 @@
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

### Comparing `mypy-boto3-ecs-1.26.78/README.md` & `mypy-boto3-ecs-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ecs"></a>
 
 # mypy-boto3-ecs
 
 [![PyPI - mypy-boto3-ecs](https://img.shields.io/pypi/v/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecs?color=blue)](https://pypistats.org/packages/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -441,15 +441,14 @@
     VolumeFromTypeDef,
     InstanceHealthCheckResultTypeDef,
     ResourceTypeDef,
     VersionInfoTypeDef,
     NetworkBindingTypeDef,
     ManagedAgentTypeDef,
     NetworkInterfaceTypeDef,
-    ResponseMetadataTypeDef,
     DeploymentControllerTypeDef,
     LoadBalancerTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     ServiceRegistryTypeDef,
     ScaleTypeDef,
     DeleteAccountSettingRequestRequestTypeDef,
@@ -471,85 +470,95 @@
     DescribeServicesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTaskDefinitionRequestRequestTypeDef,
     DescribeTaskSetsRequestRequestTypeDef,
     DescribeTasksRequestRequestTypeDef,
     DeviceTypeDef,
     DiscoverPollEndpointRequestRequestTypeDef,
+    DiscoverPollEndpointResponseTypeDef,
     DockerVolumeConfigurationTypeDef,
     EFSAuthorizationConfigTypeDef,
     EphemeralStorageTypeDef,
     ExecuteCommandLogConfigurationTypeDef,
     ExecuteCommandRequestRequestTypeDef,
     SessionTypeDef,
     FSxWindowsFileServerAuthorizationConfigTypeDef,
     GetTaskProtectionRequestRequestTypeDef,
     ProtectedTaskTypeDef,
     HostVolumePropertiesTypeDef,
     InferenceAcceleratorOverrideTypeDef,
     InferenceAcceleratorTypeDef,
     KernelCapabilitiesTypeDef,
     TmpfsTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
     ListAccountSettingsRequestRequestTypeDef,
+    ListAttributesRequestListAttributesPaginateTypeDef,
     ListAttributesRequestRequestTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListClustersResponseTypeDef,
+    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
     ListContainerInstancesRequestRequestTypeDef,
+    ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     ListServicesByNamespaceRequestRequestTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
+    ListServicesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
     ListTaskDefinitionFamiliesRequestRequestTypeDef,
+    ListTaskDefinitionFamiliesResponseTypeDef,
+    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
+    ListTaskDefinitionsResponseTypeDef,
+    ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
+    ListTasksResponseTypeDef,
     ManagedAgentStateChangeTypeDef,
+    PaginatorConfigTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
+    ResponseMetadataTypeDef,
     ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
     StopTaskRequestRequestTypeDef,
+    SubmitAttachmentStateChangesResponseTypeDef,
+    SubmitContainerStateChangeResponseTypeDef,
+    SubmitTaskStateChangeResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
     SubmitAttachmentStateChangesRequestRequestTypeDef,
     AttachmentTypeDef,
     ProxyConfigurationTypeDef,
     DeleteAttributesRequestRequestTypeDef,
+    DeleteAttributesResponseTypeDef,
+    ListAttributesResponseTypeDef,
     PutAttributesRequestRequestTypeDef,
+    PutAttributesResponseTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     NetworkConfigurationTypeDef,
     PutClusterCapacityProvidersRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UpdateClusterSettingsRequestRequestTypeDef,
     ContainerOverrideTypeDef,
     LogConfigurationTypeDef,
     ContainerInstanceHealthStatusTypeDef,
     ContainerStateChangeTypeDef,
     SubmitContainerStateChangeRequestRequestTypeDef,
     ContainerTypeDef,
-    DeleteAttributesResponseTypeDef,
-    DiscoverPollEndpointResponseTypeDef,
-    ListAttributesResponseTypeDef,
-    ListClustersResponseTypeDef,
-    ListContainerInstancesResponseTypeDef,
-    ListServicesByNamespaceResponseTypeDef,
-    ListServicesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTaskDefinitionFamiliesResponseTypeDef,
-    ListTaskDefinitionsResponseTypeDef,
-    ListTasksResponseTypeDef,
-    PutAttributesResponseTypeDef,
-    SubmitAttachmentStateChangesResponseTypeDef,
-    SubmitContainerStateChangeResponseTypeDef,
-    SubmitTaskStateChangeResponseTypeDef,
     UpdateTaskSetRequestRequestTypeDef,
     DeleteAccountSettingResponseTypeDef,
     ListAccountSettingsResponseTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
     DeploymentConfigurationTypeDef,
     DescribeServicesRequestServicesInactiveWaitTypeDef,
@@ -559,23 +568,14 @@
     EFSVolumeConfigurationTypeDef,
     ExecuteCommandConfigurationTypeDef,
     ExecuteCommandResponseTypeDef,
     FSxWindowsFileServerVolumeConfigurationTypeDef,
     GetTaskProtectionResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     LinuxParametersTypeDef,
-    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
-    ListAttributesRequestListAttributesPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
-    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
-    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
-    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
-    ListTasksRequestListTasksPaginateTypeDef,
     RegisterContainerInstanceRequestRequestTypeDef,
     ServiceConnectServiceTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
     CreateTaskSetRequestRequestTypeDef,
     TaskSetTypeDef,
@@ -640,42 +640,42 @@
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

### Comparing `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/__init__.py` & `mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/__init__.pyi` & `mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/__main__.py` & `mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECS 1.26.78\nVersion:         1.26.78\nBuilder version:"
-        " 7.12.4\nDocs:           "
+        "Type annotations for boto3.ECS 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.78")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/client.py` & `mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/client.pyi` & `mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/literals.py` & `mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,17 @@
 ServiceFieldType = Literal["TAGS"]
 ServicesInactiveWaiterName = Literal["services_inactive"]
 ServicesStableWaiterName = Literal["services_stable"]
 SettingNameType = Literal[
     "awsvpcTrunking",
     "containerInsights",
     "containerInstanceLongArnFormat",
+    "fargateFIPSMode",
     "serviceLongArnFormat",
+    "tagResourceAuthorization",
     "taskLongArnFormat",
 ]
 SortOrderType = Literal["ASC", "DESC"]
 StabilityStatusType = Literal["STABILIZING", "STEADY_STATE"]
 TargetTypeType = Literal["container-instance"]
 TaskDefinitionFamilyStatusType = Literal["ACTIVE", "ALL", "INACTIVE"]
 TaskDefinitionFieldType = Literal["TAGS"]
@@ -232,14 +234,15 @@
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
@@ -279,14 +282,15 @@
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
@@ -365,14 +369,15 @@
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
@@ -383,14 +388,15 @@
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
@@ -426,14 +432,15 @@
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
@@ -452,16 +459,19 @@
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
@@ -545,15 +555,17 @@
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

### Comparing `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/literals.pyi` & `mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,17 @@
 ServiceFieldType = Literal["TAGS"]
 ServicesInactiveWaiterName = Literal["services_inactive"]
 ServicesStableWaiterName = Literal["services_stable"]
 SettingNameType = Literal[
     "awsvpcTrunking",
     "containerInsights",
     "containerInstanceLongArnFormat",
+    "fargateFIPSMode",
     "serviceLongArnFormat",
+    "tagResourceAuthorization",
     "taskLongArnFormat",
 ]
 SortOrderType = Literal["ASC", "DESC"]
 StabilityStatusType = Literal["STABILIZING", "STEADY_STATE"]
 TargetTypeType = Literal["container-instance"]
 TaskDefinitionFamilyStatusType = Literal["ACTIVE", "ALL", "INACTIVE"]
 TaskDefinitionFieldType = Literal["TAGS"]
@@ -230,14 +232,15 @@
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
@@ -277,14 +280,15 @@
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
@@ -363,14 +367,15 @@
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
@@ -381,14 +386,15 @@
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
@@ -424,14 +430,15 @@
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
@@ -450,16 +457,19 @@
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
@@ -543,15 +553,17 @@
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

### Comparing `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/paginator.py` & `mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     def paginate(
         self,
         *,
         name: SettingNameType = ...,
         value: str = ...,
         principalArn: str = ...,
         effectiveSettings: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountSettingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listaccountsettingspaginator)
         """
 
 
@@ -122,30 +122,30 @@
     def paginate(
         self,
         *,
         targetType: Literal["container-instance"],
         cluster: str = ...,
         attributeName: str = ...,
         attributeValue: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listattributespaginator)
         """
 
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listclusterspaginator)
         """
 
 
@@ -157,15 +157,15 @@
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         filter: str = ...,
         status: ContainerInstanceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListContainerInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listcontainerinstancespaginator)
         """
 
 
@@ -177,30 +177,30 @@
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         launchType: LaunchTypeType = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicespaginator)
         """
 
 
 class ListServicesByNamespacePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicesbynamespacepaginator)
     """
 
     def paginate(
-        self, *, namespace: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, namespace: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicesByNamespaceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicesbynamespacepaginator)
         """
 
 
@@ -211,15 +211,15 @@
     """
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionFamilyStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTaskDefinitionFamiliesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionfamiliespaginator)
         """
 
 
@@ -231,15 +231,15 @@
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionStatusType = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTaskDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionspaginator)
         """
 
 
@@ -255,13 +255,13 @@
         cluster: str = ...,
         containerInstance: str = ...,
         family: str = ...,
         startedBy: str = ...,
         serviceName: str = ...,
         desiredStatus: DesiredStatusType = ...,
         launchType: LaunchTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskspaginator)
         """
```

### Comparing `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/paginator.pyi` & `mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     def paginate(
         self,
         *,
         name: SettingNameType = ...,
         value: str = ...,
         principalArn: str = ...,
         effectiveSettings: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountSettingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAccountSettings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listaccountsettingspaginator)
         """
 
 class ListAttributesPaginator(Paginator):
@@ -117,29 +117,29 @@
     def paginate(
         self,
         *,
         targetType: Literal["container-instance"],
         cluster: str = ...,
         attributeName: str = ...,
         attributeValue: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListAttributes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listattributespaginator)
         """
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listclusterspaginator)
         """
 
 class ListContainerInstancesPaginator(Paginator):
@@ -150,15 +150,15 @@
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         filter: str = ...,
         status: ContainerInstanceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListContainerInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListContainerInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listcontainerinstancespaginator)
         """
 
 class ListServicesPaginator(Paginator):
@@ -169,29 +169,29 @@
 
     def paginate(
         self,
         *,
         cluster: str = ...,
         launchType: LaunchTypeType = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicespaginator)
         """
 
 class ListServicesByNamespacePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicesbynamespacepaginator)
     """
 
     def paginate(
-        self, *, namespace: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, namespace: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListServicesByNamespaceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListServicesByNamespace.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listservicesbynamespacepaginator)
         """
 
 class ListTaskDefinitionFamiliesPaginator(Paginator):
@@ -201,15 +201,15 @@
     """
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionFamilyStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTaskDefinitionFamiliesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitionFamilies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionfamiliespaginator)
         """
 
 class ListTaskDefinitionsPaginator(Paginator):
@@ -220,15 +220,15 @@
 
     def paginate(
         self,
         *,
         familyPrefix: str = ...,
         status: TaskDefinitionStatusType = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTaskDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTaskDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskdefinitionspaginator)
         """
 
 class ListTasksPaginator(Paginator):
@@ -243,13 +243,13 @@
         cluster: str = ...,
         containerInstance: str = ...,
         family: str = ...,
         startedBy: str = ...,
         serviceName: str = ...,
         desiredStatus: DesiredStatusType = ...,
         launchType: LaunchTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Paginator.ListTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/paginators/#listtaskspaginator)
         """
```

### Comparing `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/type_defs.py` & `mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,15 +98,14 @@
     "VolumeFromTypeDef",
     "InstanceHealthCheckResultTypeDef",
     "ResourceTypeDef",
     "VersionInfoTypeDef",
     "NetworkBindingTypeDef",
     "ManagedAgentTypeDef",
     "NetworkInterfaceTypeDef",
-    "ResponseMetadataTypeDef",
     "DeploymentControllerTypeDef",
     "LoadBalancerTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "ServiceRegistryTypeDef",
     "ScaleTypeDef",
     "DeleteAccountSettingRequestRequestTypeDef",
@@ -128,85 +127,95 @@
     "DescribeServicesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTaskDefinitionRequestRequestTypeDef",
     "DescribeTaskSetsRequestRequestTypeDef",
     "DescribeTasksRequestRequestTypeDef",
     "DeviceTypeDef",
     "DiscoverPollEndpointRequestRequestTypeDef",
+    "DiscoverPollEndpointResponseTypeDef",
     "DockerVolumeConfigurationTypeDef",
     "EFSAuthorizationConfigTypeDef",
     "EphemeralStorageTypeDef",
     "ExecuteCommandLogConfigurationTypeDef",
     "ExecuteCommandRequestRequestTypeDef",
     "SessionTypeDef",
     "FSxWindowsFileServerAuthorizationConfigTypeDef",
     "GetTaskProtectionRequestRequestTypeDef",
     "ProtectedTaskTypeDef",
     "HostVolumePropertiesTypeDef",
     "InferenceAcceleratorOverrideTypeDef",
     "InferenceAcceleratorTypeDef",
     "KernelCapabilitiesTypeDef",
     "TmpfsTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
     "ListAccountSettingsRequestRequestTypeDef",
+    "ListAttributesRequestListAttributesPaginateTypeDef",
     "ListAttributesRequestRequestTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
+    "ListClustersResponseTypeDef",
+    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
     "ListContainerInstancesRequestRequestTypeDef",
+    "ListContainerInstancesResponseTypeDef",
+    "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
     "ListServicesByNamespaceRequestRequestTypeDef",
+    "ListServicesByNamespaceResponseTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
+    "ListServicesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
+    "ListTaskDefinitionFamiliesResponseTypeDef",
+    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
     "ListTaskDefinitionsRequestRequestTypeDef",
+    "ListTaskDefinitionsResponseTypeDef",
+    "ListTasksRequestListTasksPaginateTypeDef",
     "ListTasksRequestRequestTypeDef",
+    "ListTasksResponseTypeDef",
     "ManagedAgentStateChangeTypeDef",
+    "PaginatorConfigTypeDef",
     "PlatformDeviceTypeDef",
     "PutAccountSettingDefaultRequestRequestTypeDef",
     "PutAccountSettingRequestRequestTypeDef",
     "RuntimePlatformTypeDef",
     "TaskDefinitionPlacementConstraintTypeDef",
+    "ResponseMetadataTypeDef",
     "ServiceConnectClientAliasTypeDef",
     "ServiceEventTypeDef",
     "StopTaskRequestRequestTypeDef",
+    "SubmitAttachmentStateChangesResponseTypeDef",
+    "SubmitContainerStateChangeResponseTypeDef",
+    "SubmitTaskStateChangeResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContainerAgentRequestRequestTypeDef",
     "UpdateContainerInstancesStateRequestRequestTypeDef",
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     "UpdateTaskProtectionRequestRequestTypeDef",
     "SubmitAttachmentStateChangesRequestRequestTypeDef",
     "AttachmentTypeDef",
     "ProxyConfigurationTypeDef",
     "DeleteAttributesRequestRequestTypeDef",
+    "DeleteAttributesResponseTypeDef",
+    "ListAttributesResponseTypeDef",
     "PutAttributesRequestRequestTypeDef",
+    "PutAttributesResponseTypeDef",
     "AutoScalingGroupProviderTypeDef",
     "AutoScalingGroupProviderUpdateTypeDef",
     "NetworkConfigurationTypeDef",
     "PutClusterCapacityProvidersRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UpdateClusterSettingsRequestRequestTypeDef",
     "ContainerOverrideTypeDef",
     "LogConfigurationTypeDef",
     "ContainerInstanceHealthStatusTypeDef",
     "ContainerStateChangeTypeDef",
     "SubmitContainerStateChangeRequestRequestTypeDef",
     "ContainerTypeDef",
-    "DeleteAttributesResponseTypeDef",
-    "DiscoverPollEndpointResponseTypeDef",
-    "ListAttributesResponseTypeDef",
-    "ListClustersResponseTypeDef",
-    "ListContainerInstancesResponseTypeDef",
-    "ListServicesByNamespaceResponseTypeDef",
-    "ListServicesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTaskDefinitionFamiliesResponseTypeDef",
-    "ListTaskDefinitionsResponseTypeDef",
-    "ListTasksResponseTypeDef",
-    "PutAttributesResponseTypeDef",
-    "SubmitAttachmentStateChangesResponseTypeDef",
-    "SubmitContainerStateChangeResponseTypeDef",
-    "SubmitTaskStateChangeResponseTypeDef",
     "UpdateTaskSetRequestRequestTypeDef",
     "DeleteAccountSettingResponseTypeDef",
     "ListAccountSettingsResponseTypeDef",
     "PutAccountSettingDefaultResponseTypeDef",
     "PutAccountSettingResponseTypeDef",
     "DeploymentConfigurationTypeDef",
     "DescribeServicesRequestServicesInactiveWaitTypeDef",
@@ -216,23 +225,14 @@
     "EFSVolumeConfigurationTypeDef",
     "ExecuteCommandConfigurationTypeDef",
     "ExecuteCommandResponseTypeDef",
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     "GetTaskProtectionResponseTypeDef",
     "UpdateTaskProtectionResponseTypeDef",
     "LinuxParametersTypeDef",
-    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
-    "ListAttributesRequestListAttributesPaginateTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
-    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
-    "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
-    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
-    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
-    "ListTasksRequestListTasksPaginateTypeDef",
     "RegisterContainerInstanceRequestRequestTypeDef",
     "ServiceConnectServiceTypeDef",
     "CapacityProviderTypeDef",
     "CreateCapacityProviderRequestRequestTypeDef",
     "UpdateCapacityProviderRequestRequestTypeDef",
     "CreateTaskSetRequestRequestTypeDef",
     "TaskSetTypeDef",
@@ -620,25 +620,14 @@
         "attachmentId": str,
         "privateIpv4Address": str,
         "ipv6Address": str,
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
 DeploymentControllerTypeDef = TypedDict(
     "DeploymentControllerTypeDef",
     {
         "type": DeploymentControllerTypeType,
     },
 )
 
@@ -1021,14 +1010,24 @@
     {
         "containerInstance": str,
         "cluster": str,
     },
     total=False,
 )
 
+DiscoverPollEndpointResponseTypeDef = TypedDict(
+    "DiscoverPollEndpointResponseTypeDef",
+    {
+        "endpoint": str,
+        "telemetryEndpoint": str,
+        "serviceConnectEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DockerVolumeConfigurationTypeDef = TypedDict(
     "DockerVolumeConfigurationTypeDef",
     {
         "scope": ScopeType,
         "autoprovision": bool,
         "driver": str,
         "driverOpts": Dict[str, str],
@@ -1188,20 +1187,22 @@
 )
 
 
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAccountSettingsRequestListAccountSettingsPaginateTypeDef = TypedDict(
+    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "name": SettingNameType,
+        "value": str,
+        "principalArn": str,
+        "effectiveSettings": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAccountSettingsRequestRequestTypeDef = TypedDict(
     "ListAccountSettingsRequestRequestTypeDef",
     {
@@ -1211,14 +1212,39 @@
         "effectiveSettings": bool,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListAttributesRequestListAttributesPaginateTypeDef",
+    {
+        "targetType": Literal["container-instance"],
+    },
+)
+_OptionalListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListAttributesRequestListAttributesPaginateTypeDef",
+    {
+        "cluster": str,
+        "attributeName": str,
+        "attributeValue": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListAttributesRequestListAttributesPaginateTypeDef(
+    _RequiredListAttributesRequestListAttributesPaginateTypeDef,
+    _OptionalListAttributesRequestListAttributesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttributesRequestRequestTypeDef",
     {
         "targetType": Literal["container-instance"],
     },
 )
 _OptionalListAttributesRequestRequestTypeDef = TypedDict(
@@ -1236,35 +1262,94 @@
 
 class ListAttributesRequestRequestTypeDef(
     _RequiredListAttributesRequestRequestTypeDef, _OptionalListAttributesRequestRequestTypeDef
 ):
     pass
 
 
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListClustersResponseTypeDef = TypedDict(
+    "ListClustersResponseTypeDef",
+    {
+        "clusterArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListContainerInstancesRequestListContainerInstancesPaginateTypeDef = TypedDict(
+    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
+    {
+        "cluster": str,
+        "filter": str,
+        "status": ContainerInstanceStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListContainerInstancesRequestRequestTypeDef = TypedDict(
     "ListContainerInstancesRequestRequestTypeDef",
     {
         "cluster": str,
         "filter": str,
         "nextToken": str,
         "maxResults": int,
         "status": ContainerInstanceStatusType,
     },
     total=False,
 )
 
+ListContainerInstancesResponseTypeDef = TypedDict(
+    "ListContainerInstancesResponseTypeDef",
+    {
+        "containerInstanceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "namespace": str,
+    },
+)
+_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
+    _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+    _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListServicesByNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredListServicesByNamespaceRequestRequestTypeDef",
     {
         "namespace": str,
     },
 )
 _OptionalListServicesByNamespaceRequestRequestTypeDef = TypedDict(
@@ -1280,56 +1365,139 @@
 class ListServicesByNamespaceRequestRequestTypeDef(
     _RequiredListServicesByNamespaceRequestRequestTypeDef,
     _OptionalListServicesByNamespaceRequestRequestTypeDef,
 ):
     pass
 
 
+ListServicesByNamespaceResponseTypeDef = TypedDict(
+    "ListServicesByNamespaceResponseTypeDef",
+    {
+        "serviceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "cluster": str,
+        "launchType": LaunchTypeType,
+        "schedulingStrategy": SchedulingStrategyType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "cluster": str,
         "nextToken": str,
         "maxResults": int,
         "launchType": LaunchTypeType,
         "schedulingStrategy": SchedulingStrategyType,
     },
     total=False,
 )
 
+ListServicesResponseTypeDef = TypedDict(
+    "ListServicesResponseTypeDef",
+    {
+        "serviceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef = TypedDict(
+    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
+    {
+        "familyPrefix": str,
+        "status": TaskDefinitionFamilyStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTaskDefinitionFamiliesRequestRequestTypeDef = TypedDict(
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
     {
         "familyPrefix": str,
         "status": TaskDefinitionFamilyStatusType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListTaskDefinitionFamiliesResponseTypeDef = TypedDict(
+    "ListTaskDefinitionFamiliesResponseTypeDef",
+    {
+        "families": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef = TypedDict(
+    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
+    {
+        "familyPrefix": str,
+        "status": TaskDefinitionStatusType,
+        "sort": SortOrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTaskDefinitionsRequestRequestTypeDef = TypedDict(
     "ListTaskDefinitionsRequestRequestTypeDef",
     {
         "familyPrefix": str,
         "status": TaskDefinitionStatusType,
         "sort": SortOrderType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListTaskDefinitionsResponseTypeDef = TypedDict(
+    "ListTaskDefinitionsResponseTypeDef",
+    {
+        "taskDefinitionArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTasksRequestListTasksPaginateTypeDef = TypedDict(
+    "ListTasksRequestListTasksPaginateTypeDef",
+    {
+        "cluster": str,
+        "containerInstance": str,
+        "family": str,
+        "startedBy": str,
+        "serviceName": str,
+        "desiredStatus": DesiredStatusType,
+        "launchType": LaunchTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTasksRequestRequestTypeDef = TypedDict(
     "ListTasksRequestRequestTypeDef",
     {
         "cluster": str,
         "containerInstance": str,
         "family": str,
         "nextToken": str,
@@ -1338,14 +1506,23 @@
         "serviceName": str,
         "desiredStatus": DesiredStatusType,
         "launchType": LaunchTypeType,
     },
     total=False,
 )
 
+ListTasksResponseTypeDef = TypedDict(
+    "ListTasksResponseTypeDef",
+    {
+        "taskArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredManagedAgentStateChangeTypeDef = TypedDict(
     "_RequiredManagedAgentStateChangeTypeDef",
     {
         "containerName": str,
         "managedAgentName": Literal["ExecuteCommandAgent"],
         "status": str,
     },
@@ -1361,14 +1538,24 @@
 
 class ManagedAgentStateChangeTypeDef(
     _RequiredManagedAgentStateChangeTypeDef, _OptionalManagedAgentStateChangeTypeDef
 ):
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
 PlatformDeviceTypeDef = TypedDict(
     "PlatformDeviceTypeDef",
     {
         "id": str,
         "type": Literal["GPU"],
     },
 )
@@ -1417,14 +1604,25 @@
     {
         "type": Literal["memberOf"],
         "expression": str,
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
 _RequiredServiceConnectClientAliasTypeDef = TypedDict(
     "_RequiredServiceConnectClientAliasTypeDef",
     {
         "port": int,
     },
 )
 _OptionalServiceConnectClientAliasTypeDef = TypedDict(
@@ -1470,14 +1668,38 @@
 
 class StopTaskRequestRequestTypeDef(
     _RequiredStopTaskRequestRequestTypeDef, _OptionalStopTaskRequestRequestTypeDef
 ):
     pass
 
 
+SubmitAttachmentStateChangesResponseTypeDef = TypedDict(
+    "SubmitAttachmentStateChangesResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SubmitContainerStateChangeResponseTypeDef = TypedDict(
+    "SubmitContainerStateChangeResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SubmitTaskStateChangeResponseTypeDef = TypedDict(
+    "SubmitTaskStateChangeResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1632,14 +1854,31 @@
 
 class DeleteAttributesRequestRequestTypeDef(
     _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
 ):
     pass
 
 
+DeleteAttributesResponseTypeDef = TypedDict(
+    "DeleteAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAttributesResponseTypeDef = TypedDict(
+    "ListAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalPutAttributesRequestRequestTypeDef = TypedDict(
@@ -1653,14 +1892,22 @@
 
 class PutAttributesRequestRequestTypeDef(
     _RequiredPutAttributesRequestRequestTypeDef, _OptionalPutAttributesRequestRequestTypeDef
 ):
     pass
 
 
+PutAttributesResponseTypeDef = TypedDict(
+    "PutAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAutoScalingGroupProviderTypeDef = TypedDict(
     "_RequiredAutoScalingGroupProviderTypeDef",
     {
         "autoScalingGroupArn": str,
     },
 )
 _OptionalAutoScalingGroupProviderTypeDef = TypedDict(
@@ -1701,14 +1948,22 @@
     {
         "cluster": str,
         "capacityProviders": Sequence[str],
         "defaultCapacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1814,184 +2069,54 @@
         "memory": str,
         "memoryReservation": str,
         "gpuIds": List[str],
     },
     total=False,
 )
 
-DeleteAttributesResponseTypeDef = TypedDict(
-    "DeleteAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DiscoverPollEndpointResponseTypeDef = TypedDict(
-    "DiscoverPollEndpointResponseTypeDef",
-    {
-        "endpoint": str,
-        "telemetryEndpoint": str,
-        "serviceConnectEndpoint": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAttributesResponseTypeDef = TypedDict(
-    "ListAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListClustersResponseTypeDef = TypedDict(
-    "ListClustersResponseTypeDef",
-    {
-        "clusterArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListContainerInstancesResponseTypeDef = TypedDict(
-    "ListContainerInstancesResponseTypeDef",
-    {
-        "containerInstanceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListServicesByNamespaceResponseTypeDef = TypedDict(
-    "ListServicesByNamespaceResponseTypeDef",
-    {
-        "serviceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListServicesResponseTypeDef = TypedDict(
-    "ListServicesResponseTypeDef",
-    {
-        "serviceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTaskDefinitionFamiliesResponseTypeDef = TypedDict(
-    "ListTaskDefinitionFamiliesResponseTypeDef",
-    {
-        "families": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTaskDefinitionsResponseTypeDef = TypedDict(
-    "ListTaskDefinitionsResponseTypeDef",
-    {
-        "taskDefinitionArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTasksResponseTypeDef = TypedDict(
-    "ListTasksResponseTypeDef",
-    {
-        "taskArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutAttributesResponseTypeDef = TypedDict(
-    "PutAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SubmitAttachmentStateChangesResponseTypeDef = TypedDict(
-    "SubmitAttachmentStateChangesResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SubmitContainerStateChangeResponseTypeDef = TypedDict(
-    "SubmitContainerStateChangeResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SubmitTaskStateChangeResponseTypeDef = TypedDict(
-    "SubmitTaskStateChangeResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateTaskSetRequestRequestTypeDef = TypedDict(
     "UpdateTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
         "taskSet": str,
         "scale": ScaleTypeDef,
     },
 )
 
 DeleteAccountSettingResponseTypeDef = TypedDict(
     "DeleteAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAccountSettingsResponseTypeDef = TypedDict(
     "ListAccountSettingsResponseTypeDef",
     {
         "settings": List[SettingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAccountSettingDefaultResponseTypeDef = TypedDict(
     "PutAccountSettingDefaultResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAccountSettingResponseTypeDef = TypedDict(
     "PutAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentConfigurationTypeDef = TypedDict(
     "DeploymentConfigurationTypeDef",
     {
         "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
@@ -2137,15 +2262,15 @@
     {
         "clusterArn": str,
         "containerArn": str,
         "containerName": str,
         "interactive": bool,
         "session": SessionTypeDef,
         "taskArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FSxWindowsFileServerVolumeConfigurationTypeDef = TypedDict(
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
@@ -2155,24 +2280,24 @@
 )
 
 GetTaskProtectionResponseTypeDef = TypedDict(
     "GetTaskProtectionResponseTypeDef",
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTaskProtectionResponseTypeDef = TypedDict(
     "UpdateTaskProtectionResponseTypeDef",
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LinuxParametersTypeDef = TypedDict(
     "LinuxParametersTypeDef",
     {
         "capabilities": KernelCapabilitiesTypeDef,
@@ -2182,139 +2307,14 @@
         "tmpfs": List[TmpfsTypeDef],
         "maxSwap": int,
         "swappiness": int,
     },
     total=False,
 )
 
-ListAccountSettingsRequestListAccountSettingsPaginateTypeDef = TypedDict(
-    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
-    {
-        "name": SettingNameType,
-        "value": str,
-        "principalArn": str,
-        "effectiveSettings": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListAttributesRequestListAttributesPaginateTypeDef",
-    {
-        "targetType": Literal["container-instance"],
-    },
-)
-_OptionalListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListAttributesRequestListAttributesPaginateTypeDef",
-    {
-        "cluster": str,
-        "attributeName": str,
-        "attributeValue": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAttributesRequestListAttributesPaginateTypeDef(
-    _RequiredListAttributesRequestListAttributesPaginateTypeDef,
-    _OptionalListAttributesRequestListAttributesPaginateTypeDef,
-):
-    pass
-
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListContainerInstancesRequestListContainerInstancesPaginateTypeDef = TypedDict(
-    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
-    {
-        "cluster": str,
-        "filter": str,
-        "status": ContainerInstanceStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
-    "_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
-    {
-        "namespace": str,
-    },
-)
-_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
-    "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
-    _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
-    _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
-):
-    pass
-
-
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "cluster": str,
-        "launchType": LaunchTypeType,
-        "schedulingStrategy": SchedulingStrategyType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef = TypedDict(
-    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
-    {
-        "familyPrefix": str,
-        "status": TaskDefinitionFamilyStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef = TypedDict(
-    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
-    {
-        "familyPrefix": str,
-        "status": TaskDefinitionStatusType,
-        "sort": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTasksRequestListTasksPaginateTypeDef = TypedDict(
-    "ListTasksRequestListTasksPaginateTypeDef",
-    {
-        "cluster": str,
-        "containerInstance": str,
-        "family": str,
-        "startedBy": str,
-        "serviceName": str,
-        "desiredStatus": DesiredStatusType,
-        "launchType": LaunchTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
     "RegisterContainerInstanceRequestRequestTypeDef",
     {
         "cluster": str,
         "instanceIdentityDocument": str,
         "instanceIdentityDocumentSignature": str,
         "totalResources": Sequence[ResourceTypeDef],
@@ -2572,14 +2572,15 @@
         "dockerLabels": Dict[str, str],
         "ulimits": List[UlimitTypeDef],
         "logConfiguration": LogConfigurationTypeDef,
         "healthCheck": HealthCheckTypeDef,
         "systemControls": List[SystemControlTypeDef],
         "resourceRequirements": List[ResourceRequirementTypeDef],
         "firelensConfiguration": FirelensConfigurationTypeDef,
+        "credentialSpecs": List[str],
     },
     total=False,
 )
 
 _RequiredServiceConnectConfigurationTypeDef = TypedDict(
     "_RequiredServiceConnectConfigurationTypeDef",
     {
@@ -2603,82 +2604,82 @@
     pass
 
 
 CreateCapacityProviderResponseTypeDef = TypedDict(
     "CreateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCapacityProviderResponseTypeDef = TypedDict(
     "DeleteCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCapacityProvidersResponseTypeDef = TypedDict(
     "DescribeCapacityProvidersResponseTypeDef",
     {
         "capacityProviders": List[CapacityProviderTypeDef],
         "failures": List[FailureTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCapacityProviderResponseTypeDef = TypedDict(
     "UpdateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTaskSetResponseTypeDef = TypedDict(
     "CreateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteTaskSetResponseTypeDef = TypedDict(
     "DeleteTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTaskSetsResponseTypeDef = TypedDict(
     "DescribeTaskSetsResponseTypeDef",
     {
         "taskSets": List[TaskSetTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServicePrimaryTaskSetResponseTypeDef = TypedDict(
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTaskSetResponseTypeDef = TypedDict(
     "UpdateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRunTaskRequestRequestTypeDef = TypedDict(
     "_RequiredRunTaskRequestRequestTypeDef",
     {
         "taskDefinition": str,
@@ -2788,49 +2789,49 @@
     total=False,
 )
 
 DeregisterContainerInstanceResponseTypeDef = TypedDict(
     "DeregisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContainerInstancesResponseTypeDef = TypedDict(
     "DescribeContainerInstancesResponseTypeDef",
     {
         "containerInstances": List[ContainerInstanceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegisterContainerInstanceResponseTypeDef = TypedDict(
     "RegisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContainerAgentResponseTypeDef = TypedDict(
     "UpdateContainerAgentResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContainerInstancesStateResponseTypeDef = TypedDict(
     "UpdateContainerInstancesStateResponseTypeDef",
     {
         "containerInstances": List[ContainerInstanceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "clusterArn": str,
@@ -3063,125 +3064,125 @@
 
 
 DescribeTasksResponseTypeDef = TypedDict(
     "DescribeTasksResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RunTaskResponseTypeDef = TypedDict(
     "RunTaskResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartTaskResponseTypeDef = TypedDict(
     "StartTaskResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopTaskResponseTypeDef = TypedDict(
     "StopTaskResponseTypeDef",
     {
         "task": TaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "clusters": List[ClusterTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutClusterCapacityProvidersResponseTypeDef = TypedDict(
     "PutClusterCapacityProvidersResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterResponseTypeDef = TypedDict(
     "UpdateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterSettingsResponseTypeDef = TypedDict(
     "UpdateClusterSettingsResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteTaskDefinitionsResponseTypeDef = TypedDict(
     "DeleteTaskDefinitionsResponseTypeDef",
     {
         "taskDefinitions": List[TaskDefinitionTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeregisterTaskDefinitionResponseTypeDef = TypedDict(
     "DeregisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTaskDefinitionResponseTypeDef = TypedDict(
     "DescribeTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegisterTaskDefinitionResponseTypeDef = TypedDict(
     "RegisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "serviceArn": str,
@@ -3219,35 +3220,35 @@
     total=False,
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteServiceResponseTypeDef = TypedDict(
     "DeleteServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceResponseTypeDef = TypedDict(
     "UpdateServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/type_defs.pyi` & `mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -97,15 +97,14 @@
     "VolumeFromTypeDef",
     "InstanceHealthCheckResultTypeDef",
     "ResourceTypeDef",
     "VersionInfoTypeDef",
     "NetworkBindingTypeDef",
     "ManagedAgentTypeDef",
     "NetworkInterfaceTypeDef",
-    "ResponseMetadataTypeDef",
     "DeploymentControllerTypeDef",
     "LoadBalancerTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "ServiceRegistryTypeDef",
     "ScaleTypeDef",
     "DeleteAccountSettingRequestRequestTypeDef",
@@ -127,85 +126,95 @@
     "DescribeServicesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTaskDefinitionRequestRequestTypeDef",
     "DescribeTaskSetsRequestRequestTypeDef",
     "DescribeTasksRequestRequestTypeDef",
     "DeviceTypeDef",
     "DiscoverPollEndpointRequestRequestTypeDef",
+    "DiscoverPollEndpointResponseTypeDef",
     "DockerVolumeConfigurationTypeDef",
     "EFSAuthorizationConfigTypeDef",
     "EphemeralStorageTypeDef",
     "ExecuteCommandLogConfigurationTypeDef",
     "ExecuteCommandRequestRequestTypeDef",
     "SessionTypeDef",
     "FSxWindowsFileServerAuthorizationConfigTypeDef",
     "GetTaskProtectionRequestRequestTypeDef",
     "ProtectedTaskTypeDef",
     "HostVolumePropertiesTypeDef",
     "InferenceAcceleratorOverrideTypeDef",
     "InferenceAcceleratorTypeDef",
     "KernelCapabilitiesTypeDef",
     "TmpfsTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
     "ListAccountSettingsRequestRequestTypeDef",
+    "ListAttributesRequestListAttributesPaginateTypeDef",
     "ListAttributesRequestRequestTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
+    "ListClustersResponseTypeDef",
+    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
     "ListContainerInstancesRequestRequestTypeDef",
+    "ListContainerInstancesResponseTypeDef",
+    "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
     "ListServicesByNamespaceRequestRequestTypeDef",
+    "ListServicesByNamespaceResponseTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
+    "ListServicesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
+    "ListTaskDefinitionFamiliesResponseTypeDef",
+    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
     "ListTaskDefinitionsRequestRequestTypeDef",
+    "ListTaskDefinitionsResponseTypeDef",
+    "ListTasksRequestListTasksPaginateTypeDef",
     "ListTasksRequestRequestTypeDef",
+    "ListTasksResponseTypeDef",
     "ManagedAgentStateChangeTypeDef",
+    "PaginatorConfigTypeDef",
     "PlatformDeviceTypeDef",
     "PutAccountSettingDefaultRequestRequestTypeDef",
     "PutAccountSettingRequestRequestTypeDef",
     "RuntimePlatformTypeDef",
     "TaskDefinitionPlacementConstraintTypeDef",
+    "ResponseMetadataTypeDef",
     "ServiceConnectClientAliasTypeDef",
     "ServiceEventTypeDef",
     "StopTaskRequestRequestTypeDef",
+    "SubmitAttachmentStateChangesResponseTypeDef",
+    "SubmitContainerStateChangeResponseTypeDef",
+    "SubmitTaskStateChangeResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContainerAgentRequestRequestTypeDef",
     "UpdateContainerInstancesStateRequestRequestTypeDef",
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     "UpdateTaskProtectionRequestRequestTypeDef",
     "SubmitAttachmentStateChangesRequestRequestTypeDef",
     "AttachmentTypeDef",
     "ProxyConfigurationTypeDef",
     "DeleteAttributesRequestRequestTypeDef",
+    "DeleteAttributesResponseTypeDef",
+    "ListAttributesResponseTypeDef",
     "PutAttributesRequestRequestTypeDef",
+    "PutAttributesResponseTypeDef",
     "AutoScalingGroupProviderTypeDef",
     "AutoScalingGroupProviderUpdateTypeDef",
     "NetworkConfigurationTypeDef",
     "PutClusterCapacityProvidersRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UpdateClusterSettingsRequestRequestTypeDef",
     "ContainerOverrideTypeDef",
     "LogConfigurationTypeDef",
     "ContainerInstanceHealthStatusTypeDef",
     "ContainerStateChangeTypeDef",
     "SubmitContainerStateChangeRequestRequestTypeDef",
     "ContainerTypeDef",
-    "DeleteAttributesResponseTypeDef",
-    "DiscoverPollEndpointResponseTypeDef",
-    "ListAttributesResponseTypeDef",
-    "ListClustersResponseTypeDef",
-    "ListContainerInstancesResponseTypeDef",
-    "ListServicesByNamespaceResponseTypeDef",
-    "ListServicesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTaskDefinitionFamiliesResponseTypeDef",
-    "ListTaskDefinitionsResponseTypeDef",
-    "ListTasksResponseTypeDef",
-    "PutAttributesResponseTypeDef",
-    "SubmitAttachmentStateChangesResponseTypeDef",
-    "SubmitContainerStateChangeResponseTypeDef",
-    "SubmitTaskStateChangeResponseTypeDef",
     "UpdateTaskSetRequestRequestTypeDef",
     "DeleteAccountSettingResponseTypeDef",
     "ListAccountSettingsResponseTypeDef",
     "PutAccountSettingDefaultResponseTypeDef",
     "PutAccountSettingResponseTypeDef",
     "DeploymentConfigurationTypeDef",
     "DescribeServicesRequestServicesInactiveWaitTypeDef",
@@ -215,23 +224,14 @@
     "EFSVolumeConfigurationTypeDef",
     "ExecuteCommandConfigurationTypeDef",
     "ExecuteCommandResponseTypeDef",
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     "GetTaskProtectionResponseTypeDef",
     "UpdateTaskProtectionResponseTypeDef",
     "LinuxParametersTypeDef",
-    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
-    "ListAttributesRequestListAttributesPaginateTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
-    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
-    "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
-    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
-    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
-    "ListTasksRequestListTasksPaginateTypeDef",
     "RegisterContainerInstanceRequestRequestTypeDef",
     "ServiceConnectServiceTypeDef",
     "CapacityProviderTypeDef",
     "CreateCapacityProviderRequestRequestTypeDef",
     "UpdateCapacityProviderRequestRequestTypeDef",
     "CreateTaskSetRequestRequestTypeDef",
     "TaskSetTypeDef",
@@ -609,25 +609,14 @@
         "attachmentId": str,
         "privateIpv4Address": str,
         "ipv6Address": str,
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
 DeploymentControllerTypeDef = TypedDict(
     "DeploymentControllerTypeDef",
     {
         "type": DeploymentControllerTypeType,
     },
 )
 
@@ -990,14 +979,24 @@
     {
         "containerInstance": str,
         "cluster": str,
     },
     total=False,
 )
 
+DiscoverPollEndpointResponseTypeDef = TypedDict(
+    "DiscoverPollEndpointResponseTypeDef",
+    {
+        "endpoint": str,
+        "telemetryEndpoint": str,
+        "serviceConnectEndpoint": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DockerVolumeConfigurationTypeDef = TypedDict(
     "DockerVolumeConfigurationTypeDef",
     {
         "scope": ScopeType,
         "autoprovision": bool,
         "driver": str,
         "driverOpts": Dict[str, str],
@@ -1151,20 +1150,22 @@
     },
     total=False,
 )
 
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAccountSettingsRequestListAccountSettingsPaginateTypeDef = TypedDict(
+    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "name": SettingNameType,
+        "value": str,
+        "principalArn": str,
+        "effectiveSettings": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAccountSettingsRequestRequestTypeDef = TypedDict(
     "ListAccountSettingsRequestRequestTypeDef",
     {
@@ -1174,14 +1175,37 @@
         "effectiveSettings": bool,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListAttributesRequestListAttributesPaginateTypeDef",
+    {
+        "targetType": Literal["container-instance"],
+    },
+)
+_OptionalListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListAttributesRequestListAttributesPaginateTypeDef",
+    {
+        "cluster": str,
+        "attributeName": str,
+        "attributeValue": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListAttributesRequestListAttributesPaginateTypeDef(
+    _RequiredListAttributesRequestListAttributesPaginateTypeDef,
+    _OptionalListAttributesRequestListAttributesPaginateTypeDef,
+):
+    pass
+
 _RequiredListAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttributesRequestRequestTypeDef",
     {
         "targetType": Literal["container-instance"],
     },
 )
 _OptionalListAttributesRequestRequestTypeDef = TypedDict(
@@ -1197,35 +1221,92 @@
 )
 
 class ListAttributesRequestRequestTypeDef(
     _RequiredListAttributesRequestRequestTypeDef, _OptionalListAttributesRequestRequestTypeDef
 ):
     pass
 
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListClustersResponseTypeDef = TypedDict(
+    "ListClustersResponseTypeDef",
+    {
+        "clusterArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListContainerInstancesRequestListContainerInstancesPaginateTypeDef = TypedDict(
+    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
+    {
+        "cluster": str,
+        "filter": str,
+        "status": ContainerInstanceStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListContainerInstancesRequestRequestTypeDef = TypedDict(
     "ListContainerInstancesRequestRequestTypeDef",
     {
         "cluster": str,
         "filter": str,
         "nextToken": str,
         "maxResults": int,
         "status": ContainerInstanceStatusType,
     },
     total=False,
 )
 
+ListContainerInstancesResponseTypeDef = TypedDict(
+    "ListContainerInstancesResponseTypeDef",
+    {
+        "containerInstanceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "namespace": str,
+    },
+)
+_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
+    "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
+    _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+    _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
+):
+    pass
+
 _RequiredListServicesByNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredListServicesByNamespaceRequestRequestTypeDef",
     {
         "namespace": str,
     },
 )
 _OptionalListServicesByNamespaceRequestRequestTypeDef = TypedDict(
@@ -1239,56 +1320,139 @@
 
 class ListServicesByNamespaceRequestRequestTypeDef(
     _RequiredListServicesByNamespaceRequestRequestTypeDef,
     _OptionalListServicesByNamespaceRequestRequestTypeDef,
 ):
     pass
 
+ListServicesByNamespaceResponseTypeDef = TypedDict(
+    "ListServicesByNamespaceResponseTypeDef",
+    {
+        "serviceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "cluster": str,
+        "launchType": LaunchTypeType,
+        "schedulingStrategy": SchedulingStrategyType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "cluster": str,
         "nextToken": str,
         "maxResults": int,
         "launchType": LaunchTypeType,
         "schedulingStrategy": SchedulingStrategyType,
     },
     total=False,
 )
 
+ListServicesResponseTypeDef = TypedDict(
+    "ListServicesResponseTypeDef",
+    {
+        "serviceArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef = TypedDict(
+    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
+    {
+        "familyPrefix": str,
+        "status": TaskDefinitionFamilyStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTaskDefinitionFamiliesRequestRequestTypeDef = TypedDict(
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
     {
         "familyPrefix": str,
         "status": TaskDefinitionFamilyStatusType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListTaskDefinitionFamiliesResponseTypeDef = TypedDict(
+    "ListTaskDefinitionFamiliesResponseTypeDef",
+    {
+        "families": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef = TypedDict(
+    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
+    {
+        "familyPrefix": str,
+        "status": TaskDefinitionStatusType,
+        "sort": SortOrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTaskDefinitionsRequestRequestTypeDef = TypedDict(
     "ListTaskDefinitionsRequestRequestTypeDef",
     {
         "familyPrefix": str,
         "status": TaskDefinitionStatusType,
         "sort": SortOrderType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListTaskDefinitionsResponseTypeDef = TypedDict(
+    "ListTaskDefinitionsResponseTypeDef",
+    {
+        "taskDefinitionArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTasksRequestListTasksPaginateTypeDef = TypedDict(
+    "ListTasksRequestListTasksPaginateTypeDef",
+    {
+        "cluster": str,
+        "containerInstance": str,
+        "family": str,
+        "startedBy": str,
+        "serviceName": str,
+        "desiredStatus": DesiredStatusType,
+        "launchType": LaunchTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTasksRequestRequestTypeDef = TypedDict(
     "ListTasksRequestRequestTypeDef",
     {
         "cluster": str,
         "containerInstance": str,
         "family": str,
         "nextToken": str,
@@ -1297,14 +1461,23 @@
         "serviceName": str,
         "desiredStatus": DesiredStatusType,
         "launchType": LaunchTypeType,
     },
     total=False,
 )
 
+ListTasksResponseTypeDef = TypedDict(
+    "ListTasksResponseTypeDef",
+    {
+        "taskArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredManagedAgentStateChangeTypeDef = TypedDict(
     "_RequiredManagedAgentStateChangeTypeDef",
     {
         "containerName": str,
         "managedAgentName": Literal["ExecuteCommandAgent"],
         "status": str,
     },
@@ -1318,14 +1491,24 @@
 )
 
 class ManagedAgentStateChangeTypeDef(
     _RequiredManagedAgentStateChangeTypeDef, _OptionalManagedAgentStateChangeTypeDef
 ):
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
 PlatformDeviceTypeDef = TypedDict(
     "PlatformDeviceTypeDef",
     {
         "id": str,
         "type": Literal["GPU"],
     },
 )
@@ -1372,14 +1555,25 @@
     {
         "type": Literal["memberOf"],
         "expression": str,
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
 _RequiredServiceConnectClientAliasTypeDef = TypedDict(
     "_RequiredServiceConnectClientAliasTypeDef",
     {
         "port": int,
     },
 )
 _OptionalServiceConnectClientAliasTypeDef = TypedDict(
@@ -1421,14 +1615,38 @@
 )
 
 class StopTaskRequestRequestTypeDef(
     _RequiredStopTaskRequestRequestTypeDef, _OptionalStopTaskRequestRequestTypeDef
 ):
     pass
 
+SubmitAttachmentStateChangesResponseTypeDef = TypedDict(
+    "SubmitAttachmentStateChangesResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SubmitContainerStateChangeResponseTypeDef = TypedDict(
+    "SubmitContainerStateChangeResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+SubmitTaskStateChangeResponseTypeDef = TypedDict(
+    "SubmitTaskStateChangeResponseTypeDef",
+    {
+        "acknowledgment": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1571,14 +1789,31 @@
 )
 
 class DeleteAttributesRequestRequestTypeDef(
     _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
 ):
     pass
 
+DeleteAttributesResponseTypeDef = TypedDict(
+    "DeleteAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAttributesResponseTypeDef = TypedDict(
+    "ListAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalPutAttributesRequestRequestTypeDef = TypedDict(
@@ -1590,14 +1825,22 @@
 )
 
 class PutAttributesRequestRequestTypeDef(
     _RequiredPutAttributesRequestRequestTypeDef, _OptionalPutAttributesRequestRequestTypeDef
 ):
     pass
 
+PutAttributesResponseTypeDef = TypedDict(
+    "PutAttributesResponseTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAutoScalingGroupProviderTypeDef = TypedDict(
     "_RequiredAutoScalingGroupProviderTypeDef",
     {
         "autoScalingGroupArn": str,
     },
 )
 _OptionalAutoScalingGroupProviderTypeDef = TypedDict(
@@ -1636,14 +1879,22 @@
     {
         "cluster": str,
         "capacityProviders": Sequence[str],
         "defaultCapacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1747,184 +1998,54 @@
         "memory": str,
         "memoryReservation": str,
         "gpuIds": List[str],
     },
     total=False,
 )
 
-DeleteAttributesResponseTypeDef = TypedDict(
-    "DeleteAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DiscoverPollEndpointResponseTypeDef = TypedDict(
-    "DiscoverPollEndpointResponseTypeDef",
-    {
-        "endpoint": str,
-        "telemetryEndpoint": str,
-        "serviceConnectEndpoint": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAttributesResponseTypeDef = TypedDict(
-    "ListAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListClustersResponseTypeDef = TypedDict(
-    "ListClustersResponseTypeDef",
-    {
-        "clusterArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListContainerInstancesResponseTypeDef = TypedDict(
-    "ListContainerInstancesResponseTypeDef",
-    {
-        "containerInstanceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListServicesByNamespaceResponseTypeDef = TypedDict(
-    "ListServicesByNamespaceResponseTypeDef",
-    {
-        "serviceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListServicesResponseTypeDef = TypedDict(
-    "ListServicesResponseTypeDef",
-    {
-        "serviceArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTaskDefinitionFamiliesResponseTypeDef = TypedDict(
-    "ListTaskDefinitionFamiliesResponseTypeDef",
-    {
-        "families": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTaskDefinitionsResponseTypeDef = TypedDict(
-    "ListTaskDefinitionsResponseTypeDef",
-    {
-        "taskDefinitionArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTasksResponseTypeDef = TypedDict(
-    "ListTasksResponseTypeDef",
-    {
-        "taskArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutAttributesResponseTypeDef = TypedDict(
-    "PutAttributesResponseTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SubmitAttachmentStateChangesResponseTypeDef = TypedDict(
-    "SubmitAttachmentStateChangesResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SubmitContainerStateChangeResponseTypeDef = TypedDict(
-    "SubmitContainerStateChangeResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SubmitTaskStateChangeResponseTypeDef = TypedDict(
-    "SubmitTaskStateChangeResponseTypeDef",
-    {
-        "acknowledgment": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateTaskSetRequestRequestTypeDef = TypedDict(
     "UpdateTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
         "taskSet": str,
         "scale": ScaleTypeDef,
     },
 )
 
 DeleteAccountSettingResponseTypeDef = TypedDict(
     "DeleteAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAccountSettingsResponseTypeDef = TypedDict(
     "ListAccountSettingsResponseTypeDef",
     {
         "settings": List[SettingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAccountSettingDefaultResponseTypeDef = TypedDict(
     "PutAccountSettingDefaultResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAccountSettingResponseTypeDef = TypedDict(
     "PutAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentConfigurationTypeDef = TypedDict(
     "DeploymentConfigurationTypeDef",
     {
         "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
@@ -2060,15 +2181,15 @@
     {
         "clusterArn": str,
         "containerArn": str,
         "containerName": str,
         "interactive": bool,
         "session": SessionTypeDef,
         "taskArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FSxWindowsFileServerVolumeConfigurationTypeDef = TypedDict(
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
@@ -2078,24 +2199,24 @@
 )
 
 GetTaskProtectionResponseTypeDef = TypedDict(
     "GetTaskProtectionResponseTypeDef",
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTaskProtectionResponseTypeDef = TypedDict(
     "UpdateTaskProtectionResponseTypeDef",
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LinuxParametersTypeDef = TypedDict(
     "LinuxParametersTypeDef",
     {
         "capabilities": KernelCapabilitiesTypeDef,
@@ -2105,135 +2226,14 @@
         "tmpfs": List[TmpfsTypeDef],
         "maxSwap": int,
         "swappiness": int,
     },
     total=False,
 )
 
-ListAccountSettingsRequestListAccountSettingsPaginateTypeDef = TypedDict(
-    "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
-    {
-        "name": SettingNameType,
-        "value": str,
-        "principalArn": str,
-        "effectiveSettings": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListAttributesRequestListAttributesPaginateTypeDef",
-    {
-        "targetType": Literal["container-instance"],
-    },
-)
-_OptionalListAttributesRequestListAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListAttributesRequestListAttributesPaginateTypeDef",
-    {
-        "cluster": str,
-        "attributeName": str,
-        "attributeValue": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAttributesRequestListAttributesPaginateTypeDef(
-    _RequiredListAttributesRequestListAttributesPaginateTypeDef,
-    _OptionalListAttributesRequestListAttributesPaginateTypeDef,
-):
-    pass
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListContainerInstancesRequestListContainerInstancesPaginateTypeDef = TypedDict(
-    "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
-    {
-        "cluster": str,
-        "filter": str,
-        "status": ContainerInstanceStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
-    "_RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
-    {
-        "namespace": str,
-    },
-)
-_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef = TypedDict(
-    "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
-    _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
-    _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
-):
-    pass
-
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "cluster": str,
-        "launchType": LaunchTypeType,
-        "schedulingStrategy": SchedulingStrategyType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef = TypedDict(
-    "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
-    {
-        "familyPrefix": str,
-        "status": TaskDefinitionFamilyStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef = TypedDict(
-    "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
-    {
-        "familyPrefix": str,
-        "status": TaskDefinitionStatusType,
-        "sort": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTasksRequestListTasksPaginateTypeDef = TypedDict(
-    "ListTasksRequestListTasksPaginateTypeDef",
-    {
-        "cluster": str,
-        "containerInstance": str,
-        "family": str,
-        "startedBy": str,
-        "serviceName": str,
-        "desiredStatus": DesiredStatusType,
-        "launchType": LaunchTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
     "RegisterContainerInstanceRequestRequestTypeDef",
     {
         "cluster": str,
         "instanceIdentityDocument": str,
         "instanceIdentityDocumentSignature": str,
         "totalResources": Sequence[ResourceTypeDef],
@@ -2485,14 +2485,15 @@
         "dockerLabels": Dict[str, str],
         "ulimits": List[UlimitTypeDef],
         "logConfiguration": LogConfigurationTypeDef,
         "healthCheck": HealthCheckTypeDef,
         "systemControls": List[SystemControlTypeDef],
         "resourceRequirements": List[ResourceRequirementTypeDef],
         "firelensConfiguration": FirelensConfigurationTypeDef,
+        "credentialSpecs": List[str],
     },
     total=False,
 )
 
 _RequiredServiceConnectConfigurationTypeDef = TypedDict(
     "_RequiredServiceConnectConfigurationTypeDef",
     {
@@ -2514,82 +2515,82 @@
 ):
     pass
 
 CreateCapacityProviderResponseTypeDef = TypedDict(
     "CreateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCapacityProviderResponseTypeDef = TypedDict(
     "DeleteCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCapacityProvidersResponseTypeDef = TypedDict(
     "DescribeCapacityProvidersResponseTypeDef",
     {
         "capacityProviders": List[CapacityProviderTypeDef],
         "failures": List[FailureTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCapacityProviderResponseTypeDef = TypedDict(
     "UpdateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTaskSetResponseTypeDef = TypedDict(
     "CreateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteTaskSetResponseTypeDef = TypedDict(
     "DeleteTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTaskSetsResponseTypeDef = TypedDict(
     "DescribeTaskSetsResponseTypeDef",
     {
         "taskSets": List[TaskSetTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServicePrimaryTaskSetResponseTypeDef = TypedDict(
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTaskSetResponseTypeDef = TypedDict(
     "UpdateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRunTaskRequestRequestTypeDef = TypedDict(
     "_RequiredRunTaskRequestRequestTypeDef",
     {
         "taskDefinition": str,
@@ -2695,49 +2696,49 @@
     total=False,
 )
 
 DeregisterContainerInstanceResponseTypeDef = TypedDict(
     "DeregisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContainerInstancesResponseTypeDef = TypedDict(
     "DescribeContainerInstancesResponseTypeDef",
     {
         "containerInstances": List[ContainerInstanceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegisterContainerInstanceResponseTypeDef = TypedDict(
     "RegisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContainerAgentResponseTypeDef = TypedDict(
     "UpdateContainerAgentResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContainerInstancesStateResponseTypeDef = TypedDict(
     "UpdateContainerInstancesStateResponseTypeDef",
     {
         "containerInstances": List[ContainerInstanceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "clusterArn": str,
@@ -2962,125 +2963,125 @@
     pass
 
 DescribeTasksResponseTypeDef = TypedDict(
     "DescribeTasksResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RunTaskResponseTypeDef = TypedDict(
     "RunTaskResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartTaskResponseTypeDef = TypedDict(
     "StartTaskResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopTaskResponseTypeDef = TypedDict(
     "StopTaskResponseTypeDef",
     {
         "task": TaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "clusters": List[ClusterTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutClusterCapacityProvidersResponseTypeDef = TypedDict(
     "PutClusterCapacityProvidersResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterResponseTypeDef = TypedDict(
     "UpdateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateClusterSettingsResponseTypeDef = TypedDict(
     "UpdateClusterSettingsResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteTaskDefinitionsResponseTypeDef = TypedDict(
     "DeleteTaskDefinitionsResponseTypeDef",
     {
         "taskDefinitions": List[TaskDefinitionTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeregisterTaskDefinitionResponseTypeDef = TypedDict(
     "DeregisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTaskDefinitionResponseTypeDef = TypedDict(
     "DescribeTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegisterTaskDefinitionResponseTypeDef = TypedDict(
     "RegisterTaskDefinitionResponseTypeDef",
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "serviceArn": str,
@@ -3118,35 +3119,35 @@
     total=False,
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteServiceResponseTypeDef = TypedDict(
     "DeleteServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
         "failures": List[FailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceResponseTypeDef = TypedDict(
     "UpdateServiceResponseTypeDef",
     {
         "service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/waiter.py` & `mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs/waiter.pyi` & `mypy-boto3-ecs-1.27.0/mypy_boto3_ecs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/PKG-INFO` & `mypy-boto3-ecs-1.27.0/mypy_boto3_ecs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecs
-Version: 1.26.78
-Summary: Type annotations for boto3.ECS 1.26.78 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.ECS 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-ecs"></a>
 
 # mypy-boto3-ecs
 
 [![PyPI - mypy-boto3-ecs](https://img.shields.io/pypi/v/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecs?color=blue)](https://pypistats.org/packages/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -473,15 +473,14 @@
     VolumeFromTypeDef,
     InstanceHealthCheckResultTypeDef,
     ResourceTypeDef,
     VersionInfoTypeDef,
     NetworkBindingTypeDef,
     ManagedAgentTypeDef,
     NetworkInterfaceTypeDef,
-    ResponseMetadataTypeDef,
     DeploymentControllerTypeDef,
     LoadBalancerTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     ServiceRegistryTypeDef,
     ScaleTypeDef,
     DeleteAccountSettingRequestRequestTypeDef,
@@ -503,85 +502,95 @@
     DescribeServicesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTaskDefinitionRequestRequestTypeDef,
     DescribeTaskSetsRequestRequestTypeDef,
     DescribeTasksRequestRequestTypeDef,
     DeviceTypeDef,
     DiscoverPollEndpointRequestRequestTypeDef,
+    DiscoverPollEndpointResponseTypeDef,
     DockerVolumeConfigurationTypeDef,
     EFSAuthorizationConfigTypeDef,
     EphemeralStorageTypeDef,
     ExecuteCommandLogConfigurationTypeDef,
     ExecuteCommandRequestRequestTypeDef,
     SessionTypeDef,
     FSxWindowsFileServerAuthorizationConfigTypeDef,
     GetTaskProtectionRequestRequestTypeDef,
     ProtectedTaskTypeDef,
     HostVolumePropertiesTypeDef,
     InferenceAcceleratorOverrideTypeDef,
     InferenceAcceleratorTypeDef,
     KernelCapabilitiesTypeDef,
     TmpfsTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
     ListAccountSettingsRequestRequestTypeDef,
+    ListAttributesRequestListAttributesPaginateTypeDef,
     ListAttributesRequestRequestTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
+    ListClustersResponseTypeDef,
+    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
     ListContainerInstancesRequestRequestTypeDef,
+    ListContainerInstancesResponseTypeDef,
+    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     ListServicesByNamespaceRequestRequestTypeDef,
+    ListServicesByNamespaceResponseTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
+    ListServicesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
     ListTaskDefinitionFamiliesRequestRequestTypeDef,
+    ListTaskDefinitionFamiliesResponseTypeDef,
+    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
+    ListTaskDefinitionsResponseTypeDef,
+    ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
+    ListTasksResponseTypeDef,
     ManagedAgentStateChangeTypeDef,
+    PaginatorConfigTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
+    ResponseMetadataTypeDef,
     ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
     StopTaskRequestRequestTypeDef,
+    SubmitAttachmentStateChangesResponseTypeDef,
+    SubmitContainerStateChangeResponseTypeDef,
+    SubmitTaskStateChangeResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
     SubmitAttachmentStateChangesRequestRequestTypeDef,
     AttachmentTypeDef,
     ProxyConfigurationTypeDef,
     DeleteAttributesRequestRequestTypeDef,
+    DeleteAttributesResponseTypeDef,
+    ListAttributesResponseTypeDef,
     PutAttributesRequestRequestTypeDef,
+    PutAttributesResponseTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     NetworkConfigurationTypeDef,
     PutClusterCapacityProvidersRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UpdateClusterSettingsRequestRequestTypeDef,
     ContainerOverrideTypeDef,
     LogConfigurationTypeDef,
     ContainerInstanceHealthStatusTypeDef,
     ContainerStateChangeTypeDef,
     SubmitContainerStateChangeRequestRequestTypeDef,
     ContainerTypeDef,
-    DeleteAttributesResponseTypeDef,
-    DiscoverPollEndpointResponseTypeDef,
-    ListAttributesResponseTypeDef,
-    ListClustersResponseTypeDef,
-    ListContainerInstancesResponseTypeDef,
-    ListServicesByNamespaceResponseTypeDef,
-    ListServicesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTaskDefinitionFamiliesResponseTypeDef,
-    ListTaskDefinitionsResponseTypeDef,
-    ListTasksResponseTypeDef,
-    PutAttributesResponseTypeDef,
-    SubmitAttachmentStateChangesResponseTypeDef,
-    SubmitContainerStateChangeResponseTypeDef,
-    SubmitTaskStateChangeResponseTypeDef,
     UpdateTaskSetRequestRequestTypeDef,
     DeleteAccountSettingResponseTypeDef,
     ListAccountSettingsResponseTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
     DeploymentConfigurationTypeDef,
     DescribeServicesRequestServicesInactiveWaitTypeDef,
@@ -591,23 +600,14 @@
     EFSVolumeConfigurationTypeDef,
     ExecuteCommandConfigurationTypeDef,
     ExecuteCommandResponseTypeDef,
     FSxWindowsFileServerVolumeConfigurationTypeDef,
     GetTaskProtectionResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     LinuxParametersTypeDef,
-    ListAccountSettingsRequestListAccountSettingsPaginateTypeDef,
-    ListAttributesRequestListAttributesPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
-    ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
-    ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
-    ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
-    ListTasksRequestListTasksPaginateTypeDef,
     RegisterContainerInstanceRequestRequestTypeDef,
     ServiceConnectServiceTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
     CreateTaskSetRequestRequestTypeDef,
     TaskSetTypeDef,
@@ -672,42 +672,42 @@
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

### Comparing `mypy-boto3-ecs-1.26.78/mypy_boto3_ecs.egg-info/SOURCES.txt` & `mypy-boto3-ecs-1.27.0/mypy_boto3_ecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.26.78/setup.py` & `mypy-boto3-ecs-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-ecs.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecs",
-    version="1.26.78",
+    version="1.27.0",
     packages=["mypy_boto3_ecs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECS 1.26.78 service generated with mypy-boto3-builder 7.12.4"
+        "Type annotations for boto3.ECS 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/",
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


# Comparing `tmp/mypy-boto3-greengrassv2-1.26.59.tar.gz` & `tmp/mypy-boto3-greengrassv2-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-greengrassv2-1.26.59.tar", last modified: Fri Jan 27 20:32:50 2023, max compression
+gzip compressed data, was "mypy-boto3-greengrassv2-1.27.0.tar", last modified: Mon Jul  3 19:50:50 2023, max compression
```

## Comparing `mypy-boto3-greengrassv2-1.26.59.tar` & `mypy-boto3-greengrassv2-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.564096 mypy-boto3-greengrassv2-1.26.59/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-27 20:32:13.000000 mypy-boto3-greengrassv2-1.26.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-01-27 20:32:50.564096 mypy-boto3-greengrassv2-1.26.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17606 2023-01-27 20:32:13.000000 mypy-boto3-greengrassv2-1.26.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.564096 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-01-27 20:32:13.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-01-27 20:32:13.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-27 20:32:13.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25666 2023-01-27 20:32:13.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25623 2023-01-27 20:32:13.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-01-27 20:32:14.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-01-27 20:32:14.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-01-27 20:32:13.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-01-27 20:32:13.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:13.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37146 2023-01-27 20:32:14.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37113 2023-01-27 20:32:14.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-27 20:32:13.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:50.564096 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-01-27 20:32:50.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-01-27 20:32:50.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:50.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:50.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-27 20:32:50.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-27 20:32:50.000000 mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 20:32:50.564096 mypy-boto3-greengrassv2-1.26.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-01-27 20:32:13.000000 mypy-boto3-greengrassv2-1.26.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.043347 mypy-boto3-greengrassv2-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:38:40.000000 mypy-boto3-greengrassv2-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-07-03 19:50:50.035346 mypy-boto3-greengrassv2-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-07-03 19:38:40.000000 mypy-boto3-greengrassv2-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.031346 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-03 19:38:40.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-03 19:38:40.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:38:40.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25666 2023-07-03 19:38:40.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25623 2023-07-03 19:38:40.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-07-03 19:38:40.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-07-03 19:38:40.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-03 19:38:40.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-07-03 19:38:40.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:38:40.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37210 2023-07-03 19:38:42.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37177 2023-07-03 19:38:40.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:38:40.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.031346 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-07-03 19:50:49.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:50:49.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:49.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:49.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:49.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:50:49.000000 mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:50.043347 mypy-boto3-greengrassv2-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:38:39.000000 mypy-boto3-greengrassv2-1.27.0/setup.py
```

### Comparing `mypy-boto3-greengrassv2-1.26.59/LICENSE` & `mypy-boto3-greengrassv2-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-greengrassv2-1.26.59/PKG-INFO` & `mypy-boto3-greengrassv2-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrassv2
-Version: 1.26.59
-Summary: Type annotations for boto3.GreengrassV2 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.GreengrassV2 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-greengrassv2"></a>
 
 # mypy-boto3-greengrassv2
 
 [![PyPI - mypy-boto3-greengrassv2](https://img.shields.io/pypi/v/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-greengrassv2?color=blue)](https://pypistats.org/packages/mypy-boto3-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GreengrassV2 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[boto3.GreengrassV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [mypy-boto3-greengrassv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -369,73 +369,80 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_greengrassv2.type_defs import (
     AssociateClientDeviceWithCoreDeviceEntryTypeDef,
     AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateServiceRoleToAccountResponseTypeDef,
     AssociatedClientDeviceTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef,
     CancelDeploymentRequestRequestTypeDef,
+    CancelDeploymentResponseTypeDef,
     CloudComponentStatusTypeDef,
     ComponentCandidateTypeDef,
     ComponentConfigurationUpdateTypeDef,
     ComponentDependencyRequirementTypeDef,
     ComponentPlatformTypeDef,
     SystemResourceLimitsTypeDef,
     ComponentVersionListItemTypeDef,
     ConnectivityInfoTypeDef,
     CoreDeviceTypeDef,
+    CreateDeploymentResponseTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteCoreDeviceRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
     DeploymentComponentUpdatePolicyTypeDef,
     DeploymentConfigurationValidationPolicyTypeDef,
     IoTJobTimeoutConfigTypeDef,
     DeploymentTypeDef,
     DescribeComponentRequestRequestTypeDef,
+    DisassociateServiceRoleFromAccountResponseTypeDef,
     EffectiveDeploymentStatusDetailsTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetComponentRequestRequestTypeDef,
+    GetComponentResponseTypeDef,
     GetComponentVersionArtifactRequestRequestTypeDef,
+    GetComponentVersionArtifactResponseTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetCoreDeviceRequestRequestTypeDef,
+    GetCoreDeviceResponseTypeDef,
     GetDeploymentRequestRequestTypeDef,
+    GetServiceRoleForAccountResponseTypeDef,
     InstalledComponentTypeDef,
     IoTJobAbortCriteriaTypeDef,
     IoTJobRateIncreaseCriteriaTypeDef,
     LambdaDeviceMountTypeDef,
     LambdaVolumeMountTypeDef,
     LambdaEventSourceTypeDef,
-    PaginatorConfigTypeDef,
+    ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
+    ListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
     ListComponentVersionsRequestRequestTypeDef,
+    ListComponentsRequestListComponentsPaginateTypeDef,
     ListComponentsRequestRequestTypeDef,
+    ListCoreDevicesRequestListCoreDevicesPaginateTypeDef,
     ListCoreDevicesRequestRequestTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
+    ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
     ListEffectiveDeploymentsRequestRequestTypeDef,
+    ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
     ListInstalledComponentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     ResolvedComponentVersionTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateConnectivityInfoResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
-    AssociateServiceRoleToAccountResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef,
-    CancelDeploymentResponseTypeDef,
-    CreateDeploymentResponseTypeDef,
-    DisassociateServiceRoleFromAccountResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetComponentResponseTypeDef,
-    GetComponentVersionArtifactResponseTypeDef,
-    GetCoreDeviceResponseTypeDef,
-    GetServiceRoleForAccountResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateConnectivityInfoResponseTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     CreateComponentVersionResponseTypeDef,
     ComponentLatestVersionTypeDef,
     DescribeComponentResponseTypeDef,
     ResolveComponentCandidatesRequestRequestTypeDef,
@@ -447,21 +454,14 @@
     DeploymentPoliciesTypeDef,
     ListDeploymentsResponseTypeDef,
     EffectiveDeploymentTypeDef,
     ListInstalledComponentsResponseTypeDef,
     IoTJobAbortConfigTypeDef,
     IoTJobExponentialRolloutRateTypeDef,
     LambdaContainerParamsTypeDef,
-    ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
-    ListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
-    ListComponentsRequestListComponentsPaginateTypeDef,
-    ListCoreDevicesRequestListCoreDevicesPaginateTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
-    ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
     ResolveComponentCandidatesResponseTypeDef,
     ComponentTypeDef,
     ComponentDeploymentSpecificationTypeDef,
     ListEffectiveDeploymentsResponseTypeDef,
     IoTJobExecutionsRolloutConfigTypeDef,
     LambdaLinuxProcessParamsTypeDef,
     ListComponentsResponseTypeDef,
@@ -481,42 +481,42 @@
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

### Comparing `mypy-boto3-greengrassv2-1.26.59/README.md` & `mypy-boto3-greengrassv2-1.27.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-greengrassv2"></a>
 
 # mypy-boto3-greengrassv2
 
 [![PyPI - mypy-boto3-greengrassv2](https://img.shields.io/pypi/v/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-greengrassv2?color=blue)](https://pypistats.org/packages/mypy-boto3-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GreengrassV2 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[boto3.GreengrassV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [mypy-boto3-greengrassv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,73 +337,80 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_greengrassv2.type_defs import (
     AssociateClientDeviceWithCoreDeviceEntryTypeDef,
     AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateServiceRoleToAccountResponseTypeDef,
     AssociatedClientDeviceTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef,
     CancelDeploymentRequestRequestTypeDef,
+    CancelDeploymentResponseTypeDef,
     CloudComponentStatusTypeDef,
     ComponentCandidateTypeDef,
     ComponentConfigurationUpdateTypeDef,
     ComponentDependencyRequirementTypeDef,
     ComponentPlatformTypeDef,
     SystemResourceLimitsTypeDef,
     ComponentVersionListItemTypeDef,
     ConnectivityInfoTypeDef,
     CoreDeviceTypeDef,
+    CreateDeploymentResponseTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteCoreDeviceRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
     DeploymentComponentUpdatePolicyTypeDef,
     DeploymentConfigurationValidationPolicyTypeDef,
     IoTJobTimeoutConfigTypeDef,
     DeploymentTypeDef,
     DescribeComponentRequestRequestTypeDef,
+    DisassociateServiceRoleFromAccountResponseTypeDef,
     EffectiveDeploymentStatusDetailsTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetComponentRequestRequestTypeDef,
+    GetComponentResponseTypeDef,
     GetComponentVersionArtifactRequestRequestTypeDef,
+    GetComponentVersionArtifactResponseTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetCoreDeviceRequestRequestTypeDef,
+    GetCoreDeviceResponseTypeDef,
     GetDeploymentRequestRequestTypeDef,
+    GetServiceRoleForAccountResponseTypeDef,
     InstalledComponentTypeDef,
     IoTJobAbortCriteriaTypeDef,
     IoTJobRateIncreaseCriteriaTypeDef,
     LambdaDeviceMountTypeDef,
     LambdaVolumeMountTypeDef,
     LambdaEventSourceTypeDef,
-    PaginatorConfigTypeDef,
+    ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
+    ListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
     ListComponentVersionsRequestRequestTypeDef,
+    ListComponentsRequestListComponentsPaginateTypeDef,
     ListComponentsRequestRequestTypeDef,
+    ListCoreDevicesRequestListCoreDevicesPaginateTypeDef,
     ListCoreDevicesRequestRequestTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
+    ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
     ListEffectiveDeploymentsRequestRequestTypeDef,
+    ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
     ListInstalledComponentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     ResolvedComponentVersionTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateConnectivityInfoResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
-    AssociateServiceRoleToAccountResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef,
-    CancelDeploymentResponseTypeDef,
-    CreateDeploymentResponseTypeDef,
-    DisassociateServiceRoleFromAccountResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetComponentResponseTypeDef,
-    GetComponentVersionArtifactResponseTypeDef,
-    GetCoreDeviceResponseTypeDef,
-    GetServiceRoleForAccountResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateConnectivityInfoResponseTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     CreateComponentVersionResponseTypeDef,
     ComponentLatestVersionTypeDef,
     DescribeComponentResponseTypeDef,
     ResolveComponentCandidatesRequestRequestTypeDef,
@@ -415,21 +422,14 @@
     DeploymentPoliciesTypeDef,
     ListDeploymentsResponseTypeDef,
     EffectiveDeploymentTypeDef,
     ListInstalledComponentsResponseTypeDef,
     IoTJobAbortConfigTypeDef,
     IoTJobExponentialRolloutRateTypeDef,
     LambdaContainerParamsTypeDef,
-    ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
-    ListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
-    ListComponentsRequestListComponentsPaginateTypeDef,
-    ListCoreDevicesRequestListCoreDevicesPaginateTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
-    ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
     ResolveComponentCandidatesResponseTypeDef,
     ComponentTypeDef,
     ComponentDeploymentSpecificationTypeDef,
     ListEffectiveDeploymentsResponseTypeDef,
     IoTJobExecutionsRolloutConfigTypeDef,
     LambdaLinuxProcessParamsTypeDef,
     ListComponentsResponseTypeDef,
@@ -449,42 +449,42 @@
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

### Comparing `mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/__init__.py` & `mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/__init__.pyi` & `mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/__main__.py` & `mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GreengrassV2 1.26.59\nVersion:         1.26.59\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.GreengrassV2 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.59")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/client.py` & `mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/client.pyi` & `mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/literals.py` & `mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 ComponentVisibilityScopeType = Literal["PRIVATE", "PUBLIC"]
 CoreDeviceStatusType = Literal["HEALTHY", "UNHEALTHY"]
 DeploymentComponentUpdatePolicyActionType = Literal["NOTIFY_COMPONENTS", "SKIP_NOTIFY_COMPONENTS"]
 DeploymentFailureHandlingPolicyType = Literal["DO_NOTHING", "ROLLBACK"]
 DeploymentHistoryFilterType = Literal["ALL", "LATEST_ONLY"]
 DeploymentStatusType = Literal["ACTIVE", "CANCELED", "COMPLETED", "FAILED", "INACTIVE"]
 EffectiveDeploymentExecutionStatusType = Literal[
-    "CANCELED", "COMPLETED", "FAILED", "IN_PROGRESS", "QUEUED", "REJECTED", "TIMED_OUT"
+    "CANCELED", "COMPLETED", "FAILED", "IN_PROGRESS", "QUEUED", "REJECTED", "SUCCEEDED", "TIMED_OUT"
 ]
 InstalledComponentLifecycleStateType = Literal[
     "BROKEN", "ERRORED", "FINISHED", "INSTALLED", "NEW", "RUNNING", "STARTING", "STOPPING"
 ]
 InstalledComponentTopologyFilterType = Literal["ALL", "ROOT"]
 IoTJobAbortActionType = Literal["CANCEL"]
 IoTJobExecutionFailureTypeType = Literal["ALL", "FAILED", "REJECTED", "TIMED_OUT"]
@@ -98,14 +98,15 @@
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
@@ -137,21 +138,23 @@
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
@@ -230,14 +233,15 @@
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
@@ -248,14 +252,15 @@
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
@@ -291,14 +296,15 @@
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
@@ -317,16 +323,19 @@
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
@@ -406,18 +415,21 @@
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

### Comparing `mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/literals.pyi` & `mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 ComponentVisibilityScopeType = Literal["PRIVATE", "PUBLIC"]
 CoreDeviceStatusType = Literal["HEALTHY", "UNHEALTHY"]
 DeploymentComponentUpdatePolicyActionType = Literal["NOTIFY_COMPONENTS", "SKIP_NOTIFY_COMPONENTS"]
 DeploymentFailureHandlingPolicyType = Literal["DO_NOTHING", "ROLLBACK"]
 DeploymentHistoryFilterType = Literal["ALL", "LATEST_ONLY"]
 DeploymentStatusType = Literal["ACTIVE", "CANCELED", "COMPLETED", "FAILED", "INACTIVE"]
 EffectiveDeploymentExecutionStatusType = Literal[
-    "CANCELED", "COMPLETED", "FAILED", "IN_PROGRESS", "QUEUED", "REJECTED", "TIMED_OUT"
+    "CANCELED", "COMPLETED", "FAILED", "IN_PROGRESS", "QUEUED", "REJECTED", "SUCCEEDED", "TIMED_OUT"
 ]
 InstalledComponentLifecycleStateType = Literal[
     "BROKEN", "ERRORED", "FINISHED", "INSTALLED", "NEW", "RUNNING", "STARTING", "STOPPING"
 ]
 InstalledComponentTopologyFilterType = Literal["ALL", "ROOT"]
 IoTJobAbortActionType = Literal["CANCEL"]
 IoTJobExecutionFailureTypeType = Literal["ALL", "FAILED", "REJECTED", "TIMED_OUT"]
@@ -96,14 +96,15 @@
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
@@ -135,21 +136,23 @@
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
@@ -228,14 +231,15 @@
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
@@ -246,14 +250,15 @@
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
@@ -289,14 +294,15 @@
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
@@ -315,16 +321,19 @@
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
@@ -404,18 +413,21 @@
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

### Comparing `mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/paginator.py` & `mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,30 +76,30 @@
 class ListClientDevicesAssociatedWithCoreDevicePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listclientdevicesassociatedwithcoredevicepaginator)
     """
 
     def paginate(
-        self, *, coreDeviceThingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, coreDeviceThingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listclientdevicesassociatedwithcoredevicepaginator)
         """
 
 
 class ListComponentVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponentVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentversionspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentversionspaginator)
         """
 
 
@@ -109,15 +109,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentspaginator)
     """
 
     def paginate(
         self,
         *,
         scope: ComponentVisibilityScopeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentspaginator)
         """
 
 
@@ -128,15 +128,15 @@
     """
 
     def paginate(
         self,
         *,
         thingGroupArn: str = ...,
         status: CoreDeviceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCoreDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListCoreDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcoredevicespaginator)
         """
 
 
@@ -148,30 +148,30 @@
 
     def paginate(
         self,
         *,
         targetArn: str = ...,
         historyFilter: DeploymentHistoryFilterType = ...,
         parentTargetArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listdeploymentspaginator)
         """
 
 
 class ListEffectiveDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListEffectiveDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listeffectivedeploymentspaginator)
     """
 
     def paginate(
-        self, *, coreDeviceThingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, coreDeviceThingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEffectiveDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListEffectiveDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listeffectivedeploymentspaginator)
         """
 
 
@@ -182,13 +182,13 @@
     """
 
     def paginate(
         self,
         *,
         coreDeviceThingName: str,
         topologyFilter: InstalledComponentTopologyFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstalledComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListInstalledComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listinstalledcomponentspaginator)
         """
```

### Comparing `mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/paginator.pyi` & `mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -73,29 +73,29 @@
 class ListClientDevicesAssociatedWithCoreDevicePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listclientdevicesassociatedwithcoredevicepaginator)
     """
 
     def paginate(
-        self, *, coreDeviceThingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, coreDeviceThingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listclientdevicesassociatedwithcoredevicepaginator)
         """
 
 class ListComponentVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponentVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentversionspaginator)
     """
 
     def paginate(
-        self, *, arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentversionspaginator)
         """
 
 class ListComponentsPaginator(Paginator):
@@ -104,15 +104,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentspaginator)
     """
 
     def paginate(
         self,
         *,
         scope: ComponentVisibilityScopeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcomponentspaginator)
         """
 
 class ListCoreDevicesPaginator(Paginator):
@@ -122,15 +122,15 @@
     """
 
     def paginate(
         self,
         *,
         thingGroupArn: str = ...,
         status: CoreDeviceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCoreDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListCoreDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listcoredevicespaginator)
         """
 
 class ListDeploymentsPaginator(Paginator):
@@ -141,29 +141,29 @@
 
     def paginate(
         self,
         *,
         targetArn: str = ...,
         historyFilter: DeploymentHistoryFilterType = ...,
         parentTargetArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listdeploymentspaginator)
         """
 
 class ListEffectiveDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListEffectiveDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listeffectivedeploymentspaginator)
     """
 
     def paginate(
-        self, *, coreDeviceThingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, coreDeviceThingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEffectiveDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListEffectiveDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listeffectivedeploymentspaginator)
         """
 
 class ListInstalledComponentsPaginator(Paginator):
@@ -173,13 +173,13 @@
     """
 
     def paginate(
         self,
         *,
         coreDeviceThingName: str,
         topologyFilter: InstalledComponentTopologyFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInstalledComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListInstalledComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/paginators/#listinstalledcomponentspaginator)
         """
```

### Comparing `mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/type_defs.py` & `mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -43,78 +43,84 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     "AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateServiceRoleToAccountResponseTypeDef",
     "AssociatedClientDeviceTypeDef",
     "DisassociateClientDeviceFromCoreDeviceEntryTypeDef",
     "DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef",
     "CancelDeploymentRequestRequestTypeDef",
+    "CancelDeploymentResponseTypeDef",
     "CloudComponentStatusTypeDef",
     "ComponentCandidateTypeDef",
     "ComponentConfigurationUpdateTypeDef",
     "ComponentDependencyRequirementTypeDef",
     "ComponentPlatformTypeDef",
     "SystemResourceLimitsTypeDef",
     "ComponentVersionListItemTypeDef",
     "ConnectivityInfoTypeDef",
     "CoreDeviceTypeDef",
+    "CreateDeploymentResponseTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteCoreDeviceRequestRequestTypeDef",
     "DeleteDeploymentRequestRequestTypeDef",
     "DeploymentComponentUpdatePolicyTypeDef",
     "DeploymentConfigurationValidationPolicyTypeDef",
     "IoTJobTimeoutConfigTypeDef",
     "DeploymentTypeDef",
     "DescribeComponentRequestRequestTypeDef",
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
     "EffectiveDeploymentStatusDetailsTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetComponentRequestRequestTypeDef",
+    "GetComponentResponseTypeDef",
     "GetComponentVersionArtifactRequestRequestTypeDef",
+    "GetComponentVersionArtifactResponseTypeDef",
     "GetConnectivityInfoRequestRequestTypeDef",
     "GetCoreDeviceRequestRequestTypeDef",
+    "GetCoreDeviceResponseTypeDef",
     "GetDeploymentRequestRequestTypeDef",
+    "GetServiceRoleForAccountResponseTypeDef",
     "InstalledComponentTypeDef",
     "IoTJobAbortCriteriaTypeDef",
     "IoTJobRateIncreaseCriteriaTypeDef",
     "LambdaDeviceMountTypeDef",
     "LambdaVolumeMountTypeDef",
     "LambdaEventSourceTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef",
+    "ListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
     "ListComponentVersionsRequestRequestTypeDef",
+    "ListComponentsRequestListComponentsPaginateTypeDef",
     "ListComponentsRequestRequestTypeDef",
+    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
     "ListCoreDevicesRequestRequestTypeDef",
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
+    "ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
     "ListEffectiveDeploymentsRequestRequestTypeDef",
+    "ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
     "ListInstalledComponentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "ResolvedComponentVersionTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateConnectivityInfoResponseTypeDef",
     "BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef",
-    "AssociateServiceRoleToAccountResponseTypeDef",
     "BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef",
-    "CancelDeploymentResponseTypeDef",
-    "CreateDeploymentResponseTypeDef",
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetComponentResponseTypeDef",
-    "GetComponentVersionArtifactResponseTypeDef",
-    "GetCoreDeviceResponseTypeDef",
-    "GetServiceRoleForAccountResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateConnectivityInfoResponseTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     "CreateComponentVersionResponseTypeDef",
     "ComponentLatestVersionTypeDef",
     "DescribeComponentResponseTypeDef",
     "ResolveComponentCandidatesRequestRequestTypeDef",
@@ -126,21 +132,14 @@
     "DeploymentPoliciesTypeDef",
     "ListDeploymentsResponseTypeDef",
     "EffectiveDeploymentTypeDef",
     "ListInstalledComponentsResponseTypeDef",
     "IoTJobAbortConfigTypeDef",
     "IoTJobExponentialRolloutRateTypeDef",
     "LambdaContainerParamsTypeDef",
-    "ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
-    "ListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
-    "ListComponentsRequestListComponentsPaginateTypeDef",
-    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    "ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
-    "ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
     "ResolveComponentCandidatesResponseTypeDef",
     "ComponentTypeDef",
     "ComponentDeploymentSpecificationTypeDef",
     "ListEffectiveDeploymentsResponseTypeDef",
     "IoTJobExecutionsRolloutConfigTypeDef",
     "LambdaLinuxProcessParamsTypeDef",
     "ListComponentsResponseTypeDef",
@@ -172,22 +171,19 @@
 AssociateServiceRoleToAccountRequestRequestTypeDef = TypedDict(
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     {
         "roleArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
+    "AssociateServiceRoleToAccountResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "associatedAt": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociatedClientDeviceTypeDef = TypedDict(
     "AssociatedClientDeviceTypeDef",
     {
         "thingName": str,
@@ -216,14 +212,22 @@
 CancelDeploymentRequestRequestTypeDef = TypedDict(
     "CancelDeploymentRequestRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 
+CancelDeploymentResponseTypeDef = TypedDict(
+    "CancelDeploymentResponseTypeDef",
+    {
+        "message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CloudComponentStatusTypeDef = TypedDict(
     "CloudComponentStatusTypeDef",
     {
         "componentState": CloudComponentStateType,
         "message": str,
         "errors": Dict[str, str],
         "vendorGuidance": VendorGuidanceType,
@@ -305,14 +309,24 @@
         "coreDeviceThingName": str,
         "status": CoreDeviceStatusType,
         "lastStatusUpdateTimestamp": datetime,
     },
     total=False,
 )
 
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "deploymentId": str,
+        "iotJobId": str,
+        "iotJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteComponentRequestRequestTypeDef = TypedDict(
     "DeleteComponentRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -373,73 +387,127 @@
 DescribeComponentRequestRequestTypeDef = TypedDict(
     "DescribeComponentRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
+    {
+        "disassociatedAt": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EffectiveDeploymentStatusDetailsTypeDef = TypedDict(
     "EffectiveDeploymentStatusDetailsTypeDef",
     {
         "errorStack": List[str],
         "errorTypes": List[str],
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetComponentRequestRequestTypeDef = TypedDict(
     "_RequiredGetComponentRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalGetComponentRequestRequestTypeDef = TypedDict(
     "_OptionalGetComponentRequestRequestTypeDef",
     {
         "recipeOutputFormat": RecipeOutputFormatType,
     },
     total=False,
 )
 
-
 class GetComponentRequestRequestTypeDef(
     _RequiredGetComponentRequestRequestTypeDef, _OptionalGetComponentRequestRequestTypeDef
 ):
     pass
 
+GetComponentResponseTypeDef = TypedDict(
+    "GetComponentResponseTypeDef",
+    {
+        "recipeOutputFormat": RecipeOutputFormatType,
+        "recipe": bytes,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 GetComponentVersionArtifactRequestRequestTypeDef = TypedDict(
     "GetComponentVersionArtifactRequestRequestTypeDef",
     {
         "arn": str,
         "artifactName": str,
     },
 )
 
+GetComponentVersionArtifactResponseTypeDef = TypedDict(
+    "GetComponentVersionArtifactResponseTypeDef",
+    {
+        "preSignedUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetConnectivityInfoRequestRequestTypeDef = TypedDict(
     "GetConnectivityInfoRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 
 GetCoreDeviceRequestRequestTypeDef = TypedDict(
     "GetCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 
+GetCoreDeviceResponseTypeDef = TypedDict(
+    "GetCoreDeviceResponseTypeDef",
+    {
+        "coreDeviceThingName": str,
+        "coreVersion": str,
+        "platform": str,
+        "architecture": str,
+        "status": CoreDeviceStatusType,
+        "lastStatusUpdateTimestamp": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDeploymentRequestRequestTypeDef = TypedDict(
     "GetDeploymentRequestRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 
+GetServiceRoleForAccountResponseTypeDef = TypedDict(
+    "GetServiceRoleForAccountResponseTypeDef",
+    {
+        "associatedAt": str,
+        "roleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InstalledComponentTypeDef = TypedDict(
     "InstalledComponentTypeDef",
     {
         "componentName": str,
         "componentVersion": str,
         "lifecycleState": InstalledComponentLifecycleStateType,
         "lifecycleStateDetails": str,
@@ -482,21 +550,19 @@
     {
         "permission": LambdaFilesystemPermissionType,
         "addGroupOwner": bool,
     },
     total=False,
 )
 
-
 class LambdaDeviceMountTypeDef(
     _RequiredLambdaDeviceMountTypeDef, _OptionalLambdaDeviceMountTypeDef
 ):
     pass
 
-
 _RequiredLambdaVolumeMountTypeDef = TypedDict(
     "_RequiredLambdaVolumeMountTypeDef",
     {
         "sourcePath": str,
         "destinationPath": str,
     },
 )
@@ -505,39 +571,47 @@
     {
         "permission": LambdaFilesystemPermissionType,
         "addGroupOwner": bool,
     },
     total=False,
 )
 
-
 class LambdaVolumeMountTypeDef(
     _RequiredLambdaVolumeMountTypeDef, _OptionalLambdaVolumeMountTypeDef
 ):
     pass
 
-
 LambdaEventSourceTypeDef = TypedDict(
     "LambdaEventSourceTypeDef",
     {
         "topic": str,
         "type": LambdaEventSourceTypeType,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
+    "_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "coreDeviceThingName": str,
+    },
+)
+_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
+    "_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef(
+    _RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
+    _OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
+):
+    pass
+
 _RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef = TypedDict(
@@ -545,21 +619,39 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef(
     _RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
     _OptionalListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListComponentVersionsRequestListComponentVersionsPaginateTypeDef(
+    _RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
+    _OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
+):
+    pass
 
 _RequiredListComponentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentVersionsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
@@ -568,55 +660,103 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListComponentVersionsRequestRequestTypeDef(
     _RequiredListComponentVersionsRequestRequestTypeDef,
     _OptionalListComponentVersionsRequestRequestTypeDef,
 ):
     pass
 
+ListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
+    "ListComponentsRequestListComponentsPaginateTypeDef",
+    {
+        "scope": ComponentVisibilityScopeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListComponentsRequestRequestTypeDef = TypedDict(
     "ListComponentsRequestRequestTypeDef",
     {
         "scope": ComponentVisibilityScopeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListCoreDevicesRequestListCoreDevicesPaginateTypeDef = TypedDict(
+    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
+    {
+        "thingGroupArn": str,
+        "status": CoreDeviceStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCoreDevicesRequestRequestTypeDef = TypedDict(
     "ListCoreDevicesRequestRequestTypeDef",
     {
         "thingGroupArn": str,
         "status": CoreDeviceStatusType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "targetArn": str,
+        "historyFilter": DeploymentHistoryFilterType,
+        "parentTargetArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDeploymentsRequestRequestTypeDef = TypedDict(
     "ListDeploymentsRequestRequestTypeDef",
     {
         "targetArn": str,
         "historyFilter": DeploymentHistoryFilterType,
         "parentTargetArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
+    {
+        "coreDeviceThingName": str,
+    },
+)
+_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef(
+    _RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
+    _OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
+):
+    pass
+
 _RequiredListEffectiveDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListEffectiveDeploymentsRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListEffectiveDeploymentsRequestRequestTypeDef = TypedDict(
@@ -624,21 +764,40 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListEffectiveDeploymentsRequestRequestTypeDef(
     _RequiredListEffectiveDeploymentsRequestRequestTypeDef,
     _OptionalListEffectiveDeploymentsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
+    "_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
+    {
+        "coreDeviceThingName": str,
+    },
+)
+_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
+    "_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
+    {
+        "topologyFilter": InstalledComponentTopologyFilterType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef(
+    _RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
+    _OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
+):
+    pass
 
 _RequiredListInstalledComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListInstalledComponentsRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
@@ -648,42 +807,69 @@
         "maxResults": int,
         "nextToken": str,
         "topologyFilter": InstalledComponentTopologyFilterType,
     },
     total=False,
 )
 
-
 class ListInstalledComponentsRequestRequestTypeDef(
     _RequiredListInstalledComponentsRequestRequestTypeDef,
     _OptionalListInstalledComponentsRequestRequestTypeDef,
 ):
     pass
 
-
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
 ResolvedComponentVersionTypeDef = TypedDict(
     "ResolvedComponentVersionTypeDef",
     {
         "arn": str,
         "componentName": str,
         "componentVersion": str,
         "recipe": bytes,
         "vendorGuidance": VendorGuidanceType,
         "message": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -692,149 +878,57 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateConnectivityInfoResponseTypeDef = TypedDict(
+    "UpdateConnectivityInfoResponseTypeDef",
+    {
+        "version": str,
+        "message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef = TypedDict(
     "_OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef",
     {
         "entries": Sequence[AssociateClientDeviceWithCoreDeviceEntryTypeDef],
     },
     total=False,
 )
 
-
 class BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef(
     _RequiredBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
     _OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
-
-AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
-    "AssociateServiceRoleToAccountResponseTypeDef",
-    {
-        "associatedAt": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef = TypedDict(
     "BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef",
     {
         "errorEntries": List[AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelDeploymentResponseTypeDef = TypedDict(
-    "CancelDeploymentResponseTypeDef",
-    {
-        "message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "deploymentId": str,
-        "iotJobId": str,
-        "iotJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
-    {
-        "disassociatedAt": str,
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
-GetComponentResponseTypeDef = TypedDict(
-    "GetComponentResponseTypeDef",
-    {
-        "recipeOutputFormat": RecipeOutputFormatType,
-        "recipe": bytes,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetComponentVersionArtifactResponseTypeDef = TypedDict(
-    "GetComponentVersionArtifactResponseTypeDef",
-    {
-        "preSignedUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCoreDeviceResponseTypeDef = TypedDict(
-    "GetCoreDeviceResponseTypeDef",
-    {
-        "coreDeviceThingName": str,
-        "coreVersion": str,
-        "platform": str,
-        "architecture": str,
-        "status": CoreDeviceStatusType,
-        "lastStatusUpdateTimestamp": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetServiceRoleForAccountResponseTypeDef = TypedDict(
-    "GetServiceRoleForAccountResponseTypeDef",
-    {
-        "associatedAt": str,
-        "roleArn": str,
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
-UpdateConnectivityInfoResponseTypeDef = TypedDict(
-    "UpdateConnectivityInfoResponseTypeDef",
-    {
-        "version": str,
-        "message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef = TypedDict(
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     {
         "associatedClientDevices": List[AssociatedClientDeviceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
@@ -844,39 +938,37 @@
     "_OptionalBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     {
         "entries": Sequence[DisassociateClientDeviceFromCoreDeviceEntryTypeDef],
     },
     total=False,
 )
 
-
 class BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef(
     _RequiredBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     _OptionalBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
-
 BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef = TypedDict(
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     {
         "errorEntries": List[DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateComponentVersionResponseTypeDef = TypedDict(
     "CreateComponentVersionResponseTypeDef",
     {
         "arn": str,
         "componentName": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "status": CloudComponentStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ComponentLatestVersionTypeDef = TypedDict(
     "ComponentLatestVersionTypeDef",
     {
         "arn": str,
@@ -897,15 +989,15 @@
         "componentVersion": str,
         "creationTimestamp": datetime,
         "publisher": str,
         "description": str,
         "status": CloudComponentStatusTypeDef,
         "platforms": List[ComponentPlatformTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResolveComponentCandidatesRequestRequestTypeDef = TypedDict(
     "ResolveComponentCandidatesRequestRequestTypeDef",
     {
         "platform": ComponentPlatformTypeDef,
@@ -925,24 +1017,24 @@
 )
 
 ListComponentVersionsResponseTypeDef = TypedDict(
     "ListComponentVersionsResponseTypeDef",
     {
         "componentVersions": List[ComponentVersionListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConnectivityInfoResponseTypeDef = TypedDict(
     "GetConnectivityInfoResponseTypeDef",
     {
         "connectivityInfo": List[ConnectivityInfoTypeDef],
         "message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConnectivityInfoRequestRequestTypeDef = TypedDict(
     "UpdateConnectivityInfoRequestRequestTypeDef",
     {
         "thingName": str,
@@ -951,15 +1043,15 @@
 )
 
 ListCoreDevicesResponseTypeDef = TypedDict(
     "ListCoreDevicesResponseTypeDef",
     {
         "coreDevices": List[CoreDeviceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentPoliciesTypeDef = TypedDict(
     "DeploymentPoliciesTypeDef",
     {
         "failureHandlingPolicy": DeploymentFailureHandlingPolicyType,
@@ -970,15 +1062,15 @@
 )
 
 ListDeploymentsResponseTypeDef = TypedDict(
     "ListDeploymentsResponseTypeDef",
     {
         "deployments": List[DeploymentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEffectiveDeploymentTypeDef = TypedDict(
     "_RequiredEffectiveDeploymentTypeDef",
     {
         "deploymentId": str,
@@ -997,27 +1089,25 @@
         "description": str,
         "reason": str,
         "statusDetails": EffectiveDeploymentStatusDetailsTypeDef,
     },
     total=False,
 )
 
-
 class EffectiveDeploymentTypeDef(
     _RequiredEffectiveDeploymentTypeDef, _OptionalEffectiveDeploymentTypeDef
 ):
     pass
 
-
 ListInstalledComponentsResponseTypeDef = TypedDict(
     "ListInstalledComponentsResponseTypeDef",
     {
         "installedComponents": List[InstalledComponentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IoTJobAbortConfigTypeDef = TypedDict(
     "IoTJobAbortConfigTypeDef",
     {
         "criteriaList": Sequence[IoTJobAbortCriteriaTypeDef],
@@ -1040,138 +1130,19 @@
         "mountROSysfs": bool,
         "volumes": Sequence[LambdaVolumeMountTypeDef],
         "devices": Sequence[LambdaDeviceMountTypeDef],
     },
     total=False,
 )
 
-_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
-    "_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
-    {
-        "coreDeviceThingName": str,
-    },
-)
-_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
-    "_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef(
-    _RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
-    _OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
-):
-    pass
-
-
-_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListComponentVersionsRequestListComponentVersionsPaginateTypeDef(
-    _RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
-    _OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
-    "ListComponentsRequestListComponentsPaginateTypeDef",
-    {
-        "scope": ComponentVisibilityScopeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCoreDevicesRequestListCoreDevicesPaginateTypeDef = TypedDict(
-    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
-    {
-        "thingGroupArn": str,
-        "status": CoreDeviceStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "targetArn": str,
-        "historyFilter": DeploymentHistoryFilterType,
-        "parentTargetArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
-    {
-        "coreDeviceThingName": str,
-    },
-)
-_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef(
-    _RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
-    _OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
-    "_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
-    {
-        "coreDeviceThingName": str,
-    },
-)
-_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
-    "_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
-    {
-        "topologyFilter": InstalledComponentTopologyFilterType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef(
-    _RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
-    _OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
-):
-    pass
-
-
 ResolveComponentCandidatesResponseTypeDef = TypedDict(
     "ResolveComponentCandidatesResponseTypeDef",
     {
         "resolvedComponentVersions": List[ResolvedComponentVersionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ComponentTypeDef = TypedDict(
     "ComponentTypeDef",
     {
         "arn": str,
@@ -1192,15 +1163,15 @@
 )
 
 ListEffectiveDeploymentsResponseTypeDef = TypedDict(
     "ListEffectiveDeploymentsResponseTypeDef",
     {
         "effectiveDeployments": List[EffectiveDeploymentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IoTJobExecutionsRolloutConfigTypeDef = TypedDict(
     "IoTJobExecutionsRolloutConfigTypeDef",
     {
         "exponentialRate": IoTJobExponentialRolloutRateTypeDef,
@@ -1219,15 +1190,15 @@
 )
 
 ListComponentsResponseTypeDef = TypedDict(
     "ListComponentsResponseTypeDef",
     {
         "components": List[ComponentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentIoTJobConfigurationTypeDef = TypedDict(
     "DeploymentIoTJobConfigurationTypeDef",
     {
         "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigTypeDef,
@@ -1271,21 +1242,19 @@
         "parentTargetArn": str,
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-
 GetDeploymentResponseTypeDef = TypedDict(
     "GetDeploymentResponseTypeDef",
     {
         "targetArn": str,
         "revisionId": str,
         "deploymentId": str,
         "deploymentName": str,
@@ -1295,15 +1264,15 @@
         "components": Dict[str, ComponentDeploymentSpecificationTypeDef],
         "deploymentPolicies": DeploymentPoliciesTypeDef,
         "iotJobConfiguration": DeploymentIoTJobConfigurationTypeDef,
         "creationTimestamp": datetime,
         "isLatestForTarget": bool,
         "parentTargetArn": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredLambdaFunctionRecipeSourceTypeDef = TypedDict(
     "_RequiredLambdaFunctionRecipeSourceTypeDef",
     {
         "lambdaArn": str,
@@ -1317,21 +1286,19 @@
         "componentPlatforms": Sequence[ComponentPlatformTypeDef],
         "componentDependencies": Mapping[str, ComponentDependencyRequirementTypeDef],
         "componentLambdaParameters": LambdaExecutionParametersTypeDef,
     },
     total=False,
 )
 
-
 class LambdaFunctionRecipeSourceTypeDef(
     _RequiredLambdaFunctionRecipeSourceTypeDef, _OptionalLambdaFunctionRecipeSourceTypeDef
 ):
     pass
 
-
 CreateComponentVersionRequestRequestTypeDef = TypedDict(
     "CreateComponentVersionRequestRequestTypeDef",
     {
         "inlineRecipe": Union[str, bytes, IO[Any], StreamingBody],
         "lambdaFunction": LambdaFunctionRecipeSourceTypeDef,
         "tags": Mapping[str, str],
         "clientToken": str,
```

### Comparing `mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2/type_defs.pyi` & `mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,77 +43,85 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     "AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateServiceRoleToAccountResponseTypeDef",
     "AssociatedClientDeviceTypeDef",
     "DisassociateClientDeviceFromCoreDeviceEntryTypeDef",
     "DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef",
     "CancelDeploymentRequestRequestTypeDef",
+    "CancelDeploymentResponseTypeDef",
     "CloudComponentStatusTypeDef",
     "ComponentCandidateTypeDef",
     "ComponentConfigurationUpdateTypeDef",
     "ComponentDependencyRequirementTypeDef",
     "ComponentPlatformTypeDef",
     "SystemResourceLimitsTypeDef",
     "ComponentVersionListItemTypeDef",
     "ConnectivityInfoTypeDef",
     "CoreDeviceTypeDef",
+    "CreateDeploymentResponseTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteCoreDeviceRequestRequestTypeDef",
     "DeleteDeploymentRequestRequestTypeDef",
     "DeploymentComponentUpdatePolicyTypeDef",
     "DeploymentConfigurationValidationPolicyTypeDef",
     "IoTJobTimeoutConfigTypeDef",
     "DeploymentTypeDef",
     "DescribeComponentRequestRequestTypeDef",
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
     "EffectiveDeploymentStatusDetailsTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetComponentRequestRequestTypeDef",
+    "GetComponentResponseTypeDef",
     "GetComponentVersionArtifactRequestRequestTypeDef",
+    "GetComponentVersionArtifactResponseTypeDef",
     "GetConnectivityInfoRequestRequestTypeDef",
     "GetCoreDeviceRequestRequestTypeDef",
+    "GetCoreDeviceResponseTypeDef",
     "GetDeploymentRequestRequestTypeDef",
+    "GetServiceRoleForAccountResponseTypeDef",
     "InstalledComponentTypeDef",
     "IoTJobAbortCriteriaTypeDef",
     "IoTJobRateIncreaseCriteriaTypeDef",
     "LambdaDeviceMountTypeDef",
     "LambdaVolumeMountTypeDef",
     "LambdaEventSourceTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef",
+    "ListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
     "ListComponentVersionsRequestRequestTypeDef",
+    "ListComponentsRequestListComponentsPaginateTypeDef",
     "ListComponentsRequestRequestTypeDef",
+    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
     "ListCoreDevicesRequestRequestTypeDef",
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
+    "ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
     "ListEffectiveDeploymentsRequestRequestTypeDef",
+    "ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
     "ListInstalledComponentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "ResolvedComponentVersionTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateConnectivityInfoResponseTypeDef",
     "BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef",
-    "AssociateServiceRoleToAccountResponseTypeDef",
     "BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef",
-    "CancelDeploymentResponseTypeDef",
-    "CreateDeploymentResponseTypeDef",
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetComponentResponseTypeDef",
-    "GetComponentVersionArtifactResponseTypeDef",
-    "GetCoreDeviceResponseTypeDef",
-    "GetServiceRoleForAccountResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "UpdateConnectivityInfoResponseTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     "CreateComponentVersionResponseTypeDef",
     "ComponentLatestVersionTypeDef",
     "DescribeComponentResponseTypeDef",
     "ResolveComponentCandidatesRequestRequestTypeDef",
@@ -125,21 +133,14 @@
     "DeploymentPoliciesTypeDef",
     "ListDeploymentsResponseTypeDef",
     "EffectiveDeploymentTypeDef",
     "ListInstalledComponentsResponseTypeDef",
     "IoTJobAbortConfigTypeDef",
     "IoTJobExponentialRolloutRateTypeDef",
     "LambdaContainerParamsTypeDef",
-    "ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
-    "ListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
-    "ListComponentsRequestListComponentsPaginateTypeDef",
-    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    "ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
-    "ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
     "ResolveComponentCandidatesResponseTypeDef",
     "ComponentTypeDef",
     "ComponentDeploymentSpecificationTypeDef",
     "ListEffectiveDeploymentsResponseTypeDef",
     "IoTJobExecutionsRolloutConfigTypeDef",
     "LambdaLinuxProcessParamsTypeDef",
     "ListComponentsResponseTypeDef",
@@ -171,22 +172,19 @@
 AssociateServiceRoleToAccountRequestRequestTypeDef = TypedDict(
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     {
         "roleArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
+    "AssociateServiceRoleToAccountResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "associatedAt": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociatedClientDeviceTypeDef = TypedDict(
     "AssociatedClientDeviceTypeDef",
     {
         "thingName": str,
@@ -215,14 +213,22 @@
 CancelDeploymentRequestRequestTypeDef = TypedDict(
     "CancelDeploymentRequestRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 
+CancelDeploymentResponseTypeDef = TypedDict(
+    "CancelDeploymentResponseTypeDef",
+    {
+        "message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CloudComponentStatusTypeDef = TypedDict(
     "CloudComponentStatusTypeDef",
     {
         "componentState": CloudComponentStateType,
         "message": str,
         "errors": Dict[str, str],
         "vendorGuidance": VendorGuidanceType,
@@ -304,14 +310,24 @@
         "coreDeviceThingName": str,
         "status": CoreDeviceStatusType,
         "lastStatusUpdateTimestamp": datetime,
     },
     total=False,
 )
 
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "deploymentId": str,
+        "iotJobId": str,
+        "iotJobArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteComponentRequestRequestTypeDef = TypedDict(
     "DeleteComponentRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -372,71 +388,129 @@
 DescribeComponentRequestRequestTypeDef = TypedDict(
     "DescribeComponentRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
+    "DisassociateServiceRoleFromAccountResponseTypeDef",
+    {
+        "disassociatedAt": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EffectiveDeploymentStatusDetailsTypeDef = TypedDict(
     "EffectiveDeploymentStatusDetailsTypeDef",
     {
         "errorStack": List[str],
         "errorTypes": List[str],
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetComponentRequestRequestTypeDef = TypedDict(
     "_RequiredGetComponentRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalGetComponentRequestRequestTypeDef = TypedDict(
     "_OptionalGetComponentRequestRequestTypeDef",
     {
         "recipeOutputFormat": RecipeOutputFormatType,
     },
     total=False,
 )
 
+
 class GetComponentRequestRequestTypeDef(
     _RequiredGetComponentRequestRequestTypeDef, _OptionalGetComponentRequestRequestTypeDef
 ):
     pass
 
+
+GetComponentResponseTypeDef = TypedDict(
+    "GetComponentResponseTypeDef",
+    {
+        "recipeOutputFormat": RecipeOutputFormatType,
+        "recipe": bytes,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetComponentVersionArtifactRequestRequestTypeDef = TypedDict(
     "GetComponentVersionArtifactRequestRequestTypeDef",
     {
         "arn": str,
         "artifactName": str,
     },
 )
 
+GetComponentVersionArtifactResponseTypeDef = TypedDict(
+    "GetComponentVersionArtifactResponseTypeDef",
+    {
+        "preSignedUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetConnectivityInfoRequestRequestTypeDef = TypedDict(
     "GetConnectivityInfoRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 
 GetCoreDeviceRequestRequestTypeDef = TypedDict(
     "GetCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 
+GetCoreDeviceResponseTypeDef = TypedDict(
+    "GetCoreDeviceResponseTypeDef",
+    {
+        "coreDeviceThingName": str,
+        "coreVersion": str,
+        "platform": str,
+        "architecture": str,
+        "status": CoreDeviceStatusType,
+        "lastStatusUpdateTimestamp": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDeploymentRequestRequestTypeDef = TypedDict(
     "GetDeploymentRequestRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 
+GetServiceRoleForAccountResponseTypeDef = TypedDict(
+    "GetServiceRoleForAccountResponseTypeDef",
+    {
+        "associatedAt": str,
+        "roleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InstalledComponentTypeDef = TypedDict(
     "InstalledComponentTypeDef",
     {
         "componentName": str,
         "componentVersion": str,
         "lifecycleState": InstalledComponentLifecycleStateType,
         "lifecycleStateDetails": str,
@@ -479,19 +553,21 @@
     {
         "permission": LambdaFilesystemPermissionType,
         "addGroupOwner": bool,
     },
     total=False,
 )
 
+
 class LambdaDeviceMountTypeDef(
     _RequiredLambdaDeviceMountTypeDef, _OptionalLambdaDeviceMountTypeDef
 ):
     pass
 
+
 _RequiredLambdaVolumeMountTypeDef = TypedDict(
     "_RequiredLambdaVolumeMountTypeDef",
     {
         "sourcePath": str,
         "destinationPath": str,
     },
 )
@@ -500,37 +576,51 @@
     {
         "permission": LambdaFilesystemPermissionType,
         "addGroupOwner": bool,
     },
     total=False,
 )
 
+
 class LambdaVolumeMountTypeDef(
     _RequiredLambdaVolumeMountTypeDef, _OptionalLambdaVolumeMountTypeDef
 ):
     pass
 
+
 LambdaEventSourceTypeDef = TypedDict(
     "LambdaEventSourceTypeDef",
     {
         "topic": str,
         "type": LambdaEventSourceTypeType,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
+    "_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "coreDeviceThingName": str,
+    },
+)
+_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
+    "_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef(
+    _RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
+    _OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef = TypedDict(
@@ -538,20 +628,44 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef(
     _RequiredListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
     _OptionalListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
+    {
+        "arn": str,
+    },
+)
+_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListComponentVersionsRequestListComponentVersionsPaginateTypeDef(
+    _RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
+    _OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListComponentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentVersionsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListComponentVersionsRequestRequestTypeDef = TypedDict(
@@ -559,53 +673,107 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListComponentVersionsRequestRequestTypeDef(
     _RequiredListComponentVersionsRequestRequestTypeDef,
     _OptionalListComponentVersionsRequestRequestTypeDef,
 ):
     pass
 
+
+ListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
+    "ListComponentsRequestListComponentsPaginateTypeDef",
+    {
+        "scope": ComponentVisibilityScopeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListComponentsRequestRequestTypeDef = TypedDict(
     "ListComponentsRequestRequestTypeDef",
     {
         "scope": ComponentVisibilityScopeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListCoreDevicesRequestListCoreDevicesPaginateTypeDef = TypedDict(
+    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
+    {
+        "thingGroupArn": str,
+        "status": CoreDeviceStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCoreDevicesRequestRequestTypeDef = TypedDict(
     "ListCoreDevicesRequestRequestTypeDef",
     {
         "thingGroupArn": str,
         "status": CoreDeviceStatusType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "targetArn": str,
+        "historyFilter": DeploymentHistoryFilterType,
+        "parentTargetArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDeploymentsRequestRequestTypeDef = TypedDict(
     "ListDeploymentsRequestRequestTypeDef",
     {
         "targetArn": str,
         "historyFilter": DeploymentHistoryFilterType,
         "parentTargetArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
+    {
+        "coreDeviceThingName": str,
+    },
+)
+_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef(
+    _RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
+    _OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListEffectiveDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListEffectiveDeploymentsRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListEffectiveDeploymentsRequestRequestTypeDef = TypedDict(
@@ -613,20 +781,45 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListEffectiveDeploymentsRequestRequestTypeDef(
     _RequiredListEffectiveDeploymentsRequestRequestTypeDef,
     _OptionalListEffectiveDeploymentsRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
+    "_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
+    {
+        "coreDeviceThingName": str,
+    },
+)
+_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
+    "_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
+    {
+        "topologyFilter": InstalledComponentTopologyFilterType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef(
+    _RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
+    _OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListInstalledComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListInstalledComponentsRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalListInstalledComponentsRequestRequestTypeDef = TypedDict(
@@ -635,40 +828,71 @@
         "maxResults": int,
         "nextToken": str,
         "topologyFilter": InstalledComponentTopologyFilterType,
     },
     total=False,
 )
 
+
 class ListInstalledComponentsRequestRequestTypeDef(
     _RequiredListInstalledComponentsRequestRequestTypeDef,
     _OptionalListInstalledComponentsRequestRequestTypeDef,
 ):
     pass
 
+
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
 ResolvedComponentVersionTypeDef = TypedDict(
     "ResolvedComponentVersionTypeDef",
     {
         "arn": str,
         "componentName": str,
         "componentVersion": str,
         "recipe": bytes,
         "vendorGuidance": VendorGuidanceType,
         "message": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -677,147 +901,59 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateConnectivityInfoResponseTypeDef = TypedDict(
+    "UpdateConnectivityInfoResponseTypeDef",
+    {
+        "version": str,
+        "message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
     },
 )
 _OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef = TypedDict(
     "_OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef",
     {
         "entries": Sequence[AssociateClientDeviceWithCoreDeviceEntryTypeDef],
     },
     total=False,
 )
 
+
 class BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef(
     _RequiredBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
     _OptionalBatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
-AssociateServiceRoleToAccountResponseTypeDef = TypedDict(
-    "AssociateServiceRoleToAccountResponseTypeDef",
-    {
-        "associatedAt": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef = TypedDict(
     "BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef",
     {
         "errorEntries": List[AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelDeploymentResponseTypeDef = TypedDict(
-    "CancelDeploymentResponseTypeDef",
-    {
-        "message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "deploymentId": str,
-        "iotJobId": str,
-        "iotJobArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateServiceRoleFromAccountResponseTypeDef = TypedDict(
-    "DisassociateServiceRoleFromAccountResponseTypeDef",
-    {
-        "disassociatedAt": str,
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
-GetComponentResponseTypeDef = TypedDict(
-    "GetComponentResponseTypeDef",
-    {
-        "recipeOutputFormat": RecipeOutputFormatType,
-        "recipe": bytes,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetComponentVersionArtifactResponseTypeDef = TypedDict(
-    "GetComponentVersionArtifactResponseTypeDef",
-    {
-        "preSignedUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCoreDeviceResponseTypeDef = TypedDict(
-    "GetCoreDeviceResponseTypeDef",
-    {
-        "coreDeviceThingName": str,
-        "coreVersion": str,
-        "platform": str,
-        "architecture": str,
-        "status": CoreDeviceStatusType,
-        "lastStatusUpdateTimestamp": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetServiceRoleForAccountResponseTypeDef = TypedDict(
-    "GetServiceRoleForAccountResponseTypeDef",
-    {
-        "associatedAt": str,
-        "roleArn": str,
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
-UpdateConnectivityInfoResponseTypeDef = TypedDict(
-    "UpdateConnectivityInfoResponseTypeDef",
-    {
-        "version": str,
-        "message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef = TypedDict(
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     {
         "associatedClientDevices": List[AssociatedClientDeviceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     {
         "coreDeviceThingName": str,
@@ -827,37 +963,39 @@
     "_OptionalBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     {
         "entries": Sequence[DisassociateClientDeviceFromCoreDeviceEntryTypeDef],
     },
     total=False,
 )
 
+
 class BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef(
     _RequiredBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     _OptionalBatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
 ):
     pass
 
+
 BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef = TypedDict(
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     {
         "errorEntries": List[DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateComponentVersionResponseTypeDef = TypedDict(
     "CreateComponentVersionResponseTypeDef",
     {
         "arn": str,
         "componentName": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "status": CloudComponentStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ComponentLatestVersionTypeDef = TypedDict(
     "ComponentLatestVersionTypeDef",
     {
         "arn": str,
@@ -878,15 +1016,15 @@
         "componentVersion": str,
         "creationTimestamp": datetime,
         "publisher": str,
         "description": str,
         "status": CloudComponentStatusTypeDef,
         "platforms": List[ComponentPlatformTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResolveComponentCandidatesRequestRequestTypeDef = TypedDict(
     "ResolveComponentCandidatesRequestRequestTypeDef",
     {
         "platform": ComponentPlatformTypeDef,
@@ -906,24 +1044,24 @@
 )
 
 ListComponentVersionsResponseTypeDef = TypedDict(
     "ListComponentVersionsResponseTypeDef",
     {
         "componentVersions": List[ComponentVersionListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConnectivityInfoResponseTypeDef = TypedDict(
     "GetConnectivityInfoResponseTypeDef",
     {
         "connectivityInfo": List[ConnectivityInfoTypeDef],
         "message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateConnectivityInfoRequestRequestTypeDef = TypedDict(
     "UpdateConnectivityInfoRequestRequestTypeDef",
     {
         "thingName": str,
@@ -932,15 +1070,15 @@
 )
 
 ListCoreDevicesResponseTypeDef = TypedDict(
     "ListCoreDevicesResponseTypeDef",
     {
         "coreDevices": List[CoreDeviceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentPoliciesTypeDef = TypedDict(
     "DeploymentPoliciesTypeDef",
     {
         "failureHandlingPolicy": DeploymentFailureHandlingPolicyType,
@@ -951,15 +1089,15 @@
 )
 
 ListDeploymentsResponseTypeDef = TypedDict(
     "ListDeploymentsResponseTypeDef",
     {
         "deployments": List[DeploymentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredEffectiveDeploymentTypeDef = TypedDict(
     "_RequiredEffectiveDeploymentTypeDef",
     {
         "deploymentId": str,
@@ -978,25 +1116,27 @@
         "description": str,
         "reason": str,
         "statusDetails": EffectiveDeploymentStatusDetailsTypeDef,
     },
     total=False,
 )
 
+
 class EffectiveDeploymentTypeDef(
     _RequiredEffectiveDeploymentTypeDef, _OptionalEffectiveDeploymentTypeDef
 ):
     pass
 
+
 ListInstalledComponentsResponseTypeDef = TypedDict(
     "ListInstalledComponentsResponseTypeDef",
     {
         "installedComponents": List[InstalledComponentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IoTJobAbortConfigTypeDef = TypedDict(
     "IoTJobAbortConfigTypeDef",
     {
         "criteriaList": Sequence[IoTJobAbortCriteriaTypeDef],
@@ -1019,130 +1159,19 @@
         "mountROSysfs": bool,
         "volumes": Sequence[LambdaVolumeMountTypeDef],
         "devices": Sequence[LambdaDeviceMountTypeDef],
     },
     total=False,
 )
 
-_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
-    "_RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
-    {
-        "coreDeviceThingName": str,
-    },
-)
-_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef = TypedDict(
-    "_OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef(
-    _RequiredListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
-    _OptionalListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
-):
-    pass
-
-_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
-    {
-        "arn": str,
-    },
-)
-_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListComponentVersionsRequestListComponentVersionsPaginateTypeDef(
-    _RequiredListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
-    _OptionalListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
-):
-    pass
-
-ListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
-    "ListComponentsRequestListComponentsPaginateTypeDef",
-    {
-        "scope": ComponentVisibilityScopeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListCoreDevicesRequestListCoreDevicesPaginateTypeDef = TypedDict(
-    "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
-    {
-        "thingGroupArn": str,
-        "status": CoreDeviceStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "targetArn": str,
-        "historyFilter": DeploymentHistoryFilterType,
-        "parentTargetArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
-    {
-        "coreDeviceThingName": str,
-    },
-)
-_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef(
-    _RequiredListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
-    _OptionalListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
-):
-    pass
-
-_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
-    "_RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
-    {
-        "coreDeviceThingName": str,
-    },
-)
-_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef = TypedDict(
-    "_OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
-    {
-        "topologyFilter": InstalledComponentTopologyFilterType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef(
-    _RequiredListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
-    _OptionalListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
-):
-    pass
-
 ResolveComponentCandidatesResponseTypeDef = TypedDict(
     "ResolveComponentCandidatesResponseTypeDef",
     {
         "resolvedComponentVersions": List[ResolvedComponentVersionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ComponentTypeDef = TypedDict(
     "ComponentTypeDef",
     {
         "arn": str,
@@ -1163,15 +1192,15 @@
 )
 
 ListEffectiveDeploymentsResponseTypeDef = TypedDict(
     "ListEffectiveDeploymentsResponseTypeDef",
     {
         "effectiveDeployments": List[EffectiveDeploymentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IoTJobExecutionsRolloutConfigTypeDef = TypedDict(
     "IoTJobExecutionsRolloutConfigTypeDef",
     {
         "exponentialRate": IoTJobExponentialRolloutRateTypeDef,
@@ -1190,15 +1219,15 @@
 )
 
 ListComponentsResponseTypeDef = TypedDict(
     "ListComponentsResponseTypeDef",
     {
         "components": List[ComponentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentIoTJobConfigurationTypeDef = TypedDict(
     "DeploymentIoTJobConfigurationTypeDef",
     {
         "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigTypeDef,
@@ -1242,19 +1271,21 @@
         "parentTargetArn": str,
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
+
 GetDeploymentResponseTypeDef = TypedDict(
     "GetDeploymentResponseTypeDef",
     {
         "targetArn": str,
         "revisionId": str,
         "deploymentId": str,
         "deploymentName": str,
@@ -1264,15 +1295,15 @@
         "components": Dict[str, ComponentDeploymentSpecificationTypeDef],
         "deploymentPolicies": DeploymentPoliciesTypeDef,
         "iotJobConfiguration": DeploymentIoTJobConfigurationTypeDef,
         "creationTimestamp": datetime,
         "isLatestForTarget": bool,
         "parentTargetArn": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredLambdaFunctionRecipeSourceTypeDef = TypedDict(
     "_RequiredLambdaFunctionRecipeSourceTypeDef",
     {
         "lambdaArn": str,
@@ -1286,19 +1317,21 @@
         "componentPlatforms": Sequence[ComponentPlatformTypeDef],
         "componentDependencies": Mapping[str, ComponentDependencyRequirementTypeDef],
         "componentLambdaParameters": LambdaExecutionParametersTypeDef,
     },
     total=False,
 )
 
+
 class LambdaFunctionRecipeSourceTypeDef(
     _RequiredLambdaFunctionRecipeSourceTypeDef, _OptionalLambdaFunctionRecipeSourceTypeDef
 ):
     pass
 
+
 CreateComponentVersionRequestRequestTypeDef = TypedDict(
     "CreateComponentVersionRequestRequestTypeDef",
     {
         "inlineRecipe": Union[str, bytes, IO[Any], StreamingBody],
         "lambdaFunction": LambdaFunctionRecipeSourceTypeDef,
         "tags": Mapping[str, str],
         "clientToken": str,
```

### Comparing `mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2.egg-info/PKG-INFO` & `mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrassv2
-Version: 1.26.59
-Summary: Type annotations for boto3.GreengrassV2 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.GreengrassV2 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-greengrassv2"></a>
 
 # mypy-boto3-greengrassv2
 
 [![PyPI - mypy-boto3-greengrassv2](https://img.shields.io/pypi/v/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-greengrassv2?color=blue)](https://pypistats.org/packages/mypy-boto3-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GreengrassV2 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[boto3.GreengrassV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [mypy-boto3-greengrassv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -369,73 +369,80 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_greengrassv2.type_defs import (
     AssociateClientDeviceWithCoreDeviceEntryTypeDef,
     AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateServiceRoleToAccountResponseTypeDef,
     AssociatedClientDeviceTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef,
     CancelDeploymentRequestRequestTypeDef,
+    CancelDeploymentResponseTypeDef,
     CloudComponentStatusTypeDef,
     ComponentCandidateTypeDef,
     ComponentConfigurationUpdateTypeDef,
     ComponentDependencyRequirementTypeDef,
     ComponentPlatformTypeDef,
     SystemResourceLimitsTypeDef,
     ComponentVersionListItemTypeDef,
     ConnectivityInfoTypeDef,
     CoreDeviceTypeDef,
+    CreateDeploymentResponseTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteCoreDeviceRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
     DeploymentComponentUpdatePolicyTypeDef,
     DeploymentConfigurationValidationPolicyTypeDef,
     IoTJobTimeoutConfigTypeDef,
     DeploymentTypeDef,
     DescribeComponentRequestRequestTypeDef,
+    DisassociateServiceRoleFromAccountResponseTypeDef,
     EffectiveDeploymentStatusDetailsTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetComponentRequestRequestTypeDef,
+    GetComponentResponseTypeDef,
     GetComponentVersionArtifactRequestRequestTypeDef,
+    GetComponentVersionArtifactResponseTypeDef,
     GetConnectivityInfoRequestRequestTypeDef,
     GetCoreDeviceRequestRequestTypeDef,
+    GetCoreDeviceResponseTypeDef,
     GetDeploymentRequestRequestTypeDef,
+    GetServiceRoleForAccountResponseTypeDef,
     InstalledComponentTypeDef,
     IoTJobAbortCriteriaTypeDef,
     IoTJobRateIncreaseCriteriaTypeDef,
     LambdaDeviceMountTypeDef,
     LambdaVolumeMountTypeDef,
     LambdaEventSourceTypeDef,
-    PaginatorConfigTypeDef,
+    ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceRequestRequestTypeDef,
+    ListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
     ListComponentVersionsRequestRequestTypeDef,
+    ListComponentsRequestListComponentsPaginateTypeDef,
     ListComponentsRequestRequestTypeDef,
+    ListCoreDevicesRequestListCoreDevicesPaginateTypeDef,
     ListCoreDevicesRequestRequestTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
+    ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
     ListEffectiveDeploymentsRequestRequestTypeDef,
+    ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
     ListInstalledComponentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     ResolvedComponentVersionTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateConnectivityInfoResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceRequestRequestTypeDef,
-    AssociateServiceRoleToAccountResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef,
-    CancelDeploymentResponseTypeDef,
-    CreateDeploymentResponseTypeDef,
-    DisassociateServiceRoleFromAccountResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetComponentResponseTypeDef,
-    GetComponentVersionArtifactResponseTypeDef,
-    GetCoreDeviceResponseTypeDef,
-    GetServiceRoleForAccountResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateConnectivityInfoResponseTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     CreateComponentVersionResponseTypeDef,
     ComponentLatestVersionTypeDef,
     DescribeComponentResponseTypeDef,
     ResolveComponentCandidatesRequestRequestTypeDef,
@@ -447,21 +454,14 @@
     DeploymentPoliciesTypeDef,
     ListDeploymentsResponseTypeDef,
     EffectiveDeploymentTypeDef,
     ListInstalledComponentsResponseTypeDef,
     IoTJobAbortConfigTypeDef,
     IoTJobExponentialRolloutRateTypeDef,
     LambdaContainerParamsTypeDef,
-    ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef,
-    ListComponentVersionsRequestListComponentVersionsPaginateTypeDef,
-    ListComponentsRequestListComponentsPaginateTypeDef,
-    ListCoreDevicesRequestListCoreDevicesPaginateTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef,
-    ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef,
     ResolveComponentCandidatesResponseTypeDef,
     ComponentTypeDef,
     ComponentDeploymentSpecificationTypeDef,
     ListEffectiveDeploymentsResponseTypeDef,
     IoTJobExecutionsRolloutConfigTypeDef,
     LambdaLinuxProcessParamsTypeDef,
     ListComponentsResponseTypeDef,
@@ -481,42 +481,42 @@
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

### Comparing `mypy-boto3-greengrassv2-1.26.59/mypy_boto3_greengrassv2.egg-info/SOURCES.txt` & `mypy-boto3-greengrassv2-1.27.0/mypy_boto3_greengrassv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.26.59/setup.py` & `mypy-boto3-greengrassv2-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-greengrassv2.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-greengrassv2",
-    version="1.26.59",
+    version="1.27.0",
     packages=["mypy_boto3_greengrassv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GreengrassV2 1.26.59 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.GreengrassV2 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/",
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


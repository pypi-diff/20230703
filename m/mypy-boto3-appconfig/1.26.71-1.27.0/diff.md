# Comparing `tmp/mypy-boto3-appconfig-1.26.71.tar.gz` & `tmp/mypy-boto3-appconfig-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appconfig-1.26.71.tar", last modified: Tue Feb 14 20:27:05 2023, max compression
+gzip compressed data, was "mypy-boto3-appconfig-1.27.0.tar", last modified: Mon Jul  3 19:50:20 2023, max compression
```

## Comparing `mypy-boto3-appconfig-1.26.71.tar` & `mypy-boto3-appconfig-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:27:05.966803 mypy-boto3-appconfig-1.26.71/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-14 20:26:12.000000 mypy-boto3-appconfig-1.26.71/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-02-14 20:27:05.962803 mypy-boto3-appconfig-1.26.71/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13691 2023-02-14 20:26:12.000000 mypy-boto3-appconfig-1.26.71/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:27:05.962803 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-14 20:26:12.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-14 20:26:12.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-14 20:26:12.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29069 2023-02-14 20:26:12.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29020 2023-02-14 20:26:12.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-02-14 20:26:12.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-02-14 20:26:12.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 20:26:12.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31158 2023-02-14 20:26:13.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31113 2023-02-14 20:26:13.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-14 20:26:12.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 20:27:05.962803 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-02-14 20:27:05.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-02-14 20:27:05.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 20:27:05.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 20:27:05.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-14 20:27:05.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-14 20:27:05.000000 mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 20:27:05.966803 mypy-boto3-appconfig-1.26.71/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-14 20:26:12.000000 mypy-boto3-appconfig-1.26.71/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:20.342781 mypy-boto3-appconfig-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:22.000000 mypy-boto3-appconfig-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-03 19:50:20.342781 mypy-boto3-appconfig-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-07-03 19:32:22.000000 mypy-boto3-appconfig-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:20.338781 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-03 19:32:22.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 19:32:22.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:32:22.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29069 2023-07-03 19:32:22.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29020 2023-07-03 19:32:22.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-07-03 19:32:23.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-07-03 19:32:23.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:22.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31196 2023-07-03 19:32:24.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31151 2023-07-03 19:32:24.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:22.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:20.342781 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-03 19:50:20.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-03 19:50:20.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:20.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:20.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:20.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:50:20.000000 mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:20.342781 mypy-boto3-appconfig-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:32:22.000000 mypy-boto3-appconfig-1.27.0/setup.py
```

### Comparing `mypy-boto3-appconfig-1.26.71/LICENSE` & `mypy-boto3-appconfig-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-appconfig-1.26.71/PKG-INFO` & `mypy-boto3-appconfig-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appconfig
-Version: 1.26.71
-Summary: Type annotations for boto3.AppConfig 1.26.71 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.AppConfig 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-appconfig"></a>
 
 # mypy-boto3-appconfig
 
 [![PyPI - mypy-boto3-appconfig](https://img.shields.io/pypi/v/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appconfig?color=blue)](https://pypistats.org/packages/mypy-boto3-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfig 1.26.71](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[boto3.AppConfig 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [mypy-boto3-appconfig docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,71 +305,71 @@
 `mypy_boto3_appconfig.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appconfig.type_defs import (
     ActionInvocationTypeDef,
     ActionTypeDef,
-    ResponseMetadataTypeDef,
+    ApplicationResponseMetadataTypeDef,
     ApplicationTypeDef,
     AppliedExtensionTypeDef,
     ConfigurationProfileSummaryTypeDef,
     ValidatorTypeDef,
+    ConfigurationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateDeploymentStrategyRequestRequestTypeDef,
     MonitorTypeDef,
     CreateExtensionAssociationRequestRequestTypeDef,
     ParameterTypeDef,
     CreateHostedConfigurationVersionRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteConfigurationProfileRequestRequestTypeDef,
     DeleteDeploymentStrategyRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteExtensionAssociationRequestRequestTypeDef,
     DeleteExtensionRequestRequestTypeDef,
     DeleteHostedConfigurationVersionRequestRequestTypeDef,
     DeploymentStrategyTypeDef,
+    DeploymentStrategyResponseMetadataTypeDef,
     DeploymentSummaryTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExtensionAssociationSummaryTypeDef,
+    ExtensionAssociationTypeDef,
     ExtensionSummaryTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetConfigurationProfileRequestRequestTypeDef,
     GetConfigurationRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetDeploymentStrategyRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetExtensionAssociationRequestRequestTypeDef,
     GetExtensionRequestRequestTypeDef,
     GetHostedConfigurationVersionRequestRequestTypeDef,
     HostedConfigurationVersionSummaryTypeDef,
+    HostedConfigurationVersionTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListConfigurationProfilesRequestRequestTypeDef,
     ListDeploymentStrategiesRequestRequestTypeDef,
     ListDeploymentsRequestRequestTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListExtensionAssociationsRequestRequestTypeDef,
     ListExtensionsRequestRequestTypeDef,
     ListHostedConfigurationVersionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ResourceTagsTypeDef,
+    ResponseMetadataTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StopDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateDeploymentStrategyRequestRequestTypeDef,
     UpdateExtensionAssociationRequestRequestTypeDef,
     ValidateConfigurationRequestRequestTypeDef,
     DeploymentEventTypeDef,
-    ApplicationResponseMetadataTypeDef,
-    ConfigurationTypeDef,
-    DeploymentStrategyResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExtensionAssociationTypeDef,
-    HostedConfigurationVersionTypeDef,
-    ResourceTagsTypeDef,
     ApplicationsTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     CreateConfigurationProfileRequestRequestTypeDef,
     UpdateConfigurationProfileRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     EnvironmentResponseMetadataTypeDef,
@@ -395,42 +395,42 @@
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

### Comparing `mypy-boto3-appconfig-1.26.71/README.md` & `mypy-boto3-appconfig-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-appconfig"></a>
 
 # mypy-boto3-appconfig
 
 [![PyPI - mypy-boto3-appconfig](https://img.shields.io/pypi/v/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appconfig?color=blue)](https://pypistats.org/packages/mypy-boto3-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfig 1.26.71](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[boto3.AppConfig 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [mypy-boto3-appconfig docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/).
 
 See how it helps to find and fix potential bugs:
 
@@ -273,71 +273,71 @@
 `mypy_boto3_appconfig.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appconfig.type_defs import (
     ActionInvocationTypeDef,
     ActionTypeDef,
-    ResponseMetadataTypeDef,
+    ApplicationResponseMetadataTypeDef,
     ApplicationTypeDef,
     AppliedExtensionTypeDef,
     ConfigurationProfileSummaryTypeDef,
     ValidatorTypeDef,
+    ConfigurationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateDeploymentStrategyRequestRequestTypeDef,
     MonitorTypeDef,
     CreateExtensionAssociationRequestRequestTypeDef,
     ParameterTypeDef,
     CreateHostedConfigurationVersionRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteConfigurationProfileRequestRequestTypeDef,
     DeleteDeploymentStrategyRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteExtensionAssociationRequestRequestTypeDef,
     DeleteExtensionRequestRequestTypeDef,
     DeleteHostedConfigurationVersionRequestRequestTypeDef,
     DeploymentStrategyTypeDef,
+    DeploymentStrategyResponseMetadataTypeDef,
     DeploymentSummaryTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExtensionAssociationSummaryTypeDef,
+    ExtensionAssociationTypeDef,
     ExtensionSummaryTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetConfigurationProfileRequestRequestTypeDef,
     GetConfigurationRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetDeploymentStrategyRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetExtensionAssociationRequestRequestTypeDef,
     GetExtensionRequestRequestTypeDef,
     GetHostedConfigurationVersionRequestRequestTypeDef,
     HostedConfigurationVersionSummaryTypeDef,
+    HostedConfigurationVersionTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListConfigurationProfilesRequestRequestTypeDef,
     ListDeploymentStrategiesRequestRequestTypeDef,
     ListDeploymentsRequestRequestTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListExtensionAssociationsRequestRequestTypeDef,
     ListExtensionsRequestRequestTypeDef,
     ListHostedConfigurationVersionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ResourceTagsTypeDef,
+    ResponseMetadataTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StopDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateDeploymentStrategyRequestRequestTypeDef,
     UpdateExtensionAssociationRequestRequestTypeDef,
     ValidateConfigurationRequestRequestTypeDef,
     DeploymentEventTypeDef,
-    ApplicationResponseMetadataTypeDef,
-    ConfigurationTypeDef,
-    DeploymentStrategyResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExtensionAssociationTypeDef,
-    HostedConfigurationVersionTypeDef,
-    ResourceTagsTypeDef,
     ApplicationsTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     CreateConfigurationProfileRequestRequestTypeDef,
     UpdateConfigurationProfileRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     EnvironmentResponseMetadataTypeDef,
@@ -363,42 +363,42 @@
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

### Comparing `mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/__main__.py` & `mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppConfig 1.26.71\nVersion:         1.26.71\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.AppConfig 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.71")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/client.py` & `mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/client.pyi` & `mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/literals.py` & `mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ActionPointType",
     "DeploymentEventTypeType",
     "DeploymentStateType",
     "EnvironmentStateType",
     "GrowthTypeType",
     "ReplicateToType",
@@ -30,15 +29,14 @@
     "ValidatorTypeType",
     "AppConfigServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ActionPointType = Literal[
     "ON_DEPLOYMENT_BAKING",
     "ON_DEPLOYMENT_COMPLETE",
     "ON_DEPLOYMENT_ROLLED_BACK",
     "ON_DEPLOYMENT_START",
     "ON_DEPLOYMENT_STEP",
     "PRE_CREATE_HOSTED_CONFIGURATION_VERSION",
@@ -72,14 +70,15 @@
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
@@ -119,14 +118,15 @@
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
@@ -205,14 +205,15 @@
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
@@ -223,14 +224,15 @@
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
@@ -266,14 +268,15 @@
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
@@ -292,16 +295,19 @@
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
@@ -381,18 +387,21 @@
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

### Comparing `mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/literals.pyi` & `mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ActionPointType",
     "DeploymentEventTypeType",
     "DeploymentStateType",
     "EnvironmentStateType",
     "GrowthTypeType",
     "ReplicateToType",
@@ -29,14 +30,15 @@
     "ValidatorTypeType",
     "AppConfigServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 ActionPointType = Literal[
     "ON_DEPLOYMENT_BAKING",
     "ON_DEPLOYMENT_COMPLETE",
     "ON_DEPLOYMENT_ROLLED_BACK",
     "ON_DEPLOYMENT_START",
     "ON_DEPLOYMENT_STEP",
     "PRE_CREATE_HOSTED_CONFIGURATION_VERSION",
@@ -70,14 +72,15 @@
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
@@ -117,14 +120,15 @@
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
@@ -203,14 +207,15 @@
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
@@ -221,14 +226,15 @@
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
@@ -264,14 +270,15 @@
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
@@ -290,16 +297,19 @@
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
@@ -379,18 +389,21 @@
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

### Comparing `mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/type_defs.py` & `mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,71 +33,71 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ActionInvocationTypeDef",
     "ActionTypeDef",
-    "ResponseMetadataTypeDef",
+    "ApplicationResponseMetadataTypeDef",
     "ApplicationTypeDef",
     "AppliedExtensionTypeDef",
     "ConfigurationProfileSummaryTypeDef",
     "ValidatorTypeDef",
+    "ConfigurationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateDeploymentStrategyRequestRequestTypeDef",
     "MonitorTypeDef",
     "CreateExtensionAssociationRequestRequestTypeDef",
     "ParameterTypeDef",
     "CreateHostedConfigurationVersionRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteConfigurationProfileRequestRequestTypeDef",
     "DeleteDeploymentStrategyRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteExtensionAssociationRequestRequestTypeDef",
     "DeleteExtensionRequestRequestTypeDef",
     "DeleteHostedConfigurationVersionRequestRequestTypeDef",
     "DeploymentStrategyTypeDef",
+    "DeploymentStrategyResponseMetadataTypeDef",
     "DeploymentSummaryTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExtensionAssociationSummaryTypeDef",
+    "ExtensionAssociationTypeDef",
     "ExtensionSummaryTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetConfigurationProfileRequestRequestTypeDef",
     "GetConfigurationRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
     "GetDeploymentStrategyRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetExtensionAssociationRequestRequestTypeDef",
     "GetExtensionRequestRequestTypeDef",
     "GetHostedConfigurationVersionRequestRequestTypeDef",
     "HostedConfigurationVersionSummaryTypeDef",
+    "HostedConfigurationVersionTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListConfigurationProfilesRequestRequestTypeDef",
     "ListDeploymentStrategiesRequestRequestTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListExtensionAssociationsRequestRequestTypeDef",
     "ListExtensionsRequestRequestTypeDef",
     "ListHostedConfigurationVersionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ResourceTagsTypeDef",
+    "ResponseMetadataTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StopDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateDeploymentStrategyRequestRequestTypeDef",
     "UpdateExtensionAssociationRequestRequestTypeDef",
     "ValidateConfigurationRequestRequestTypeDef",
     "DeploymentEventTypeDef",
-    "ApplicationResponseMetadataTypeDef",
-    "ConfigurationTypeDef",
-    "DeploymentStrategyResponseMetadataTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExtensionAssociationTypeDef",
-    "HostedConfigurationVersionTypeDef",
-    "ResourceTagsTypeDef",
     "ApplicationsTypeDef",
     "ConfigurationProfilesTypeDef",
     "ConfigurationProfileTypeDef",
     "CreateConfigurationProfileRequestRequestTypeDef",
     "UpdateConfigurationProfileRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "EnvironmentResponseMetadataTypeDef",
@@ -136,22 +136,21 @@
         "Description": str,
         "Uri": str,
         "RoleArn": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ApplicationResponseMetadataTypeDef = TypedDict(
+    "ApplicationResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Id": str,
@@ -189,14 +188,24 @@
     "ValidatorTypeDef",
     {
         "Type": ValidatorTypeType,
         "Content": str,
     },
 )
 
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
+    {
+        "Content": StreamingBody,
+        "ConfigurationVersion": str,
+        "ContentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
@@ -401,14 +410,29 @@
         "GrowthFactor": float,
         "FinalBakeTimeInMinutes": int,
         "ReplicateTo": ReplicateToType,
     },
     total=False,
 )
 
+DeploymentStrategyResponseMetadataTypeDef = TypedDict(
+    "DeploymentStrategyResponseMetadataTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "DeploymentDurationInMinutes": int,
+        "GrowthType": GrowthTypeType,
+        "GrowthFactor": float,
+        "FinalBakeTimeInMinutes": int,
+        "ReplicateTo": ReplicateToType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeploymentSummaryTypeDef = TypedDict(
     "DeploymentSummaryTypeDef",
     {
         "DeploymentNumber": int,
         "ConfigurationName": str,
         "ConfigurationVersion": str,
         "DeploymentDurationInMinutes": int,
@@ -419,24 +443,44 @@
         "PercentageComplete": float,
         "StartedAt": datetime,
         "CompletedAt": datetime,
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
 ExtensionAssociationSummaryTypeDef = TypedDict(
     "ExtensionAssociationSummaryTypeDef",
     {
         "Id": str,
         "ExtensionArn": str,
         "ResourceArn": str,
     },
     total=False,
 )
 
+ExtensionAssociationTypeDef = TypedDict(
+    "ExtensionAssociationTypeDef",
+    {
+        "Id": str,
+        "ExtensionArn": str,
+        "ResourceArn": str,
+        "Arn": str,
+        "Parameters": Dict[str, str],
+        "ExtensionVersionNumber": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExtensionSummaryTypeDef = TypedDict(
     "ExtensionSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "VersionNumber": int,
         "Arn": str,
@@ -554,14 +598,28 @@
         "Description": str,
         "ContentType": str,
         "VersionLabel": str,
     },
     total=False,
 )
 
+HostedConfigurationVersionTypeDef = TypedDict(
+    "HostedConfigurationVersionTypeDef",
+    {
+        "ApplicationId": str,
+        "ConfigurationProfileId": str,
+        "VersionNumber": int,
+        "Description": str,
+        "Content": StreamingBody,
+        "ContentType": str,
+        "VersionLabel": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -695,14 +753,33 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ResourceTagsTypeDef = TypedDict(
+    "ResourceTagsTypeDef",
+    {
+        "Tags": Dict[str, str],
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
 _RequiredStartDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartDeploymentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EnvironmentId": str,
         "DeploymentStrategyId": str,
         "ConfigurationProfileId": str,
@@ -838,121 +915,44 @@
         "Description": str,
         "ActionInvocations": List[ActionInvocationTypeDef],
         "OccurredAt": datetime,
     },
     total=False,
 )
 
-ApplicationResponseMetadataTypeDef = TypedDict(
-    "ApplicationResponseMetadataTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
-    {
-        "Content": StreamingBody,
-        "ConfigurationVersion": str,
-        "ContentType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeploymentStrategyResponseMetadataTypeDef = TypedDict(
-    "DeploymentStrategyResponseMetadataTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "DeploymentDurationInMinutes": int,
-        "GrowthType": GrowthTypeType,
-        "GrowthFactor": float,
-        "FinalBakeTimeInMinutes": int,
-        "ReplicateTo": ReplicateToType,
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
-ExtensionAssociationTypeDef = TypedDict(
-    "ExtensionAssociationTypeDef",
-    {
-        "Id": str,
-        "ExtensionArn": str,
-        "ResourceArn": str,
-        "Arn": str,
-        "Parameters": Dict[str, str],
-        "ExtensionVersionNumber": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-HostedConfigurationVersionTypeDef = TypedDict(
-    "HostedConfigurationVersionTypeDef",
-    {
-        "ApplicationId": str,
-        "ConfigurationProfileId": str,
-        "VersionNumber": int,
-        "Description": str,
-        "Content": StreamingBody,
-        "ContentType": str,
-        "VersionLabel": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ResourceTagsTypeDef = TypedDict(
-    "ResourceTagsTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ApplicationsTypeDef = TypedDict(
     "ApplicationsTypeDef",
     {
         "Items": List[ApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigurationProfilesTypeDef = TypedDict(
     "ConfigurationProfilesTypeDef",
     {
         "Items": List[ConfigurationProfileSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigurationProfileTypeDef = TypedDict(
     "ConfigurationProfileTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "LocationUri": str,
         "RetrievalRoleArn": str,
         "Validators": List[ValidatorTypeDef],
         "Type": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateConfigurationProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationProfileRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -1035,15 +1035,15 @@
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "State": EnvironmentStateType,
         "Monitors": List[MonitorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "ApplicationId": str,
@@ -1111,15 +1111,15 @@
         "Id": str,
         "Name": str,
         "VersionNumber": int,
         "Arn": str,
         "Description": str,
         "Actions": Dict[ActionPointType, List[ActionTypeDef]],
         "Parameters": Dict[str, ParameterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateExtensionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExtensionRequestRequestTypeDef",
     {
         "ExtensionIdentifier": str,
@@ -1144,51 +1144,51 @@
 
 
 DeploymentStrategiesTypeDef = TypedDict(
     "DeploymentStrategiesTypeDef",
     {
         "Items": List[DeploymentStrategyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentsTypeDef = TypedDict(
     "DeploymentsTypeDef",
     {
         "Items": List[DeploymentSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExtensionAssociationsTypeDef = TypedDict(
     "ExtensionAssociationsTypeDef",
     {
         "Items": List[ExtensionAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExtensionsTypeDef = TypedDict(
     "ExtensionsTypeDef",
     {
         "Items": List[ExtensionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HostedConfigurationVersionsTypeDef = TypedDict(
     "HostedConfigurationVersionsTypeDef",
     {
         "Items": List[HostedConfigurationVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "ApplicationId": str,
@@ -1208,19 +1208,19 @@
         "EventLog": List[DeploymentEventTypeDef],
         "PercentageComplete": float,
         "StartedAt": datetime,
         "CompletedAt": datetime,
         "AppliedExtensions": List[AppliedExtensionTypeDef],
         "KmsKeyArn": str,
         "KmsKeyIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentsTypeDef = TypedDict(
     "EnvironmentsTypeDef",
     {
         "Items": List[EnvironmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig/type_defs.pyi` & `mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,71 +32,71 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActionInvocationTypeDef",
     "ActionTypeDef",
-    "ResponseMetadataTypeDef",
+    "ApplicationResponseMetadataTypeDef",
     "ApplicationTypeDef",
     "AppliedExtensionTypeDef",
     "ConfigurationProfileSummaryTypeDef",
     "ValidatorTypeDef",
+    "ConfigurationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateDeploymentStrategyRequestRequestTypeDef",
     "MonitorTypeDef",
     "CreateExtensionAssociationRequestRequestTypeDef",
     "ParameterTypeDef",
     "CreateHostedConfigurationVersionRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteConfigurationProfileRequestRequestTypeDef",
     "DeleteDeploymentStrategyRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteExtensionAssociationRequestRequestTypeDef",
     "DeleteExtensionRequestRequestTypeDef",
     "DeleteHostedConfigurationVersionRequestRequestTypeDef",
     "DeploymentStrategyTypeDef",
+    "DeploymentStrategyResponseMetadataTypeDef",
     "DeploymentSummaryTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExtensionAssociationSummaryTypeDef",
+    "ExtensionAssociationTypeDef",
     "ExtensionSummaryTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetConfigurationProfileRequestRequestTypeDef",
     "GetConfigurationRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
     "GetDeploymentStrategyRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetExtensionAssociationRequestRequestTypeDef",
     "GetExtensionRequestRequestTypeDef",
     "GetHostedConfigurationVersionRequestRequestTypeDef",
     "HostedConfigurationVersionSummaryTypeDef",
+    "HostedConfigurationVersionTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListConfigurationProfilesRequestRequestTypeDef",
     "ListDeploymentStrategiesRequestRequestTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListExtensionAssociationsRequestRequestTypeDef",
     "ListExtensionsRequestRequestTypeDef",
     "ListHostedConfigurationVersionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ResourceTagsTypeDef",
+    "ResponseMetadataTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StopDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateDeploymentStrategyRequestRequestTypeDef",
     "UpdateExtensionAssociationRequestRequestTypeDef",
     "ValidateConfigurationRequestRequestTypeDef",
     "DeploymentEventTypeDef",
-    "ApplicationResponseMetadataTypeDef",
-    "ConfigurationTypeDef",
-    "DeploymentStrategyResponseMetadataTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExtensionAssociationTypeDef",
-    "HostedConfigurationVersionTypeDef",
-    "ResourceTagsTypeDef",
     "ApplicationsTypeDef",
     "ConfigurationProfilesTypeDef",
     "ConfigurationProfileTypeDef",
     "CreateConfigurationProfileRequestRequestTypeDef",
     "UpdateConfigurationProfileRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "EnvironmentResponseMetadataTypeDef",
@@ -135,22 +135,21 @@
         "Description": str,
         "Uri": str,
         "RoleArn": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ApplicationResponseMetadataTypeDef = TypedDict(
+    "ApplicationResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Id": str,
@@ -188,14 +187,24 @@
     "ValidatorTypeDef",
     {
         "Type": ValidatorTypeType,
         "Content": str,
     },
 )
 
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
+    {
+        "Content": StreamingBody,
+        "ConfigurationVersion": str,
+        "ContentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateApplicationRequestRequestTypeDef = TypedDict(
@@ -388,14 +397,29 @@
         "GrowthFactor": float,
         "FinalBakeTimeInMinutes": int,
         "ReplicateTo": ReplicateToType,
     },
     total=False,
 )
 
+DeploymentStrategyResponseMetadataTypeDef = TypedDict(
+    "DeploymentStrategyResponseMetadataTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "DeploymentDurationInMinutes": int,
+        "GrowthType": GrowthTypeType,
+        "GrowthFactor": float,
+        "FinalBakeTimeInMinutes": int,
+        "ReplicateTo": ReplicateToType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeploymentSummaryTypeDef = TypedDict(
     "DeploymentSummaryTypeDef",
     {
         "DeploymentNumber": int,
         "ConfigurationName": str,
         "ConfigurationVersion": str,
         "DeploymentDurationInMinutes": int,
@@ -406,24 +430,44 @@
         "PercentageComplete": float,
         "StartedAt": datetime,
         "CompletedAt": datetime,
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
 ExtensionAssociationSummaryTypeDef = TypedDict(
     "ExtensionAssociationSummaryTypeDef",
     {
         "Id": str,
         "ExtensionArn": str,
         "ResourceArn": str,
     },
     total=False,
 )
 
+ExtensionAssociationTypeDef = TypedDict(
+    "ExtensionAssociationTypeDef",
+    {
+        "Id": str,
+        "ExtensionArn": str,
+        "ResourceArn": str,
+        "Arn": str,
+        "Parameters": Dict[str, str],
+        "ExtensionVersionNumber": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExtensionSummaryTypeDef = TypedDict(
     "ExtensionSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "VersionNumber": int,
         "Arn": str,
@@ -537,14 +581,28 @@
         "Description": str,
         "ContentType": str,
         "VersionLabel": str,
     },
     total=False,
 )
 
+HostedConfigurationVersionTypeDef = TypedDict(
+    "HostedConfigurationVersionTypeDef",
+    {
+        "ApplicationId": str,
+        "ConfigurationProfileId": str,
+        "VersionNumber": int,
+        "Description": str,
+        "Content": StreamingBody,
+        "ContentType": str,
+        "VersionLabel": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -670,14 +728,33 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ResourceTagsTypeDef = TypedDict(
+    "ResourceTagsTypeDef",
+    {
+        "Tags": Dict[str, str],
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
 _RequiredStartDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartDeploymentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EnvironmentId": str,
         "DeploymentStrategyId": str,
         "ConfigurationProfileId": str,
@@ -805,121 +882,44 @@
         "Description": str,
         "ActionInvocations": List[ActionInvocationTypeDef],
         "OccurredAt": datetime,
     },
     total=False,
 )
 
-ApplicationResponseMetadataTypeDef = TypedDict(
-    "ApplicationResponseMetadataTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
-    {
-        "Content": StreamingBody,
-        "ConfigurationVersion": str,
-        "ContentType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeploymentStrategyResponseMetadataTypeDef = TypedDict(
-    "DeploymentStrategyResponseMetadataTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "DeploymentDurationInMinutes": int,
-        "GrowthType": GrowthTypeType,
-        "GrowthFactor": float,
-        "FinalBakeTimeInMinutes": int,
-        "ReplicateTo": ReplicateToType,
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
-ExtensionAssociationTypeDef = TypedDict(
-    "ExtensionAssociationTypeDef",
-    {
-        "Id": str,
-        "ExtensionArn": str,
-        "ResourceArn": str,
-        "Arn": str,
-        "Parameters": Dict[str, str],
-        "ExtensionVersionNumber": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-HostedConfigurationVersionTypeDef = TypedDict(
-    "HostedConfigurationVersionTypeDef",
-    {
-        "ApplicationId": str,
-        "ConfigurationProfileId": str,
-        "VersionNumber": int,
-        "Description": str,
-        "Content": StreamingBody,
-        "ContentType": str,
-        "VersionLabel": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ResourceTagsTypeDef = TypedDict(
-    "ResourceTagsTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ApplicationsTypeDef = TypedDict(
     "ApplicationsTypeDef",
     {
         "Items": List[ApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigurationProfilesTypeDef = TypedDict(
     "ConfigurationProfilesTypeDef",
     {
         "Items": List[ConfigurationProfileSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigurationProfileTypeDef = TypedDict(
     "ConfigurationProfileTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "LocationUri": str,
         "RetrievalRoleArn": str,
         "Validators": List[ValidatorTypeDef],
         "Type": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateConfigurationProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationProfileRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -996,15 +996,15 @@
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "State": EnvironmentStateType,
         "Monitors": List[MonitorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "ApplicationId": str,
@@ -1068,15 +1068,15 @@
         "Id": str,
         "Name": str,
         "VersionNumber": int,
         "Arn": str,
         "Description": str,
         "Actions": Dict[ActionPointType, List[ActionTypeDef]],
         "Parameters": Dict[str, ParameterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateExtensionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExtensionRequestRequestTypeDef",
     {
         "ExtensionIdentifier": str,
@@ -1099,51 +1099,51 @@
     pass
 
 DeploymentStrategiesTypeDef = TypedDict(
     "DeploymentStrategiesTypeDef",
     {
         "Items": List[DeploymentStrategyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentsTypeDef = TypedDict(
     "DeploymentsTypeDef",
     {
         "Items": List[DeploymentSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExtensionAssociationsTypeDef = TypedDict(
     "ExtensionAssociationsTypeDef",
     {
         "Items": List[ExtensionAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExtensionsTypeDef = TypedDict(
     "ExtensionsTypeDef",
     {
         "Items": List[ExtensionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HostedConfigurationVersionsTypeDef = TypedDict(
     "HostedConfigurationVersionsTypeDef",
     {
         "Items": List[HostedConfigurationVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "ApplicationId": str,
@@ -1163,19 +1163,19 @@
         "EventLog": List[DeploymentEventTypeDef],
         "PercentageComplete": float,
         "StartedAt": datetime,
         "CompletedAt": datetime,
         "AppliedExtensions": List[AppliedExtensionTypeDef],
         "KmsKeyArn": str,
         "KmsKeyIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EnvironmentsTypeDef = TypedDict(
     "EnvironmentsTypeDef",
     {
         "Items": List[EnvironmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig.egg-info/PKG-INFO` & `mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appconfig
-Version: 1.26.71
-Summary: Type annotations for boto3.AppConfig 1.26.71 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.AppConfig 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-appconfig"></a>
 
 # mypy-boto3-appconfig
 
 [![PyPI - mypy-boto3-appconfig](https://img.shields.io/pypi/v/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appconfig?color=blue)](https://pypistats.org/packages/mypy-boto3-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfig 1.26.71](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[boto3.AppConfig 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [mypy-boto3-appconfig docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,71 +305,71 @@
 `mypy_boto3_appconfig.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appconfig.type_defs import (
     ActionInvocationTypeDef,
     ActionTypeDef,
-    ResponseMetadataTypeDef,
+    ApplicationResponseMetadataTypeDef,
     ApplicationTypeDef,
     AppliedExtensionTypeDef,
     ConfigurationProfileSummaryTypeDef,
     ValidatorTypeDef,
+    ConfigurationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateDeploymentStrategyRequestRequestTypeDef,
     MonitorTypeDef,
     CreateExtensionAssociationRequestRequestTypeDef,
     ParameterTypeDef,
     CreateHostedConfigurationVersionRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteConfigurationProfileRequestRequestTypeDef,
     DeleteDeploymentStrategyRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteExtensionAssociationRequestRequestTypeDef,
     DeleteExtensionRequestRequestTypeDef,
     DeleteHostedConfigurationVersionRequestRequestTypeDef,
     DeploymentStrategyTypeDef,
+    DeploymentStrategyResponseMetadataTypeDef,
     DeploymentSummaryTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExtensionAssociationSummaryTypeDef,
+    ExtensionAssociationTypeDef,
     ExtensionSummaryTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetConfigurationProfileRequestRequestTypeDef,
     GetConfigurationRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetDeploymentStrategyRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetExtensionAssociationRequestRequestTypeDef,
     GetExtensionRequestRequestTypeDef,
     GetHostedConfigurationVersionRequestRequestTypeDef,
     HostedConfigurationVersionSummaryTypeDef,
+    HostedConfigurationVersionTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListConfigurationProfilesRequestRequestTypeDef,
     ListDeploymentStrategiesRequestRequestTypeDef,
     ListDeploymentsRequestRequestTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListExtensionAssociationsRequestRequestTypeDef,
     ListExtensionsRequestRequestTypeDef,
     ListHostedConfigurationVersionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ResourceTagsTypeDef,
+    ResponseMetadataTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StopDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateDeploymentStrategyRequestRequestTypeDef,
     UpdateExtensionAssociationRequestRequestTypeDef,
     ValidateConfigurationRequestRequestTypeDef,
     DeploymentEventTypeDef,
-    ApplicationResponseMetadataTypeDef,
-    ConfigurationTypeDef,
-    DeploymentStrategyResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExtensionAssociationTypeDef,
-    HostedConfigurationVersionTypeDef,
-    ResourceTagsTypeDef,
     ApplicationsTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     CreateConfigurationProfileRequestRequestTypeDef,
     UpdateConfigurationProfileRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     EnvironmentResponseMetadataTypeDef,
@@ -395,42 +395,42 @@
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

### Comparing `mypy-boto3-appconfig-1.26.71/mypy_boto3_appconfig.egg-info/SOURCES.txt` & `mypy-boto3-appconfig-1.27.0/mypy_boto3_appconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfig-1.26.71/setup.py` & `mypy-boto3-appconfig-1.27.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-appconfig.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appconfig",
-    version="1.26.71",
+    version="1.27.0",
     packages=["mypy_boto3_appconfig"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppConfig 1.26.71 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.AppConfig 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/",
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


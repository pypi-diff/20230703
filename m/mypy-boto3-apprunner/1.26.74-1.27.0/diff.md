# Comparing `tmp/mypy-boto3-apprunner-1.26.74.tar.gz` & `tmp/mypy-boto3-apprunner-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apprunner-1.26.74.tar", last modified: Fri Feb 17 20:26:41 2023, max compression
+gzip compressed data, was "mypy-boto3-apprunner-1.27.0.tar", last modified: Mon Jul  3 19:50:22 2023, max compression
```

## Comparing `mypy-boto3-apprunner-1.26.74.tar` & `mypy-boto3-apprunner-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:26:41.075546 mypy-boto3-apprunner-1.26.74/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-17 20:26:17.000000 mypy-boto3-apprunner-1.26.74/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16695 2023-02-17 20:26:41.075546 mypy-boto3-apprunner-1.26.74/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15200 2023-02-17 20:26:17.000000 mypy-boto3-apprunner-1.26.74/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:26:41.075546 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-17 20:26:17.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-17 20:26:17.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-17 20:26:17.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25678 2023-02-17 20:26:17.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-02-17 20:26:17.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-02-17 20:26:17.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-02-17 20:26:17.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 20:26:17.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35581 2023-02-17 20:26:18.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35546 2023-02-17 20:26:18.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-17 20:26:17.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:26:41.075546 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16695 2023-02-17 20:26:40.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-02-17 20:26:40.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 20:26:40.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 20:26:40.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-17 20:26:40.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-17 20:26:40.000000 mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 20:26:41.075546 mypy-boto3-apprunner-1.26.74/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-17 20:26:17.000000 mypy-boto3-apprunner-1.26.74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.590823 mypy-boto3-apprunner-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:39.000000 mypy-boto3-apprunner-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16673 2023-07-03 19:50:22.590823 mypy-boto3-apprunner-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-03 19:32:39.000000 mypy-boto3-apprunner-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.590823 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-03 19:32:39.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 19:32:39.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:32:39.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25678 2023-07-03 19:32:39.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-03 19:32:39.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-07-03 19:32:39.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-07-03 19:32:39.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:39.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35647 2023-07-03 19:32:41.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35612 2023-07-03 19:32:40.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:39.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.590823 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16673 2023-07-03 19:50:22.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-03 19:50:22.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:22.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:50:22.000000 mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:22.590823 mypy-boto3-apprunner-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:32:39.000000 mypy-boto3-apprunner-1.27.0/setup.py
```

### Comparing `mypy-boto3-apprunner-1.26.74/LICENSE` & `mypy-boto3-apprunner-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-apprunner-1.26.74/PKG-INFO` & `mypy-boto3-apprunner-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apprunner
-Version: 1.26.74
-Summary: Type annotations for boto3.AppRunner 1.26.74 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.AppRunner 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-apprunner"></a>
 
 # mypy-boto3-apprunner
 
 [![PyPI - mypy-boto3-apprunner](https://img.shields.io/pypi/v/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apprunner?color=blue)](https://pypistats.org/packages/mypy-boto3-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRunner 1.26.74](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[boto3.AppRunner 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
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
 [mypy-boto3-apprunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,15 +314,14 @@
 
 `mypy_boto3_apprunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apprunner.type_defs import (
     AssociateCustomDomainRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     VpcDNSTargetTypeDef,
     AuthenticationConfigurationTypeDef,
     AutoScalingConfigurationSummaryTypeDef,
     AutoScalingConfigurationTypeDef,
     CertificateValidationRecordTypeDef,
     CodeConfigurationValuesTypeDef,
     SourceCodeVersionTypeDef,
@@ -361,18 +360,19 @@
     ListServicesRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVpcConnectorsRequestRequestTypeDef,
     ListVpcIngressConnectionsFilterTypeDef,
     VpcIngressConnectionSummaryTypeDef,
     PauseServiceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ResumeServiceRequestRequestTypeDef,
     StartDeploymentRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
     StartDeploymentResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
     ListAutoScalingConfigurationsResponseTypeDef,
     CreateAutoScalingConfigurationResponseTypeDef,
     DeleteAutoScalingConfigurationResponseTypeDef,
     DescribeAutoScalingConfigurationResponseTypeDef,
     CustomDomainTypeDef,
     CodeConfigurationTypeDef,
     ListConnectionsResponseTypeDef,
@@ -430,42 +430,42 @@
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

### Comparing `mypy-boto3-apprunner-1.26.74/README.md` & `mypy-boto3-apprunner-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-apprunner"></a>
 
 # mypy-boto3-apprunner
 
 [![PyPI - mypy-boto3-apprunner](https://img.shields.io/pypi/v/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apprunner?color=blue)](https://pypistats.org/packages/mypy-boto3-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRunner 1.26.74](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[boto3.AppRunner 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
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
 [mypy-boto3-apprunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -282,15 +282,14 @@
 
 `mypy_boto3_apprunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apprunner.type_defs import (
     AssociateCustomDomainRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     VpcDNSTargetTypeDef,
     AuthenticationConfigurationTypeDef,
     AutoScalingConfigurationSummaryTypeDef,
     AutoScalingConfigurationTypeDef,
     CertificateValidationRecordTypeDef,
     CodeConfigurationValuesTypeDef,
     SourceCodeVersionTypeDef,
@@ -329,18 +328,19 @@
     ListServicesRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVpcConnectorsRequestRequestTypeDef,
     ListVpcIngressConnectionsFilterTypeDef,
     VpcIngressConnectionSummaryTypeDef,
     PauseServiceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ResumeServiceRequestRequestTypeDef,
     StartDeploymentRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
     StartDeploymentResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
     ListAutoScalingConfigurationsResponseTypeDef,
     CreateAutoScalingConfigurationResponseTypeDef,
     DeleteAutoScalingConfigurationResponseTypeDef,
     DescribeAutoScalingConfigurationResponseTypeDef,
     CustomDomainTypeDef,
     CodeConfigurationTypeDef,
     ListConnectionsResponseTypeDef,
@@ -398,42 +398,42 @@
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

### Comparing `mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/__main__.py` & `mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppRunner 1.26.74\nVersion:         1.26.74\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.AppRunner 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.74")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/client.py` & `mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/client.pyi` & `mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/literals.py` & `mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,14 +120,15 @@
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
@@ -167,14 +168,15 @@
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
@@ -253,14 +255,15 @@
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
@@ -271,14 +274,15 @@
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
@@ -314,14 +318,15 @@
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
@@ -340,16 +345,19 @@
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
@@ -429,18 +437,21 @@
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
@@ -458,8 +469,17 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-RegionName = Literal["ap-northeast-1", "eu-west-1", "us-east-1", "us-east-2", "us-west-2"]
+RegionName = Literal[
+    "ap-northeast-1",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "eu-central-1",
+    "eu-west-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/literals.pyi` & `mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -118,14 +118,15 @@
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
@@ -165,14 +166,15 @@
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
@@ -251,14 +253,15 @@
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
@@ -269,14 +272,15 @@
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
@@ -312,14 +316,15 @@
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
@@ -338,16 +343,19 @@
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
@@ -427,18 +435,21 @@
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
@@ -456,8 +467,17 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-RegionName = Literal["ap-northeast-1", "eu-west-1", "us-east-1", "us-east-2", "us-west-2"]
+RegionName = Literal[
+    "ap-northeast-1",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "eu-central-1",
+    "eu-west-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/type_defs.py` & `mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateCustomDomainRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "VpcDNSTargetTypeDef",
     "AuthenticationConfigurationTypeDef",
     "AutoScalingConfigurationSummaryTypeDef",
     "AutoScalingConfigurationTypeDef",
     "CertificateValidationRecordTypeDef",
     "CodeConfigurationValuesTypeDef",
     "SourceCodeVersionTypeDef",
@@ -88,18 +87,19 @@
     "ListServicesRequestRequestTypeDef",
     "ServiceSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVpcConnectorsRequestRequestTypeDef",
     "ListVpcIngressConnectionsFilterTypeDef",
     "VpcIngressConnectionSummaryTypeDef",
     "PauseServiceRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ResumeServiceRequestRequestTypeDef",
     "StartDeploymentRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
     "StartDeploymentResponseTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "ListAutoScalingConfigurationsResponseTypeDef",
     "CreateAutoScalingConfigurationResponseTypeDef",
     "DeleteAutoScalingConfigurationResponseTypeDef",
     "DescribeAutoScalingConfigurationResponseTypeDef",
     "CustomDomainTypeDef",
     "CodeConfigurationTypeDef",
     "ListConnectionsResponseTypeDef",
@@ -168,25 +168,14 @@
 class AssociateCustomDomainRequestRequestTypeDef(
     _RequiredAssociateCustomDomainRequestRequestTypeDef,
     _OptionalAssociateCustomDomainRequestRequestTypeDef,
 ):
     pass
 
 
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
 VpcDNSTargetTypeDef = TypedDict(
     "VpcDNSTargetTypeDef",
     {
         "VpcIngressConnectionArn": str,
         "VpcId": str,
         "DomainName": str,
     },
@@ -663,74 +652,85 @@
 PauseServiceRequestRequestTypeDef = TypedDict(
     "PauseServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
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
 ResumeServiceRequestRequestTypeDef = TypedDict(
     "ResumeServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 
 StartDeploymentRequestRequestTypeDef = TypedDict(
     "StartDeploymentRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StartDeploymentResponseTypeDef = TypedDict(
+    "StartDeploymentResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartDeploymentResponseTypeDef = TypedDict(
-    "StartDeploymentResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
 ListAutoScalingConfigurationsResponseTypeDef = TypedDict(
     "ListAutoScalingConfigurationsResponseTypeDef",
     {
         "AutoScalingConfigurationSummaryList": List[AutoScalingConfigurationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAutoScalingConfigurationResponseTypeDef = TypedDict(
     "CreateAutoScalingConfigurationResponseTypeDef",
     {
         "AutoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAutoScalingConfigurationResponseTypeDef = TypedDict(
     "DeleteAutoScalingConfigurationResponseTypeDef",
     {
         "AutoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAutoScalingConfigurationResponseTypeDef = TypedDict(
     "DescribeAutoScalingConfigurationResponseTypeDef",
     {
         "AutoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCustomDomainTypeDef = TypedDict(
     "_RequiredCustomDomainTypeDef",
     {
         "DomainName": str,
@@ -773,31 +773,31 @@
 
 
 ListConnectionsResponseTypeDef = TypedDict(
     "ListConnectionsResponseTypeDef",
     {
         "ConnectionSummaryList": List[ConnectionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateConnectionResponseTypeDef = TypedDict(
     "CreateConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteConnectionResponseTypeDef = TypedDict(
     "DeleteConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAutoScalingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoScalingConfigurationRequestRequestTypeDef",
     {
         "AutoScalingConfigurationName": str,
@@ -868,15 +868,15 @@
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -922,40 +922,40 @@
     total=False,
 )
 
 CreateVpcConnectorResponseTypeDef = TypedDict(
     "CreateVpcConnectorResponseTypeDef",
     {
         "VpcConnector": VpcConnectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVpcConnectorResponseTypeDef = TypedDict(
     "DeleteVpcConnectorResponseTypeDef",
     {
         "VpcConnector": VpcConnectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVpcConnectorResponseTypeDef = TypedDict(
     "DescribeVpcConnectorResponseTypeDef",
     {
         "VpcConnector": VpcConnectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcConnectorsResponseTypeDef = TypedDict(
     "ListVpcConnectorsResponseTypeDef",
     {
         "VpcConnectors": List[VpcConnectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateVpcIngressConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcIngressConnectionRequestRequestTypeDef",
     {
         "ServiceArn": str,
@@ -1033,33 +1033,33 @@
 )
 
 ListObservabilityConfigurationsResponseTypeDef = TypedDict(
     "ListObservabilityConfigurationsResponseTypeDef",
     {
         "ObservabilityConfigurationSummaryList": List[ObservabilityConfigurationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "OperationSummaryList": List[OperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "ServiceSummaryList": List[ServiceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcIngressConnectionsRequestRequestTypeDef = TypedDict(
     "ListVpcIngressConnectionsRequestRequestTypeDef",
     {
         "Filter": ListVpcIngressConnectionsFilterTypeDef,
@@ -1070,49 +1070,49 @@
 )
 
 ListVpcIngressConnectionsResponseTypeDef = TypedDict(
     "ListVpcIngressConnectionsResponseTypeDef",
     {
         "VpcIngressConnectionSummaryList": List[VpcIngressConnectionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateCustomDomainResponseTypeDef = TypedDict(
     "AssociateCustomDomainResponseTypeDef",
     {
         "DNSTarget": str,
         "ServiceArn": str,
         "CustomDomain": CustomDomainTypeDef,
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCustomDomainsResponseTypeDef = TypedDict(
     "DescribeCustomDomainsResponseTypeDef",
     {
         "DNSTarget": str,
         "ServiceArn": str,
         "CustomDomains": List[CustomDomainTypeDef],
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateCustomDomainResponseTypeDef = TypedDict(
     "DisassociateCustomDomainResponseTypeDef",
     {
         "DNSTarget": str,
         "ServiceArn": str,
         "CustomDomain": CustomDomainTypeDef,
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCodeRepositoryTypeDef = TypedDict(
     "_RequiredCodeRepositoryTypeDef",
     {
         "RepositoryUrl": str,
@@ -1132,63 +1132,63 @@
     pass
 
 
 CreateObservabilityConfigurationResponseTypeDef = TypedDict(
     "CreateObservabilityConfigurationResponseTypeDef",
     {
         "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteObservabilityConfigurationResponseTypeDef = TypedDict(
     "DeleteObservabilityConfigurationResponseTypeDef",
     {
         "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeObservabilityConfigurationResponseTypeDef = TypedDict(
     "DescribeObservabilityConfigurationResponseTypeDef",
     {
         "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVpcIngressConnectionResponseTypeDef = TypedDict(
     "CreateVpcIngressConnectionResponseTypeDef",
     {
         "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVpcIngressConnectionResponseTypeDef = TypedDict(
     "DeleteVpcIngressConnectionResponseTypeDef",
     {
         "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVpcIngressConnectionResponseTypeDef = TypedDict(
     "DescribeVpcIngressConnectionResponseTypeDef",
     {
         "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVpcIngressConnectionResponseTypeDef = TypedDict(
     "UpdateVpcIngressConnectionResponseTypeDef",
     {
         "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "CodeRepository": CodeRepositoryTypeDef,
@@ -1286,54 +1286,54 @@
 
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteServiceResponseTypeDef = TypedDict(
     "DeleteServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeServiceResponseTypeDef = TypedDict(
     "DescribeServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PauseServiceResponseTypeDef = TypedDict(
     "PauseServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResumeServiceResponseTypeDef = TypedDict(
     "ResumeServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceResponseTypeDef = TypedDict(
     "UpdateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner/type_defs.pyi` & `mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateCustomDomainRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "VpcDNSTargetTypeDef",
     "AuthenticationConfigurationTypeDef",
     "AutoScalingConfigurationSummaryTypeDef",
     "AutoScalingConfigurationTypeDef",
     "CertificateValidationRecordTypeDef",
     "CodeConfigurationValuesTypeDef",
     "SourceCodeVersionTypeDef",
@@ -87,18 +86,19 @@
     "ListServicesRequestRequestTypeDef",
     "ServiceSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVpcConnectorsRequestRequestTypeDef",
     "ListVpcIngressConnectionsFilterTypeDef",
     "VpcIngressConnectionSummaryTypeDef",
     "PauseServiceRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ResumeServiceRequestRequestTypeDef",
     "StartDeploymentRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
     "StartDeploymentResponseTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "ListAutoScalingConfigurationsResponseTypeDef",
     "CreateAutoScalingConfigurationResponseTypeDef",
     "DeleteAutoScalingConfigurationResponseTypeDef",
     "DescribeAutoScalingConfigurationResponseTypeDef",
     "CustomDomainTypeDef",
     "CodeConfigurationTypeDef",
     "ListConnectionsResponseTypeDef",
@@ -165,25 +165,14 @@
 
 class AssociateCustomDomainRequestRequestTypeDef(
     _RequiredAssociateCustomDomainRequestRequestTypeDef,
     _OptionalAssociateCustomDomainRequestRequestTypeDef,
 ):
     pass
 
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
 VpcDNSTargetTypeDef = TypedDict(
     "VpcDNSTargetTypeDef",
     {
         "VpcIngressConnectionArn": str,
         "VpcId": str,
         "DomainName": str,
     },
@@ -652,74 +641,85 @@
 PauseServiceRequestRequestTypeDef = TypedDict(
     "PauseServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
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
 ResumeServiceRequestRequestTypeDef = TypedDict(
     "ResumeServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 
 StartDeploymentRequestRequestTypeDef = TypedDict(
     "StartDeploymentRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+StartDeploymentResponseTypeDef = TypedDict(
+    "StartDeploymentResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "OperationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartDeploymentResponseTypeDef = TypedDict(
-    "StartDeploymentResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
 ListAutoScalingConfigurationsResponseTypeDef = TypedDict(
     "ListAutoScalingConfigurationsResponseTypeDef",
     {
         "AutoScalingConfigurationSummaryList": List[AutoScalingConfigurationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAutoScalingConfigurationResponseTypeDef = TypedDict(
     "CreateAutoScalingConfigurationResponseTypeDef",
     {
         "AutoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAutoScalingConfigurationResponseTypeDef = TypedDict(
     "DeleteAutoScalingConfigurationResponseTypeDef",
     {
         "AutoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAutoScalingConfigurationResponseTypeDef = TypedDict(
     "DescribeAutoScalingConfigurationResponseTypeDef",
     {
         "AutoScalingConfiguration": AutoScalingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCustomDomainTypeDef = TypedDict(
     "_RequiredCustomDomainTypeDef",
     {
         "DomainName": str,
@@ -758,31 +758,31 @@
     pass
 
 ListConnectionsResponseTypeDef = TypedDict(
     "ListConnectionsResponseTypeDef",
     {
         "ConnectionSummaryList": List[ConnectionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateConnectionResponseTypeDef = TypedDict(
     "CreateConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteConnectionResponseTypeDef = TypedDict(
     "DeleteConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAutoScalingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoScalingConfigurationRequestRequestTypeDef",
     {
         "AutoScalingConfigurationName": str,
@@ -847,15 +847,15 @@
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -899,40 +899,40 @@
     total=False,
 )
 
 CreateVpcConnectorResponseTypeDef = TypedDict(
     "CreateVpcConnectorResponseTypeDef",
     {
         "VpcConnector": VpcConnectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVpcConnectorResponseTypeDef = TypedDict(
     "DeleteVpcConnectorResponseTypeDef",
     {
         "VpcConnector": VpcConnectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVpcConnectorResponseTypeDef = TypedDict(
     "DescribeVpcConnectorResponseTypeDef",
     {
         "VpcConnector": VpcConnectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcConnectorsResponseTypeDef = TypedDict(
     "ListVpcConnectorsResponseTypeDef",
     {
         "VpcConnectors": List[VpcConnectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateVpcIngressConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcIngressConnectionRequestRequestTypeDef",
     {
         "ServiceArn": str,
@@ -1006,33 +1006,33 @@
 )
 
 ListObservabilityConfigurationsResponseTypeDef = TypedDict(
     "ListObservabilityConfigurationsResponseTypeDef",
     {
         "ObservabilityConfigurationSummaryList": List[ObservabilityConfigurationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "OperationSummaryList": List[OperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "ServiceSummaryList": List[ServiceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVpcIngressConnectionsRequestRequestTypeDef = TypedDict(
     "ListVpcIngressConnectionsRequestRequestTypeDef",
     {
         "Filter": ListVpcIngressConnectionsFilterTypeDef,
@@ -1043,49 +1043,49 @@
 )
 
 ListVpcIngressConnectionsResponseTypeDef = TypedDict(
     "ListVpcIngressConnectionsResponseTypeDef",
     {
         "VpcIngressConnectionSummaryList": List[VpcIngressConnectionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateCustomDomainResponseTypeDef = TypedDict(
     "AssociateCustomDomainResponseTypeDef",
     {
         "DNSTarget": str,
         "ServiceArn": str,
         "CustomDomain": CustomDomainTypeDef,
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCustomDomainsResponseTypeDef = TypedDict(
     "DescribeCustomDomainsResponseTypeDef",
     {
         "DNSTarget": str,
         "ServiceArn": str,
         "CustomDomains": List[CustomDomainTypeDef],
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateCustomDomainResponseTypeDef = TypedDict(
     "DisassociateCustomDomainResponseTypeDef",
     {
         "DNSTarget": str,
         "ServiceArn": str,
         "CustomDomain": CustomDomainTypeDef,
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCodeRepositoryTypeDef = TypedDict(
     "_RequiredCodeRepositoryTypeDef",
     {
         "RepositoryUrl": str,
@@ -1103,63 +1103,63 @@
 class CodeRepositoryTypeDef(_RequiredCodeRepositoryTypeDef, _OptionalCodeRepositoryTypeDef):
     pass
 
 CreateObservabilityConfigurationResponseTypeDef = TypedDict(
     "CreateObservabilityConfigurationResponseTypeDef",
     {
         "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteObservabilityConfigurationResponseTypeDef = TypedDict(
     "DeleteObservabilityConfigurationResponseTypeDef",
     {
         "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeObservabilityConfigurationResponseTypeDef = TypedDict(
     "DescribeObservabilityConfigurationResponseTypeDef",
     {
         "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateVpcIngressConnectionResponseTypeDef = TypedDict(
     "CreateVpcIngressConnectionResponseTypeDef",
     {
         "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteVpcIngressConnectionResponseTypeDef = TypedDict(
     "DeleteVpcIngressConnectionResponseTypeDef",
     {
         "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVpcIngressConnectionResponseTypeDef = TypedDict(
     "DescribeVpcIngressConnectionResponseTypeDef",
     {
         "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateVpcIngressConnectionResponseTypeDef = TypedDict(
     "UpdateVpcIngressConnectionResponseTypeDef",
     {
         "VpcIngressConnection": VpcIngressConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "CodeRepository": CodeRepositoryTypeDef,
@@ -1251,54 +1251,54 @@
     pass
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteServiceResponseTypeDef = TypedDict(
     "DeleteServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeServiceResponseTypeDef = TypedDict(
     "DescribeServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PauseServiceResponseTypeDef = TypedDict(
     "PauseServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResumeServiceResponseTypeDef = TypedDict(
     "ResumeServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateServiceResponseTypeDef = TypedDict(
     "UpdateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner.egg-info/PKG-INFO` & `mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apprunner
-Version: 1.26.74
-Summary: Type annotations for boto3.AppRunner 1.26.74 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.AppRunner 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-apprunner"></a>
 
 # mypy-boto3-apprunner
 
 [![PyPI - mypy-boto3-apprunner](https://img.shields.io/pypi/v/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apprunner?color=blue)](https://pypistats.org/packages/mypy-boto3-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRunner 1.26.74](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[boto3.AppRunner 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
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
 [mypy-boto3-apprunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,15 +314,14 @@
 
 `mypy_boto3_apprunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apprunner.type_defs import (
     AssociateCustomDomainRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     VpcDNSTargetTypeDef,
     AuthenticationConfigurationTypeDef,
     AutoScalingConfigurationSummaryTypeDef,
     AutoScalingConfigurationTypeDef,
     CertificateValidationRecordTypeDef,
     CodeConfigurationValuesTypeDef,
     SourceCodeVersionTypeDef,
@@ -361,18 +360,19 @@
     ListServicesRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVpcConnectorsRequestRequestTypeDef,
     ListVpcIngressConnectionsFilterTypeDef,
     VpcIngressConnectionSummaryTypeDef,
     PauseServiceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ResumeServiceRequestRequestTypeDef,
     StartDeploymentRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
     StartDeploymentResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
     ListAutoScalingConfigurationsResponseTypeDef,
     CreateAutoScalingConfigurationResponseTypeDef,
     DeleteAutoScalingConfigurationResponseTypeDef,
     DescribeAutoScalingConfigurationResponseTypeDef,
     CustomDomainTypeDef,
     CodeConfigurationTypeDef,
     ListConnectionsResponseTypeDef,
@@ -430,42 +430,42 @@
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

### Comparing `mypy-boto3-apprunner-1.26.74/mypy_boto3_apprunner.egg-info/SOURCES.txt` & `mypy-boto3-apprunner-1.27.0/mypy_boto3_apprunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.26.74/setup.py` & `mypy-boto3-apprunner-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-apprunner.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-apprunner",
-    version="1.26.74",
+    version="1.27.0",
     packages=["mypy_boto3_apprunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppRunner 1.26.74 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.AppRunner 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/",
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


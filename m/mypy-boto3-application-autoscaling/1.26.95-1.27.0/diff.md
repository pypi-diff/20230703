# Comparing `tmp/mypy-boto3-application-autoscaling-1.26.95.tar.gz` & `tmp/mypy-boto3-application-autoscaling-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-application-autoscaling-1.26.95.tar", last modified: Mon Mar 20 19:32:46 2023, max compression
+gzip compressed data, was "mypy-boto3-application-autoscaling-1.27.0.tar", last modified: Mon Jul  3 19:50:22 2023, max compression
```

## Comparing `mypy-boto3-application-autoscaling-1.26.95.tar` & `mypy-boto3-application-autoscaling-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:46.571025 mypy-boto3-application-autoscaling-1.26.95/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-03-20 19:32:46.571025 mypy-boto3-application-autoscaling-1.26.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:46.571025 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22719 2023-03-20 19:32:25.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22676 2023-03-20 19:32:25.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:32:46.571025 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-03-20 19:32:46.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-20 19:32:46.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 19:32:46.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 19:32:46.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-20 19:32:46.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-20 19:32:46.000000 mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 19:32:46.571025 mypy-boto3-application-autoscaling-1.26.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-20 19:32:24.000000 mypy-boto3-application-autoscaling-1.26.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.522822 mypy-boto3-application-autoscaling-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-07-03 19:50:22.522822 mypy-boto3-application-autoscaling-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14584 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.522822 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22698 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.522822 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-07-03 19:50:22.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-03 19:50:22.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:22.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-03 19:50:22.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:22.522822 mypy-boto3-application-autoscaling-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/setup.py
```

### Comparing `mypy-boto3-application-autoscaling-1.26.95/LICENSE` & `mypy-boto3-application-autoscaling-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-application-autoscaling-1.26.95/PKG-INFO` & `mypy-boto3-application-autoscaling-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-autoscaling
-Version: 1.26.95
-Summary: Type annotations for boto3.ApplicationAutoScaling 1.26.95 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.ApplicationAutoScaling 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-application-autoscaling"></a>
 
 # mypy-boto3-application-autoscaling
 
 [![PyPI - mypy-boto3-application-autoscaling](https://img.shields.io/pypi/v/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-application-autoscaling?color=blue)](https://pypistats.org/packages/mypy-boto3-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationAutoScaling 1.26.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[boto3.ApplicationAutoScaling 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
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
 [mypy-boto3-application-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,36 +352,36 @@
 ```python
 from mypy_boto3_application_autoscaling.type_defs import (
     AlarmTypeDef,
     MetricDimensionTypeDef,
     DeleteScalingPolicyRequestRequestTypeDef,
     DeleteScheduledActionRequestRequestTypeDef,
     DeregisterScalableTargetRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
     DescribeScalableTargetsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingActivitiesRequestRequestTypeDef,
+    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     DescribeScalingPoliciesRequestRequestTypeDef,
+    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NotScaledReasonTypeDef,
+    PaginatorConfigTypeDef,
     PredefinedMetricSpecificationTypeDef,
     ScalableTargetActionTypeDef,
     SuspendedStateTypeDef,
+    RegisterScalableTargetResponseTypeDef,
+    ResponseMetadataTypeDef,
     StepAdjustmentTypeDef,
     TagResourceRequestRequestTypeDef,
     TargetTrackingMetricDimensionTypeDef,
     UntagResourceRequestRequestTypeDef,
-    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
-    RegisterScalableTargetResponseTypeDef,
     ScalingActivityTypeDef,
     PutScheduledActionRequestRequestTypeDef,
     ScheduledActionTypeDef,
     RegisterScalableTargetRequestRequestTypeDef,
     ScalableTargetTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     TargetTrackingMetricTypeDef,
@@ -405,42 +405,42 @@
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

### Comparing `mypy-boto3-application-autoscaling-1.26.95/README.md` & `mypy-boto3-application-autoscaling-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-application-autoscaling"></a>
 
 # mypy-boto3-application-autoscaling
 
 [![PyPI - mypy-boto3-application-autoscaling](https://img.shields.io/pypi/v/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-application-autoscaling?color=blue)](https://pypistats.org/packages/mypy-boto3-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationAutoScaling 1.26.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[boto3.ApplicationAutoScaling 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
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
 [mypy-boto3-application-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,36 +320,36 @@
 ```python
 from mypy_boto3_application_autoscaling.type_defs import (
     AlarmTypeDef,
     MetricDimensionTypeDef,
     DeleteScalingPolicyRequestRequestTypeDef,
     DeleteScheduledActionRequestRequestTypeDef,
     DeregisterScalableTargetRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
     DescribeScalableTargetsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingActivitiesRequestRequestTypeDef,
+    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     DescribeScalingPoliciesRequestRequestTypeDef,
+    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NotScaledReasonTypeDef,
+    PaginatorConfigTypeDef,
     PredefinedMetricSpecificationTypeDef,
     ScalableTargetActionTypeDef,
     SuspendedStateTypeDef,
+    RegisterScalableTargetResponseTypeDef,
+    ResponseMetadataTypeDef,
     StepAdjustmentTypeDef,
     TagResourceRequestRequestTypeDef,
     TargetTrackingMetricDimensionTypeDef,
     UntagResourceRequestRequestTypeDef,
-    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
-    RegisterScalableTargetResponseTypeDef,
     ScalingActivityTypeDef,
     PutScheduledActionRequestRequestTypeDef,
     ScheduledActionTypeDef,
     RegisterScalableTargetRequestRequestTypeDef,
     ScalableTargetTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     TargetTrackingMetricTypeDef,
@@ -373,42 +373,42 @@
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

### Comparing `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/__init__.py` & `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/__init__.pyi` & `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/__main__.py` & `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApplicationAutoScaling 1.26.95\nVersion:        "
-        " 1.26.95\nBuilder version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.ApplicationAutoScaling 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.95")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/client.py` & `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/client.pyi` & `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/literals.py` & `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/literals.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,23 +56,25 @@
     "DynamoDBReadCapacityUtilization",
     "DynamoDBWriteCapacityUtilization",
     "EC2SpotFleetRequestAverageCPUUtilization",
     "EC2SpotFleetRequestAverageNetworkIn",
     "EC2SpotFleetRequestAverageNetworkOut",
     "ECSServiceAverageCPUUtilization",
     "ECSServiceAverageMemoryUtilization",
+    "ElastiCacheDatabaseCapacityUsageCountedForEvictPercentage",
     "ElastiCacheDatabaseMemoryUsageCountedForEvictPercentage",
     "ElastiCachePrimaryEngineCPUUtilization",
     "ElastiCacheReplicaEngineCPUUtilization",
     "KafkaBrokerStorageUtilization",
     "LambdaProvisionedConcurrencyUtilization",
     "NeptuneReaderAverageCPUUtilization",
     "RDSReaderAverageCPUUtilization",
     "RDSReaderAverageDatabaseConnections",
     "SageMakerVariantInvocationsPerInstance",
+    "SageMakerVariantProvisionedConcurrencyUtilization",
 ]
 PolicyTypeType = Literal["StepScaling", "TargetTrackingScaling"]
 ScalableDimensionType = Literal[
     "appstream:fleet:DesiredCapacity",
     "cassandra:table:ReadCapacityUnits",
     "cassandra:table:WriteCapacityUnits",
     "comprehend:document-classifier-endpoint:DesiredInferenceUnits",
@@ -88,14 +90,15 @@
     "elasticache:replication-group:Replicas",
     "elasticmapreduce:instancegroup:InstanceCount",
     "kafka:broker-storage:VolumeSize",
     "lambda:function:ProvisionedConcurrency",
     "neptune:cluster:ReadReplicaCount",
     "rds:cluster:ReadReplicaCount",
     "sagemaker:variant:DesiredInstanceCount",
+    "sagemaker:variant:DesiredProvisionedConcurrency",
 ]
 ScalingActivityStatusCodeType = Literal[
     "Failed", "InProgress", "Overridden", "Pending", "Successful", "Unfulfilled"
 ]
 ServiceNamespaceType = Literal[
     "appstream",
     "cassandra",
@@ -124,14 +127,15 @@
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
@@ -171,14 +175,15 @@
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
@@ -276,14 +281,15 @@
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
@@ -319,14 +325,15 @@
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
@@ -345,16 +352,19 @@
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
@@ -438,15 +448,17 @@
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

### Comparing `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/literals.pyi` & `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/literals.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -54,23 +54,25 @@
     "DynamoDBReadCapacityUtilization",
     "DynamoDBWriteCapacityUtilization",
     "EC2SpotFleetRequestAverageCPUUtilization",
     "EC2SpotFleetRequestAverageNetworkIn",
     "EC2SpotFleetRequestAverageNetworkOut",
     "ECSServiceAverageCPUUtilization",
     "ECSServiceAverageMemoryUtilization",
+    "ElastiCacheDatabaseCapacityUsageCountedForEvictPercentage",
     "ElastiCacheDatabaseMemoryUsageCountedForEvictPercentage",
     "ElastiCachePrimaryEngineCPUUtilization",
     "ElastiCacheReplicaEngineCPUUtilization",
     "KafkaBrokerStorageUtilization",
     "LambdaProvisionedConcurrencyUtilization",
     "NeptuneReaderAverageCPUUtilization",
     "RDSReaderAverageCPUUtilization",
     "RDSReaderAverageDatabaseConnections",
     "SageMakerVariantInvocationsPerInstance",
+    "SageMakerVariantProvisionedConcurrencyUtilization",
 ]
 PolicyTypeType = Literal["StepScaling", "TargetTrackingScaling"]
 ScalableDimensionType = Literal[
     "appstream:fleet:DesiredCapacity",
     "cassandra:table:ReadCapacityUnits",
     "cassandra:table:WriteCapacityUnits",
     "comprehend:document-classifier-endpoint:DesiredInferenceUnits",
@@ -86,14 +88,15 @@
     "elasticache:replication-group:Replicas",
     "elasticmapreduce:instancegroup:InstanceCount",
     "kafka:broker-storage:VolumeSize",
     "lambda:function:ProvisionedConcurrency",
     "neptune:cluster:ReadReplicaCount",
     "rds:cluster:ReadReplicaCount",
     "sagemaker:variant:DesiredInstanceCount",
+    "sagemaker:variant:DesiredProvisionedConcurrency",
 ]
 ScalingActivityStatusCodeType = Literal[
     "Failed", "InProgress", "Overridden", "Pending", "Successful", "Unfulfilled"
 ]
 ServiceNamespaceType = Literal[
     "appstream",
     "cassandra",
@@ -122,14 +125,15 @@
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
@@ -169,14 +173,15 @@
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
@@ -274,14 +279,15 @@
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
@@ -317,14 +323,15 @@
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
@@ -343,16 +350,19 @@
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
@@ -436,15 +446,17 @@
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

### Comparing `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/paginator.py` & `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceIds: Sequence[str] = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScalableTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalableTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalabletargetspaginator)
         """
 
 
@@ -85,15 +85,15 @@
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         IncludeNotScaledActivities: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScalingActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
 
@@ -106,15 +106,15 @@
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         PolicyNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScalingPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalingpoliciespaginator)
         """
 
 
@@ -127,13 +127,13 @@
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScheduledActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescheduledactionspaginator)
         """
```

### Comparing `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/paginator.pyi` & `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceIds: Sequence[str] = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScalableTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalableTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalabletargetspaginator)
         """
 
 class DescribeScalingActivitiesPaginator(Paginator):
@@ -81,15 +81,15 @@
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         IncludeNotScaledActivities: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScalingActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
 class DescribeScalingPoliciesPaginator(Paginator):
@@ -101,15 +101,15 @@
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         PolicyNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScalingPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescalingpoliciespaginator)
         """
 
 class DescribeScheduledActionsPaginator(Paginator):
@@ -121,13 +121,13 @@
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScheduledActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/paginators/#describescheduledactionspaginator)
         """
```

### Comparing `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/type_defs.py` & `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,36 +34,36 @@
 
 __all__ = (
     "AlarmTypeDef",
     "MetricDimensionTypeDef",
     "DeleteScalingPolicyRequestRequestTypeDef",
     "DeleteScheduledActionRequestRequestTypeDef",
     "DeregisterScalableTargetRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
     "DescribeScalableTargetsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     "DescribeScalingActivitiesRequestRequestTypeDef",
+    "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     "DescribeScalingPoliciesRequestRequestTypeDef",
+    "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "NotScaledReasonTypeDef",
+    "PaginatorConfigTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "ScalableTargetActionTypeDef",
     "SuspendedStateTypeDef",
+    "RegisterScalableTargetResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "StepAdjustmentTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TargetTrackingMetricDimensionTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
-    "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
-    "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
-    "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PutScalingPolicyResponseTypeDef",
-    "RegisterScalableTargetResponseTypeDef",
     "ScalingActivityTypeDef",
     "PutScheduledActionRequestRequestTypeDef",
     "ScheduledActionTypeDef",
     "RegisterScalableTargetRequestRequestTypeDef",
     "ScalableTargetTypeDef",
     "StepScalingPolicyConfigurationTypeDef",
     "TargetTrackingMetricTypeDef",
@@ -120,24 +120,38 @@
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ServiceNamespace": ServiceNamespaceType,
+    },
+)
+_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+    {
+        "ResourceIds": Sequence[str],
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
+    _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeScalableTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalableTargetsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalableTargetsRequestRequestTypeDef = TypedDict(
@@ -155,24 +169,38 @@
 class DescribeScalableTargetsRequestRequestTypeDef(
     _RequiredDescribeScalableTargetsRequestRequestTypeDef,
     _OptionalDescribeScalableTargetsRequestRequestTypeDef,
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ServiceNamespace": ServiceNamespaceType,
     },
 )
+_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+    {
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "IncludeNotScaledActivities": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
+    _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+):
+    pass
+
 
 _RequiredDescribeScalingActivitiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingActivitiesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
@@ -192,14 +220,39 @@
 class DescribeScalingActivitiesRequestRequestTypeDef(
     _RequiredDescribeScalingActivitiesRequestRequestTypeDef,
     _OptionalDescribeScalingActivitiesRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
+    {
+        "ServiceNamespace": ServiceNamespaceType,
+    },
+)
+_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
+    {
+        "PolicyNames": Sequence[str],
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
+    _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+    _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPoliciesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
@@ -218,14 +271,39 @@
 class DescribeScalingPoliciesRequestRequestTypeDef(
     _RequiredDescribeScalingPoliciesRequestRequestTypeDef,
     _OptionalDescribeScalingPoliciesRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    {
+        "ServiceNamespace": ServiceNamespaceType,
+    },
+)
+_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    {
+        "ScheduledActionNames": Sequence[str],
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
+    _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+    _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduledActionsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
@@ -251,14 +329,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredNotScaledReasonTypeDef = TypedDict(
     "_RequiredNotScaledReasonTypeDef",
     {
         "Code": str,
     },
 )
 _OptionalNotScaledReasonTypeDef = TypedDict(
@@ -272,14 +358,24 @@
 )
 
 
 class NotScaledReasonTypeDef(_RequiredNotScaledReasonTypeDef, _OptionalNotScaledReasonTypeDef):
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
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
@@ -312,14 +408,33 @@
         "DynamicScalingInSuspended": bool,
         "DynamicScalingOutSuspended": bool,
         "ScheduledScalingSuspended": bool,
     },
     total=False,
 )
 
+RegisterScalableTargetResponseTypeDef = TypedDict(
+    "RegisterScalableTargetResponseTypeDef",
+    {
+        "ScalableTargetARN": str,
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
 _RequiredStepAdjustmentTypeDef = TypedDict(
     "_RequiredStepAdjustmentTypeDef",
     {
         "ScalingAdjustment": int,
     },
 )
 _OptionalStepAdjustmentTypeDef = TypedDict(
@@ -356,135 +471,20 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
-    {
-        "ResourceIds": Sequence[str],
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
-    _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-    _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
-    {
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "IncludeNotScaledActivities": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
-    _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-    _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
-    {
-        "PolicyNames": Sequence[str],
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
-    _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-    _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
-    {
-        "ScheduledActionNames": Sequence[str],
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
-    _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-    _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-):
-    pass
-
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PutScalingPolicyResponseTypeDef = TypedDict(
     "PutScalingPolicyResponseTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterScalableTargetResponseTypeDef = TypedDict(
-    "RegisterScalableTargetResponseTypeDef",
-    {
-        "ScalableTargetARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredScalingActivityTypeDef = TypedDict(
     "_RequiredScalingActivityTypeDef",
     {
         "ActivityId": str,
@@ -647,33 +647,33 @@
 )
 
 DescribeScalingActivitiesResponseTypeDef = TypedDict(
     "DescribeScalingActivitiesResponseTypeDef",
     {
         "ScalingActivities": List[ScalingActivityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeScheduledActionsResponseTypeDef = TypedDict(
     "DescribeScheduledActionsResponseTypeDef",
     {
         "ScheduledActions": List[ScheduledActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeScalableTargetsResponseTypeDef = TypedDict(
     "DescribeScalableTargetsResponseTypeDef",
     {
         "ScalableTargets": List[ScalableTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTargetTrackingMetricStatTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatTypeDef",
     {
         "Metric": TargetTrackingMetricTypeDef,
@@ -812,10 +812,10 @@
 
 
 DescribeScalingPoliciesResponseTypeDef = TypedDict(
     "DescribeScalingPoliciesResponseTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling/type_defs.pyi` & `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,36 +33,36 @@
 
 __all__ = (
     "AlarmTypeDef",
     "MetricDimensionTypeDef",
     "DeleteScalingPolicyRequestRequestTypeDef",
     "DeleteScheduledActionRequestRequestTypeDef",
     "DeregisterScalableTargetRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
     "DescribeScalableTargetsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     "DescribeScalingActivitiesRequestRequestTypeDef",
+    "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     "DescribeScalingPoliciesRequestRequestTypeDef",
+    "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "NotScaledReasonTypeDef",
+    "PaginatorConfigTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "ScalableTargetActionTypeDef",
     "SuspendedStateTypeDef",
+    "RegisterScalableTargetResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "StepAdjustmentTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TargetTrackingMetricDimensionTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
-    "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
-    "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
-    "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PutScalingPolicyResponseTypeDef",
-    "RegisterScalableTargetResponseTypeDef",
     "ScalingActivityTypeDef",
     "PutScheduledActionRequestRequestTypeDef",
     "ScheduledActionTypeDef",
     "RegisterScalableTargetRequestRequestTypeDef",
     "ScalableTargetTypeDef",
     "StepScalingPolicyConfigurationTypeDef",
     "TargetTrackingMetricTypeDef",
@@ -119,24 +119,36 @@
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ServiceNamespace": ServiceNamespaceType,
+    },
+)
+_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+    {
+        "ResourceIds": Sequence[str],
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
+    _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeScalableTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalableTargetsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalableTargetsRequestRequestTypeDef = TypedDict(
@@ -152,24 +164,36 @@
 
 class DescribeScalableTargetsRequestRequestTypeDef(
     _RequiredDescribeScalableTargetsRequestRequestTypeDef,
     _OptionalDescribeScalableTargetsRequestRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ServiceNamespace": ServiceNamespaceType,
     },
 )
+_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+    {
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "IncludeNotScaledActivities": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
+    _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+):
+    pass
 
 _RequiredDescribeScalingActivitiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingActivitiesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
@@ -187,14 +211,37 @@
 
 class DescribeScalingActivitiesRequestRequestTypeDef(
     _RequiredDescribeScalingActivitiesRequestRequestTypeDef,
     _OptionalDescribeScalingActivitiesRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
+    {
+        "ServiceNamespace": ServiceNamespaceType,
+    },
+)
+_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
+    {
+        "PolicyNames": Sequence[str],
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
+    _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+    _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPoliciesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
@@ -211,14 +258,37 @@
 
 class DescribeScalingPoliciesRequestRequestTypeDef(
     _RequiredDescribeScalingPoliciesRequestRequestTypeDef,
     _OptionalDescribeScalingPoliciesRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    {
+        "ServiceNamespace": ServiceNamespaceType,
+    },
+)
+_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    {
+        "ScheduledActionNames": Sequence[str],
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
+    _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+    _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduledActionsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
@@ -242,14 +312,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredNotScaledReasonTypeDef = TypedDict(
     "_RequiredNotScaledReasonTypeDef",
     {
         "Code": str,
     },
 )
 _OptionalNotScaledReasonTypeDef = TypedDict(
@@ -261,14 +339,24 @@
     },
     total=False,
 )
 
 class NotScaledReasonTypeDef(_RequiredNotScaledReasonTypeDef, _OptionalNotScaledReasonTypeDef):
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
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
@@ -299,14 +387,33 @@
         "DynamicScalingInSuspended": bool,
         "DynamicScalingOutSuspended": bool,
         "ScheduledScalingSuspended": bool,
     },
     total=False,
 )
 
+RegisterScalableTargetResponseTypeDef = TypedDict(
+    "RegisterScalableTargetResponseTypeDef",
+    {
+        "ScalableTargetARN": str,
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
 _RequiredStepAdjustmentTypeDef = TypedDict(
     "_RequiredStepAdjustmentTypeDef",
     {
         "ScalingAdjustment": int,
     },
 )
 _OptionalStepAdjustmentTypeDef = TypedDict(
@@ -341,127 +448,20 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
-    {
-        "ResourceIds": Sequence[str],
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
-    _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-    _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
-    {
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "IncludeNotScaledActivities": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
-    _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-    _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
-    {
-        "PolicyNames": Sequence[str],
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
-    _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-    _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-):
-    pass
-
-_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
-    {
-        "ScheduledActionNames": Sequence[str],
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
-    _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-    _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-):
-    pass
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PutScalingPolicyResponseTypeDef = TypedDict(
     "PutScalingPolicyResponseTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterScalableTargetResponseTypeDef = TypedDict(
-    "RegisterScalableTargetResponseTypeDef",
-    {
-        "ScalableTargetARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredScalingActivityTypeDef = TypedDict(
     "_RequiredScalingActivityTypeDef",
     {
         "ActivityId": str,
@@ -614,33 +614,33 @@
 )
 
 DescribeScalingActivitiesResponseTypeDef = TypedDict(
     "DescribeScalingActivitiesResponseTypeDef",
     {
         "ScalingActivities": List[ScalingActivityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeScheduledActionsResponseTypeDef = TypedDict(
     "DescribeScheduledActionsResponseTypeDef",
     {
         "ScheduledActions": List[ScheduledActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeScalableTargetsResponseTypeDef = TypedDict(
     "DescribeScalableTargetsResponseTypeDef",
     {
         "ScalableTargets": List[ScalableTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTargetTrackingMetricStatTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatTypeDef",
     {
         "Metric": TargetTrackingMetricTypeDef,
@@ -769,10 +769,10 @@
     pass
 
 DescribeScalingPoliciesResponseTypeDef = TypedDict(
     "DescribeScalingPoliciesResponseTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/PKG-INFO` & `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-autoscaling
-Version: 1.26.95
-Summary: Type annotations for boto3.ApplicationAutoScaling 1.26.95 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.ApplicationAutoScaling 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-application-autoscaling"></a>
 
 # mypy-boto3-application-autoscaling
 
 [![PyPI - mypy-boto3-application-autoscaling](https://img.shields.io/pypi/v/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-application-autoscaling?color=blue)](https://pypistats.org/packages/mypy-boto3-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationAutoScaling 1.26.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[boto3.ApplicationAutoScaling 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
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
 [mypy-boto3-application-autoscaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,36 +352,36 @@
 ```python
 from mypy_boto3_application_autoscaling.type_defs import (
     AlarmTypeDef,
     MetricDimensionTypeDef,
     DeleteScalingPolicyRequestRequestTypeDef,
     DeleteScheduledActionRequestRequestTypeDef,
     DeregisterScalableTargetRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
     DescribeScalableTargetsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingActivitiesRequestRequestTypeDef,
+    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     DescribeScalingPoliciesRequestRequestTypeDef,
+    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NotScaledReasonTypeDef,
+    PaginatorConfigTypeDef,
     PredefinedMetricSpecificationTypeDef,
     ScalableTargetActionTypeDef,
     SuspendedStateTypeDef,
+    RegisterScalableTargetResponseTypeDef,
+    ResponseMetadataTypeDef,
     StepAdjustmentTypeDef,
     TagResourceRequestRequestTypeDef,
     TargetTrackingMetricDimensionTypeDef,
     UntagResourceRequestRequestTypeDef,
-    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
-    RegisterScalableTargetResponseTypeDef,
     ScalingActivityTypeDef,
     PutScheduledActionRequestRequestTypeDef,
     ScheduledActionTypeDef,
     RegisterScalableTargetRequestRequestTypeDef,
     ScalableTargetTypeDef,
     StepScalingPolicyConfigurationTypeDef,
     TargetTrackingMetricTypeDef,
@@ -405,42 +405,42 @@
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

### Comparing `mypy-boto3-application-autoscaling-1.26.95/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt` & `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.26.95/setup.py` & `mypy-boto3-application-autoscaling-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-application-autoscaling.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-application-autoscaling",
-    version="1.26.95",
+    version="1.27.0",
     packages=["mypy_boto3_application_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApplicationAutoScaling 1.26.95 service generated with"
-        " mypy-boto3-builder 7.13.0"
+        "Type annotations for boto3.ApplicationAutoScaling 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -49,11 +49,11 @@
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/"
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


# Comparing `tmp/mypy-boto3-autoscaling-plans-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-autoscaling-plans-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-autoscaling-plans-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:07 2022, max compression
+gzip compressed data, was "mypy-boto3-autoscaling-plans-1.27.0.tar", last modified: Mon Jul  3 19:50:24 2023, max compression
```

## Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1.tar` & `mypy-boto3-autoscaling-plans-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:07.736833 mypy-boto3-autoscaling-plans-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:30:51.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14768 2022-11-01 21:43:07.732833 mypy-boto3-autoscaling-plans-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13288 2022-11-01 21:30:51.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:07.732833 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-11-01 21:30:51.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-11-01 21:30:51.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-11-01 21:30:51.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9084 2022-11-01 21:30:51.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     9069 2022-11-01 21:30:51.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10139 2022-11-01 21:30:52.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    10137 2022-11-01 21:30:51.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3556 2022-11-01 21:30:51.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-11-01 21:30:51.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:30:51.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    14012 2022-11-01 21:30:52.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    13987 2022-11-01 21:30:52.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:30:51.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:07.732833 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14768 2022-11-01 21:43:07.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-11-01 21:43:07.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:07.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:07.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:07.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-01 21:43:07.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:07.736833 mypy-boto3-autoscaling-plans-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-11-01 21:30:51.000000 mypy-boto3-autoscaling-plans-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.810863 mypy-boto3-autoscaling-plans-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:58.000000 mypy-boto3-autoscaling-plans-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-07-03 19:50:24.810863 mypy-boto3-autoscaling-plans-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-07-03 19:32:58.000000 mypy-boto3-autoscaling-plans-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.806862 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-03 19:32:58.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-03 19:32:58.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 19:32:58.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-07-03 19:32:58.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-07-03 19:32:58.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-07-03 19:32:59.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-07-03 19:32:58.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-03 19:32:58.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-03 19:32:58.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:58.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-07-03 19:32:59.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-07-03 19:32:59.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:58.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.810863 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-07-03 19:50:24.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-03 19:50:24.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:24.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 19:50:24.000000 mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:24.810863 mypy-boto3-autoscaling-plans-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-03 19:32:58.000000 mypy-boto3-autoscaling-plans-1.27.0/setup.py
```

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/LICENSE` & `mypy-boto3-autoscaling-plans-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/PKG-INFO` & `mypy-boto3-autoscaling-plans-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling-plans
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.AutoScalingPlans 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.AutoScalingPlans 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/
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
 
 <a id="mypy-boto3-autoscaling-plans"></a>
 
 # mypy-boto3-autoscaling-plans
 
 [![PyPI - mypy-boto3-autoscaling-plans](https://img.shields.io/pypi/v/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-autoscaling-plans?color=blue)](https://pypistats.org/packages/mypy-boto3-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScalingPlans 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[boto3.AutoScalingPlans 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [mypy-boto3-autoscaling-plans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,29 +342,29 @@
 
 `mypy_boto3_autoscaling_plans.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling_plans.type_defs import (
     TagFilterTypeDef,
-    ResponseMetadataTypeDef,
+    CreateScalingPlanResponseTypeDef,
     MetricDimensionTypeDef,
     DatapointTypeDef,
     DeleteScalingPlanRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     DescribeScalingPlanResourcesRequestRequestTypeDef,
     GetScalingPlanResourceForecastDataRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PredefinedLoadMetricSpecificationTypeDef,
     PredefinedScalingMetricSpecificationTypeDef,
+    ResponseMetadataTypeDef,
     ApplicationSourceTypeDef,
-    CreateScalingPlanResponseTypeDef,
     CustomizedLoadMetricSpecificationTypeDef,
     CustomizedScalingMetricSpecificationTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
-    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
     DescribeScalingPlansRequestRequestTypeDef,
     TargetTrackingConfigurationTypeDef,
     ScalingInstructionTypeDef,
     ScalingPolicyTypeDef,
     CreateScalingPlanRequestRequestTypeDef,
     ScalingPlanTypeDef,
@@ -381,42 +382,42 @@
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

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/README.md` & `mypy-boto3-autoscaling-plans-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-autoscaling-plans"></a>
 
 # mypy-boto3-autoscaling-plans
 
 [![PyPI - mypy-boto3-autoscaling-plans](https://img.shields.io/pypi/v/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-autoscaling-plans?color=blue)](https://pypistats.org/packages/mypy-boto3-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScalingPlans 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[boto3.AutoScalingPlans 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [mypy-boto3-autoscaling-plans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,29 +310,29 @@
 
 `mypy_boto3_autoscaling_plans.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling_plans.type_defs import (
     TagFilterTypeDef,
-    ResponseMetadataTypeDef,
+    CreateScalingPlanResponseTypeDef,
     MetricDimensionTypeDef,
     DatapointTypeDef,
     DeleteScalingPlanRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     DescribeScalingPlanResourcesRequestRequestTypeDef,
     GetScalingPlanResourceForecastDataRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PredefinedLoadMetricSpecificationTypeDef,
     PredefinedScalingMetricSpecificationTypeDef,
+    ResponseMetadataTypeDef,
     ApplicationSourceTypeDef,
-    CreateScalingPlanResponseTypeDef,
     CustomizedLoadMetricSpecificationTypeDef,
     CustomizedScalingMetricSpecificationTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
-    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
     DescribeScalingPlansRequestRequestTypeDef,
     TargetTrackingConfigurationTypeDef,
     ScalingInstructionTypeDef,
     ScalingPolicyTypeDef,
     CreateScalingPlanRequestRequestTypeDef,
     ScalingPlanTypeDef,
@@ -350,42 +350,42 @@
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

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/__init__.py` & `mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/__init__.pyi` & `mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/__main__.py` & `mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AutoScalingPlans 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.AutoScalingPlans 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans\nOther"
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

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/client.py` & `mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/client.pyi` & `mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/literals.py` & `mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,23 +111,25 @@
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
@@ -137,30 +139,35 @@
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
@@ -186,14 +193,15 @@
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
@@ -238,51 +246,57 @@
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
@@ -295,14 +309,15 @@
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
@@ -314,28 +329,35 @@
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
@@ -344,14 +366,15 @@
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
@@ -362,55 +385,64 @@
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

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/literals.pyi` & `mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -109,23 +109,25 @@
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
@@ -135,30 +137,35 @@
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
@@ -184,14 +191,15 @@
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
@@ -236,51 +244,57 @@
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
@@ -293,14 +307,15 @@
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
@@ -312,28 +327,35 @@
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
@@ -342,14 +364,15 @@
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
@@ -360,55 +383,64 @@
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

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/paginator.py` & `mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScalingPlanResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlanResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/paginators/#describescalingplanresourcespaginator)
         """
 
 
@@ -72,13 +72,13 @@
 
     def paginate(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
         ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScalingPlansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/paginators/#describescalingplanspaginator)
         """
```

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/paginator.pyi` & `mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScalingPlanResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlanResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/paginators/#describescalingplanresourcespaginator)
         """
 
 class DescribeScalingPlansPaginator(Paginator):
@@ -68,13 +68,13 @@
 
     def paginate(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
         ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeScalingPlansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/paginators/#describescalingplanspaginator)
         """
```

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/type_defs.py` & `mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,29 +37,29 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagFilterTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateScalingPlanResponseTypeDef",
     "MetricDimensionTypeDef",
     "DatapointTypeDef",
     "DeleteScalingPlanRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     "DescribeScalingPlanResourcesRequestRequestTypeDef",
     "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PredefinedLoadMetricSpecificationTypeDef",
     "PredefinedScalingMetricSpecificationTypeDef",
+    "ResponseMetadataTypeDef",
     "ApplicationSourceTypeDef",
-    "CreateScalingPlanResponseTypeDef",
     "CustomizedLoadMetricSpecificationTypeDef",
     "CustomizedScalingMetricSpecificationTypeDef",
     "GetScalingPlanResourceForecastDataResponseTypeDef",
-    "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     "DescribeScalingPlansRequestRequestTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "ScalingInstructionTypeDef",
     "ScalingPolicyTypeDef",
     "CreateScalingPlanRequestRequestTypeDef",
     "ScalingPlanTypeDef",
@@ -74,22 +74,19 @@
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateScalingPlanResponseTypeDef = TypedDict(
+    "CreateScalingPlanResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ScalingPlanVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Name": str,
@@ -110,24 +107,37 @@
     "DeleteScalingPlanRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ScalingPlanName": str,
+        "ScalingPlanVersion": int,
+    },
+)
+_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
+    _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+    _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeScalingPlanResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPlanResourcesRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
@@ -158,14 +168,24 @@
         "ScalableDimension": ScalableDimensionType,
         "ForecastDataType": ForecastDataTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
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
 _RequiredPredefinedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedLoadMetricSpecificationTypeDef",
     {
         "PredefinedLoadMetricType": LoadMetricTypeType,
     },
 )
 _OptionalPredefinedLoadMetricSpecificationTypeDef = TypedDict(
@@ -202,31 +222,34 @@
 class PredefinedScalingMetricSpecificationTypeDef(
     _RequiredPredefinedScalingMetricSpecificationTypeDef,
     _OptionalPredefinedScalingMetricSpecificationTypeDef,
 ):
     pass
 
 
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
 ApplicationSourceTypeDef = TypedDict(
     "ApplicationSourceTypeDef",
     {
         "CloudFormationStackARN": str,
         "TagFilters": Sequence[TagFilterTypeDef],
     },
     total=False,
 )
 
-CreateScalingPlanResponseTypeDef = TypedDict(
-    "CreateScalingPlanResponseTypeDef",
-    {
-        "ScalingPlanVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCustomizedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedLoadMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
@@ -273,48 +296,25 @@
     pass
 
 
 GetScalingPlanResourceForecastDataResponseTypeDef = TypedDict(
     "GetScalingPlanResourceForecastDataResponseTypeDef",
     {
         "Datapoints": List[DatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ScalingPlanVersion": int,
-    },
-)
-_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
-    _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-    _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-):
-    pass
-
-
 DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     {
         "ScalingPlanNames": Sequence[str],
         "ScalingPlanVersion": int,
         "ApplicationSources": Sequence[ApplicationSourceTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeScalingPlansRequestRequestTypeDef = TypedDict(
     "DescribeScalingPlansRequestRequestTypeDef",
     {
@@ -491,19 +491,19 @@
 
 
 DescribeScalingPlansResponseTypeDef = TypedDict(
     "DescribeScalingPlansResponseTypeDef",
     {
         "ScalingPlans": List[ScalingPlanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeScalingPlanResourcesResponseTypeDef = TypedDict(
     "DescribeScalingPlanResourcesResponseTypeDef",
     {
         "ScalingPlanResources": List[ScalingPlanResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans/type_defs.pyi` & `mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -36,29 +36,29 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagFilterTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateScalingPlanResponseTypeDef",
     "MetricDimensionTypeDef",
     "DatapointTypeDef",
     "DeleteScalingPlanRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     "DescribeScalingPlanResourcesRequestRequestTypeDef",
     "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PredefinedLoadMetricSpecificationTypeDef",
     "PredefinedScalingMetricSpecificationTypeDef",
+    "ResponseMetadataTypeDef",
     "ApplicationSourceTypeDef",
-    "CreateScalingPlanResponseTypeDef",
     "CustomizedLoadMetricSpecificationTypeDef",
     "CustomizedScalingMetricSpecificationTypeDef",
     "GetScalingPlanResourceForecastDataResponseTypeDef",
-    "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     "DescribeScalingPlansRequestRequestTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "ScalingInstructionTypeDef",
     "ScalingPolicyTypeDef",
     "CreateScalingPlanRequestRequestTypeDef",
     "ScalingPlanTypeDef",
@@ -73,22 +73,19 @@
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateScalingPlanResponseTypeDef = TypedDict(
+    "CreateScalingPlanResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ScalingPlanVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Name": str,
@@ -109,24 +106,35 @@
     "DeleteScalingPlanRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ScalingPlanName": str,
+        "ScalingPlanVersion": int,
+    },
+)
+_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
+    _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+    _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeScalingPlanResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPlanResourcesRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
@@ -155,14 +163,24 @@
         "ScalableDimension": ScalableDimensionType,
         "ForecastDataType": ForecastDataTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
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
 _RequiredPredefinedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedLoadMetricSpecificationTypeDef",
     {
         "PredefinedLoadMetricType": LoadMetricTypeType,
     },
 )
 _OptionalPredefinedLoadMetricSpecificationTypeDef = TypedDict(
@@ -195,31 +213,34 @@
 
 class PredefinedScalingMetricSpecificationTypeDef(
     _RequiredPredefinedScalingMetricSpecificationTypeDef,
     _OptionalPredefinedScalingMetricSpecificationTypeDef,
 ):
     pass
 
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
 ApplicationSourceTypeDef = TypedDict(
     "ApplicationSourceTypeDef",
     {
         "CloudFormationStackARN": str,
         "TagFilters": Sequence[TagFilterTypeDef],
     },
     total=False,
 )
 
-CreateScalingPlanResponseTypeDef = TypedDict(
-    "CreateScalingPlanResponseTypeDef",
-    {
-        "ScalingPlanVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCustomizedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedLoadMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
@@ -262,46 +283,25 @@
 ):
     pass
 
 GetScalingPlanResourceForecastDataResponseTypeDef = TypedDict(
     "GetScalingPlanResourceForecastDataResponseTypeDef",
     {
         "Datapoints": List[DatapointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ScalingPlanVersion": int,
-    },
-)
-_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
-    _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-    _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-):
-    pass
-
 DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     {
         "ScalingPlanNames": Sequence[str],
         "ScalingPlanVersion": int,
         "ApplicationSources": Sequence[ApplicationSourceTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeScalingPlansRequestRequestTypeDef = TypedDict(
     "DescribeScalingPlansRequestRequestTypeDef",
     {
@@ -466,19 +466,19 @@
     pass
 
 DescribeScalingPlansResponseTypeDef = TypedDict(
     "DescribeScalingPlansResponseTypeDef",
     {
         "ScalingPlans": List[ScalingPlanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeScalingPlanResourcesResponseTypeDef = TypedDict(
     "DescribeScalingPlanResourcesResponseTypeDef",
     {
         "ScalingPlanResources": List[ScalingPlanResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO` & `mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling-plans
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.AutoScalingPlans 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.AutoScalingPlans 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/
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
 
 <a id="mypy-boto3-autoscaling-plans"></a>
 
 # mypy-boto3-autoscaling-plans
 
 [![PyPI - mypy-boto3-autoscaling-plans](https://img.shields.io/pypi/v/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-autoscaling-plans?color=blue)](https://pypistats.org/packages/mypy-boto3-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScalingPlans 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[boto3.AutoScalingPlans 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [mypy-boto3-autoscaling-plans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,29 +342,29 @@
 
 `mypy_boto3_autoscaling_plans.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling_plans.type_defs import (
     TagFilterTypeDef,
-    ResponseMetadataTypeDef,
+    CreateScalingPlanResponseTypeDef,
     MetricDimensionTypeDef,
     DatapointTypeDef,
     DeleteScalingPlanRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     DescribeScalingPlanResourcesRequestRequestTypeDef,
     GetScalingPlanResourceForecastDataRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PredefinedLoadMetricSpecificationTypeDef,
     PredefinedScalingMetricSpecificationTypeDef,
+    ResponseMetadataTypeDef,
     ApplicationSourceTypeDef,
-    CreateScalingPlanResponseTypeDef,
     CustomizedLoadMetricSpecificationTypeDef,
     CustomizedScalingMetricSpecificationTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
-    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
     DescribeScalingPlansRequestRequestTypeDef,
     TargetTrackingConfigurationTypeDef,
     ScalingInstructionTypeDef,
     ScalingPolicyTypeDef,
     CreateScalingPlanRequestRequestTypeDef,
     ScalingPlanTypeDef,
@@ -381,42 +382,42 @@
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

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt` & `mypy-boto3-autoscaling-plans-1.27.0/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.26.0.post1/setup.py` & `mypy-boto3-autoscaling-plans-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-autoscaling-plans.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-autoscaling-plans",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_autoscaling_plans"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AutoScalingPlans 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.AutoScalingPlans 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
     keywords="boto3 autoscaling-plans type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_autoscaling_plans": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_autoscaling_plans": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/",
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


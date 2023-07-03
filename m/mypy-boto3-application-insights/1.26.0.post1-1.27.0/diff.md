# Comparing `tmp/mypy-boto3-application-insights-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-application-insights-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-application-insights-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:05 2022, max compression
+gzip compressed data, was "mypy-boto3-application-insights-1.27.0.tar", last modified: Mon Jul  3 19:50:22 2023, max compression
```

## Comparing `mypy-boto3-application-insights-1.26.0.post1.tar` & `mypy-boto3-application-insights-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:05.704831 mypy-boto3-application-insights-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:30:30.000000 mypy-boto3-application-insights-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14947 2022-11-01 21:43:05.704831 mypy-boto3-application-insights-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13455 2022-11-01 21:30:30.000000 mypy-boto3-application-insights-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:05.696831 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-11-01 21:30:30.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-11-01 21:30:30.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-11-01 21:30:30.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20939 2022-11-01 21:30:31.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    20905 2022-11-01 21:30:30.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8800 2022-11-01 21:30:31.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8798 2022-11-01 21:30:31.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:30:30.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    19758 2022-11-01 21:30:31.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    19743 2022-11-01 21:30:31.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:30:30.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:05.704831 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14947 2022-11-01 21:43:05.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-11-01 21:43:05.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:05.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:05.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:05.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-01 21:43:05.000000 mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:05.704831 mypy-boto3-application-insights-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2082 2022-11-01 21:30:30.000000 mypy-boto3-application-insights-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.570823 mypy-boto3-application-insights-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:32.000000 mypy-boto3-application-insights-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-07-03 19:50:22.566823 mypy-boto3-application-insights-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-07-03 19:32:32.000000 mypy-boto3-application-insights-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.562823 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-03 19:32:32.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-03 19:32:32.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-03 19:32:32.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20934 2023-07-03 19:32:33.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20900 2023-07-03 19:32:32.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-07-03 19:32:33.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-07-03 19:32:33.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:32.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19796 2023-07-03 19:32:33.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-07-03 19:32:33.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:32.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.566823 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-07-03 19:50:22.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-03 19:50:22.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:22.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 19:50:22.000000 mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:22.570823 mypy-boto3-application-insights-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-03 19:32:32.000000 mypy-boto3-application-insights-1.27.0/setup.py
```

### Comparing `mypy-boto3-application-insights-1.26.0.post1/LICENSE` & `mypy-boto3-application-insights-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-application-insights-1.26.0.post1/PKG-INFO` & `mypy-boto3-application-insights-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-insights
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ApplicationInsights 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ApplicationInsights 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/
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
 
 <a id="mypy-boto3-application-insights"></a>
 
 # mypy-boto3-application-insights
 
 [![PyPI - mypy-boto3-application-insights](https://img.shields.io/pypi/v/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-application-insights?color=blue)](https://pypistats.org/packages/mypy-boto3-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationInsights 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[boto3.ApplicationInsights 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [mypy-boto3-application-insights docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,56 +313,56 @@
 
 ```python
 from mypy_boto3_application_insights.type_defs import (
     ApplicationComponentTypeDef,
     ApplicationInfoTypeDef,
     ConfigurationEventTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     CreateComponentRequestRequestTypeDef,
     CreateLogPatternRequestRequestTypeDef,
     LogPatternTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteLogPatternRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeComponentConfigurationRecommendationRequestRequestTypeDef,
+    DescribeComponentConfigurationRecommendationResponseTypeDef,
     DescribeComponentConfigurationRequestRequestTypeDef,
+    DescribeComponentConfigurationResponseTypeDef,
     DescribeComponentRequestRequestTypeDef,
     DescribeLogPatternRequestRequestTypeDef,
     DescribeObservationRequestRequestTypeDef,
     ObservationTypeDef,
     DescribeProblemObservationsRequestRequestTypeDef,
     DescribeProblemRequestRequestTypeDef,
     ProblemTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListConfigurationHistoryRequestRequestTypeDef,
     ListLogPatternSetsRequestRequestTypeDef,
+    ListLogPatternSetsResponseTypeDef,
     ListLogPatternsRequestRequestTypeDef,
     ListProblemsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateComponentConfigurationRequestRequestTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateLogPatternRequestRequestTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
+    DescribeComponentResponseTypeDef,
+    ListComponentsResponseTypeDef,
     CreateApplicationResponseTypeDef,
     DescribeApplicationResponseTypeDef,
-    DescribeComponentConfigurationRecommendationResponseTypeDef,
-    DescribeComponentConfigurationResponseTypeDef,
-    DescribeComponentResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListComponentsResponseTypeDef,
+    UpdateApplicationResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
-    ListLogPatternSetsResponseTypeDef,
+    CreateApplicationRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     RelatedObservationsTypeDef,
     DescribeProblemResponseTypeDef,
@@ -377,42 +378,42 @@
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

### Comparing `mypy-boto3-application-insights-1.26.0.post1/README.md` & `mypy-boto3-application-insights-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-application-insights"></a>
 
 # mypy-boto3-application-insights
 
 [![PyPI - mypy-boto3-application-insights](https://img.shields.io/pypi/v/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-application-insights?color=blue)](https://pypistats.org/packages/mypy-boto3-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationInsights 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[boto3.ApplicationInsights 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [mypy-boto3-application-insights docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,56 +281,56 @@
 
 ```python
 from mypy_boto3_application_insights.type_defs import (
     ApplicationComponentTypeDef,
     ApplicationInfoTypeDef,
     ConfigurationEventTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     CreateComponentRequestRequestTypeDef,
     CreateLogPatternRequestRequestTypeDef,
     LogPatternTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteLogPatternRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeComponentConfigurationRecommendationRequestRequestTypeDef,
+    DescribeComponentConfigurationRecommendationResponseTypeDef,
     DescribeComponentConfigurationRequestRequestTypeDef,
+    DescribeComponentConfigurationResponseTypeDef,
     DescribeComponentRequestRequestTypeDef,
     DescribeLogPatternRequestRequestTypeDef,
     DescribeObservationRequestRequestTypeDef,
     ObservationTypeDef,
     DescribeProblemObservationsRequestRequestTypeDef,
     DescribeProblemRequestRequestTypeDef,
     ProblemTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListConfigurationHistoryRequestRequestTypeDef,
     ListLogPatternSetsRequestRequestTypeDef,
+    ListLogPatternSetsResponseTypeDef,
     ListLogPatternsRequestRequestTypeDef,
     ListProblemsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateComponentConfigurationRequestRequestTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateLogPatternRequestRequestTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
+    DescribeComponentResponseTypeDef,
+    ListComponentsResponseTypeDef,
     CreateApplicationResponseTypeDef,
     DescribeApplicationResponseTypeDef,
-    DescribeComponentConfigurationRecommendationResponseTypeDef,
-    DescribeComponentConfigurationResponseTypeDef,
-    DescribeComponentResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListComponentsResponseTypeDef,
+    UpdateApplicationResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
-    ListLogPatternSetsResponseTypeDef,
+    CreateApplicationRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     RelatedObservationsTypeDef,
     DescribeProblemResponseTypeDef,
@@ -346,42 +346,42 @@
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

### Comparing `mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/__main__.py` & `mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApplicationInsights 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.ApplicationInsights 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights\nOther"
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

### Comparing `mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/client.py` & `mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         ResourceGroupName: str,
         PatternSetName: str,
         PatternName: str,
         Pattern: str,
         Rank: int
     ) -> CreateLogPatternResponseTypeDef:
         """
-        Adds an log pattern to a `LogPatternSet` .
+        Adds an log pattern to a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.create_log_pattern)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#create_log_pattern)
         """
 
     def delete_application(self, *, ResourceGroupName: str) -> Dict[str, Any]:
         """
@@ -166,15 +166,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#delete_component)
         """
 
     def delete_log_pattern(
         self, *, ResourceGroupName: str, PatternSetName: str, PatternName: str
     ) -> Dict[str, Any]:
         """
-        Removes the specified log pattern from a `LogPatternSet` .
+        Removes the specified log pattern from a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.delete_log_pattern)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#delete_log_pattern)
         """
 
     def describe_application(self, *, ResourceGroupName: str) -> DescribeApplicationResponseTypeDef:
         """
@@ -215,15 +215,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_component_configuration_recommendation)
         """
 
     def describe_log_pattern(
         self, *, ResourceGroupName: str, PatternSetName: str, PatternName: str
     ) -> DescribeLogPatternResponseTypeDef:
         """
-        Describe a specific log pattern from a `LogPatternSet` .
+        Describe a specific log pattern from a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_log_pattern)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_log_pattern)
         """
 
     def describe_observation(self, *, ObservationId: str) -> DescribeObservationResponseTypeDef:
         """
@@ -318,15 +318,15 @@
         *,
         ResourceGroupName: str,
         PatternSetName: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListLogPatternsResponseTypeDef:
         """
-        Lists the log patterns in the specific log `LogPatternSet` .
+        Lists the log patterns in the specific log `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_patterns)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_log_patterns)
         """
 
     def list_problems(
         self,
@@ -426,12 +426,12 @@
         ResourceGroupName: str,
         PatternSetName: str,
         PatternName: str,
         Pattern: str = ...,
         Rank: int = ...
     ) -> UpdateLogPatternResponseTypeDef:
         """
-        Adds a log pattern to a `LogPatternSet` .
+        Adds a log pattern to a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_log_pattern)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#update_log_pattern)
         """
```

### Comparing `mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/client.pyi` & `mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         ResourceGroupName: str,
         PatternSetName: str,
         PatternName: str,
         Pattern: str,
         Rank: int
     ) -> CreateLogPatternResponseTypeDef:
         """
-        Adds an log pattern to a `LogPatternSet` .
+        Adds an log pattern to a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.create_log_pattern)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#create_log_pattern)
         """
     def delete_application(self, *, ResourceGroupName: str) -> Dict[str, Any]:
         """
         Removes the specified application from monitoring.
@@ -154,15 +154,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.delete_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#delete_component)
         """
     def delete_log_pattern(
         self, *, ResourceGroupName: str, PatternSetName: str, PatternName: str
     ) -> Dict[str, Any]:
         """
-        Removes the specified log pattern from a `LogPatternSet` .
+        Removes the specified log pattern from a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.delete_log_pattern)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#delete_log_pattern)
         """
     def describe_application(self, *, ResourceGroupName: str) -> DescribeApplicationResponseTypeDef:
         """
         Describes the application.
@@ -198,15 +198,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_component_configuration_recommendation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_component_configuration_recommendation)
         """
     def describe_log_pattern(
         self, *, ResourceGroupName: str, PatternSetName: str, PatternName: str
     ) -> DescribeLogPatternResponseTypeDef:
         """
-        Describe a specific log pattern from a `LogPatternSet` .
+        Describe a specific log pattern from a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.describe_log_pattern)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#describe_log_pattern)
         """
     def describe_observation(self, *, ObservationId: str) -> DescribeObservationResponseTypeDef:
         """
         Describes an anomaly or error with the application.
@@ -292,15 +292,15 @@
         *,
         ResourceGroupName: str,
         PatternSetName: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListLogPatternsResponseTypeDef:
         """
-        Lists the log patterns in the specific log `LogPatternSet` .
+        Lists the log patterns in the specific log `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_patterns)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_log_patterns)
         """
     def list_problems(
         self,
         *,
@@ -392,12 +392,12 @@
         ResourceGroupName: str,
         PatternSetName: str,
         PatternName: str,
         Pattern: str = ...,
         Rank: int = ...
     ) -> UpdateLogPatternResponseTypeDef:
         """
-        Adds a log pattern to a `LogPatternSet` .
+        Adds a log pattern to a `LogPatternSet`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.update_log_pattern)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#update_log_pattern)
         """
```

### Comparing `mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/literals.py` & `mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "CloudWatchEventSourceType",
     "ConfigurationEventResourceTypeType",
     "ConfigurationEventStatusType",
     "DiscoveryTypeType",
     "FeedbackKeyType",
     "FeedbackValueType",
@@ -34,15 +33,14 @@
     "TierType",
     "ApplicationInsightsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 CloudWatchEventSourceType = Literal["CODE_DEPLOY", "EC2", "HEALTH", "RDS"]
 ConfigurationEventResourceTypeType = Literal[
     "CLOUDFORMATION", "CLOUDWATCH_ALARM", "CLOUDWATCH_LOG", "SSM_ASSOCIATION"
 ]
 ConfigurationEventStatusType = Literal["ERROR", "INFO", "WARN"]
 DiscoveryTypeType = Literal["ACCOUNT_BASED", "RESOURCE_GROUP_BASED"]
 FeedbackKeyType = Literal["INSIGHTS_FEEDBACK"]
@@ -84,23 +82,25 @@
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
@@ -110,30 +110,35 @@
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
@@ -159,14 +164,15 @@
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
@@ -211,51 +217,57 @@
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
@@ -268,14 +280,15 @@
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
@@ -287,28 +300,35 @@
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
@@ -317,14 +337,15 @@
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
@@ -335,55 +356,64 @@
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
@@ -410,14 +440,15 @@
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
```

### Comparing `mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/literals.pyi` & `mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "CloudWatchEventSourceType",
     "ConfigurationEventResourceTypeType",
     "ConfigurationEventStatusType",
     "DiscoveryTypeType",
     "FeedbackKeyType",
     "FeedbackValueType",
@@ -33,14 +34,15 @@
     "TierType",
     "ApplicationInsightsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 CloudWatchEventSourceType = Literal["CODE_DEPLOY", "EC2", "HEALTH", "RDS"]
 ConfigurationEventResourceTypeType = Literal[
     "CLOUDFORMATION", "CLOUDWATCH_ALARM", "CLOUDWATCH_LOG", "SSM_ASSOCIATION"
 ]
 ConfigurationEventStatusType = Literal["ERROR", "INFO", "WARN"]
 DiscoveryTypeType = Literal["ACCOUNT_BASED", "RESOURCE_GROUP_BASED"]
 FeedbackKeyType = Literal["INSIGHTS_FEEDBACK"]
@@ -82,23 +84,25 @@
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
@@ -108,30 +112,35 @@
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
@@ -157,14 +166,15 @@
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
@@ -209,51 +219,57 @@
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
@@ -266,14 +282,15 @@
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
@@ -285,28 +302,35 @@
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
@@ -315,14 +339,15 @@
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
@@ -333,55 +358,64 @@
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
@@ -408,14 +442,15 @@
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
```

### Comparing `mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/type_defs.py` & `mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,56 +39,56 @@
 
 
 __all__ = (
     "ApplicationComponentTypeDef",
     "ApplicationInfoTypeDef",
     "ConfigurationEventTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateComponentRequestRequestTypeDef",
     "CreateLogPatternRequestRequestTypeDef",
     "LogPatternTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteLogPatternRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DescribeComponentConfigurationRecommendationRequestRequestTypeDef",
+    "DescribeComponentConfigurationRecommendationResponseTypeDef",
     "DescribeComponentConfigurationRequestRequestTypeDef",
+    "DescribeComponentConfigurationResponseTypeDef",
     "DescribeComponentRequestRequestTypeDef",
     "DescribeLogPatternRequestRequestTypeDef",
     "DescribeObservationRequestRequestTypeDef",
     "ObservationTypeDef",
     "DescribeProblemObservationsRequestRequestTypeDef",
     "DescribeProblemRequestRequestTypeDef",
     "ProblemTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListConfigurationHistoryRequestRequestTypeDef",
     "ListLogPatternSetsRequestRequestTypeDef",
+    "ListLogPatternSetsResponseTypeDef",
     "ListLogPatternsRequestRequestTypeDef",
     "ListProblemsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateComponentConfigurationRequestRequestTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "UpdateLogPatternRequestRequestTypeDef",
-    "CreateApplicationRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "DescribeComponentResponseTypeDef",
+    "ListComponentsResponseTypeDef",
     "CreateApplicationResponseTypeDef",
     "DescribeApplicationResponseTypeDef",
-    "DescribeComponentConfigurationRecommendationResponseTypeDef",
-    "DescribeComponentConfigurationResponseTypeDef",
-    "DescribeComponentResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "ListComponentsResponseTypeDef",
+    "UpdateApplicationResponseTypeDef",
     "ListConfigurationHistoryResponseTypeDef",
-    "ListLogPatternSetsResponseTypeDef",
+    "CreateApplicationRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "UpdateApplicationResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateLogPatternResponseTypeDef",
     "DescribeLogPatternResponseTypeDef",
     "ListLogPatternsResponseTypeDef",
     "UpdateLogPatternResponseTypeDef",
     "DescribeObservationResponseTypeDef",
     "RelatedObservationsTypeDef",
     "DescribeProblemResponseTypeDef",
@@ -142,25 +142,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
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
 CreateComponentRequestRequestTypeDef = TypedDict(
     "CreateComponentRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
         "ResourceList": Sequence[str],
     },
@@ -224,22 +213,40 @@
     {
         "ResourceGroupName": str,
         "ComponentName": str,
         "Tier": TierType,
     },
 )
 
+DescribeComponentConfigurationRecommendationResponseTypeDef = TypedDict(
+    "DescribeComponentConfigurationRecommendationResponseTypeDef",
+    {
+        "ComponentConfiguration": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeComponentConfigurationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
 
+DescribeComponentConfigurationResponseTypeDef = TypedDict(
+    "DescribeComponentConfigurationResponseTypeDef",
+    {
+        "Monitor": bool,
+        "Tier": TierType,
+        "ComponentConfiguration": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeComponentRequestRequestTypeDef = TypedDict(
     "DescribeComponentRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
@@ -408,14 +415,24 @@
 class ListLogPatternSetsRequestRequestTypeDef(
     _RequiredListLogPatternSetsRequestRequestTypeDef,
     _OptionalListLogPatternSetsRequestRequestTypeDef,
 ):
     pass
 
 
+ListLogPatternSetsResponseTypeDef = TypedDict(
+    "ListLogPatternSetsResponseTypeDef",
+    {
+        "ResourceGroupName": str,
+        "LogPatternSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListLogPatternsRequestRequestTypeDef = TypedDict(
     "_RequiredListLogPatternsRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
     },
 )
 _OptionalListLogPatternsRequestRequestTypeDef = TypedDict(
@@ -451,14 +468,25 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -557,175 +585,147 @@
 
 class UpdateLogPatternRequestRequestTypeDef(
     _RequiredUpdateLogPatternRequestRequestTypeDef, _OptionalUpdateLogPatternRequestRequestTypeDef
 ):
     pass
 
 
-CreateApplicationRequestRequestTypeDef = TypedDict(
-    "CreateApplicationRequestRequestTypeDef",
+DescribeComponentResponseTypeDef = TypedDict(
+    "DescribeComponentResponseTypeDef",
     {
-        "ResourceGroupName": str,
-        "OpsCenterEnabled": bool,
-        "CWEMonitorEnabled": bool,
-        "OpsItemSNSTopicArn": str,
-        "Tags": Sequence[TagTypeDef],
-        "AutoConfigEnabled": bool,
-        "AutoCreate": bool,
-        "GroupingType": Literal["ACCOUNT_BASED"],
+        "ApplicationComponent": ApplicationComponentTypeDef,
+        "ResourceList": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+ListComponentsResponseTypeDef = TypedDict(
+    "ListComponentsResponseTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "ApplicationComponentList": List[ApplicationComponentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeApplicationResponseTypeDef = TypedDict(
     "DescribeApplicationResponseTypeDef",
     {
         "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeComponentConfigurationRecommendationResponseTypeDef = TypedDict(
-    "DescribeComponentConfigurationRecommendationResponseTypeDef",
-    {
-        "ComponentConfiguration": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeComponentConfigurationResponseTypeDef = TypedDict(
-    "DescribeComponentConfigurationResponseTypeDef",
-    {
-        "Monitor": bool,
-        "Tier": TierType,
-        "ComponentConfiguration": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeComponentResponseTypeDef = TypedDict(
-    "DescribeComponentResponseTypeDef",
-    {
-        "ApplicationComponent": ApplicationComponentTypeDef,
-        "ResourceList": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationInfoList": List[ApplicationInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListComponentsResponseTypeDef = TypedDict(
-    "ListComponentsResponseTypeDef",
+UpdateApplicationResponseTypeDef = TypedDict(
+    "UpdateApplicationResponseTypeDef",
     {
-        "ApplicationComponentList": List[ApplicationComponentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationInfo": ApplicationInfoTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListConfigurationHistoryResponseTypeDef = TypedDict(
     "ListConfigurationHistoryResponseTypeDef",
     {
         "EventList": List[ConfigurationEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListLogPatternSetsResponseTypeDef = TypedDict(
-    "ListLogPatternSetsResponseTypeDef",
+CreateApplicationRequestRequestTypeDef = TypedDict(
+    "CreateApplicationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
-        "LogPatternSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "OpsCenterEnabled": bool,
+        "CWEMonitorEnabled": bool,
+        "OpsItemSNSTopicArn": str,
+        "Tags": Sequence[TagTypeDef],
+        "AutoConfigEnabled": bool,
+        "AutoCreate": bool,
+        "GroupingType": Literal["ACCOUNT_BASED"],
     },
+    total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApplicationResponseTypeDef = TypedDict(
-    "UpdateApplicationResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreateLogPatternResponseTypeDef = TypedDict(
     "CreateLogPatternResponseTypeDef",
     {
         "LogPattern": LogPatternTypeDef,
         "ResourceGroupName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLogPatternResponseTypeDef = TypedDict(
     "DescribeLogPatternResponseTypeDef",
     {
         "ResourceGroupName": str,
         "LogPattern": LogPatternTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLogPatternsResponseTypeDef = TypedDict(
     "ListLogPatternsResponseTypeDef",
     {
         "ResourceGroupName": str,
         "LogPatterns": List[LogPatternTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLogPatternResponseTypeDef = TypedDict(
     "UpdateLogPatternResponseTypeDef",
     {
         "ResourceGroupName": str,
         "LogPattern": LogPatternTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeObservationResponseTypeDef = TypedDict(
     "DescribeObservationResponseTypeDef",
     {
         "Observation": ObservationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RelatedObservationsTypeDef = TypedDict(
     "RelatedObservationsTypeDef",
     {
         "ObservationList": List[ObservationTypeDef],
@@ -733,28 +733,28 @@
     total=False,
 )
 
 DescribeProblemResponseTypeDef = TypedDict(
     "DescribeProblemResponseTypeDef",
     {
         "Problem": ProblemTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProblemsResponseTypeDef = TypedDict(
     "ListProblemsResponseTypeDef",
     {
         "ProblemList": List[ProblemTypeDef],
         "NextToken": str,
         "ResourceGroupName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeProblemObservationsResponseTypeDef = TypedDict(
     "DescribeProblemObservationsResponseTypeDef",
     {
         "RelatedObservations": RelatedObservationsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights/type_defs.pyi` & `mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,56 +38,56 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApplicationComponentTypeDef",
     "ApplicationInfoTypeDef",
     "ConfigurationEventTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateComponentRequestRequestTypeDef",
     "CreateLogPatternRequestRequestTypeDef",
     "LogPatternTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteLogPatternRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DescribeComponentConfigurationRecommendationRequestRequestTypeDef",
+    "DescribeComponentConfigurationRecommendationResponseTypeDef",
     "DescribeComponentConfigurationRequestRequestTypeDef",
+    "DescribeComponentConfigurationResponseTypeDef",
     "DescribeComponentRequestRequestTypeDef",
     "DescribeLogPatternRequestRequestTypeDef",
     "DescribeObservationRequestRequestTypeDef",
     "ObservationTypeDef",
     "DescribeProblemObservationsRequestRequestTypeDef",
     "DescribeProblemRequestRequestTypeDef",
     "ProblemTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListConfigurationHistoryRequestRequestTypeDef",
     "ListLogPatternSetsRequestRequestTypeDef",
+    "ListLogPatternSetsResponseTypeDef",
     "ListLogPatternsRequestRequestTypeDef",
     "ListProblemsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateComponentConfigurationRequestRequestTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "UpdateLogPatternRequestRequestTypeDef",
-    "CreateApplicationRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "DescribeComponentResponseTypeDef",
+    "ListComponentsResponseTypeDef",
     "CreateApplicationResponseTypeDef",
     "DescribeApplicationResponseTypeDef",
-    "DescribeComponentConfigurationRecommendationResponseTypeDef",
-    "DescribeComponentConfigurationResponseTypeDef",
-    "DescribeComponentResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "ListComponentsResponseTypeDef",
+    "UpdateApplicationResponseTypeDef",
     "ListConfigurationHistoryResponseTypeDef",
-    "ListLogPatternSetsResponseTypeDef",
+    "CreateApplicationRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "UpdateApplicationResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateLogPatternResponseTypeDef",
     "DescribeLogPatternResponseTypeDef",
     "ListLogPatternsResponseTypeDef",
     "UpdateLogPatternResponseTypeDef",
     "DescribeObservationResponseTypeDef",
     "RelatedObservationsTypeDef",
     "DescribeProblemResponseTypeDef",
@@ -141,25 +141,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
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
 CreateComponentRequestRequestTypeDef = TypedDict(
     "CreateComponentRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
         "ResourceList": Sequence[str],
     },
@@ -223,22 +212,40 @@
     {
         "ResourceGroupName": str,
         "ComponentName": str,
         "Tier": TierType,
     },
 )
 
+DescribeComponentConfigurationRecommendationResponseTypeDef = TypedDict(
+    "DescribeComponentConfigurationRecommendationResponseTypeDef",
+    {
+        "ComponentConfiguration": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeComponentConfigurationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
 
+DescribeComponentConfigurationResponseTypeDef = TypedDict(
+    "DescribeComponentConfigurationResponseTypeDef",
+    {
+        "Monitor": bool,
+        "Tier": TierType,
+        "ComponentConfiguration": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeComponentRequestRequestTypeDef = TypedDict(
     "DescribeComponentRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
@@ -403,14 +410,24 @@
 
 class ListLogPatternSetsRequestRequestTypeDef(
     _RequiredListLogPatternSetsRequestRequestTypeDef,
     _OptionalListLogPatternSetsRequestRequestTypeDef,
 ):
     pass
 
+ListLogPatternSetsResponseTypeDef = TypedDict(
+    "ListLogPatternSetsResponseTypeDef",
+    {
+        "ResourceGroupName": str,
+        "LogPatternSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListLogPatternsRequestRequestTypeDef = TypedDict(
     "_RequiredListLogPatternsRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
     },
 )
 _OptionalListLogPatternsRequestRequestTypeDef = TypedDict(
@@ -444,14 +461,25 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -542,175 +570,147 @@
 )
 
 class UpdateLogPatternRequestRequestTypeDef(
     _RequiredUpdateLogPatternRequestRequestTypeDef, _OptionalUpdateLogPatternRequestRequestTypeDef
 ):
     pass
 
-CreateApplicationRequestRequestTypeDef = TypedDict(
-    "CreateApplicationRequestRequestTypeDef",
+DescribeComponentResponseTypeDef = TypedDict(
+    "DescribeComponentResponseTypeDef",
     {
-        "ResourceGroupName": str,
-        "OpsCenterEnabled": bool,
-        "CWEMonitorEnabled": bool,
-        "OpsItemSNSTopicArn": str,
-        "Tags": Sequence[TagTypeDef],
-        "AutoConfigEnabled": bool,
-        "AutoCreate": bool,
-        "GroupingType": Literal["ACCOUNT_BASED"],
+        "ApplicationComponent": ApplicationComponentTypeDef,
+        "ResourceList": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+ListComponentsResponseTypeDef = TypedDict(
+    "ListComponentsResponseTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "ApplicationComponentList": List[ApplicationComponentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeApplicationResponseTypeDef = TypedDict(
     "DescribeApplicationResponseTypeDef",
     {
         "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeComponentConfigurationRecommendationResponseTypeDef = TypedDict(
-    "DescribeComponentConfigurationRecommendationResponseTypeDef",
-    {
-        "ComponentConfiguration": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeComponentConfigurationResponseTypeDef = TypedDict(
-    "DescribeComponentConfigurationResponseTypeDef",
-    {
-        "Monitor": bool,
-        "Tier": TierType,
-        "ComponentConfiguration": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeComponentResponseTypeDef = TypedDict(
-    "DescribeComponentResponseTypeDef",
-    {
-        "ApplicationComponent": ApplicationComponentTypeDef,
-        "ResourceList": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationInfoList": List[ApplicationInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListComponentsResponseTypeDef = TypedDict(
-    "ListComponentsResponseTypeDef",
+UpdateApplicationResponseTypeDef = TypedDict(
+    "UpdateApplicationResponseTypeDef",
     {
-        "ApplicationComponentList": List[ApplicationComponentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ApplicationInfo": ApplicationInfoTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListConfigurationHistoryResponseTypeDef = TypedDict(
     "ListConfigurationHistoryResponseTypeDef",
     {
         "EventList": List[ConfigurationEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListLogPatternSetsResponseTypeDef = TypedDict(
-    "ListLogPatternSetsResponseTypeDef",
+CreateApplicationRequestRequestTypeDef = TypedDict(
+    "CreateApplicationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
-        "LogPatternSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "OpsCenterEnabled": bool,
+        "CWEMonitorEnabled": bool,
+        "OpsItemSNSTopicArn": str,
+        "Tags": Sequence[TagTypeDef],
+        "AutoConfigEnabled": bool,
+        "AutoCreate": bool,
+        "GroupingType": Literal["ACCOUNT_BASED"],
     },
+    total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateApplicationResponseTypeDef = TypedDict(
-    "UpdateApplicationResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreateLogPatternResponseTypeDef = TypedDict(
     "CreateLogPatternResponseTypeDef",
     {
         "LogPattern": LogPatternTypeDef,
         "ResourceGroupName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLogPatternResponseTypeDef = TypedDict(
     "DescribeLogPatternResponseTypeDef",
     {
         "ResourceGroupName": str,
         "LogPattern": LogPatternTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLogPatternsResponseTypeDef = TypedDict(
     "ListLogPatternsResponseTypeDef",
     {
         "ResourceGroupName": str,
         "LogPatterns": List[LogPatternTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateLogPatternResponseTypeDef = TypedDict(
     "UpdateLogPatternResponseTypeDef",
     {
         "ResourceGroupName": str,
         "LogPattern": LogPatternTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeObservationResponseTypeDef = TypedDict(
     "DescribeObservationResponseTypeDef",
     {
         "Observation": ObservationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RelatedObservationsTypeDef = TypedDict(
     "RelatedObservationsTypeDef",
     {
         "ObservationList": List[ObservationTypeDef],
@@ -718,28 +718,28 @@
     total=False,
 )
 
 DescribeProblemResponseTypeDef = TypedDict(
     "DescribeProblemResponseTypeDef",
     {
         "Problem": ProblemTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProblemsResponseTypeDef = TypedDict(
     "ListProblemsResponseTypeDef",
     {
         "ProblemList": List[ProblemTypeDef],
         "NextToken": str,
         "ResourceGroupName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeProblemObservationsResponseTypeDef = TypedDict(
     "DescribeProblemObservationsResponseTypeDef",
     {
         "RelatedObservations": RelatedObservationsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights.egg-info/PKG-INFO` & `mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-insights
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ApplicationInsights 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ApplicationInsights 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/
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
 
 <a id="mypy-boto3-application-insights"></a>
 
 # mypy-boto3-application-insights
 
 [![PyPI - mypy-boto3-application-insights](https://img.shields.io/pypi/v/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-application-insights?color=blue)](https://pypistats.org/packages/mypy-boto3-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationInsights 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[boto3.ApplicationInsights 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [mypy-boto3-application-insights docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,56 +313,56 @@
 
 ```python
 from mypy_boto3_application_insights.type_defs import (
     ApplicationComponentTypeDef,
     ApplicationInfoTypeDef,
     ConfigurationEventTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     CreateComponentRequestRequestTypeDef,
     CreateLogPatternRequestRequestTypeDef,
     LogPatternTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteLogPatternRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeComponentConfigurationRecommendationRequestRequestTypeDef,
+    DescribeComponentConfigurationRecommendationResponseTypeDef,
     DescribeComponentConfigurationRequestRequestTypeDef,
+    DescribeComponentConfigurationResponseTypeDef,
     DescribeComponentRequestRequestTypeDef,
     DescribeLogPatternRequestRequestTypeDef,
     DescribeObservationRequestRequestTypeDef,
     ObservationTypeDef,
     DescribeProblemObservationsRequestRequestTypeDef,
     DescribeProblemRequestRequestTypeDef,
     ProblemTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListConfigurationHistoryRequestRequestTypeDef,
     ListLogPatternSetsRequestRequestTypeDef,
+    ListLogPatternSetsResponseTypeDef,
     ListLogPatternsRequestRequestTypeDef,
     ListProblemsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateComponentConfigurationRequestRequestTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateLogPatternRequestRequestTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
+    DescribeComponentResponseTypeDef,
+    ListComponentsResponseTypeDef,
     CreateApplicationResponseTypeDef,
     DescribeApplicationResponseTypeDef,
-    DescribeComponentConfigurationRecommendationResponseTypeDef,
-    DescribeComponentConfigurationResponseTypeDef,
-    DescribeComponentResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListComponentsResponseTypeDef,
+    UpdateApplicationResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
-    ListLogPatternSetsResponseTypeDef,
+    CreateApplicationRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     RelatedObservationsTypeDef,
     DescribeProblemResponseTypeDef,
@@ -377,42 +378,42 @@
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

### Comparing `mypy-boto3-application-insights-1.26.0.post1/mypy_boto3_application_insights.egg-info/SOURCES.txt` & `mypy-boto3-application-insights-1.27.0/mypy_boto3_application_insights.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-insights-1.26.0.post1/setup.py` & `mypy-boto3-application-insights-1.27.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 """
 Setup script for mypy-boto3-application-insights.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-application-insights",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_application_insights"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApplicationInsights 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.ApplicationInsights 1.27.0 service generated with"
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
     keywords="boto3 application-insights type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_application_insights": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_application_insights": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/"
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


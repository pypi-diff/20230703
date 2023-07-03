# Comparing `tmp/mypy-boto3-inspector-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-inspector-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-inspector-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:32 2022, max compression
+gzip compressed data, was "mypy-boto3-inspector-1.27.0.tar", last modified: Mon Jul  3 19:50:52 2023, max compression
```

## Comparing `mypy-boto3-inspector-1.26.0.post1.tar` & `mypy-boto3-inspector-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:32.412828 mypy-boto3-inspector-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:35:48.000000 mypy-boto3-inspector-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    18821 2022-11-01 21:43:32.412828 mypy-boto3-inspector-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17372 2022-11-01 21:35:48.000000 mypy-boto3-inspector-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:32.404828 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-11-01 21:35:48.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-11-01 21:35:48.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-11-01 21:35:48.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31933 2022-11-01 21:35:48.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    31880 2022-11-01 21:35:48.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10198 2022-11-01 21:35:48.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    10196 2022-11-01 21:35:48.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11258 2022-11-01 21:35:48.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    11247 2022-11-01 21:35:48.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:35:48.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    40434 2022-11-01 21:35:49.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    40369 2022-11-01 21:35:49.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:35:48.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:32.412828 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18821 2022-11-01 21:43:32.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-11-01 21:43:32.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:32.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:32.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:32.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-01 21:43:32.000000 mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:32.412828 mypy-boto3-inspector-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-11-01 21:35:48.000000 mypy-boto3-inspector-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.475396 mypy-boto3-inspector-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:08.000000 mypy-boto3-inspector-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18845 2023-07-03 19:50:52.467395 mypy-boto3-inspector-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17352 2023-07-03 19:39:08.000000 mypy-boto3-inspector-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.463395 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-03 19:39:08.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-03 19:39:08.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:39:08.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31933 2023-07-03 19:39:08.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31880 2023-07-03 19:39:08.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-07-03 19:39:09.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-07-03 19:39:09.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-07-03 19:39:09.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-07-03 19:39:08.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:08.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40510 2023-07-03 19:39:10.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40445 2023-07-03 19:39:09.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:08.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:52.467395 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18845 2023-07-03 19:50:52.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 19:50:52.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:52.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:52.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:52.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:50:52.000000 mypy-boto3-inspector-1.27.0/mypy_boto3_inspector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:52.475396 mypy-boto3-inspector-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:39:08.000000 mypy-boto3-inspector-1.27.0/setup.py
```

### Comparing `mypy-boto3-inspector-1.26.0.post1/LICENSE` & `mypy-boto3-inspector-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-inspector-1.26.0.post1/PKG-INFO` & `mypy-boto3-inspector-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Inspector 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Inspector 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/
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
 
 <a id="mypy-boto3-inspector"></a>
 
 # mypy-boto3-inspector
 
 [![PyPI - mypy-boto3-inspector](https://img.shields.io/pypi/v/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-inspector?color=blue)](https://pypistats.org/packages/mypy-boto3-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
+[boto3.Inspector 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [mypy-boto3-inspector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -372,103 +373,103 @@
 `mypy_boto3_inspector.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_inspector.type_defs import (
     AttributeTypeDef,
     FailedItemDetailsTypeDef,
-    ResponseMetadataTypeDef,
     AgentFilterTypeDef,
     AgentPreviewTypeDef,
     TelemetryMetadataTypeDef,
     DurationRangeTypeDef,
     TimestampRangeTypeDef,
     AssessmentRunNotificationTypeDef,
     AssessmentRunStateChangeTypeDef,
     AssessmentTargetFilterTypeDef,
     AssessmentTargetTypeDef,
     TagTypeDef,
     CreateAssessmentTargetRequestRequestTypeDef,
+    CreateAssessmentTargetResponseTypeDef,
+    CreateAssessmentTemplateResponseTypeDef,
     CreateExclusionsPreviewRequestRequestTypeDef,
+    CreateExclusionsPreviewResponseTypeDef,
     ResourceGroupTagTypeDef,
+    CreateResourceGroupResponseTypeDef,
     DeleteAssessmentRunRequestRequestTypeDef,
     DeleteAssessmentTargetRequestRequestTypeDef,
     DeleteAssessmentTemplateRequestRequestTypeDef,
     DescribeAssessmentRunsRequestRequestTypeDef,
     DescribeAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTemplatesRequestRequestTypeDef,
+    DescribeCrossAccountAccessRoleResponseTypeDef,
     DescribeExclusionsRequestRequestTypeDef,
     DescribeFindingsRequestRequestTypeDef,
     DescribeResourceGroupsRequestRequestTypeDef,
     DescribeRulesPackagesRequestRequestTypeDef,
     RulesPackageTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventSubscriptionTypeDef,
     ScopeTypeDef,
     InspectorServiceAttributesTypeDef,
     GetAssessmentReportRequestRequestTypeDef,
+    GetAssessmentReportResponseTypeDef,
     GetExclusionsPreviewRequestRequestTypeDef,
     GetTelemetryMetadataRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssessmentRunsResponseTypeDef,
+    ListAssessmentTargetsResponseTypeDef,
+    ListAssessmentTemplatesResponseTypeDef,
+    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
     ListEventSubscriptionsRequestRequestTypeDef,
+    ListExclusionsRequestListExclusionsPaginateTypeDef,
     ListExclusionsRequestRequestTypeDef,
+    ListExclusionsResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
     ListRulesPackagesRequestRequestTypeDef,
+    ListRulesPackagesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PrivateIpTypeDef,
     SecurityGroupTypeDef,
+    PaginatorConfigTypeDef,
+    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     PreviewAgentsRequestRequestTypeDef,
     RegisterCrossAccountAccessRoleRequestRequestTypeDef,
     RemoveAttributesFromFindingsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     StartAssessmentRunRequestRequestTypeDef,
+    StartAssessmentRunResponseTypeDef,
     StopAssessmentRunRequestRequestTypeDef,
     SubscribeToEventRequestRequestTypeDef,
     UnsubscribeFromEventRequestRequestTypeDef,
     UpdateAssessmentTargetRequestRequestTypeDef,
     AddAttributesToFindingsRequestRequestTypeDef,
     AssessmentTemplateTypeDef,
     CreateAssessmentTemplateRequestRequestTypeDef,
     AddAttributesToFindingsResponseTypeDef,
-    CreateAssessmentTargetResponseTypeDef,
-    CreateAssessmentTemplateResponseTypeDef,
-    CreateExclusionsPreviewResponseTypeDef,
-    CreateResourceGroupResponseTypeDef,
-    DescribeCrossAccountAccessRoleResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAssessmentReportResponseTypeDef,
-    ListAssessmentRunsResponseTypeDef,
-    ListAssessmentTargetsResponseTypeDef,
-    ListAssessmentTemplatesResponseTypeDef,
-    ListExclusionsResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListRulesPackagesResponseTypeDef,
     RemoveAttributesFromFindingsResponseTypeDef,
-    StartAssessmentRunResponseTypeDef,
+    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
     ListAssessmentRunAgentsRequestRequestTypeDef,
     PreviewAgentsResponseTypeDef,
     AssessmentRunAgentTypeDef,
     GetTelemetryMetadataResponseTypeDef,
     AssessmentTemplateFilterTypeDef,
     AssessmentRunFilterTypeDef,
     FindingFilterTypeDef,
     AssessmentRunTypeDef,
+    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
     ListAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTargetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SetTagsForResourceRequestRequestTypeDef,
     CreateResourceGroupRequestRequestTypeDef,
     ResourceGroupTypeDef,
     DescribeRulesPackagesResponseTypeDef,
     SubscriptionTypeDef,
     ExclusionPreviewTypeDef,
     ExclusionTypeDef,
-    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
-    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
-    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
-    ListExclusionsRequestListExclusionsPaginateTypeDef,
-    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
-    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     NetworkInterfaceTypeDef,
     DescribeAssessmentTemplatesResponseTypeDef,
     ListAssessmentRunAgentsResponseTypeDef,
     ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef,
     ListAssessmentTemplatesRequestRequestTypeDef,
     ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
     ListAssessmentRunsRequestRequestTypeDef,
@@ -492,42 +493,42 @@
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

### Comparing `mypy-boto3-inspector-1.26.0.post1/README.md` & `mypy-boto3-inspector-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-inspector"></a>
 
 # mypy-boto3-inspector
 
 [![PyPI - mypy-boto3-inspector](https://img.shields.io/pypi/v/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-inspector?color=blue)](https://pypistats.org/packages/mypy-boto3-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
+[boto3.Inspector 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [mypy-boto3-inspector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,103 +341,103 @@
 `mypy_boto3_inspector.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_inspector.type_defs import (
     AttributeTypeDef,
     FailedItemDetailsTypeDef,
-    ResponseMetadataTypeDef,
     AgentFilterTypeDef,
     AgentPreviewTypeDef,
     TelemetryMetadataTypeDef,
     DurationRangeTypeDef,
     TimestampRangeTypeDef,
     AssessmentRunNotificationTypeDef,
     AssessmentRunStateChangeTypeDef,
     AssessmentTargetFilterTypeDef,
     AssessmentTargetTypeDef,
     TagTypeDef,
     CreateAssessmentTargetRequestRequestTypeDef,
+    CreateAssessmentTargetResponseTypeDef,
+    CreateAssessmentTemplateResponseTypeDef,
     CreateExclusionsPreviewRequestRequestTypeDef,
+    CreateExclusionsPreviewResponseTypeDef,
     ResourceGroupTagTypeDef,
+    CreateResourceGroupResponseTypeDef,
     DeleteAssessmentRunRequestRequestTypeDef,
     DeleteAssessmentTargetRequestRequestTypeDef,
     DeleteAssessmentTemplateRequestRequestTypeDef,
     DescribeAssessmentRunsRequestRequestTypeDef,
     DescribeAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTemplatesRequestRequestTypeDef,
+    DescribeCrossAccountAccessRoleResponseTypeDef,
     DescribeExclusionsRequestRequestTypeDef,
     DescribeFindingsRequestRequestTypeDef,
     DescribeResourceGroupsRequestRequestTypeDef,
     DescribeRulesPackagesRequestRequestTypeDef,
     RulesPackageTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventSubscriptionTypeDef,
     ScopeTypeDef,
     InspectorServiceAttributesTypeDef,
     GetAssessmentReportRequestRequestTypeDef,
+    GetAssessmentReportResponseTypeDef,
     GetExclusionsPreviewRequestRequestTypeDef,
     GetTelemetryMetadataRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssessmentRunsResponseTypeDef,
+    ListAssessmentTargetsResponseTypeDef,
+    ListAssessmentTemplatesResponseTypeDef,
+    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
     ListEventSubscriptionsRequestRequestTypeDef,
+    ListExclusionsRequestListExclusionsPaginateTypeDef,
     ListExclusionsRequestRequestTypeDef,
+    ListExclusionsResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
     ListRulesPackagesRequestRequestTypeDef,
+    ListRulesPackagesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PrivateIpTypeDef,
     SecurityGroupTypeDef,
+    PaginatorConfigTypeDef,
+    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     PreviewAgentsRequestRequestTypeDef,
     RegisterCrossAccountAccessRoleRequestRequestTypeDef,
     RemoveAttributesFromFindingsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     StartAssessmentRunRequestRequestTypeDef,
+    StartAssessmentRunResponseTypeDef,
     StopAssessmentRunRequestRequestTypeDef,
     SubscribeToEventRequestRequestTypeDef,
     UnsubscribeFromEventRequestRequestTypeDef,
     UpdateAssessmentTargetRequestRequestTypeDef,
     AddAttributesToFindingsRequestRequestTypeDef,
     AssessmentTemplateTypeDef,
     CreateAssessmentTemplateRequestRequestTypeDef,
     AddAttributesToFindingsResponseTypeDef,
-    CreateAssessmentTargetResponseTypeDef,
-    CreateAssessmentTemplateResponseTypeDef,
-    CreateExclusionsPreviewResponseTypeDef,
-    CreateResourceGroupResponseTypeDef,
-    DescribeCrossAccountAccessRoleResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAssessmentReportResponseTypeDef,
-    ListAssessmentRunsResponseTypeDef,
-    ListAssessmentTargetsResponseTypeDef,
-    ListAssessmentTemplatesResponseTypeDef,
-    ListExclusionsResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListRulesPackagesResponseTypeDef,
     RemoveAttributesFromFindingsResponseTypeDef,
-    StartAssessmentRunResponseTypeDef,
+    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
     ListAssessmentRunAgentsRequestRequestTypeDef,
     PreviewAgentsResponseTypeDef,
     AssessmentRunAgentTypeDef,
     GetTelemetryMetadataResponseTypeDef,
     AssessmentTemplateFilterTypeDef,
     AssessmentRunFilterTypeDef,
     FindingFilterTypeDef,
     AssessmentRunTypeDef,
+    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
     ListAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTargetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SetTagsForResourceRequestRequestTypeDef,
     CreateResourceGroupRequestRequestTypeDef,
     ResourceGroupTypeDef,
     DescribeRulesPackagesResponseTypeDef,
     SubscriptionTypeDef,
     ExclusionPreviewTypeDef,
     ExclusionTypeDef,
-    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
-    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
-    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
-    ListExclusionsRequestListExclusionsPaginateTypeDef,
-    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
-    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     NetworkInterfaceTypeDef,
     DescribeAssessmentTemplatesResponseTypeDef,
     ListAssessmentRunAgentsResponseTypeDef,
     ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef,
     ListAssessmentTemplatesRequestRequestTypeDef,
     ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
     ListAssessmentRunsRequestRequestTypeDef,
@@ -461,42 +461,42 @@
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

### Comparing `mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/__init__.py` & `mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/__init__.pyi` & `mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/__main__.py` & `mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Inspector 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.Inspector 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector\nOther"
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

### Comparing `mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/client.py` & `mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/client.pyi` & `mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/literals.py` & `mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AgentHealthCodeType",
     "AgentHealthType",
     "AssessmentRunNotificationSnsStatusCodeType",
     "AssessmentRunStateType",
     "AssetTypeType",
     "FailedItemErrorCodeType",
@@ -47,15 +46,14 @@
     "InspectorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AgentHealthCodeType = Literal["IDLE", "RUNNING", "SHUTDOWN", "THROTTLED", "UNHEALTHY", "UNKNOWN"]
 AgentHealthType = Literal["HEALTHY", "UNHEALTHY", "UNKNOWN"]
 AssessmentRunNotificationSnsStatusCodeType = Literal[
     "ACCESS_DENIED", "INTERNAL_ERROR", "SUCCESS", "TOPIC_DOES_NOT_EXIST"
 ]
 AssessmentRunStateType = Literal[
     "CANCELED",
@@ -117,23 +115,25 @@
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
@@ -143,30 +143,35 @@
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
@@ -192,14 +197,15 @@
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
@@ -244,51 +250,57 @@
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
@@ -301,14 +313,15 @@
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
@@ -320,28 +333,35 @@
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
@@ -350,14 +370,15 @@
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
@@ -368,55 +389,64 @@
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

### Comparing `mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/literals.pyi` & `mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AgentHealthCodeType",
     "AgentHealthType",
     "AssessmentRunNotificationSnsStatusCodeType",
     "AssessmentRunStateType",
     "AssetTypeType",
     "FailedItemErrorCodeType",
@@ -46,14 +47,15 @@
     "InspectorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AgentHealthCodeType = Literal["IDLE", "RUNNING", "SHUTDOWN", "THROTTLED", "UNHEALTHY", "UNKNOWN"]
 AgentHealthType = Literal["HEALTHY", "UNHEALTHY", "UNKNOWN"]
 AssessmentRunNotificationSnsStatusCodeType = Literal[
     "ACCESS_DENIED", "INTERNAL_ERROR", "SUCCESS", "TOPIC_DOES_NOT_EXIST"
 ]
 AssessmentRunStateType = Literal[
     "CANCELED",
@@ -115,23 +117,25 @@
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
@@ -141,30 +145,35 @@
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
@@ -190,14 +199,15 @@
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
@@ -242,51 +252,57 @@
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
@@ -299,14 +315,15 @@
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
@@ -318,28 +335,35 @@
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
@@ -348,14 +372,15 @@
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
@@ -366,55 +391,64 @@
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

### Comparing `mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/paginator.py` & `mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -65,170 +65,159 @@
     "ListEventSubscriptionsPaginator",
     "ListExclusionsPaginator",
     "ListFindingsPaginator",
     "ListRulesPackagesPaginator",
     "PreviewAgentsPaginator",
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
 class ListAssessmentRunAgentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRunAgents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunagentspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentRunArn: str,
         filter: AgentFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssessmentRunAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRunAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunagentspaginator)
         """
 
-
 class ListAssessmentRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentTemplateArns: Sequence[str] = ...,
         filter: AssessmentRunFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssessmentRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunspaginator)
         """
 
-
 class ListAssessmentTargetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTargets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttargetspaginator)
     """
 
     def paginate(
         self,
         *,
         filter: AssessmentTargetFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssessmentTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttargetspaginator)
         """
 
-
 class ListAssessmentTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentTargetArns: Sequence[str] = ...,
         filter: AssessmentTemplateFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssessmentTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttemplatespaginator)
         """
 
-
 class ListEventSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListEventSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listeventsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listeventsubscriptionspaginator)
         """
 
-
 class ListExclusionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListExclusions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listexclusionspaginator)
     """
 
     def paginate(
-        self, *, assessmentRunArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, assessmentRunArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExclusionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListExclusions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listexclusionspaginator)
         """
 
-
 class ListFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentRunArns: Sequence[str] = ...,
         filter: FindingFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listfindingspaginator)
         """
 
-
 class ListRulesPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListRulesPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listrulespackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRulesPackagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListRulesPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listrulespackagespaginator)
         """
 
-
 class PreviewAgentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.PreviewAgents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#previewagentspaginator)
     """
 
     def paginate(
-        self, *, previewAgentsArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, previewAgentsArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[PreviewAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.PreviewAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#previewagentspaginator)
         """
```

### Comparing `mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/paginator.pyi` & `mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,159 +65,170 @@
     "ListEventSubscriptionsPaginator",
     "ListExclusionsPaginator",
     "ListFindingsPaginator",
     "ListRulesPackagesPaginator",
     "PreviewAgentsPaginator",
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
 class ListAssessmentRunAgentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRunAgents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunagentspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentRunArn: str,
         filter: AgentFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssessmentRunAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRunAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunagentspaginator)
         """
 
+
 class ListAssessmentRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentTemplateArns: Sequence[str] = ...,
         filter: AssessmentRunFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssessmentRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmentrunspaginator)
         """
 
+
 class ListAssessmentTargetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTargets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttargetspaginator)
     """
 
     def paginate(
         self,
         *,
         filter: AssessmentTargetFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssessmentTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTargets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttargetspaginator)
         """
 
+
 class ListAssessmentTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentTargetArns: Sequence[str] = ...,
         filter: AssessmentTemplateFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssessmentTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listassessmenttemplatespaginator)
         """
 
+
 class ListEventSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListEventSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listeventsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listeventsubscriptionspaginator)
         """
 
+
 class ListExclusionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListExclusions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listexclusionspaginator)
     """
 
     def paginate(
-        self, *, assessmentRunArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, assessmentRunArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListExclusionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListExclusions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listexclusionspaginator)
         """
 
+
 class ListFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentRunArns: Sequence[str] = ...,
         filter: FindingFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listfindingspaginator)
         """
 
+
 class ListRulesPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListRulesPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listrulespackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRulesPackagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListRulesPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#listrulespackagespaginator)
         """
 
+
 class PreviewAgentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.PreviewAgents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#previewagentspaginator)
     """
 
     def paginate(
-        self, *, previewAgentsArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, previewAgentsArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[PreviewAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.PreviewAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/paginators/#previewagentspaginator)
         """
```

### Comparing `mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/type_defs.py` & `mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -36,107 +36,106 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AttributeTypeDef",
     "FailedItemDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "AgentFilterTypeDef",
     "AgentPreviewTypeDef",
     "TelemetryMetadataTypeDef",
     "DurationRangeTypeDef",
     "TimestampRangeTypeDef",
     "AssessmentRunNotificationTypeDef",
     "AssessmentRunStateChangeTypeDef",
     "AssessmentTargetFilterTypeDef",
     "AssessmentTargetTypeDef",
     "TagTypeDef",
     "CreateAssessmentTargetRequestRequestTypeDef",
+    "CreateAssessmentTargetResponseTypeDef",
+    "CreateAssessmentTemplateResponseTypeDef",
     "CreateExclusionsPreviewRequestRequestTypeDef",
+    "CreateExclusionsPreviewResponseTypeDef",
     "ResourceGroupTagTypeDef",
+    "CreateResourceGroupResponseTypeDef",
     "DeleteAssessmentRunRequestRequestTypeDef",
     "DeleteAssessmentTargetRequestRequestTypeDef",
     "DeleteAssessmentTemplateRequestRequestTypeDef",
     "DescribeAssessmentRunsRequestRequestTypeDef",
     "DescribeAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTemplatesRequestRequestTypeDef",
+    "DescribeCrossAccountAccessRoleResponseTypeDef",
     "DescribeExclusionsRequestRequestTypeDef",
     "DescribeFindingsRequestRequestTypeDef",
     "DescribeResourceGroupsRequestRequestTypeDef",
     "DescribeRulesPackagesRequestRequestTypeDef",
     "RulesPackageTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventSubscriptionTypeDef",
     "ScopeTypeDef",
     "InspectorServiceAttributesTypeDef",
     "GetAssessmentReportRequestRequestTypeDef",
+    "GetAssessmentReportResponseTypeDef",
     "GetExclusionsPreviewRequestRequestTypeDef",
     "GetTelemetryMetadataRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAssessmentRunsResponseTypeDef",
+    "ListAssessmentTargetsResponseTypeDef",
+    "ListAssessmentTemplatesResponseTypeDef",
+    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
     "ListEventSubscriptionsRequestRequestTypeDef",
+    "ListExclusionsRequestListExclusionsPaginateTypeDef",
     "ListExclusionsRequestRequestTypeDef",
+    "ListExclusionsResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
     "ListRulesPackagesRequestRequestTypeDef",
+    "ListRulesPackagesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PrivateIpTypeDef",
     "SecurityGroupTypeDef",
+    "PaginatorConfigTypeDef",
+    "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "PreviewAgentsRequestRequestTypeDef",
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "StartAssessmentRunRequestRequestTypeDef",
+    "StartAssessmentRunResponseTypeDef",
     "StopAssessmentRunRequestRequestTypeDef",
     "SubscribeToEventRequestRequestTypeDef",
     "UnsubscribeFromEventRequestRequestTypeDef",
     "UpdateAssessmentTargetRequestRequestTypeDef",
     "AddAttributesToFindingsRequestRequestTypeDef",
     "AssessmentTemplateTypeDef",
     "CreateAssessmentTemplateRequestRequestTypeDef",
     "AddAttributesToFindingsResponseTypeDef",
-    "CreateAssessmentTargetResponseTypeDef",
-    "CreateAssessmentTemplateResponseTypeDef",
-    "CreateExclusionsPreviewResponseTypeDef",
-    "CreateResourceGroupResponseTypeDef",
-    "DescribeCrossAccountAccessRoleResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAssessmentReportResponseTypeDef",
-    "ListAssessmentRunsResponseTypeDef",
-    "ListAssessmentTargetsResponseTypeDef",
-    "ListAssessmentTemplatesResponseTypeDef",
-    "ListExclusionsResponseTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListRulesPackagesResponseTypeDef",
     "RemoveAttributesFromFindingsResponseTypeDef",
-    "StartAssessmentRunResponseTypeDef",
+    "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
     "ListAssessmentRunAgentsRequestRequestTypeDef",
     "PreviewAgentsResponseTypeDef",
     "AssessmentRunAgentTypeDef",
     "GetTelemetryMetadataResponseTypeDef",
     "AssessmentTemplateFilterTypeDef",
     "AssessmentRunFilterTypeDef",
     "FindingFilterTypeDef",
     "AssessmentRunTypeDef",
+    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
     "ListAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTargetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SetTagsForResourceRequestRequestTypeDef",
     "CreateResourceGroupRequestRequestTypeDef",
     "ResourceGroupTypeDef",
     "DescribeRulesPackagesResponseTypeDef",
     "SubscriptionTypeDef",
     "ExclusionPreviewTypeDef",
     "ExclusionTypeDef",
-    "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
-    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
-    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
-    "ListExclusionsRequestListExclusionsPaginateTypeDef",
-    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
-    "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeAssessmentTemplatesResponseTypeDef",
     "ListAssessmentRunAgentsResponseTypeDef",
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     "ListAssessmentTemplatesRequestRequestTypeDef",
     "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
     "ListAssessmentRunsRequestRequestTypeDef",
@@ -162,38 +161,25 @@
     "_OptionalAttributeTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
-
 FailedItemDetailsTypeDef = TypedDict(
     "FailedItemDetailsTypeDef",
     {
         "failureCode": FailedItemErrorCodeType,
         "retryable": bool,
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
 AgentFilterTypeDef = TypedDict(
     "AgentFilterTypeDef",
     {
         "agentHealths": Sequence[AgentHealthType],
         "agentHealthCodes": Sequence[AgentHealthCodeType],
     },
 )
@@ -214,19 +200,17 @@
         "operatingSystem": str,
         "kernelVersion": str,
         "ipv4Address": str,
     },
     total=False,
 )
 
-
 class AgentPreviewTypeDef(_RequiredAgentPreviewTypeDef, _OptionalAgentPreviewTypeDef):
     pass
 
-
 _RequiredTelemetryMetadataTypeDef = TypedDict(
     "_RequiredTelemetryMetadataTypeDef",
     {
         "messageType": str,
         "count": int,
     },
 )
@@ -234,21 +218,19 @@
     "_OptionalTelemetryMetadataTypeDef",
     {
         "dataSize": int,
     },
     total=False,
 )
 
-
 class TelemetryMetadataTypeDef(
     _RequiredTelemetryMetadataTypeDef, _OptionalTelemetryMetadataTypeDef
 ):
     pass
 
-
 DurationRangeTypeDef = TypedDict(
     "DurationRangeTypeDef",
     {
         "minSeconds": int,
         "maxSeconds": int,
     },
     total=False,
@@ -277,21 +259,19 @@
         "message": str,
         "snsTopicArn": str,
         "snsPublishStatusCode": AssessmentRunNotificationSnsStatusCodeType,
     },
     total=False,
 )
 
-
 class AssessmentRunNotificationTypeDef(
     _RequiredAssessmentRunNotificationTypeDef, _OptionalAssessmentRunNotificationTypeDef
 ):
     pass
 
-
 AssessmentRunStateChangeTypeDef = TypedDict(
     "AssessmentRunStateChangeTypeDef",
     {
         "stateChangedAt": datetime,
         "state": AssessmentRunStateType,
     },
 )
@@ -317,85 +297,109 @@
     "_OptionalAssessmentTargetTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
-
 class AssessmentTargetTypeDef(_RequiredAssessmentTargetTypeDef, _OptionalAssessmentTargetTypeDef):
     pass
 
-
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
     "_OptionalTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 _RequiredCreateAssessmentTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTargetRequestRequestTypeDef",
     {
         "assessmentTargetName": str,
     },
 )
 _OptionalCreateAssessmentTargetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAssessmentTargetRequestRequestTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
-
 class CreateAssessmentTargetRequestRequestTypeDef(
     _RequiredCreateAssessmentTargetRequestRequestTypeDef,
     _OptionalCreateAssessmentTargetRequestRequestTypeDef,
 ):
     pass
 
+CreateAssessmentTargetResponseTypeDef = TypedDict(
+    "CreateAssessmentTargetResponseTypeDef",
+    {
+        "assessmentTargetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateAssessmentTemplateResponseTypeDef = TypedDict(
+    "CreateAssessmentTemplateResponseTypeDef",
+    {
+        "assessmentTemplateArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 CreateExclusionsPreviewRequestRequestTypeDef = TypedDict(
     "CreateExclusionsPreviewRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
     },
 )
 
+CreateExclusionsPreviewResponseTypeDef = TypedDict(
+    "CreateExclusionsPreviewResponseTypeDef",
+    {
+        "previewToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredResourceGroupTagTypeDef = TypedDict(
     "_RequiredResourceGroupTagTypeDef",
     {
         "key": str,
     },
 )
 _OptionalResourceGroupTagTypeDef = TypedDict(
     "_OptionalResourceGroupTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
 class ResourceGroupTagTypeDef(_RequiredResourceGroupTagTypeDef, _OptionalResourceGroupTagTypeDef):
     pass
 
+CreateResourceGroupResponseTypeDef = TypedDict(
+    "CreateResourceGroupResponseTypeDef",
+    {
+        "resourceGroupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 DeleteAssessmentRunRequestRequestTypeDef = TypedDict(
     "DeleteAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
@@ -431,57 +435,63 @@
 DescribeAssessmentTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeAssessmentTemplatesRequestRequestTypeDef",
     {
         "assessmentTemplateArns": Sequence[str],
     },
 )
 
+DescribeCrossAccountAccessRoleResponseTypeDef = TypedDict(
+    "DescribeCrossAccountAccessRoleResponseTypeDef",
+    {
+        "roleArn": str,
+        "valid": bool,
+        "registeredAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeExclusionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeExclusionsRequestRequestTypeDef",
     {
         "exclusionArns": Sequence[str],
     },
 )
 _OptionalDescribeExclusionsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeExclusionsRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
-
 class DescribeExclusionsRequestRequestTypeDef(
     _RequiredDescribeExclusionsRequestRequestTypeDef,
     _OptionalDescribeExclusionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
     },
 )
 _OptionalDescribeFindingsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeFindingsRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
-
 class DescribeFindingsRequestRequestTypeDef(
     _RequiredDescribeFindingsRequestRequestTypeDef, _OptionalDescribeFindingsRequestRequestTypeDef
 ):
     pass
 
-
 DescribeResourceGroupsRequestRequestTypeDef = TypedDict(
     "DescribeResourceGroupsRequestRequestTypeDef",
     {
         "resourceGroupArns": Sequence[str],
     },
 )
 
@@ -495,22 +505,20 @@
     "_OptionalDescribeRulesPackagesRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
-
 class DescribeRulesPackagesRequestRequestTypeDef(
     _RequiredDescribeRulesPackagesRequestRequestTypeDef,
     _OptionalDescribeRulesPackagesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredRulesPackageTypeDef = TypedDict(
     "_RequiredRulesPackageTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "provider": str,
@@ -520,18 +528,23 @@
     "_OptionalRulesPackageTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class RulesPackageTypeDef(_RequiredRulesPackageTypeDef, _OptionalRulesPackageTypeDef):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 EventSubscriptionTypeDef = TypedDict(
     "EventSubscriptionTypeDef",
     {
         "event": InspectorEventType,
         "subscribedAt": datetime,
     },
@@ -557,30 +570,37 @@
     {
         "assessmentRunArn": str,
         "rulesPackageArn": str,
     },
     total=False,
 )
 
-
 class InspectorServiceAttributesTypeDef(
     _RequiredInspectorServiceAttributesTypeDef, _OptionalInspectorServiceAttributesTypeDef
 ):
     pass
 
-
 GetAssessmentReportRequestRequestTypeDef = TypedDict(
     "GetAssessmentReportRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
         "reportFileFormat": ReportFileFormatType,
         "reportType": ReportTypeType,
     },
 )
 
+GetAssessmentReportResponseTypeDef = TypedDict(
+    "GetAssessmentReportResponseTypeDef",
+    {
+        "status": ReportStatusType,
+        "url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetExclusionsPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetExclusionsPreviewRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
         "previewToken": str,
     },
 )
@@ -590,49 +610,93 @@
         "nextToken": str,
         "maxResults": int,
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
-
 class GetExclusionsPreviewRequestRequestTypeDef(
     _RequiredGetExclusionsPreviewRequestRequestTypeDef,
     _OptionalGetExclusionsPreviewRequestRequestTypeDef,
 ):
     pass
 
-
 GetTelemetryMetadataRequestRequestTypeDef = TypedDict(
     "GetTelemetryMetadataRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAssessmentRunsResponseTypeDef = TypedDict(
+    "ListAssessmentRunsResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "assessmentRunArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAssessmentTargetsResponseTypeDef = TypedDict(
+    "ListAssessmentTargetsResponseTypeDef",
+    {
+        "assessmentTargetArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAssessmentTemplatesResponseTypeDef = TypedDict(
+    "ListAssessmentTemplatesResponseTypeDef",
+    {
+        "assessmentTemplateArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef = TypedDict(
+    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+    {
+        "resourceArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListEventSubscriptionsRequestRequestTypeDef = TypedDict(
     "ListEventSubscriptionsRequestRequestTypeDef",
     {
         "resourceArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
+    "_RequiredListExclusionsRequestListExclusionsPaginateTypeDef",
+    {
+        "assessmentRunArn": str,
+    },
+)
+_OptionalListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
+    "_OptionalListExclusionsRequestListExclusionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListExclusionsRequestListExclusionsPaginateTypeDef(
+    _RequiredListExclusionsRequestListExclusionsPaginateTypeDef,
+    _OptionalListExclusionsRequestListExclusionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListExclusionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExclusionsRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 _OptionalListExclusionsRequestRequestTypeDef = TypedDict(
@@ -640,30 +704,63 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListExclusionsRequestRequestTypeDef(
     _RequiredListExclusionsRequestRequestTypeDef, _OptionalListExclusionsRequestRequestTypeDef
 ):
     pass
 
+ListExclusionsResponseTypeDef = TypedDict(
+    "ListExclusionsResponseTypeDef",
+    {
+        "exclusionArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
+    {
+        "findingArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListRulesPackagesRequestListRulesPackagesPaginateTypeDef = TypedDict(
+    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListRulesPackagesRequestRequestTypeDef = TypedDict(
     "ListRulesPackagesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListRulesPackagesResponseTypeDef = TypedDict(
+    "ListRulesPackagesResponseTypeDef",
+    {
+        "rulesPackageArns": List[str],
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
 
@@ -681,14 +778,44 @@
     {
         "groupName": str,
         "groupId": str,
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
+_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
+    "_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
+    {
+        "previewAgentsArn": str,
+    },
+)
+_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
+    "_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class PreviewAgentsRequestPreviewAgentsPaginateTypeDef(
+    _RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
+    _OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
+):
+    pass
+
 _RequiredPreviewAgentsRequestRequestTypeDef = TypedDict(
     "_RequiredPreviewAgentsRequestRequestTypeDef",
     {
         "previewAgentsArn": str,
     },
 )
 _OptionalPreviewAgentsRequestRequestTypeDef = TypedDict(
@@ -696,21 +823,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class PreviewAgentsRequestRequestTypeDef(
     _RequiredPreviewAgentsRequestRequestTypeDef, _OptionalPreviewAgentsRequestRequestTypeDef
 ):
     pass
 
-
 RegisterCrossAccountAccessRoleRequestRequestTypeDef = TypedDict(
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     {
         "roleArn": str,
     },
 )
 
@@ -718,35 +843,52 @@
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributeKeys": Sequence[str],
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
 _RequiredStartAssessmentRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssessmentRunRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
     },
 )
 _OptionalStartAssessmentRunRequestRequestTypeDef = TypedDict(
     "_OptionalStartAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunName": str,
     },
     total=False,
 )
 
-
 class StartAssessmentRunRequestRequestTypeDef(
     _RequiredStartAssessmentRunRequestRequestTypeDef,
     _OptionalStartAssessmentRunRequestRequestTypeDef,
 ):
     pass
 
+StartAssessmentRunResponseTypeDef = TypedDict(
+    "StartAssessmentRunResponseTypeDef",
+    {
+        "assessmentRunArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredStopAssessmentRunRequestRequestTypeDef = TypedDict(
     "_RequiredStopAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
@@ -754,21 +896,19 @@
     "_OptionalStopAssessmentRunRequestRequestTypeDef",
     {
         "stopAction": StopActionType,
     },
     total=False,
 )
 
-
 class StopAssessmentRunRequestRequestTypeDef(
     _RequiredStopAssessmentRunRequestRequestTypeDef, _OptionalStopAssessmentRunRequestRequestTypeDef
 ):
     pass
 
-
 SubscribeToEventRequestRequestTypeDef = TypedDict(
     "SubscribeToEventRequestRequestTypeDef",
     {
         "resourceArn": str,
         "event": InspectorEventType,
         "topicArn": str,
     },
@@ -794,22 +934,20 @@
     "_OptionalUpdateAssessmentTargetRequestRequestTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
-
 class UpdateAssessmentTargetRequestRequestTypeDef(
     _RequiredUpdateAssessmentTargetRequestRequestTypeDef,
     _OptionalUpdateAssessmentTargetRequestRequestTypeDef,
 ):
     pass
 
-
 AddAttributesToFindingsRequestRequestTypeDef = TypedDict(
     "AddAttributesToFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributes": Sequence[AttributeTypeDef],
     },
 )
@@ -831,21 +969,19 @@
     "_OptionalAssessmentTemplateTypeDef",
     {
         "lastAssessmentRunArn": str,
     },
     total=False,
 )
 
-
 class AssessmentTemplateTypeDef(
     _RequiredAssessmentTemplateTypeDef, _OptionalAssessmentTemplateTypeDef
 ):
     pass
 
-
 _RequiredCreateAssessmentTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTemplateRequestRequestTypeDef",
     {
         "assessmentTargetArn": str,
         "assessmentTemplateName": str,
         "durationInSeconds": int,
         "rulesPackageArns": Sequence[str],
@@ -855,157 +991,56 @@
     "_OptionalCreateAssessmentTemplateRequestRequestTypeDef",
     {
         "userAttributesForFindings": Sequence[AttributeTypeDef],
     },
     total=False,
 )
 
-
 class CreateAssessmentTemplateRequestRequestTypeDef(
     _RequiredCreateAssessmentTemplateRequestRequestTypeDef,
     _OptionalCreateAssessmentTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 AddAttributesToFindingsResponseTypeDef = TypedDict(
     "AddAttributesToFindingsResponseTypeDef",
     {
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAssessmentTargetResponseTypeDef = TypedDict(
-    "CreateAssessmentTargetResponseTypeDef",
-    {
-        "assessmentTargetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAssessmentTemplateResponseTypeDef = TypedDict(
-    "CreateAssessmentTemplateResponseTypeDef",
-    {
-        "assessmentTemplateArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateExclusionsPreviewResponseTypeDef = TypedDict(
-    "CreateExclusionsPreviewResponseTypeDef",
-    {
-        "previewToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateResourceGroupResponseTypeDef = TypedDict(
-    "CreateResourceGroupResponseTypeDef",
-    {
-        "resourceGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeCrossAccountAccessRoleResponseTypeDef = TypedDict(
-    "DescribeCrossAccountAccessRoleResponseTypeDef",
-    {
-        "roleArn": str,
-        "valid": bool,
-        "registeredAt": datetime,
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
-GetAssessmentReportResponseTypeDef = TypedDict(
-    "GetAssessmentReportResponseTypeDef",
-    {
-        "status": ReportStatusType,
-        "url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAssessmentRunsResponseTypeDef = TypedDict(
-    "ListAssessmentRunsResponseTypeDef",
-    {
-        "assessmentRunArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAssessmentTargetsResponseTypeDef = TypedDict(
-    "ListAssessmentTargetsResponseTypeDef",
-    {
-        "assessmentTargetArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAssessmentTemplatesResponseTypeDef = TypedDict(
-    "ListAssessmentTemplatesResponseTypeDef",
-    {
-        "assessmentTemplateArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListExclusionsResponseTypeDef = TypedDict(
-    "ListExclusionsResponseTypeDef",
-    {
-        "exclusionArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "findingArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListRulesPackagesResponseTypeDef = TypedDict(
-    "ListRulesPackagesResponseTypeDef",
-    {
-        "rulesPackageArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RemoveAttributesFromFindingsResponseTypeDef = TypedDict(
     "RemoveAttributesFromFindingsResponseTypeDef",
     {
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartAssessmentRunResponseTypeDef = TypedDict(
-    "StartAssessmentRunResponseTypeDef",
+_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
+    "_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
     {
         "assessmentRunArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
+    "_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+    {
+        "filter": AgentFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef(
+    _RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    _OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+):
+    pass
 
 _RequiredListAssessmentRunAgentsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssessmentRunAgentsRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
@@ -1015,28 +1050,26 @@
         "filter": AgentFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAssessmentRunAgentsRequestRequestTypeDef(
     _RequiredListAssessmentRunAgentsRequestRequestTypeDef,
     _OptionalListAssessmentRunAgentsRequestRequestTypeDef,
 ):
     pass
 
-
 PreviewAgentsResponseTypeDef = TypedDict(
     "PreviewAgentsResponseTypeDef",
     {
         "agentPreviews": List[AgentPreviewTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAssessmentRunAgentTypeDef = TypedDict(
     "_RequiredAssessmentRunAgentTypeDef",
     {
         "agentId": str,
@@ -1051,26 +1084,24 @@
     {
         "agentHealthDetails": str,
         "autoScalingGroup": str,
     },
     total=False,
 )
 
-
 class AssessmentRunAgentTypeDef(
     _RequiredAssessmentRunAgentTypeDef, _OptionalAssessmentRunAgentTypeDef
 ):
     pass
 
-
 GetTelemetryMetadataResponseTypeDef = TypedDict(
     "GetTelemetryMetadataResponseTypeDef",
     {
         "telemetryMetadata": List[TelemetryMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssessmentTemplateFilterTypeDef = TypedDict(
     "AssessmentTemplateFilterTypeDef",
     {
         "namePattern": str,
@@ -1132,18 +1163,25 @@
     {
         "startedAt": datetime,
         "completedAt": datetime,
     },
     total=False,
 )
 
-
 class AssessmentRunTypeDef(_RequiredAssessmentRunTypeDef, _OptionalAssessmentRunTypeDef):
     pass
 
+ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef = TypedDict(
+    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
+    {
+        "filter": AssessmentTargetFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
 
 ListAssessmentTargetsRequestRequestTypeDef = TypedDict(
     "ListAssessmentTargetsRequestRequestTypeDef",
     {
         "filter": AssessmentTargetFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
@@ -1152,23 +1190,23 @@
 )
 
 DescribeAssessmentTargetsResponseTypeDef = TypedDict(
     "DescribeAssessmentTargetsResponseTypeDef",
     {
         "assessmentTargets": List[AssessmentTargetTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSetTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredSetTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1178,22 +1216,20 @@
     "_OptionalSetTagsForResourceRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class SetTagsForResourceRequestRequestTypeDef(
     _RequiredSetTagsForResourceRequestRequestTypeDef,
     _OptionalSetTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 CreateResourceGroupRequestRequestTypeDef = TypedDict(
     "CreateResourceGroupRequestRequestTypeDef",
     {
         "resourceGroupTags": Sequence[ResourceGroupTagTypeDef],
     },
 )
 
@@ -1207,15 +1243,15 @@
 )
 
 DescribeRulesPackagesResponseTypeDef = TypedDict(
     "DescribeRulesPackagesResponseTypeDef",
     {
         "rulesPackages": List[RulesPackageTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "resourceArn": str,
@@ -1237,19 +1273,17 @@
     "_OptionalExclusionPreviewTypeDef",
     {
         "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
-
 class ExclusionPreviewTypeDef(_RequiredExclusionPreviewTypeDef, _OptionalExclusionPreviewTypeDef):
     pass
 
-
 _RequiredExclusionTypeDef = TypedDict(
     "_RequiredExclusionTypeDef",
     {
         "arn": str,
         "title": str,
         "description": str,
         "recommendation": str,
@@ -1260,112 +1294,17 @@
     "_OptionalExclusionTypeDef",
     {
         "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
-
 class ExclusionTypeDef(_RequiredExclusionTypeDef, _OptionalExclusionTypeDef):
     pass
 
-
-_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
-    "_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
-    {
-        "assessmentRunArn": str,
-    },
-)
-_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
-    "_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
-    {
-        "filter": AgentFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef(
-    _RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
-    _OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
-):
-    pass
-
-
-ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef = TypedDict(
-    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
-    {
-        "filter": AssessmentTargetFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef = TypedDict(
-    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
-    {
-        "resourceArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
-    "_RequiredListExclusionsRequestListExclusionsPaginateTypeDef",
-    {
-        "assessmentRunArn": str,
-    },
-)
-_OptionalListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
-    "_OptionalListExclusionsRequestListExclusionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListExclusionsRequestListExclusionsPaginateTypeDef(
-    _RequiredListExclusionsRequestListExclusionsPaginateTypeDef,
-    _OptionalListExclusionsRequestListExclusionsPaginateTypeDef,
-):
-    pass
-
-
-ListRulesPackagesRequestListRulesPackagesPaginateTypeDef = TypedDict(
-    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
-    "_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
-    {
-        "previewAgentsArn": str,
-    },
-)
-_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
-    "_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class PreviewAgentsRequestPreviewAgentsPaginateTypeDef(
-    _RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
-    _OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
-):
-    pass
-
-
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "networkInterfaceId": str,
         "subnetId": str,
         "vpcId": str,
         "privateDnsName": str,
@@ -1380,33 +1319,33 @@
 )
 
 DescribeAssessmentTemplatesResponseTypeDef = TypedDict(
     "DescribeAssessmentTemplatesResponseTypeDef",
     {
         "assessmentTemplates": List[AssessmentTemplateTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssessmentRunAgentsResponseTypeDef = TypedDict(
     "ListAssessmentRunAgentsResponseTypeDef",
     {
         "assessmentRunAgents": List[AssessmentRunAgentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef = TypedDict(
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     {
         "assessmentTargetArns": Sequence[str],
         "filter": AssessmentTemplateFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAssessmentTemplatesRequestRequestTypeDef = TypedDict(
     "ListAssessmentTemplatesRequestRequestTypeDef",
     {
@@ -1419,15 +1358,15 @@
 )
 
 ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef = TypedDict(
     "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
     {
         "assessmentTemplateArns": Sequence[str],
         "filter": AssessmentRunFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAssessmentRunsRequestRequestTypeDef = TypedDict(
     "ListAssessmentRunsRequestRequestTypeDef",
     {
@@ -1440,15 +1379,15 @@
 )
 
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "assessmentRunArns": Sequence[str],
         "filter": FindingFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
@@ -1461,52 +1400,52 @@
 )
 
 DescribeAssessmentRunsResponseTypeDef = TypedDict(
     "DescribeAssessmentRunsResponseTypeDef",
     {
         "assessmentRuns": List[AssessmentRunTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeResourceGroupsResponseTypeDef = TypedDict(
     "DescribeResourceGroupsResponseTypeDef",
     {
         "resourceGroups": List[ResourceGroupTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventSubscriptionsResponseTypeDef = TypedDict(
     "ListEventSubscriptionsResponseTypeDef",
     {
         "subscriptions": List[SubscriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExclusionsPreviewResponseTypeDef = TypedDict(
     "GetExclusionsPreviewResponseTypeDef",
     {
         "previewStatus": PreviewStatusType,
         "exclusionPreviews": List[ExclusionPreviewTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExclusionsResponseTypeDef = TypedDict(
     "DescribeExclusionsResponseTypeDef",
     {
         "exclusions": Dict[str, ExclusionTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAssetAttributesTypeDef = TypedDict(
     "_RequiredAssetAttributesTypeDef",
     {
         "schemaVersion": int,
@@ -1522,19 +1461,17 @@
         "ipv4Addresses": List[str],
         "tags": List[TagTypeDef],
         "networkInterfaces": List[NetworkInterfaceTypeDef],
     },
     total=False,
 )
 
-
 class AssetAttributesTypeDef(_RequiredAssetAttributesTypeDef, _OptionalAssetAttributesTypeDef):
     pass
 
-
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "arn": str,
         "attributes": List[AttributeTypeDef],
         "userAttributes": List[AttributeTypeDef],
         "createdAt": datetime,
@@ -1557,20 +1494,18 @@
         "numericSeverity": float,
         "confidence": int,
         "indicatorOfCompromise": bool,
     },
     total=False,
 )
 
-
 class FindingTypeDef(_RequiredFindingTypeDef, _OptionalFindingTypeDef):
     pass
 
-
 DescribeFindingsResponseTypeDef = TypedDict(
     "DescribeFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector/type_defs.pyi` & `mypy-boto3-inspector-1.27.0/mypy_boto3_inspector/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,106 +36,107 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AttributeTypeDef",
     "FailedItemDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "AgentFilterTypeDef",
     "AgentPreviewTypeDef",
     "TelemetryMetadataTypeDef",
     "DurationRangeTypeDef",
     "TimestampRangeTypeDef",
     "AssessmentRunNotificationTypeDef",
     "AssessmentRunStateChangeTypeDef",
     "AssessmentTargetFilterTypeDef",
     "AssessmentTargetTypeDef",
     "TagTypeDef",
     "CreateAssessmentTargetRequestRequestTypeDef",
+    "CreateAssessmentTargetResponseTypeDef",
+    "CreateAssessmentTemplateResponseTypeDef",
     "CreateExclusionsPreviewRequestRequestTypeDef",
+    "CreateExclusionsPreviewResponseTypeDef",
     "ResourceGroupTagTypeDef",
+    "CreateResourceGroupResponseTypeDef",
     "DeleteAssessmentRunRequestRequestTypeDef",
     "DeleteAssessmentTargetRequestRequestTypeDef",
     "DeleteAssessmentTemplateRequestRequestTypeDef",
     "DescribeAssessmentRunsRequestRequestTypeDef",
     "DescribeAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTemplatesRequestRequestTypeDef",
+    "DescribeCrossAccountAccessRoleResponseTypeDef",
     "DescribeExclusionsRequestRequestTypeDef",
     "DescribeFindingsRequestRequestTypeDef",
     "DescribeResourceGroupsRequestRequestTypeDef",
     "DescribeRulesPackagesRequestRequestTypeDef",
     "RulesPackageTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventSubscriptionTypeDef",
     "ScopeTypeDef",
     "InspectorServiceAttributesTypeDef",
     "GetAssessmentReportRequestRequestTypeDef",
+    "GetAssessmentReportResponseTypeDef",
     "GetExclusionsPreviewRequestRequestTypeDef",
     "GetTelemetryMetadataRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAssessmentRunsResponseTypeDef",
+    "ListAssessmentTargetsResponseTypeDef",
+    "ListAssessmentTemplatesResponseTypeDef",
+    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
     "ListEventSubscriptionsRequestRequestTypeDef",
+    "ListExclusionsRequestListExclusionsPaginateTypeDef",
     "ListExclusionsRequestRequestTypeDef",
+    "ListExclusionsResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
     "ListRulesPackagesRequestRequestTypeDef",
+    "ListRulesPackagesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PrivateIpTypeDef",
     "SecurityGroupTypeDef",
+    "PaginatorConfigTypeDef",
+    "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "PreviewAgentsRequestRequestTypeDef",
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "StartAssessmentRunRequestRequestTypeDef",
+    "StartAssessmentRunResponseTypeDef",
     "StopAssessmentRunRequestRequestTypeDef",
     "SubscribeToEventRequestRequestTypeDef",
     "UnsubscribeFromEventRequestRequestTypeDef",
     "UpdateAssessmentTargetRequestRequestTypeDef",
     "AddAttributesToFindingsRequestRequestTypeDef",
     "AssessmentTemplateTypeDef",
     "CreateAssessmentTemplateRequestRequestTypeDef",
     "AddAttributesToFindingsResponseTypeDef",
-    "CreateAssessmentTargetResponseTypeDef",
-    "CreateAssessmentTemplateResponseTypeDef",
-    "CreateExclusionsPreviewResponseTypeDef",
-    "CreateResourceGroupResponseTypeDef",
-    "DescribeCrossAccountAccessRoleResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAssessmentReportResponseTypeDef",
-    "ListAssessmentRunsResponseTypeDef",
-    "ListAssessmentTargetsResponseTypeDef",
-    "ListAssessmentTemplatesResponseTypeDef",
-    "ListExclusionsResponseTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListRulesPackagesResponseTypeDef",
     "RemoveAttributesFromFindingsResponseTypeDef",
-    "StartAssessmentRunResponseTypeDef",
+    "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
     "ListAssessmentRunAgentsRequestRequestTypeDef",
     "PreviewAgentsResponseTypeDef",
     "AssessmentRunAgentTypeDef",
     "GetTelemetryMetadataResponseTypeDef",
     "AssessmentTemplateFilterTypeDef",
     "AssessmentRunFilterTypeDef",
     "FindingFilterTypeDef",
     "AssessmentRunTypeDef",
+    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
     "ListAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTargetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SetTagsForResourceRequestRequestTypeDef",
     "CreateResourceGroupRequestRequestTypeDef",
     "ResourceGroupTypeDef",
     "DescribeRulesPackagesResponseTypeDef",
     "SubscriptionTypeDef",
     "ExclusionPreviewTypeDef",
     "ExclusionTypeDef",
-    "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
-    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
-    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
-    "ListExclusionsRequestListExclusionsPaginateTypeDef",
-    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
-    "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeAssessmentTemplatesResponseTypeDef",
     "ListAssessmentRunAgentsResponseTypeDef",
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     "ListAssessmentTemplatesRequestRequestTypeDef",
     "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
     "ListAssessmentRunsRequestRequestTypeDef",
@@ -161,36 +162,27 @@
     "_OptionalAttributeTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
+
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
+
 FailedItemDetailsTypeDef = TypedDict(
     "FailedItemDetailsTypeDef",
     {
         "failureCode": FailedItemErrorCodeType,
         "retryable": bool,
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
 AgentFilterTypeDef = TypedDict(
     "AgentFilterTypeDef",
     {
         "agentHealths": Sequence[AgentHealthType],
         "agentHealthCodes": Sequence[AgentHealthCodeType],
     },
 )
@@ -211,17 +203,19 @@
         "operatingSystem": str,
         "kernelVersion": str,
         "ipv4Address": str,
     },
     total=False,
 )
 
+
 class AgentPreviewTypeDef(_RequiredAgentPreviewTypeDef, _OptionalAgentPreviewTypeDef):
     pass
 
+
 _RequiredTelemetryMetadataTypeDef = TypedDict(
     "_RequiredTelemetryMetadataTypeDef",
     {
         "messageType": str,
         "count": int,
     },
 )
@@ -229,19 +223,21 @@
     "_OptionalTelemetryMetadataTypeDef",
     {
         "dataSize": int,
     },
     total=False,
 )
 
+
 class TelemetryMetadataTypeDef(
     _RequiredTelemetryMetadataTypeDef, _OptionalTelemetryMetadataTypeDef
 ):
     pass
 
+
 DurationRangeTypeDef = TypedDict(
     "DurationRangeTypeDef",
     {
         "minSeconds": int,
         "maxSeconds": int,
     },
     total=False,
@@ -270,19 +266,21 @@
         "message": str,
         "snsTopicArn": str,
         "snsPublishStatusCode": AssessmentRunNotificationSnsStatusCodeType,
     },
     total=False,
 )
 
+
 class AssessmentRunNotificationTypeDef(
     _RequiredAssessmentRunNotificationTypeDef, _OptionalAssessmentRunNotificationTypeDef
 ):
     pass
 
+
 AssessmentRunStateChangeTypeDef = TypedDict(
     "AssessmentRunStateChangeTypeDef",
     {
         "stateChangedAt": datetime,
         "state": AssessmentRunStateType,
     },
 )
@@ -308,78 +306,118 @@
     "_OptionalAssessmentTargetTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
+
 class AssessmentTargetTypeDef(_RequiredAssessmentTargetTypeDef, _OptionalAssessmentTargetTypeDef):
     pass
 
+
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
     "_OptionalTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 _RequiredCreateAssessmentTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTargetRequestRequestTypeDef",
     {
         "assessmentTargetName": str,
     },
 )
 _OptionalCreateAssessmentTargetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAssessmentTargetRequestRequestTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
+
 class CreateAssessmentTargetRequestRequestTypeDef(
     _RequiredCreateAssessmentTargetRequestRequestTypeDef,
     _OptionalCreateAssessmentTargetRequestRequestTypeDef,
 ):
     pass
 
+
+CreateAssessmentTargetResponseTypeDef = TypedDict(
+    "CreateAssessmentTargetResponseTypeDef",
+    {
+        "assessmentTargetArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateAssessmentTemplateResponseTypeDef = TypedDict(
+    "CreateAssessmentTemplateResponseTypeDef",
+    {
+        "assessmentTemplateArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateExclusionsPreviewRequestRequestTypeDef = TypedDict(
     "CreateExclusionsPreviewRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
     },
 )
 
+CreateExclusionsPreviewResponseTypeDef = TypedDict(
+    "CreateExclusionsPreviewResponseTypeDef",
+    {
+        "previewToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredResourceGroupTagTypeDef = TypedDict(
     "_RequiredResourceGroupTagTypeDef",
     {
         "key": str,
     },
 )
 _OptionalResourceGroupTagTypeDef = TypedDict(
     "_OptionalResourceGroupTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
+
 class ResourceGroupTagTypeDef(_RequiredResourceGroupTagTypeDef, _OptionalResourceGroupTagTypeDef):
     pass
 
+
+CreateResourceGroupResponseTypeDef = TypedDict(
+    "CreateResourceGroupResponseTypeDef",
+    {
+        "resourceGroupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteAssessmentRunRequestRequestTypeDef = TypedDict(
     "DeleteAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 
@@ -414,53 +452,67 @@
 DescribeAssessmentTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeAssessmentTemplatesRequestRequestTypeDef",
     {
         "assessmentTemplateArns": Sequence[str],
     },
 )
 
+DescribeCrossAccountAccessRoleResponseTypeDef = TypedDict(
+    "DescribeCrossAccountAccessRoleResponseTypeDef",
+    {
+        "roleArn": str,
+        "valid": bool,
+        "registeredAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeExclusionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeExclusionsRequestRequestTypeDef",
     {
         "exclusionArns": Sequence[str],
     },
 )
 _OptionalDescribeExclusionsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeExclusionsRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
+
 class DescribeExclusionsRequestRequestTypeDef(
     _RequiredDescribeExclusionsRequestRequestTypeDef,
     _OptionalDescribeExclusionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
     },
 )
 _OptionalDescribeFindingsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeFindingsRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
+
 class DescribeFindingsRequestRequestTypeDef(
     _RequiredDescribeFindingsRequestRequestTypeDef, _OptionalDescribeFindingsRequestRequestTypeDef
 ):
     pass
 
+
 DescribeResourceGroupsRequestRequestTypeDef = TypedDict(
     "DescribeResourceGroupsRequestRequestTypeDef",
     {
         "resourceGroupArns": Sequence[str],
     },
 )
 
@@ -474,20 +526,22 @@
     "_OptionalDescribeRulesPackagesRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
+
 class DescribeRulesPackagesRequestRequestTypeDef(
     _RequiredDescribeRulesPackagesRequestRequestTypeDef,
     _OptionalDescribeRulesPackagesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredRulesPackageTypeDef = TypedDict(
     "_RequiredRulesPackageTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "provider": str,
@@ -497,17 +551,26 @@
     "_OptionalRulesPackageTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class RulesPackageTypeDef(_RequiredRulesPackageTypeDef, _OptionalRulesPackageTypeDef):
     pass
 
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EventSubscriptionTypeDef = TypedDict(
     "EventSubscriptionTypeDef",
     {
         "event": InspectorEventType,
         "subscribedAt": datetime,
     },
 )
@@ -532,28 +595,39 @@
     {
         "assessmentRunArn": str,
         "rulesPackageArn": str,
     },
     total=False,
 )
 
+
 class InspectorServiceAttributesTypeDef(
     _RequiredInspectorServiceAttributesTypeDef, _OptionalInspectorServiceAttributesTypeDef
 ):
     pass
 
+
 GetAssessmentReportRequestRequestTypeDef = TypedDict(
     "GetAssessmentReportRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
         "reportFileFormat": ReportFileFormatType,
         "reportType": ReportTypeType,
     },
 )
 
+GetAssessmentReportResponseTypeDef = TypedDict(
+    "GetAssessmentReportResponseTypeDef",
+    {
+        "status": ReportStatusType,
+        "url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetExclusionsPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetExclusionsPreviewRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
         "previewToken": str,
     },
 )
@@ -563,47 +637,97 @@
         "nextToken": str,
         "maxResults": int,
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
+
 class GetExclusionsPreviewRequestRequestTypeDef(
     _RequiredGetExclusionsPreviewRequestRequestTypeDef,
     _OptionalGetExclusionsPreviewRequestRequestTypeDef,
 ):
     pass
 
+
 GetTelemetryMetadataRequestRequestTypeDef = TypedDict(
     "GetTelemetryMetadataRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListAssessmentRunsResponseTypeDef = TypedDict(
+    "ListAssessmentRunsResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "assessmentRunArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAssessmentTargetsResponseTypeDef = TypedDict(
+    "ListAssessmentTargetsResponseTypeDef",
+    {
+        "assessmentTargetArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListAssessmentTemplatesResponseTypeDef = TypedDict(
+    "ListAssessmentTemplatesResponseTypeDef",
+    {
+        "assessmentTemplateArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef = TypedDict(
+    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+    {
+        "resourceArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListEventSubscriptionsRequestRequestTypeDef = TypedDict(
     "ListEventSubscriptionsRequestRequestTypeDef",
     {
         "resourceArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
+    "_RequiredListExclusionsRequestListExclusionsPaginateTypeDef",
+    {
+        "assessmentRunArn": str,
+    },
+)
+_OptionalListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
+    "_OptionalListExclusionsRequestListExclusionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListExclusionsRequestListExclusionsPaginateTypeDef(
+    _RequiredListExclusionsRequestListExclusionsPaginateTypeDef,
+    _OptionalListExclusionsRequestListExclusionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListExclusionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExclusionsRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 _OptionalListExclusionsRequestRequestTypeDef = TypedDict(
@@ -611,28 +735,65 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListExclusionsRequestRequestTypeDef(
     _RequiredListExclusionsRequestRequestTypeDef, _OptionalListExclusionsRequestRequestTypeDef
 ):
     pass
 
+
+ListExclusionsResponseTypeDef = TypedDict(
+    "ListExclusionsResponseTypeDef",
+    {
+        "exclusionArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
+    {
+        "findingArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListRulesPackagesRequestListRulesPackagesPaginateTypeDef = TypedDict(
+    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRulesPackagesRequestRequestTypeDef = TypedDict(
     "ListRulesPackagesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+ListRulesPackagesResponseTypeDef = TypedDict(
+    "ListRulesPackagesResponseTypeDef",
+    {
+        "rulesPackageArns": List[str],
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
 
@@ -650,14 +811,46 @@
     {
         "groupName": str,
         "groupId": str,
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
+_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
+    "_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
+    {
+        "previewAgentsArn": str,
+    },
+)
+_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
+    "_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class PreviewAgentsRequestPreviewAgentsPaginateTypeDef(
+    _RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
+    _OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredPreviewAgentsRequestRequestTypeDef = TypedDict(
     "_RequiredPreviewAgentsRequestRequestTypeDef",
     {
         "previewAgentsArn": str,
     },
 )
 _OptionalPreviewAgentsRequestRequestTypeDef = TypedDict(
@@ -665,19 +858,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class PreviewAgentsRequestRequestTypeDef(
     _RequiredPreviewAgentsRequestRequestTypeDef, _OptionalPreviewAgentsRequestRequestTypeDef
 ):
     pass
 
+
 RegisterCrossAccountAccessRoleRequestRequestTypeDef = TypedDict(
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     {
         "roleArn": str,
     },
 )
 
@@ -685,53 +880,76 @@
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributeKeys": Sequence[str],
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
 _RequiredStartAssessmentRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssessmentRunRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
     },
 )
 _OptionalStartAssessmentRunRequestRequestTypeDef = TypedDict(
     "_OptionalStartAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunName": str,
     },
     total=False,
 )
 
+
 class StartAssessmentRunRequestRequestTypeDef(
     _RequiredStartAssessmentRunRequestRequestTypeDef,
     _OptionalStartAssessmentRunRequestRequestTypeDef,
 ):
     pass
 
+
+StartAssessmentRunResponseTypeDef = TypedDict(
+    "StartAssessmentRunResponseTypeDef",
+    {
+        "assessmentRunArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStopAssessmentRunRequestRequestTypeDef = TypedDict(
     "_RequiredStopAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 _OptionalStopAssessmentRunRequestRequestTypeDef = TypedDict(
     "_OptionalStopAssessmentRunRequestRequestTypeDef",
     {
         "stopAction": StopActionType,
     },
     total=False,
 )
 
+
 class StopAssessmentRunRequestRequestTypeDef(
     _RequiredStopAssessmentRunRequestRequestTypeDef, _OptionalStopAssessmentRunRequestRequestTypeDef
 ):
     pass
 
+
 SubscribeToEventRequestRequestTypeDef = TypedDict(
     "SubscribeToEventRequestRequestTypeDef",
     {
         "resourceArn": str,
         "event": InspectorEventType,
         "topicArn": str,
     },
@@ -757,20 +975,22 @@
     "_OptionalUpdateAssessmentTargetRequestRequestTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
+
 class UpdateAssessmentTargetRequestRequestTypeDef(
     _RequiredUpdateAssessmentTargetRequestRequestTypeDef,
     _OptionalUpdateAssessmentTargetRequestRequestTypeDef,
 ):
     pass
 
+
 AddAttributesToFindingsRequestRequestTypeDef = TypedDict(
     "AddAttributesToFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributes": Sequence[AttributeTypeDef],
     },
 )
@@ -792,19 +1012,21 @@
     "_OptionalAssessmentTemplateTypeDef",
     {
         "lastAssessmentRunArn": str,
     },
     total=False,
 )
 
+
 class AssessmentTemplateTypeDef(
     _RequiredAssessmentTemplateTypeDef, _OptionalAssessmentTemplateTypeDef
 ):
     pass
 
+
 _RequiredCreateAssessmentTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTemplateRequestRequestTypeDef",
     {
         "assessmentTargetArn": str,
         "assessmentTemplateName": str,
         "durationInSeconds": int,
         "rulesPackageArns": Sequence[str],
@@ -814,155 +1036,60 @@
     "_OptionalCreateAssessmentTemplateRequestRequestTypeDef",
     {
         "userAttributesForFindings": Sequence[AttributeTypeDef],
     },
     total=False,
 )
 
+
 class CreateAssessmentTemplateRequestRequestTypeDef(
     _RequiredCreateAssessmentTemplateRequestRequestTypeDef,
     _OptionalCreateAssessmentTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 AddAttributesToFindingsResponseTypeDef = TypedDict(
     "AddAttributesToFindingsResponseTypeDef",
     {
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateAssessmentTargetResponseTypeDef = TypedDict(
-    "CreateAssessmentTargetResponseTypeDef",
-    {
-        "assessmentTargetArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAssessmentTemplateResponseTypeDef = TypedDict(
-    "CreateAssessmentTemplateResponseTypeDef",
-    {
-        "assessmentTemplateArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateExclusionsPreviewResponseTypeDef = TypedDict(
-    "CreateExclusionsPreviewResponseTypeDef",
-    {
-        "previewToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateResourceGroupResponseTypeDef = TypedDict(
-    "CreateResourceGroupResponseTypeDef",
-    {
-        "resourceGroupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeCrossAccountAccessRoleResponseTypeDef = TypedDict(
-    "DescribeCrossAccountAccessRoleResponseTypeDef",
-    {
-        "roleArn": str,
-        "valid": bool,
-        "registeredAt": datetime,
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
-GetAssessmentReportResponseTypeDef = TypedDict(
-    "GetAssessmentReportResponseTypeDef",
-    {
-        "status": ReportStatusType,
-        "url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAssessmentRunsResponseTypeDef = TypedDict(
-    "ListAssessmentRunsResponseTypeDef",
-    {
-        "assessmentRunArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAssessmentTargetsResponseTypeDef = TypedDict(
-    "ListAssessmentTargetsResponseTypeDef",
+RemoveAttributesFromFindingsResponseTypeDef = TypedDict(
+    "RemoveAttributesFromFindingsResponseTypeDef",
     {
-        "assessmentTargetArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "failedItems": Dict[str, FailedItemDetailsTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAssessmentTemplatesResponseTypeDef = TypedDict(
-    "ListAssessmentTemplatesResponseTypeDef",
+_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
+    "_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
     {
-        "assessmentTemplateArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "assessmentRunArn": str,
     },
 )
-
-ListExclusionsResponseTypeDef = TypedDict(
-    "ListExclusionsResponseTypeDef",
+_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
+    "_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
     {
-        "exclusionArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "filter": AgentFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
+    total=False,
 )
 
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "findingArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-ListRulesPackagesResponseTypeDef = TypedDict(
-    "ListRulesPackagesResponseTypeDef",
-    {
-        "rulesPackageArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef(
+    _RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    _OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+):
+    pass
 
-RemoveAttributesFromFindingsResponseTypeDef = TypedDict(
-    "RemoveAttributesFromFindingsResponseTypeDef",
-    {
-        "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartAssessmentRunResponseTypeDef = TypedDict(
-    "StartAssessmentRunResponseTypeDef",
-    {
-        "assessmentRunArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 _RequiredListAssessmentRunAgentsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssessmentRunAgentsRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
@@ -972,26 +1099,28 @@
         "filter": AgentFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAssessmentRunAgentsRequestRequestTypeDef(
     _RequiredListAssessmentRunAgentsRequestRequestTypeDef,
     _OptionalListAssessmentRunAgentsRequestRequestTypeDef,
 ):
     pass
 
+
 PreviewAgentsResponseTypeDef = TypedDict(
     "PreviewAgentsResponseTypeDef",
     {
         "agentPreviews": List[AgentPreviewTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAssessmentRunAgentTypeDef = TypedDict(
     "_RequiredAssessmentRunAgentTypeDef",
     {
         "agentId": str,
@@ -1006,24 +1135,26 @@
     {
         "agentHealthDetails": str,
         "autoScalingGroup": str,
     },
     total=False,
 )
 
+
 class AssessmentRunAgentTypeDef(
     _RequiredAssessmentRunAgentTypeDef, _OptionalAssessmentRunAgentTypeDef
 ):
     pass
 
+
 GetTelemetryMetadataResponseTypeDef = TypedDict(
     "GetTelemetryMetadataResponseTypeDef",
     {
         "telemetryMetadata": List[TelemetryMetadataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssessmentTemplateFilterTypeDef = TypedDict(
     "AssessmentTemplateFilterTypeDef",
     {
         "namePattern": str,
@@ -1085,17 +1216,28 @@
     {
         "startedAt": datetime,
         "completedAt": datetime,
     },
     total=False,
 )
 
+
 class AssessmentRunTypeDef(_RequiredAssessmentRunTypeDef, _OptionalAssessmentRunTypeDef):
     pass
 
+
+ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef = TypedDict(
+    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
+    {
+        "filter": AssessmentTargetFilterTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListAssessmentTargetsRequestRequestTypeDef = TypedDict(
     "ListAssessmentTargetsRequestRequestTypeDef",
     {
         "filter": AssessmentTargetFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1103,23 +1245,23 @@
 )
 
 DescribeAssessmentTargetsResponseTypeDef = TypedDict(
     "DescribeAssessmentTargetsResponseTypeDef",
     {
         "assessmentTargets": List[AssessmentTargetTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSetTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredSetTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1129,20 +1271,22 @@
     "_OptionalSetTagsForResourceRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class SetTagsForResourceRequestRequestTypeDef(
     _RequiredSetTagsForResourceRequestRequestTypeDef,
     _OptionalSetTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 CreateResourceGroupRequestRequestTypeDef = TypedDict(
     "CreateResourceGroupRequestRequestTypeDef",
     {
         "resourceGroupTags": Sequence[ResourceGroupTagTypeDef],
     },
 )
 
@@ -1156,15 +1300,15 @@
 )
 
 DescribeRulesPackagesResponseTypeDef = TypedDict(
     "DescribeRulesPackagesResponseTypeDef",
     {
         "rulesPackages": List[RulesPackageTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "resourceArn": str,
@@ -1186,17 +1330,19 @@
     "_OptionalExclusionPreviewTypeDef",
     {
         "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
+
 class ExclusionPreviewTypeDef(_RequiredExclusionPreviewTypeDef, _OptionalExclusionPreviewTypeDef):
     pass
 
+
 _RequiredExclusionTypeDef = TypedDict(
     "_RequiredExclusionTypeDef",
     {
         "arn": str,
         "title": str,
         "description": str,
         "recommendation": str,
@@ -1207,103 +1353,18 @@
     "_OptionalExclusionTypeDef",
     {
         "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
-class ExclusionTypeDef(_RequiredExclusionTypeDef, _OptionalExclusionTypeDef):
-    pass
-
-_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
-    "_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
-    {
-        "assessmentRunArn": str,
-    },
-)
-_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
-    "_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
-    {
-        "filter": AgentFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef(
-    _RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
-    _OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
-):
-    pass
-
-ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef = TypedDict(
-    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
-    {
-        "filter": AssessmentTargetFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef = TypedDict(
-    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
-    {
-        "resourceArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
-_RequiredListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
-    "_RequiredListExclusionsRequestListExclusionsPaginateTypeDef",
-    {
-        "assessmentRunArn": str,
-    },
-)
-_OptionalListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
-    "_OptionalListExclusionsRequestListExclusionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListExclusionsRequestListExclusionsPaginateTypeDef(
-    _RequiredListExclusionsRequestListExclusionsPaginateTypeDef,
-    _OptionalListExclusionsRequestListExclusionsPaginateTypeDef,
-):
+class ExclusionTypeDef(_RequiredExclusionTypeDef, _OptionalExclusionTypeDef):
     pass
 
-ListRulesPackagesRequestListRulesPackagesPaginateTypeDef = TypedDict(
-    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
-    "_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
-    {
-        "previewAgentsArn": str,
-    },
-)
-_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
-    "_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class PreviewAgentsRequestPreviewAgentsPaginateTypeDef(
-    _RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
-    _OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
-):
-    pass
 
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "networkInterfaceId": str,
         "subnetId": str,
         "vpcId": str,
@@ -1319,33 +1380,33 @@
 )
 
 DescribeAssessmentTemplatesResponseTypeDef = TypedDict(
     "DescribeAssessmentTemplatesResponseTypeDef",
     {
         "assessmentTemplates": List[AssessmentTemplateTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssessmentRunAgentsResponseTypeDef = TypedDict(
     "ListAssessmentRunAgentsResponseTypeDef",
     {
         "assessmentRunAgents": List[AssessmentRunAgentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef = TypedDict(
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     {
         "assessmentTargetArns": Sequence[str],
         "filter": AssessmentTemplateFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAssessmentTemplatesRequestRequestTypeDef = TypedDict(
     "ListAssessmentTemplatesRequestRequestTypeDef",
     {
@@ -1358,15 +1419,15 @@
 )
 
 ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef = TypedDict(
     "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
     {
         "assessmentTemplateArns": Sequence[str],
         "filter": AssessmentRunFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListAssessmentRunsRequestRequestTypeDef = TypedDict(
     "ListAssessmentRunsRequestRequestTypeDef",
     {
@@ -1379,15 +1440,15 @@
 )
 
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "assessmentRunArns": Sequence[str],
         "filter": FindingFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
@@ -1400,52 +1461,52 @@
 )
 
 DescribeAssessmentRunsResponseTypeDef = TypedDict(
     "DescribeAssessmentRunsResponseTypeDef",
     {
         "assessmentRuns": List[AssessmentRunTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeResourceGroupsResponseTypeDef = TypedDict(
     "DescribeResourceGroupsResponseTypeDef",
     {
         "resourceGroups": List[ResourceGroupTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventSubscriptionsResponseTypeDef = TypedDict(
     "ListEventSubscriptionsResponseTypeDef",
     {
         "subscriptions": List[SubscriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetExclusionsPreviewResponseTypeDef = TypedDict(
     "GetExclusionsPreviewResponseTypeDef",
     {
         "previewStatus": PreviewStatusType,
         "exclusionPreviews": List[ExclusionPreviewTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExclusionsResponseTypeDef = TypedDict(
     "DescribeExclusionsResponseTypeDef",
     {
         "exclusions": Dict[str, ExclusionTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAssetAttributesTypeDef = TypedDict(
     "_RequiredAssetAttributesTypeDef",
     {
         "schemaVersion": int,
@@ -1461,17 +1522,19 @@
         "ipv4Addresses": List[str],
         "tags": List[TagTypeDef],
         "networkInterfaces": List[NetworkInterfaceTypeDef],
     },
     total=False,
 )
 
+
 class AssetAttributesTypeDef(_RequiredAssetAttributesTypeDef, _OptionalAssetAttributesTypeDef):
     pass
 
+
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "arn": str,
         "attributes": List[AttributeTypeDef],
         "userAttributes": List[AttributeTypeDef],
         "createdAt": datetime,
@@ -1494,18 +1557,20 @@
         "numericSeverity": float,
         "confidence": int,
         "indicatorOfCompromise": bool,
     },
     total=False,
 )
 
+
 class FindingTypeDef(_RequiredFindingTypeDef, _OptionalFindingTypeDef):
     pass
 
+
 DescribeFindingsResponseTypeDef = TypedDict(
     "DescribeFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector.egg-info/PKG-INFO` & `mypy-boto3-inspector-1.27.0/mypy_boto3_inspector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.Inspector 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Inspector 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/
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
 
 <a id="mypy-boto3-inspector"></a>
 
 # mypy-boto3-inspector
 
 [![PyPI - mypy-boto3-inspector](https://img.shields.io/pypi/v/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-inspector?color=blue)](https://pypistats.org/packages/mypy-boto3-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
+[boto3.Inspector 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [mypy-boto3-inspector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -372,103 +373,103 @@
 `mypy_boto3_inspector.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_inspector.type_defs import (
     AttributeTypeDef,
     FailedItemDetailsTypeDef,
-    ResponseMetadataTypeDef,
     AgentFilterTypeDef,
     AgentPreviewTypeDef,
     TelemetryMetadataTypeDef,
     DurationRangeTypeDef,
     TimestampRangeTypeDef,
     AssessmentRunNotificationTypeDef,
     AssessmentRunStateChangeTypeDef,
     AssessmentTargetFilterTypeDef,
     AssessmentTargetTypeDef,
     TagTypeDef,
     CreateAssessmentTargetRequestRequestTypeDef,
+    CreateAssessmentTargetResponseTypeDef,
+    CreateAssessmentTemplateResponseTypeDef,
     CreateExclusionsPreviewRequestRequestTypeDef,
+    CreateExclusionsPreviewResponseTypeDef,
     ResourceGroupTagTypeDef,
+    CreateResourceGroupResponseTypeDef,
     DeleteAssessmentRunRequestRequestTypeDef,
     DeleteAssessmentTargetRequestRequestTypeDef,
     DeleteAssessmentTemplateRequestRequestTypeDef,
     DescribeAssessmentRunsRequestRequestTypeDef,
     DescribeAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTemplatesRequestRequestTypeDef,
+    DescribeCrossAccountAccessRoleResponseTypeDef,
     DescribeExclusionsRequestRequestTypeDef,
     DescribeFindingsRequestRequestTypeDef,
     DescribeResourceGroupsRequestRequestTypeDef,
     DescribeRulesPackagesRequestRequestTypeDef,
     RulesPackageTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventSubscriptionTypeDef,
     ScopeTypeDef,
     InspectorServiceAttributesTypeDef,
     GetAssessmentReportRequestRequestTypeDef,
+    GetAssessmentReportResponseTypeDef,
     GetExclusionsPreviewRequestRequestTypeDef,
     GetTelemetryMetadataRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssessmentRunsResponseTypeDef,
+    ListAssessmentTargetsResponseTypeDef,
+    ListAssessmentTemplatesResponseTypeDef,
+    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
     ListEventSubscriptionsRequestRequestTypeDef,
+    ListExclusionsRequestListExclusionsPaginateTypeDef,
     ListExclusionsRequestRequestTypeDef,
+    ListExclusionsResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
     ListRulesPackagesRequestRequestTypeDef,
+    ListRulesPackagesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PrivateIpTypeDef,
     SecurityGroupTypeDef,
+    PaginatorConfigTypeDef,
+    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     PreviewAgentsRequestRequestTypeDef,
     RegisterCrossAccountAccessRoleRequestRequestTypeDef,
     RemoveAttributesFromFindingsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     StartAssessmentRunRequestRequestTypeDef,
+    StartAssessmentRunResponseTypeDef,
     StopAssessmentRunRequestRequestTypeDef,
     SubscribeToEventRequestRequestTypeDef,
     UnsubscribeFromEventRequestRequestTypeDef,
     UpdateAssessmentTargetRequestRequestTypeDef,
     AddAttributesToFindingsRequestRequestTypeDef,
     AssessmentTemplateTypeDef,
     CreateAssessmentTemplateRequestRequestTypeDef,
     AddAttributesToFindingsResponseTypeDef,
-    CreateAssessmentTargetResponseTypeDef,
-    CreateAssessmentTemplateResponseTypeDef,
-    CreateExclusionsPreviewResponseTypeDef,
-    CreateResourceGroupResponseTypeDef,
-    DescribeCrossAccountAccessRoleResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAssessmentReportResponseTypeDef,
-    ListAssessmentRunsResponseTypeDef,
-    ListAssessmentTargetsResponseTypeDef,
-    ListAssessmentTemplatesResponseTypeDef,
-    ListExclusionsResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListRulesPackagesResponseTypeDef,
     RemoveAttributesFromFindingsResponseTypeDef,
-    StartAssessmentRunResponseTypeDef,
+    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
     ListAssessmentRunAgentsRequestRequestTypeDef,
     PreviewAgentsResponseTypeDef,
     AssessmentRunAgentTypeDef,
     GetTelemetryMetadataResponseTypeDef,
     AssessmentTemplateFilterTypeDef,
     AssessmentRunFilterTypeDef,
     FindingFilterTypeDef,
     AssessmentRunTypeDef,
+    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
     ListAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTargetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SetTagsForResourceRequestRequestTypeDef,
     CreateResourceGroupRequestRequestTypeDef,
     ResourceGroupTypeDef,
     DescribeRulesPackagesResponseTypeDef,
     SubscriptionTypeDef,
     ExclusionPreviewTypeDef,
     ExclusionTypeDef,
-    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
-    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
-    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
-    ListExclusionsRequestListExclusionsPaginateTypeDef,
-    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
-    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     NetworkInterfaceTypeDef,
     DescribeAssessmentTemplatesResponseTypeDef,
     ListAssessmentRunAgentsResponseTypeDef,
     ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef,
     ListAssessmentTemplatesRequestRequestTypeDef,
     ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
     ListAssessmentRunsRequestRequestTypeDef,
@@ -492,42 +493,42 @@
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

### Comparing `mypy-boto3-inspector-1.26.0.post1/mypy_boto3_inspector.egg-info/SOURCES.txt` & `mypy-boto3-inspector-1.27.0/mypy_boto3_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.26.0.post1/setup.py` & `mypy-boto3-inspector-1.27.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-inspector.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-inspector",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_inspector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Inspector 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.Inspector 1.27.0 service generated with mypy-boto3-builder"
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
     keywords="boto3 inspector type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_inspector": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_inspector": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/",
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


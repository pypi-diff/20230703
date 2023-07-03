# Comparing `tmp/mypy-boto3-resiliencehub-1.26.97.tar.gz` & `tmp/mypy-boto3-resiliencehub-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resiliencehub-1.26.97.tar", last modified: Wed Mar 22 19:32:31 2023, max compression
+gzip compressed data, was "mypy-boto3-resiliencehub-1.27.0.tar", last modified: Mon Jul  3 19:51:19 2023, max compression
```

## Comparing `mypy-boto3-resiliencehub-1.26.97.tar` & `mypy-boto3-resiliencehub-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.373775 mypy-boto3-resiliencehub-1.26.97/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-03-22 19:32:31.369775 mypy-boto3-resiliencehub-1.26.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17200 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.365775 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39566 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39508 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-03-22 19:32:12.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-03-22 19:32:12.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60670 2023-03-22 19:32:13.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60565 2023-03-22 19:32:12.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.369775 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-03-22 19:32:31.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-22 19:32:31.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:32:31.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:32:31.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-22 19:32:31.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-22 19:32:31.000000 mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 19:32:31.373775 mypy-boto3-resiliencehub-1.26.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-03-22 19:32:11.000000 mypy-boto3-resiliencehub-1.26.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.779879 mypy-boto3-resiliencehub-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:15.000000 mypy-boto3-resiliencehub-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18723 2023-07-03 19:51:19.779879 mypy-boto3-resiliencehub-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-07-03 19:46:15.000000 mypy-boto3-resiliencehub-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.779879 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-03 19:46:15.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-03 19:46:15.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 19:46:15.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39572 2023-07-03 19:46:15.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39514 2023-07-03 19:46:15.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-07-03 19:46:15.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-07-03 19:46:15.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:15.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60883 2023-07-03 19:46:17.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60778 2023-07-03 19:46:16.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:15.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:19.779879 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18723 2023-07-03 19:51:19.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-03 19:51:19.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:19.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:19.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:19.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 19:51:19.000000 mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:19.779879 mypy-boto3-resiliencehub-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-03 19:46:15.000000 mypy-boto3-resiliencehub-1.27.0/setup.py
```

### Comparing `mypy-boto3-resiliencehub-1.26.97/LICENSE` & `mypy-boto3-resiliencehub-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-resiliencehub-1.26.97/PKG-INFO` & `mypy-boto3-resiliencehub-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resiliencehub
-Version: 1.26.97
-Summary: Type annotations for boto3.ResilienceHub 1.26.97 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.ResilienceHub 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-resiliencehub"></a>
 
 # mypy-boto3-resiliencehub
 
 [![PyPI - mypy-boto3-resiliencehub](https://img.shields.io/pypi/v/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resiliencehub?color=blue)](https://pypistats.org/packages/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,14 +298,15 @@
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStatusTypeType,
     ResourceImportStrategyTypeType,
     ResourceMappingTypeType,
     ResourceResolutionStatusTypeType,
+    ResourceSourceTypeType,
     SopServiceTypeType,
     TemplateFormatType,
     TestRiskType,
     TestTypeType,
     ResilienceHubServiceName,
     ServiceName,
     ResourceServiceName,
@@ -322,15 +323,14 @@
 ### Typed dictionaries
 
 `mypy_boto3_resiliencehub.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resiliencehub.type_defs import (
-    ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
     EksSourceClusterNamespaceTypeDef,
     TerraformSourceTypeDef,
@@ -340,25 +340,33 @@
     RecommendationDisruptionComplianceTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
     LogicalResourceIdTypeDef,
     CreateRecommendationTemplateRequestRequestTypeDef,
     FailurePolicyTypeDef,
     DeleteAppAssessmentRequestRequestTypeDef,
+    DeleteAppAssessmentResponseTypeDef,
     DeleteAppRequestRequestTypeDef,
+    DeleteAppResponseTypeDef,
     DeleteAppVersionAppComponentRequestRequestTypeDef,
     DeleteRecommendationTemplateRequestRequestTypeDef,
+    DeleteRecommendationTemplateResponseTypeDef,
     DeleteResiliencyPolicyRequestRequestTypeDef,
+    DeleteResiliencyPolicyResponseTypeDef,
     DescribeAppAssessmentRequestRequestTypeDef,
     DescribeAppRequestRequestTypeDef,
     DescribeAppVersionAppComponentRequestRequestTypeDef,
     DescribeAppVersionRequestRequestTypeDef,
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
+    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
+    DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
+    DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
+    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
     EksSourceTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
@@ -368,42 +376,35 @@
     ListAppVersionsRequestRequestTypeDef,
     ListAppsRequestRequestTypeDef,
     ListRecommendationTemplatesRequestRequestTypeDef,
     ListResiliencyPoliciesRequestRequestTypeDef,
     ListSopRecommendationsRequestRequestTypeDef,
     ListSuggestedResiliencyPoliciesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsRequestRequestTypeDef,
     ListUnsupportedAppVersionResourcesRequestRequestTypeDef,
     PhysicalResourceIdTypeDef,
     PublishAppVersionRequestRequestTypeDef,
+    PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateRequestRequestTypeDef,
+    PutDraftAppVersionTemplateResponseTypeDef,
     S3LocationTypeDef,
     RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
+    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesRequestRequestTypeDef,
+    ResolveAppVersionResourcesResponseTypeDef,
     ResourceErrorTypeDef,
+    ResponseMetadataTypeDef,
     StartAppAssessmentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     UpdateAppVersionAppComponentRequestRequestTypeDef,
     UpdateAppVersionRequestRequestTypeDef,
-    DeleteAppAssessmentResponseTypeDef,
-    DeleteAppResponseTypeDef,
-    DeleteRecommendationTemplateResponseTypeDef,
-    DeleteResiliencyPolicyResponseTypeDef,
-    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
-    DescribeAppVersionResponseTypeDef,
-    DescribeAppVersionTemplateResponseTypeDef,
-    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PublishAppVersionResponseTypeDef,
-    PutDraftAppVersionTemplateResponseTypeDef,
-    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
-    ResolveAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
     AlarmRecommendationTypeDef,
     SopRecommendationTypeDef,
     TestRecommendationTypeDef,
     AppAssessmentSummaryTypeDef,
     AppComponentComplianceTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
@@ -460,53 +461,53 @@
     AppAssessmentTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     DescribeAppAssessmentResponseTypeDef,
     StartAppAssessmentResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> RecommendationItemTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-resiliencehub-1.26.97/README.md` & `mypy-boto3-resiliencehub-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-resiliencehub"></a>
 
 # mypy-boto3-resiliencehub
 
 [![PyPI - mypy-boto3-resiliencehub](https://img.shields.io/pypi/v/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resiliencehub?color=blue)](https://pypistats.org/packages/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,14 +266,15 @@
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStatusTypeType,
     ResourceImportStrategyTypeType,
     ResourceMappingTypeType,
     ResourceResolutionStatusTypeType,
+    ResourceSourceTypeType,
     SopServiceTypeType,
     TemplateFormatType,
     TestRiskType,
     TestTypeType,
     ResilienceHubServiceName,
     ServiceName,
     ResourceServiceName,
@@ -290,15 +291,14 @@
 ### Typed dictionaries
 
 `mypy_boto3_resiliencehub.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resiliencehub.type_defs import (
-    ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
     EksSourceClusterNamespaceTypeDef,
     TerraformSourceTypeDef,
@@ -308,25 +308,33 @@
     RecommendationDisruptionComplianceTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
     LogicalResourceIdTypeDef,
     CreateRecommendationTemplateRequestRequestTypeDef,
     FailurePolicyTypeDef,
     DeleteAppAssessmentRequestRequestTypeDef,
+    DeleteAppAssessmentResponseTypeDef,
     DeleteAppRequestRequestTypeDef,
+    DeleteAppResponseTypeDef,
     DeleteAppVersionAppComponentRequestRequestTypeDef,
     DeleteRecommendationTemplateRequestRequestTypeDef,
+    DeleteRecommendationTemplateResponseTypeDef,
     DeleteResiliencyPolicyRequestRequestTypeDef,
+    DeleteResiliencyPolicyResponseTypeDef,
     DescribeAppAssessmentRequestRequestTypeDef,
     DescribeAppRequestRequestTypeDef,
     DescribeAppVersionAppComponentRequestRequestTypeDef,
     DescribeAppVersionRequestRequestTypeDef,
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
+    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
+    DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
+    DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
+    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
     EksSourceTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
@@ -336,42 +344,35 @@
     ListAppVersionsRequestRequestTypeDef,
     ListAppsRequestRequestTypeDef,
     ListRecommendationTemplatesRequestRequestTypeDef,
     ListResiliencyPoliciesRequestRequestTypeDef,
     ListSopRecommendationsRequestRequestTypeDef,
     ListSuggestedResiliencyPoliciesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsRequestRequestTypeDef,
     ListUnsupportedAppVersionResourcesRequestRequestTypeDef,
     PhysicalResourceIdTypeDef,
     PublishAppVersionRequestRequestTypeDef,
+    PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateRequestRequestTypeDef,
+    PutDraftAppVersionTemplateResponseTypeDef,
     S3LocationTypeDef,
     RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
+    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesRequestRequestTypeDef,
+    ResolveAppVersionResourcesResponseTypeDef,
     ResourceErrorTypeDef,
+    ResponseMetadataTypeDef,
     StartAppAssessmentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     UpdateAppVersionAppComponentRequestRequestTypeDef,
     UpdateAppVersionRequestRequestTypeDef,
-    DeleteAppAssessmentResponseTypeDef,
-    DeleteAppResponseTypeDef,
-    DeleteRecommendationTemplateResponseTypeDef,
-    DeleteResiliencyPolicyResponseTypeDef,
-    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
-    DescribeAppVersionResponseTypeDef,
-    DescribeAppVersionTemplateResponseTypeDef,
-    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PublishAppVersionResponseTypeDef,
-    PutDraftAppVersionTemplateResponseTypeDef,
-    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
-    ResolveAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
     AlarmRecommendationTypeDef,
     SopRecommendationTypeDef,
     TestRecommendationTypeDef,
     AppAssessmentSummaryTypeDef,
     AppComponentComplianceTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
@@ -428,53 +429,53 @@
     AppAssessmentTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     DescribeAppAssessmentResponseTypeDef,
     StartAppAssessmentResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> RecommendationItemTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/__main__.py` & `mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResilienceHub 1.26.97\nVersion:         1.26.97\nBuilder"
-        " version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.ResilienceHub 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub\nOther"
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

### Comparing `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/client.py` & `mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,20 +191,20 @@
     def create_app_version_resource(
         self,
         *,
         appArn: str,
         appComponents: Sequence[str],
         logicalResourceId: LogicalResourceIdTypeDef,
         physicalResourceId: str,
-        resourceName: str,
         resourceType: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         awsAccountId: str = ...,
         awsRegion: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
+        resourceName: str = ...
     ) -> CreateAppVersionResourceResponseTypeDef:
         """
         Adds a resource to the Resilience Hub application and assigns it to the
         specified Application Components.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_app_version_resource)
```

### Comparing `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/client.pyi` & `mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -182,20 +182,20 @@
     def create_app_version_resource(
         self,
         *,
         appArn: str,
         appComponents: Sequence[str],
         logicalResourceId: LogicalResourceIdTypeDef,
         physicalResourceId: str,
-        resourceName: str,
         resourceType: str,
         additionalInfo: Mapping[str, Sequence[str]] = ...,
         awsAccountId: str = ...,
         awsRegion: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
+        resourceName: str = ...
     ) -> CreateAppVersionResourceResponseTypeDef:
         """
         Adds a resource to the Resilience Hub application and assigns it to the
         specified Application Components.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app_version_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#create_app_version_resource)
```

### Comparing `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/literals.py` & `mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     "RecommendationTemplateStatusType",
     "RenderRecommendationTypeType",
     "ResiliencyPolicyTierType",
     "ResourceImportStatusTypeType",
     "ResourceImportStrategyTypeType",
     "ResourceMappingTypeType",
     "ResourceResolutionStatusTypeType",
+    "ResourceSourceTypeType",
     "SopServiceTypeType",
     "TemplateFormatType",
     "TestRiskType",
     "TestTypeType",
     "ResilienceHubServiceName",
     "ServiceName",
     "ResourceServiceName",
@@ -88,14 +89,15 @@
 ]
 ResourceImportStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
 ResourceImportStrategyTypeType = Literal["AddOnly", "ReplaceAll"]
 ResourceMappingTypeType = Literal[
     "AppRegistryApp", "CfnStack", "EKS", "Resource", "ResourceGroup", "Terraform"
 ]
 ResourceResolutionStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
+ResourceSourceTypeType = Literal["AppTemplate", "Discovered"]
 SopServiceTypeType = Literal["SSM"]
 TemplateFormatType = Literal["CfnJson", "CfnYaml"]
 TestRiskType = Literal["High", "Medium", "Small"]
 TestTypeType = Literal["AZ", "Hardware", "Region", "Software"]
 ResilienceHubServiceName = Literal["resiliencehub"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -108,14 +110,15 @@
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
@@ -155,14 +158,15 @@
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
@@ -260,14 +264,15 @@
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
@@ -303,14 +308,15 @@
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
@@ -329,16 +335,19 @@
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
@@ -422,15 +431,17 @@
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

### Comparing `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/literals.pyi` & `mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     "RecommendationTemplateStatusType",
     "RenderRecommendationTypeType",
     "ResiliencyPolicyTierType",
     "ResourceImportStatusTypeType",
     "ResourceImportStrategyTypeType",
     "ResourceMappingTypeType",
     "ResourceResolutionStatusTypeType",
+    "ResourceSourceTypeType",
     "SopServiceTypeType",
     "TemplateFormatType",
     "TestRiskType",
     "TestTypeType",
     "ResilienceHubServiceName",
     "ServiceName",
     "ResourceServiceName",
@@ -86,14 +87,15 @@
 ]
 ResourceImportStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
 ResourceImportStrategyTypeType = Literal["AddOnly", "ReplaceAll"]
 ResourceMappingTypeType = Literal[
     "AppRegistryApp", "CfnStack", "EKS", "Resource", "ResourceGroup", "Terraform"
 ]
 ResourceResolutionStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
+ResourceSourceTypeType = Literal["AppTemplate", "Discovered"]
 SopServiceTypeType = Literal["SSM"]
 TemplateFormatType = Literal["CfnJson", "CfnYaml"]
 TestRiskType = Literal["High", "Medium", "Small"]
 TestTypeType = Literal["AZ", "Hardware", "Region", "Software"]
 ResilienceHubServiceName = Literal["resiliencehub"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -106,14 +108,15 @@
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
@@ -153,14 +156,15 @@
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
@@ -258,14 +262,15 @@
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
@@ -301,14 +306,15 @@
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
@@ -327,16 +333,19 @@
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
@@ -420,15 +429,17 @@
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

### Comparing `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/type_defs.py` & `mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for resiliencehub service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_resiliencehub.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_resiliencehub.type_defs import RecommendationItemTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: RecommendationItemTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -34,14 +34,15 @@
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStatusTypeType,
     ResourceImportStrategyTypeType,
     ResourceMappingTypeType,
     ResourceResolutionStatusTypeType,
+    ResourceSourceTypeType,
     TemplateFormatType,
     TestRiskType,
     TestTypeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -50,15 +51,14 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ResponseMetadataTypeDef",
     "RecommendationItemTypeDef",
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
     "EksSourceClusterNamespaceTypeDef",
     "TerraformSourceTypeDef",
@@ -68,25 +68,33 @@
     "RecommendationDisruptionComplianceTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
+    "DeleteAppAssessmentResponseTypeDef",
     "DeleteAppRequestRequestTypeDef",
+    "DeleteAppResponseTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
     "DeleteRecommendationTemplateRequestRequestTypeDef",
+    "DeleteRecommendationTemplateResponseTypeDef",
     "DeleteResiliencyPolicyRequestRequestTypeDef",
+    "DeleteResiliencyPolicyResponseTypeDef",
     "DescribeAppAssessmentRequestRequestTypeDef",
     "DescribeAppRequestRequestTypeDef",
     "DescribeAppVersionAppComponentRequestRequestTypeDef",
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
+    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
+    "DescribeAppVersionResponseTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
+    "DescribeAppVersionTemplateResponseTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
+    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     "EksSourceTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
@@ -96,42 +104,35 @@
     "ListAppVersionsRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "ListRecommendationTemplatesRequestRequestTypeDef",
     "ListResiliencyPoliciesRequestRequestTypeDef",
     "ListSopRecommendationsRequestRequestTypeDef",
     "ListSuggestedResiliencyPoliciesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTestRecommendationsRequestRequestTypeDef",
     "ListUnsupportedAppVersionResourcesRequestRequestTypeDef",
     "PhysicalResourceIdTypeDef",
     "PublishAppVersionRequestRequestTypeDef",
+    "PublishAppVersionResponseTypeDef",
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
+    "PutDraftAppVersionTemplateResponseTypeDef",
     "S3LocationTypeDef",
     "RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
+    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
     "ResolveAppVersionResourcesRequestRequestTypeDef",
+    "ResolveAppVersionResourcesResponseTypeDef",
     "ResourceErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "StartAppAssessmentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "UpdateAppVersionAppComponentRequestRequestTypeDef",
     "UpdateAppVersionRequestRequestTypeDef",
-    "DeleteAppAssessmentResponseTypeDef",
-    "DeleteAppResponseTypeDef",
-    "DeleteRecommendationTemplateResponseTypeDef",
-    "DeleteResiliencyPolicyResponseTypeDef",
-    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
-    "DescribeAppVersionResponseTypeDef",
-    "DescribeAppVersionTemplateResponseTypeDef",
-    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PublishAppVersionResponseTypeDef",
-    "PutDraftAppVersionTemplateResponseTypeDef",
-    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
-    "ResolveAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResponseTypeDef",
     "AlarmRecommendationTypeDef",
     "SopRecommendationTypeDef",
     "TestRecommendationTypeDef",
     "AppAssessmentSummaryTypeDef",
     "AppComponentComplianceTypeDef",
     "CreateAppVersionAppComponentResponseTypeDef",
@@ -187,25 +188,14 @@
     "ListRecommendationTemplatesResponseTypeDef",
     "AppAssessmentTypeDef",
     "ListAppComponentRecommendationsResponseTypeDef",
     "DescribeAppAssessmentResponseTypeDef",
     "StartAppAssessmentResponseTypeDef",
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
 RecommendationItemTypeDef = TypedDict(
     "RecommendationItemTypeDef",
     {
         "alreadyImplemented": bool,
         "resourceId": str,
         "targetAccountId": str,
         "targetRegion": str,
@@ -510,14 +500,23 @@
 class DeleteAppAssessmentRequestRequestTypeDef(
     _RequiredDeleteAppAssessmentRequestRequestTypeDef,
     _OptionalDeleteAppAssessmentRequestRequestTypeDef,
 ):
     pass
 
 
+DeleteAppAssessmentResponseTypeDef = TypedDict(
+    "DeleteAppAssessmentResponseTypeDef",
+    {
+        "assessmentArn": str,
+        "assessmentStatus": AssessmentStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteAppRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAppRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 _OptionalDeleteAppRequestRequestTypeDef = TypedDict(
@@ -532,14 +531,22 @@
 
 class DeleteAppRequestRequestTypeDef(
     _RequiredDeleteAppRequestRequestTypeDef, _OptionalDeleteAppRequestRequestTypeDef
 ):
     pass
 
 
+DeleteAppResponseTypeDef = TypedDict(
+    "DeleteAppResponseTypeDef",
+    {
+        "appArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "id": str,
     },
 )
@@ -577,14 +584,23 @@
 class DeleteRecommendationTemplateRequestRequestTypeDef(
     _RequiredDeleteRecommendationTemplateRequestRequestTypeDef,
     _OptionalDeleteRecommendationTemplateRequestRequestTypeDef,
 ):
     pass
 
 
+DeleteRecommendationTemplateResponseTypeDef = TypedDict(
+    "DeleteRecommendationTemplateResponseTypeDef",
+    {
+        "recommendationTemplateArn": str,
+        "status": RecommendationTemplateStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 _OptionalDeleteResiliencyPolicyRequestRequestTypeDef = TypedDict(
@@ -599,14 +615,22 @@
 class DeleteResiliencyPolicyRequestRequestTypeDef(
     _RequiredDeleteResiliencyPolicyRequestRequestTypeDef,
     _OptionalDeleteResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
 
+DeleteResiliencyPolicyResponseTypeDef = TypedDict(
+    "DeleteResiliencyPolicyResponseTypeDef",
+    {
+        "policyArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeAppAssessmentRequestRequestTypeDef = TypedDict(
     "DescribeAppAssessmentRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 
@@ -653,29 +677,73 @@
 class DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef(
     _RequiredDescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
     _OptionalDescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
 ):
     pass
 
 
+DescribeAppVersionResourcesResolutionStatusResponseTypeDef = TypedDict(
+    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "errorMessage": str,
+        "resolutionId": str,
+        "status": ResourceResolutionStatusTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAppVersionResponseTypeDef = TypedDict(
+    "DescribeAppVersionResponseTypeDef",
+    {
+        "additionalInfo": Dict[str, List[str]],
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
     },
 )
 
+DescribeAppVersionTemplateResponseTypeDef = TypedDict(
+    "DescribeAppVersionTemplateResponseTypeDef",
+    {
+        "appArn": str,
+        "appTemplateBody": str,
+        "appVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef = TypedDict(
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 
+DescribeDraftAppVersionResourcesImportStatusResponseTypeDef = TypedDict(
+    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "errorMessage": str,
+        "status": ResourceImportStatusTypeType,
+        "statusChangeTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 
@@ -973,14 +1041,22 @@
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
 _RequiredListTestRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListTestRecommendationsRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 _OptionalListTestRecommendationsRequestRequestTypeDef = TypedDict(
@@ -1051,22 +1127,40 @@
 PublishAppVersionRequestRequestTypeDef = TypedDict(
     "PublishAppVersionRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 
+PublishAppVersionResponseTypeDef = TypedDict(
+    "PublishAppVersionResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutDraftAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appTemplateBody": str,
     },
 )
 
+PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
+    "PutDraftAppVersionTemplateResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
@@ -1095,32 +1189,63 @@
 class RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef(
     _RequiredRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
     _OptionalRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
 ):
     pass
 
 
+RemoveDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
+    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ResolveAppVersionResourcesRequestRequestTypeDef = TypedDict(
     "ResolveAppVersionResourcesRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
     },
 )
 
+ResolveAppVersionResourcesResponseTypeDef = TypedDict(
+    "ResolveAppVersionResourcesResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "resolutionId": str,
+        "status": ResourceResolutionStatusTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ResourceErrorTypeDef = TypedDict(
     "ResourceErrorTypeDef",
     {
         "logicalResourceId": str,
         "physicalResourceId": str,
         "reason": str,
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
 _RequiredStartAppAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredStartAppAssessmentRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
     },
@@ -1224,145 +1349,21 @@
 
 class UpdateAppVersionRequestRequestTypeDef(
     _RequiredUpdateAppVersionRequestRequestTypeDef, _OptionalUpdateAppVersionRequestRequestTypeDef
 ):
     pass
 
 
-DeleteAppAssessmentResponseTypeDef = TypedDict(
-    "DeleteAppAssessmentResponseTypeDef",
-    {
-        "assessmentArn": str,
-        "assessmentStatus": AssessmentStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteAppResponseTypeDef = TypedDict(
-    "DeleteAppResponseTypeDef",
-    {
-        "appArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteRecommendationTemplateResponseTypeDef = TypedDict(
-    "DeleteRecommendationTemplateResponseTypeDef",
-    {
-        "recommendationTemplateArn": str,
-        "status": RecommendationTemplateStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteResiliencyPolicyResponseTypeDef = TypedDict(
-    "DeleteResiliencyPolicyResponseTypeDef",
-    {
-        "policyArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAppVersionResourcesResolutionStatusResponseTypeDef = TypedDict(
-    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "errorMessage": str,
-        "resolutionId": str,
-        "status": ResourceResolutionStatusTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAppVersionResponseTypeDef = TypedDict(
-    "DescribeAppVersionResponseTypeDef",
-    {
-        "additionalInfo": Dict[str, List[str]],
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAppVersionTemplateResponseTypeDef = TypedDict(
-    "DescribeAppVersionTemplateResponseTypeDef",
-    {
-        "appArn": str,
-        "appTemplateBody": str,
-        "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDraftAppVersionResourcesImportStatusResponseTypeDef = TypedDict(
-    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "errorMessage": str,
-        "status": ResourceImportStatusTypeType,
-        "statusChangeTime": datetime,
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
-PublishAppVersionResponseTypeDef = TypedDict(
-    "PublishAppVersionResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
-    "PutDraftAppVersionTemplateResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
-    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ResolveAppVersionResourcesResponseTypeDef = TypedDict(
-    "ResolveAppVersionResourcesResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "resolutionId": str,
-        "status": ResourceResolutionStatusTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateAppVersionResponseTypeDef = TypedDict(
     "UpdateAppVersionResponseTypeDef",
     {
         "additionalInfo": Dict[str, List[str]],
         "appArn": str,
         "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAlarmRecommendationTypeDef = TypedDict(
     "_RequiredAlarmRecommendationTypeDef",
     {
         "name": str,
@@ -1492,56 +1493,56 @@
 
 CreateAppVersionAppComponentResponseTypeDef = TypedDict(
     "CreateAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAppVersionAppComponentResponseTypeDef = TypedDict(
     "DeleteAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppVersionAppComponentResponseTypeDef = TypedDict(
     "DescribeAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppVersionAppComponentsResponseTypeDef = TypedDict(
     "ListAppVersionAppComponentsResponseTypeDef",
     {
         "appArn": str,
         "appComponents": List[AppComponentTypeDef],
         "appVersion": str,
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAppVersionAppComponentResponseTypeDef = TypedDict(
     "UpdateAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAppInputSourceTypeDef = TypedDict(
     "_RequiredAppInputSourceTypeDef",
     {
         "importType": ResourceMappingTypeType,
@@ -1590,48 +1591,48 @@
 
 
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAppResponseTypeDef = TypedDict(
     "CreateAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppResponseTypeDef = TypedDict(
     "DescribeAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAppResponseTypeDef = TypedDict(
     "UpdateAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppVersionsResponseTypeDef = TypedDict(
     "ListAppVersionsResponseTypeDef",
     {
         "appVersions": List[AppVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredConfigRecommendationTypeDef = TypedDict(
     "_RequiredConfigRecommendationTypeDef",
     {
         "name": str,
@@ -1665,25 +1666,25 @@
 _RequiredCreateAppVersionResourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppVersionResourceRequestRequestTypeDef",
     {
         "appArn": str,
         "appComponents": Sequence[str],
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": str,
-        "resourceName": str,
         "resourceType": str,
     },
 )
 _OptionalCreateAppVersionResourceRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAppVersionResourceRequestRequestTypeDef",
     {
         "additionalInfo": Mapping[str, Sequence[str]],
         "awsAccountId": str,
         "awsRegion": str,
         "clientToken": str,
+        "resourceName": str,
     },
     total=False,
 )
 
 
 class CreateAppVersionResourceRequestRequestTypeDef(
     _RequiredCreateAppVersionResourceRequestRequestTypeDef,
@@ -1875,15 +1876,15 @@
     {
         "appArn": str,
         "appVersion": str,
         "eksSources": List[EksSourceTypeDef],
         "sourceArns": List[str],
         "status": ResourceImportStatusTypeType,
         "terraformSources": List[TerraformSourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
@@ -1893,15 +1894,17 @@
 )
 _OptionalPhysicalResourceTypeDef = TypedDict(
     "_OptionalPhysicalResourceTypeDef",
     {
         "additionalInfo": Dict[str, List[str]],
         "appComponents": List[AppComponentTypeDef],
         "excluded": bool,
+        "parentResourceName": str,
         "resourceName": str,
+        "sourceType": ResourceSourceTypeType,
     },
     total=False,
 )
 
 
 class PhysicalResourceTypeDef(_RequiredPhysicalResourceTypeDef, _OptionalPhysicalResourceTypeDef):
     pass
@@ -1998,69 +2001,69 @@
 )
 
 ListAlarmRecommendationsResponseTypeDef = TypedDict(
     "ListAlarmRecommendationsResponseTypeDef",
     {
         "alarmRecommendations": List[AlarmRecommendationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSopRecommendationsResponseTypeDef = TypedDict(
     "ListSopRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "sopRecommendations": List[SopRecommendationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTestRecommendationsResponseTypeDef = TypedDict(
     "ListTestRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "testRecommendations": List[TestRecommendationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppAssessmentsResponseTypeDef = TypedDict(
     "ListAppAssessmentsResponseTypeDef",
     {
         "assessmentSummaries": List[AppAssessmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppComponentCompliancesResponseTypeDef = TypedDict(
     "ListAppComponentCompliancesResponseTypeDef",
     {
         "componentCompliances": List[AppComponentComplianceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAppInputSourceResponseTypeDef = TypedDict(
     "DeleteAppInputSourceResponseTypeDef",
     {
         "appArn": str,
         "appInputSource": AppInputSourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppInputSourcesResponseTypeDef = TypedDict(
     "ListAppInputSourcesResponseTypeDef",
     {
         "appInputSources": List[AppInputSourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ComponentRecommendationTypeDef = TypedDict(
     "ComponentRecommendationTypeDef",
     {
         "appComponentName": str,
@@ -2069,99 +2072,99 @@
     },
 )
 
 CreateResiliencyPolicyResponseTypeDef = TypedDict(
     "CreateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeResiliencyPolicyResponseTypeDef = TypedDict(
     "DescribeResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResiliencyPoliciesResponseTypeDef = TypedDict(
     "ListResiliencyPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "resiliencyPolicies": List[ResiliencyPolicyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSuggestedResiliencyPoliciesResponseTypeDef = TypedDict(
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "resiliencyPolicies": List[ResiliencyPolicyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateResiliencyPolicyResponseTypeDef = TypedDict(
     "UpdateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAppVersionResourceResponseTypeDef = TypedDict(
     "CreateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAppVersionResourceResponseTypeDef = TypedDict(
     "DeleteAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppVersionResourceResponseTypeDef = TypedDict(
     "DescribeAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppVersionResourcesResponseTypeDef = TypedDict(
     "ListAppVersionResourcesResponseTypeDef",
     {
         "nextToken": str,
         "physicalResources": List[PhysicalResourceTypeDef],
         "resolutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAppVersionResourceResponseTypeDef = TypedDict(
     "UpdateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddDraftAppVersionResourceMappingsRequestRequestTypeDef = TypedDict(
     "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     {
         "appArn": str,
@@ -2171,51 +2174,51 @@
 
 AddDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "resourceMappings": List[ResourceMappingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "ListAppVersionResourceMappingsResponseTypeDef",
     {
         "nextToken": str,
         "resourceMappings": List[ResourceMappingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUnsupportedAppVersionResourcesResponseTypeDef = TypedDict(
     "ListUnsupportedAppVersionResourcesResponseTypeDef",
     {
         "nextToken": str,
         "resolutionId": str,
         "unsupportedResources": List[UnsupportedResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRecommendationTemplateResponseTypeDef = TypedDict(
     "CreateRecommendationTemplateResponseTypeDef",
     {
         "recommendationTemplate": RecommendationTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecommendationTemplatesResponseTypeDef = TypedDict(
     "ListRecommendationTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationTemplates": List[RecommendationTemplateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAppAssessmentTypeDef = TypedDict(
     "_RequiredAppAssessmentTypeDef",
     {
         "assessmentArn": str,
@@ -2249,26 +2252,26 @@
 
 
 ListAppComponentRecommendationsResponseTypeDef = TypedDict(
     "ListAppComponentRecommendationsResponseTypeDef",
     {
         "componentRecommendations": List[ComponentRecommendationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppAssessmentResponseTypeDef = TypedDict(
     "DescribeAppAssessmentResponseTypeDef",
     {
         "assessment": AppAssessmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartAppAssessmentResponseTypeDef = TypedDict(
     "StartAppAssessmentResponseTypeDef",
     {
         "assessment": AppAssessmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub/type_defs.pyi` & `mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for resiliencehub service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_resiliencehub.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_resiliencehub.type_defs import RecommendationItemTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: RecommendationItemTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -34,14 +34,15 @@
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStatusTypeType,
     ResourceImportStrategyTypeType,
     ResourceMappingTypeType,
     ResourceResolutionStatusTypeType,
+    ResourceSourceTypeType,
     TemplateFormatType,
     TestRiskType,
     TestTypeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -49,15 +50,14 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ResponseMetadataTypeDef",
     "RecommendationItemTypeDef",
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
     "EksSourceClusterNamespaceTypeDef",
     "TerraformSourceTypeDef",
@@ -67,25 +67,33 @@
     "RecommendationDisruptionComplianceTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
+    "DeleteAppAssessmentResponseTypeDef",
     "DeleteAppRequestRequestTypeDef",
+    "DeleteAppResponseTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
     "DeleteRecommendationTemplateRequestRequestTypeDef",
+    "DeleteRecommendationTemplateResponseTypeDef",
     "DeleteResiliencyPolicyRequestRequestTypeDef",
+    "DeleteResiliencyPolicyResponseTypeDef",
     "DescribeAppAssessmentRequestRequestTypeDef",
     "DescribeAppRequestRequestTypeDef",
     "DescribeAppVersionAppComponentRequestRequestTypeDef",
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
+    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
+    "DescribeAppVersionResponseTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
+    "DescribeAppVersionTemplateResponseTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
+    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     "EksSourceTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
@@ -95,42 +103,35 @@
     "ListAppVersionsRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "ListRecommendationTemplatesRequestRequestTypeDef",
     "ListResiliencyPoliciesRequestRequestTypeDef",
     "ListSopRecommendationsRequestRequestTypeDef",
     "ListSuggestedResiliencyPoliciesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTestRecommendationsRequestRequestTypeDef",
     "ListUnsupportedAppVersionResourcesRequestRequestTypeDef",
     "PhysicalResourceIdTypeDef",
     "PublishAppVersionRequestRequestTypeDef",
+    "PublishAppVersionResponseTypeDef",
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
+    "PutDraftAppVersionTemplateResponseTypeDef",
     "S3LocationTypeDef",
     "RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
+    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
     "ResolveAppVersionResourcesRequestRequestTypeDef",
+    "ResolveAppVersionResourcesResponseTypeDef",
     "ResourceErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "StartAppAssessmentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "UpdateAppVersionAppComponentRequestRequestTypeDef",
     "UpdateAppVersionRequestRequestTypeDef",
-    "DeleteAppAssessmentResponseTypeDef",
-    "DeleteAppResponseTypeDef",
-    "DeleteRecommendationTemplateResponseTypeDef",
-    "DeleteResiliencyPolicyResponseTypeDef",
-    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
-    "DescribeAppVersionResponseTypeDef",
-    "DescribeAppVersionTemplateResponseTypeDef",
-    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PublishAppVersionResponseTypeDef",
-    "PutDraftAppVersionTemplateResponseTypeDef",
-    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
-    "ResolveAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResponseTypeDef",
     "AlarmRecommendationTypeDef",
     "SopRecommendationTypeDef",
     "TestRecommendationTypeDef",
     "AppAssessmentSummaryTypeDef",
     "AppComponentComplianceTypeDef",
     "CreateAppVersionAppComponentResponseTypeDef",
@@ -186,25 +187,14 @@
     "ListRecommendationTemplatesResponseTypeDef",
     "AppAssessmentTypeDef",
     "ListAppComponentRecommendationsResponseTypeDef",
     "DescribeAppAssessmentResponseTypeDef",
     "StartAppAssessmentResponseTypeDef",
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
 RecommendationItemTypeDef = TypedDict(
     "RecommendationItemTypeDef",
     {
         "alreadyImplemented": bool,
         "resourceId": str,
         "targetAccountId": str,
         "targetRegion": str,
@@ -489,14 +479,23 @@
 
 class DeleteAppAssessmentRequestRequestTypeDef(
     _RequiredDeleteAppAssessmentRequestRequestTypeDef,
     _OptionalDeleteAppAssessmentRequestRequestTypeDef,
 ):
     pass
 
+DeleteAppAssessmentResponseTypeDef = TypedDict(
+    "DeleteAppAssessmentResponseTypeDef",
+    {
+        "assessmentArn": str,
+        "assessmentStatus": AssessmentStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteAppRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAppRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 _OptionalDeleteAppRequestRequestTypeDef = TypedDict(
@@ -509,14 +508,22 @@
 )
 
 class DeleteAppRequestRequestTypeDef(
     _RequiredDeleteAppRequestRequestTypeDef, _OptionalDeleteAppRequestRequestTypeDef
 ):
     pass
 
+DeleteAppResponseTypeDef = TypedDict(
+    "DeleteAppResponseTypeDef",
+    {
+        "appArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "id": str,
     },
 )
@@ -550,14 +557,23 @@
 
 class DeleteRecommendationTemplateRequestRequestTypeDef(
     _RequiredDeleteRecommendationTemplateRequestRequestTypeDef,
     _OptionalDeleteRecommendationTemplateRequestRequestTypeDef,
 ):
     pass
 
+DeleteRecommendationTemplateResponseTypeDef = TypedDict(
+    "DeleteRecommendationTemplateResponseTypeDef",
+    {
+        "recommendationTemplateArn": str,
+        "status": RecommendationTemplateStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 _OptionalDeleteResiliencyPolicyRequestRequestTypeDef = TypedDict(
@@ -570,14 +586,22 @@
 
 class DeleteResiliencyPolicyRequestRequestTypeDef(
     _RequiredDeleteResiliencyPolicyRequestRequestTypeDef,
     _OptionalDeleteResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
+DeleteResiliencyPolicyResponseTypeDef = TypedDict(
+    "DeleteResiliencyPolicyResponseTypeDef",
+    {
+        "policyArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeAppAssessmentRequestRequestTypeDef = TypedDict(
     "DescribeAppAssessmentRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 
@@ -622,29 +646,73 @@
 
 class DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef(
     _RequiredDescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
     _OptionalDescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
 ):
     pass
 
+DescribeAppVersionResourcesResolutionStatusResponseTypeDef = TypedDict(
+    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "errorMessage": str,
+        "resolutionId": str,
+        "status": ResourceResolutionStatusTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAppVersionResponseTypeDef = TypedDict(
+    "DescribeAppVersionResponseTypeDef",
+    {
+        "additionalInfo": Dict[str, List[str]],
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
     },
 )
 
+DescribeAppVersionTemplateResponseTypeDef = TypedDict(
+    "DescribeAppVersionTemplateResponseTypeDef",
+    {
+        "appArn": str,
+        "appTemplateBody": str,
+        "appVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef = TypedDict(
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 
+DescribeDraftAppVersionResourcesImportStatusResponseTypeDef = TypedDict(
+    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "errorMessage": str,
+        "status": ResourceImportStatusTypeType,
+        "statusChangeTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 
@@ -922,14 +990,22 @@
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
 _RequiredListTestRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListTestRecommendationsRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 _OptionalListTestRecommendationsRequestRequestTypeDef = TypedDict(
@@ -994,22 +1070,40 @@
 PublishAppVersionRequestRequestTypeDef = TypedDict(
     "PublishAppVersionRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 
+PublishAppVersionResponseTypeDef = TypedDict(
+    "PublishAppVersionResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutDraftAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appTemplateBody": str,
     },
 )
 
+PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
+    "PutDraftAppVersionTemplateResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
@@ -1036,32 +1130,63 @@
 
 class RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef(
     _RequiredRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
     _OptionalRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
 ):
     pass
 
+RemoveDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
+    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ResolveAppVersionResourcesRequestRequestTypeDef = TypedDict(
     "ResolveAppVersionResourcesRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
     },
 )
 
+ResolveAppVersionResourcesResponseTypeDef = TypedDict(
+    "ResolveAppVersionResourcesResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "resolutionId": str,
+        "status": ResourceResolutionStatusTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ResourceErrorTypeDef = TypedDict(
     "ResourceErrorTypeDef",
     {
         "logicalResourceId": str,
         "physicalResourceId": str,
         "reason": str,
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
 _RequiredStartAppAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredStartAppAssessmentRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
     },
@@ -1157,145 +1282,21 @@
 )
 
 class UpdateAppVersionRequestRequestTypeDef(
     _RequiredUpdateAppVersionRequestRequestTypeDef, _OptionalUpdateAppVersionRequestRequestTypeDef
 ):
     pass
 
-DeleteAppAssessmentResponseTypeDef = TypedDict(
-    "DeleteAppAssessmentResponseTypeDef",
-    {
-        "assessmentArn": str,
-        "assessmentStatus": AssessmentStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteAppResponseTypeDef = TypedDict(
-    "DeleteAppResponseTypeDef",
-    {
-        "appArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteRecommendationTemplateResponseTypeDef = TypedDict(
-    "DeleteRecommendationTemplateResponseTypeDef",
-    {
-        "recommendationTemplateArn": str,
-        "status": RecommendationTemplateStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteResiliencyPolicyResponseTypeDef = TypedDict(
-    "DeleteResiliencyPolicyResponseTypeDef",
-    {
-        "policyArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAppVersionResourcesResolutionStatusResponseTypeDef = TypedDict(
-    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "errorMessage": str,
-        "resolutionId": str,
-        "status": ResourceResolutionStatusTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAppVersionResponseTypeDef = TypedDict(
-    "DescribeAppVersionResponseTypeDef",
-    {
-        "additionalInfo": Dict[str, List[str]],
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAppVersionTemplateResponseTypeDef = TypedDict(
-    "DescribeAppVersionTemplateResponseTypeDef",
-    {
-        "appArn": str,
-        "appTemplateBody": str,
-        "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDraftAppVersionResourcesImportStatusResponseTypeDef = TypedDict(
-    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "errorMessage": str,
-        "status": ResourceImportStatusTypeType,
-        "statusChangeTime": datetime,
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
-PublishAppVersionResponseTypeDef = TypedDict(
-    "PublishAppVersionResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
-    "PutDraftAppVersionTemplateResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
-    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ResolveAppVersionResourcesResponseTypeDef = TypedDict(
-    "ResolveAppVersionResourcesResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "resolutionId": str,
-        "status": ResourceResolutionStatusTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateAppVersionResponseTypeDef = TypedDict(
     "UpdateAppVersionResponseTypeDef",
     {
         "additionalInfo": Dict[str, List[str]],
         "appArn": str,
         "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAlarmRecommendationTypeDef = TypedDict(
     "_RequiredAlarmRecommendationTypeDef",
     {
         "name": str,
@@ -1417,56 +1418,56 @@
 
 CreateAppVersionAppComponentResponseTypeDef = TypedDict(
     "CreateAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAppVersionAppComponentResponseTypeDef = TypedDict(
     "DeleteAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppVersionAppComponentResponseTypeDef = TypedDict(
     "DescribeAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppVersionAppComponentsResponseTypeDef = TypedDict(
     "ListAppVersionAppComponentsResponseTypeDef",
     {
         "appArn": str,
         "appComponents": List[AppComponentTypeDef],
         "appVersion": str,
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAppVersionAppComponentResponseTypeDef = TypedDict(
     "UpdateAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAppInputSourceTypeDef = TypedDict(
     "_RequiredAppInputSourceTypeDef",
     {
         "importType": ResourceMappingTypeType,
@@ -1511,48 +1512,48 @@
     pass
 
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAppResponseTypeDef = TypedDict(
     "CreateAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppResponseTypeDef = TypedDict(
     "DescribeAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAppResponseTypeDef = TypedDict(
     "UpdateAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppVersionsResponseTypeDef = TypedDict(
     "ListAppVersionsResponseTypeDef",
     {
         "appVersions": List[AppVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredConfigRecommendationTypeDef = TypedDict(
     "_RequiredConfigRecommendationTypeDef",
     {
         "name": str,
@@ -1584,25 +1585,25 @@
 _RequiredCreateAppVersionResourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppVersionResourceRequestRequestTypeDef",
     {
         "appArn": str,
         "appComponents": Sequence[str],
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": str,
-        "resourceName": str,
         "resourceType": str,
     },
 )
 _OptionalCreateAppVersionResourceRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAppVersionResourceRequestRequestTypeDef",
     {
         "additionalInfo": Mapping[str, Sequence[str]],
         "awsAccountId": str,
         "awsRegion": str,
         "clientToken": str,
+        "resourceName": str,
     },
     total=False,
 )
 
 class CreateAppVersionResourceRequestRequestTypeDef(
     _RequiredCreateAppVersionResourceRequestRequestTypeDef,
     _OptionalCreateAppVersionResourceRequestRequestTypeDef,
@@ -1780,15 +1781,15 @@
     {
         "appArn": str,
         "appVersion": str,
         "eksSources": List[EksSourceTypeDef],
         "sourceArns": List[str],
         "status": ResourceImportStatusTypeType,
         "terraformSources": List[TerraformSourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
@@ -1798,15 +1799,17 @@
 )
 _OptionalPhysicalResourceTypeDef = TypedDict(
     "_OptionalPhysicalResourceTypeDef",
     {
         "additionalInfo": Dict[str, List[str]],
         "appComponents": List[AppComponentTypeDef],
         "excluded": bool,
+        "parentResourceName": str,
         "resourceName": str,
+        "sourceType": ResourceSourceTypeType,
     },
     total=False,
 )
 
 class PhysicalResourceTypeDef(_RequiredPhysicalResourceTypeDef, _OptionalPhysicalResourceTypeDef):
     pass
 
@@ -1895,69 +1898,69 @@
 )
 
 ListAlarmRecommendationsResponseTypeDef = TypedDict(
     "ListAlarmRecommendationsResponseTypeDef",
     {
         "alarmRecommendations": List[AlarmRecommendationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSopRecommendationsResponseTypeDef = TypedDict(
     "ListSopRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "sopRecommendations": List[SopRecommendationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTestRecommendationsResponseTypeDef = TypedDict(
     "ListTestRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "testRecommendations": List[TestRecommendationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppAssessmentsResponseTypeDef = TypedDict(
     "ListAppAssessmentsResponseTypeDef",
     {
         "assessmentSummaries": List[AppAssessmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppComponentCompliancesResponseTypeDef = TypedDict(
     "ListAppComponentCompliancesResponseTypeDef",
     {
         "componentCompliances": List[AppComponentComplianceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAppInputSourceResponseTypeDef = TypedDict(
     "DeleteAppInputSourceResponseTypeDef",
     {
         "appArn": str,
         "appInputSource": AppInputSourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppInputSourcesResponseTypeDef = TypedDict(
     "ListAppInputSourcesResponseTypeDef",
     {
         "appInputSources": List[AppInputSourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ComponentRecommendationTypeDef = TypedDict(
     "ComponentRecommendationTypeDef",
     {
         "appComponentName": str,
@@ -1966,99 +1969,99 @@
     },
 )
 
 CreateResiliencyPolicyResponseTypeDef = TypedDict(
     "CreateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeResiliencyPolicyResponseTypeDef = TypedDict(
     "DescribeResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResiliencyPoliciesResponseTypeDef = TypedDict(
     "ListResiliencyPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "resiliencyPolicies": List[ResiliencyPolicyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSuggestedResiliencyPoliciesResponseTypeDef = TypedDict(
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "resiliencyPolicies": List[ResiliencyPolicyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateResiliencyPolicyResponseTypeDef = TypedDict(
     "UpdateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAppVersionResourceResponseTypeDef = TypedDict(
     "CreateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAppVersionResourceResponseTypeDef = TypedDict(
     "DeleteAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppVersionResourceResponseTypeDef = TypedDict(
     "DescribeAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppVersionResourcesResponseTypeDef = TypedDict(
     "ListAppVersionResourcesResponseTypeDef",
     {
         "nextToken": str,
         "physicalResources": List[PhysicalResourceTypeDef],
         "resolutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAppVersionResourceResponseTypeDef = TypedDict(
     "UpdateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AddDraftAppVersionResourceMappingsRequestRequestTypeDef = TypedDict(
     "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     {
         "appArn": str,
@@ -2068,51 +2071,51 @@
 
 AddDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "resourceMappings": List[ResourceMappingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "ListAppVersionResourceMappingsResponseTypeDef",
     {
         "nextToken": str,
         "resourceMappings": List[ResourceMappingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListUnsupportedAppVersionResourcesResponseTypeDef = TypedDict(
     "ListUnsupportedAppVersionResourcesResponseTypeDef",
     {
         "nextToken": str,
         "resolutionId": str,
         "unsupportedResources": List[UnsupportedResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRecommendationTemplateResponseTypeDef = TypedDict(
     "CreateRecommendationTemplateResponseTypeDef",
     {
         "recommendationTemplate": RecommendationTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecommendationTemplatesResponseTypeDef = TypedDict(
     "ListRecommendationTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationTemplates": List[RecommendationTemplateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAppAssessmentTypeDef = TypedDict(
     "_RequiredAppAssessmentTypeDef",
     {
         "assessmentArn": str,
@@ -2144,26 +2147,26 @@
     pass
 
 ListAppComponentRecommendationsResponseTypeDef = TypedDict(
     "ListAppComponentRecommendationsResponseTypeDef",
     {
         "componentRecommendations": List[ComponentRecommendationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeAppAssessmentResponseTypeDef = TypedDict(
     "DescribeAppAssessmentResponseTypeDef",
     {
         "assessment": AppAssessmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartAppAssessmentResponseTypeDef = TypedDict(
     "StartAppAssessmentResponseTypeDef",
     {
         "assessment": AppAssessmentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/PKG-INFO` & `mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resiliencehub
-Version: 1.26.97
-Summary: Type annotations for boto3.ResilienceHub 1.26.97 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.ResilienceHub 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-resiliencehub"></a>
 
 # mypy-boto3-resiliencehub
 
 [![PyPI - mypy-boto3-resiliencehub](https://img.shields.io/pypi/v/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resiliencehub?color=blue)](https://pypistats.org/packages/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,14 +298,15 @@
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStatusTypeType,
     ResourceImportStrategyTypeType,
     ResourceMappingTypeType,
     ResourceResolutionStatusTypeType,
+    ResourceSourceTypeType,
     SopServiceTypeType,
     TemplateFormatType,
     TestRiskType,
     TestTypeType,
     ResilienceHubServiceName,
     ServiceName,
     ResourceServiceName,
@@ -322,15 +323,14 @@
 ### Typed dictionaries
 
 `mypy_boto3_resiliencehub.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resiliencehub.type_defs import (
-    ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
     EksSourceClusterNamespaceTypeDef,
     TerraformSourceTypeDef,
@@ -340,25 +340,33 @@
     RecommendationDisruptionComplianceTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
     LogicalResourceIdTypeDef,
     CreateRecommendationTemplateRequestRequestTypeDef,
     FailurePolicyTypeDef,
     DeleteAppAssessmentRequestRequestTypeDef,
+    DeleteAppAssessmentResponseTypeDef,
     DeleteAppRequestRequestTypeDef,
+    DeleteAppResponseTypeDef,
     DeleteAppVersionAppComponentRequestRequestTypeDef,
     DeleteRecommendationTemplateRequestRequestTypeDef,
+    DeleteRecommendationTemplateResponseTypeDef,
     DeleteResiliencyPolicyRequestRequestTypeDef,
+    DeleteResiliencyPolicyResponseTypeDef,
     DescribeAppAssessmentRequestRequestTypeDef,
     DescribeAppRequestRequestTypeDef,
     DescribeAppVersionAppComponentRequestRequestTypeDef,
     DescribeAppVersionRequestRequestTypeDef,
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
+    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
+    DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
+    DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
+    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
     EksSourceTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
@@ -368,42 +376,35 @@
     ListAppVersionsRequestRequestTypeDef,
     ListAppsRequestRequestTypeDef,
     ListRecommendationTemplatesRequestRequestTypeDef,
     ListResiliencyPoliciesRequestRequestTypeDef,
     ListSopRecommendationsRequestRequestTypeDef,
     ListSuggestedResiliencyPoliciesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsRequestRequestTypeDef,
     ListUnsupportedAppVersionResourcesRequestRequestTypeDef,
     PhysicalResourceIdTypeDef,
     PublishAppVersionRequestRequestTypeDef,
+    PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateRequestRequestTypeDef,
+    PutDraftAppVersionTemplateResponseTypeDef,
     S3LocationTypeDef,
     RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
+    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesRequestRequestTypeDef,
+    ResolveAppVersionResourcesResponseTypeDef,
     ResourceErrorTypeDef,
+    ResponseMetadataTypeDef,
     StartAppAssessmentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     UpdateAppVersionAppComponentRequestRequestTypeDef,
     UpdateAppVersionRequestRequestTypeDef,
-    DeleteAppAssessmentResponseTypeDef,
-    DeleteAppResponseTypeDef,
-    DeleteRecommendationTemplateResponseTypeDef,
-    DeleteResiliencyPolicyResponseTypeDef,
-    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
-    DescribeAppVersionResponseTypeDef,
-    DescribeAppVersionTemplateResponseTypeDef,
-    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PublishAppVersionResponseTypeDef,
-    PutDraftAppVersionTemplateResponseTypeDef,
-    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
-    ResolveAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
     AlarmRecommendationTypeDef,
     SopRecommendationTypeDef,
     TestRecommendationTypeDef,
     AppAssessmentSummaryTypeDef,
     AppComponentComplianceTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
@@ -460,53 +461,53 @@
     AppAssessmentTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     DescribeAppAssessmentResponseTypeDef,
     StartAppAssessmentResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> RecommendationItemTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-resiliencehub-1.26.97/mypy_boto3_resiliencehub.egg-info/SOURCES.txt` & `mypy-boto3-resiliencehub-1.27.0/mypy_boto3_resiliencehub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.26.97/setup.py` & `mypy-boto3-resiliencehub-1.27.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-resiliencehub.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resiliencehub",
-    version="1.26.97",
+    version="1.27.0",
     packages=["mypy_boto3_resiliencehub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResilienceHub 1.26.97 service generated with mypy-boto3-builder"
-        " 7.13.0"
+        "Type annotations for boto3.ResilienceHub 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/",
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


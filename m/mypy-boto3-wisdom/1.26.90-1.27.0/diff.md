# Comparing `tmp/mypy-boto3-wisdom-1.26.90.tar.gz` & `tmp/mypy-boto3-wisdom-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wisdom-1.26.90.tar", last modified: Mon Mar 13 19:32:22 2023, max compression
+gzip compressed data, was "mypy-boto3-wisdom-1.27.0.tar", last modified: Mon Jul  3 19:51:36 2023, max compression
```

## Comparing `mypy-boto3-wisdom-1.26.90.tar` & `mypy-boto3-wisdom-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:22.887339 mypy-boto3-wisdom-1.26.90/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-13 19:32:11.000000 mypy-boto3-wisdom-1.26.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17629 2023-03-13 19:32:22.887339 mypy-boto3-wisdom-1.26.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-03-13 19:32:11.000000 mypy-boto3-wisdom-1.26.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:22.887339 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-13 19:32:11.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-03-13 19:32:11.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-13 19:32:11.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-03-13 19:32:11.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-03-13 19:32:11.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-03-13 19:32:11.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-03-13 19:32:11.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-03-13 19:32:11.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-03-13 19:32:11.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:11.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35510 2023-03-13 19:32:12.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35449 2023-03-13 19:32:11.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-13 19:32:11.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 19:32:22.887339 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17629 2023-03-13 19:32:22.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-13 19:32:22.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 19:32:22.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 19:32:22.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-13 19:32:22.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-13 19:32:22.000000 mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 19:32:22.887339 mypy-boto3-wisdom-1.26.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-13 19:32:11.000000 mypy-boto3-wisdom-1.26.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:36.476148 mypy-boto3-wisdom-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:43.000000 mypy-boto3-wisdom-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-07-03 19:51:36.476148 mypy-boto3-wisdom-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-07-03 19:49:43.000000 mypy-boto3-wisdom-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:36.476148 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-03 19:49:43.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-03 19:49:43.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 19:49:43.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-07-03 19:49:43.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-07-03 19:49:43.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-07-03 19:49:43.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-03 19:49:43.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-07-03 19:49:43.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-03 19:49:43.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:43.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35572 2023-07-03 19:49:44.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35511 2023-07-03 19:49:44.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:43.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:36.476148 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-07-03 19:51:36.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 19:51:36.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:36.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:36.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:36.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 19:51:36.000000 mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:36.476148 mypy-boto3-wisdom-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:49:43.000000 mypy-boto3-wisdom-1.27.0/setup.py
```

### Comparing `mypy-boto3-wisdom-1.26.90/LICENSE` & `mypy-boto3-wisdom-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-wisdom-1.26.90/PKG-INFO` & `mypy-boto3-wisdom-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wisdom
-Version: 1.26.90
-Summary: Type annotations for boto3.ConnectWisdomService 1.26.90 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.ConnectWisdomService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-wisdom"></a>
 
 # mypy-boto3-wisdom
 
 [![PyPI - mypy-boto3-wisdom](https://img.shields.io/pypi/v/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wisdom?color=blue)](https://pypistats.org/packages/mypy-boto3-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectWisdomService 1.26.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[boto3.ConnectWisdomService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,15 +361,14 @@
     AppIntegrationsConfigurationTypeDef,
     AssistantAssociationInputDataTypeDef,
     KnowledgeBaseAssociationDataTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     ContentDataTypeDef,
     ContentReferenceTypeDef,
     ContentSummaryTypeDef,
-    ResponseMetadataTypeDef,
     CreateContentRequestRequestTypeDef,
     RenderingConfigurationTypeDef,
     CreateSessionRequestRequestTypeDef,
     SessionDataTypeDef,
     DeleteAssistantAssociationRequestRequestTypeDef,
     DeleteAssistantRequestRequestTypeDef,
     DeleteContentRequestRequestTypeDef,
@@ -379,54 +378,55 @@
     GetAssistantAssociationRequestRequestTypeDef,
     GetAssistantRequestRequestTypeDef,
     GetContentRequestRequestTypeDef,
     GetContentSummaryRequestRequestTypeDef,
     GetKnowledgeBaseRequestRequestTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
     ListAssistantAssociationsRequestRequestTypeDef,
+    ListAssistantsRequestListAssistantsPaginateTypeDef,
     ListAssistantsRequestRequestTypeDef,
+    ListContentsRequestListContentsPaginateTypeDef,
     ListContentsRequestRequestTypeDef,
+    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
     ListKnowledgeBasesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NotifyRecommendationsReceivedErrorTypeDef,
     NotifyRecommendationsReceivedRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     QueryAssistantRequestRequestTypeDef,
     QueryRecommendationTriggerDataTypeDef,
     RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SessionSummaryTypeDef,
     StartContentUploadRequestRequestTypeDef,
+    StartContentUploadResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContentRequestRequestTypeDef,
     UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef,
     SourceConfigurationTypeDef,
     CreateAssistantAssociationRequestRequestTypeDef,
     AssistantAssociationOutputDataTypeDef,
     AssistantDataTypeDef,
     AssistantSummaryTypeDef,
     CreateAssistantRequestRequestTypeDef,
     CreateContentResponseTypeDef,
     GetContentResponseTypeDef,
+    UpdateContentResponseTypeDef,
     GetContentSummaryResponseTypeDef,
     ListContentsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     SearchContentResponseTypeDef,
-    StartContentUploadResponseTypeDef,
-    UpdateContentResponseTypeDef,
     CreateSessionResponseTypeDef,
     GetSessionResponseTypeDef,
     DocumentTextTypeDef,
     SearchExpressionTypeDef,
-    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
-    ListAssistantsRequestListAssistantsPaginateTypeDef,
-    ListContentsRequestListContentsPaginateTypeDef,
-    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
-    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     NotifyRecommendationsReceivedResponseTypeDef,
     RecommendationTriggerDataTypeDef,
     SearchSessionsResponseTypeDef,
     CreateKnowledgeBaseRequestRequestTypeDef,
     KnowledgeBaseDataTypeDef,
     KnowledgeBaseSummaryTypeDef,
     AssistantAssociationDataTypeDef,
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

### Comparing `mypy-boto3-wisdom-1.26.90/README.md` & `mypy-boto3-wisdom-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-wisdom"></a>
 
 # mypy-boto3-wisdom
 
 [![PyPI - mypy-boto3-wisdom](https://img.shields.io/pypi/v/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wisdom?color=blue)](https://pypistats.org/packages/mypy-boto3-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectWisdomService 1.26.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[boto3.ConnectWisdomService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,15 +329,14 @@
     AppIntegrationsConfigurationTypeDef,
     AssistantAssociationInputDataTypeDef,
     KnowledgeBaseAssociationDataTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     ContentDataTypeDef,
     ContentReferenceTypeDef,
     ContentSummaryTypeDef,
-    ResponseMetadataTypeDef,
     CreateContentRequestRequestTypeDef,
     RenderingConfigurationTypeDef,
     CreateSessionRequestRequestTypeDef,
     SessionDataTypeDef,
     DeleteAssistantAssociationRequestRequestTypeDef,
     DeleteAssistantRequestRequestTypeDef,
     DeleteContentRequestRequestTypeDef,
@@ -347,54 +346,55 @@
     GetAssistantAssociationRequestRequestTypeDef,
     GetAssistantRequestRequestTypeDef,
     GetContentRequestRequestTypeDef,
     GetContentSummaryRequestRequestTypeDef,
     GetKnowledgeBaseRequestRequestTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
     ListAssistantAssociationsRequestRequestTypeDef,
+    ListAssistantsRequestListAssistantsPaginateTypeDef,
     ListAssistantsRequestRequestTypeDef,
+    ListContentsRequestListContentsPaginateTypeDef,
     ListContentsRequestRequestTypeDef,
+    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
     ListKnowledgeBasesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NotifyRecommendationsReceivedErrorTypeDef,
     NotifyRecommendationsReceivedRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     QueryAssistantRequestRequestTypeDef,
     QueryRecommendationTriggerDataTypeDef,
     RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SessionSummaryTypeDef,
     StartContentUploadRequestRequestTypeDef,
+    StartContentUploadResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContentRequestRequestTypeDef,
     UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef,
     SourceConfigurationTypeDef,
     CreateAssistantAssociationRequestRequestTypeDef,
     AssistantAssociationOutputDataTypeDef,
     AssistantDataTypeDef,
     AssistantSummaryTypeDef,
     CreateAssistantRequestRequestTypeDef,
     CreateContentResponseTypeDef,
     GetContentResponseTypeDef,
+    UpdateContentResponseTypeDef,
     GetContentSummaryResponseTypeDef,
     ListContentsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     SearchContentResponseTypeDef,
-    StartContentUploadResponseTypeDef,
-    UpdateContentResponseTypeDef,
     CreateSessionResponseTypeDef,
     GetSessionResponseTypeDef,
     DocumentTextTypeDef,
     SearchExpressionTypeDef,
-    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
-    ListAssistantsRequestListAssistantsPaginateTypeDef,
-    ListContentsRequestListContentsPaginateTypeDef,
-    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
-    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     NotifyRecommendationsReceivedResponseTypeDef,
     RecommendationTriggerDataTypeDef,
     SearchSessionsResponseTypeDef,
     CreateKnowledgeBaseRequestRequestTypeDef,
     KnowledgeBaseDataTypeDef,
     KnowledgeBaseSummaryTypeDef,
     AssistantAssociationDataTypeDef,
@@ -429,42 +429,42 @@
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

### Comparing `mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/__init__.py` & `mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/__init__.pyi` & `mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/__main__.py` & `mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectWisdomService 1.26.90\nVersion:         1.26.90\nBuilder"
-        " version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.ConnectWisdomService 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.90")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/client.py` & `mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/client.pyi` & `mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/literals.py` & `mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,15 @@
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
@@ -147,14 +148,15 @@
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
@@ -252,14 +254,15 @@
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
@@ -295,14 +298,15 @@
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
@@ -321,16 +325,19 @@
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
@@ -414,15 +421,17 @@
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

### Comparing `mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/literals.pyi` & `mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/literals.pyi`

 * *Files 3% similar despite different names*

```diff
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
@@ -145,14 +146,15 @@
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
@@ -250,14 +252,15 @@
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
@@ -293,14 +296,15 @@
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
@@ -319,16 +323,19 @@
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
@@ -412,15 +419,17 @@
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

### Comparing `mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/paginator.py` & `mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,75 +71,75 @@
 class ListAssistantAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistantAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantassociationspaginator)
     """
 
     def paginate(
-        self, *, assistantId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, assistantId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssistantAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistantAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantassociationspaginator)
         """
 
 
 class ListAssistantsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistants)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssistantsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistants.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantspaginator)
         """
 
 
 class ListContentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListContents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listcontentspaginator)
     """
 
     def paginate(
-        self, *, knowledgeBaseId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, knowledgeBaseId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListContents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listcontentspaginator)
         """
 
 
 class ListKnowledgeBasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListKnowledgeBases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listknowledgebasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListKnowledgeBasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListKnowledgeBases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listknowledgebasespaginator)
         """
 
 
 class QueryAssistantPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.QueryAssistant)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#queryassistantpaginator)
     """
 
     def paginate(
-        self, *, assistantId: str, queryText: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, assistantId: str, queryText: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[QueryAssistantResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.QueryAssistant.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#queryassistantpaginator)
         """
 
 
@@ -150,15 +150,15 @@
     """
 
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchContentResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchContent.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#searchcontentpaginator)
         """
 
 
@@ -169,13 +169,13 @@
     """
 
     def paginate(
         self,
         *,
         assistantId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#searchsessionspaginator)
         """
```

### Comparing `mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/paginator.pyi` & `mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -68,71 +68,71 @@
 class ListAssistantAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistantAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantassociationspaginator)
     """
 
     def paginate(
-        self, *, assistantId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, assistantId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssistantAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistantAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantassociationspaginator)
         """
 
 class ListAssistantsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistants)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAssistantsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistants.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listassistantspaginator)
         """
 
 class ListContentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListContents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listcontentspaginator)
     """
 
     def paginate(
-        self, *, knowledgeBaseId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, knowledgeBaseId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListContents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listcontentspaginator)
         """
 
 class ListKnowledgeBasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListKnowledgeBases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listknowledgebasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListKnowledgeBasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListKnowledgeBases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#listknowledgebasespaginator)
         """
 
 class QueryAssistantPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.QueryAssistant)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#queryassistantpaginator)
     """
 
     def paginate(
-        self, *, assistantId: str, queryText: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, assistantId: str, queryText: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[QueryAssistantResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.QueryAssistant.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#queryassistantpaginator)
         """
 
 class SearchContentPaginator(Paginator):
@@ -142,15 +142,15 @@
     """
 
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchContentResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchContent.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#searchcontentpaginator)
         """
 
 class SearchSessionsPaginator(Paginator):
@@ -160,13 +160,13 @@
     """
 
     def paginate(
         self,
         *,
         assistantId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SearchSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/paginators/#searchsessionspaginator)
         """
```

### Comparing `mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/type_defs.py` & `mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     "AppIntegrationsConfigurationTypeDef",
     "AssistantAssociationInputDataTypeDef",
     "KnowledgeBaseAssociationDataTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "ContentDataTypeDef",
     "ContentReferenceTypeDef",
     "ContentSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateContentRequestRequestTypeDef",
     "RenderingConfigurationTypeDef",
     "CreateSessionRequestRequestTypeDef",
     "SessionDataTypeDef",
     "DeleteAssistantAssociationRequestRequestTypeDef",
     "DeleteAssistantRequestRequestTypeDef",
     "DeleteContentRequestRequestTypeDef",
@@ -56,54 +55,55 @@
     "GetAssistantAssociationRequestRequestTypeDef",
     "GetAssistantRequestRequestTypeDef",
     "GetContentRequestRequestTypeDef",
     "GetContentSummaryRequestRequestTypeDef",
     "GetKnowledgeBaseRequestRequestTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
     "ListAssistantAssociationsRequestRequestTypeDef",
+    "ListAssistantsRequestListAssistantsPaginateTypeDef",
     "ListAssistantsRequestRequestTypeDef",
+    "ListContentsRequestListContentsPaginateTypeDef",
     "ListContentsRequestRequestTypeDef",
+    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     "ListKnowledgeBasesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "NotifyRecommendationsReceivedErrorTypeDef",
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "QueryAssistantRequestRequestTypeDef",
     "QueryRecommendationTriggerDataTypeDef",
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SessionSummaryTypeDef",
     "StartContentUploadRequestRequestTypeDef",
+    "StartContentUploadResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContentRequestRequestTypeDef",
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
     "SourceConfigurationTypeDef",
     "CreateAssistantAssociationRequestRequestTypeDef",
     "AssistantAssociationOutputDataTypeDef",
     "AssistantDataTypeDef",
     "AssistantSummaryTypeDef",
     "CreateAssistantRequestRequestTypeDef",
     "CreateContentResponseTypeDef",
     "GetContentResponseTypeDef",
+    "UpdateContentResponseTypeDef",
     "GetContentSummaryResponseTypeDef",
     "ListContentsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "SearchContentResponseTypeDef",
-    "StartContentUploadResponseTypeDef",
-    "UpdateContentResponseTypeDef",
     "CreateSessionResponseTypeDef",
     "GetSessionResponseTypeDef",
     "DocumentTextTypeDef",
     "SearchExpressionTypeDef",
-    "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
-    "ListAssistantsRequestListAssistantsPaginateTypeDef",
-    "ListContentsRequestListContentsPaginateTypeDef",
-    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
-    "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "NotifyRecommendationsReceivedResponseTypeDef",
     "RecommendationTriggerDataTypeDef",
     "SearchSessionsResponseTypeDef",
     "CreateKnowledgeBaseRequestRequestTypeDef",
     "KnowledgeBaseDataTypeDef",
     "KnowledgeBaseSummaryTypeDef",
     "AssistantAssociationDataTypeDef",
@@ -242,25 +242,14 @@
 )
 
 
 class ContentSummaryTypeDef(_RequiredContentSummaryTypeDef, _OptionalContentSummaryTypeDef):
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
 _RequiredCreateContentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContentRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "name": str,
         "uploadId": str,
     },
@@ -452,24 +441,36 @@
     "GetSessionRequestRequestTypeDef",
     {
         "assistantId": str,
         "sessionId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "assistantId": str,
+    },
+)
+_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef(
+    _RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    _OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAssistantAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssistantAssociationsRequestRequestTypeDef",
     {
         "assistantId": str,
     },
 )
 _OptionalListAssistantAssociationsRequestRequestTypeDef = TypedDict(
@@ -485,23 +486,53 @@
 class ListAssistantAssociationsRequestRequestTypeDef(
     _RequiredListAssistantAssociationsRequestRequestTypeDef,
     _OptionalListAssistantAssociationsRequestRequestTypeDef,
 ):
     pass
 
 
+ListAssistantsRequestListAssistantsPaginateTypeDef = TypedDict(
+    "ListAssistantsRequestListAssistantsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListAssistantsRequestRequestTypeDef = TypedDict(
     "ListAssistantsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListContentsRequestListContentsPaginateTypeDef = TypedDict(
+    "_RequiredListContentsRequestListContentsPaginateTypeDef",
+    {
+        "knowledgeBaseId": str,
+    },
+)
+_OptionalListContentsRequestListContentsPaginateTypeDef = TypedDict(
+    "_OptionalListContentsRequestListContentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListContentsRequestListContentsPaginateTypeDef(
+    _RequiredListContentsRequestListContentsPaginateTypeDef,
+    _OptionalListContentsRequestListContentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListContentsRequestRequestTypeDef = TypedDict(
     "_RequiredListContentsRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
     },
 )
 _OptionalListContentsRequestRequestTypeDef = TypedDict(
@@ -516,14 +547,22 @@
 
 class ListContentsRequestRequestTypeDef(
     _RequiredListContentsRequestRequestTypeDef, _OptionalListContentsRequestRequestTypeDef
 ):
     pass
 
 
+ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = TypedDict(
+    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListKnowledgeBasesRequestRequestTypeDef = TypedDict(
     "ListKnowledgeBasesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -532,14 +571,22 @@
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
 NotifyRecommendationsReceivedErrorTypeDef = TypedDict(
     "NotifyRecommendationsReceivedErrorTypeDef",
     {
         "message": str,
         "recommendationId": str,
     },
     total=False,
@@ -550,14 +597,47 @@
     {
         "assistantId": str,
         "recommendationIds": Sequence[str],
         "sessionId": str,
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
+_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
+    "_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef",
+    {
+        "assistantId": str,
+        "queryText": str,
+    },
+)
+_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
+    "_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class QueryAssistantRequestQueryAssistantPaginateTypeDef(
+    _RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef,
+    _OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef,
+):
+    pass
+
+
 _RequiredQueryAssistantRequestRequestTypeDef = TypedDict(
     "_RequiredQueryAssistantRequestRequestTypeDef",
     {
         "assistantId": str,
         "queryText": str,
     },
 )
@@ -588,14 +668,25 @@
 RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef = TypedDict(
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
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
 SessionSummaryTypeDef = TypedDict(
     "SessionSummaryTypeDef",
     {
         "assistantArn": str,
         "assistantId": str,
         "sessionArn": str,
         "sessionId": str,
@@ -606,14 +697,25 @@
     "StartContentUploadRequestRequestTypeDef",
     {
         "contentType": str,
         "knowledgeBaseId": str,
     },
 )
 
+StartContentUploadResponseTypeDef = TypedDict(
+    "StartContentUploadResponseTypeDef",
+    {
+        "headersToInclude": Dict[str, str],
+        "uploadId": str,
+        "url": str,
+        "urlExpiry": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -777,92 +879,73 @@
     pass
 
 
 CreateContentResponseTypeDef = TypedDict(
     "CreateContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContentResponseTypeDef = TypedDict(
     "GetContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateContentResponseTypeDef = TypedDict(
+    "UpdateContentResponseTypeDef",
+    {
+        "content": ContentDataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContentSummaryResponseTypeDef = TypedDict(
     "GetContentSummaryResponseTypeDef",
     {
         "contentSummary": ContentSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListContentsResponseTypeDef = TypedDict(
     "ListContentsResponseTypeDef",
     {
         "contentSummaries": List[ContentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchContentResponseTypeDef = TypedDict(
     "SearchContentResponseTypeDef",
     {
         "contentSummaries": List[ContentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartContentUploadResponseTypeDef = TypedDict(
-    "StartContentUploadResponseTypeDef",
-    {
-        "headersToInclude": Dict[str, str],
-        "uploadId": str,
-        "url": str,
-        "urlExpiry": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateContentResponseTypeDef = TypedDict(
-    "UpdateContentResponseTypeDef",
-    {
-        "content": ContentDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSessionResponseTypeDef = TypedDict(
     "CreateSessionResponseTypeDef",
     {
         "session": SessionDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "session": SessionDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DocumentTextTypeDef = TypedDict(
     "DocumentTextTypeDef",
     {
         "highlights": List[HighlightTypeDef],
@@ -874,103 +957,20 @@
 SearchExpressionTypeDef = TypedDict(
     "SearchExpressionTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
     },
 )
 
-_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
-    {
-        "assistantId": str,
-    },
-)
-_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef(
-    _RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
-    _OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
-):
-    pass
-
-
-ListAssistantsRequestListAssistantsPaginateTypeDef = TypedDict(
-    "ListAssistantsRequestListAssistantsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListContentsRequestListContentsPaginateTypeDef = TypedDict(
-    "_RequiredListContentsRequestListContentsPaginateTypeDef",
-    {
-        "knowledgeBaseId": str,
-    },
-)
-_OptionalListContentsRequestListContentsPaginateTypeDef = TypedDict(
-    "_OptionalListContentsRequestListContentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListContentsRequestListContentsPaginateTypeDef(
-    _RequiredListContentsRequestListContentsPaginateTypeDef,
-    _OptionalListContentsRequestListContentsPaginateTypeDef,
-):
-    pass
-
-
-ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = TypedDict(
-    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
-    "_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef",
-    {
-        "assistantId": str,
-        "queryText": str,
-    },
-)
-_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
-    "_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class QueryAssistantRequestQueryAssistantPaginateTypeDef(
-    _RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef,
-    _OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef,
-):
-    pass
-
-
 NotifyRecommendationsReceivedResponseTypeDef = TypedDict(
     "NotifyRecommendationsReceivedResponseTypeDef",
     {
         "errors": List[NotifyRecommendationsReceivedErrorTypeDef],
         "recommendationIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommendationTriggerDataTypeDef = TypedDict(
     "RecommendationTriggerDataTypeDef",
     {
         "query": QueryRecommendationTriggerDataTypeDef,
@@ -979,15 +979,15 @@
 )
 
 SearchSessionsResponseTypeDef = TypedDict(
     "SearchSessionsResponseTypeDef",
     {
         "nextToken": str,
         "sessionSummaries": List[SessionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
     {
         "knowledgeBaseType": KnowledgeBaseTypeType,
@@ -1126,32 +1126,32 @@
     pass
 
 
 CreateAssistantResponseTypeDef = TypedDict(
     "CreateAssistantResponseTypeDef",
     {
         "assistant": AssistantDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAssistantResponseTypeDef = TypedDict(
     "GetAssistantResponseTypeDef",
     {
         "assistant": AssistantDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssistantsResponseTypeDef = TypedDict(
     "ListAssistantsResponseTypeDef",
     {
         "assistantSummaries": List[AssistantSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDocumentTypeDef = TypedDict(
     "_RequiredDocumentTypeDef",
     {
         "contentReference": ContentReferenceTypeDef,
@@ -1200,15 +1200,15 @@
         "knowledgeBaseId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
 _OptionalSearchContentRequestSearchContentPaginateTypeDef = TypedDict(
     "_OptionalSearchContentRequestSearchContentPaginateTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class SearchContentRequestSearchContentPaginateTypeDef(
     _RequiredSearchContentRequestSearchContentPaginateTypeDef,
@@ -1246,15 +1246,15 @@
         "assistantId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
 _OptionalSearchSessionsRequestSearchSessionsPaginateTypeDef = TypedDict(
     "_OptionalSearchSessionsRequestSearchSessionsPaginateTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class SearchSessionsRequestSearchSessionsPaginateTypeDef(
     _RequiredSearchSessionsRequestSearchSessionsPaginateTypeDef,
@@ -1274,65 +1274,65 @@
     },
 )
 
 CreateKnowledgeBaseResponseTypeDef = TypedDict(
     "CreateKnowledgeBaseResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKnowledgeBaseResponseTypeDef = TypedDict(
     "GetKnowledgeBaseResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateKnowledgeBaseTemplateUriResponseTypeDef = TypedDict(
     "UpdateKnowledgeBaseTemplateUriResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKnowledgeBasesResponseTypeDef = TypedDict(
     "ListKnowledgeBasesResponseTypeDef",
     {
         "knowledgeBaseSummaries": List[KnowledgeBaseSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAssistantAssociationResponseTypeDef = TypedDict(
     "CreateAssistantAssociationResponseTypeDef",
     {
         "assistantAssociation": AssistantAssociationDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAssistantAssociationResponseTypeDef = TypedDict(
     "GetAssistantAssociationResponseTypeDef",
     {
         "assistantAssociation": AssistantAssociationDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssistantAssociationsResponseTypeDef = TypedDict(
     "ListAssistantAssociationsResponseTypeDef",
     {
         "assistantAssociationSummaries": List[AssistantAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRecommendationDataTypeDef = TypedDict(
     "_RequiredRecommendationDataTypeDef",
     {
         "document": DocumentTypeDef,
@@ -1377,19 +1377,19 @@
 
 
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "recommendations": List[RecommendationDataTypeDef],
         "triggers": List[RecommendationTriggerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryAssistantResponseTypeDef = TypedDict(
     "QueryAssistantResponseTypeDef",
     {
         "nextToken": str,
         "results": List[ResultDataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom/type_defs.pyi` & `mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     "AppIntegrationsConfigurationTypeDef",
     "AssistantAssociationInputDataTypeDef",
     "KnowledgeBaseAssociationDataTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "ContentDataTypeDef",
     "ContentReferenceTypeDef",
     "ContentSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateContentRequestRequestTypeDef",
     "RenderingConfigurationTypeDef",
     "CreateSessionRequestRequestTypeDef",
     "SessionDataTypeDef",
     "DeleteAssistantAssociationRequestRequestTypeDef",
     "DeleteAssistantRequestRequestTypeDef",
     "DeleteContentRequestRequestTypeDef",
@@ -55,54 +54,55 @@
     "GetAssistantAssociationRequestRequestTypeDef",
     "GetAssistantRequestRequestTypeDef",
     "GetContentRequestRequestTypeDef",
     "GetContentSummaryRequestRequestTypeDef",
     "GetKnowledgeBaseRequestRequestTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
     "ListAssistantAssociationsRequestRequestTypeDef",
+    "ListAssistantsRequestListAssistantsPaginateTypeDef",
     "ListAssistantsRequestRequestTypeDef",
+    "ListContentsRequestListContentsPaginateTypeDef",
     "ListContentsRequestRequestTypeDef",
+    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     "ListKnowledgeBasesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "NotifyRecommendationsReceivedErrorTypeDef",
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
+    "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "QueryAssistantRequestRequestTypeDef",
     "QueryRecommendationTriggerDataTypeDef",
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SessionSummaryTypeDef",
     "StartContentUploadRequestRequestTypeDef",
+    "StartContentUploadResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContentRequestRequestTypeDef",
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
     "SourceConfigurationTypeDef",
     "CreateAssistantAssociationRequestRequestTypeDef",
     "AssistantAssociationOutputDataTypeDef",
     "AssistantDataTypeDef",
     "AssistantSummaryTypeDef",
     "CreateAssistantRequestRequestTypeDef",
     "CreateContentResponseTypeDef",
     "GetContentResponseTypeDef",
+    "UpdateContentResponseTypeDef",
     "GetContentSummaryResponseTypeDef",
     "ListContentsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "SearchContentResponseTypeDef",
-    "StartContentUploadResponseTypeDef",
-    "UpdateContentResponseTypeDef",
     "CreateSessionResponseTypeDef",
     "GetSessionResponseTypeDef",
     "DocumentTextTypeDef",
     "SearchExpressionTypeDef",
-    "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
-    "ListAssistantsRequestListAssistantsPaginateTypeDef",
-    "ListContentsRequestListContentsPaginateTypeDef",
-    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
-    "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "NotifyRecommendationsReceivedResponseTypeDef",
     "RecommendationTriggerDataTypeDef",
     "SearchSessionsResponseTypeDef",
     "CreateKnowledgeBaseRequestRequestTypeDef",
     "KnowledgeBaseDataTypeDef",
     "KnowledgeBaseSummaryTypeDef",
     "AssistantAssociationDataTypeDef",
@@ -235,25 +235,14 @@
     },
     total=False,
 )
 
 class ContentSummaryTypeDef(_RequiredContentSummaryTypeDef, _OptionalContentSummaryTypeDef):
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
 _RequiredCreateContentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContentRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "name": str,
         "uploadId": str,
     },
@@ -437,24 +426,34 @@
     "GetSessionRequestRequestTypeDef",
     {
         "assistantId": str,
         "sessionId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "assistantId": str,
+    },
+)
+_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef(
+    _RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    _OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+):
+    pass
+
 _RequiredListAssistantAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssistantAssociationsRequestRequestTypeDef",
     {
         "assistantId": str,
     },
 )
 _OptionalListAssistantAssociationsRequestRequestTypeDef = TypedDict(
@@ -468,23 +467,51 @@
 
 class ListAssistantAssociationsRequestRequestTypeDef(
     _RequiredListAssistantAssociationsRequestRequestTypeDef,
     _OptionalListAssistantAssociationsRequestRequestTypeDef,
 ):
     pass
 
+ListAssistantsRequestListAssistantsPaginateTypeDef = TypedDict(
+    "ListAssistantsRequestListAssistantsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListAssistantsRequestRequestTypeDef = TypedDict(
     "ListAssistantsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListContentsRequestListContentsPaginateTypeDef = TypedDict(
+    "_RequiredListContentsRequestListContentsPaginateTypeDef",
+    {
+        "knowledgeBaseId": str,
+    },
+)
+_OptionalListContentsRequestListContentsPaginateTypeDef = TypedDict(
+    "_OptionalListContentsRequestListContentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListContentsRequestListContentsPaginateTypeDef(
+    _RequiredListContentsRequestListContentsPaginateTypeDef,
+    _OptionalListContentsRequestListContentsPaginateTypeDef,
+):
+    pass
+
 _RequiredListContentsRequestRequestTypeDef = TypedDict(
     "_RequiredListContentsRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
     },
 )
 _OptionalListContentsRequestRequestTypeDef = TypedDict(
@@ -497,14 +524,22 @@
 )
 
 class ListContentsRequestRequestTypeDef(
     _RequiredListContentsRequestRequestTypeDef, _OptionalListContentsRequestRequestTypeDef
 ):
     pass
 
+ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = TypedDict(
+    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListKnowledgeBasesRequestRequestTypeDef = TypedDict(
     "ListKnowledgeBasesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -513,14 +548,22 @@
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
 NotifyRecommendationsReceivedErrorTypeDef = TypedDict(
     "NotifyRecommendationsReceivedErrorTypeDef",
     {
         "message": str,
         "recommendationId": str,
     },
     total=False,
@@ -531,14 +574,45 @@
     {
         "assistantId": str,
         "recommendationIds": Sequence[str],
         "sessionId": str,
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
+_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
+    "_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef",
+    {
+        "assistantId": str,
+        "queryText": str,
+    },
+)
+_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
+    "_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class QueryAssistantRequestQueryAssistantPaginateTypeDef(
+    _RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef,
+    _OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef,
+):
+    pass
+
 _RequiredQueryAssistantRequestRequestTypeDef = TypedDict(
     "_RequiredQueryAssistantRequestRequestTypeDef",
     {
         "assistantId": str,
         "queryText": str,
     },
 )
@@ -567,14 +641,25 @@
 RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef = TypedDict(
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
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
 SessionSummaryTypeDef = TypedDict(
     "SessionSummaryTypeDef",
     {
         "assistantArn": str,
         "assistantId": str,
         "sessionArn": str,
         "sessionId": str,
@@ -585,14 +670,25 @@
     "StartContentUploadRequestRequestTypeDef",
     {
         "contentType": str,
         "knowledgeBaseId": str,
     },
 )
 
+StartContentUploadResponseTypeDef = TypedDict(
+    "StartContentUploadResponseTypeDef",
+    {
+        "headersToInclude": Dict[str, str],
+        "uploadId": str,
+        "url": str,
+        "urlExpiry": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -746,92 +842,73 @@
 ):
     pass
 
 CreateContentResponseTypeDef = TypedDict(
     "CreateContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContentResponseTypeDef = TypedDict(
     "GetContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateContentResponseTypeDef = TypedDict(
+    "UpdateContentResponseTypeDef",
+    {
+        "content": ContentDataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContentSummaryResponseTypeDef = TypedDict(
     "GetContentSummaryResponseTypeDef",
     {
         "contentSummary": ContentSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListContentsResponseTypeDef = TypedDict(
     "ListContentsResponseTypeDef",
     {
         "contentSummaries": List[ContentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchContentResponseTypeDef = TypedDict(
     "SearchContentResponseTypeDef",
     {
         "contentSummaries": List[ContentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartContentUploadResponseTypeDef = TypedDict(
-    "StartContentUploadResponseTypeDef",
-    {
-        "headersToInclude": Dict[str, str],
-        "uploadId": str,
-        "url": str,
-        "urlExpiry": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateContentResponseTypeDef = TypedDict(
-    "UpdateContentResponseTypeDef",
-    {
-        "content": ContentDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateSessionResponseTypeDef = TypedDict(
     "CreateSessionResponseTypeDef",
     {
         "session": SessionDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "session": SessionDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DocumentTextTypeDef = TypedDict(
     "DocumentTextTypeDef",
     {
         "highlights": List[HighlightTypeDef],
@@ -843,97 +920,20 @@
 SearchExpressionTypeDef = TypedDict(
     "SearchExpressionTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
     },
 )
 
-_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
-    {
-        "assistantId": str,
-    },
-)
-_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef(
-    _RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
-    _OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
-):
-    pass
-
-ListAssistantsRequestListAssistantsPaginateTypeDef = TypedDict(
-    "ListAssistantsRequestListAssistantsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListContentsRequestListContentsPaginateTypeDef = TypedDict(
-    "_RequiredListContentsRequestListContentsPaginateTypeDef",
-    {
-        "knowledgeBaseId": str,
-    },
-)
-_OptionalListContentsRequestListContentsPaginateTypeDef = TypedDict(
-    "_OptionalListContentsRequestListContentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListContentsRequestListContentsPaginateTypeDef(
-    _RequiredListContentsRequestListContentsPaginateTypeDef,
-    _OptionalListContentsRequestListContentsPaginateTypeDef,
-):
-    pass
-
-ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = TypedDict(
-    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
-    "_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef",
-    {
-        "assistantId": str,
-        "queryText": str,
-    },
-)
-_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
-    "_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class QueryAssistantRequestQueryAssistantPaginateTypeDef(
-    _RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef,
-    _OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef,
-):
-    pass
-
 NotifyRecommendationsReceivedResponseTypeDef = TypedDict(
     "NotifyRecommendationsReceivedResponseTypeDef",
     {
         "errors": List[NotifyRecommendationsReceivedErrorTypeDef],
         "recommendationIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommendationTriggerDataTypeDef = TypedDict(
     "RecommendationTriggerDataTypeDef",
     {
         "query": QueryRecommendationTriggerDataTypeDef,
@@ -942,15 +942,15 @@
 )
 
 SearchSessionsResponseTypeDef = TypedDict(
     "SearchSessionsResponseTypeDef",
     {
         "nextToken": str,
         "sessionSummaries": List[SessionSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
     {
         "knowledgeBaseType": KnowledgeBaseTypeType,
@@ -1079,32 +1079,32 @@
 ):
     pass
 
 CreateAssistantResponseTypeDef = TypedDict(
     "CreateAssistantResponseTypeDef",
     {
         "assistant": AssistantDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAssistantResponseTypeDef = TypedDict(
     "GetAssistantResponseTypeDef",
     {
         "assistant": AssistantDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssistantsResponseTypeDef = TypedDict(
     "ListAssistantsResponseTypeDef",
     {
         "assistantSummaries": List[AssistantSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDocumentTypeDef = TypedDict(
     "_RequiredDocumentTypeDef",
     {
         "contentReference": ContentReferenceTypeDef,
@@ -1149,15 +1149,15 @@
         "knowledgeBaseId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
 _OptionalSearchContentRequestSearchContentPaginateTypeDef = TypedDict(
     "_OptionalSearchContentRequestSearchContentPaginateTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class SearchContentRequestSearchContentPaginateTypeDef(
     _RequiredSearchContentRequestSearchContentPaginateTypeDef,
     _OptionalSearchContentRequestSearchContentPaginateTypeDef,
@@ -1191,15 +1191,15 @@
         "assistantId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
 _OptionalSearchSessionsRequestSearchSessionsPaginateTypeDef = TypedDict(
     "_OptionalSearchSessionsRequestSearchSessionsPaginateTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class SearchSessionsRequestSearchSessionsPaginateTypeDef(
     _RequiredSearchSessionsRequestSearchSessionsPaginateTypeDef,
     _OptionalSearchSessionsRequestSearchSessionsPaginateTypeDef,
@@ -1217,65 +1217,65 @@
     },
 )
 
 CreateKnowledgeBaseResponseTypeDef = TypedDict(
     "CreateKnowledgeBaseResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKnowledgeBaseResponseTypeDef = TypedDict(
     "GetKnowledgeBaseResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateKnowledgeBaseTemplateUriResponseTypeDef = TypedDict(
     "UpdateKnowledgeBaseTemplateUriResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListKnowledgeBasesResponseTypeDef = TypedDict(
     "ListKnowledgeBasesResponseTypeDef",
     {
         "knowledgeBaseSummaries": List[KnowledgeBaseSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAssistantAssociationResponseTypeDef = TypedDict(
     "CreateAssistantAssociationResponseTypeDef",
     {
         "assistantAssociation": AssistantAssociationDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAssistantAssociationResponseTypeDef = TypedDict(
     "GetAssistantAssociationResponseTypeDef",
     {
         "assistantAssociation": AssistantAssociationDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAssistantAssociationsResponseTypeDef = TypedDict(
     "ListAssistantAssociationsResponseTypeDef",
     {
         "assistantAssociationSummaries": List[AssistantAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRecommendationDataTypeDef = TypedDict(
     "_RequiredRecommendationDataTypeDef",
     {
         "document": DocumentTypeDef,
@@ -1316,19 +1316,19 @@
     pass
 
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "recommendations": List[RecommendationDataTypeDef],
         "triggers": List[RecommendationTriggerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryAssistantResponseTypeDef = TypedDict(
     "QueryAssistantResponseTypeDef",
     {
         "nextToken": str,
         "results": List[ResultDataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom.egg-info/PKG-INFO` & `mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wisdom
-Version: 1.26.90
-Summary: Type annotations for boto3.ConnectWisdomService 1.26.90 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.ConnectWisdomService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-wisdom"></a>
 
 # mypy-boto3-wisdom
 
 [![PyPI - mypy-boto3-wisdom](https://img.shields.io/pypi/v/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wisdom?color=blue)](https://pypistats.org/packages/mypy-boto3-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectWisdomService 1.26.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[boto3.ConnectWisdomService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,15 +361,14 @@
     AppIntegrationsConfigurationTypeDef,
     AssistantAssociationInputDataTypeDef,
     KnowledgeBaseAssociationDataTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     ContentDataTypeDef,
     ContentReferenceTypeDef,
     ContentSummaryTypeDef,
-    ResponseMetadataTypeDef,
     CreateContentRequestRequestTypeDef,
     RenderingConfigurationTypeDef,
     CreateSessionRequestRequestTypeDef,
     SessionDataTypeDef,
     DeleteAssistantAssociationRequestRequestTypeDef,
     DeleteAssistantRequestRequestTypeDef,
     DeleteContentRequestRequestTypeDef,
@@ -379,54 +378,55 @@
     GetAssistantAssociationRequestRequestTypeDef,
     GetAssistantRequestRequestTypeDef,
     GetContentRequestRequestTypeDef,
     GetContentSummaryRequestRequestTypeDef,
     GetKnowledgeBaseRequestRequestTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
     ListAssistantAssociationsRequestRequestTypeDef,
+    ListAssistantsRequestListAssistantsPaginateTypeDef,
     ListAssistantsRequestRequestTypeDef,
+    ListContentsRequestListContentsPaginateTypeDef,
     ListContentsRequestRequestTypeDef,
+    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
     ListKnowledgeBasesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     NotifyRecommendationsReceivedErrorTypeDef,
     NotifyRecommendationsReceivedRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
+    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     QueryAssistantRequestRequestTypeDef,
     QueryRecommendationTriggerDataTypeDef,
     RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SessionSummaryTypeDef,
     StartContentUploadRequestRequestTypeDef,
+    StartContentUploadResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContentRequestRequestTypeDef,
     UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef,
     SourceConfigurationTypeDef,
     CreateAssistantAssociationRequestRequestTypeDef,
     AssistantAssociationOutputDataTypeDef,
     AssistantDataTypeDef,
     AssistantSummaryTypeDef,
     CreateAssistantRequestRequestTypeDef,
     CreateContentResponseTypeDef,
     GetContentResponseTypeDef,
+    UpdateContentResponseTypeDef,
     GetContentSummaryResponseTypeDef,
     ListContentsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     SearchContentResponseTypeDef,
-    StartContentUploadResponseTypeDef,
-    UpdateContentResponseTypeDef,
     CreateSessionResponseTypeDef,
     GetSessionResponseTypeDef,
     DocumentTextTypeDef,
     SearchExpressionTypeDef,
-    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
-    ListAssistantsRequestListAssistantsPaginateTypeDef,
-    ListContentsRequestListContentsPaginateTypeDef,
-    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
-    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     NotifyRecommendationsReceivedResponseTypeDef,
     RecommendationTriggerDataTypeDef,
     SearchSessionsResponseTypeDef,
     CreateKnowledgeBaseRequestRequestTypeDef,
     KnowledgeBaseDataTypeDef,
     KnowledgeBaseSummaryTypeDef,
     AssistantAssociationDataTypeDef,
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

### Comparing `mypy-boto3-wisdom-1.26.90/mypy_boto3_wisdom.egg-info/SOURCES.txt` & `mypy-boto3-wisdom-1.27.0/mypy_boto3_wisdom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.26.90/setup.py` & `mypy-boto3-wisdom-1.27.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-wisdom.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wisdom",
-    version="1.26.90",
+    version="1.27.0",
     packages=["mypy_boto3_wisdom"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectWisdomService 1.26.90 service generated with"
-        " mypy-boto3-builder 7.13.0"
+        "Type annotations for boto3.ConnectWisdomService 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/",
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


# Comparing `tmp/mypy-boto3-codeguru-reviewer-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-codeguru-reviewer-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeguru-reviewer-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:14 2022, max compression
+gzip compressed data, was "mypy-boto3-codeguru-reviewer-1.27.0.tar", last modified: Mon Jul  3 19:50:32 2023, max compression
```

## Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1.tar` & `mypy-boto3-codeguru-reviewer-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.100817 mypy-boto3-codeguru-reviewer-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16491 2022-11-01 21:43:14.096817 mypy-boto3-codeguru-reviewer-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15011 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.084817 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15164 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    15140 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8957 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     8955 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2377 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    20981 2022-11-01 21:31:55.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    20959 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2674 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2672 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.096817 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16491 2022-11-01 21:43:13.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-11-01 21:43:13.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:13.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:13.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:13.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-01 21:43:13.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:14.100817 mypy-boto3-codeguru-reviewer-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-11-01 21:31:54.000000 mypy-boto3-codeguru-reviewer-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:32.122991 mypy-boto3-codeguru-reviewer-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-07-03 19:50:32.114991 mypy-boto3-codeguru-reviewer-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:32.114991 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21005 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:32.114991 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-07-03 19:50:31.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-03 19:50:31.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:31.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 19:50:31.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:32.122991 mypy-boto3-codeguru-reviewer-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/setup.py
```

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/LICENSE` & `mypy-boto3-codeguru-reviewer-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/PKG-INFO` & `mypy-boto3-codeguru-reviewer-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-reviewer
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodeGuruReviewer 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeGuruReviewer 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/
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
 
 <a id="mypy-boto3-codeguru-reviewer"></a>
 
 # mypy-boto3-codeguru-reviewer
 
 [![PyPI - mypy-boto3-codeguru-reviewer](https://img.shields.io/pypi/v/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-reviewer?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruReviewer 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[boto3.CodeGuruReviewer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
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
 [mypy-boto3-codeguru-reviewer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,15 +364,14 @@
 
 `mypy_boto3_codeguru_reviewer.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_reviewer.type_defs import (
     KMSKeyDetailsTypeDef,
-    ResponseMetadataTypeDef,
     BranchDiffSourceCodeTypeTypeDef,
     CodeArtifactsTypeDef,
     CodeCommitRepositoryTypeDef,
     MetricsSummaryTypeDef,
     MetricsTypeDef,
     CommitDiffSourceCodeTypeTypeDef,
     WaiterConfigTypeDef,
@@ -381,33 +381,34 @@
     DescribeRepositoryAssociationRequestRequestTypeDef,
     DisassociateRepositoryRequestRequestTypeDef,
     EventInfoTypeDef,
     ListCodeReviewsRequestRequestTypeDef,
     ListRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackSummaryTypeDef,
     ListRecommendationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
     ListRepositoryAssociationsRequestRequestTypeDef,
     RepositoryAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutRecommendationFeedbackRequestRequestTypeDef,
     RuleMetadataTypeDef,
     RepositoryHeadSourceCodeTypeTypeDef,
     S3RepositoryTypeDef,
     ThirdPartySourceRepositoryTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     S3RepositoryDetailsTypeDef,
     DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
     DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
     DescribeRecommendationFeedbackResponseTypeDef,
     RequestMetadataTypeDef,
     ListRecommendationFeedbackResponseTypeDef,
-    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
     ListRepositoryAssociationsResponseTypeDef,
     RecommendationSummaryTypeDef,
     RepositoryTypeDef,
     RepositoryAssociationTypeDef,
     S3BucketRepositoryTypeDef,
     ListRecommendationsResponseTypeDef,
     AssociateRepositoryRequestRequestTypeDef,
@@ -433,42 +434,42 @@
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

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/README.md` & `mypy-boto3-codeguru-reviewer-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codeguru-reviewer"></a>
 
 # mypy-boto3-codeguru-reviewer
 
 [![PyPI - mypy-boto3-codeguru-reviewer](https://img.shields.io/pypi/v/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-reviewer?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruReviewer 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[boto3.CodeGuruReviewer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
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
 [mypy-boto3-codeguru-reviewer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,15 +332,14 @@
 
 `mypy_boto3_codeguru_reviewer.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_reviewer.type_defs import (
     KMSKeyDetailsTypeDef,
-    ResponseMetadataTypeDef,
     BranchDiffSourceCodeTypeTypeDef,
     CodeArtifactsTypeDef,
     CodeCommitRepositoryTypeDef,
     MetricsSummaryTypeDef,
     MetricsTypeDef,
     CommitDiffSourceCodeTypeTypeDef,
     WaiterConfigTypeDef,
@@ -350,33 +349,34 @@
     DescribeRepositoryAssociationRequestRequestTypeDef,
     DisassociateRepositoryRequestRequestTypeDef,
     EventInfoTypeDef,
     ListCodeReviewsRequestRequestTypeDef,
     ListRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackSummaryTypeDef,
     ListRecommendationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
     ListRepositoryAssociationsRequestRequestTypeDef,
     RepositoryAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutRecommendationFeedbackRequestRequestTypeDef,
     RuleMetadataTypeDef,
     RepositoryHeadSourceCodeTypeTypeDef,
     S3RepositoryTypeDef,
     ThirdPartySourceRepositoryTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     S3RepositoryDetailsTypeDef,
     DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
     DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
     DescribeRecommendationFeedbackResponseTypeDef,
     RequestMetadataTypeDef,
     ListRecommendationFeedbackResponseTypeDef,
-    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
     ListRepositoryAssociationsResponseTypeDef,
     RecommendationSummaryTypeDef,
     RepositoryTypeDef,
     RepositoryAssociationTypeDef,
     S3BucketRepositoryTypeDef,
     ListRecommendationsResponseTypeDef,
     AssociateRepositoryRequestRequestTypeDef,
@@ -402,42 +402,42 @@
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

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/__init__.py` & `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/__init__.pyi` & `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/__main__.py` & `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeGuruReviewer 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.CodeGuruReviewer 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer\nOther"
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

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/client.py` & `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/client.pyi` & `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/literals.py` & `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,23 +85,25 @@
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
@@ -111,30 +113,35 @@
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
@@ -160,14 +167,15 @@
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
@@ -212,51 +220,57 @@
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
@@ -269,14 +283,15 @@
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
@@ -288,28 +303,35 @@
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
@@ -318,14 +340,15 @@
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
@@ -336,55 +359,64 @@
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

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/literals.pyi` & `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -83,23 +83,25 @@
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
@@ -109,30 +111,35 @@
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
@@ -158,14 +165,15 @@
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
@@ -210,51 +218,57 @@
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
@@ -267,14 +281,15 @@
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
@@ -286,28 +301,35 @@
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
@@ -316,14 +338,15 @@
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
@@ -334,55 +357,64 @@
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

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/paginator.py` & `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,13 +48,13 @@
     def paginate(
         self,
         *,
         ProviderTypes: Sequence[ProviderTypeType] = ...,
         States: Sequence[RepositoryAssociationStateType] = ...,
         Names: Sequence[str] = ...,
         Owners: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRepositoryAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Paginator.ListRepositoryAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/paginators/#listrepositoryassociationspaginator)
         """
```

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/paginator.pyi` & `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,13 +45,13 @@
     def paginate(
         self,
         *,
         ProviderTypes: Sequence[ProviderTypeType] = ...,
         States: Sequence[RepositoryAssociationStateType] = ...,
         Names: Sequence[str] = ...,
         Owners: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRepositoryAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Paginator.ListRepositoryAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/paginators/#listrepositoryassociationspaginator)
         """
```

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/type_defs.py` & `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "KMSKeyDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "BranchDiffSourceCodeTypeTypeDef",
     "CodeArtifactsTypeDef",
     "CodeCommitRepositoryTypeDef",
     "MetricsSummaryTypeDef",
     "MetricsTypeDef",
     "CommitDiffSourceCodeTypeTypeDef",
     "WaiterConfigTypeDef",
@@ -51,33 +50,34 @@
     "DescribeRepositoryAssociationRequestRequestTypeDef",
     "DisassociateRepositoryRequestRequestTypeDef",
     "EventInfoTypeDef",
     "ListCodeReviewsRequestRequestTypeDef",
     "ListRecommendationFeedbackRequestRequestTypeDef",
     "RecommendationFeedbackSummaryTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
     "ListRepositoryAssociationsRequestRequestTypeDef",
     "RepositoryAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PutRecommendationFeedbackRequestRequestTypeDef",
     "RuleMetadataTypeDef",
     "RepositoryHeadSourceCodeTypeTypeDef",
     "S3RepositoryTypeDef",
     "ThirdPartySourceRepositoryTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "S3RepositoryDetailsTypeDef",
     "DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef",
     "DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef",
     "DescribeRecommendationFeedbackResponseTypeDef",
     "RequestMetadataTypeDef",
     "ListRecommendationFeedbackResponseTypeDef",
-    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
     "ListRepositoryAssociationsResponseTypeDef",
     "RecommendationSummaryTypeDef",
     "RepositoryTypeDef",
     "RepositoryAssociationTypeDef",
     "S3BucketRepositoryTypeDef",
     "ListRecommendationsResponseTypeDef",
     "AssociateRepositoryRequestRequestTypeDef",
@@ -100,25 +100,14 @@
     {
         "KMSKeyId": str,
         "EncryptionOption": EncryptionOptionType,
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
 BranchDiffSourceCodeTypeTypeDef = TypedDict(
     "BranchDiffSourceCodeTypeTypeDef",
     {
         "SourceBranchName": str,
         "DestinationBranchName": str,
     },
 )
@@ -333,20 +322,22 @@
 class ListRecommendationsRequestRequestTypeDef(
     _RequiredListRecommendationsRequestRequestTypeDef,
     _OptionalListRecommendationsRequestRequestTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef = TypedDict(
+    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ProviderTypes": Sequence[ProviderTypeType],
+        "States": Sequence[RepositoryAssociationStateType],
+        "Names": Sequence[str],
+        "Owners": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListRepositoryAssociationsRequestRequestTypeDef = TypedDict(
     "ListRepositoryAssociationsRequestRequestTypeDef",
     {
@@ -378,14 +369,32 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
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
 PutRecommendationFeedbackRequestRequestTypeDef = TypedDict(
     "PutRecommendationFeedbackRequestRequestTypeDef",
     {
         "CodeReviewArn": str,
         "RecommendationId": str,
         "Reactions": Sequence[ReactionType],
     },
@@ -423,14 +432,25 @@
     {
         "Name": str,
         "ConnectionArn": str,
         "Owner": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -439,22 +459,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 S3RepositoryDetailsTypeDef = TypedDict(
     "S3RepositoryDetailsTypeDef",
     {
         "BucketName": str,
         "CodeArtifacts": CodeArtifactsTypeDef,
     },
     total=False,
@@ -504,15 +516,15 @@
     pass
 
 
 DescribeRecommendationFeedbackResponseTypeDef = TypedDict(
     "DescribeRecommendationFeedbackResponseTypeDef",
     {
         "RecommendationFeedback": RecommendationFeedbackTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RequestMetadataTypeDef = TypedDict(
     "RequestMetadataTypeDef",
     {
         "RequestId": str,
@@ -524,36 +536,24 @@
 )
 
 ListRecommendationFeedbackResponseTypeDef = TypedDict(
     "ListRecommendationFeedbackResponseTypeDef",
     {
         "RecommendationFeedbackSummaries": List[RecommendationFeedbackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef = TypedDict(
-    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
-    {
-        "ProviderTypes": Sequence[ProviderTypeType],
-        "States": Sequence[RepositoryAssociationStateType],
-        "Names": Sequence[str],
-        "Owners": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListRepositoryAssociationsResponseTypeDef = TypedDict(
     "ListRepositoryAssociationsResponseTypeDef",
     {
         "RepositoryAssociationSummaries": List[RepositoryAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommendationSummaryTypeDef = TypedDict(
     "RecommendationSummaryTypeDef",
     {
         "FilePath": str,
@@ -620,15 +620,15 @@
 
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "RecommendationSummaries": List[RecommendationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAssociateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateRepositoryRequestRequestTypeDef",
     {
         "Repository": RepositoryTypeDef,
@@ -653,33 +653,33 @@
 
 
 AssociateRepositoryResponseTypeDef = TypedDict(
     "AssociateRepositoryResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRepositoryAssociationResponseTypeDef = TypedDict(
     "DescribeRepositoryAssociationResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateRepositoryResponseTypeDef = TypedDict(
     "DisassociateRepositoryResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceCodeTypeTypeDef = TypedDict(
     "SourceCodeTypeTypeDef",
     {
         "CommitDiff": CommitDiffSourceCodeTypeTypeDef,
@@ -743,31 +743,31 @@
 )
 
 ListCodeReviewsResponseTypeDef = TypedDict(
     "ListCodeReviewsResponseTypeDef",
     {
         "CodeReviewSummaries": List[CodeReviewSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCodeReviewResponseTypeDef = TypedDict(
     "CreateCodeReviewResponseTypeDef",
     {
         "CodeReview": CodeReviewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCodeReviewResponseTypeDef = TypedDict(
     "DescribeCodeReviewResponseTypeDef",
     {
         "CodeReview": CodeReviewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCodeReviewTypeTypeDef = TypedDict(
     "_RequiredCodeReviewTypeTypeDef",
     {
         "RepositoryAnalysis": RepositoryAnalysisTypeDef,
```

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/type_defs.pyi` & `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "KMSKeyDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "BranchDiffSourceCodeTypeTypeDef",
     "CodeArtifactsTypeDef",
     "CodeCommitRepositoryTypeDef",
     "MetricsSummaryTypeDef",
     "MetricsTypeDef",
     "CommitDiffSourceCodeTypeTypeDef",
     "WaiterConfigTypeDef",
@@ -50,33 +49,34 @@
     "DescribeRepositoryAssociationRequestRequestTypeDef",
     "DisassociateRepositoryRequestRequestTypeDef",
     "EventInfoTypeDef",
     "ListCodeReviewsRequestRequestTypeDef",
     "ListRecommendationFeedbackRequestRequestTypeDef",
     "RecommendationFeedbackSummaryTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
     "ListRepositoryAssociationsRequestRequestTypeDef",
     "RepositoryAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "PutRecommendationFeedbackRequestRequestTypeDef",
     "RuleMetadataTypeDef",
     "RepositoryHeadSourceCodeTypeTypeDef",
     "S3RepositoryTypeDef",
     "ThirdPartySourceRepositoryTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "S3RepositoryDetailsTypeDef",
     "DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef",
     "DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef",
     "DescribeRecommendationFeedbackResponseTypeDef",
     "RequestMetadataTypeDef",
     "ListRecommendationFeedbackResponseTypeDef",
-    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
     "ListRepositoryAssociationsResponseTypeDef",
     "RecommendationSummaryTypeDef",
     "RepositoryTypeDef",
     "RepositoryAssociationTypeDef",
     "S3BucketRepositoryTypeDef",
     "ListRecommendationsResponseTypeDef",
     "AssociateRepositoryRequestRequestTypeDef",
@@ -99,25 +99,14 @@
     {
         "KMSKeyId": str,
         "EncryptionOption": EncryptionOptionType,
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
 BranchDiffSourceCodeTypeTypeDef = TypedDict(
     "BranchDiffSourceCodeTypeTypeDef",
     {
         "SourceBranchName": str,
         "DestinationBranchName": str,
     },
 )
@@ -322,20 +311,22 @@
 
 class ListRecommendationsRequestRequestTypeDef(
     _RequiredListRecommendationsRequestRequestTypeDef,
     _OptionalListRecommendationsRequestRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef = TypedDict(
+    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ProviderTypes": Sequence[ProviderTypeType],
+        "States": Sequence[RepositoryAssociationStateType],
+        "Names": Sequence[str],
+        "Owners": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListRepositoryAssociationsRequestRequestTypeDef = TypedDict(
     "ListRepositoryAssociationsRequestRequestTypeDef",
     {
@@ -367,14 +358,32 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
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
 PutRecommendationFeedbackRequestRequestTypeDef = TypedDict(
     "PutRecommendationFeedbackRequestRequestTypeDef",
     {
         "CodeReviewArn": str,
         "RecommendationId": str,
         "Reactions": Sequence[ReactionType],
     },
@@ -412,14 +421,25 @@
     {
         "Name": str,
         "ConnectionArn": str,
         "Owner": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -428,22 +448,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 S3RepositoryDetailsTypeDef = TypedDict(
     "S3RepositoryDetailsTypeDef",
     {
         "BucketName": str,
         "CodeArtifacts": CodeArtifactsTypeDef,
     },
     total=False,
@@ -489,15 +501,15 @@
 ):
     pass
 
 DescribeRecommendationFeedbackResponseTypeDef = TypedDict(
     "DescribeRecommendationFeedbackResponseTypeDef",
     {
         "RecommendationFeedback": RecommendationFeedbackTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RequestMetadataTypeDef = TypedDict(
     "RequestMetadataTypeDef",
     {
         "RequestId": str,
@@ -509,36 +521,24 @@
 )
 
 ListRecommendationFeedbackResponseTypeDef = TypedDict(
     "ListRecommendationFeedbackResponseTypeDef",
     {
         "RecommendationFeedbackSummaries": List[RecommendationFeedbackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef = TypedDict(
-    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
-    {
-        "ProviderTypes": Sequence[ProviderTypeType],
-        "States": Sequence[RepositoryAssociationStateType],
-        "Names": Sequence[str],
-        "Owners": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListRepositoryAssociationsResponseTypeDef = TypedDict(
     "ListRepositoryAssociationsResponseTypeDef",
     {
         "RepositoryAssociationSummaries": List[RepositoryAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommendationSummaryTypeDef = TypedDict(
     "RecommendationSummaryTypeDef",
     {
         "FilePath": str,
@@ -603,15 +603,15 @@
     pass
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "RecommendationSummaries": List[RecommendationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAssociateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateRepositoryRequestRequestTypeDef",
     {
         "Repository": RepositoryTypeDef,
@@ -634,33 +634,33 @@
     pass
 
 AssociateRepositoryResponseTypeDef = TypedDict(
     "AssociateRepositoryResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRepositoryAssociationResponseTypeDef = TypedDict(
     "DescribeRepositoryAssociationResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateRepositoryResponseTypeDef = TypedDict(
     "DisassociateRepositoryResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceCodeTypeTypeDef = TypedDict(
     "SourceCodeTypeTypeDef",
     {
         "CommitDiff": CommitDiffSourceCodeTypeTypeDef,
@@ -724,31 +724,31 @@
 )
 
 ListCodeReviewsResponseTypeDef = TypedDict(
     "ListCodeReviewsResponseTypeDef",
     {
         "CodeReviewSummaries": List[CodeReviewSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCodeReviewResponseTypeDef = TypedDict(
     "CreateCodeReviewResponseTypeDef",
     {
         "CodeReview": CodeReviewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCodeReviewResponseTypeDef = TypedDict(
     "DescribeCodeReviewResponseTypeDef",
     {
         "CodeReview": CodeReviewTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCodeReviewTypeTypeDef = TypedDict(
     "_RequiredCodeReviewTypeTypeDef",
     {
         "RepositoryAnalysis": RepositoryAnalysisTypeDef,
```

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/waiter.py` & `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer/waiter.pyi` & `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO` & `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-reviewer
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodeGuruReviewer 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.CodeGuruReviewer 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/
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
 
 <a id="mypy-boto3-codeguru-reviewer"></a>
 
 # mypy-boto3-codeguru-reviewer
 
 [![PyPI - mypy-boto3-codeguru-reviewer](https://img.shields.io/pypi/v/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-reviewer?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruReviewer 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[boto3.CodeGuruReviewer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
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
 [mypy-boto3-codeguru-reviewer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,15 +364,14 @@
 
 `mypy_boto3_codeguru_reviewer.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_reviewer.type_defs import (
     KMSKeyDetailsTypeDef,
-    ResponseMetadataTypeDef,
     BranchDiffSourceCodeTypeTypeDef,
     CodeArtifactsTypeDef,
     CodeCommitRepositoryTypeDef,
     MetricsSummaryTypeDef,
     MetricsTypeDef,
     CommitDiffSourceCodeTypeTypeDef,
     WaiterConfigTypeDef,
@@ -381,33 +381,34 @@
     DescribeRepositoryAssociationRequestRequestTypeDef,
     DisassociateRepositoryRequestRequestTypeDef,
     EventInfoTypeDef,
     ListCodeReviewsRequestRequestTypeDef,
     ListRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackSummaryTypeDef,
     ListRecommendationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
     ListRepositoryAssociationsRequestRequestTypeDef,
     RepositoryAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
     PutRecommendationFeedbackRequestRequestTypeDef,
     RuleMetadataTypeDef,
     RepositoryHeadSourceCodeTypeTypeDef,
     S3RepositoryTypeDef,
     ThirdPartySourceRepositoryTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     S3RepositoryDetailsTypeDef,
     DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
     DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
     DescribeRecommendationFeedbackResponseTypeDef,
     RequestMetadataTypeDef,
     ListRecommendationFeedbackResponseTypeDef,
-    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
     ListRepositoryAssociationsResponseTypeDef,
     RecommendationSummaryTypeDef,
     RepositoryTypeDef,
     RepositoryAssociationTypeDef,
     S3BucketRepositoryTypeDef,
     ListRecommendationsResponseTypeDef,
     AssociateRepositoryRequestRequestTypeDef,
@@ -433,42 +434,42 @@
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

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt` & `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.26.0.post1/setup.py` & `mypy-boto3-codeguru-reviewer-1.27.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-codeguru-reviewer.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeguru-reviewer",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_codeguru_reviewer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeGuruReviewer 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.CodeGuruReviewer 1.27.0 service generated with"
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
     keywords="boto3 codeguru-reviewer type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_codeguru_reviewer": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_codeguru_reviewer": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/",
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


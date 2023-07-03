# Comparing `tmp/mypy-boto3-ecr-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-ecr-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecr-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:22 2022, max compression
+gzip compressed data, was "mypy-boto3-ecr-1.27.0.tar", last modified: Mon Jul  3 19:50:42 2023, max compression
```

## Comparing `mypy-boto3-ecr-1.26.0.post1.tar` & `mypy-boto3-ecr-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:22.372825 mypy-boto3-ecr-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:33:58.000000 mypy-boto3-ecr-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    19986 2022-11-01 21:43:22.372825 mypy-boto3-ecr-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18561 2022-11-01 21:33:58.000000 mypy-boto3-ecr-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:22.372825 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-11-01 21:33:58.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2243 2022-11-01 21:33:58.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-11-01 21:33:58.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33677 2022-11-01 21:33:59.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    33621 2022-11-01 21:33:58.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10322 2022-11-01 21:33:59.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    10320 2022-11-01 21:33:59.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8159 2022-11-01 21:33:59.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     8151 2022-11-01 21:33:59.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:33:58.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    51877 2022-11-01 21:34:00.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    51804 2022-11-01 21:33:59.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:33:58.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2922 2022-11-01 21:33:59.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-11-01 21:33:59.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:22.372825 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    19986 2022-11-01 21:43:22.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-11-01 21:43:22.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:22.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:22.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:22.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-01 21:43:22.000000 mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:22.372825 mypy-boto3-ecr-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-11-01 21:33:58.000000 mypy-boto3-ecr-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:42.587180 mypy-boto3-ecr-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:36:54.000000 mypy-boto3-ecr-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-07-03 19:50:42.587180 mypy-boto3-ecr-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-07-03 19:36:54.000000 mypy-boto3-ecr-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:42.587180 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-03 19:36:54.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-03 19:36:54.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:36:54.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33677 2023-07-03 19:36:55.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33621 2023-07-03 19:36:55.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-07-03 19:36:55.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-03 19:36:55.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-07-03 19:36:55.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-07-03 19:36:55.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:36:54.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    51967 2023-07-03 19:36:56.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51894 2023-07-03 19:36:55.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:36:54.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-03 19:36:55.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-03 19:36:55.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:42.587180 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-07-03 19:50:42.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 19:50:42.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:42.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:42.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:42.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:42.000000 mypy-boto3-ecr-1.27.0/mypy_boto3_ecr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:42.587180 mypy-boto3-ecr-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:36:54.000000 mypy-boto3-ecr-1.27.0/setup.py
```

### Comparing `mypy-boto3-ecr-1.26.0.post1/LICENSE` & `mypy-boto3-ecr-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-ecr-1.26.0.post1/PKG-INFO` & `mypy-boto3-ecr-1.27.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ECR 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ECR 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/
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
 
 <a id="mypy-boto3-ecr"></a>
 
 # mypy-boto3-ecr
 
 [![PyPI - mypy-boto3-ecr](https://img.shields.io/pypi/v/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecr?color=blue)](https://pypistats.org/packages/mypy-boto3-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECR 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[boto3.ECR 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -389,101 +390,101 @@
 from mypy_boto3_ecr.type_defs import (
     AttributeTypeDef,
     AuthorizationDataTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
-    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
     BatchGetRepositoryScanningConfigurationRequestRequestTypeDef,
     RepositoryScanningConfigurationFailureTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
+    CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleRequestRequestTypeDef,
+    CreatePullThroughCacheRuleResponseTypeDef,
     EncryptionConfigurationTypeDef,
     ImageScanningConfigurationTypeDef,
     TagTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
+    DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleRequestRequestTypeDef,
+    DeletePullThroughCacheRuleResponseTypeDef,
+    DeleteRegistryPolicyResponseTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
     ImageReplicationStatusTypeDef,
-    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     ImageScanStatusTypeDef,
     DescribeImagesFilterTypeDef,
+    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
     DescribePullThroughCacheRulesRequestRequestTypeDef,
     PullThroughCacheRuleTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
     GetDownloadUrlForLayerRequestRequestTypeDef,
+    GetDownloadUrlForLayerResponseTypeDef,
     LifecyclePolicyPreviewFilterTypeDef,
     LifecyclePolicyPreviewSummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
+    GetLifecyclePolicyResponseTypeDef,
+    GetRegistryPolicyResponseTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
     ImageScanFindingsSummaryTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
+    InitiateLayerUploadResponseTypeDef,
     LifecyclePolicyRuleActionTypeDef,
     ListImagesFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     VulnerablePackageTypeDef,
+    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutImageTagMutabilityRequestRequestTypeDef,
+    PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyRequestRequestTypeDef,
+    PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyRequestRequestTypeDef,
+    PutRegistryPolicyResponseTypeDef,
     RecommendationTypeDef,
     ScanningRepositoryFilterTypeDef,
     ReplicationDestinationTypeDef,
     RepositoryFilterTypeDef,
+    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
     StartLifecyclePolicyPreviewRequestRequestTypeDef,
+    StartLifecyclePolicyPreviewResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UploadLayerPartRequestRequestTypeDef,
+    UploadLayerPartResponseTypeDef,
     ImageScanFindingTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
     ResourceDetailsTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
-    CompleteLayerUploadResponseTypeDef,
-    CreatePullThroughCacheRuleResponseTypeDef,
-    DeleteLifecyclePolicyResponseTypeDef,
-    DeletePullThroughCacheRuleResponseTypeDef,
-    DeleteRegistryPolicyResponseTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
-    GetDownloadUrlForLayerResponseTypeDef,
-    GetLifecyclePolicyResponseTypeDef,
-    GetRegistryPolicyResponseTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
-    InitiateLayerUploadResponseTypeDef,
-    PutImageTagMutabilityResponseTypeDef,
-    PutLifecyclePolicyResponseTypeDef,
-    PutRegistryPolicyResponseTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
-    StartLifecyclePolicyPreviewResponseTypeDef,
-    UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
     BatchGetImageRequestRequestTypeDef,
     DescribeImageReplicationStatusRequestRequestTypeDef,
+    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
     DescribeImageScanFindingsRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     ListImagesResponseTypeDef,
     StartImageScanRequestRequestTypeDef,
     PutImageScanningConfigurationRequestRequestTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     RepositoryTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CvssScoreDetailsTypeDef,
     DescribeImageReplicationStatusResponseTypeDef,
-    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
-    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     StartImageScanResponseTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     DescribePullThroughCacheRulesResponseTypeDef,
     GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
@@ -529,42 +530,42 @@
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

### Comparing `mypy-boto3-ecr-1.26.0.post1/README.md` & `mypy-boto3-ecr-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ecr"></a>
 
 # mypy-boto3-ecr
 
 [![PyPI - mypy-boto3-ecr](https://img.shields.io/pypi/v/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecr?color=blue)](https://pypistats.org/packages/mypy-boto3-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECR 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[boto3.ECR 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,101 +358,101 @@
 from mypy_boto3_ecr.type_defs import (
     AttributeTypeDef,
     AuthorizationDataTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
-    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
     BatchGetRepositoryScanningConfigurationRequestRequestTypeDef,
     RepositoryScanningConfigurationFailureTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
+    CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleRequestRequestTypeDef,
+    CreatePullThroughCacheRuleResponseTypeDef,
     EncryptionConfigurationTypeDef,
     ImageScanningConfigurationTypeDef,
     TagTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
+    DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleRequestRequestTypeDef,
+    DeletePullThroughCacheRuleResponseTypeDef,
+    DeleteRegistryPolicyResponseTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
     ImageReplicationStatusTypeDef,
-    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     ImageScanStatusTypeDef,
     DescribeImagesFilterTypeDef,
+    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
     DescribePullThroughCacheRulesRequestRequestTypeDef,
     PullThroughCacheRuleTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
     GetDownloadUrlForLayerRequestRequestTypeDef,
+    GetDownloadUrlForLayerResponseTypeDef,
     LifecyclePolicyPreviewFilterTypeDef,
     LifecyclePolicyPreviewSummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
+    GetLifecyclePolicyResponseTypeDef,
+    GetRegistryPolicyResponseTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
     ImageScanFindingsSummaryTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
+    InitiateLayerUploadResponseTypeDef,
     LifecyclePolicyRuleActionTypeDef,
     ListImagesFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     VulnerablePackageTypeDef,
+    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutImageTagMutabilityRequestRequestTypeDef,
+    PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyRequestRequestTypeDef,
+    PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyRequestRequestTypeDef,
+    PutRegistryPolicyResponseTypeDef,
     RecommendationTypeDef,
     ScanningRepositoryFilterTypeDef,
     ReplicationDestinationTypeDef,
     RepositoryFilterTypeDef,
+    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
     StartLifecyclePolicyPreviewRequestRequestTypeDef,
+    StartLifecyclePolicyPreviewResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UploadLayerPartRequestRequestTypeDef,
+    UploadLayerPartResponseTypeDef,
     ImageScanFindingTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
     ResourceDetailsTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
-    CompleteLayerUploadResponseTypeDef,
-    CreatePullThroughCacheRuleResponseTypeDef,
-    DeleteLifecyclePolicyResponseTypeDef,
-    DeletePullThroughCacheRuleResponseTypeDef,
-    DeleteRegistryPolicyResponseTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
-    GetDownloadUrlForLayerResponseTypeDef,
-    GetLifecyclePolicyResponseTypeDef,
-    GetRegistryPolicyResponseTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
-    InitiateLayerUploadResponseTypeDef,
-    PutImageTagMutabilityResponseTypeDef,
-    PutLifecyclePolicyResponseTypeDef,
-    PutRegistryPolicyResponseTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
-    StartLifecyclePolicyPreviewResponseTypeDef,
-    UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
     BatchGetImageRequestRequestTypeDef,
     DescribeImageReplicationStatusRequestRequestTypeDef,
+    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
     DescribeImageScanFindingsRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     ListImagesResponseTypeDef,
     StartImageScanRequestRequestTypeDef,
     PutImageScanningConfigurationRequestRequestTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     RepositoryTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CvssScoreDetailsTypeDef,
     DescribeImageReplicationStatusResponseTypeDef,
-    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
-    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     StartImageScanResponseTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     DescribePullThroughCacheRulesResponseTypeDef,
     GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
@@ -498,42 +498,42 @@
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

### Comparing `mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/__init__.py` & `mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/__init__.pyi` & `mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/__main__.py` & `mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECR 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.ECR 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR\nOther"
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

### Comparing `mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/client.py` & `mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/client.pyi` & `mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/literals.py` & `mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/literals.pyi`

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
     "DescribeImageScanFindingsPaginatorName",
     "DescribeImagesPaginatorName",
     "DescribePullThroughCacheRulesPaginatorName",
     "DescribeRepositoriesPaginatorName",
     "EncryptionTypeType",
     "FindingSeverityType",
@@ -48,15 +47,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 DescribeImageScanFindingsPaginatorName = Literal["describe_image_scan_findings"]
 DescribeImagesPaginatorName = Literal["describe_images"]
 DescribePullThroughCacheRulesPaginatorName = Literal["describe_pull_through_cache_rules"]
 DescribeRepositoriesPaginatorName = Literal["describe_repositories"]
 EncryptionTypeType = Literal["AES256", "KMS"]
 FindingSeverityType = Literal["CRITICAL", "HIGH", "INFORMATIONAL", "LOW", "MEDIUM", "UNDEFINED"]
 GetLifecyclePolicyPreviewPaginatorName = Literal["get_lifecycle_policy_preview"]
@@ -106,23 +104,25 @@
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
@@ -132,30 +132,35 @@
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
@@ -181,14 +186,15 @@
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
@@ -233,51 +239,57 @@
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
@@ -290,14 +302,15 @@
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
@@ -309,28 +322,35 @@
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
@@ -339,14 +359,15 @@
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
@@ -357,55 +378,64 @@
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
@@ -439,21 +469,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/literals.pyi` & `mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/literals.py`

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
     "DescribeImageScanFindingsPaginatorName",
     "DescribeImagesPaginatorName",
     "DescribePullThroughCacheRulesPaginatorName",
     "DescribeRepositoriesPaginatorName",
     "EncryptionTypeType",
     "FindingSeverityType",
@@ -47,14 +48,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 DescribeImageScanFindingsPaginatorName = Literal["describe_image_scan_findings"]
 DescribeImagesPaginatorName = Literal["describe_images"]
 DescribePullThroughCacheRulesPaginatorName = Literal["describe_pull_through_cache_rules"]
 DescribeRepositoriesPaginatorName = Literal["describe_repositories"]
 EncryptionTypeType = Literal["AES256", "KMS"]
 FindingSeverityType = Literal["CRITICAL", "HIGH", "INFORMATIONAL", "LOW", "MEDIUM", "UNDEFINED"]
 GetLifecyclePolicyPreviewPaginatorName = Literal["get_lifecycle_policy_preview"]
@@ -104,23 +106,25 @@
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
@@ -130,30 +134,35 @@
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
@@ -179,14 +188,15 @@
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
@@ -231,51 +241,57 @@
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
@@ -288,14 +304,15 @@
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
@@ -307,28 +324,35 @@
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
@@ -337,14 +361,15 @@
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
@@ -355,55 +380,64 @@
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
@@ -437,21 +471,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/paginator.py` & `mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -52,136 +52,128 @@
     "DescribeImagesPaginator",
     "DescribePullThroughCacheRulesPaginator",
     "DescribeRepositoriesPaginator",
     "GetLifecyclePolicyPreviewPaginator",
     "ListImagesPaginator",
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
 class DescribeImageScanFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImageScanFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describeimagescanfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         imageId: ImageIdentifierTypeDef,
         registryId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeImageScanFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImageScanFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describeimagescanfindingspaginator)
         """
 
-
 class DescribeImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describeimagespaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: DescribeImagesFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describeimagespaginator)
         """
 
-
 class DescribePullThroughCacheRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribePullThroughCacheRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describepullthroughcacherulespaginator)
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         ecrRepositoryPrefixes: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribePullThroughCacheRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribePullThroughCacheRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describepullthroughcacherulespaginator)
         """
 
-
 class DescribeRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describerepositoriespaginator)
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describerepositoriespaginator)
         """
 
-
 class GetLifecyclePolicyPreviewPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.GetLifecyclePolicyPreview)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#getlifecyclepolicypreviewpaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: LifecyclePolicyPreviewFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetLifecyclePolicyPreviewResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.GetLifecyclePolicyPreview.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#getlifecyclepolicypreviewpaginator)
         """
 
-
 class ListImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.ListImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#listimagespaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         filter: ListImagesFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.ListImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#listimagespaginator)
         """
```

### Comparing `mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/paginator.pyi` & `mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/paginator.py`

 * *Files 18% similar despite different names*

```diff
@@ -52,128 +52,136 @@
     "DescribeImagesPaginator",
     "DescribePullThroughCacheRulesPaginator",
     "DescribeRepositoriesPaginator",
     "GetLifecyclePolicyPreviewPaginator",
     "ListImagesPaginator",
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
 class DescribeImageScanFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImageScanFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describeimagescanfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         imageId: ImageIdentifierTypeDef,
         registryId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeImageScanFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImageScanFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describeimagescanfindingspaginator)
         """
 
+
 class DescribeImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describeimagespaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: DescribeImagesFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describeimagespaginator)
         """
 
+
 class DescribePullThroughCacheRulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribePullThroughCacheRules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describepullthroughcacherulespaginator)
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         ecrRepositoryPrefixes: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribePullThroughCacheRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribePullThroughCacheRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describepullthroughcacherulespaginator)
         """
 
+
 class DescribeRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describerepositoriespaginator)
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#describerepositoriespaginator)
         """
 
+
 class GetLifecyclePolicyPreviewPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.GetLifecyclePolicyPreview)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#getlifecyclepolicypreviewpaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: LifecyclePolicyPreviewFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetLifecyclePolicyPreviewResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.GetLifecyclePolicyPreview.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#getlifecyclepolicypreviewpaginator)
         """
 
+
 class ListImagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.ListImages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#listimagespaginator)
     """
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         filter: ListImagesFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.ListImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/paginators/#listimagespaginator)
         """
```

### Comparing `mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/type_defs.py` & `mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,101 +45,101 @@
 __all__ = (
     "AttributeTypeDef",
     "AuthorizationDataTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
-    "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
     "BatchGetRepositoryScanningConfigurationRequestRequestTypeDef",
     "RepositoryScanningConfigurationFailureTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
+    "CompleteLayerUploadResponseTypeDef",
     "CreatePullThroughCacheRuleRequestRequestTypeDef",
+    "CreatePullThroughCacheRuleResponseTypeDef",
     "EncryptionConfigurationTypeDef",
     "ImageScanningConfigurationTypeDef",
     "TagTypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DeleteLifecyclePolicyRequestRequestTypeDef",
+    "DeleteLifecyclePolicyResponseTypeDef",
     "DeletePullThroughCacheRuleRequestRequestTypeDef",
+    "DeletePullThroughCacheRuleResponseTypeDef",
+    "DeleteRegistryPolicyResponseTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
+    "DeleteRepositoryPolicyResponseTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
     "ImageReplicationStatusTypeDef",
-    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "ImageScanStatusTypeDef",
     "DescribeImagesFilterTypeDef",
+    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
     "DescribePullThroughCacheRulesRequestRequestTypeDef",
     "PullThroughCacheRuleTypeDef",
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeRepositoriesRequestRequestTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
     "GetDownloadUrlForLayerRequestRequestTypeDef",
+    "GetDownloadUrlForLayerResponseTypeDef",
     "LifecyclePolicyPreviewFilterTypeDef",
     "LifecyclePolicyPreviewSummaryTypeDef",
     "GetLifecyclePolicyRequestRequestTypeDef",
+    "GetLifecyclePolicyResponseTypeDef",
+    "GetRegistryPolicyResponseTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
+    "GetRepositoryPolicyResponseTypeDef",
     "ImageScanFindingsSummaryTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
+    "InitiateLayerUploadResponseTypeDef",
     "LifecyclePolicyRuleActionTypeDef",
     "ListImagesFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "VulnerablePackageTypeDef",
+    "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutImageTagMutabilityRequestRequestTypeDef",
+    "PutImageTagMutabilityResponseTypeDef",
     "PutLifecyclePolicyRequestRequestTypeDef",
+    "PutLifecyclePolicyResponseTypeDef",
     "PutRegistryPolicyRequestRequestTypeDef",
+    "PutRegistryPolicyResponseTypeDef",
     "RecommendationTypeDef",
     "ScanningRepositoryFilterTypeDef",
     "ReplicationDestinationTypeDef",
     "RepositoryFilterTypeDef",
+    "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
+    "SetRepositoryPolicyResponseTypeDef",
     "StartLifecyclePolicyPreviewRequestRequestTypeDef",
+    "StartLifecyclePolicyPreviewResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UploadLayerPartRequestRequestTypeDef",
+    "UploadLayerPartResponseTypeDef",
     "ImageScanFindingTypeDef",
+    "GetAuthorizationTokenResponseTypeDef",
     "ResourceDetailsTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
-    "CompleteLayerUploadResponseTypeDef",
-    "CreatePullThroughCacheRuleResponseTypeDef",
-    "DeleteLifecyclePolicyResponseTypeDef",
-    "DeletePullThroughCacheRuleResponseTypeDef",
-    "DeleteRegistryPolicyResponseTypeDef",
-    "DeleteRepositoryPolicyResponseTypeDef",
-    "GetAuthorizationTokenResponseTypeDef",
-    "GetDownloadUrlForLayerResponseTypeDef",
-    "GetLifecyclePolicyResponseTypeDef",
-    "GetRegistryPolicyResponseTypeDef",
-    "GetRepositoryPolicyResponseTypeDef",
-    "InitiateLayerUploadResponseTypeDef",
-    "PutImageTagMutabilityResponseTypeDef",
-    "PutLifecyclePolicyResponseTypeDef",
-    "PutRegistryPolicyResponseTypeDef",
-    "SetRepositoryPolicyResponseTypeDef",
-    "StartLifecyclePolicyPreviewResponseTypeDef",
-    "UploadLayerPartResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
     "BatchGetImageRequestRequestTypeDef",
     "DescribeImageReplicationStatusRequestRequestTypeDef",
+    "DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
     "DescribeImageScanFindingsRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "ListImagesResponseTypeDef",
     "StartImageScanRequestRequestTypeDef",
     "PutImageScanningConfigurationRequestRequestTypeDef",
     "PutImageScanningConfigurationResponseTypeDef",
     "RepositoryTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CvssScoreDetailsTypeDef",
     "DescribeImageReplicationStatusResponseTypeDef",
-    "DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
-    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
     "StartImageScanResponseTypeDef",
     "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "DescribePullThroughCacheRulesResponseTypeDef",
     "GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     "GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef",
@@ -261,25 +261,14 @@
         "layerAvailability": LayerAvailabilityType,
         "layerSize": int,
         "mediaType": str,
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
 ImageIdentifierTypeDef = TypedDict(
     "ImageIdentifierTypeDef",
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
@@ -322,14 +311,25 @@
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
 
+CompleteLayerUploadResponseTypeDef = TypedDict(
+    "CompleteLayerUploadResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "layerDigest": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreatePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePullThroughCacheRuleRequestRequestTypeDef",
     {
         "ecrRepositoryPrefix": str,
         "upstreamRegistryUrl": str,
     },
 )
@@ -345,14 +345,25 @@
 class CreatePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredCreatePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalCreatePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
 
+CreatePullThroughCacheRuleResponseTypeDef = TypedDict(
+    "CreatePullThroughCacheRuleResponseTypeDef",
+    {
+        "ecrRepositoryPrefix": str,
+        "upstreamRegistryUrl": str,
+        "createdAt": datetime,
+        "registryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEncryptionConfigurationTypeDef = TypedDict(
     "_RequiredEncryptionConfigurationTypeDef",
     {
         "encryptionType": EncryptionTypeType,
     },
 )
 _OptionalEncryptionConfigurationTypeDef = TypedDict(
@@ -425,14 +436,25 @@
 class DeleteLifecyclePolicyRequestRequestTypeDef(
     _RequiredDeleteLifecyclePolicyRequestRequestTypeDef,
     _OptionalDeleteLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
 
+DeleteLifecyclePolicyResponseTypeDef = TypedDict(
+    "DeleteLifecyclePolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "lastEvaluatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeletePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePullThroughCacheRuleRequestRequestTypeDef",
     {
         "ecrRepositoryPrefix": str,
     },
 )
 _OptionalDeletePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
@@ -447,14 +469,34 @@
 class DeletePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredDeletePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalDeletePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
 
+DeletePullThroughCacheRuleResponseTypeDef = TypedDict(
+    "DeletePullThroughCacheRuleResponseTypeDef",
+    {
+        "ecrRepositoryPrefix": str,
+        "upstreamRegistryUrl": str,
+        "createdAt": datetime,
+        "registryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteRegistryPolicyResponseTypeDef = TypedDict(
+    "DeleteRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDeleteRepositoryPolicyRequestRequestTypeDef = TypedDict(
@@ -469,14 +511,24 @@
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
 
+DeleteRepositoryPolicyResponseTypeDef = TypedDict(
+    "DeleteRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDeleteRepositoryRequestRequestTypeDef = TypedDict(
@@ -502,24 +554,14 @@
         "registryId": str,
         "status": ReplicationStatusType,
         "failureCode": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -538,14 +580,24 @@
     "DescribeImagesFilterTypeDef",
     {
         "tagStatus": TagStatusType,
     },
     total=False,
 )
 
+DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef = TypedDict(
+    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
+    {
+        "registryId": str,
+        "ecrRepositoryPrefixes": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribePullThroughCacheRulesRequestRequestTypeDef = TypedDict(
     "DescribePullThroughCacheRulesRequestRequestTypeDef",
     {
         "registryId": str,
         "ecrRepositoryPrefixes": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -560,14 +612,24 @@
         "upstreamRegistryUrl": str,
         "createdAt": datetime,
         "registryId": str,
     },
     total=False,
 )
 
+DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
+    {
+        "registryId": str,
+        "repositoryNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeRepositoriesRequestRequestTypeDef = TypedDict(
     "DescribeRepositoriesRequestRequestTypeDef",
     {
         "registryId": str,
         "repositoryNames": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -602,14 +664,23 @@
 class GetDownloadUrlForLayerRequestRequestTypeDef(
     _RequiredGetDownloadUrlForLayerRequestRequestTypeDef,
     _OptionalGetDownloadUrlForLayerRequestRequestTypeDef,
 ):
     pass
 
 
+GetDownloadUrlForLayerResponseTypeDef = TypedDict(
+    "GetDownloadUrlForLayerResponseTypeDef",
+    {
+        "downloadUrl": str,
+        "layerDigest": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LifecyclePolicyPreviewFilterTypeDef = TypedDict(
     "LifecyclePolicyPreviewFilterTypeDef",
     {
         "tagStatus": TagStatusType,
     },
     total=False,
 )
@@ -640,14 +711,34 @@
 class GetLifecyclePolicyRequestRequestTypeDef(
     _RequiredGetLifecyclePolicyRequestRequestTypeDef,
     _OptionalGetLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
 
+GetLifecyclePolicyResponseTypeDef = TypedDict(
+    "GetLifecyclePolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "lastEvaluatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetRegistryPolicyResponseTypeDef = TypedDict(
+    "GetRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
@@ -662,14 +753,24 @@
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
 
+GetRepositoryPolicyResponseTypeDef = TypedDict(
+    "GetRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ImageScanFindingsSummaryTypeDef = TypedDict(
     "ImageScanFindingsSummaryTypeDef",
     {
         "imageScanCompletedAt": datetime,
         "vulnerabilitySourceUpdatedAt": datetime,
         "findingSeverityCounts": Dict[FindingSeverityType, int],
     },
@@ -694,14 +795,23 @@
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
 
+InitiateLayerUploadResponseTypeDef = TypedDict(
+    "InitiateLayerUploadResponseTypeDef",
+    {
+        "uploadId": str,
+        "partSize": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LifecyclePolicyRuleActionTypeDef = TypedDict(
     "LifecyclePolicyRuleActionTypeDef",
     {
         "type": Literal["EXPIRE"],
     },
     total=False,
 )
@@ -732,14 +842,24 @@
         "release": str,
         "sourceLayerHash": str,
         "version": str,
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
 _RequiredPutImageRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageManifest": str,
     },
 )
@@ -780,14 +900,24 @@
 class PutImageTagMutabilityRequestRequestTypeDef(
     _RequiredPutImageTagMutabilityRequestRequestTypeDef,
     _OptionalPutImageTagMutabilityRequestRequestTypeDef,
 ):
     pass
 
 
+PutImageTagMutabilityResponseTypeDef = TypedDict(
+    "PutImageTagMutabilityResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "imageTagMutability": ImageTagMutabilityType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutLifecyclePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutLifecyclePolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "lifecyclePolicyText": str,
     },
 )
@@ -803,21 +933,40 @@
 class PutLifecyclePolicyRequestRequestTypeDef(
     _RequiredPutLifecyclePolicyRequestRequestTypeDef,
     _OptionalPutLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
 
+PutLifecyclePolicyResponseTypeDef = TypedDict(
+    "PutLifecyclePolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutRegistryPolicyRequestRequestTypeDef = TypedDict(
     "PutRegistryPolicyRequestRequestTypeDef",
     {
         "policyText": str,
     },
 )
 
+PutRegistryPolicyResponseTypeDef = TypedDict(
+    "PutRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "url": str,
         "text": str,
     },
     total=False,
@@ -843,14 +992,25 @@
     "RepositoryFilterTypeDef",
     {
         "filter": str,
         "filterType": Literal["PREFIX_MATCH"],
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
 _RequiredSetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "policyText": str,
     },
 )
@@ -867,14 +1027,24 @@
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
 
+SetRepositoryPolicyResponseTypeDef = TypedDict(
+    "SetRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalStartLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
@@ -890,14 +1060,25 @@
 class StartLifecyclePolicyPreviewRequestRequestTypeDef(
     _RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef,
     _OptionalStartLifecyclePolicyPreviewRequestRequestTypeDef,
 ):
     pass
 
 
+StartLifecyclePolicyPreviewResponseTypeDef = TypedDict(
+    "StartLifecyclePolicyPreviewResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "status": LifecyclePolicyPreviewStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -923,220 +1104,59 @@
 
 class UploadLayerPartRequestRequestTypeDef(
     _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
 
+UploadLayerPartResponseTypeDef = TypedDict(
+    "UploadLayerPartResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "lastByteReceived": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ImageScanFindingTypeDef = TypedDict(
     "ImageScanFindingTypeDef",
     {
         "name": str,
         "description": str,
         "uri": str,
         "severity": FindingSeverityType,
         "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
+GetAuthorizationTokenResponseTypeDef = TypedDict(
+    "GetAuthorizationTokenResponseTypeDef",
+    {
+        "authorizationData": List[AuthorizationDataTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "awsEcrContainerImage": AwsEcrContainerImageDetailsTypeDef,
     },
     total=False,
 )
 
 BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
     "BatchCheckLayerAvailabilityResponseTypeDef",
     {
         "layers": List[LayerTypeDef],
         "failures": List[LayerFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CompleteLayerUploadResponseTypeDef = TypedDict(
-    "CompleteLayerUploadResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "layerDigest": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePullThroughCacheRuleResponseTypeDef = TypedDict(
-    "CreatePullThroughCacheRuleResponseTypeDef",
-    {
-        "ecrRepositoryPrefix": str,
-        "upstreamRegistryUrl": str,
-        "createdAt": datetime,
-        "registryId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteLifecyclePolicyResponseTypeDef = TypedDict(
-    "DeleteLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "lastEvaluatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePullThroughCacheRuleResponseTypeDef = TypedDict(
-    "DeletePullThroughCacheRuleResponseTypeDef",
-    {
-        "ecrRepositoryPrefix": str,
-        "upstreamRegistryUrl": str,
-        "createdAt": datetime,
-        "registryId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteRegistryPolicyResponseTypeDef = TypedDict(
-    "DeleteRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteRepositoryPolicyResponseTypeDef = TypedDict(
-    "DeleteRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAuthorizationTokenResponseTypeDef = TypedDict(
-    "GetAuthorizationTokenResponseTypeDef",
-    {
-        "authorizationData": List[AuthorizationDataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDownloadUrlForLayerResponseTypeDef = TypedDict(
-    "GetDownloadUrlForLayerResponseTypeDef",
-    {
-        "downloadUrl": str,
-        "layerDigest": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLifecyclePolicyResponseTypeDef = TypedDict(
-    "GetLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "lastEvaluatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRegistryPolicyResponseTypeDef = TypedDict(
-    "GetRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRepositoryPolicyResponseTypeDef = TypedDict(
-    "GetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InitiateLayerUploadResponseTypeDef = TypedDict(
-    "InitiateLayerUploadResponseTypeDef",
-    {
-        "uploadId": str,
-        "partSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutImageTagMutabilityResponseTypeDef = TypedDict(
-    "PutImageTagMutabilityResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "imageTagMutability": ImageTagMutabilityType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutLifecyclePolicyResponseTypeDef = TypedDict(
-    "PutLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutRegistryPolicyResponseTypeDef = TypedDict(
-    "PutRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetRepositoryPolicyResponseTypeDef = TypedDict(
-    "SetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartLifecyclePolicyPreviewResponseTypeDef = TypedDict(
-    "StartLifecyclePolicyPreviewResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "status": LifecyclePolicyPreviewStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UploadLayerPartResponseTypeDef = TypedDict(
-    "UploadLayerPartResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "lastByteReceived": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteImageRequestRequestTypeDef",
     {
         "repositoryName": str,
@@ -1200,14 +1220,38 @@
 class DescribeImageReplicationStatusRequestRequestTypeDef(
     _RequiredDescribeImageReplicationStatusRequestRequestTypeDef,
     _OptionalDescribeImageReplicationStatusRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "imageId": ImageIdentifierTypeDef,
+    },
+)
+_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    {
+        "registryId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef(
+    _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+    _OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeImageScanFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1252,15 +1296,15 @@
 )
 
 ListImagesResponseTypeDef = TypedDict(
     "ListImagesResponseTypeDef",
     {
         "imageIds": List[ImageIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartImageScanRequestRequestTypeDef = TypedDict(
     "_RequiredStartImageScanRequestRequestTypeDef",
     {
         "repositoryName": str,
@@ -1307,15 +1351,15 @@
 
 PutImageScanningConfigurationResponseTypeDef = TypedDict(
     "PutImageScanningConfigurationResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RepositoryTypeDef = TypedDict(
     "RepositoryTypeDef",
     {
         "repositoryArn": str,
@@ -1355,15 +1399,15 @@
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1385,62 +1429,18 @@
 
 DescribeImageReplicationStatusResponseTypeDef = TypedDict(
     "DescribeImageReplicationStatusResponseTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
         "replicationStatuses": List[ImageReplicationStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
-    },
-)
-_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
-    {
-        "registryId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef(
-    _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
-    _OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
-):
-    pass
-
-
-DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef = TypedDict(
-    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
-    {
-        "registryId": str,
-        "ecrRepositoryPrefixes": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
-    {
-        "registryId": str,
-        "repositoryNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1466,15 +1466,15 @@
 StartImageScanResponseTypeDef = TypedDict(
     "StartImageScanResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "repositoryName": str,
@@ -1482,15 +1482,15 @@
 )
 _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "registryId": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": DescribeImagesFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class DescribeImagesRequestDescribeImagesPaginateTypeDef(
     _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
@@ -1525,15 +1525,15 @@
 
 
 DescribePullThroughCacheRulesResponseTypeDef = TypedDict(
     "DescribePullThroughCacheRulesResponseTypeDef",
     {
         "pullThroughCacheRules": List[PullThroughCacheRuleTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     {
         "repositoryName": str,
@@ -1541,15 +1541,15 @@
 )
 _OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef = TypedDict(
     "_OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     {
         "registryId": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": LifecyclePolicyPreviewFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
@@ -1648,15 +1648,15 @@
     },
 )
 _OptionalListImagesRequestListImagesPaginateTypeDef = TypedDict(
     "_OptionalListImagesRequestListImagesPaginateTypeDef",
     {
         "registryId": str,
         "filter": ListImagesFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListImagesRequestListImagesPaginateTypeDef(
     _RequiredListImagesRequestListImagesPaginateTypeDef,
@@ -1765,57 +1765,57 @@
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
         "imageIds": List[ImageIdentifierTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetImageResponseTypeDef = TypedDict(
     "BatchGetImageResponseTypeDef",
     {
         "images": List[ImageTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutImageResponseTypeDef = TypedDict(
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRepositoryResponseTypeDef = TypedDict(
     "CreateRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRepositoryResponseTypeDef = TypedDict(
     "DeleteRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRepositoriesResponseTypeDef = TypedDict(
     "DescribeRepositoriesResponseTypeDef",
     {
         "repositories": List[RepositoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScoreDetailsTypeDef = TypedDict(
     "ScoreDetailsTypeDef",
     {
         "cvss": CvssScoreDetailsTypeDef,
@@ -1824,29 +1824,29 @@
 )
 
 DescribeImagesResponseTypeDef = TypedDict(
     "DescribeImagesResponseTypeDef",
     {
         "imageDetails": List[ImageDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLifecyclePolicyPreviewResponseTypeDef = TypedDict(
     "GetLifecyclePolicyPreviewResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "status": LifecyclePolicyPreviewStatusType,
         "nextToken": str,
         "previewResults": List[LifecyclePolicyPreviewResultTypeDef],
         "summary": LifecyclePolicyPreviewSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
     "PutRegistryScanningConfigurationRequestRequestTypeDef",
     {
         "scanType": ScanTypeType,
@@ -1865,15 +1865,15 @@
 )
 
 BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     {
         "scanningConfigurations": List[RepositoryScanningConfigurationTypeDef],
         "failures": List[RepositoryScanningConfigurationFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
         "rules": List[ReplicationRuleTypeDef],
@@ -1903,47 +1903,47 @@
 )
 
 GetRegistryScanningConfigurationResponseTypeDef = TypedDict(
     "GetRegistryScanningConfigurationResponseTypeDef",
     {
         "registryId": str,
         "scanningConfiguration": RegistryScanningConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRegistryScanningConfigurationResponseTypeDef = TypedDict(
     "PutRegistryScanningConfigurationResponseTypeDef",
     {
         "registryScanningConfiguration": RegistryScanningConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRegistryResponseTypeDef = TypedDict(
     "DescribeRegistryResponseTypeDef",
     {
         "registryId": str,
         "replicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutReplicationConfigurationRequestRequestTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationTypeDef,
     },
 )
 
 PutReplicationConfigurationResponseTypeDef = TypedDict(
     "PutReplicationConfigurationResponseTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImageScanFindingsTypeDef = TypedDict(
     "ImageScanFindingsTypeDef",
     {
         "imageScanCompletedAt": datetime,
@@ -1960,10 +1960,10 @@
     {
         "registryId": str,
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
         "imageScanFindings": ImageScanFindingsTypeDef,
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/type_defs.pyi` & `mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -44,101 +44,101 @@
 __all__ = (
     "AttributeTypeDef",
     "AuthorizationDataTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
-    "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
     "BatchGetRepositoryScanningConfigurationRequestRequestTypeDef",
     "RepositoryScanningConfigurationFailureTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
+    "CompleteLayerUploadResponseTypeDef",
     "CreatePullThroughCacheRuleRequestRequestTypeDef",
+    "CreatePullThroughCacheRuleResponseTypeDef",
     "EncryptionConfigurationTypeDef",
     "ImageScanningConfigurationTypeDef",
     "TagTypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DeleteLifecyclePolicyRequestRequestTypeDef",
+    "DeleteLifecyclePolicyResponseTypeDef",
     "DeletePullThroughCacheRuleRequestRequestTypeDef",
+    "DeletePullThroughCacheRuleResponseTypeDef",
+    "DeleteRegistryPolicyResponseTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
+    "DeleteRepositoryPolicyResponseTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
     "ImageReplicationStatusTypeDef",
-    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "ImageScanStatusTypeDef",
     "DescribeImagesFilterTypeDef",
+    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
     "DescribePullThroughCacheRulesRequestRequestTypeDef",
     "PullThroughCacheRuleTypeDef",
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeRepositoriesRequestRequestTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
     "GetDownloadUrlForLayerRequestRequestTypeDef",
+    "GetDownloadUrlForLayerResponseTypeDef",
     "LifecyclePolicyPreviewFilterTypeDef",
     "LifecyclePolicyPreviewSummaryTypeDef",
     "GetLifecyclePolicyRequestRequestTypeDef",
+    "GetLifecyclePolicyResponseTypeDef",
+    "GetRegistryPolicyResponseTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
+    "GetRepositoryPolicyResponseTypeDef",
     "ImageScanFindingsSummaryTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
+    "InitiateLayerUploadResponseTypeDef",
     "LifecyclePolicyRuleActionTypeDef",
     "ListImagesFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "VulnerablePackageTypeDef",
+    "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutImageTagMutabilityRequestRequestTypeDef",
+    "PutImageTagMutabilityResponseTypeDef",
     "PutLifecyclePolicyRequestRequestTypeDef",
+    "PutLifecyclePolicyResponseTypeDef",
     "PutRegistryPolicyRequestRequestTypeDef",
+    "PutRegistryPolicyResponseTypeDef",
     "RecommendationTypeDef",
     "ScanningRepositoryFilterTypeDef",
     "ReplicationDestinationTypeDef",
     "RepositoryFilterTypeDef",
+    "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
+    "SetRepositoryPolicyResponseTypeDef",
     "StartLifecyclePolicyPreviewRequestRequestTypeDef",
+    "StartLifecyclePolicyPreviewResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UploadLayerPartRequestRequestTypeDef",
+    "UploadLayerPartResponseTypeDef",
     "ImageScanFindingTypeDef",
+    "GetAuthorizationTokenResponseTypeDef",
     "ResourceDetailsTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
-    "CompleteLayerUploadResponseTypeDef",
-    "CreatePullThroughCacheRuleResponseTypeDef",
-    "DeleteLifecyclePolicyResponseTypeDef",
-    "DeletePullThroughCacheRuleResponseTypeDef",
-    "DeleteRegistryPolicyResponseTypeDef",
-    "DeleteRepositoryPolicyResponseTypeDef",
-    "GetAuthorizationTokenResponseTypeDef",
-    "GetDownloadUrlForLayerResponseTypeDef",
-    "GetLifecyclePolicyResponseTypeDef",
-    "GetRegistryPolicyResponseTypeDef",
-    "GetRepositoryPolicyResponseTypeDef",
-    "InitiateLayerUploadResponseTypeDef",
-    "PutImageTagMutabilityResponseTypeDef",
-    "PutLifecyclePolicyResponseTypeDef",
-    "PutRegistryPolicyResponseTypeDef",
-    "SetRepositoryPolicyResponseTypeDef",
-    "StartLifecyclePolicyPreviewResponseTypeDef",
-    "UploadLayerPartResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
     "BatchGetImageRequestRequestTypeDef",
     "DescribeImageReplicationStatusRequestRequestTypeDef",
+    "DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
     "DescribeImageScanFindingsRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "ListImagesResponseTypeDef",
     "StartImageScanRequestRequestTypeDef",
     "PutImageScanningConfigurationRequestRequestTypeDef",
     "PutImageScanningConfigurationResponseTypeDef",
     "RepositoryTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CvssScoreDetailsTypeDef",
     "DescribeImageReplicationStatusResponseTypeDef",
-    "DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
-    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
     "StartImageScanResponseTypeDef",
     "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "DescribePullThroughCacheRulesResponseTypeDef",
     "GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     "GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef",
@@ -256,25 +256,14 @@
         "layerAvailability": LayerAvailabilityType,
         "layerSize": int,
         "mediaType": str,
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
 ImageIdentifierTypeDef = TypedDict(
     "ImageIdentifierTypeDef",
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
@@ -315,14 +304,25 @@
 
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
+CompleteLayerUploadResponseTypeDef = TypedDict(
+    "CompleteLayerUploadResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "layerDigest": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreatePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePullThroughCacheRuleRequestRequestTypeDef",
     {
         "ecrRepositoryPrefix": str,
         "upstreamRegistryUrl": str,
     },
 )
@@ -336,14 +336,25 @@
 
 class CreatePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredCreatePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalCreatePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
+CreatePullThroughCacheRuleResponseTypeDef = TypedDict(
+    "CreatePullThroughCacheRuleResponseTypeDef",
+    {
+        "ecrRepositoryPrefix": str,
+        "upstreamRegistryUrl": str,
+        "createdAt": datetime,
+        "registryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredEncryptionConfigurationTypeDef = TypedDict(
     "_RequiredEncryptionConfigurationTypeDef",
     {
         "encryptionType": EncryptionTypeType,
     },
 )
 _OptionalEncryptionConfigurationTypeDef = TypedDict(
@@ -412,14 +423,25 @@
 
 class DeleteLifecyclePolicyRequestRequestTypeDef(
     _RequiredDeleteLifecyclePolicyRequestRequestTypeDef,
     _OptionalDeleteLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
+DeleteLifecyclePolicyResponseTypeDef = TypedDict(
+    "DeleteLifecyclePolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "lastEvaluatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeletePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePullThroughCacheRuleRequestRequestTypeDef",
     {
         "ecrRepositoryPrefix": str,
     },
 )
 _OptionalDeletePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
@@ -432,14 +454,34 @@
 
 class DeletePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredDeletePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalDeletePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
+DeletePullThroughCacheRuleResponseTypeDef = TypedDict(
+    "DeletePullThroughCacheRuleResponseTypeDef",
+    {
+        "ecrRepositoryPrefix": str,
+        "upstreamRegistryUrl": str,
+        "createdAt": datetime,
+        "registryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteRegistryPolicyResponseTypeDef = TypedDict(
+    "DeleteRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDeleteRepositoryPolicyRequestRequestTypeDef = TypedDict(
@@ -452,14 +494,24 @@
 
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
+DeleteRepositoryPolicyResponseTypeDef = TypedDict(
+    "DeleteRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDeleteRepositoryRequestRequestTypeDef = TypedDict(
@@ -483,24 +535,14 @@
         "registryId": str,
         "status": ReplicationStatusType,
         "failureCode": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -519,14 +561,24 @@
     "DescribeImagesFilterTypeDef",
     {
         "tagStatus": TagStatusType,
     },
     total=False,
 )
 
+DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef = TypedDict(
+    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
+    {
+        "registryId": str,
+        "ecrRepositoryPrefixes": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribePullThroughCacheRulesRequestRequestTypeDef = TypedDict(
     "DescribePullThroughCacheRulesRequestRequestTypeDef",
     {
         "registryId": str,
         "ecrRepositoryPrefixes": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -541,14 +593,24 @@
         "upstreamRegistryUrl": str,
         "createdAt": datetime,
         "registryId": str,
     },
     total=False,
 )
 
+DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
+    {
+        "registryId": str,
+        "repositoryNames": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeRepositoriesRequestRequestTypeDef = TypedDict(
     "DescribeRepositoriesRequestRequestTypeDef",
     {
         "registryId": str,
         "repositoryNames": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -581,14 +643,23 @@
 
 class GetDownloadUrlForLayerRequestRequestTypeDef(
     _RequiredGetDownloadUrlForLayerRequestRequestTypeDef,
     _OptionalGetDownloadUrlForLayerRequestRequestTypeDef,
 ):
     pass
 
+GetDownloadUrlForLayerResponseTypeDef = TypedDict(
+    "GetDownloadUrlForLayerResponseTypeDef",
+    {
+        "downloadUrl": str,
+        "layerDigest": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LifecyclePolicyPreviewFilterTypeDef = TypedDict(
     "LifecyclePolicyPreviewFilterTypeDef",
     {
         "tagStatus": TagStatusType,
     },
     total=False,
 )
@@ -617,14 +688,34 @@
 
 class GetLifecyclePolicyRequestRequestTypeDef(
     _RequiredGetLifecyclePolicyRequestRequestTypeDef,
     _OptionalGetLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
+GetLifecyclePolicyResponseTypeDef = TypedDict(
+    "GetLifecyclePolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "lastEvaluatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetRegistryPolicyResponseTypeDef = TypedDict(
+    "GetRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
@@ -637,14 +728,24 @@
 
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
+GetRepositoryPolicyResponseTypeDef = TypedDict(
+    "GetRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ImageScanFindingsSummaryTypeDef = TypedDict(
     "ImageScanFindingsSummaryTypeDef",
     {
         "imageScanCompletedAt": datetime,
         "vulnerabilitySourceUpdatedAt": datetime,
         "findingSeverityCounts": Dict[FindingSeverityType, int],
     },
@@ -667,14 +768,23 @@
 
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
+InitiateLayerUploadResponseTypeDef = TypedDict(
+    "InitiateLayerUploadResponseTypeDef",
+    {
+        "uploadId": str,
+        "partSize": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 LifecyclePolicyRuleActionTypeDef = TypedDict(
     "LifecyclePolicyRuleActionTypeDef",
     {
         "type": Literal["EXPIRE"],
     },
     total=False,
 )
@@ -705,14 +815,24 @@
         "release": str,
         "sourceLayerHash": str,
         "version": str,
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
 _RequiredPutImageRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageManifest": str,
     },
 )
@@ -749,14 +869,24 @@
 
 class PutImageTagMutabilityRequestRequestTypeDef(
     _RequiredPutImageTagMutabilityRequestRequestTypeDef,
     _OptionalPutImageTagMutabilityRequestRequestTypeDef,
 ):
     pass
 
+PutImageTagMutabilityResponseTypeDef = TypedDict(
+    "PutImageTagMutabilityResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "imageTagMutability": ImageTagMutabilityType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutLifecyclePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutLifecyclePolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "lifecyclePolicyText": str,
     },
 )
@@ -770,21 +900,40 @@
 
 class PutLifecyclePolicyRequestRequestTypeDef(
     _RequiredPutLifecyclePolicyRequestRequestTypeDef,
     _OptionalPutLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
+PutLifecyclePolicyResponseTypeDef = TypedDict(
+    "PutLifecyclePolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutRegistryPolicyRequestRequestTypeDef = TypedDict(
     "PutRegistryPolicyRequestRequestTypeDef",
     {
         "policyText": str,
     },
 )
 
+PutRegistryPolicyResponseTypeDef = TypedDict(
+    "PutRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "url": str,
         "text": str,
     },
     total=False,
@@ -810,14 +959,25 @@
     "RepositoryFilterTypeDef",
     {
         "filter": str,
         "filterType": Literal["PREFIX_MATCH"],
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
 _RequiredSetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "policyText": str,
     },
 )
@@ -832,14 +992,24 @@
 
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
+SetRepositoryPolicyResponseTypeDef = TypedDict(
+    "SetRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalStartLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
@@ -853,14 +1023,25 @@
 
 class StartLifecyclePolicyPreviewRequestRequestTypeDef(
     _RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef,
     _OptionalStartLifecyclePolicyPreviewRequestRequestTypeDef,
 ):
     pass
 
+StartLifecyclePolicyPreviewResponseTypeDef = TypedDict(
+    "StartLifecyclePolicyPreviewResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "status": LifecyclePolicyPreviewStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -884,220 +1065,59 @@
 )
 
 class UploadLayerPartRequestRequestTypeDef(
     _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
+UploadLayerPartResponseTypeDef = TypedDict(
+    "UploadLayerPartResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "lastByteReceived": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ImageScanFindingTypeDef = TypedDict(
     "ImageScanFindingTypeDef",
     {
         "name": str,
         "description": str,
         "uri": str,
         "severity": FindingSeverityType,
         "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
+GetAuthorizationTokenResponseTypeDef = TypedDict(
+    "GetAuthorizationTokenResponseTypeDef",
+    {
+        "authorizationData": List[AuthorizationDataTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "awsEcrContainerImage": AwsEcrContainerImageDetailsTypeDef,
     },
     total=False,
 )
 
 BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
     "BatchCheckLayerAvailabilityResponseTypeDef",
     {
         "layers": List[LayerTypeDef],
         "failures": List[LayerFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CompleteLayerUploadResponseTypeDef = TypedDict(
-    "CompleteLayerUploadResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "layerDigest": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePullThroughCacheRuleResponseTypeDef = TypedDict(
-    "CreatePullThroughCacheRuleResponseTypeDef",
-    {
-        "ecrRepositoryPrefix": str,
-        "upstreamRegistryUrl": str,
-        "createdAt": datetime,
-        "registryId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteLifecyclePolicyResponseTypeDef = TypedDict(
-    "DeleteLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "lastEvaluatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePullThroughCacheRuleResponseTypeDef = TypedDict(
-    "DeletePullThroughCacheRuleResponseTypeDef",
-    {
-        "ecrRepositoryPrefix": str,
-        "upstreamRegistryUrl": str,
-        "createdAt": datetime,
-        "registryId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteRegistryPolicyResponseTypeDef = TypedDict(
-    "DeleteRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteRepositoryPolicyResponseTypeDef = TypedDict(
-    "DeleteRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAuthorizationTokenResponseTypeDef = TypedDict(
-    "GetAuthorizationTokenResponseTypeDef",
-    {
-        "authorizationData": List[AuthorizationDataTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDownloadUrlForLayerResponseTypeDef = TypedDict(
-    "GetDownloadUrlForLayerResponseTypeDef",
-    {
-        "downloadUrl": str,
-        "layerDigest": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLifecyclePolicyResponseTypeDef = TypedDict(
-    "GetLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "lastEvaluatedAt": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRegistryPolicyResponseTypeDef = TypedDict(
-    "GetRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRepositoryPolicyResponseTypeDef = TypedDict(
-    "GetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InitiateLayerUploadResponseTypeDef = TypedDict(
-    "InitiateLayerUploadResponseTypeDef",
-    {
-        "uploadId": str,
-        "partSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutImageTagMutabilityResponseTypeDef = TypedDict(
-    "PutImageTagMutabilityResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "imageTagMutability": ImageTagMutabilityType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutLifecyclePolicyResponseTypeDef = TypedDict(
-    "PutLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutRegistryPolicyResponseTypeDef = TypedDict(
-    "PutRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SetRepositoryPolicyResponseTypeDef = TypedDict(
-    "SetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartLifecyclePolicyPreviewResponseTypeDef = TypedDict(
-    "StartLifecyclePolicyPreviewResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "status": LifecyclePolicyPreviewStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UploadLayerPartResponseTypeDef = TypedDict(
-    "UploadLayerPartResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "lastByteReceived": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteImageRequestRequestTypeDef",
     {
         "repositoryName": str,
@@ -1155,14 +1175,36 @@
 
 class DescribeImageReplicationStatusRequestRequestTypeDef(
     _RequiredDescribeImageReplicationStatusRequestRequestTypeDef,
     _OptionalDescribeImageReplicationStatusRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "imageId": ImageIdentifierTypeDef,
+    },
+)
+_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    {
+        "registryId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef(
+    _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+    _OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeImageScanFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1205,15 +1247,15 @@
 )
 
 ListImagesResponseTypeDef = TypedDict(
     "ListImagesResponseTypeDef",
     {
         "imageIds": List[ImageIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartImageScanRequestRequestTypeDef = TypedDict(
     "_RequiredStartImageScanRequestRequestTypeDef",
     {
         "repositoryName": str,
@@ -1256,15 +1298,15 @@
 
 PutImageScanningConfigurationResponseTypeDef = TypedDict(
     "PutImageScanningConfigurationResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RepositoryTypeDef = TypedDict(
     "RepositoryTypeDef",
     {
         "repositoryArn": str,
@@ -1302,15 +1344,15 @@
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1332,60 +1374,18 @@
 
 DescribeImageReplicationStatusResponseTypeDef = TypedDict(
     "DescribeImageReplicationStatusResponseTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
         "replicationStatuses": List[ImageReplicationStatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
-    },
-)
-_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
-    {
-        "registryId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef(
-    _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
-    _OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
-):
-    pass
-
-DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef = TypedDict(
-    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
-    {
-        "registryId": str,
-        "ecrRepositoryPrefixes": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
-    {
-        "registryId": str,
-        "repositoryNames": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1409,15 +1409,15 @@
 StartImageScanResponseTypeDef = TypedDict(
     "StartImageScanResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "repositoryName": str,
@@ -1425,15 +1425,15 @@
 )
 _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "registryId": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": DescribeImagesFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class DescribeImagesRequestDescribeImagesPaginateTypeDef(
     _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
     _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
@@ -1464,15 +1464,15 @@
     pass
 
 DescribePullThroughCacheRulesResponseTypeDef = TypedDict(
     "DescribePullThroughCacheRulesResponseTypeDef",
     {
         "pullThroughCacheRules": List[PullThroughCacheRuleTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     {
         "repositoryName": str,
@@ -1480,15 +1480,15 @@
 )
 _OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef = TypedDict(
     "_OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     {
         "registryId": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": LifecyclePolicyPreviewFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
@@ -1581,15 +1581,15 @@
     },
 )
 _OptionalListImagesRequestListImagesPaginateTypeDef = TypedDict(
     "_OptionalListImagesRequestListImagesPaginateTypeDef",
     {
         "registryId": str,
         "filter": ListImagesFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListImagesRequestListImagesPaginateTypeDef(
     _RequiredListImagesRequestListImagesPaginateTypeDef,
     _OptionalListImagesRequestListImagesPaginateTypeDef,
@@ -1692,57 +1692,57 @@
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
         "imageIds": List[ImageIdentifierTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetImageResponseTypeDef = TypedDict(
     "BatchGetImageResponseTypeDef",
     {
         "images": List[ImageTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutImageResponseTypeDef = TypedDict(
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateRepositoryResponseTypeDef = TypedDict(
     "CreateRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteRepositoryResponseTypeDef = TypedDict(
     "DeleteRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRepositoriesResponseTypeDef = TypedDict(
     "DescribeRepositoriesResponseTypeDef",
     {
         "repositories": List[RepositoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScoreDetailsTypeDef = TypedDict(
     "ScoreDetailsTypeDef",
     {
         "cvss": CvssScoreDetailsTypeDef,
@@ -1751,29 +1751,29 @@
 )
 
 DescribeImagesResponseTypeDef = TypedDict(
     "DescribeImagesResponseTypeDef",
     {
         "imageDetails": List[ImageDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLifecyclePolicyPreviewResponseTypeDef = TypedDict(
     "GetLifecyclePolicyPreviewResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "status": LifecyclePolicyPreviewStatusType,
         "nextToken": str,
         "previewResults": List[LifecyclePolicyPreviewResultTypeDef],
         "summary": LifecyclePolicyPreviewSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
     "PutRegistryScanningConfigurationRequestRequestTypeDef",
     {
         "scanType": ScanTypeType,
@@ -1792,15 +1792,15 @@
 )
 
 BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     {
         "scanningConfigurations": List[RepositoryScanningConfigurationTypeDef],
         "failures": List[RepositoryScanningConfigurationFailureTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
         "rules": List[ReplicationRuleTypeDef],
@@ -1830,47 +1830,47 @@
 )
 
 GetRegistryScanningConfigurationResponseTypeDef = TypedDict(
     "GetRegistryScanningConfigurationResponseTypeDef",
     {
         "registryId": str,
         "scanningConfiguration": RegistryScanningConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutRegistryScanningConfigurationResponseTypeDef = TypedDict(
     "PutRegistryScanningConfigurationResponseTypeDef",
     {
         "registryScanningConfiguration": RegistryScanningConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRegistryResponseTypeDef = TypedDict(
     "DescribeRegistryResponseTypeDef",
     {
         "registryId": str,
         "replicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutReplicationConfigurationRequestRequestTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationTypeDef,
     },
 )
 
 PutReplicationConfigurationResponseTypeDef = TypedDict(
     "PutReplicationConfigurationResponseTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImageScanFindingsTypeDef = TypedDict(
     "ImageScanFindingsTypeDef",
     {
         "imageScanCompletedAt": datetime,
@@ -1887,10 +1887,10 @@
     {
         "registryId": str,
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
         "imageScanFindings": ImageScanFindingsTypeDef,
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/waiter.py` & `mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr/waiter.pyi` & `mypy-boto3-ecr-1.27.0/mypy_boto3_ecr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr.egg-info/PKG-INFO` & `mypy-boto3-ecr-1.27.0/mypy_boto3_ecr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.ECR 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.ECR 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/
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
 
 <a id="mypy-boto3-ecr"></a>
 
 # mypy-boto3-ecr
 
 [![PyPI - mypy-boto3-ecr](https://img.shields.io/pypi/v/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecr?color=blue)](https://pypistats.org/packages/mypy-boto3-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECR 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[boto3.ECR 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -389,101 +390,101 @@
 from mypy_boto3_ecr.type_defs import (
     AttributeTypeDef,
     AuthorizationDataTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
-    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
     BatchGetRepositoryScanningConfigurationRequestRequestTypeDef,
     RepositoryScanningConfigurationFailureTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
+    CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleRequestRequestTypeDef,
+    CreatePullThroughCacheRuleResponseTypeDef,
     EncryptionConfigurationTypeDef,
     ImageScanningConfigurationTypeDef,
     TagTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
+    DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleRequestRequestTypeDef,
+    DeletePullThroughCacheRuleResponseTypeDef,
+    DeleteRegistryPolicyResponseTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
     ImageReplicationStatusTypeDef,
-    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     ImageScanStatusTypeDef,
     DescribeImagesFilterTypeDef,
+    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
     DescribePullThroughCacheRulesRequestRequestTypeDef,
     PullThroughCacheRuleTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
     GetDownloadUrlForLayerRequestRequestTypeDef,
+    GetDownloadUrlForLayerResponseTypeDef,
     LifecyclePolicyPreviewFilterTypeDef,
     LifecyclePolicyPreviewSummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
+    GetLifecyclePolicyResponseTypeDef,
+    GetRegistryPolicyResponseTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
     ImageScanFindingsSummaryTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
+    InitiateLayerUploadResponseTypeDef,
     LifecyclePolicyRuleActionTypeDef,
     ListImagesFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     VulnerablePackageTypeDef,
+    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutImageTagMutabilityRequestRequestTypeDef,
+    PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyRequestRequestTypeDef,
+    PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyRequestRequestTypeDef,
+    PutRegistryPolicyResponseTypeDef,
     RecommendationTypeDef,
     ScanningRepositoryFilterTypeDef,
     ReplicationDestinationTypeDef,
     RepositoryFilterTypeDef,
+    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
     StartLifecyclePolicyPreviewRequestRequestTypeDef,
+    StartLifecyclePolicyPreviewResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UploadLayerPartRequestRequestTypeDef,
+    UploadLayerPartResponseTypeDef,
     ImageScanFindingTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
     ResourceDetailsTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
-    CompleteLayerUploadResponseTypeDef,
-    CreatePullThroughCacheRuleResponseTypeDef,
-    DeleteLifecyclePolicyResponseTypeDef,
-    DeletePullThroughCacheRuleResponseTypeDef,
-    DeleteRegistryPolicyResponseTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
-    GetDownloadUrlForLayerResponseTypeDef,
-    GetLifecyclePolicyResponseTypeDef,
-    GetRegistryPolicyResponseTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
-    InitiateLayerUploadResponseTypeDef,
-    PutImageTagMutabilityResponseTypeDef,
-    PutLifecyclePolicyResponseTypeDef,
-    PutRegistryPolicyResponseTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
-    StartLifecyclePolicyPreviewResponseTypeDef,
-    UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
     BatchGetImageRequestRequestTypeDef,
     DescribeImageReplicationStatusRequestRequestTypeDef,
+    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
     DescribeImageScanFindingsRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     ListImagesResponseTypeDef,
     StartImageScanRequestRequestTypeDef,
     PutImageScanningConfigurationRequestRequestTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     RepositoryTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CvssScoreDetailsTypeDef,
     DescribeImageReplicationStatusResponseTypeDef,
-    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
-    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     StartImageScanResponseTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     DescribePullThroughCacheRulesResponseTypeDef,
     GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
@@ -529,42 +530,42 @@
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

### Comparing `mypy-boto3-ecr-1.26.0.post1/mypy_boto3_ecr.egg-info/SOURCES.txt` & `mypy-boto3-ecr-1.27.0/mypy_boto3_ecr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.26.0.post1/setup.py` & `mypy-boto3-ecr-1.27.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-ecr.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecr",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_ecr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECR 1.26.0 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.ECR 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 ecr type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_ecr": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_ecr": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/",
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


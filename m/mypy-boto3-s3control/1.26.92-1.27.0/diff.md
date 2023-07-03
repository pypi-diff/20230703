# Comparing `tmp/mypy-boto3-s3control-1.26.92.tar.gz` & `tmp/mypy-boto3-s3control-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3control-1.26.92.tar", last modified: Wed Mar 15 19:32:09 2023, max compression
+gzip compressed data, was "mypy-boto3-s3control-1.27.0.tar", last modified: Mon Jul  3 19:51:22 2023, max compression
```

## Comparing `mypy-boto3-s3control-1.26.92.tar` & `mypy-boto3-s3control-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 19:32:09.719555 mypy-boto3-s3control-1.26.92/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-03-15 19:32:09.719555 mypy-boto3-s3control-1.26.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21217 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 19:32:09.715555 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43053 2023-03-15 19:31:58.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42981 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-03-15 19:31:58.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13411 2023-03-15 19:31:58.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-15 19:31:58.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-03-15 19:31:58.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    70164 2023-03-15 19:32:00.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    70087 2023-03-15 19:31:58.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 19:32:09.715555 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-03-15 19:32:09.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-15 19:32:09.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 19:32:09.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 19:32:09.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-15 19:32:09.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-15 19:32:09.000000 mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 19:32:09.719555 mypy-boto3-s3control-1.26.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-15 19:31:57.000000 mypy-boto3-s3control-1.26.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:22.707915 mypy-boto3-s3control-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:53.000000 mypy-boto3-s3control-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22690 2023-07-03 19:51:22.707915 mypy-boto3-s3control-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21197 2023-07-03 19:46:53.000000 mypy-boto3-s3control-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:22.703915 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-03 19:46:53.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-03 19:46:53.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:46:53.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43055 2023-07-03 19:46:53.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42983 2023-07-03 19:46:53.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-07-03 19:46:54.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-07-03 19:46:53.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-03 19:46:53.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-03 19:46:53.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:53.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    70244 2023-07-03 19:46:57.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70167 2023-07-03 19:46:54.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:53.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:22.707915 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22690 2023-07-03 19:51:22.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-03 19:51:22.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:22.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:22.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:22.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:51:22.000000 mypy-boto3-s3control-1.27.0/mypy_boto3_s3control.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:22.707915 mypy-boto3-s3control-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:46:53.000000 mypy-boto3-s3control-1.27.0/setup.py
```

### Comparing `mypy-boto3-s3control-1.26.92/LICENSE` & `mypy-boto3-s3control-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-s3control-1.26.92/PKG-INFO` & `mypy-boto3-s3control-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3control
-Version: 1.26.92
-Summary: Type annotations for boto3.S3Control 1.26.92 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.S3Control 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-s3control"></a>
 
 # mypy-boto3-s3control
 
 [![PyPI - mypy-boto3-s3control](https://img.shields.io/pypi/v/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3control?color=blue)](https://pypistats.org/packages/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.26.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
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
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
 See how it helps to find and fix potential bugs:
 
@@ -377,55 +377,65 @@
     DetailedStatusCodesMetricsTypeDef,
     AsyncErrorDetailsTypeDef,
     DeleteMultiRegionAccessPointInputTypeDef,
     PutMultiRegionAccessPointPolicyInputTypeDef,
     AwsLambdaTransformationTypeDef,
     CloudWatchMetricsTypeDef,
     ObjectLambdaAccessPointAliasTypeDef,
-    ResponseMetadataTypeDef,
     PublicAccessBlockConfigurationTypeDef,
+    CreateAccessPointResultTypeDef,
     CreateBucketConfigurationTypeDef,
+    CreateBucketResultTypeDef,
     JobReportTypeDef,
     S3TagTypeDef,
+    CreateJobResultTypeDef,
     RegionTypeDef,
+    CreateMultiRegionAccessPointResultTypeDef,
     DeleteAccessPointForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyRequestRequestTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteBucketLifecycleConfigurationRequestRequestTypeDef,
     DeleteBucketPolicyRequestRequestTypeDef,
     DeleteBucketReplicationRequestRequestTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteJobTaggingRequestRequestTypeDef,
     DeleteMarkerReplicationTypeDef,
+    DeleteMultiRegionAccessPointResultTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     DeleteStorageLensConfigurationRequestRequestTypeDef,
     DeleteStorageLensConfigurationTaggingRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeMultiRegionAccessPointOperationRequestRequestTypeDef,
     EncryptionConfigurationTypeDef,
+    EmptyResponseMetadataTypeDef,
     EstablishedMultiRegionAccessPointPolicyTypeDef,
     ExcludeTypeDef,
     ExistingObjectReplicationTypeDef,
     SSEKMSEncryptionTypeDef,
     GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
     GetAccessPointForObjectLambdaRequestRequestTypeDef,
     GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
+    GetAccessPointPolicyForObjectLambdaResultTypeDef,
     GetAccessPointPolicyRequestRequestTypeDef,
+    GetAccessPointPolicyResultTypeDef,
     GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef,
     PolicyStatusTypeDef,
     GetAccessPointPolicyStatusRequestRequestTypeDef,
     GetAccessPointRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
+    GetBucketPolicyResultTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
     GetBucketRequestRequestTypeDef,
+    GetBucketResultTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
+    GetBucketVersioningResultTypeDef,
     GetJobTaggingRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef,
     GetMultiRegionAccessPointRequestRequestTypeDef,
     GetMultiRegionAccessPointRoutesRequestRequestTypeDef,
     MultiRegionAccessPointRouteTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
@@ -440,63 +450,54 @@
     LambdaInvokeOperationTypeDef,
     S3InitiateRestoreObjectOperationTypeDef,
     JobTimersTypeDef,
     LifecycleExpirationTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     ListAccessPointsForObjectLambdaRequestRequestTypeDef,
     ListAccessPointsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListMultiRegionAccessPointsRequestRequestTypeDef,
     ListRegionalBucketsRequestRequestTypeDef,
     RegionalBucketTypeDef,
     ListStorageLensConfigurationEntryTypeDef,
     ListStorageLensConfigurationsRequestRequestTypeDef,
     ReplicationTimeValueTypeDef,
     ProposedMultiRegionAccessPointPolicyTypeDef,
     MultiRegionAccessPointRegionalResponseTypeDef,
     RegionReportTypeDef,
+    PaginatorConfigTypeDef,
     SelectionCriteriaTypeDef,
     PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     PutAccessPointPolicyRequestRequestTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     VersioningConfigurationTypeDef,
+    PutMultiRegionAccessPointPolicyResultTypeDef,
     ReplicaModificationsTypeDef,
+    ResponseMetadataTypeDef,
     S3ObjectOwnerTypeDef,
     S3ObjectMetadataTypeDef,
     S3GranteeTypeDef,
     S3ObjectLockLegalHoldTypeDef,
     S3RetentionTypeDef,
     SSEKMSTypeDef,
     SseKmsEncryptedObjectsTypeDef,
     StorageLensAwsOrgTypeDef,
     UpdateJobPriorityRequestRequestTypeDef,
+    UpdateJobPriorityResultTypeDef,
     UpdateJobStatusRequestRequestTypeDef,
+    UpdateJobStatusResultTypeDef,
     AccessPointTypeDef,
     DeleteMultiRegionAccessPointRequestRequestTypeDef,
     PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
     ObjectLambdaContentTransformationTypeDef,
-    ObjectLambdaAccessPointTypeDef,
     CreateAccessPointForObjectLambdaResultTypeDef,
-    CreateAccessPointResultTypeDef,
-    CreateBucketResultTypeDef,
-    CreateJobResultTypeDef,
-    CreateMultiRegionAccessPointResultTypeDef,
-    DeleteMultiRegionAccessPointResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAccessPointPolicyForObjectLambdaResultTypeDef,
-    GetAccessPointPolicyResultTypeDef,
-    GetBucketPolicyResultTypeDef,
-    GetBucketResultTypeDef,
-    GetBucketVersioningResultTypeDef,
-    PutMultiRegionAccessPointPolicyResultTypeDef,
-    UpdateJobPriorityResultTypeDef,
-    UpdateJobStatusResultTypeDef,
+    ObjectLambdaAccessPointTypeDef,
     CreateAccessPointRequestRequestTypeDef,
     GetAccessPointForObjectLambdaResultTypeDef,
     GetAccessPointResultTypeDef,
     GetPublicAccessBlockOutputTypeDef,
     PutPublicAccessBlockRequestRequestTypeDef,
     CreateBucketRequestRequestTypeDef,
     GetBucketTaggingResultTypeDef,
@@ -514,15 +515,14 @@
     GetMultiRegionAccessPointRoutesResultTypeDef,
     SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
     PutStorageLensConfigurationTaggingRequestRequestTypeDef,
     S3GeneratedManifestDescriptorTypeDef,
     JobManifestTypeDef,
     JobProgressSummaryTypeDef,
-    ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     MultiRegionAccessPointPolicyDocumentTypeDef,
     MultiRegionAccessPointsAsyncResponseTypeDef,
     MultiRegionAccessPointReportTypeDef,
@@ -591,42 +591,42 @@
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

### Comparing `mypy-boto3-s3control-1.26.92/README.md` & `mypy-boto3-s3control-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-s3control"></a>
 
 # mypy-boto3-s3control
 
 [![PyPI - mypy-boto3-s3control](https://img.shields.io/pypi/v/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3control?color=blue)](https://pypistats.org/packages/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.26.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
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
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,55 +345,65 @@
     DetailedStatusCodesMetricsTypeDef,
     AsyncErrorDetailsTypeDef,
     DeleteMultiRegionAccessPointInputTypeDef,
     PutMultiRegionAccessPointPolicyInputTypeDef,
     AwsLambdaTransformationTypeDef,
     CloudWatchMetricsTypeDef,
     ObjectLambdaAccessPointAliasTypeDef,
-    ResponseMetadataTypeDef,
     PublicAccessBlockConfigurationTypeDef,
+    CreateAccessPointResultTypeDef,
     CreateBucketConfigurationTypeDef,
+    CreateBucketResultTypeDef,
     JobReportTypeDef,
     S3TagTypeDef,
+    CreateJobResultTypeDef,
     RegionTypeDef,
+    CreateMultiRegionAccessPointResultTypeDef,
     DeleteAccessPointForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyRequestRequestTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteBucketLifecycleConfigurationRequestRequestTypeDef,
     DeleteBucketPolicyRequestRequestTypeDef,
     DeleteBucketReplicationRequestRequestTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteJobTaggingRequestRequestTypeDef,
     DeleteMarkerReplicationTypeDef,
+    DeleteMultiRegionAccessPointResultTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     DeleteStorageLensConfigurationRequestRequestTypeDef,
     DeleteStorageLensConfigurationTaggingRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeMultiRegionAccessPointOperationRequestRequestTypeDef,
     EncryptionConfigurationTypeDef,
+    EmptyResponseMetadataTypeDef,
     EstablishedMultiRegionAccessPointPolicyTypeDef,
     ExcludeTypeDef,
     ExistingObjectReplicationTypeDef,
     SSEKMSEncryptionTypeDef,
     GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
     GetAccessPointForObjectLambdaRequestRequestTypeDef,
     GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
+    GetAccessPointPolicyForObjectLambdaResultTypeDef,
     GetAccessPointPolicyRequestRequestTypeDef,
+    GetAccessPointPolicyResultTypeDef,
     GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef,
     PolicyStatusTypeDef,
     GetAccessPointPolicyStatusRequestRequestTypeDef,
     GetAccessPointRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
+    GetBucketPolicyResultTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
     GetBucketRequestRequestTypeDef,
+    GetBucketResultTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
+    GetBucketVersioningResultTypeDef,
     GetJobTaggingRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef,
     GetMultiRegionAccessPointRequestRequestTypeDef,
     GetMultiRegionAccessPointRoutesRequestRequestTypeDef,
     MultiRegionAccessPointRouteTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
@@ -408,63 +418,54 @@
     LambdaInvokeOperationTypeDef,
     S3InitiateRestoreObjectOperationTypeDef,
     JobTimersTypeDef,
     LifecycleExpirationTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     ListAccessPointsForObjectLambdaRequestRequestTypeDef,
     ListAccessPointsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListMultiRegionAccessPointsRequestRequestTypeDef,
     ListRegionalBucketsRequestRequestTypeDef,
     RegionalBucketTypeDef,
     ListStorageLensConfigurationEntryTypeDef,
     ListStorageLensConfigurationsRequestRequestTypeDef,
     ReplicationTimeValueTypeDef,
     ProposedMultiRegionAccessPointPolicyTypeDef,
     MultiRegionAccessPointRegionalResponseTypeDef,
     RegionReportTypeDef,
+    PaginatorConfigTypeDef,
     SelectionCriteriaTypeDef,
     PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     PutAccessPointPolicyRequestRequestTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     VersioningConfigurationTypeDef,
+    PutMultiRegionAccessPointPolicyResultTypeDef,
     ReplicaModificationsTypeDef,
+    ResponseMetadataTypeDef,
     S3ObjectOwnerTypeDef,
     S3ObjectMetadataTypeDef,
     S3GranteeTypeDef,
     S3ObjectLockLegalHoldTypeDef,
     S3RetentionTypeDef,
     SSEKMSTypeDef,
     SseKmsEncryptedObjectsTypeDef,
     StorageLensAwsOrgTypeDef,
     UpdateJobPriorityRequestRequestTypeDef,
+    UpdateJobPriorityResultTypeDef,
     UpdateJobStatusRequestRequestTypeDef,
+    UpdateJobStatusResultTypeDef,
     AccessPointTypeDef,
     DeleteMultiRegionAccessPointRequestRequestTypeDef,
     PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
     ObjectLambdaContentTransformationTypeDef,
-    ObjectLambdaAccessPointTypeDef,
     CreateAccessPointForObjectLambdaResultTypeDef,
-    CreateAccessPointResultTypeDef,
-    CreateBucketResultTypeDef,
-    CreateJobResultTypeDef,
-    CreateMultiRegionAccessPointResultTypeDef,
-    DeleteMultiRegionAccessPointResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAccessPointPolicyForObjectLambdaResultTypeDef,
-    GetAccessPointPolicyResultTypeDef,
-    GetBucketPolicyResultTypeDef,
-    GetBucketResultTypeDef,
-    GetBucketVersioningResultTypeDef,
-    PutMultiRegionAccessPointPolicyResultTypeDef,
-    UpdateJobPriorityResultTypeDef,
-    UpdateJobStatusResultTypeDef,
+    ObjectLambdaAccessPointTypeDef,
     CreateAccessPointRequestRequestTypeDef,
     GetAccessPointForObjectLambdaResultTypeDef,
     GetAccessPointResultTypeDef,
     GetPublicAccessBlockOutputTypeDef,
     PutPublicAccessBlockRequestRequestTypeDef,
     CreateBucketRequestRequestTypeDef,
     GetBucketTaggingResultTypeDef,
@@ -482,15 +483,14 @@
     GetMultiRegionAccessPointRoutesResultTypeDef,
     SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
     PutStorageLensConfigurationTaggingRequestRequestTypeDef,
     S3GeneratedManifestDescriptorTypeDef,
     JobManifestTypeDef,
     JobProgressSummaryTypeDef,
-    ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     MultiRegionAccessPointPolicyDocumentTypeDef,
     MultiRegionAccessPointsAsyncResponseTypeDef,
     MultiRegionAccessPointReportTypeDef,
@@ -559,42 +559,42 @@
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

### Comparing `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/__init__.py` & `mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/__init__.pyi` & `mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/__main__.py` & `mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3Control 1.26.92\nVersion:         1.26.92\nBuilder version:"
-        " 7.13.0\nDocs:           "
+        "Type annotations for boto3.S3Control 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.92")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/client.py` & `mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,17 +410,17 @@
         """
 
     def get_access_point_for_object_lambda(
         self, *, AccountId: str, Name: str
     ) -> GetAccessPointForObjectLambdaResultTypeDef:
         """
         Returns configuration information about the specified Object Lambda Access Point
-        The following actions are related to `GetAccessPointForObjectLambda`  *
+        The following actions are related to `GetAccessPointForObjectLambda`: *
         `CreateAccessPointForObjectLambda
-        <https://docs.aws.amazon.com/AmazonS3/latest/API/API_control_CreateAccessPointForObjectLambda.htm...`.
+        <https://docs.aws.amazon.com/AmazonS3/latest/API/API_control_CreateAccessPointForObjectLambda.html>...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_for_object_lambda)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#get_access_point_for_object_lambda)
         """
 
     def get_access_point_policy(
         self, *, AccountId: str, Name: str
```

### Comparing `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/client.pyi` & `mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -379,17 +379,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#get_access_point_configuration_for_object_lambda)
         """
     def get_access_point_for_object_lambda(
         self, *, AccountId: str, Name: str
     ) -> GetAccessPointForObjectLambdaResultTypeDef:
         """
         Returns configuration information about the specified Object Lambda Access Point
-        The following actions are related to `GetAccessPointForObjectLambda`  *
+        The following actions are related to `GetAccessPointForObjectLambda`: *
         `CreateAccessPointForObjectLambda
-        <https://docs.aws.amazon.com/AmazonS3/latest/API/API_control_CreateAccessPointForObjectLambda.htm...`.
+        <https://docs.aws.amazon.com/AmazonS3/latest/API/API_control_CreateAccessPointForObjectLambda.html>...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.get_access_point_for_object_lambda)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#get_access_point_for_object_lambda)
         """
     def get_access_point_policy(
         self, *, AccountId: str, Name: str
     ) -> GetAccessPointPolicyResultTypeDef:
```

### Comparing `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/literals.py` & `mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,15 @@
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
@@ -256,14 +257,15 @@
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
@@ -361,14 +363,15 @@
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
@@ -404,14 +407,15 @@
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
@@ -430,16 +434,19 @@
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
@@ -523,15 +530,17 @@
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

### Comparing `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/literals.pyi` & `mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,15 @@
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
@@ -254,14 +255,15 @@
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
@@ -359,14 +361,15 @@
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
@@ -402,14 +405,15 @@
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
@@ -428,16 +432,19 @@
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
@@ -521,15 +528,17 @@
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

### Comparing `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/paginator.py` & `mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListAccessPointsForObjectLambdaPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Paginator.ListAccessPointsForObjectLambda)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/paginators/#listaccesspointsforobjectlambdapaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccessPointsForObjectLambdaResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Paginator.ListAccessPointsForObjectLambda.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/paginators/#listaccesspointsforobjectlambdapaginator)
         """
```

### Comparing `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/paginator.pyi` & `mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListAccessPointsForObjectLambdaPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Paginator.ListAccessPointsForObjectLambda)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/paginators/#listaccesspointsforobjectlambdapaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccessPointsForObjectLambdaResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Paginator.ListAccessPointsForObjectLambda.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/paginators/#listaccesspointsforobjectlambdapaginator)
         """
```

### Comparing `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/type_defs.py` & `mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,55 +78,65 @@
     "DetailedStatusCodesMetricsTypeDef",
     "AsyncErrorDetailsTypeDef",
     "DeleteMultiRegionAccessPointInputTypeDef",
     "PutMultiRegionAccessPointPolicyInputTypeDef",
     "AwsLambdaTransformationTypeDef",
     "CloudWatchMetricsTypeDef",
     "ObjectLambdaAccessPointAliasTypeDef",
-    "ResponseMetadataTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
+    "CreateAccessPointResultTypeDef",
     "CreateBucketConfigurationTypeDef",
+    "CreateBucketResultTypeDef",
     "JobReportTypeDef",
     "S3TagTypeDef",
+    "CreateJobResultTypeDef",
     "RegionTypeDef",
+    "CreateMultiRegionAccessPointResultTypeDef",
     "DeleteAccessPointForObjectLambdaRequestRequestTypeDef",
     "DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "DeleteAccessPointPolicyRequestRequestTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteBucketLifecycleConfigurationRequestRequestTypeDef",
     "DeleteBucketPolicyRequestRequestTypeDef",
     "DeleteBucketReplicationRequestRequestTypeDef",
     "DeleteBucketRequestRequestTypeDef",
     "DeleteBucketTaggingRequestRequestTypeDef",
     "DeleteJobTaggingRequestRequestTypeDef",
     "DeleteMarkerReplicationTypeDef",
+    "DeleteMultiRegionAccessPointResultTypeDef",
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "DeleteStorageLensConfigurationRequestRequestTypeDef",
     "DeleteStorageLensConfigurationTaggingRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeMultiRegionAccessPointOperationRequestRequestTypeDef",
     "EncryptionConfigurationTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EstablishedMultiRegionAccessPointPolicyTypeDef",
     "ExcludeTypeDef",
     "ExistingObjectReplicationTypeDef",
     "SSEKMSEncryptionTypeDef",
     "GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
+    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
     "GetAccessPointPolicyRequestRequestTypeDef",
+    "GetAccessPointPolicyResultTypeDef",
     "GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef",
     "PolicyStatusTypeDef",
     "GetAccessPointPolicyStatusRequestRequestTypeDef",
     "GetAccessPointRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketPolicyRequestRequestTypeDef",
+    "GetBucketPolicyResultTypeDef",
     "GetBucketReplicationRequestRequestTypeDef",
     "GetBucketRequestRequestTypeDef",
+    "GetBucketResultTypeDef",
     "GetBucketTaggingRequestRequestTypeDef",
     "GetBucketVersioningRequestRequestTypeDef",
+    "GetBucketVersioningResultTypeDef",
     "GetJobTaggingRequestRequestTypeDef",
     "GetMultiRegionAccessPointPolicyRequestRequestTypeDef",
     "GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef",
     "GetMultiRegionAccessPointRequestRequestTypeDef",
     "GetMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "MultiRegionAccessPointRouteTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
@@ -141,63 +151,54 @@
     "LambdaInvokeOperationTypeDef",
     "S3InitiateRestoreObjectOperationTypeDef",
     "JobTimersTypeDef",
     "LifecycleExpirationTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
     "TransitionTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     "ListAccessPointsForObjectLambdaRequestRequestTypeDef",
     "ListAccessPointsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListMultiRegionAccessPointsRequestRequestTypeDef",
     "ListRegionalBucketsRequestRequestTypeDef",
     "RegionalBucketTypeDef",
     "ListStorageLensConfigurationEntryTypeDef",
     "ListStorageLensConfigurationsRequestRequestTypeDef",
     "ReplicationTimeValueTypeDef",
     "ProposedMultiRegionAccessPointPolicyTypeDef",
     "MultiRegionAccessPointRegionalResponseTypeDef",
     "RegionReportTypeDef",
+    "PaginatorConfigTypeDef",
     "SelectionCriteriaTypeDef",
     "PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "PutAccessPointPolicyRequestRequestTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "VersioningConfigurationTypeDef",
+    "PutMultiRegionAccessPointPolicyResultTypeDef",
     "ReplicaModificationsTypeDef",
+    "ResponseMetadataTypeDef",
     "S3ObjectOwnerTypeDef",
     "S3ObjectMetadataTypeDef",
     "S3GranteeTypeDef",
     "S3ObjectLockLegalHoldTypeDef",
     "S3RetentionTypeDef",
     "SSEKMSTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
     "StorageLensAwsOrgTypeDef",
     "UpdateJobPriorityRequestRequestTypeDef",
+    "UpdateJobPriorityResultTypeDef",
     "UpdateJobStatusRequestRequestTypeDef",
+    "UpdateJobStatusResultTypeDef",
     "AccessPointTypeDef",
     "DeleteMultiRegionAccessPointRequestRequestTypeDef",
     "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
     "ObjectLambdaContentTransformationTypeDef",
-    "ObjectLambdaAccessPointTypeDef",
     "CreateAccessPointForObjectLambdaResultTypeDef",
-    "CreateAccessPointResultTypeDef",
-    "CreateBucketResultTypeDef",
-    "CreateJobResultTypeDef",
-    "CreateMultiRegionAccessPointResultTypeDef",
-    "DeleteMultiRegionAccessPointResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
-    "GetAccessPointPolicyResultTypeDef",
-    "GetBucketPolicyResultTypeDef",
-    "GetBucketResultTypeDef",
-    "GetBucketVersioningResultTypeDef",
-    "PutMultiRegionAccessPointPolicyResultTypeDef",
-    "UpdateJobPriorityResultTypeDef",
-    "UpdateJobStatusResultTypeDef",
+    "ObjectLambdaAccessPointTypeDef",
     "CreateAccessPointRequestRequestTypeDef",
     "GetAccessPointForObjectLambdaResultTypeDef",
     "GetAccessPointResultTypeDef",
     "GetPublicAccessBlockOutputTypeDef",
     "PutPublicAccessBlockRequestRequestTypeDef",
     "CreateBucketRequestRequestTypeDef",
     "GetBucketTaggingResultTypeDef",
@@ -215,15 +216,14 @@
     "GetMultiRegionAccessPointRoutesResultTypeDef",
     "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingResultTypeDef",
     "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
     "S3GeneratedManifestDescriptorTypeDef",
     "JobManifestTypeDef",
     "JobProgressSummaryTypeDef",
-    "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     "ListRegionalBucketsResultTypeDef",
     "ListStorageLensConfigurationsResultTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "MultiRegionAccessPointPolicyDocumentTypeDef",
     "MultiRegionAccessPointsAsyncResponseTypeDef",
     "MultiRegionAccessPointReportTypeDef",
@@ -397,44 +397,51 @@
     {
         "Value": str,
         "Status": ObjectLambdaAccessPointAliasStatusType,
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
 PublicAccessBlockConfigurationTypeDef = TypedDict(
     "PublicAccessBlockConfigurationTypeDef",
     {
         "BlockPublicAcls": bool,
         "IgnorePublicAcls": bool,
         "BlockPublicPolicy": bool,
         "RestrictPublicBuckets": bool,
     },
     total=False,
 )
 
+CreateAccessPointResultTypeDef = TypedDict(
+    "CreateAccessPointResultTypeDef",
+    {
+        "AccessPointArn": str,
+        "Alias": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateBucketConfigurationTypeDef = TypedDict(
     "CreateBucketConfigurationTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
     },
     total=False,
 )
 
+CreateBucketResultTypeDef = TypedDict(
+    "CreateBucketResultTypeDef",
+    {
+        "Location": str,
+        "BucketArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredJobReportTypeDef = TypedDict(
     "_RequiredJobReportTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalJobReportTypeDef = TypedDict(
@@ -457,14 +464,22 @@
     "S3TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateJobResultTypeDef = TypedDict(
+    "CreateJobResultTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRegionTypeDef = TypedDict(
     "_RequiredRegionTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalRegionTypeDef = TypedDict(
@@ -476,14 +491,22 @@
 )
 
 
 class RegionTypeDef(_RequiredRegionTypeDef, _OptionalRegionTypeDef):
     pass
 
 
+CreateMultiRegionAccessPointResultTypeDef = TypedDict(
+    "CreateMultiRegionAccessPointResultTypeDef",
+    {
+        "RequestTokenARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteAccessPointForObjectLambdaRequestRequestTypeDef = TypedDict(
     "DeleteAccessPointForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
@@ -563,14 +586,22 @@
 DeleteMarkerReplicationTypeDef = TypedDict(
     "DeleteMarkerReplicationTypeDef",
     {
         "Status": DeleteMarkerReplicationStatusType,
     },
 )
 
+DeleteMultiRegionAccessPointResultTypeDef = TypedDict(
+    "DeleteMultiRegionAccessPointResultTypeDef",
+    {
+        "RequestTokenARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePublicAccessBlockRequestRequestTypeDef = TypedDict(
     "DeletePublicAccessBlockRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 
@@ -610,14 +641,21 @@
     "EncryptionConfigurationTypeDef",
     {
         "ReplicaKmsKeyID": str,
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
 EstablishedMultiRegionAccessPointPolicyTypeDef = TypedDict(
     "EstablishedMultiRegionAccessPointPolicyTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
@@ -665,22 +703,38 @@
     "GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
 
+GetAccessPointPolicyForObjectLambdaResultTypeDef = TypedDict(
+    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAccessPointPolicyRequestRequestTypeDef = TypedDict(
     "GetAccessPointPolicyRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
 
+GetAccessPointPolicyResultTypeDef = TypedDict(
+    "GetAccessPointPolicyResultTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef = TypedDict(
     "GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
@@ -721,14 +775,22 @@
     "GetBucketPolicyRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
 
+GetBucketPolicyResultTypeDef = TypedDict(
+    "GetBucketPolicyResultTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBucketReplicationRequestRequestTypeDef = TypedDict(
     "GetBucketReplicationRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
@@ -737,14 +799,24 @@
     "GetBucketRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
 
+GetBucketResultTypeDef = TypedDict(
+    "GetBucketResultTypeDef",
+    {
+        "Bucket": str,
+        "PublicAccessBlockEnabled": bool,
+        "CreationDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBucketTaggingRequestRequestTypeDef = TypedDict(
     "GetBucketTaggingRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
@@ -753,14 +825,23 @@
     "GetBucketVersioningRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
 
+GetBucketVersioningResultTypeDef = TypedDict(
+    "GetBucketVersioningResultTypeDef",
+    {
+        "Status": BucketVersioningStatusType,
+        "MFADelete": MFADeleteStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetJobTaggingRequestRequestTypeDef = TypedDict(
     "GetJobTaggingRequestRequestTypeDef",
     {
         "AccountId": str,
         "JobId": str,
     },
 )
@@ -979,24 +1060,36 @@
         "Date": datetime,
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
+    "_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "AccountId": str,
+    },
+)
+_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
+    "_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef(
+    _RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
+    _OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAccessPointsForObjectLambdaRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessPointsForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListAccessPointsForObjectLambdaRequestRequestTypeDef = TypedDict(
@@ -1208,14 +1301,24 @@
         "Bucket": str,
         "Region": str,
         "BucketAccountId": str,
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
 SelectionCriteriaTypeDef = TypedDict(
     "SelectionCriteriaTypeDef",
     {
         "Delimiter": str,
         "MaxDepth": int,
         "MinStorageBytesPercentage": float,
     },
@@ -1268,21 +1371,40 @@
     {
         "MFADelete": MFADeleteType,
         "Status": BucketVersioningStatusType,
     },
     total=False,
 )
 
+PutMultiRegionAccessPointPolicyResultTypeDef = TypedDict(
+    "PutMultiRegionAccessPointPolicyResultTypeDef",
+    {
+        "RequestTokenARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ReplicaModificationsTypeDef = TypedDict(
     "ReplicaModificationsTypeDef",
     {
         "Status": ReplicaModificationsStatusType,
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
 S3ObjectOwnerTypeDef = TypedDict(
     "S3ObjectOwnerTypeDef",
     {
         "ID": str,
         "DisplayName": str,
     },
     total=False,
@@ -1358,14 +1480,23 @@
     {
         "AccountId": str,
         "JobId": str,
         "Priority": int,
     },
 )
 
+UpdateJobPriorityResultTypeDef = TypedDict(
+    "UpdateJobPriorityResultTypeDef",
+    {
+        "JobId": str,
+        "Priority": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateJobStatusRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobStatusRequestRequestTypeDef",
     {
         "AccountId": str,
         "JobId": str,
         "RequestedJobStatus": RequestedJobStatusType,
     },
@@ -1381,14 +1512,24 @@
 
 class UpdateJobStatusRequestRequestTypeDef(
     _RequiredUpdateJobStatusRequestRequestTypeDef, _OptionalUpdateJobStatusRequestRequestTypeDef
 ):
     pass
 
 
+UpdateJobStatusResultTypeDef = TypedDict(
+    "UpdateJobStatusResultTypeDef",
+    {
+        "JobId": str,
+        "Status": JobStatusType,
+        "StatusUpdateReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAccessPointTypeDef = TypedDict(
     "_RequiredAccessPointTypeDef",
     {
         "Name": str,
         "NetworkOrigin": NetworkOriginType,
         "Bucket": str,
     },
@@ -1431,14 +1572,23 @@
     "ObjectLambdaContentTransformationTypeDef",
     {
         "AwsLambda": AwsLambdaTransformationTypeDef,
     },
     total=False,
 )
 
+CreateAccessPointForObjectLambdaResultTypeDef = TypedDict(
+    "CreateAccessPointForObjectLambdaResultTypeDef",
+    {
+        "ObjectLambdaAccessPointArn": str,
+        "Alias": ObjectLambdaAccessPointAliasTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredObjectLambdaAccessPointTypeDef = TypedDict(
     "_RequiredObjectLambdaAccessPointTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalObjectLambdaAccessPointTypeDef = TypedDict(
@@ -1453,142 +1603,14 @@
 
 class ObjectLambdaAccessPointTypeDef(
     _RequiredObjectLambdaAccessPointTypeDef, _OptionalObjectLambdaAccessPointTypeDef
 ):
     pass
 
 
-CreateAccessPointForObjectLambdaResultTypeDef = TypedDict(
-    "CreateAccessPointForObjectLambdaResultTypeDef",
-    {
-        "ObjectLambdaAccessPointArn": str,
-        "Alias": ObjectLambdaAccessPointAliasTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAccessPointResultTypeDef = TypedDict(
-    "CreateAccessPointResultTypeDef",
-    {
-        "AccessPointArn": str,
-        "Alias": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBucketResultTypeDef = TypedDict(
-    "CreateBucketResultTypeDef",
-    {
-        "Location": str,
-        "BucketArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobResultTypeDef = TypedDict(
-    "CreateJobResultTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMultiRegionAccessPointResultTypeDef = TypedDict(
-    "CreateMultiRegionAccessPointResultTypeDef",
-    {
-        "RequestTokenARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteMultiRegionAccessPointResultTypeDef = TypedDict(
-    "DeleteMultiRegionAccessPointResultTypeDef",
-    {
-        "RequestTokenARN": str,
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
-GetAccessPointPolicyForObjectLambdaResultTypeDef = TypedDict(
-    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAccessPointPolicyResultTypeDef = TypedDict(
-    "GetAccessPointPolicyResultTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBucketPolicyResultTypeDef = TypedDict(
-    "GetBucketPolicyResultTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBucketResultTypeDef = TypedDict(
-    "GetBucketResultTypeDef",
-    {
-        "Bucket": str,
-        "PublicAccessBlockEnabled": bool,
-        "CreationDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBucketVersioningResultTypeDef = TypedDict(
-    "GetBucketVersioningResultTypeDef",
-    {
-        "Status": BucketVersioningStatusType,
-        "MFADelete": MFADeleteStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutMultiRegionAccessPointPolicyResultTypeDef = TypedDict(
-    "PutMultiRegionAccessPointPolicyResultTypeDef",
-    {
-        "RequestTokenARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateJobPriorityResultTypeDef = TypedDict(
-    "UpdateJobPriorityResultTypeDef",
-    {
-        "JobId": str,
-        "Priority": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateJobStatusResultTypeDef = TypedDict(
-    "UpdateJobStatusResultTypeDef",
-    {
-        "JobId": str,
-        "Status": JobStatusType,
-        "StatusUpdateReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateAccessPointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPointRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
         "Bucket": str,
     },
@@ -1613,15 +1635,15 @@
 GetAccessPointForObjectLambdaResultTypeDef = TypedDict(
     "GetAccessPointForObjectLambdaResultTypeDef",
     {
         "Name": str,
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "CreationDate": datetime,
         "Alias": ObjectLambdaAccessPointAliasTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccessPointResultTypeDef = TypedDict(
     "GetAccessPointResultTypeDef",
     {
         "Name": str,
@@ -1630,23 +1652,23 @@
         "VpcConfiguration": VpcConfigurationTypeDef,
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "CreationDate": datetime,
         "Alias": str,
         "AccessPointArn": str,
         "Endpoints": Dict[str, str],
         "BucketAccountId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPublicAccessBlockOutputTypeDef = TypedDict(
     "GetPublicAccessBlockOutputTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "PutPublicAccessBlockRequestRequestTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
@@ -1683,23 +1705,23 @@
     pass
 
 
 GetBucketTaggingResultTypeDef = TypedDict(
     "GetBucketTaggingResultTypeDef",
     {
         "TagSet": List[S3TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobTaggingResultTypeDef = TypedDict(
     "GetJobTaggingResultTypeDef",
     {
         "Tags": List[S3TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": str,
@@ -1775,40 +1797,40 @@
     total=False,
 )
 
 GetAccessPointPolicyStatusForObjectLambdaResultTypeDef = TypedDict(
     "GetAccessPointPolicyStatusForObjectLambdaResultTypeDef",
     {
         "PolicyStatus": PolicyStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccessPointPolicyStatusResultTypeDef = TypedDict(
     "GetAccessPointPolicyStatusResultTypeDef",
     {
         "PolicyStatus": PolicyStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMultiRegionAccessPointPolicyStatusResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointPolicyStatusResultTypeDef",
     {
         "Established": PolicyStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMultiRegionAccessPointRoutesResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointRoutesResultTypeDef",
     {
         "Mrap": str,
         "Routes": List[MultiRegionAccessPointRouteTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef = TypedDict(
     "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -1817,15 +1839,15 @@
     },
 )
 
 GetStorageLensConfigurationTaggingResultTypeDef = TypedDict(
     "GetStorageLensConfigurationTaggingResultTypeDef",
     {
         "Tags": List[StorageLensTagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutStorageLensConfigurationTaggingRequestRequestTypeDef = TypedDict(
     "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
     {
         "ConfigId": str,
@@ -1858,51 +1880,29 @@
         "NumberOfTasksSucceeded": int,
         "NumberOfTasksFailed": int,
         "Timers": JobTimersTypeDef,
     },
     total=False,
 )
 
-_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
-    "_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
-    "_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef(
-    _RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
-    _OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
-):
-    pass
-
-
 ListRegionalBucketsResultTypeDef = TypedDict(
     "ListRegionalBucketsResultTypeDef",
     {
         "RegionalBucketList": List[RegionalBucketTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStorageLensConfigurationsResultTypeDef = TypedDict(
     "ListStorageLensConfigurationsResultTypeDef",
     {
         "NextToken": str,
         "StorageLensConfigurationList": List[ListStorageLensConfigurationEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMetricsTypeDef = TypedDict(
     "_RequiredMetricsTypeDef",
     {
         "Status": MetricsStatusType,
@@ -2048,15 +2048,15 @@
 )
 
 ListAccessPointsResultTypeDef = TypedDict(
     "ListAccessPointsResultTypeDef",
     {
         "AccessPointList": List[AccessPointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ObjectLambdaTransformationConfigurationTypeDef = TypedDict(
     "ObjectLambdaTransformationConfigurationTypeDef",
     {
         "Actions": Sequence[ObjectLambdaTransformationConfigurationActionType],
@@ -2065,15 +2065,15 @@
 )
 
 ListAccessPointsForObjectLambdaResultTypeDef = TypedDict(
     "ListAccessPointsForObjectLambdaResultTypeDef",
     {
         "ObjectLambdaAccessPointList": List[ObjectLambdaAccessPointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": str,
@@ -2186,15 +2186,15 @@
     pass
 
 
 GetMultiRegionAccessPointPolicyResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointPolicyResultTypeDef",
     {
         "Policy": MultiRegionAccessPointPolicyDocumentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AsyncResponseDetailsTypeDef = TypedDict(
     "AsyncResponseDetailsTypeDef",
     {
         "MultiRegionAccessPointDetails": MultiRegionAccessPointsAsyncResponseTypeDef,
@@ -2203,24 +2203,24 @@
     total=False,
 )
 
 GetMultiRegionAccessPointResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointResultTypeDef",
     {
         "AccessPoint": MultiRegionAccessPointReportTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMultiRegionAccessPointsResultTypeDef = TypedDict(
     "ListMultiRegionAccessPointsResultTypeDef",
     {
         "AccessPoints": List[MultiRegionAccessPointReportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PrefixLevelTypeDef = TypedDict(
     "PrefixLevelTypeDef",
     {
         "StorageMetrics": PrefixLevelStorageMetricsTypeDef,
@@ -2371,15 +2371,15 @@
 
 
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "NextToken": str,
         "Jobs": List[JobListDescriptorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredReplicationRuleTypeDef = TypedDict(
     "_RequiredReplicationRuleTypeDef",
     {
         "Status": ReplicationRuleStatusType,
@@ -2458,15 +2458,15 @@
     },
 )
 
 GetAccessPointConfigurationForObjectLambdaResultTypeDef = TypedDict(
     "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
     {
         "Configuration": ObjectLambdaConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef = TypedDict(
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -2475,15 +2475,15 @@
     },
 )
 
 GetBucketLifecycleConfigurationResultTypeDef = TypedDict(
     "GetBucketLifecycleConfigurationResultTypeDef",
     {
         "Rules": List[LifecycleRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LifecycleConfigurationTypeDef = TypedDict(
     "LifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[LifecycleRuleTypeDef],
@@ -2507,15 +2507,15 @@
     },
 )
 
 DescribeMultiRegionAccessPointOperationResultTypeDef = TypedDict(
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
     {
         "AsyncOperation": AsyncOperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAccountLevelTypeDef = TypedDict(
     "_RequiredAccountLevelTypeDef",
     {
         "BucketLevel": BucketLevelTypeDef,
@@ -2568,15 +2568,15 @@
     pass
 
 
 GetBucketReplicationResultTypeDef = TypedDict(
     "GetBucketReplicationResultTypeDef",
     {
         "ReplicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutBucketReplicationRequestRequestTypeDef = TypedDict(
     "PutBucketReplicationRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -2628,15 +2628,15 @@
     total=False,
 )
 
 GetStorageLensConfigurationResultTypeDef = TypedDict(
     "GetStorageLensConfigurationResultTypeDef",
     {
         "StorageLensConfiguration": StorageLensConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutStorageLensConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutStorageLensConfigurationRequestRequestTypeDef",
     {
         "ConfigId": str,
@@ -2716,10 +2716,10 @@
     total=False,
 )
 
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "Job": JobDescriptorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control/type_defs.pyi` & `mypy-boto3-s3control-1.27.0/mypy_boto3_s3control/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -77,55 +77,65 @@
     "DetailedStatusCodesMetricsTypeDef",
     "AsyncErrorDetailsTypeDef",
     "DeleteMultiRegionAccessPointInputTypeDef",
     "PutMultiRegionAccessPointPolicyInputTypeDef",
     "AwsLambdaTransformationTypeDef",
     "CloudWatchMetricsTypeDef",
     "ObjectLambdaAccessPointAliasTypeDef",
-    "ResponseMetadataTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
+    "CreateAccessPointResultTypeDef",
     "CreateBucketConfigurationTypeDef",
+    "CreateBucketResultTypeDef",
     "JobReportTypeDef",
     "S3TagTypeDef",
+    "CreateJobResultTypeDef",
     "RegionTypeDef",
+    "CreateMultiRegionAccessPointResultTypeDef",
     "DeleteAccessPointForObjectLambdaRequestRequestTypeDef",
     "DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "DeleteAccessPointPolicyRequestRequestTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteBucketLifecycleConfigurationRequestRequestTypeDef",
     "DeleteBucketPolicyRequestRequestTypeDef",
     "DeleteBucketReplicationRequestRequestTypeDef",
     "DeleteBucketRequestRequestTypeDef",
     "DeleteBucketTaggingRequestRequestTypeDef",
     "DeleteJobTaggingRequestRequestTypeDef",
     "DeleteMarkerReplicationTypeDef",
+    "DeleteMultiRegionAccessPointResultTypeDef",
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "DeleteStorageLensConfigurationRequestRequestTypeDef",
     "DeleteStorageLensConfigurationTaggingRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeMultiRegionAccessPointOperationRequestRequestTypeDef",
     "EncryptionConfigurationTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EstablishedMultiRegionAccessPointPolicyTypeDef",
     "ExcludeTypeDef",
     "ExistingObjectReplicationTypeDef",
     "SSEKMSEncryptionTypeDef",
     "GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
+    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
     "GetAccessPointPolicyRequestRequestTypeDef",
+    "GetAccessPointPolicyResultTypeDef",
     "GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef",
     "PolicyStatusTypeDef",
     "GetAccessPointPolicyStatusRequestRequestTypeDef",
     "GetAccessPointRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketPolicyRequestRequestTypeDef",
+    "GetBucketPolicyResultTypeDef",
     "GetBucketReplicationRequestRequestTypeDef",
     "GetBucketRequestRequestTypeDef",
+    "GetBucketResultTypeDef",
     "GetBucketTaggingRequestRequestTypeDef",
     "GetBucketVersioningRequestRequestTypeDef",
+    "GetBucketVersioningResultTypeDef",
     "GetJobTaggingRequestRequestTypeDef",
     "GetMultiRegionAccessPointPolicyRequestRequestTypeDef",
     "GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef",
     "GetMultiRegionAccessPointRequestRequestTypeDef",
     "GetMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "MultiRegionAccessPointRouteTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
@@ -140,63 +150,54 @@
     "LambdaInvokeOperationTypeDef",
     "S3InitiateRestoreObjectOperationTypeDef",
     "JobTimersTypeDef",
     "LifecycleExpirationTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
     "TransitionTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     "ListAccessPointsForObjectLambdaRequestRequestTypeDef",
     "ListAccessPointsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListMultiRegionAccessPointsRequestRequestTypeDef",
     "ListRegionalBucketsRequestRequestTypeDef",
     "RegionalBucketTypeDef",
     "ListStorageLensConfigurationEntryTypeDef",
     "ListStorageLensConfigurationsRequestRequestTypeDef",
     "ReplicationTimeValueTypeDef",
     "ProposedMultiRegionAccessPointPolicyTypeDef",
     "MultiRegionAccessPointRegionalResponseTypeDef",
     "RegionReportTypeDef",
+    "PaginatorConfigTypeDef",
     "SelectionCriteriaTypeDef",
     "PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "PutAccessPointPolicyRequestRequestTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "VersioningConfigurationTypeDef",
+    "PutMultiRegionAccessPointPolicyResultTypeDef",
     "ReplicaModificationsTypeDef",
+    "ResponseMetadataTypeDef",
     "S3ObjectOwnerTypeDef",
     "S3ObjectMetadataTypeDef",
     "S3GranteeTypeDef",
     "S3ObjectLockLegalHoldTypeDef",
     "S3RetentionTypeDef",
     "SSEKMSTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
     "StorageLensAwsOrgTypeDef",
     "UpdateJobPriorityRequestRequestTypeDef",
+    "UpdateJobPriorityResultTypeDef",
     "UpdateJobStatusRequestRequestTypeDef",
+    "UpdateJobStatusResultTypeDef",
     "AccessPointTypeDef",
     "DeleteMultiRegionAccessPointRequestRequestTypeDef",
     "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
     "ObjectLambdaContentTransformationTypeDef",
-    "ObjectLambdaAccessPointTypeDef",
     "CreateAccessPointForObjectLambdaResultTypeDef",
-    "CreateAccessPointResultTypeDef",
-    "CreateBucketResultTypeDef",
-    "CreateJobResultTypeDef",
-    "CreateMultiRegionAccessPointResultTypeDef",
-    "DeleteMultiRegionAccessPointResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
-    "GetAccessPointPolicyResultTypeDef",
-    "GetBucketPolicyResultTypeDef",
-    "GetBucketResultTypeDef",
-    "GetBucketVersioningResultTypeDef",
-    "PutMultiRegionAccessPointPolicyResultTypeDef",
-    "UpdateJobPriorityResultTypeDef",
-    "UpdateJobStatusResultTypeDef",
+    "ObjectLambdaAccessPointTypeDef",
     "CreateAccessPointRequestRequestTypeDef",
     "GetAccessPointForObjectLambdaResultTypeDef",
     "GetAccessPointResultTypeDef",
     "GetPublicAccessBlockOutputTypeDef",
     "PutPublicAccessBlockRequestRequestTypeDef",
     "CreateBucketRequestRequestTypeDef",
     "GetBucketTaggingResultTypeDef",
@@ -214,15 +215,14 @@
     "GetMultiRegionAccessPointRoutesResultTypeDef",
     "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingResultTypeDef",
     "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
     "S3GeneratedManifestDescriptorTypeDef",
     "JobManifestTypeDef",
     "JobProgressSummaryTypeDef",
-    "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     "ListRegionalBucketsResultTypeDef",
     "ListStorageLensConfigurationsResultTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "MultiRegionAccessPointPolicyDocumentTypeDef",
     "MultiRegionAccessPointsAsyncResponseTypeDef",
     "MultiRegionAccessPointReportTypeDef",
@@ -394,44 +394,51 @@
     {
         "Value": str,
         "Status": ObjectLambdaAccessPointAliasStatusType,
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
 PublicAccessBlockConfigurationTypeDef = TypedDict(
     "PublicAccessBlockConfigurationTypeDef",
     {
         "BlockPublicAcls": bool,
         "IgnorePublicAcls": bool,
         "BlockPublicPolicy": bool,
         "RestrictPublicBuckets": bool,
     },
     total=False,
 )
 
+CreateAccessPointResultTypeDef = TypedDict(
+    "CreateAccessPointResultTypeDef",
+    {
+        "AccessPointArn": str,
+        "Alias": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateBucketConfigurationTypeDef = TypedDict(
     "CreateBucketConfigurationTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
     },
     total=False,
 )
 
+CreateBucketResultTypeDef = TypedDict(
+    "CreateBucketResultTypeDef",
+    {
+        "Location": str,
+        "BucketArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredJobReportTypeDef = TypedDict(
     "_RequiredJobReportTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalJobReportTypeDef = TypedDict(
@@ -452,14 +459,22 @@
     "S3TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateJobResultTypeDef = TypedDict(
+    "CreateJobResultTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRegionTypeDef = TypedDict(
     "_RequiredRegionTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalRegionTypeDef = TypedDict(
@@ -469,14 +484,22 @@
     },
     total=False,
 )
 
 class RegionTypeDef(_RequiredRegionTypeDef, _OptionalRegionTypeDef):
     pass
 
+CreateMultiRegionAccessPointResultTypeDef = TypedDict(
+    "CreateMultiRegionAccessPointResultTypeDef",
+    {
+        "RequestTokenARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteAccessPointForObjectLambdaRequestRequestTypeDef = TypedDict(
     "DeleteAccessPointForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
@@ -556,14 +579,22 @@
 DeleteMarkerReplicationTypeDef = TypedDict(
     "DeleteMarkerReplicationTypeDef",
     {
         "Status": DeleteMarkerReplicationStatusType,
     },
 )
 
+DeleteMultiRegionAccessPointResultTypeDef = TypedDict(
+    "DeleteMultiRegionAccessPointResultTypeDef",
+    {
+        "RequestTokenARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePublicAccessBlockRequestRequestTypeDef = TypedDict(
     "DeletePublicAccessBlockRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 
@@ -603,14 +634,21 @@
     "EncryptionConfigurationTypeDef",
     {
         "ReplicaKmsKeyID": str,
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
 EstablishedMultiRegionAccessPointPolicyTypeDef = TypedDict(
     "EstablishedMultiRegionAccessPointPolicyTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
@@ -658,22 +696,38 @@
     "GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
 
+GetAccessPointPolicyForObjectLambdaResultTypeDef = TypedDict(
+    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAccessPointPolicyRequestRequestTypeDef = TypedDict(
     "GetAccessPointPolicyRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
 
+GetAccessPointPolicyResultTypeDef = TypedDict(
+    "GetAccessPointPolicyResultTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef = TypedDict(
     "GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
@@ -714,14 +768,22 @@
     "GetBucketPolicyRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
 
+GetBucketPolicyResultTypeDef = TypedDict(
+    "GetBucketPolicyResultTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBucketReplicationRequestRequestTypeDef = TypedDict(
     "GetBucketReplicationRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
@@ -730,14 +792,24 @@
     "GetBucketRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
 
+GetBucketResultTypeDef = TypedDict(
+    "GetBucketResultTypeDef",
+    {
+        "Bucket": str,
+        "PublicAccessBlockEnabled": bool,
+        "CreationDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBucketTaggingRequestRequestTypeDef = TypedDict(
     "GetBucketTaggingRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
@@ -746,14 +818,23 @@
     "GetBucketVersioningRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
 
+GetBucketVersioningResultTypeDef = TypedDict(
+    "GetBucketVersioningResultTypeDef",
+    {
+        "Status": BucketVersioningStatusType,
+        "MFADelete": MFADeleteStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetJobTaggingRequestRequestTypeDef = TypedDict(
     "GetJobTaggingRequestRequestTypeDef",
     {
         "AccountId": str,
         "JobId": str,
     },
 )
@@ -966,24 +1047,34 @@
         "Date": datetime,
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
+    "_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "AccountId": str,
+    },
+)
+_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
+    "_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef(
+    _RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
+    _OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
+):
+    pass
+
 _RequiredListAccessPointsForObjectLambdaRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessPointsForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListAccessPointsForObjectLambdaRequestRequestTypeDef = TypedDict(
@@ -1179,14 +1270,24 @@
         "Bucket": str,
         "Region": str,
         "BucketAccountId": str,
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
 SelectionCriteriaTypeDef = TypedDict(
     "SelectionCriteriaTypeDef",
     {
         "Delimiter": str,
         "MaxDepth": int,
         "MinStorageBytesPercentage": float,
     },
@@ -1237,21 +1338,40 @@
     {
         "MFADelete": MFADeleteType,
         "Status": BucketVersioningStatusType,
     },
     total=False,
 )
 
+PutMultiRegionAccessPointPolicyResultTypeDef = TypedDict(
+    "PutMultiRegionAccessPointPolicyResultTypeDef",
+    {
+        "RequestTokenARN": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ReplicaModificationsTypeDef = TypedDict(
     "ReplicaModificationsTypeDef",
     {
         "Status": ReplicaModificationsStatusType,
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
 S3ObjectOwnerTypeDef = TypedDict(
     "S3ObjectOwnerTypeDef",
     {
         "ID": str,
         "DisplayName": str,
     },
     total=False,
@@ -1327,14 +1447,23 @@
     {
         "AccountId": str,
         "JobId": str,
         "Priority": int,
     },
 )
 
+UpdateJobPriorityResultTypeDef = TypedDict(
+    "UpdateJobPriorityResultTypeDef",
+    {
+        "JobId": str,
+        "Priority": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateJobStatusRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobStatusRequestRequestTypeDef",
     {
         "AccountId": str,
         "JobId": str,
         "RequestedJobStatus": RequestedJobStatusType,
     },
@@ -1348,14 +1477,24 @@
 )
 
 class UpdateJobStatusRequestRequestTypeDef(
     _RequiredUpdateJobStatusRequestRequestTypeDef, _OptionalUpdateJobStatusRequestRequestTypeDef
 ):
     pass
 
+UpdateJobStatusResultTypeDef = TypedDict(
+    "UpdateJobStatusResultTypeDef",
+    {
+        "JobId": str,
+        "Status": JobStatusType,
+        "StatusUpdateReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredAccessPointTypeDef = TypedDict(
     "_RequiredAccessPointTypeDef",
     {
         "Name": str,
         "NetworkOrigin": NetworkOriginType,
         "Bucket": str,
     },
@@ -1396,14 +1535,23 @@
     "ObjectLambdaContentTransformationTypeDef",
     {
         "AwsLambda": AwsLambdaTransformationTypeDef,
     },
     total=False,
 )
 
+CreateAccessPointForObjectLambdaResultTypeDef = TypedDict(
+    "CreateAccessPointForObjectLambdaResultTypeDef",
+    {
+        "ObjectLambdaAccessPointArn": str,
+        "Alias": ObjectLambdaAccessPointAliasTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredObjectLambdaAccessPointTypeDef = TypedDict(
     "_RequiredObjectLambdaAccessPointTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalObjectLambdaAccessPointTypeDef = TypedDict(
@@ -1416,142 +1564,14 @@
 )
 
 class ObjectLambdaAccessPointTypeDef(
     _RequiredObjectLambdaAccessPointTypeDef, _OptionalObjectLambdaAccessPointTypeDef
 ):
     pass
 
-CreateAccessPointForObjectLambdaResultTypeDef = TypedDict(
-    "CreateAccessPointForObjectLambdaResultTypeDef",
-    {
-        "ObjectLambdaAccessPointArn": str,
-        "Alias": ObjectLambdaAccessPointAliasTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAccessPointResultTypeDef = TypedDict(
-    "CreateAccessPointResultTypeDef",
-    {
-        "AccessPointArn": str,
-        "Alias": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBucketResultTypeDef = TypedDict(
-    "CreateBucketResultTypeDef",
-    {
-        "Location": str,
-        "BucketArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobResultTypeDef = TypedDict(
-    "CreateJobResultTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMultiRegionAccessPointResultTypeDef = TypedDict(
-    "CreateMultiRegionAccessPointResultTypeDef",
-    {
-        "RequestTokenARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteMultiRegionAccessPointResultTypeDef = TypedDict(
-    "DeleteMultiRegionAccessPointResultTypeDef",
-    {
-        "RequestTokenARN": str,
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
-GetAccessPointPolicyForObjectLambdaResultTypeDef = TypedDict(
-    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAccessPointPolicyResultTypeDef = TypedDict(
-    "GetAccessPointPolicyResultTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBucketPolicyResultTypeDef = TypedDict(
-    "GetBucketPolicyResultTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBucketResultTypeDef = TypedDict(
-    "GetBucketResultTypeDef",
-    {
-        "Bucket": str,
-        "PublicAccessBlockEnabled": bool,
-        "CreationDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBucketVersioningResultTypeDef = TypedDict(
-    "GetBucketVersioningResultTypeDef",
-    {
-        "Status": BucketVersioningStatusType,
-        "MFADelete": MFADeleteStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutMultiRegionAccessPointPolicyResultTypeDef = TypedDict(
-    "PutMultiRegionAccessPointPolicyResultTypeDef",
-    {
-        "RequestTokenARN": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateJobPriorityResultTypeDef = TypedDict(
-    "UpdateJobPriorityResultTypeDef",
-    {
-        "JobId": str,
-        "Priority": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateJobStatusResultTypeDef = TypedDict(
-    "UpdateJobStatusResultTypeDef",
-    {
-        "JobId": str,
-        "Status": JobStatusType,
-        "StatusUpdateReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateAccessPointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessPointRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
         "Bucket": str,
     },
@@ -1574,15 +1594,15 @@
 GetAccessPointForObjectLambdaResultTypeDef = TypedDict(
     "GetAccessPointForObjectLambdaResultTypeDef",
     {
         "Name": str,
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "CreationDate": datetime,
         "Alias": ObjectLambdaAccessPointAliasTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccessPointResultTypeDef = TypedDict(
     "GetAccessPointResultTypeDef",
     {
         "Name": str,
@@ -1591,23 +1611,23 @@
         "VpcConfiguration": VpcConfigurationTypeDef,
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "CreationDate": datetime,
         "Alias": str,
         "AccessPointArn": str,
         "Endpoints": Dict[str, str],
         "BucketAccountId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPublicAccessBlockOutputTypeDef = TypedDict(
     "GetPublicAccessBlockOutputTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "PutPublicAccessBlockRequestRequestTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
@@ -1642,23 +1662,23 @@
 ):
     pass
 
 GetBucketTaggingResultTypeDef = TypedDict(
     "GetBucketTaggingResultTypeDef",
     {
         "TagSet": List[S3TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobTaggingResultTypeDef = TypedDict(
     "GetJobTaggingResultTypeDef",
     {
         "Tags": List[S3TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": str,
@@ -1732,40 +1752,40 @@
     total=False,
 )
 
 GetAccessPointPolicyStatusForObjectLambdaResultTypeDef = TypedDict(
     "GetAccessPointPolicyStatusForObjectLambdaResultTypeDef",
     {
         "PolicyStatus": PolicyStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccessPointPolicyStatusResultTypeDef = TypedDict(
     "GetAccessPointPolicyStatusResultTypeDef",
     {
         "PolicyStatus": PolicyStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMultiRegionAccessPointPolicyStatusResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointPolicyStatusResultTypeDef",
     {
         "Established": PolicyStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMultiRegionAccessPointRoutesResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointRoutesResultTypeDef",
     {
         "Mrap": str,
         "Routes": List[MultiRegionAccessPointRouteTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef = TypedDict(
     "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -1774,15 +1794,15 @@
     },
 )
 
 GetStorageLensConfigurationTaggingResultTypeDef = TypedDict(
     "GetStorageLensConfigurationTaggingResultTypeDef",
     {
         "Tags": List[StorageLensTagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutStorageLensConfigurationTaggingRequestRequestTypeDef = TypedDict(
     "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
     {
         "ConfigId": str,
@@ -1815,49 +1835,29 @@
         "NumberOfTasksSucceeded": int,
         "NumberOfTasksFailed": int,
         "Timers": JobTimersTypeDef,
     },
     total=False,
 )
 
-_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
-    "_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
-    "_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef(
-    _RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
-    _OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
-):
-    pass
-
 ListRegionalBucketsResultTypeDef = TypedDict(
     "ListRegionalBucketsResultTypeDef",
     {
         "RegionalBucketList": List[RegionalBucketTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStorageLensConfigurationsResultTypeDef = TypedDict(
     "ListStorageLensConfigurationsResultTypeDef",
     {
         "NextToken": str,
         "StorageLensConfigurationList": List[ListStorageLensConfigurationEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredMetricsTypeDef = TypedDict(
     "_RequiredMetricsTypeDef",
     {
         "Status": MetricsStatusType,
@@ -1997,15 +1997,15 @@
 )
 
 ListAccessPointsResultTypeDef = TypedDict(
     "ListAccessPointsResultTypeDef",
     {
         "AccessPointList": List[AccessPointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ObjectLambdaTransformationConfigurationTypeDef = TypedDict(
     "ObjectLambdaTransformationConfigurationTypeDef",
     {
         "Actions": Sequence[ObjectLambdaTransformationConfigurationActionType],
@@ -2014,15 +2014,15 @@
 )
 
 ListAccessPointsForObjectLambdaResultTypeDef = TypedDict(
     "ListAccessPointsForObjectLambdaResultTypeDef",
     {
         "ObjectLambdaAccessPointList": List[ObjectLambdaAccessPointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": str,
@@ -2131,15 +2131,15 @@
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
 GetMultiRegionAccessPointPolicyResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointPolicyResultTypeDef",
     {
         "Policy": MultiRegionAccessPointPolicyDocumentTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AsyncResponseDetailsTypeDef = TypedDict(
     "AsyncResponseDetailsTypeDef",
     {
         "MultiRegionAccessPointDetails": MultiRegionAccessPointsAsyncResponseTypeDef,
@@ -2148,24 +2148,24 @@
     total=False,
 )
 
 GetMultiRegionAccessPointResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointResultTypeDef",
     {
         "AccessPoint": MultiRegionAccessPointReportTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMultiRegionAccessPointsResultTypeDef = TypedDict(
     "ListMultiRegionAccessPointsResultTypeDef",
     {
         "AccessPoints": List[MultiRegionAccessPointReportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PrefixLevelTypeDef = TypedDict(
     "PrefixLevelTypeDef",
     {
         "StorageMetrics": PrefixLevelStorageMetricsTypeDef,
@@ -2306,15 +2306,15 @@
     pass
 
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "NextToken": str,
         "Jobs": List[JobListDescriptorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredReplicationRuleTypeDef = TypedDict(
     "_RequiredReplicationRuleTypeDef",
     {
         "Status": ReplicationRuleStatusType,
@@ -2391,15 +2391,15 @@
     },
 )
 
 GetAccessPointConfigurationForObjectLambdaResultTypeDef = TypedDict(
     "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
     {
         "Configuration": ObjectLambdaConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef = TypedDict(
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -2408,15 +2408,15 @@
     },
 )
 
 GetBucketLifecycleConfigurationResultTypeDef = TypedDict(
     "GetBucketLifecycleConfigurationResultTypeDef",
     {
         "Rules": List[LifecycleRuleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LifecycleConfigurationTypeDef = TypedDict(
     "LifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[LifecycleRuleTypeDef],
@@ -2440,15 +2440,15 @@
     },
 )
 
 DescribeMultiRegionAccessPointOperationResultTypeDef = TypedDict(
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
     {
         "AsyncOperation": AsyncOperationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAccountLevelTypeDef = TypedDict(
     "_RequiredAccountLevelTypeDef",
     {
         "BucketLevel": BucketLevelTypeDef,
@@ -2497,15 +2497,15 @@
 ):
     pass
 
 GetBucketReplicationResultTypeDef = TypedDict(
     "GetBucketReplicationResultTypeDef",
     {
         "ReplicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutBucketReplicationRequestRequestTypeDef = TypedDict(
     "PutBucketReplicationRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -2555,15 +2555,15 @@
     total=False,
 )
 
 GetStorageLensConfigurationResultTypeDef = TypedDict(
     "GetStorageLensConfigurationResultTypeDef",
     {
         "StorageLensConfiguration": StorageLensConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutStorageLensConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutStorageLensConfigurationRequestRequestTypeDef",
     {
         "ConfigId": str,
@@ -2639,10 +2639,10 @@
     total=False,
 )
 
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "Job": JobDescriptorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/PKG-INFO` & `mypy-boto3-s3control-1.27.0/mypy_boto3_s3control.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3control
-Version: 1.26.92
-Summary: Type annotations for boto3.S3Control 1.26.92 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.S3Control 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-s3control"></a>
 
 # mypy-boto3-s3control
 
 [![PyPI - mypy-boto3-s3control](https://img.shields.io/pypi/v/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3control?color=blue)](https://pypistats.org/packages/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.26.92](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
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
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
 See how it helps to find and fix potential bugs:
 
@@ -377,55 +377,65 @@
     DetailedStatusCodesMetricsTypeDef,
     AsyncErrorDetailsTypeDef,
     DeleteMultiRegionAccessPointInputTypeDef,
     PutMultiRegionAccessPointPolicyInputTypeDef,
     AwsLambdaTransformationTypeDef,
     CloudWatchMetricsTypeDef,
     ObjectLambdaAccessPointAliasTypeDef,
-    ResponseMetadataTypeDef,
     PublicAccessBlockConfigurationTypeDef,
+    CreateAccessPointResultTypeDef,
     CreateBucketConfigurationTypeDef,
+    CreateBucketResultTypeDef,
     JobReportTypeDef,
     S3TagTypeDef,
+    CreateJobResultTypeDef,
     RegionTypeDef,
+    CreateMultiRegionAccessPointResultTypeDef,
     DeleteAccessPointForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyRequestRequestTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteBucketLifecycleConfigurationRequestRequestTypeDef,
     DeleteBucketPolicyRequestRequestTypeDef,
     DeleteBucketReplicationRequestRequestTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteJobTaggingRequestRequestTypeDef,
     DeleteMarkerReplicationTypeDef,
+    DeleteMultiRegionAccessPointResultTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     DeleteStorageLensConfigurationRequestRequestTypeDef,
     DeleteStorageLensConfigurationTaggingRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeMultiRegionAccessPointOperationRequestRequestTypeDef,
     EncryptionConfigurationTypeDef,
+    EmptyResponseMetadataTypeDef,
     EstablishedMultiRegionAccessPointPolicyTypeDef,
     ExcludeTypeDef,
     ExistingObjectReplicationTypeDef,
     SSEKMSEncryptionTypeDef,
     GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
     GetAccessPointForObjectLambdaRequestRequestTypeDef,
     GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
+    GetAccessPointPolicyForObjectLambdaResultTypeDef,
     GetAccessPointPolicyRequestRequestTypeDef,
+    GetAccessPointPolicyResultTypeDef,
     GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef,
     PolicyStatusTypeDef,
     GetAccessPointPolicyStatusRequestRequestTypeDef,
     GetAccessPointRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
+    GetBucketPolicyResultTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
     GetBucketRequestRequestTypeDef,
+    GetBucketResultTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
+    GetBucketVersioningResultTypeDef,
     GetJobTaggingRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef,
     GetMultiRegionAccessPointRequestRequestTypeDef,
     GetMultiRegionAccessPointRoutesRequestRequestTypeDef,
     MultiRegionAccessPointRouteTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
@@ -440,63 +450,54 @@
     LambdaInvokeOperationTypeDef,
     S3InitiateRestoreObjectOperationTypeDef,
     JobTimersTypeDef,
     LifecycleExpirationTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
-    PaginatorConfigTypeDef,
+    ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     ListAccessPointsForObjectLambdaRequestRequestTypeDef,
     ListAccessPointsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListMultiRegionAccessPointsRequestRequestTypeDef,
     ListRegionalBucketsRequestRequestTypeDef,
     RegionalBucketTypeDef,
     ListStorageLensConfigurationEntryTypeDef,
     ListStorageLensConfigurationsRequestRequestTypeDef,
     ReplicationTimeValueTypeDef,
     ProposedMultiRegionAccessPointPolicyTypeDef,
     MultiRegionAccessPointRegionalResponseTypeDef,
     RegionReportTypeDef,
+    PaginatorConfigTypeDef,
     SelectionCriteriaTypeDef,
     PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     PutAccessPointPolicyRequestRequestTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     VersioningConfigurationTypeDef,
+    PutMultiRegionAccessPointPolicyResultTypeDef,
     ReplicaModificationsTypeDef,
+    ResponseMetadataTypeDef,
     S3ObjectOwnerTypeDef,
     S3ObjectMetadataTypeDef,
     S3GranteeTypeDef,
     S3ObjectLockLegalHoldTypeDef,
     S3RetentionTypeDef,
     SSEKMSTypeDef,
     SseKmsEncryptedObjectsTypeDef,
     StorageLensAwsOrgTypeDef,
     UpdateJobPriorityRequestRequestTypeDef,
+    UpdateJobPriorityResultTypeDef,
     UpdateJobStatusRequestRequestTypeDef,
+    UpdateJobStatusResultTypeDef,
     AccessPointTypeDef,
     DeleteMultiRegionAccessPointRequestRequestTypeDef,
     PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
     ObjectLambdaContentTransformationTypeDef,
-    ObjectLambdaAccessPointTypeDef,
     CreateAccessPointForObjectLambdaResultTypeDef,
-    CreateAccessPointResultTypeDef,
-    CreateBucketResultTypeDef,
-    CreateJobResultTypeDef,
-    CreateMultiRegionAccessPointResultTypeDef,
-    DeleteMultiRegionAccessPointResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAccessPointPolicyForObjectLambdaResultTypeDef,
-    GetAccessPointPolicyResultTypeDef,
-    GetBucketPolicyResultTypeDef,
-    GetBucketResultTypeDef,
-    GetBucketVersioningResultTypeDef,
-    PutMultiRegionAccessPointPolicyResultTypeDef,
-    UpdateJobPriorityResultTypeDef,
-    UpdateJobStatusResultTypeDef,
+    ObjectLambdaAccessPointTypeDef,
     CreateAccessPointRequestRequestTypeDef,
     GetAccessPointForObjectLambdaResultTypeDef,
     GetAccessPointResultTypeDef,
     GetPublicAccessBlockOutputTypeDef,
     PutPublicAccessBlockRequestRequestTypeDef,
     CreateBucketRequestRequestTypeDef,
     GetBucketTaggingResultTypeDef,
@@ -514,15 +515,14 @@
     GetMultiRegionAccessPointRoutesResultTypeDef,
     SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
     PutStorageLensConfigurationTaggingRequestRequestTypeDef,
     S3GeneratedManifestDescriptorTypeDef,
     JobManifestTypeDef,
     JobProgressSummaryTypeDef,
-    ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     MultiRegionAccessPointPolicyDocumentTypeDef,
     MultiRegionAccessPointsAsyncResponseTypeDef,
     MultiRegionAccessPointReportTypeDef,
@@ -591,42 +591,42 @@
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

### Comparing `mypy-boto3-s3control-1.26.92/mypy_boto3_s3control.egg-info/SOURCES.txt` & `mypy-boto3-s3control-1.27.0/mypy_boto3_s3control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.26.92/setup.py` & `mypy-boto3-s3control-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-s3control.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-s3control",
-    version="1.26.92",
+    version="1.27.0",
     packages=["mypy_boto3_s3control"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.S3Control 1.26.92 service generated with mypy-boto3-builder"
-        " 7.13.0"
+        "Type annotations for boto3.S3Control 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/",
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


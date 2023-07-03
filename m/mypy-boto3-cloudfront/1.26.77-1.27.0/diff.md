# Comparing `tmp/mypy-boto3-cloudfront-1.26.77.tar.gz` & `tmp/mypy-boto3-cloudfront-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudfront-1.26.77.tar", last modified: Wed Feb 22 20:34:22 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudfront-1.27.0.tar", last modified: Mon Jul  3 19:50:29 2023, max compression
```

## Comparing `mypy-boto3-cloudfront-1.26.77.tar` & `mypy-boto3-cloudfront-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.526112 mypy-boto3-cloudfront-1.26.77/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-22 20:33:51.000000 mypy-boto3-cloudfront-1.26.77/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30713 2023-02-22 20:34:22.518112 mypy-boto3-cloudfront-1.26.77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    29214 2023-02-22 20:33:51.000000 mypy-boto3-cloudfront-1.26.77/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.518112 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-02-22 20:33:51.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-02-22 20:33:51.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-22 20:33:51.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79426 2023-02-22 20:33:52.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    79306 2023-02-22 20:33:52.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12243 2023-02-22 20:33:53.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-02-22 20:33:52.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-02-22 20:33:52.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-02-22 20:33:52.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 20:33:51.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   138327 2023-02-22 20:33:56.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   138064 2023-02-22 20:33:54.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-22 20:33:51.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-02-22 20:33:52.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-02-22 20:33:52.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.518112 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30713 2023-02-22 20:34:22.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-02-22 20:34:22.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-22 20:34:22.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 20:34:22.000000 mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 20:34:22.526112 mypy-boto3-cloudfront-1.26.77/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-02-22 20:33:51.000000 mypy-boto3-cloudfront-1.26.77/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.458944 mypy-boto3-cloudfront-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:49.000000 mypy-boto3-cloudfront-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    30692 2023-07-03 19:50:29.458944 mypy-boto3-cloudfront-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    29195 2023-07-03 19:33:49.000000 mypy-boto3-cloudfront-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.458944 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-03 19:33:49.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-03 19:33:49.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:33:49.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79436 2023-07-03 19:33:50.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79316 2023-07-03 19:33:49.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-03 19:33:50.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-03 19:33:50.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-03 19:33:50.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-03 19:33:50.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:49.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   138513 2023-07-03 19:33:53.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138250 2023-07-03 19:33:51.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:49.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-03 19:33:50.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-03 19:33:50.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:29.458944 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30692 2023-07-03 19:50:29.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-03 19:50:29.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:29.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:29.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:29.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:50:29.000000 mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:29.458944 mypy-boto3-cloudfront-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:33:48.000000 mypy-boto3-cloudfront-1.27.0/setup.py
```

### Comparing `mypy-boto3-cloudfront-1.26.77/LICENSE` & `mypy-boto3-cloudfront-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-cloudfront-1.26.77/PKG-INFO` & `mypy-boto3-cloudfront-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudfront
-Version: 1.26.77
-Summary: Type annotations for boto3.CloudFront 1.26.77 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudFront 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-cloudfront"></a>
 
 # mypy-boto3-cloudfront
 
 [![PyPI - mypy-boto3-cloudfront](https://img.shields.io/pypi/v/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudfront?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
 
@@ -423,15 +423,14 @@
     CloudFrontOriginAccessIdentitySummaryTypeDef,
     ConflictingAliasTypeDef,
     ContentTypeProfileTypeDef,
     StagingDistributionDnsNamesTypeDef,
     ContinuousDeploymentSingleHeaderConfigTypeDef,
     SessionStickinessConfigTypeDef,
     CopyDistributionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     FunctionConfigTypeDef,
     KeyGroupConfigTypeDef,
     OriginAccessControlConfigTypeDef,
     PublicKeyConfigTypeDef,
     CustomErrorResponseTypeDef,
     OriginCustomHeaderTypeDef,
     OriginSslProtocolsTypeDef,
@@ -450,14 +449,15 @@
     DeleteRealtimeLogConfigRequestRequestTypeDef,
     DeleteResponseHeadersPolicyRequestRequestTypeDef,
     DeleteStreamingDistributionRequestRequestTypeDef,
     DescribeFunctionRequestRequestTypeDef,
     LoggingConfigTypeDef,
     ViewerCertificateTypeDef,
     DistributionIdListTypeDef,
+    EmptyResponseMetadataTypeDef,
     FieldPatternsTypeDef,
     KinesisStreamConfigTypeDef,
     QueryStringCacheKeysTypeDef,
     FunctionAssociationTypeDef,
     FunctionMetadataTypeDef,
     GeoRestrictionTypeDef,
     GetCachePolicyConfigRequestRequestTypeDef,
@@ -470,14 +470,15 @@
     WaiterConfigTypeDef,
     GetDistributionRequestRequestTypeDef,
     GetFieldLevelEncryptionConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileRequestRequestTypeDef,
     GetFieldLevelEncryptionRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
+    GetFunctionResultTypeDef,
     GetInvalidationRequestRequestTypeDef,
     GetKeyGroupConfigRequestRequestTypeDef,
     GetKeyGroupRequestRequestTypeDef,
     GetMonitoringSubscriptionRequestRequestTypeDef,
     GetOriginAccessControlConfigRequestRequestTypeDef,
     GetOriginAccessControlRequestRequestTypeDef,
     GetOriginRequestPolicyConfigRequestRequestTypeDef,
@@ -490,43 +491,47 @@
     GetStreamingDistributionConfigRequestRequestTypeDef,
     GetStreamingDistributionRequestRequestTypeDef,
     PathsTypeDef,
     InvalidationSummaryTypeDef,
     KeyPairIdsTypeDef,
     LambdaFunctionAssociationTypeDef,
     ListCachePoliciesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
     ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef,
     ListConflictingAliasesRequestRequestTypeDef,
     ListContinuousDeploymentPoliciesRequestRequestTypeDef,
     ListDistributionsByCachePolicyIdRequestRequestTypeDef,
     ListDistributionsByKeyGroupRequestRequestTypeDef,
     ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
     ListDistributionsByRealtimeLogConfigRequestRequestTypeDef,
     ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
     ListDistributionsByWebACLIdRequestRequestTypeDef,
+    ListDistributionsRequestListDistributionsPaginateTypeDef,
     ListDistributionsRequestRequestTypeDef,
     ListFieldLevelEncryptionConfigsRequestRequestTypeDef,
     ListFieldLevelEncryptionProfilesRequestRequestTypeDef,
     ListFunctionsRequestRequestTypeDef,
+    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
     ListInvalidationsRequestRequestTypeDef,
     ListKeyGroupsRequestRequestTypeDef,
     ListOriginAccessControlsRequestRequestTypeDef,
     ListOriginRequestPoliciesRequestRequestTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     ListRealtimeLogConfigsRequestRequestTypeDef,
     ListResponseHeadersPoliciesRequestRequestTypeDef,
+    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     ListStreamingDistributionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RealtimeMetricsSubscriptionConfigTypeDef,
     OriginAccessControlSummaryTypeDef,
     StatusCodesTypeDef,
     OriginGroupMemberTypeDef,
     OriginShieldTypeDef,
     S3OriginConfigTypeDef,
+    PaginatorConfigTypeDef,
     PublicKeySummaryTypeDef,
     PublishFunctionRequestRequestTypeDef,
     QueryArgProfileTypeDef,
     ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
     ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
     ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
     ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
@@ -535,14 +540,15 @@
     ResponseHeadersPolicyContentTypeOptionsTypeDef,
     ResponseHeadersPolicyCustomHeaderTypeDef,
     ResponseHeadersPolicyFrameOptionsTypeDef,
     ResponseHeadersPolicyReferrerPolicyTypeDef,
     ResponseHeadersPolicyRemoveHeaderTypeDef,
     ResponseHeadersPolicyStrictTransportSecurityTypeDef,
     ResponseHeadersPolicyXSSProtectionTypeDef,
+    ResponseMetadataTypeDef,
     S3OriginTypeDef,
     StreamingLoggingConfigTypeDef,
     TagKeysTypeDef,
     TagTypeDef,
     TestFunctionRequestRequestTypeDef,
     UpdateDistributionWithStagingConfigRequestRequestTypeDef,
     AllowedMethodsTypeDef,
@@ -551,22 +557,20 @@
     OriginRequestPolicyCookiesConfigTypeDef,
     CachePolicyHeadersConfigTypeDef,
     OriginRequestPolicyHeadersConfigTypeDef,
     CachePolicyQueryStringsConfigTypeDef,
     OriginRequestPolicyQueryStringsConfigTypeDef,
     CloudFrontOriginAccessIdentityTypeDef,
     CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
+    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     CloudFrontOriginAccessIdentityListTypeDef,
     ConflictingAliasesListTypeDef,
     ContentTypeProfilesTypeDef,
     ContinuousDeploymentSingleWeightConfigTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
-    GetFunctionResultTypeDef,
     CreateFunctionRequestRequestTypeDef,
     UpdateFunctionRequestRequestTypeDef,
     CreateKeyGroupRequestRequestTypeDef,
     GetKeyGroupConfigResultTypeDef,
     KeyGroupTypeDef,
     UpdateKeyGroupRequestRequestTypeDef,
     CreateOriginAccessControlRequestRequestTypeDef,
@@ -593,18 +597,14 @@
     GetInvalidationRequestInvalidationCompletedWaitTypeDef,
     GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
     InvalidationBatchTypeDef,
     InvalidationListTypeDef,
     KGKeyPairIdsTypeDef,
     SignerTypeDef,
     LambdaFunctionAssociationsTypeDef,
-    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
-    ListDistributionsRequestListDistributionsPaginateTypeDef,
-    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
-    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlListTypeDef,
     OriginGroupFailoverCriteriaTypeDef,
     OriginGroupMembersTypeDef,
     PublicKeyListTypeDef,
     QueryArgProfilesTypeDef,
     ResponseHeadersPolicyCorsConfigTypeDef,
@@ -781,42 +781,42 @@
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

### Comparing `mypy-boto3-cloudfront-1.26.77/README.md` & `mypy-boto3-cloudfront-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cloudfront"></a>
 
 # mypy-boto3-cloudfront
 
 [![PyPI - mypy-boto3-cloudfront](https://img.shields.io/pypi/v/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudfront?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
 
@@ -391,15 +391,14 @@
     CloudFrontOriginAccessIdentitySummaryTypeDef,
     ConflictingAliasTypeDef,
     ContentTypeProfileTypeDef,
     StagingDistributionDnsNamesTypeDef,
     ContinuousDeploymentSingleHeaderConfigTypeDef,
     SessionStickinessConfigTypeDef,
     CopyDistributionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     FunctionConfigTypeDef,
     KeyGroupConfigTypeDef,
     OriginAccessControlConfigTypeDef,
     PublicKeyConfigTypeDef,
     CustomErrorResponseTypeDef,
     OriginCustomHeaderTypeDef,
     OriginSslProtocolsTypeDef,
@@ -418,14 +417,15 @@
     DeleteRealtimeLogConfigRequestRequestTypeDef,
     DeleteResponseHeadersPolicyRequestRequestTypeDef,
     DeleteStreamingDistributionRequestRequestTypeDef,
     DescribeFunctionRequestRequestTypeDef,
     LoggingConfigTypeDef,
     ViewerCertificateTypeDef,
     DistributionIdListTypeDef,
+    EmptyResponseMetadataTypeDef,
     FieldPatternsTypeDef,
     KinesisStreamConfigTypeDef,
     QueryStringCacheKeysTypeDef,
     FunctionAssociationTypeDef,
     FunctionMetadataTypeDef,
     GeoRestrictionTypeDef,
     GetCachePolicyConfigRequestRequestTypeDef,
@@ -438,14 +438,15 @@
     WaiterConfigTypeDef,
     GetDistributionRequestRequestTypeDef,
     GetFieldLevelEncryptionConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileRequestRequestTypeDef,
     GetFieldLevelEncryptionRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
+    GetFunctionResultTypeDef,
     GetInvalidationRequestRequestTypeDef,
     GetKeyGroupConfigRequestRequestTypeDef,
     GetKeyGroupRequestRequestTypeDef,
     GetMonitoringSubscriptionRequestRequestTypeDef,
     GetOriginAccessControlConfigRequestRequestTypeDef,
     GetOriginAccessControlRequestRequestTypeDef,
     GetOriginRequestPolicyConfigRequestRequestTypeDef,
@@ -458,43 +459,47 @@
     GetStreamingDistributionConfigRequestRequestTypeDef,
     GetStreamingDistributionRequestRequestTypeDef,
     PathsTypeDef,
     InvalidationSummaryTypeDef,
     KeyPairIdsTypeDef,
     LambdaFunctionAssociationTypeDef,
     ListCachePoliciesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
     ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef,
     ListConflictingAliasesRequestRequestTypeDef,
     ListContinuousDeploymentPoliciesRequestRequestTypeDef,
     ListDistributionsByCachePolicyIdRequestRequestTypeDef,
     ListDistributionsByKeyGroupRequestRequestTypeDef,
     ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
     ListDistributionsByRealtimeLogConfigRequestRequestTypeDef,
     ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
     ListDistributionsByWebACLIdRequestRequestTypeDef,
+    ListDistributionsRequestListDistributionsPaginateTypeDef,
     ListDistributionsRequestRequestTypeDef,
     ListFieldLevelEncryptionConfigsRequestRequestTypeDef,
     ListFieldLevelEncryptionProfilesRequestRequestTypeDef,
     ListFunctionsRequestRequestTypeDef,
+    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
     ListInvalidationsRequestRequestTypeDef,
     ListKeyGroupsRequestRequestTypeDef,
     ListOriginAccessControlsRequestRequestTypeDef,
     ListOriginRequestPoliciesRequestRequestTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     ListRealtimeLogConfigsRequestRequestTypeDef,
     ListResponseHeadersPoliciesRequestRequestTypeDef,
+    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     ListStreamingDistributionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RealtimeMetricsSubscriptionConfigTypeDef,
     OriginAccessControlSummaryTypeDef,
     StatusCodesTypeDef,
     OriginGroupMemberTypeDef,
     OriginShieldTypeDef,
     S3OriginConfigTypeDef,
+    PaginatorConfigTypeDef,
     PublicKeySummaryTypeDef,
     PublishFunctionRequestRequestTypeDef,
     QueryArgProfileTypeDef,
     ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
     ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
     ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
     ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
@@ -503,14 +508,15 @@
     ResponseHeadersPolicyContentTypeOptionsTypeDef,
     ResponseHeadersPolicyCustomHeaderTypeDef,
     ResponseHeadersPolicyFrameOptionsTypeDef,
     ResponseHeadersPolicyReferrerPolicyTypeDef,
     ResponseHeadersPolicyRemoveHeaderTypeDef,
     ResponseHeadersPolicyStrictTransportSecurityTypeDef,
     ResponseHeadersPolicyXSSProtectionTypeDef,
+    ResponseMetadataTypeDef,
     S3OriginTypeDef,
     StreamingLoggingConfigTypeDef,
     TagKeysTypeDef,
     TagTypeDef,
     TestFunctionRequestRequestTypeDef,
     UpdateDistributionWithStagingConfigRequestRequestTypeDef,
     AllowedMethodsTypeDef,
@@ -519,22 +525,20 @@
     OriginRequestPolicyCookiesConfigTypeDef,
     CachePolicyHeadersConfigTypeDef,
     OriginRequestPolicyHeadersConfigTypeDef,
     CachePolicyQueryStringsConfigTypeDef,
     OriginRequestPolicyQueryStringsConfigTypeDef,
     CloudFrontOriginAccessIdentityTypeDef,
     CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
+    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     CloudFrontOriginAccessIdentityListTypeDef,
     ConflictingAliasesListTypeDef,
     ContentTypeProfilesTypeDef,
     ContinuousDeploymentSingleWeightConfigTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
-    GetFunctionResultTypeDef,
     CreateFunctionRequestRequestTypeDef,
     UpdateFunctionRequestRequestTypeDef,
     CreateKeyGroupRequestRequestTypeDef,
     GetKeyGroupConfigResultTypeDef,
     KeyGroupTypeDef,
     UpdateKeyGroupRequestRequestTypeDef,
     CreateOriginAccessControlRequestRequestTypeDef,
@@ -561,18 +565,14 @@
     GetInvalidationRequestInvalidationCompletedWaitTypeDef,
     GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
     InvalidationBatchTypeDef,
     InvalidationListTypeDef,
     KGKeyPairIdsTypeDef,
     SignerTypeDef,
     LambdaFunctionAssociationsTypeDef,
-    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
-    ListDistributionsRequestListDistributionsPaginateTypeDef,
-    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
-    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlListTypeDef,
     OriginGroupFailoverCriteriaTypeDef,
     OriginGroupMembersTypeDef,
     PublicKeyListTypeDef,
     QueryArgProfilesTypeDef,
     ResponseHeadersPolicyCorsConfigTypeDef,
@@ -749,42 +749,42 @@
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

### Comparing `mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/__init__.py` & `mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/__init__.pyi` & `mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/__main__.py` & `mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudFront 1.26.77\nVersion:         1.26.77\nBuilder version:"
-        " 7.12.4\nDocs:           "
+        "Type annotations for boto3.CloudFront 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.77")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/client.py` & `mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -149,26 +149,23 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudFrontClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDenied: Type[BotocoreClientError]
     BatchTooLarge: Type[BotocoreClientError]
     CNAMEAlreadyExists: Type[BotocoreClientError]
     CachePolicyAlreadyExists: Type[BotocoreClientError]
     CachePolicyInUse: Type[BotocoreClientError]
     CannotChangeImmutablePublicKeyFields: Type[BotocoreClientError]
@@ -308,15 +305,14 @@
     TooManyStreamingDistributionCNAMEs: Type[BotocoreClientError]
     TooManyStreamingDistributions: Type[BotocoreClientError]
     TooManyTrustedSigners: Type[BotocoreClientError]
     TrustedKeyGroupDoesNotExist: Type[BotocoreClientError]
     TrustedSignerDoesNotExist: Type[BotocoreClientError]
     UnsupportedOperation: Type[BotocoreClientError]
 
-
 class CloudFrontClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/)
     """
 
     meta: ClientMeta
@@ -325,42 +321,38 @@
     def exceptions(self) -> Exceptions:
         """
         CloudFrontClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#exceptions)
         """
-
     def associate_alias(
         self, *, TargetDistributionId: str, Alias: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Associates an alias (also known as a CNAME or an alternate domain name) with a
         CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.associate_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#associate_alias)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#close)
         """
-
     def copy_distribution(
         self,
         *,
         PrimaryDistributionId: str,
         CallerReference: str,
         Staging: bool = ...,
         IfMatch: str = ...
@@ -368,718 +360,647 @@
         """
         Creates a staging distribution using the configuration of the provided primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#copy_distribution)
         """
-
     def create_cache_policy(
         self, *, CachePolicyConfig: CachePolicyConfigTypeDef
     ) -> CreateCachePolicyResultTypeDef:
         """
         Creates a cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cache_policy)
         """
-
     def create_cloud_front_origin_access_identity(
         self, *, CloudFrontOriginAccessIdentityConfig: CloudFrontOriginAccessIdentityConfigTypeDef
     ) -> CreateCloudFrontOriginAccessIdentityResultTypeDef:
         """
         Creates a new origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cloud_front_origin_access_identity)
         """
-
     def create_continuous_deployment_policy(
         self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef
     ) -> CreateContinuousDeploymentPolicyResultTypeDef:
         """
         Creates a continuous deployment policy that distributes traffic for a custom
         domain name to two different CloudFront distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_continuous_deployment_policy)
         """
-
     def create_distribution(
         self, *, DistributionConfig: DistributionConfigTypeDef
     ) -> CreateDistributionResultTypeDef:
         """
         Creates a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution)
         """
-
     def create_distribution_with_tags(
         self, *, DistributionConfigWithTags: DistributionConfigWithTagsTypeDef
     ) -> CreateDistributionWithTagsResultTypeDef:
         """
         Create a new distribution with tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution_with_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution_with_tags)
         """
-
     def create_field_level_encryption_config(
         self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef
     ) -> CreateFieldLevelEncryptionConfigResultTypeDef:
         """
         Create a new field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_config)
         """
-
     def create_field_level_encryption_profile(
         self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef
     ) -> CreateFieldLevelEncryptionProfileResultTypeDef:
         """
         Create a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_profile)
         """
-
     def create_function(
         self,
         *,
         Name: str,
         FunctionConfig: FunctionConfigTypeDef,
         FunctionCode: Union[str, bytes, IO[Any], StreamingBody]
     ) -> CreateFunctionResultTypeDef:
         """
         Creates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_function)
         """
-
     def create_invalidation(
         self, *, DistributionId: str, InvalidationBatch: InvalidationBatchTypeDef
     ) -> CreateInvalidationResultTypeDef:
         """
         Create a new invalidation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_invalidation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_invalidation)
         """
-
     def create_key_group(
         self, *, KeyGroupConfig: KeyGroupConfigTypeDef
     ) -> CreateKeyGroupResultTypeDef:
         """
         Creates a key group that you can use with [CloudFront signed URLs and signed
         cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_key_group)
         """
-
     def create_monitoring_subscription(
         self, *, DistributionId: str, MonitoringSubscription: MonitoringSubscriptionTypeDef
     ) -> CreateMonitoringSubscriptionResultTypeDef:
         """
         Enables additional CloudWatch metrics for the specified CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_monitoring_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_monitoring_subscription)
         """
-
     def create_origin_access_control(
         self, *, OriginAccessControlConfig: OriginAccessControlConfigTypeDef
     ) -> CreateOriginAccessControlResultTypeDef:
         """
         Creates a new origin access control in CloudFront.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_access_control)
         """
-
     def create_origin_request_policy(
         self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef
     ) -> CreateOriginRequestPolicyResultTypeDef:
         """
         Creates an origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_request_policy)
         """
-
     def create_public_key(
         self, *, PublicKeyConfig: PublicKeyConfigTypeDef
     ) -> CreatePublicKeyResultTypeDef:
         """
         Uploads a public key to CloudFront that you can use with [signed URLs and signed
         cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html)_,
         or with `field-level encryption
         <https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/field-level-
         enc...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_public_key)
         """
-
     def create_realtime_log_config(
         self,
         *,
         EndPoints: Sequence[EndPointTypeDef],
         Fields: Sequence[str],
         Name: str,
         SamplingRate: int
     ) -> CreateRealtimeLogConfigResultTypeDef:
         """
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_realtime_log_config)
         """
-
     def create_response_headers_policy(
         self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef
     ) -> CreateResponseHeadersPolicyResultTypeDef:
         """
         Creates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_response_headers_policy)
         """
-
     def create_streaming_distribution(
         self, *, StreamingDistributionConfig: StreamingDistributionConfigTypeDef
     ) -> CreateStreamingDistributionResultTypeDef:
         """
         This API is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_streaming_distribution)
         """
-
     def create_streaming_distribution_with_tags(
         self, *, StreamingDistributionConfigWithTags: StreamingDistributionConfigWithTagsTypeDef
     ) -> CreateStreamingDistributionWithTagsResultTypeDef:
         """
         This API is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution_with_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_streaming_distribution_with_tags)
         """
-
     def delete_cache_policy(self, *, Id: str, IfMatch: str = ...) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_cache_policy)
         """
-
     def delete_cloud_front_origin_access_identity(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete an origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_cloud_front_origin_access_identity)
         """
-
     def delete_continuous_deployment_policy(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_continuous_deployment_policy)
         """
-
     def delete_distribution(self, *, Id: str, IfMatch: str = ...) -> EmptyResponseMetadataTypeDef:
         """
         Delete a distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_distribution)
         """
-
     def delete_field_level_encryption_config(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Remove a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_field_level_encryption_config)
         """
-
     def delete_field_level_encryption_profile(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Remove a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_field_level_encryption_profile)
         """
-
     def delete_function(self, *, Name: str, IfMatch: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_function)
         """
-
     def delete_key_group(self, *, Id: str, IfMatch: str = ...) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_key_group)
         """
-
     def delete_monitoring_subscription(self, *, DistributionId: str) -> Dict[str, Any]:
         """
         Disables additional CloudWatch metrics for the specified CloudFront
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_monitoring_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_monitoring_subscription)
         """
-
     def delete_origin_access_control(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a CloudFront origin access control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_origin_access_control)
         """
-
     def delete_origin_request_policy(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_origin_request_policy)
         """
-
     def delete_public_key(self, *, Id: str, IfMatch: str = ...) -> EmptyResponseMetadataTypeDef:
         """
         Remove a public key you previously added to CloudFront.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_public_key)
         """
-
     def delete_realtime_log_config(
         self, *, Name: str = ..., ARN: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_realtime_log_config)
         """
-
     def delete_response_headers_policy(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_response_headers_policy)
         """
-
     def delete_streaming_distribution(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_streaming_distribution)
         """
-
     def describe_function(
         self, *, Name: str, Stage: FunctionStageType = ...
     ) -> DescribeFunctionResultTypeDef:
         """
         Gets configuration information and metadata about a CloudFront function, but not
         the function's code.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.describe_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#describe_function)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#generate_presigned_url)
         """
-
     def get_cache_policy(self, *, Id: str) -> GetCachePolicyResultTypeDef:
         """
-        Gets a cache policy, including the following metadata * The policy's identifier.
+        Gets a cache policy, including the following metadata: * The policy's
+        identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_cache_policy)
         """
-
     def get_cache_policy_config(self, *, Id: str) -> GetCachePolicyConfigResultTypeDef:
         """
         Gets a cache policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_cache_policy_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_cache_policy_config)
         """
-
     def get_cloud_front_origin_access_identity(
         self, *, Id: str
     ) -> GetCloudFrontOriginAccessIdentityResultTypeDef:
         """
         Get the information about an origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_cloud_front_origin_access_identity)
         """
-
     def get_cloud_front_origin_access_identity_config(
         self, *, Id: str
     ) -> GetCloudFrontOriginAccessIdentityConfigResultTypeDef:
         """
         Get the configuration information about an origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_cloud_front_origin_access_identity_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_cloud_front_origin_access_identity_config)
         """
-
     def get_continuous_deployment_policy(
         self, *, Id: str
     ) -> GetContinuousDeploymentPolicyResultTypeDef:
         """
         Gets a continuous deployment policy, including metadata (the policy's identifier
         and the date and time when the policy was last modified).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_continuous_deployment_policy)
         """
-
     def get_continuous_deployment_policy_config(
         self, *, Id: str
     ) -> GetContinuousDeploymentPolicyConfigResultTypeDef:
         """
         Gets configuration information about a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_continuous_deployment_policy_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_continuous_deployment_policy_config)
         """
-
     def get_distribution(self, *, Id: str) -> GetDistributionResultTypeDef:
         """
         Get the information about a distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_distribution)
         """
-
     def get_distribution_config(self, *, Id: str) -> GetDistributionConfigResultTypeDef:
         """
         Get the configuration information about a distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_distribution_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_distribution_config)
         """
-
     def get_field_level_encryption(self, *, Id: str) -> GetFieldLevelEncryptionResultTypeDef:
         """
         Get the field-level encryption configuration information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_field_level_encryption)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_field_level_encryption)
         """
-
     def get_field_level_encryption_config(
         self, *, Id: str
     ) -> GetFieldLevelEncryptionConfigResultTypeDef:
         """
         Get the field-level encryption configuration information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_field_level_encryption_config)
         """
-
     def get_field_level_encryption_profile(
         self, *, Id: str
     ) -> GetFieldLevelEncryptionProfileResultTypeDef:
         """
         Get the field-level encryption profile information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_field_level_encryption_profile)
         """
-
     def get_field_level_encryption_profile_config(
         self, *, Id: str
     ) -> GetFieldLevelEncryptionProfileConfigResultTypeDef:
         """
         Get the field-level encryption profile configuration information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_field_level_encryption_profile_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_field_level_encryption_profile_config)
         """
-
     def get_function(
         self, *, Name: str, Stage: FunctionStageType = ...
     ) -> GetFunctionResultTypeDef:
         """
         Gets the code of a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_function)
         """
-
     def get_invalidation(self, *, DistributionId: str, Id: str) -> GetInvalidationResultTypeDef:
         """
         Get the information about an invalidation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_invalidation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_invalidation)
         """
-
     def get_key_group(self, *, Id: str) -> GetKeyGroupResultTypeDef:
         """
         Gets a key group, including the date and time when the key group was last
         modified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_key_group)
         """
-
     def get_key_group_config(self, *, Id: str) -> GetKeyGroupConfigResultTypeDef:
         """
         Gets a key group configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_key_group_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_key_group_config)
         """
-
     def get_monitoring_subscription(
         self, *, DistributionId: str
     ) -> GetMonitoringSubscriptionResultTypeDef:
         """
         Gets information about whether additional CloudWatch metrics are enabled for the
         specified CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_monitoring_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_monitoring_subscription)
         """
-
     def get_origin_access_control(self, *, Id: str) -> GetOriginAccessControlResultTypeDef:
         """
         Gets a CloudFront origin access control, including its unique identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_origin_access_control)
         """
-
     def get_origin_access_control_config(
         self, *, Id: str
     ) -> GetOriginAccessControlConfigResultTypeDef:
         """
         Gets a CloudFront origin access control configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_origin_access_control_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_origin_access_control_config)
         """
-
     def get_origin_request_policy(self, *, Id: str) -> GetOriginRequestPolicyResultTypeDef:
         """
-        Gets an origin request policy, including the following metadata * The policy's
+        Gets an origin request policy, including the following metadata: * The policy's
         identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_origin_request_policy)
         """
-
     def get_origin_request_policy_config(
         self, *, Id: str
     ) -> GetOriginRequestPolicyConfigResultTypeDef:
         """
         Gets an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_origin_request_policy_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_origin_request_policy_config)
         """
-
     def get_public_key(self, *, Id: str) -> GetPublicKeyResultTypeDef:
         """
         Gets a public key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_public_key)
         """
-
     def get_public_key_config(self, *, Id: str) -> GetPublicKeyConfigResultTypeDef:
         """
         Gets a public key configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_public_key_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_public_key_config)
         """
-
     def get_realtime_log_config(
         self, *, Name: str = ..., ARN: str = ...
     ) -> GetRealtimeLogConfigResultTypeDef:
         """
         Gets a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_realtime_log_config)
         """
-
     def get_response_headers_policy(self, *, Id: str) -> GetResponseHeadersPolicyResultTypeDef:
         """
         Gets a response headers policy, including metadata (the policy's identifier and
         the date and time when the policy was last modified).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_response_headers_policy)
         """
-
     def get_response_headers_policy_config(
         self, *, Id: str
     ) -> GetResponseHeadersPolicyConfigResultTypeDef:
         """
         Gets a response headers policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_response_headers_policy_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_response_headers_policy_config)
         """
-
     def get_streaming_distribution(self, *, Id: str) -> GetStreamingDistributionResultTypeDef:
         """
         Gets information about a specified RTMP distribution, including the distribution
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_streaming_distribution)
         """
-
     def get_streaming_distribution_config(
         self, *, Id: str
     ) -> GetStreamingDistributionConfigResultTypeDef:
         """
         Get the configuration information about a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_streaming_distribution_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_streaming_distribution_config)
         """
-
     def list_cache_policies(
         self, *, Type: CachePolicyTypeType = ..., Marker: str = ..., MaxItems: str = ...
     ) -> ListCachePoliciesResultTypeDef:
         """
         Gets a list of cache policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_cache_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_cache_policies)
         """
-
     def list_cloud_front_origin_access_identities(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListCloudFrontOriginAccessIdentitiesResultTypeDef:
         """
         Lists origin access identities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_cloud_front_origin_access_identities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_cloud_front_origin_access_identities)
         """
-
     def list_conflicting_aliases(
         self, *, DistributionId: str, Alias: str, Marker: str = ..., MaxItems: int = ...
     ) -> ListConflictingAliasesResultTypeDef:
         """
         Gets a list of aliases (also called CNAMEs or alternate domain names) that
         conflict or overlap with the provided alias, and the associated CloudFront
         distributions and Amazon Web Services accounts for each conflicting alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_conflicting_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_conflicting_aliases)
         """
-
     def list_continuous_deployment_policies(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListContinuousDeploymentPoliciesResultTypeDef:
         """
         Gets a list of the continuous deployment policies in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_continuous_deployment_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_continuous_deployment_policies)
         """
-
     def list_distributions(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListDistributionsResultTypeDef:
         """
         List CloudFront distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_distributions)
         """
-
     def list_distributions_by_cache_policy_id(
         self, *, CachePolicyId: str, Marker: str = ..., MaxItems: str = ...
     ) -> ListDistributionsByCachePolicyIdResultTypeDef:
         """
         Gets a list of distribution IDs for distributions that have a cache behavior
         that's associated with the specified cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_cache_policy_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_distributions_by_cache_policy_id)
         """
-
     def list_distributions_by_key_group(
         self, *, KeyGroupId: str, Marker: str = ..., MaxItems: str = ...
     ) -> ListDistributionsByKeyGroupResultTypeDef:
         """
         Gets a list of distribution IDs for distributions that have a cache behavior
         that references the specified key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_distributions_by_key_group)
         """
-
     def list_distributions_by_origin_request_policy_id(
         self, *, OriginRequestPolicyId: str, Marker: str = ..., MaxItems: str = ...
     ) -> ListDistributionsByOriginRequestPolicyIdResultTypeDef:
         """
         Gets a list of distribution IDs for distributions that have a cache behavior
         that's associated with the specified origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_origin_request_policy_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_distributions_by_origin_request_policy_id)
         """
-
     def list_distributions_by_realtime_log_config(
         self,
         *,
         Marker: str = ...,
         MaxItems: str = ...,
         RealtimeLogConfigName: str = ...,
         RealtimeLogConfigArn: str = ...
@@ -1087,349 +1008,318 @@
         """
         Gets a list of distributions that have a cache behavior that's associated with
         the specified real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_distributions_by_realtime_log_config)
         """
-
     def list_distributions_by_response_headers_policy_id(
         self, *, ResponseHeadersPolicyId: str, Marker: str = ..., MaxItems: str = ...
     ) -> ListDistributionsByResponseHeadersPolicyIdResultTypeDef:
         """
         Gets a list of distribution IDs for distributions that have a cache behavior
         that's associated with the specified response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_response_headers_policy_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_distributions_by_response_headers_policy_id)
         """
-
     def list_distributions_by_web_acl_id(
         self, *, WebACLId: str, Marker: str = ..., MaxItems: str = ...
     ) -> ListDistributionsByWebACLIdResultTypeDef:
         """
         List the distributions that are associated with a specified WAF web ACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_web_acl_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_distributions_by_web_acl_id)
         """
-
     def list_field_level_encryption_configs(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListFieldLevelEncryptionConfigsResultTypeDef:
         """
         List all field-level encryption configurations that have been created in
         CloudFront for this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_field_level_encryption_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_field_level_encryption_configs)
         """
-
     def list_field_level_encryption_profiles(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListFieldLevelEncryptionProfilesResultTypeDef:
         """
         Request a list of field-level encryption profiles that have been created in
         CloudFront for this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_field_level_encryption_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_field_level_encryption_profiles)
         """
-
     def list_functions(
         self, *, Marker: str = ..., MaxItems: str = ..., Stage: FunctionStageType = ...
     ) -> ListFunctionsResultTypeDef:
         """
         Gets a list of all CloudFront functions in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_functions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_functions)
         """
-
     def list_invalidations(
         self, *, DistributionId: str, Marker: str = ..., MaxItems: str = ...
     ) -> ListInvalidationsResultTypeDef:
         """
         Lists invalidation batches.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_invalidations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_invalidations)
         """
-
     def list_key_groups(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListKeyGroupsResultTypeDef:
         """
         Gets a list of key groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_key_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_key_groups)
         """
-
     def list_origin_access_controls(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListOriginAccessControlsResultTypeDef:
         """
         Gets the list of CloudFront origin access controls in this Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_origin_access_controls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_origin_access_controls)
         """
-
     def list_origin_request_policies(
         self, *, Type: OriginRequestPolicyTypeType = ..., Marker: str = ..., MaxItems: str = ...
     ) -> ListOriginRequestPoliciesResultTypeDef:
         """
         Gets a list of origin request policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_origin_request_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_origin_request_policies)
         """
-
     def list_public_keys(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListPublicKeysResultTypeDef:
         """
         List all public keys that have been added to CloudFront for this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_public_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_public_keys)
         """
-
     def list_realtime_log_configs(
         self, *, MaxItems: str = ..., Marker: str = ...
     ) -> ListRealtimeLogConfigsResultTypeDef:
         """
         Gets a list of real-time log configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_realtime_log_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_realtime_log_configs)
         """
-
     def list_response_headers_policies(
         self, *, Type: ResponseHeadersPolicyTypeType = ..., Marker: str = ..., MaxItems: str = ...
     ) -> ListResponseHeadersPoliciesResultTypeDef:
         """
         Gets a list of response headers policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_response_headers_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_response_headers_policies)
         """
-
     def list_streaming_distributions(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListStreamingDistributionsResultTypeDef:
         """
         List streaming distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_streaming_distributions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_streaming_distributions)
         """
-
     def list_tags_for_resource(self, *, Resource: str) -> ListTagsForResourceResultTypeDef:
         """
         List tags for a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_tags_for_resource)
         """
-
     def publish_function(self, *, Name: str, IfMatch: str) -> PublishFunctionResultTypeDef:
         """
         Publishes a CloudFront function by copying the function code from the
         `DEVELOPMENT` stage to `LIVE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.publish_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#publish_function)
         """
-
     def tag_resource(self, *, Resource: str, Tags: TagsTypeDef) -> EmptyResponseMetadataTypeDef:
         """
         Add tags to a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#tag_resource)
         """
-
     def test_function(
         self,
         *,
         Name: str,
         IfMatch: str,
         EventObject: Union[str, bytes, IO[Any], StreamingBody],
         Stage: FunctionStageType = ...
     ) -> TestFunctionResultTypeDef:
         """
         Tests a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.test_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#test_function)
         """
-
     def untag_resource(
         self, *, Resource: str, TagKeys: TagKeysTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Remove tags from a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#untag_resource)
         """
-
     def update_cache_policy(
         self, *, CachePolicyConfig: CachePolicyConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateCachePolicyResultTypeDef:
         """
         Updates a cache policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cache_policy)
         """
-
     def update_cloud_front_origin_access_identity(
         self,
         *,
         CloudFrontOriginAccessIdentityConfig: CloudFrontOriginAccessIdentityConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateCloudFrontOriginAccessIdentityResultTypeDef:
         """
         Update an origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
-
     def update_continuous_deployment_policy(
         self,
         *,
         ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_continuous_deployment_policy)
         """
-
     def update_distribution(
         self, *, DistributionConfig: DistributionConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates the configuration for a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution)
         """
-
     def update_distribution_with_staging_config(
         self, *, Id: str, StagingDistributionId: str = ..., IfMatch: str = ...
     ) -> UpdateDistributionWithStagingConfigResultTypeDef:
         """
         Copies the staging distribution's configuration to its corresponding primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution_with_staging_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution_with_staging_config)
         """
-
     def update_field_level_encryption_config(
         self,
         *,
         FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_field_level_encryption_config)
         """
-
     def update_field_level_encryption_profile(
         self,
         *,
         FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_field_level_encryption_profile)
         """
-
     def update_function(
         self,
         *,
         Name: str,
         IfMatch: str,
         FunctionConfig: FunctionConfigTypeDef,
         FunctionCode: Union[str, bytes, IO[Any], StreamingBody]
     ) -> UpdateFunctionResultTypeDef:
         """
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_function)
         """
-
     def update_key_group(
         self, *, KeyGroupConfig: KeyGroupConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateKeyGroupResultTypeDef:
         """
         Updates a key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_key_group)
         """
-
     def update_origin_access_control(
         self,
         *,
         OriginAccessControlConfig: OriginAccessControlConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateOriginAccessControlResultTypeDef:
         """
         Updates a CloudFront origin access control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_origin_access_control)
         """
-
     def update_origin_request_policy(
         self,
         *,
         OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_origin_request_policy)
         """
-
     def update_public_key(
         self, *, PublicKeyConfig: PublicKeyConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdatePublicKeyResultTypeDef:
         """
         Update public key information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_public_key)
         """
-
     def update_realtime_log_config(
         self,
         *,
         EndPoints: Sequence[EndPointTypeDef] = ...,
         Fields: Sequence[str] = ...,
         Name: str = ...,
         ARN: str = ...,
@@ -1437,97 +1327,88 @@
     ) -> UpdateRealtimeLogConfigResultTypeDef:
         """
         Updates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_realtime_log_config)
         """
-
     def update_response_headers_policy(
         self,
         *,
         ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_response_headers_policy)
         """
-
     def update_streaming_distribution(
         self,
         *,
         StreamingDistributionConfig: StreamingDistributionConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_streaming_distribution)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_cloud_front_origin_access_identities"]
     ) -> ListCloudFrontOriginAccessIdentitiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_distributions"]
     ) -> ListDistributionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_invalidations"]
     ) -> ListInvalidationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_streaming_distributions"]
     ) -> ListStreamingDistributionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_paginator)
         """
-
     @overload
     def get_waiter(
         self, waiter_name: Literal["distribution_deployed"]
     ) -> DistributionDeployedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_waiter)
         """
-
     @overload
     def get_waiter(
         self, waiter_name: Literal["invalidation_completed"]
     ) -> InvalidationCompletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_waiter)
         """
-
     @overload
     def get_waiter(
         self, waiter_name: Literal["streaming_distribution_deployed"]
     ) -> StreamingDistributionDeployedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_waiter)
```

### Comparing `mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/client.pyi` & `mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,23 +149,26 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("CloudFrontClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDenied: Type[BotocoreClientError]
     BatchTooLarge: Type[BotocoreClientError]
     CNAMEAlreadyExists: Type[BotocoreClientError]
     CachePolicyAlreadyExists: Type[BotocoreClientError]
     CachePolicyInUse: Type[BotocoreClientError]
     CannotChangeImmutablePublicKeyFields: Type[BotocoreClientError]
@@ -305,14 +308,15 @@
     TooManyStreamingDistributionCNAMEs: Type[BotocoreClientError]
     TooManyStreamingDistributions: Type[BotocoreClientError]
     TooManyTrustedSigners: Type[BotocoreClientError]
     TrustedKeyGroupDoesNotExist: Type[BotocoreClientError]
     TrustedSignerDoesNotExist: Type[BotocoreClientError]
     UnsupportedOperation: Type[BotocoreClientError]
 
+
 class CloudFrontClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/)
     """
 
     meta: ClientMeta
@@ -321,38 +325,42 @@
     def exceptions(self) -> Exceptions:
         """
         CloudFrontClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#exceptions)
         """
+
     def associate_alias(
         self, *, TargetDistributionId: str, Alias: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Associates an alias (also known as a CNAME or an alternate domain name) with a
         CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.associate_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#associate_alias)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#close)
         """
+
     def copy_distribution(
         self,
         *,
         PrimaryDistributionId: str,
         CallerReference: str,
         Staging: bool = ...,
         IfMatch: str = ...
@@ -360,646 +368,719 @@
         """
         Creates a staging distribution using the configuration of the provided primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#copy_distribution)
         """
+
     def create_cache_policy(
         self, *, CachePolicyConfig: CachePolicyConfigTypeDef
     ) -> CreateCachePolicyResultTypeDef:
         """
         Creates a cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cache_policy)
         """
+
     def create_cloud_front_origin_access_identity(
         self, *, CloudFrontOriginAccessIdentityConfig: CloudFrontOriginAccessIdentityConfigTypeDef
     ) -> CreateCloudFrontOriginAccessIdentityResultTypeDef:
         """
         Creates a new origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cloud_front_origin_access_identity)
         """
+
     def create_continuous_deployment_policy(
         self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef
     ) -> CreateContinuousDeploymentPolicyResultTypeDef:
         """
         Creates a continuous deployment policy that distributes traffic for a custom
         domain name to two different CloudFront distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_continuous_deployment_policy)
         """
+
     def create_distribution(
         self, *, DistributionConfig: DistributionConfigTypeDef
     ) -> CreateDistributionResultTypeDef:
         """
         Creates a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution)
         """
+
     def create_distribution_with_tags(
         self, *, DistributionConfigWithTags: DistributionConfigWithTagsTypeDef
     ) -> CreateDistributionWithTagsResultTypeDef:
         """
         Create a new distribution with tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution_with_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution_with_tags)
         """
+
     def create_field_level_encryption_config(
         self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef
     ) -> CreateFieldLevelEncryptionConfigResultTypeDef:
         """
         Create a new field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_config)
         """
+
     def create_field_level_encryption_profile(
         self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef
     ) -> CreateFieldLevelEncryptionProfileResultTypeDef:
         """
         Create a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_profile)
         """
+
     def create_function(
         self,
         *,
         Name: str,
         FunctionConfig: FunctionConfigTypeDef,
         FunctionCode: Union[str, bytes, IO[Any], StreamingBody]
     ) -> CreateFunctionResultTypeDef:
         """
         Creates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_function)
         """
+
     def create_invalidation(
         self, *, DistributionId: str, InvalidationBatch: InvalidationBatchTypeDef
     ) -> CreateInvalidationResultTypeDef:
         """
         Create a new invalidation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_invalidation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_invalidation)
         """
+
     def create_key_group(
         self, *, KeyGroupConfig: KeyGroupConfigTypeDef
     ) -> CreateKeyGroupResultTypeDef:
         """
         Creates a key group that you can use with [CloudFront signed URLs and signed
         cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_key_group)
         """
+
     def create_monitoring_subscription(
         self, *, DistributionId: str, MonitoringSubscription: MonitoringSubscriptionTypeDef
     ) -> CreateMonitoringSubscriptionResultTypeDef:
         """
         Enables additional CloudWatch metrics for the specified CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_monitoring_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_monitoring_subscription)
         """
+
     def create_origin_access_control(
         self, *, OriginAccessControlConfig: OriginAccessControlConfigTypeDef
     ) -> CreateOriginAccessControlResultTypeDef:
         """
         Creates a new origin access control in CloudFront.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_access_control)
         """
+
     def create_origin_request_policy(
         self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef
     ) -> CreateOriginRequestPolicyResultTypeDef:
         """
         Creates an origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_request_policy)
         """
+
     def create_public_key(
         self, *, PublicKeyConfig: PublicKeyConfigTypeDef
     ) -> CreatePublicKeyResultTypeDef:
         """
         Uploads a public key to CloudFront that you can use with [signed URLs and signed
         cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html)_,
         or with `field-level encryption
         <https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/field-level-
         enc...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_public_key)
         """
+
     def create_realtime_log_config(
         self,
         *,
         EndPoints: Sequence[EndPointTypeDef],
         Fields: Sequence[str],
         Name: str,
         SamplingRate: int
     ) -> CreateRealtimeLogConfigResultTypeDef:
         """
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_realtime_log_config)
         """
+
     def create_response_headers_policy(
         self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef
     ) -> CreateResponseHeadersPolicyResultTypeDef:
         """
         Creates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_response_headers_policy)
         """
+
     def create_streaming_distribution(
         self, *, StreamingDistributionConfig: StreamingDistributionConfigTypeDef
     ) -> CreateStreamingDistributionResultTypeDef:
         """
         This API is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_streaming_distribution)
         """
+
     def create_streaming_distribution_with_tags(
         self, *, StreamingDistributionConfigWithTags: StreamingDistributionConfigWithTagsTypeDef
     ) -> CreateStreamingDistributionWithTagsResultTypeDef:
         """
         This API is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution_with_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_streaming_distribution_with_tags)
         """
+
     def delete_cache_policy(self, *, Id: str, IfMatch: str = ...) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_cache_policy)
         """
+
     def delete_cloud_front_origin_access_identity(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete an origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_cloud_front_origin_access_identity)
         """
+
     def delete_continuous_deployment_policy(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_continuous_deployment_policy)
         """
+
     def delete_distribution(self, *, Id: str, IfMatch: str = ...) -> EmptyResponseMetadataTypeDef:
         """
         Delete a distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_distribution)
         """
+
     def delete_field_level_encryption_config(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Remove a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_field_level_encryption_config)
         """
+
     def delete_field_level_encryption_profile(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Remove a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_field_level_encryption_profile)
         """
+
     def delete_function(self, *, Name: str, IfMatch: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_function)
         """
+
     def delete_key_group(self, *, Id: str, IfMatch: str = ...) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_key_group)
         """
+
     def delete_monitoring_subscription(self, *, DistributionId: str) -> Dict[str, Any]:
         """
         Disables additional CloudWatch metrics for the specified CloudFront
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_monitoring_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_monitoring_subscription)
         """
+
     def delete_origin_access_control(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a CloudFront origin access control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_origin_access_control)
         """
+
     def delete_origin_request_policy(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_origin_request_policy)
         """
+
     def delete_public_key(self, *, Id: str, IfMatch: str = ...) -> EmptyResponseMetadataTypeDef:
         """
         Remove a public key you previously added to CloudFront.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_public_key)
         """
+
     def delete_realtime_log_config(
         self, *, Name: str = ..., ARN: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_realtime_log_config)
         """
+
     def delete_response_headers_policy(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_response_headers_policy)
         """
+
     def delete_streaming_distribution(
         self, *, Id: str, IfMatch: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.delete_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#delete_streaming_distribution)
         """
+
     def describe_function(
         self, *, Name: str, Stage: FunctionStageType = ...
     ) -> DescribeFunctionResultTypeDef:
         """
         Gets configuration information and metadata about a CloudFront function, but not
         the function's code.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.describe_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#describe_function)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#generate_presigned_url)
         """
+
     def get_cache_policy(self, *, Id: str) -> GetCachePolicyResultTypeDef:
         """
-        Gets a cache policy, including the following metadata * The policy's identifier.
+        Gets a cache policy, including the following metadata: * The policy's
+        identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_cache_policy)
         """
+
     def get_cache_policy_config(self, *, Id: str) -> GetCachePolicyConfigResultTypeDef:
         """
         Gets a cache policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_cache_policy_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_cache_policy_config)
         """
+
     def get_cloud_front_origin_access_identity(
         self, *, Id: str
     ) -> GetCloudFrontOriginAccessIdentityResultTypeDef:
         """
         Get the information about an origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_cloud_front_origin_access_identity)
         """
+
     def get_cloud_front_origin_access_identity_config(
         self, *, Id: str
     ) -> GetCloudFrontOriginAccessIdentityConfigResultTypeDef:
         """
         Get the configuration information about an origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_cloud_front_origin_access_identity_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_cloud_front_origin_access_identity_config)
         """
+
     def get_continuous_deployment_policy(
         self, *, Id: str
     ) -> GetContinuousDeploymentPolicyResultTypeDef:
         """
         Gets a continuous deployment policy, including metadata (the policy's identifier
         and the date and time when the policy was last modified).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_continuous_deployment_policy)
         """
+
     def get_continuous_deployment_policy_config(
         self, *, Id: str
     ) -> GetContinuousDeploymentPolicyConfigResultTypeDef:
         """
         Gets configuration information about a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_continuous_deployment_policy_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_continuous_deployment_policy_config)
         """
+
     def get_distribution(self, *, Id: str) -> GetDistributionResultTypeDef:
         """
         Get the information about a distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_distribution)
         """
+
     def get_distribution_config(self, *, Id: str) -> GetDistributionConfigResultTypeDef:
         """
         Get the configuration information about a distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_distribution_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_distribution_config)
         """
+
     def get_field_level_encryption(self, *, Id: str) -> GetFieldLevelEncryptionResultTypeDef:
         """
         Get the field-level encryption configuration information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_field_level_encryption)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_field_level_encryption)
         """
+
     def get_field_level_encryption_config(
         self, *, Id: str
     ) -> GetFieldLevelEncryptionConfigResultTypeDef:
         """
         Get the field-level encryption configuration information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_field_level_encryption_config)
         """
+
     def get_field_level_encryption_profile(
         self, *, Id: str
     ) -> GetFieldLevelEncryptionProfileResultTypeDef:
         """
         Get the field-level encryption profile information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_field_level_encryption_profile)
         """
+
     def get_field_level_encryption_profile_config(
         self, *, Id: str
     ) -> GetFieldLevelEncryptionProfileConfigResultTypeDef:
         """
         Get the field-level encryption profile configuration information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_field_level_encryption_profile_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_field_level_encryption_profile_config)
         """
+
     def get_function(
         self, *, Name: str, Stage: FunctionStageType = ...
     ) -> GetFunctionResultTypeDef:
         """
         Gets the code of a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_function)
         """
+
     def get_invalidation(self, *, DistributionId: str, Id: str) -> GetInvalidationResultTypeDef:
         """
         Get the information about an invalidation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_invalidation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_invalidation)
         """
+
     def get_key_group(self, *, Id: str) -> GetKeyGroupResultTypeDef:
         """
         Gets a key group, including the date and time when the key group was last
         modified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_key_group)
         """
+
     def get_key_group_config(self, *, Id: str) -> GetKeyGroupConfigResultTypeDef:
         """
         Gets a key group configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_key_group_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_key_group_config)
         """
+
     def get_monitoring_subscription(
         self, *, DistributionId: str
     ) -> GetMonitoringSubscriptionResultTypeDef:
         """
         Gets information about whether additional CloudWatch metrics are enabled for the
         specified CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_monitoring_subscription)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_monitoring_subscription)
         """
+
     def get_origin_access_control(self, *, Id: str) -> GetOriginAccessControlResultTypeDef:
         """
         Gets a CloudFront origin access control, including its unique identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_origin_access_control)
         """
+
     def get_origin_access_control_config(
         self, *, Id: str
     ) -> GetOriginAccessControlConfigResultTypeDef:
         """
         Gets a CloudFront origin access control configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_origin_access_control_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_origin_access_control_config)
         """
+
     def get_origin_request_policy(self, *, Id: str) -> GetOriginRequestPolicyResultTypeDef:
         """
-        Gets an origin request policy, including the following metadata * The policy's
+        Gets an origin request policy, including the following metadata: * The policy's
         identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_origin_request_policy)
         """
+
     def get_origin_request_policy_config(
         self, *, Id: str
     ) -> GetOriginRequestPolicyConfigResultTypeDef:
         """
         Gets an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_origin_request_policy_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_origin_request_policy_config)
         """
+
     def get_public_key(self, *, Id: str) -> GetPublicKeyResultTypeDef:
         """
         Gets a public key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_public_key)
         """
+
     def get_public_key_config(self, *, Id: str) -> GetPublicKeyConfigResultTypeDef:
         """
         Gets a public key configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_public_key_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_public_key_config)
         """
+
     def get_realtime_log_config(
         self, *, Name: str = ..., ARN: str = ...
     ) -> GetRealtimeLogConfigResultTypeDef:
         """
         Gets a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_realtime_log_config)
         """
+
     def get_response_headers_policy(self, *, Id: str) -> GetResponseHeadersPolicyResultTypeDef:
         """
         Gets a response headers policy, including metadata (the policy's identifier and
         the date and time when the policy was last modified).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_response_headers_policy)
         """
+
     def get_response_headers_policy_config(
         self, *, Id: str
     ) -> GetResponseHeadersPolicyConfigResultTypeDef:
         """
         Gets a response headers policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_response_headers_policy_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_response_headers_policy_config)
         """
+
     def get_streaming_distribution(self, *, Id: str) -> GetStreamingDistributionResultTypeDef:
         """
         Gets information about a specified RTMP distribution, including the distribution
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_streaming_distribution)
         """
+
     def get_streaming_distribution_config(
         self, *, Id: str
     ) -> GetStreamingDistributionConfigResultTypeDef:
         """
         Get the configuration information about a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_streaming_distribution_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_streaming_distribution_config)
         """
+
     def list_cache_policies(
         self, *, Type: CachePolicyTypeType = ..., Marker: str = ..., MaxItems: str = ...
     ) -> ListCachePoliciesResultTypeDef:
         """
         Gets a list of cache policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_cache_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_cache_policies)
         """
+
     def list_cloud_front_origin_access_identities(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListCloudFrontOriginAccessIdentitiesResultTypeDef:
         """
         Lists origin access identities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_cloud_front_origin_access_identities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_cloud_front_origin_access_identities)
         """
+
     def list_conflicting_aliases(
         self, *, DistributionId: str, Alias: str, Marker: str = ..., MaxItems: int = ...
     ) -> ListConflictingAliasesResultTypeDef:
         """
         Gets a list of aliases (also called CNAMEs or alternate domain names) that
         conflict or overlap with the provided alias, and the associated CloudFront
         distributions and Amazon Web Services accounts for each conflicting alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_conflicting_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_conflicting_aliases)
         """
+
     def list_continuous_deployment_policies(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListContinuousDeploymentPoliciesResultTypeDef:
         """
         Gets a list of the continuous deployment policies in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_continuous_deployment_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_continuous_deployment_policies)
         """
+
     def list_distributions(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListDistributionsResultTypeDef:
         """
         List CloudFront distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_distributions)
         """
+
     def list_distributions_by_cache_policy_id(
         self, *, CachePolicyId: str, Marker: str = ..., MaxItems: str = ...
     ) -> ListDistributionsByCachePolicyIdResultTypeDef:
         """
         Gets a list of distribution IDs for distributions that have a cache behavior
         that's associated with the specified cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_cache_policy_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_distributions_by_cache_policy_id)
         """
+
     def list_distributions_by_key_group(
         self, *, KeyGroupId: str, Marker: str = ..., MaxItems: str = ...
     ) -> ListDistributionsByKeyGroupResultTypeDef:
         """
         Gets a list of distribution IDs for distributions that have a cache behavior
         that references the specified key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_distributions_by_key_group)
         """
+
     def list_distributions_by_origin_request_policy_id(
         self, *, OriginRequestPolicyId: str, Marker: str = ..., MaxItems: str = ...
     ) -> ListDistributionsByOriginRequestPolicyIdResultTypeDef:
         """
         Gets a list of distribution IDs for distributions that have a cache behavior
         that's associated with the specified origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_origin_request_policy_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_distributions_by_origin_request_policy_id)
         """
+
     def list_distributions_by_realtime_log_config(
         self,
         *,
         Marker: str = ...,
         MaxItems: str = ...,
         RealtimeLogConfigName: str = ...,
         RealtimeLogConfigArn: str = ...
@@ -1007,318 +1088,349 @@
         """
         Gets a list of distributions that have a cache behavior that's associated with
         the specified real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_distributions_by_realtime_log_config)
         """
+
     def list_distributions_by_response_headers_policy_id(
         self, *, ResponseHeadersPolicyId: str, Marker: str = ..., MaxItems: str = ...
     ) -> ListDistributionsByResponseHeadersPolicyIdResultTypeDef:
         """
         Gets a list of distribution IDs for distributions that have a cache behavior
         that's associated with the specified response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_response_headers_policy_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_distributions_by_response_headers_policy_id)
         """
+
     def list_distributions_by_web_acl_id(
         self, *, WebACLId: str, Marker: str = ..., MaxItems: str = ...
     ) -> ListDistributionsByWebACLIdResultTypeDef:
         """
         List the distributions that are associated with a specified WAF web ACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_distributions_by_web_acl_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_distributions_by_web_acl_id)
         """
+
     def list_field_level_encryption_configs(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListFieldLevelEncryptionConfigsResultTypeDef:
         """
         List all field-level encryption configurations that have been created in
         CloudFront for this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_field_level_encryption_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_field_level_encryption_configs)
         """
+
     def list_field_level_encryption_profiles(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListFieldLevelEncryptionProfilesResultTypeDef:
         """
         Request a list of field-level encryption profiles that have been created in
         CloudFront for this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_field_level_encryption_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_field_level_encryption_profiles)
         """
+
     def list_functions(
         self, *, Marker: str = ..., MaxItems: str = ..., Stage: FunctionStageType = ...
     ) -> ListFunctionsResultTypeDef:
         """
         Gets a list of all CloudFront functions in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_functions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_functions)
         """
+
     def list_invalidations(
         self, *, DistributionId: str, Marker: str = ..., MaxItems: str = ...
     ) -> ListInvalidationsResultTypeDef:
         """
         Lists invalidation batches.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_invalidations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_invalidations)
         """
+
     def list_key_groups(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListKeyGroupsResultTypeDef:
         """
         Gets a list of key groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_key_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_key_groups)
         """
+
     def list_origin_access_controls(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListOriginAccessControlsResultTypeDef:
         """
         Gets the list of CloudFront origin access controls in this Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_origin_access_controls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_origin_access_controls)
         """
+
     def list_origin_request_policies(
         self, *, Type: OriginRequestPolicyTypeType = ..., Marker: str = ..., MaxItems: str = ...
     ) -> ListOriginRequestPoliciesResultTypeDef:
         """
         Gets a list of origin request policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_origin_request_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_origin_request_policies)
         """
+
     def list_public_keys(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListPublicKeysResultTypeDef:
         """
         List all public keys that have been added to CloudFront for this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_public_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_public_keys)
         """
+
     def list_realtime_log_configs(
         self, *, MaxItems: str = ..., Marker: str = ...
     ) -> ListRealtimeLogConfigsResultTypeDef:
         """
         Gets a list of real-time log configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_realtime_log_configs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_realtime_log_configs)
         """
+
     def list_response_headers_policies(
         self, *, Type: ResponseHeadersPolicyTypeType = ..., Marker: str = ..., MaxItems: str = ...
     ) -> ListResponseHeadersPoliciesResultTypeDef:
         """
         Gets a list of response headers policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_response_headers_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_response_headers_policies)
         """
+
     def list_streaming_distributions(
         self, *, Marker: str = ..., MaxItems: str = ...
     ) -> ListStreamingDistributionsResultTypeDef:
         """
         List streaming distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_streaming_distributions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_streaming_distributions)
         """
+
     def list_tags_for_resource(self, *, Resource: str) -> ListTagsForResourceResultTypeDef:
         """
         List tags for a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#list_tags_for_resource)
         """
+
     def publish_function(self, *, Name: str, IfMatch: str) -> PublishFunctionResultTypeDef:
         """
         Publishes a CloudFront function by copying the function code from the
         `DEVELOPMENT` stage to `LIVE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.publish_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#publish_function)
         """
+
     def tag_resource(self, *, Resource: str, Tags: TagsTypeDef) -> EmptyResponseMetadataTypeDef:
         """
         Add tags to a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#tag_resource)
         """
+
     def test_function(
         self,
         *,
         Name: str,
         IfMatch: str,
         EventObject: Union[str, bytes, IO[Any], StreamingBody],
         Stage: FunctionStageType = ...
     ) -> TestFunctionResultTypeDef:
         """
         Tests a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.test_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#test_function)
         """
+
     def untag_resource(
         self, *, Resource: str, TagKeys: TagKeysTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Remove tags from a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#untag_resource)
         """
+
     def update_cache_policy(
         self, *, CachePolicyConfig: CachePolicyConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateCachePolicyResultTypeDef:
         """
         Updates a cache policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cache_policy)
         """
+
     def update_cloud_front_origin_access_identity(
         self,
         *,
         CloudFrontOriginAccessIdentityConfig: CloudFrontOriginAccessIdentityConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateCloudFrontOriginAccessIdentityResultTypeDef:
         """
         Update an origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
+
     def update_continuous_deployment_policy(
         self,
         *,
         ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_continuous_deployment_policy)
         """
+
     def update_distribution(
         self, *, DistributionConfig: DistributionConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates the configuration for a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution)
         """
+
     def update_distribution_with_staging_config(
         self, *, Id: str, StagingDistributionId: str = ..., IfMatch: str = ...
     ) -> UpdateDistributionWithStagingConfigResultTypeDef:
         """
         Copies the staging distribution's configuration to its corresponding primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution_with_staging_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution_with_staging_config)
         """
+
     def update_field_level_encryption_config(
         self,
         *,
         FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_field_level_encryption_config)
         """
+
     def update_field_level_encryption_profile(
         self,
         *,
         FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_field_level_encryption_profile)
         """
+
     def update_function(
         self,
         *,
         Name: str,
         IfMatch: str,
         FunctionConfig: FunctionConfigTypeDef,
         FunctionCode: Union[str, bytes, IO[Any], StreamingBody]
     ) -> UpdateFunctionResultTypeDef:
         """
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_function)
         """
+
     def update_key_group(
         self, *, KeyGroupConfig: KeyGroupConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateKeyGroupResultTypeDef:
         """
         Updates a key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_key_group)
         """
+
     def update_origin_access_control(
         self,
         *,
         OriginAccessControlConfig: OriginAccessControlConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateOriginAccessControlResultTypeDef:
         """
         Updates a CloudFront origin access control.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_origin_access_control)
         """
+
     def update_origin_request_policy(
         self,
         *,
         OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_origin_request_policy)
         """
+
     def update_public_key(
         self, *, PublicKeyConfig: PublicKeyConfigTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdatePublicKeyResultTypeDef:
         """
         Update public key information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_public_key)
         """
+
     def update_realtime_log_config(
         self,
         *,
         EndPoints: Sequence[EndPointTypeDef] = ...,
         Fields: Sequence[str] = ...,
         Name: str = ...,
         ARN: str = ...,
@@ -1326,88 +1438,97 @@
     ) -> UpdateRealtimeLogConfigResultTypeDef:
         """
         Updates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_realtime_log_config)
         """
+
     def update_response_headers_policy(
         self,
         *,
         ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_response_headers_policy)
         """
+
     def update_streaming_distribution(
         self,
         *,
         StreamingDistributionConfig: StreamingDistributionConfigTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_streaming_distribution)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_cloud_front_origin_access_identities"]
     ) -> ListCloudFrontOriginAccessIdentitiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_distributions"]
     ) -> ListDistributionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_invalidations"]
     ) -> ListInvalidationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_streaming_distributions"]
     ) -> ListStreamingDistributionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_paginator)
         """
+
     @overload
     def get_waiter(
         self, waiter_name: Literal["distribution_deployed"]
     ) -> DistributionDeployedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_waiter)
         """
+
     @overload
     def get_waiter(
         self, waiter_name: Literal["invalidation_completed"]
     ) -> InvalidationCompletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_waiter)
         """
+
     @overload
     def get_waiter(
         self, waiter_name: Literal["streaming_distribution_deployed"]
     ) -> StreamingDistributionDeployedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#get_waiter)
```

### Comparing `mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/literals.py` & `mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,15 @@
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
@@ -184,14 +185,15 @@
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
@@ -270,14 +272,15 @@
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
@@ -288,14 +291,15 @@
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
@@ -331,14 +335,15 @@
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
@@ -357,16 +362,19 @@
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
@@ -450,15 +458,17 @@
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

### Comparing `mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/literals.pyi` & `mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
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
@@ -182,14 +183,15 @@
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
@@ -268,14 +270,15 @@
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
@@ -286,14 +289,15 @@
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
@@ -329,14 +333,15 @@
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
@@ -355,16 +360,19 @@
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
@@ -448,15 +456,17 @@
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

### Comparing `mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/paginator.py` & `mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,58 +58,58 @@
 class ListCloudFrontOriginAccessIdentitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCloudFrontOriginAccessIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
         """
 
 
 class ListDistributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listdistributionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDistributionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listdistributionspaginator)
         """
 
 
 class ListInvalidationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listinvalidationspaginator)
     """
 
     def paginate(
-        self, *, DistributionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DistributionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInvalidationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listinvalidationspaginator)
         """
 
 
 class ListStreamingDistributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#liststreamingdistributionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamingDistributionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#liststreamingdistributionspaginator)
         """
```

### Comparing `mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/paginator.pyi` & `mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -55,55 +55,55 @@
 class ListCloudFrontOriginAccessIdentitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCloudFrontOriginAccessIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
         """
 
 class ListDistributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listdistributionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDistributionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listdistributionspaginator)
         """
 
 class ListInvalidationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listinvalidationspaginator)
     """
 
     def paginate(
-        self, *, DistributionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DistributionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListInvalidationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#listinvalidationspaginator)
         """
 
 class ListStreamingDistributionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#liststreamingdistributionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListStreamingDistributionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/paginators/#liststreamingdistributionspaginator)
         """
```

### Comparing `mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/type_defs.py` & `mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     "CloudFrontOriginAccessIdentitySummaryTypeDef",
     "ConflictingAliasTypeDef",
     "ContentTypeProfileTypeDef",
     "StagingDistributionDnsNamesTypeDef",
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     "SessionStickinessConfigTypeDef",
     "CopyDistributionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "FunctionConfigTypeDef",
     "KeyGroupConfigTypeDef",
     "OriginAccessControlConfigTypeDef",
     "PublicKeyConfigTypeDef",
     "CustomErrorResponseTypeDef",
     "OriginCustomHeaderTypeDef",
     "OriginSslProtocolsTypeDef",
@@ -101,14 +100,15 @@
     "DeleteRealtimeLogConfigRequestRequestTypeDef",
     "DeleteResponseHeadersPolicyRequestRequestTypeDef",
     "DeleteStreamingDistributionRequestRequestTypeDef",
     "DescribeFunctionRequestRequestTypeDef",
     "LoggingConfigTypeDef",
     "ViewerCertificateTypeDef",
     "DistributionIdListTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "FieldPatternsTypeDef",
     "KinesisStreamConfigTypeDef",
     "QueryStringCacheKeysTypeDef",
     "FunctionAssociationTypeDef",
     "FunctionMetadataTypeDef",
     "GeoRestrictionTypeDef",
     "GetCachePolicyConfigRequestRequestTypeDef",
@@ -121,14 +121,15 @@
     "WaiterConfigTypeDef",
     "GetDistributionRequestRequestTypeDef",
     "GetFieldLevelEncryptionConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileRequestRequestTypeDef",
     "GetFieldLevelEncryptionRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
+    "GetFunctionResultTypeDef",
     "GetInvalidationRequestRequestTypeDef",
     "GetKeyGroupConfigRequestRequestTypeDef",
     "GetKeyGroupRequestRequestTypeDef",
     "GetMonitoringSubscriptionRequestRequestTypeDef",
     "GetOriginAccessControlConfigRequestRequestTypeDef",
     "GetOriginAccessControlRequestRequestTypeDef",
     "GetOriginRequestPolicyConfigRequestRequestTypeDef",
@@ -141,43 +142,47 @@
     "GetStreamingDistributionConfigRequestRequestTypeDef",
     "GetStreamingDistributionRequestRequestTypeDef",
     "PathsTypeDef",
     "InvalidationSummaryTypeDef",
     "KeyPairIdsTypeDef",
     "LambdaFunctionAssociationTypeDef",
     "ListCachePoliciesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
     "ListConflictingAliasesRequestRequestTypeDef",
     "ListContinuousDeploymentPoliciesRequestRequestTypeDef",
     "ListDistributionsByCachePolicyIdRequestRequestTypeDef",
     "ListDistributionsByKeyGroupRequestRequestTypeDef",
     "ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef",
     "ListDistributionsByRealtimeLogConfigRequestRequestTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef",
     "ListDistributionsByWebACLIdRequestRequestTypeDef",
+    "ListDistributionsRequestListDistributionsPaginateTypeDef",
     "ListDistributionsRequestRequestTypeDef",
     "ListFieldLevelEncryptionConfigsRequestRequestTypeDef",
     "ListFieldLevelEncryptionProfilesRequestRequestTypeDef",
     "ListFunctionsRequestRequestTypeDef",
+    "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
     "ListInvalidationsRequestRequestTypeDef",
     "ListKeyGroupsRequestRequestTypeDef",
     "ListOriginAccessControlsRequestRequestTypeDef",
     "ListOriginRequestPoliciesRequestRequestTypeDef",
     "ListPublicKeysRequestRequestTypeDef",
     "ListRealtimeLogConfigsRequestRequestTypeDef",
     "ListResponseHeadersPoliciesRequestRequestTypeDef",
+    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "ListStreamingDistributionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RealtimeMetricsSubscriptionConfigTypeDef",
     "OriginAccessControlSummaryTypeDef",
     "StatusCodesTypeDef",
     "OriginGroupMemberTypeDef",
     "OriginShieldTypeDef",
     "S3OriginConfigTypeDef",
+    "PaginatorConfigTypeDef",
     "PublicKeySummaryTypeDef",
     "PublishFunctionRequestRequestTypeDef",
     "QueryArgProfileTypeDef",
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
     "ResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
@@ -186,14 +191,15 @@
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
     "ResponseHeadersPolicyCustomHeaderTypeDef",
     "ResponseHeadersPolicyFrameOptionsTypeDef",
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
     "ResponseHeadersPolicyRemoveHeaderTypeDef",
     "ResponseHeadersPolicyStrictTransportSecurityTypeDef",
     "ResponseHeadersPolicyXSSProtectionTypeDef",
+    "ResponseMetadataTypeDef",
     "S3OriginTypeDef",
     "StreamingLoggingConfigTypeDef",
     "TagKeysTypeDef",
     "TagTypeDef",
     "TestFunctionRequestRequestTypeDef",
     "UpdateDistributionWithStagingConfigRequestRequestTypeDef",
     "AllowedMethodsTypeDef",
@@ -202,22 +208,20 @@
     "OriginRequestPolicyCookiesConfigTypeDef",
     "CachePolicyHeadersConfigTypeDef",
     "OriginRequestPolicyHeadersConfigTypeDef",
     "CachePolicyQueryStringsConfigTypeDef",
     "OriginRequestPolicyQueryStringsConfigTypeDef",
     "CloudFrontOriginAccessIdentityTypeDef",
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
+    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
     "UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "CloudFrontOriginAccessIdentityListTypeDef",
     "ConflictingAliasesListTypeDef",
     "ContentTypeProfilesTypeDef",
     "ContinuousDeploymentSingleWeightConfigTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
-    "GetFunctionResultTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
     "CreateKeyGroupRequestRequestTypeDef",
     "GetKeyGroupConfigResultTypeDef",
     "KeyGroupTypeDef",
     "UpdateKeyGroupRequestRequestTypeDef",
     "CreateOriginAccessControlRequestRequestTypeDef",
@@ -244,18 +248,14 @@
     "GetInvalidationRequestInvalidationCompletedWaitTypeDef",
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     "InvalidationBatchTypeDef",
     "InvalidationListTypeDef",
     "KGKeyPairIdsTypeDef",
     "SignerTypeDef",
     "LambdaFunctionAssociationsTypeDef",
-    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
-    "ListDistributionsRequestListDistributionsPaginateTypeDef",
-    "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
-    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "MonitoringSubscriptionTypeDef",
     "OriginAccessControlListTypeDef",
     "OriginGroupFailoverCriteriaTypeDef",
     "OriginGroupMembersTypeDef",
     "PublicKeyListTypeDef",
     "QueryArgProfilesTypeDef",
     "ResponseHeadersPolicyCorsConfigTypeDef",
@@ -670,25 +670,14 @@
 
 class CopyDistributionRequestRequestTypeDef(
     _RequiredCopyDistributionRequestRequestTypeDef, _OptionalCopyDistributionRequestRequestTypeDef
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
 FunctionConfigTypeDef = TypedDict(
     "FunctionConfigTypeDef",
     {
         "Comment": str,
         "Runtime": Literal["cloudfront-js-1.0"],
     },
 )
@@ -1148,14 +1137,21 @@
 
 class DistributionIdListTypeDef(
     _RequiredDistributionIdListTypeDef, _OptionalDistributionIdListTypeDef
 ):
     pass
 
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFieldPatternsTypeDef = TypedDict(
     "_RequiredFieldPatternsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalFieldPatternsTypeDef = TypedDict(
@@ -1359,14 +1355,24 @@
 
 class GetFunctionRequestRequestTypeDef(
     _RequiredGetFunctionRequestRequestTypeDef, _OptionalGetFunctionRequestRequestTypeDef
 ):
     pass
 
 
+GetFunctionResultTypeDef = TypedDict(
+    "GetFunctionResultTypeDef",
+    {
+        "FunctionCode": StreamingBody,
+        "ETag": str,
+        "ContentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetInvalidationRequestRequestTypeDef = TypedDict(
     "GetInvalidationRequestRequestTypeDef",
     {
         "DistributionId": str,
         "Id": str,
     },
 )
@@ -1546,20 +1552,18 @@
         "Type": CachePolicyTypeType,
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
+    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
     {
@@ -1724,14 +1728,22 @@
 class ListDistributionsByWebACLIdRequestRequestTypeDef(
     _RequiredListDistributionsByWebACLIdRequestRequestTypeDef,
     _OptionalListDistributionsByWebACLIdRequestRequestTypeDef,
 ):
     pass
 
 
+ListDistributionsRequestListDistributionsPaginateTypeDef = TypedDict(
+    "ListDistributionsRequestListDistributionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDistributionsRequestRequestTypeDef = TypedDict(
     "ListDistributionsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1761,14 +1773,36 @@
         "Marker": str,
         "MaxItems": str,
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
+_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
+    "_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    {
+        "DistributionId": str,
+    },
+)
+_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
+    "_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListInvalidationsRequestListInvalidationsPaginateTypeDef(
+    _RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef,
+    _OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListInvalidationsRequestRequestTypeDef = TypedDict(
     "_RequiredListInvalidationsRequestRequestTypeDef",
     {
         "DistributionId": str,
     },
 )
 _OptionalListInvalidationsRequestRequestTypeDef = TypedDict(
@@ -1839,14 +1873,22 @@
         "Type": ResponseHeadersPolicyTypeType,
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef = TypedDict(
+    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStreamingDistributionsRequestRequestTypeDef = TypedDict(
     "ListStreamingDistributionsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1915,14 +1957,24 @@
 S3OriginConfigTypeDef = TypedDict(
     "S3OriginConfigTypeDef",
     {
         "OriginAccessIdentity": str,
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
 _RequiredPublicKeySummaryTypeDef = TypedDict(
     "_RequiredPublicKeySummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "CreatedTime": datetime,
         "EncodedKey": str,
@@ -2116,14 +2168,25 @@
 class ResponseHeadersPolicyXSSProtectionTypeDef(
     _RequiredResponseHeadersPolicyXSSProtectionTypeDef,
     _OptionalResponseHeadersPolicyXSSProtectionTypeDef,
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
 S3OriginTypeDef = TypedDict(
     "S3OriginTypeDef",
     {
         "DomainName": str,
         "OriginAccessIdentity": str,
     },
 )
@@ -2403,14 +2466,23 @@
 CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
     },
 )
 
+GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
+    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
+    {
+        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
         "Id": str,
     },
 )
@@ -2506,40 +2578,14 @@
 class ContinuousDeploymentSingleWeightConfigTypeDef(
     _RequiredContinuousDeploymentSingleWeightConfigTypeDef,
     _OptionalContinuousDeploymentSingleWeightConfigTypeDef,
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
-    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
-    {
-        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetFunctionResultTypeDef = TypedDict(
-    "GetFunctionResultTypeDef",
-    {
-        "FunctionCode": StreamingBody,
-        "ETag": str,
-        "ContentType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateFunctionRequestRequestTypeDef = TypedDict(
     "CreateFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "FunctionConfig": FunctionConfigTypeDef,
         "FunctionCode": Union[str, bytes, IO[Any], StreamingBody],
     },
@@ -2563,15 +2609,15 @@
 )
 
 GetKeyGroupConfigResultTypeDef = TypedDict(
     "GetKeyGroupConfigResultTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 KeyGroupTypeDef = TypedDict(
     "KeyGroupTypeDef",
     {
         "Id": str,
@@ -2610,15 +2656,15 @@
 )
 
 GetOriginAccessControlConfigResultTypeDef = TypedDict(
     "GetOriginAccessControlConfigResultTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredOriginAccessControlTypeDef = TypedDict(
     "_RequiredOriginAccessControlTypeDef",
     {
         "Id": str,
@@ -2670,15 +2716,15 @@
 )
 
 GetPublicKeyConfigResultTypeDef = TypedDict(
     "GetPublicKeyConfigResultTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PublicKeyTypeDef = TypedDict(
     "PublicKeyTypeDef",
     {
         "Id": str,
@@ -2774,39 +2820,39 @@
     pass
 
 
 ListDistributionsByCachePolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByCachePolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDistributionsByKeyGroupResultTypeDef = TypedDict(
     "ListDistributionsByKeyGroupResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDistributionsByOriginRequestPolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDistributionsByResponseHeadersPolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EncryptionEntityTypeDef = TypedDict(
     "EncryptionEntityTypeDef",
     {
         "PublicKeyId": str,
@@ -3016,60 +3062,14 @@
 
 class LambdaFunctionAssociationsTypeDef(
     _RequiredLambdaFunctionAssociationsTypeDef, _OptionalLambdaFunctionAssociationsTypeDef
 ):
     pass
 
 
-ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
-    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDistributionsRequestListDistributionsPaginateTypeDef = TypedDict(
-    "ListDistributionsRequestListDistributionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
-    "_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef",
-    {
-        "DistributionId": str,
-    },
-)
-_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
-    "_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListInvalidationsRequestListInvalidationsPaginateTypeDef(
-    _RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef,
-    _OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef,
-):
-    pass
-
-
-ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef = TypedDict(
-    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 MonitoringSubscriptionTypeDef = TypedDict(
     "MonitoringSubscriptionTypeDef",
     {
         "RealtimeMetricsSubscriptionConfig": RealtimeMetricsSubscriptionConfigTypeDef,
     },
     total=False,
 )
@@ -3369,49 +3369,49 @@
 
 CreateCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCloudFrontOriginAccessIdentitiesResultTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     {
         "CloudFrontOriginAccessIdentityList": CloudFrontOriginAccessIdentityListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListConflictingAliasesResultTypeDef = TypedDict(
     "ListConflictingAliasesResultTypeDef",
     {
         "ConflictingAliasesList": ConflictingAliasesListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredContentTypeProfileConfigTypeDef = TypedDict(
     "_RequiredContentTypeProfileConfigTypeDef",
     {
         "ForwardWhenContentTypeIsUnknown": bool,
@@ -3454,24 +3454,24 @@
 
 CreateKeyGroupResultTypeDef = TypedDict(
     "CreateKeyGroupResultTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKeyGroupResultTypeDef = TypedDict(
     "GetKeyGroupResultTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 KeyGroupSummaryTypeDef = TypedDict(
     "KeyGroupSummaryTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
@@ -3479,71 +3479,71 @@
 )
 
 UpdateKeyGroupResultTypeDef = TypedDict(
     "UpdateKeyGroupResultTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateOriginAccessControlResultTypeDef = TypedDict(
     "CreateOriginAccessControlResultTypeDef",
     {
         "OriginAccessControl": OriginAccessControlTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOriginAccessControlResultTypeDef = TypedDict(
     "GetOriginAccessControlResultTypeDef",
     {
         "OriginAccessControl": OriginAccessControlTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateOriginAccessControlResultTypeDef = TypedDict(
     "UpdateOriginAccessControlResultTypeDef",
     {
         "OriginAccessControl": OriginAccessControlTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePublicKeyResultTypeDef = TypedDict(
     "CreatePublicKeyResultTypeDef",
     {
         "PublicKey": PublicKeyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPublicKeyResultTypeDef = TypedDict(
     "GetPublicKeyResultTypeDef",
     {
         "PublicKey": PublicKeyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePublicKeyResultTypeDef = TypedDict(
     "UpdatePublicKeyResultTypeDef",
     {
         "PublicKey": PublicKeyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredOriginTypeDef = TypedDict(
     "_RequiredOriginTypeDef",
     {
         "Id": str,
@@ -3626,24 +3626,24 @@
 
 CreateFunctionResultTypeDef = TypedDict(
     "CreateFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFunctionResultTypeDef = TypedDict(
     "DescribeFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFunctionListTypeDef = TypedDict(
     "_RequiredFunctionListTypeDef",
     {
         "MaxItems": int,
@@ -3664,15 +3664,15 @@
     pass
 
 
 PublishFunctionResultTypeDef = TypedDict(
     "PublishFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestResultTypeDef = TypedDict(
     "TestResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
@@ -3685,15 +3685,15 @@
 )
 
 UpdateFunctionResultTypeDef = TypedDict(
     "UpdateFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInvalidationRequestRequestTypeDef = TypedDict(
     "CreateInvalidationRequestRequestTypeDef",
     {
         "DistributionId": str,
@@ -3711,15 +3711,15 @@
     },
 )
 
 ListInvalidationsResultTypeDef = TypedDict(
     "ListInvalidationsResultTypeDef",
     {
         "InvalidationList": InvalidationListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredActiveTrustedKeyGroupsTypeDef = TypedDict(
     "_RequiredActiveTrustedKeyGroupsTypeDef",
     {
         "Enabled": bool,
@@ -3771,31 +3771,31 @@
     },
 )
 
 CreateMonitoringSubscriptionResultTypeDef = TypedDict(
     "CreateMonitoringSubscriptionResultTypeDef",
     {
         "MonitoringSubscription": MonitoringSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMonitoringSubscriptionResultTypeDef = TypedDict(
     "GetMonitoringSubscriptionResultTypeDef",
     {
         "MonitoringSubscription": MonitoringSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOriginAccessControlsResultTypeDef = TypedDict(
     "ListOriginAccessControlsResultTypeDef",
     {
         "OriginAccessControlList": OriginAccessControlListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OriginGroupTypeDef = TypedDict(
     "OriginGroupTypeDef",
     {
         "Id": str,
@@ -3804,15 +3804,15 @@
     },
 )
 
 ListPublicKeysResultTypeDef = TypedDict(
     "ListPublicKeysResultTypeDef",
     {
         "PublicKeyList": PublicKeyListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredQueryArgProfileConfigTypeDef = TypedDict(
     "_RequiredQueryArgProfileConfigTypeDef",
     {
         "ForwardWhenQueryArgProfileIsUnknown": bool,
@@ -3892,15 +3892,15 @@
 )
 
 GetStreamingDistributionConfigResultTypeDef = TypedDict(
     "GetStreamingDistributionConfigResultTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
@@ -3923,15 +3923,15 @@
     pass
 
 
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "Tags": TagsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StreamingDistributionConfigWithTagsTypeDef = TypedDict(
     "StreamingDistributionConfigWithTagsTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
@@ -4053,15 +4053,15 @@
 )
 
 GetOriginRequestPolicyConfigResultTypeDef = TypedDict(
     "GetOriginRequestPolicyConfigResultTypeDef",
     {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OriginRequestPolicyTypeDef = TypedDict(
     "OriginRequestPolicyTypeDef",
     {
         "Id": str,
@@ -4194,23 +4194,23 @@
     pass
 
 
 CreateRealtimeLogConfigResultTypeDef = TypedDict(
     "CreateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRealtimeLogConfigResultTypeDef = TypedDict(
     "GetRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRealtimeLogConfigsTypeDef = TypedDict(
     "_RequiredRealtimeLogConfigsTypeDef",
     {
         "MaxItems": int,
@@ -4234,48 +4234,48 @@
     pass
 
 
 UpdateRealtimeLogConfigResultTypeDef = TypedDict(
     "UpdateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFunctionsResultTypeDef = TypedDict(
     "ListFunctionsResultTypeDef",
     {
         "FunctionList": FunctionListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestFunctionResultTypeDef = TypedDict(
     "TestFunctionResultTypeDef",
     {
         "TestResult": TestResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInvalidationResultTypeDef = TypedDict(
     "CreateInvalidationResultTypeDef",
     {
         "Location": str,
         "Invalidation": InvalidationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInvalidationResultTypeDef = TypedDict(
     "GetInvalidationResultTypeDef",
     {
         "Invalidation": InvalidationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStreamingDistributionTypeDef = TypedDict(
     "_RequiredStreamingDistributionTypeDef",
     {
         "Id": str,
@@ -4375,15 +4375,15 @@
 )
 
 GetResponseHeadersPolicyConfigResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyConfigResultTypeDef",
     {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseHeadersPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyTypeDef",
     {
         "Id": str,
@@ -4415,15 +4415,15 @@
     pass
 
 
 ListStreamingDistributionsResultTypeDef = TypedDict(
     "ListStreamingDistributionsResultTypeDef",
     {
         "StreamingDistributionList": StreamingDistributionListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStreamingDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
     {
         "StreamingDistributionConfigWithTags": StreamingDistributionConfigWithTagsTypeDef,
@@ -4466,15 +4466,15 @@
 )
 
 GetCachePolicyConfigResultTypeDef = TypedDict(
     "GetCachePolicyConfigResultTypeDef",
     {
         "CachePolicyConfig": CachePolicyConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateCachePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCachePolicyRequestRequestTypeDef",
     {
         "CachePolicyConfig": CachePolicyConfigTypeDef,
@@ -4498,24 +4498,24 @@
 
 CreateOriginRequestPolicyResultTypeDef = TypedDict(
     "CreateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOriginRequestPolicyResultTypeDef = TypedDict(
     "GetOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OriginRequestPolicySummaryTypeDef = TypedDict(
     "OriginRequestPolicySummaryTypeDef",
     {
         "Type": OriginRequestPolicyTypeType,
@@ -4524,15 +4524,15 @@
 )
 
 UpdateOriginRequestPolicyResultTypeDef = TypedDict(
     "UpdateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ContinuousDeploymentPolicyTypeDef = TypedDict(
     "ContinuousDeploymentPolicyTypeDef",
     {
         "Id": str,
@@ -4549,15 +4549,15 @@
 )
 
 GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
     "GetContinuousDeploymentPolicyConfigResultTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
@@ -4580,15 +4580,15 @@
     pass
 
 
 ListKeyGroupsResultTypeDef = TypedDict(
     "ListKeyGroupsResultTypeDef",
     {
         "KeyGroupList": KeyGroupListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
@@ -4605,15 +4605,15 @@
 )
 
 GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
@@ -4659,53 +4659,53 @@
     pass
 
 
 ListRealtimeLogConfigsResultTypeDef = TypedDict(
     "ListRealtimeLogConfigsResultTypeDef",
     {
         "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStreamingDistributionResultTypeDef = TypedDict(
     "CreateStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStreamingDistributionWithTagsResultTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStreamingDistributionResultTypeDef = TypedDict(
     "GetStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStreamingDistributionResultTypeDef = TypedDict(
     "UpdateStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
@@ -4722,15 +4722,15 @@
 )
 
 GetFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
@@ -4778,24 +4778,24 @@
 
 CreateResponseHeadersPolicyResultTypeDef = TypedDict(
     "CreateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResponseHeadersPolicyResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseHeadersPolicySummaryTypeDef = TypedDict(
     "ResponseHeadersPolicySummaryTypeDef",
     {
         "Type": ResponseHeadersPolicyTypeType,
@@ -4804,15 +4804,15 @@
 )
 
 UpdateResponseHeadersPolicyResultTypeDef = TypedDict(
     "UpdateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDistributionConfigTypeDef = TypedDict(
     "_RequiredDistributionConfigTypeDef",
     {
         "CallerReference": str,
@@ -4900,33 +4900,33 @@
 
 CreateCachePolicyResultTypeDef = TypedDict(
     "CreateCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCachePolicyResultTypeDef = TypedDict(
     "GetCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCachePolicyResultTypeDef = TypedDict(
     "UpdateCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredOriginRequestPolicyListTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -4958,105 +4958,105 @@
 
 CreateContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "CreateContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "GetContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "UpdateContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "CreateFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "UpdateFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFieldLevelEncryptionProfilesResultTypeDef = TypedDict(
     "ListFieldLevelEncryptionProfilesResultTypeDef",
     {
         "FieldLevelEncryptionProfileList": FieldLevelEncryptionProfileListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "CreateFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFieldLevelEncryptionResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFieldLevelEncryptionConfigsResultTypeDef = TypedDict(
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     {
         "FieldLevelEncryptionList": FieldLevelEncryptionListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredResponseHeadersPolicyListTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -5122,15 +5122,15 @@
 
 
 GetDistributionConfigResultTypeDef = TypedDict(
     "GetDistributionConfigResultTypeDef",
     {
         "DistributionConfig": DistributionConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionRequestRequestTypeDef",
     {
         "DistributionConfig": DistributionConfigTypeDef,
@@ -5197,15 +5197,15 @@
     pass
 
 
 ListOriginRequestPoliciesResultTypeDef = TypedDict(
     "ListOriginRequestPoliciesResultTypeDef",
     {
         "OriginRequestPolicyList": OriginRequestPolicyListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredContinuousDeploymentPolicyListTypeDef = TypedDict(
     "_RequiredContinuousDeploymentPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -5228,15 +5228,15 @@
     pass
 
 
 ListResponseHeadersPoliciesResultTypeDef = TypedDict(
     "ListResponseHeadersPoliciesResultTypeDef",
     {
         "ResponseHeadersPolicyList": ResponseHeadersPolicyListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateDistributionWithTagsRequestRequestTypeDef",
     {
         "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
@@ -5245,97 +5245,97 @@
 
 CopyDistributionResultTypeDef = TypedDict(
     "CopyDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDistributionResultTypeDef = TypedDict(
     "CreateDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDistributionWithTagsResultTypeDef = TypedDict(
     "CreateDistributionWithTagsResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDistributionResultTypeDef = TypedDict(
     "GetDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDistributionResultTypeDef = TypedDict(
     "UpdateDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDistributionWithStagingConfigResultTypeDef = TypedDict(
     "UpdateDistributionWithStagingConfigResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDistributionsByRealtimeLogConfigResultTypeDef = TypedDict(
     "ListDistributionsByRealtimeLogConfigResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDistributionsByWebACLIdResultTypeDef = TypedDict(
     "ListDistributionsByWebACLIdResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDistributionsResultTypeDef = TypedDict(
     "ListDistributionsResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCachePoliciesResultTypeDef = TypedDict(
     "ListCachePoliciesResultTypeDef",
     {
         "CachePolicyList": CachePolicyListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListContinuousDeploymentPoliciesResultTypeDef = TypedDict(
     "ListContinuousDeploymentPoliciesResultTypeDef",
     {
         "ContinuousDeploymentPolicyList": ContinuousDeploymentPolicyListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/type_defs.pyi` & `mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -73,15 +73,14 @@
     "CloudFrontOriginAccessIdentitySummaryTypeDef",
     "ConflictingAliasTypeDef",
     "ContentTypeProfileTypeDef",
     "StagingDistributionDnsNamesTypeDef",
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     "SessionStickinessConfigTypeDef",
     "CopyDistributionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "FunctionConfigTypeDef",
     "KeyGroupConfigTypeDef",
     "OriginAccessControlConfigTypeDef",
     "PublicKeyConfigTypeDef",
     "CustomErrorResponseTypeDef",
     "OriginCustomHeaderTypeDef",
     "OriginSslProtocolsTypeDef",
@@ -100,14 +99,15 @@
     "DeleteRealtimeLogConfigRequestRequestTypeDef",
     "DeleteResponseHeadersPolicyRequestRequestTypeDef",
     "DeleteStreamingDistributionRequestRequestTypeDef",
     "DescribeFunctionRequestRequestTypeDef",
     "LoggingConfigTypeDef",
     "ViewerCertificateTypeDef",
     "DistributionIdListTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "FieldPatternsTypeDef",
     "KinesisStreamConfigTypeDef",
     "QueryStringCacheKeysTypeDef",
     "FunctionAssociationTypeDef",
     "FunctionMetadataTypeDef",
     "GeoRestrictionTypeDef",
     "GetCachePolicyConfigRequestRequestTypeDef",
@@ -120,14 +120,15 @@
     "WaiterConfigTypeDef",
     "GetDistributionRequestRequestTypeDef",
     "GetFieldLevelEncryptionConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileRequestRequestTypeDef",
     "GetFieldLevelEncryptionRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
+    "GetFunctionResultTypeDef",
     "GetInvalidationRequestRequestTypeDef",
     "GetKeyGroupConfigRequestRequestTypeDef",
     "GetKeyGroupRequestRequestTypeDef",
     "GetMonitoringSubscriptionRequestRequestTypeDef",
     "GetOriginAccessControlConfigRequestRequestTypeDef",
     "GetOriginAccessControlRequestRequestTypeDef",
     "GetOriginRequestPolicyConfigRequestRequestTypeDef",
@@ -140,43 +141,47 @@
     "GetStreamingDistributionConfigRequestRequestTypeDef",
     "GetStreamingDistributionRequestRequestTypeDef",
     "PathsTypeDef",
     "InvalidationSummaryTypeDef",
     "KeyPairIdsTypeDef",
     "LambdaFunctionAssociationTypeDef",
     "ListCachePoliciesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
     "ListConflictingAliasesRequestRequestTypeDef",
     "ListContinuousDeploymentPoliciesRequestRequestTypeDef",
     "ListDistributionsByCachePolicyIdRequestRequestTypeDef",
     "ListDistributionsByKeyGroupRequestRequestTypeDef",
     "ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef",
     "ListDistributionsByRealtimeLogConfigRequestRequestTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef",
     "ListDistributionsByWebACLIdRequestRequestTypeDef",
+    "ListDistributionsRequestListDistributionsPaginateTypeDef",
     "ListDistributionsRequestRequestTypeDef",
     "ListFieldLevelEncryptionConfigsRequestRequestTypeDef",
     "ListFieldLevelEncryptionProfilesRequestRequestTypeDef",
     "ListFunctionsRequestRequestTypeDef",
+    "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
     "ListInvalidationsRequestRequestTypeDef",
     "ListKeyGroupsRequestRequestTypeDef",
     "ListOriginAccessControlsRequestRequestTypeDef",
     "ListOriginRequestPoliciesRequestRequestTypeDef",
     "ListPublicKeysRequestRequestTypeDef",
     "ListRealtimeLogConfigsRequestRequestTypeDef",
     "ListResponseHeadersPoliciesRequestRequestTypeDef",
+    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "ListStreamingDistributionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RealtimeMetricsSubscriptionConfigTypeDef",
     "OriginAccessControlSummaryTypeDef",
     "StatusCodesTypeDef",
     "OriginGroupMemberTypeDef",
     "OriginShieldTypeDef",
     "S3OriginConfigTypeDef",
+    "PaginatorConfigTypeDef",
     "PublicKeySummaryTypeDef",
     "PublishFunctionRequestRequestTypeDef",
     "QueryArgProfileTypeDef",
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
     "ResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
@@ -185,14 +190,15 @@
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
     "ResponseHeadersPolicyCustomHeaderTypeDef",
     "ResponseHeadersPolicyFrameOptionsTypeDef",
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
     "ResponseHeadersPolicyRemoveHeaderTypeDef",
     "ResponseHeadersPolicyStrictTransportSecurityTypeDef",
     "ResponseHeadersPolicyXSSProtectionTypeDef",
+    "ResponseMetadataTypeDef",
     "S3OriginTypeDef",
     "StreamingLoggingConfigTypeDef",
     "TagKeysTypeDef",
     "TagTypeDef",
     "TestFunctionRequestRequestTypeDef",
     "UpdateDistributionWithStagingConfigRequestRequestTypeDef",
     "AllowedMethodsTypeDef",
@@ -201,22 +207,20 @@
     "OriginRequestPolicyCookiesConfigTypeDef",
     "CachePolicyHeadersConfigTypeDef",
     "OriginRequestPolicyHeadersConfigTypeDef",
     "CachePolicyQueryStringsConfigTypeDef",
     "OriginRequestPolicyQueryStringsConfigTypeDef",
     "CloudFrontOriginAccessIdentityTypeDef",
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
+    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
     "UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "CloudFrontOriginAccessIdentityListTypeDef",
     "ConflictingAliasesListTypeDef",
     "ContentTypeProfilesTypeDef",
     "ContinuousDeploymentSingleWeightConfigTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
-    "GetFunctionResultTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
     "CreateKeyGroupRequestRequestTypeDef",
     "GetKeyGroupConfigResultTypeDef",
     "KeyGroupTypeDef",
     "UpdateKeyGroupRequestRequestTypeDef",
     "CreateOriginAccessControlRequestRequestTypeDef",
@@ -243,18 +247,14 @@
     "GetInvalidationRequestInvalidationCompletedWaitTypeDef",
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     "InvalidationBatchTypeDef",
     "InvalidationListTypeDef",
     "KGKeyPairIdsTypeDef",
     "SignerTypeDef",
     "LambdaFunctionAssociationsTypeDef",
-    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
-    "ListDistributionsRequestListDistributionsPaginateTypeDef",
-    "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
-    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "MonitoringSubscriptionTypeDef",
     "OriginAccessControlListTypeDef",
     "OriginGroupFailoverCriteriaTypeDef",
     "OriginGroupMembersTypeDef",
     "PublicKeyListTypeDef",
     "QueryArgProfilesTypeDef",
     "ResponseHeadersPolicyCorsConfigTypeDef",
@@ -651,25 +651,14 @@
 )
 
 class CopyDistributionRequestRequestTypeDef(
     _RequiredCopyDistributionRequestRequestTypeDef, _OptionalCopyDistributionRequestRequestTypeDef
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
 FunctionConfigTypeDef = TypedDict(
     "FunctionConfigTypeDef",
     {
         "Comment": str,
         "Runtime": Literal["cloudfront-js-1.0"],
     },
 )
@@ -1093,14 +1082,21 @@
 )
 
 class DistributionIdListTypeDef(
     _RequiredDistributionIdListTypeDef, _OptionalDistributionIdListTypeDef
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFieldPatternsTypeDef = TypedDict(
     "_RequiredFieldPatternsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalFieldPatternsTypeDef = TypedDict(
@@ -1294,14 +1290,24 @@
 )
 
 class GetFunctionRequestRequestTypeDef(
     _RequiredGetFunctionRequestRequestTypeDef, _OptionalGetFunctionRequestRequestTypeDef
 ):
     pass
 
+GetFunctionResultTypeDef = TypedDict(
+    "GetFunctionResultTypeDef",
+    {
+        "FunctionCode": StreamingBody,
+        "ETag": str,
+        "ContentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetInvalidationRequestRequestTypeDef = TypedDict(
     "GetInvalidationRequestRequestTypeDef",
     {
         "DistributionId": str,
         "Id": str,
     },
 )
@@ -1475,20 +1481,18 @@
         "Type": CachePolicyTypeType,
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
+    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
     {
@@ -1641,14 +1645,22 @@
 
 class ListDistributionsByWebACLIdRequestRequestTypeDef(
     _RequiredListDistributionsByWebACLIdRequestRequestTypeDef,
     _OptionalListDistributionsByWebACLIdRequestRequestTypeDef,
 ):
     pass
 
+ListDistributionsRequestListDistributionsPaginateTypeDef = TypedDict(
+    "ListDistributionsRequestListDistributionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListDistributionsRequestRequestTypeDef = TypedDict(
     "ListDistributionsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1678,14 +1690,34 @@
         "Marker": str,
         "MaxItems": str,
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
+_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
+    "_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    {
+        "DistributionId": str,
+    },
+)
+_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
+    "_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListInvalidationsRequestListInvalidationsPaginateTypeDef(
+    _RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef,
+    _OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef,
+):
+    pass
+
 _RequiredListInvalidationsRequestRequestTypeDef = TypedDict(
     "_RequiredListInvalidationsRequestRequestTypeDef",
     {
         "DistributionId": str,
     },
 )
 _OptionalListInvalidationsRequestRequestTypeDef = TypedDict(
@@ -1754,14 +1786,22 @@
         "Type": ResponseHeadersPolicyTypeType,
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef = TypedDict(
+    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListStreamingDistributionsRequestRequestTypeDef = TypedDict(
     "ListStreamingDistributionsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1828,14 +1868,24 @@
 S3OriginConfigTypeDef = TypedDict(
     "S3OriginConfigTypeDef",
     {
         "OriginAccessIdentity": str,
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
 _RequiredPublicKeySummaryTypeDef = TypedDict(
     "_RequiredPublicKeySummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "CreatedTime": datetime,
         "EncodedKey": str,
@@ -2019,14 +2069,25 @@
 
 class ResponseHeadersPolicyXSSProtectionTypeDef(
     _RequiredResponseHeadersPolicyXSSProtectionTypeDef,
     _OptionalResponseHeadersPolicyXSSProtectionTypeDef,
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
 S3OriginTypeDef = TypedDict(
     "S3OriginTypeDef",
     {
         "DomainName": str,
         "OriginAccessIdentity": str,
     },
 )
@@ -2282,14 +2343,23 @@
 CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
     },
 )
 
+GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
+    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
+    {
+        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
         "Id": str,
     },
 )
@@ -2377,40 +2447,14 @@
 
 class ContinuousDeploymentSingleWeightConfigTypeDef(
     _RequiredContinuousDeploymentSingleWeightConfigTypeDef,
     _OptionalContinuousDeploymentSingleWeightConfigTypeDef,
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
-    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
-    {
-        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetFunctionResultTypeDef = TypedDict(
-    "GetFunctionResultTypeDef",
-    {
-        "FunctionCode": StreamingBody,
-        "ETag": str,
-        "ContentType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateFunctionRequestRequestTypeDef = TypedDict(
     "CreateFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "FunctionConfig": FunctionConfigTypeDef,
         "FunctionCode": Union[str, bytes, IO[Any], StreamingBody],
     },
@@ -2434,15 +2478,15 @@
 )
 
 GetKeyGroupConfigResultTypeDef = TypedDict(
     "GetKeyGroupConfigResultTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 KeyGroupTypeDef = TypedDict(
     "KeyGroupTypeDef",
     {
         "Id": str,
@@ -2479,15 +2523,15 @@
 )
 
 GetOriginAccessControlConfigResultTypeDef = TypedDict(
     "GetOriginAccessControlConfigResultTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredOriginAccessControlTypeDef = TypedDict(
     "_RequiredOriginAccessControlTypeDef",
     {
         "Id": str,
@@ -2535,15 +2579,15 @@
 )
 
 GetPublicKeyConfigResultTypeDef = TypedDict(
     "GetPublicKeyConfigResultTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PublicKeyTypeDef = TypedDict(
     "PublicKeyTypeDef",
     {
         "Id": str,
@@ -2631,39 +2675,39 @@
 ):
     pass
 
 ListDistributionsByCachePolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByCachePolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDistributionsByKeyGroupResultTypeDef = TypedDict(
     "ListDistributionsByKeyGroupResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDistributionsByOriginRequestPolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDistributionsByResponseHeadersPolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EncryptionEntityTypeDef = TypedDict(
     "EncryptionEntityTypeDef",
     {
         "PublicKeyId": str,
@@ -2857,58 +2901,14 @@
 )
 
 class LambdaFunctionAssociationsTypeDef(
     _RequiredLambdaFunctionAssociationsTypeDef, _OptionalLambdaFunctionAssociationsTypeDef
 ):
     pass
 
-ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
-    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListDistributionsRequestListDistributionsPaginateTypeDef = TypedDict(
-    "ListDistributionsRequestListDistributionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
-    "_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef",
-    {
-        "DistributionId": str,
-    },
-)
-_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
-    "_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListInvalidationsRequestListInvalidationsPaginateTypeDef(
-    _RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef,
-    _OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef,
-):
-    pass
-
-ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef = TypedDict(
-    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 MonitoringSubscriptionTypeDef = TypedDict(
     "MonitoringSubscriptionTypeDef",
     {
         "RealtimeMetricsSubscriptionConfig": RealtimeMetricsSubscriptionConfigTypeDef,
     },
     total=False,
 )
@@ -3188,49 +3188,49 @@
 
 CreateCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCloudFrontOriginAccessIdentitiesResultTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     {
         "CloudFrontOriginAccessIdentityList": CloudFrontOriginAccessIdentityListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListConflictingAliasesResultTypeDef = TypedDict(
     "ListConflictingAliasesResultTypeDef",
     {
         "ConflictingAliasesList": ConflictingAliasesListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredContentTypeProfileConfigTypeDef = TypedDict(
     "_RequiredContentTypeProfileConfigTypeDef",
     {
         "ForwardWhenContentTypeIsUnknown": bool,
@@ -3269,24 +3269,24 @@
 
 CreateKeyGroupResultTypeDef = TypedDict(
     "CreateKeyGroupResultTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetKeyGroupResultTypeDef = TypedDict(
     "GetKeyGroupResultTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 KeyGroupSummaryTypeDef = TypedDict(
     "KeyGroupSummaryTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
@@ -3294,71 +3294,71 @@
 )
 
 UpdateKeyGroupResultTypeDef = TypedDict(
     "UpdateKeyGroupResultTypeDef",
     {
         "KeyGroup": KeyGroupTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateOriginAccessControlResultTypeDef = TypedDict(
     "CreateOriginAccessControlResultTypeDef",
     {
         "OriginAccessControl": OriginAccessControlTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOriginAccessControlResultTypeDef = TypedDict(
     "GetOriginAccessControlResultTypeDef",
     {
         "OriginAccessControl": OriginAccessControlTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateOriginAccessControlResultTypeDef = TypedDict(
     "UpdateOriginAccessControlResultTypeDef",
     {
         "OriginAccessControl": OriginAccessControlTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreatePublicKeyResultTypeDef = TypedDict(
     "CreatePublicKeyResultTypeDef",
     {
         "PublicKey": PublicKeyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPublicKeyResultTypeDef = TypedDict(
     "GetPublicKeyResultTypeDef",
     {
         "PublicKey": PublicKeyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePublicKeyResultTypeDef = TypedDict(
     "UpdatePublicKeyResultTypeDef",
     {
         "PublicKey": PublicKeyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredOriginTypeDef = TypedDict(
     "_RequiredOriginTypeDef",
     {
         "Id": str,
@@ -3437,24 +3437,24 @@
 
 CreateFunctionResultTypeDef = TypedDict(
     "CreateFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFunctionResultTypeDef = TypedDict(
     "DescribeFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFunctionListTypeDef = TypedDict(
     "_RequiredFunctionListTypeDef",
     {
         "MaxItems": int,
@@ -3473,15 +3473,15 @@
 class FunctionListTypeDef(_RequiredFunctionListTypeDef, _OptionalFunctionListTypeDef):
     pass
 
 PublishFunctionResultTypeDef = TypedDict(
     "PublishFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestResultTypeDef = TypedDict(
     "TestResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
@@ -3494,15 +3494,15 @@
 )
 
 UpdateFunctionResultTypeDef = TypedDict(
     "UpdateFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInvalidationRequestRequestTypeDef = TypedDict(
     "CreateInvalidationRequestRequestTypeDef",
     {
         "DistributionId": str,
@@ -3520,15 +3520,15 @@
     },
 )
 
 ListInvalidationsResultTypeDef = TypedDict(
     "ListInvalidationsResultTypeDef",
     {
         "InvalidationList": InvalidationListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredActiveTrustedKeyGroupsTypeDef = TypedDict(
     "_RequiredActiveTrustedKeyGroupsTypeDef",
     {
         "Enabled": bool,
@@ -3576,31 +3576,31 @@
     },
 )
 
 CreateMonitoringSubscriptionResultTypeDef = TypedDict(
     "CreateMonitoringSubscriptionResultTypeDef",
     {
         "MonitoringSubscription": MonitoringSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMonitoringSubscriptionResultTypeDef = TypedDict(
     "GetMonitoringSubscriptionResultTypeDef",
     {
         "MonitoringSubscription": MonitoringSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListOriginAccessControlsResultTypeDef = TypedDict(
     "ListOriginAccessControlsResultTypeDef",
     {
         "OriginAccessControlList": OriginAccessControlListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OriginGroupTypeDef = TypedDict(
     "OriginGroupTypeDef",
     {
         "Id": str,
@@ -3609,15 +3609,15 @@
     },
 )
 
 ListPublicKeysResultTypeDef = TypedDict(
     "ListPublicKeysResultTypeDef",
     {
         "PublicKeyList": PublicKeyListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredQueryArgProfileConfigTypeDef = TypedDict(
     "_RequiredQueryArgProfileConfigTypeDef",
     {
         "ForwardWhenQueryArgProfileIsUnknown": bool,
@@ -3691,15 +3691,15 @@
 )
 
 GetStreamingDistributionConfigResultTypeDef = TypedDict(
     "GetStreamingDistributionConfigResultTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
@@ -3720,15 +3720,15 @@
 ):
     pass
 
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "Tags": TagsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StreamingDistributionConfigWithTagsTypeDef = TypedDict(
     "StreamingDistributionConfigWithTagsTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
@@ -3844,15 +3844,15 @@
 )
 
 GetOriginRequestPolicyConfigResultTypeDef = TypedDict(
     "GetOriginRequestPolicyConfigResultTypeDef",
     {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OriginRequestPolicyTypeDef = TypedDict(
     "OriginRequestPolicyTypeDef",
     {
         "Id": str,
@@ -3975,23 +3975,23 @@
 ):
     pass
 
 CreateRealtimeLogConfigResultTypeDef = TypedDict(
     "CreateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetRealtimeLogConfigResultTypeDef = TypedDict(
     "GetRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredRealtimeLogConfigsTypeDef = TypedDict(
     "_RequiredRealtimeLogConfigsTypeDef",
     {
         "MaxItems": int,
@@ -4013,48 +4013,48 @@
 ):
     pass
 
 UpdateRealtimeLogConfigResultTypeDef = TypedDict(
     "UpdateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFunctionsResultTypeDef = TypedDict(
     "ListFunctionsResultTypeDef",
     {
         "FunctionList": FunctionListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestFunctionResultTypeDef = TypedDict(
     "TestFunctionResultTypeDef",
     {
         "TestResult": TestResultTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateInvalidationResultTypeDef = TypedDict(
     "CreateInvalidationResultTypeDef",
     {
         "Location": str,
         "Invalidation": InvalidationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetInvalidationResultTypeDef = TypedDict(
     "GetInvalidationResultTypeDef",
     {
         "Invalidation": InvalidationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStreamingDistributionTypeDef = TypedDict(
     "_RequiredStreamingDistributionTypeDef",
     {
         "Id": str,
@@ -4146,15 +4146,15 @@
 )
 
 GetResponseHeadersPolicyConfigResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyConfigResultTypeDef",
     {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseHeadersPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyTypeDef",
     {
         "Id": str,
@@ -4184,15 +4184,15 @@
 ):
     pass
 
 ListStreamingDistributionsResultTypeDef = TypedDict(
     "ListStreamingDistributionsResultTypeDef",
     {
         "StreamingDistributionList": StreamingDistributionListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStreamingDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
     {
         "StreamingDistributionConfigWithTags": StreamingDistributionConfigWithTagsTypeDef,
@@ -4233,15 +4233,15 @@
 )
 
 GetCachePolicyConfigResultTypeDef = TypedDict(
     "GetCachePolicyConfigResultTypeDef",
     {
         "CachePolicyConfig": CachePolicyConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateCachePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCachePolicyRequestRequestTypeDef",
     {
         "CachePolicyConfig": CachePolicyConfigTypeDef,
@@ -4263,24 +4263,24 @@
 
 CreateOriginRequestPolicyResultTypeDef = TypedDict(
     "CreateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetOriginRequestPolicyResultTypeDef = TypedDict(
     "GetOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OriginRequestPolicySummaryTypeDef = TypedDict(
     "OriginRequestPolicySummaryTypeDef",
     {
         "Type": OriginRequestPolicyTypeType,
@@ -4289,15 +4289,15 @@
 )
 
 UpdateOriginRequestPolicyResultTypeDef = TypedDict(
     "UpdateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ContinuousDeploymentPolicyTypeDef = TypedDict(
     "ContinuousDeploymentPolicyTypeDef",
     {
         "Id": str,
@@ -4314,15 +4314,15 @@
 )
 
 GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
     "GetContinuousDeploymentPolicyConfigResultTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
@@ -4343,15 +4343,15 @@
 ):
     pass
 
 ListKeyGroupsResultTypeDef = TypedDict(
     "ListKeyGroupsResultTypeDef",
     {
         "KeyGroupList": KeyGroupListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
@@ -4368,15 +4368,15 @@
 )
 
 GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
@@ -4418,53 +4418,53 @@
 ):
     pass
 
 ListRealtimeLogConfigsResultTypeDef = TypedDict(
     "ListRealtimeLogConfigsResultTypeDef",
     {
         "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStreamingDistributionResultTypeDef = TypedDict(
     "CreateStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStreamingDistributionWithTagsResultTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStreamingDistributionResultTypeDef = TypedDict(
     "GetStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateStreamingDistributionResultTypeDef = TypedDict(
     "UpdateStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
@@ -4481,15 +4481,15 @@
 )
 
 GetFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
@@ -4533,24 +4533,24 @@
 
 CreateResponseHeadersPolicyResultTypeDef = TypedDict(
     "CreateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResponseHeadersPolicyResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseHeadersPolicySummaryTypeDef = TypedDict(
     "ResponseHeadersPolicySummaryTypeDef",
     {
         "Type": ResponseHeadersPolicyTypeType,
@@ -4559,15 +4559,15 @@
 )
 
 UpdateResponseHeadersPolicyResultTypeDef = TypedDict(
     "UpdateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDistributionConfigTypeDef = TypedDict(
     "_RequiredDistributionConfigTypeDef",
     {
         "CallerReference": str,
@@ -4651,33 +4651,33 @@
 
 CreateCachePolicyResultTypeDef = TypedDict(
     "CreateCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCachePolicyResultTypeDef = TypedDict(
     "GetCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCachePolicyResultTypeDef = TypedDict(
     "UpdateCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredOriginRequestPolicyListTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -4707,105 +4707,105 @@
 
 CreateContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "CreateContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "GetContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "UpdateContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "CreateFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "UpdateFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFieldLevelEncryptionProfilesResultTypeDef = TypedDict(
     "ListFieldLevelEncryptionProfilesResultTypeDef",
     {
         "FieldLevelEncryptionProfileList": FieldLevelEncryptionProfileListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "CreateFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFieldLevelEncryptionResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFieldLevelEncryptionConfigsResultTypeDef = TypedDict(
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     {
         "FieldLevelEncryptionList": FieldLevelEncryptionListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredResponseHeadersPolicyListTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -4867,15 +4867,15 @@
     pass
 
 GetDistributionConfigResultTypeDef = TypedDict(
     "GetDistributionConfigResultTypeDef",
     {
         "DistributionConfig": DistributionConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionRequestRequestTypeDef",
     {
         "DistributionConfig": DistributionConfigTypeDef,
@@ -4936,15 +4936,15 @@
 class CachePolicyListTypeDef(_RequiredCachePolicyListTypeDef, _OptionalCachePolicyListTypeDef):
     pass
 
 ListOriginRequestPoliciesResultTypeDef = TypedDict(
     "ListOriginRequestPoliciesResultTypeDef",
     {
         "OriginRequestPolicyList": OriginRequestPolicyListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredContinuousDeploymentPolicyListTypeDef = TypedDict(
     "_RequiredContinuousDeploymentPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -4965,15 +4965,15 @@
 ):
     pass
 
 ListResponseHeadersPoliciesResultTypeDef = TypedDict(
     "ListResponseHeadersPoliciesResultTypeDef",
     {
         "ResponseHeadersPolicyList": ResponseHeadersPolicyListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateDistributionWithTagsRequestRequestTypeDef",
     {
         "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
@@ -4982,97 +4982,97 @@
 
 CopyDistributionResultTypeDef = TypedDict(
     "CopyDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDistributionResultTypeDef = TypedDict(
     "CreateDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDistributionWithTagsResultTypeDef = TypedDict(
     "CreateDistributionWithTagsResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDistributionResultTypeDef = TypedDict(
     "GetDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDistributionResultTypeDef = TypedDict(
     "UpdateDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDistributionWithStagingConfigResultTypeDef = TypedDict(
     "UpdateDistributionWithStagingConfigResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDistributionsByRealtimeLogConfigResultTypeDef = TypedDict(
     "ListDistributionsByRealtimeLogConfigResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDistributionsByWebACLIdResultTypeDef = TypedDict(
     "ListDistributionsByWebACLIdResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDistributionsResultTypeDef = TypedDict(
     "ListDistributionsResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCachePoliciesResultTypeDef = TypedDict(
     "ListCachePoliciesResultTypeDef",
     {
         "CachePolicyList": CachePolicyListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListContinuousDeploymentPoliciesResultTypeDef = TypedDict(
     "ListContinuousDeploymentPoliciesResultTypeDef",
     {
         "ContinuousDeploymentPolicyList": ContinuousDeploymentPolicyListTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/waiter.py` & `mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront/waiter.pyi` & `mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront.egg-info/PKG-INFO` & `mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudfront
-Version: 1.26.77
-Summary: Type annotations for boto3.CloudFront 1.26.77 service generated with mypy-boto3-builder 7.12.4
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudFront 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-cloudfront"></a>
 
 # mypy-boto3-cloudfront
 
 [![PyPI - mypy-boto3-cloudfront](https://img.shields.io/pypi/v/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudfront?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
 
@@ -423,15 +423,14 @@
     CloudFrontOriginAccessIdentitySummaryTypeDef,
     ConflictingAliasTypeDef,
     ContentTypeProfileTypeDef,
     StagingDistributionDnsNamesTypeDef,
     ContinuousDeploymentSingleHeaderConfigTypeDef,
     SessionStickinessConfigTypeDef,
     CopyDistributionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     FunctionConfigTypeDef,
     KeyGroupConfigTypeDef,
     OriginAccessControlConfigTypeDef,
     PublicKeyConfigTypeDef,
     CustomErrorResponseTypeDef,
     OriginCustomHeaderTypeDef,
     OriginSslProtocolsTypeDef,
@@ -450,14 +449,15 @@
     DeleteRealtimeLogConfigRequestRequestTypeDef,
     DeleteResponseHeadersPolicyRequestRequestTypeDef,
     DeleteStreamingDistributionRequestRequestTypeDef,
     DescribeFunctionRequestRequestTypeDef,
     LoggingConfigTypeDef,
     ViewerCertificateTypeDef,
     DistributionIdListTypeDef,
+    EmptyResponseMetadataTypeDef,
     FieldPatternsTypeDef,
     KinesisStreamConfigTypeDef,
     QueryStringCacheKeysTypeDef,
     FunctionAssociationTypeDef,
     FunctionMetadataTypeDef,
     GeoRestrictionTypeDef,
     GetCachePolicyConfigRequestRequestTypeDef,
@@ -470,14 +470,15 @@
     WaiterConfigTypeDef,
     GetDistributionRequestRequestTypeDef,
     GetFieldLevelEncryptionConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileRequestRequestTypeDef,
     GetFieldLevelEncryptionRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
+    GetFunctionResultTypeDef,
     GetInvalidationRequestRequestTypeDef,
     GetKeyGroupConfigRequestRequestTypeDef,
     GetKeyGroupRequestRequestTypeDef,
     GetMonitoringSubscriptionRequestRequestTypeDef,
     GetOriginAccessControlConfigRequestRequestTypeDef,
     GetOriginAccessControlRequestRequestTypeDef,
     GetOriginRequestPolicyConfigRequestRequestTypeDef,
@@ -490,43 +491,47 @@
     GetStreamingDistributionConfigRequestRequestTypeDef,
     GetStreamingDistributionRequestRequestTypeDef,
     PathsTypeDef,
     InvalidationSummaryTypeDef,
     KeyPairIdsTypeDef,
     LambdaFunctionAssociationTypeDef,
     ListCachePoliciesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
     ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef,
     ListConflictingAliasesRequestRequestTypeDef,
     ListContinuousDeploymentPoliciesRequestRequestTypeDef,
     ListDistributionsByCachePolicyIdRequestRequestTypeDef,
     ListDistributionsByKeyGroupRequestRequestTypeDef,
     ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
     ListDistributionsByRealtimeLogConfigRequestRequestTypeDef,
     ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
     ListDistributionsByWebACLIdRequestRequestTypeDef,
+    ListDistributionsRequestListDistributionsPaginateTypeDef,
     ListDistributionsRequestRequestTypeDef,
     ListFieldLevelEncryptionConfigsRequestRequestTypeDef,
     ListFieldLevelEncryptionProfilesRequestRequestTypeDef,
     ListFunctionsRequestRequestTypeDef,
+    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
     ListInvalidationsRequestRequestTypeDef,
     ListKeyGroupsRequestRequestTypeDef,
     ListOriginAccessControlsRequestRequestTypeDef,
     ListOriginRequestPoliciesRequestRequestTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     ListRealtimeLogConfigsRequestRequestTypeDef,
     ListResponseHeadersPoliciesRequestRequestTypeDef,
+    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     ListStreamingDistributionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RealtimeMetricsSubscriptionConfigTypeDef,
     OriginAccessControlSummaryTypeDef,
     StatusCodesTypeDef,
     OriginGroupMemberTypeDef,
     OriginShieldTypeDef,
     S3OriginConfigTypeDef,
+    PaginatorConfigTypeDef,
     PublicKeySummaryTypeDef,
     PublishFunctionRequestRequestTypeDef,
     QueryArgProfileTypeDef,
     ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
     ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
     ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
     ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
@@ -535,14 +540,15 @@
     ResponseHeadersPolicyContentTypeOptionsTypeDef,
     ResponseHeadersPolicyCustomHeaderTypeDef,
     ResponseHeadersPolicyFrameOptionsTypeDef,
     ResponseHeadersPolicyReferrerPolicyTypeDef,
     ResponseHeadersPolicyRemoveHeaderTypeDef,
     ResponseHeadersPolicyStrictTransportSecurityTypeDef,
     ResponseHeadersPolicyXSSProtectionTypeDef,
+    ResponseMetadataTypeDef,
     S3OriginTypeDef,
     StreamingLoggingConfigTypeDef,
     TagKeysTypeDef,
     TagTypeDef,
     TestFunctionRequestRequestTypeDef,
     UpdateDistributionWithStagingConfigRequestRequestTypeDef,
     AllowedMethodsTypeDef,
@@ -551,22 +557,20 @@
     OriginRequestPolicyCookiesConfigTypeDef,
     CachePolicyHeadersConfigTypeDef,
     OriginRequestPolicyHeadersConfigTypeDef,
     CachePolicyQueryStringsConfigTypeDef,
     OriginRequestPolicyQueryStringsConfigTypeDef,
     CloudFrontOriginAccessIdentityTypeDef,
     CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
+    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     CloudFrontOriginAccessIdentityListTypeDef,
     ConflictingAliasesListTypeDef,
     ContentTypeProfilesTypeDef,
     ContinuousDeploymentSingleWeightConfigTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
-    GetFunctionResultTypeDef,
     CreateFunctionRequestRequestTypeDef,
     UpdateFunctionRequestRequestTypeDef,
     CreateKeyGroupRequestRequestTypeDef,
     GetKeyGroupConfigResultTypeDef,
     KeyGroupTypeDef,
     UpdateKeyGroupRequestRequestTypeDef,
     CreateOriginAccessControlRequestRequestTypeDef,
@@ -593,18 +597,14 @@
     GetInvalidationRequestInvalidationCompletedWaitTypeDef,
     GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
     InvalidationBatchTypeDef,
     InvalidationListTypeDef,
     KGKeyPairIdsTypeDef,
     SignerTypeDef,
     LambdaFunctionAssociationsTypeDef,
-    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
-    ListDistributionsRequestListDistributionsPaginateTypeDef,
-    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
-    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlListTypeDef,
     OriginGroupFailoverCriteriaTypeDef,
     OriginGroupMembersTypeDef,
     PublicKeyListTypeDef,
     QueryArgProfilesTypeDef,
     ResponseHeadersPolicyCorsConfigTypeDef,
@@ -781,42 +781,42 @@
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

### Comparing `mypy-boto3-cloudfront-1.26.77/mypy_boto3_cloudfront.egg-info/SOURCES.txt` & `mypy-boto3-cloudfront-1.27.0/mypy_boto3_cloudfront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.26.77/setup.py` & `mypy-boto3-cloudfront-1.27.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-cloudfront.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudfront",
-    version="1.26.77",
+    version="1.27.0",
     packages=["mypy_boto3_cloudfront"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudFront 1.26.77 service generated with mypy-boto3-builder"
-        " 7.12.4"
+        "Type annotations for boto3.CloudFront 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/",
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


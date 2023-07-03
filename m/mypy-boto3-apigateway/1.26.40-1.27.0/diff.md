# Comparing `tmp/mypy-boto3-apigateway-1.26.40.tar.gz` & `tmp/mypy-boto3-apigateway-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apigateway-1.26.40.tar", last modified: Thu Dec 29 20:24:58 2022, max compression
+gzip compressed data, was "mypy-boto3-apigateway-1.27.0.tar", last modified: Mon Jul  3 19:50:20 2023, max compression
```

## Comparing `mypy-boto3-apigateway-1.26.40.tar` & `mypy-boto3-apigateway-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 20:24:58.504753 mypy-boto3-apigateway-1.26.40/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-29 20:24:39.000000 mypy-boto3-apigateway-1.26.40/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24760 2022-12-29 20:24:58.504753 mypy-boto3-apigateway-1.26.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23261 2022-12-29 20:24:39.000000 mypy-boto3-apigateway-1.26.40/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 20:24:58.504753 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2022-12-29 20:24:39.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2022-12-29 20:24:39.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2022-12-29 20:24:40.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83079 2022-12-29 20:24:40.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    82934 2022-12-29 20:24:40.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2022-12-29 20:24:41.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12643 2022-12-29 20:24:41.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19996 2022-12-29 20:24:40.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19976 2022-12-29 20:24:40.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 20:24:40.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    92980 2022-12-29 20:24:43.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    92831 2022-12-29 20:24:42.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-29 20:24:39.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 20:24:58.504753 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24760 2022-12-29 20:24:58.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2022-12-29 20:24:58.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 20:24:58.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 20:24:58.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-29 20:24:58.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-29 20:24:58.000000 mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-29 20:24:58.504753 mypy-boto3-apigateway-1.26.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2022-12-29 20:24:39.000000 mypy-boto3-apigateway-1.26.40/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:20.346782 mypy-boto3-apigateway-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:13.000000 mypy-boto3-apigateway-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24739 2023-07-03 19:50:20.346782 mypy-boto3-apigateway-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23242 2023-07-03 19:32:13.000000 mypy-boto3-apigateway-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:20.346782 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-03 19:32:13.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-03 19:32:13.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:32:13.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83079 2023-07-03 19:32:15.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82934 2023-07-03 19:32:14.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-07-03 19:32:15.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-07-03 19:32:15.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20032 2023-07-03 19:32:15.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-07-03 19:32:15.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:13.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    93118 2023-07-03 19:32:17.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92969 2023-07-03 19:32:16.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:13.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:20.346782 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24739 2023-07-03 19:50:20.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:50:20.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:20.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:20.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:20.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:50:20.000000 mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:20.346782 mypy-boto3-apigateway-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:32:13.000000 mypy-boto3-apigateway-1.27.0/setup.py
```

### Comparing `mypy-boto3-apigateway-1.26.40/LICENSE` & `mypy-boto3-apigateway-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-apigateway-1.26.40/PKG-INFO` & `mypy-boto3-apigateway-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigateway
-Version: 1.26.40
-Summary: Type annotations for boto3.APIGateway 1.26.40 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.APIGateway 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-apigateway"></a>
 
 # mypy-boto3-apigateway
 
 [![PyPI - mypy-boto3-apigateway](https://img.shields.io/pypi/v/mypy-boto3-apigateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigateway)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apigateway?color=blue)](https://pypistats.org/packages/mypy-boto3-apigateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.APIGateway 1.26.40](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
+[boto3.APIGateway 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-apigateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -405,20 +405,24 @@
 
 `mypy_boto3_apigateway.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apigateway.type_defs import (
     AccessLogSettingsTypeDef,
-    ResponseMetadataTypeDef,
     ThrottleSettingsTypeDef,
+    ApiKeyIdsTypeDef,
+    ApiKeyResponseMetadataTypeDef,
     ApiKeyTypeDef,
+    AuthorizerResponseMetadataTypeDef,
     AuthorizerTypeDef,
+    BasePathMappingResponseMetadataTypeDef,
     BasePathMappingTypeDef,
     CanarySettingsTypeDef,
+    ClientCertificateResponseMetadataTypeDef,
     ClientCertificateTypeDef,
     StageKeyTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     CreateBasePathMappingRequestRequestTypeDef,
     DeploymentCanarySettingsTypeDef,
     DocumentationPartLocationTypeDef,
     CreateDocumentationVersionRequestRequestTypeDef,
@@ -448,110 +452,124 @@
     DeleteResourceRequestRequestTypeDef,
     DeleteRestApiRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteUsagePlanKeyRequestRequestTypeDef,
     DeleteUsagePlanRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     MethodSnapshotTypeDef,
+    DocumentationPartIdsTypeDef,
+    DocumentationVersionResponseMetadataTypeDef,
     DocumentationVersionTypeDef,
     MutualTlsAuthenticationTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportResponseTypeDef,
     FlushStageAuthorizersCacheRequestRequestTypeDef,
     FlushStageCacheRequestRequestTypeDef,
+    GatewayResponseResponseMetadataTypeDef,
     GatewayResponseTypeDef,
     GenerateClientCertificateRequestRequestTypeDef,
     GetApiKeyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetApiKeysRequestGetApiKeysPaginateTypeDef,
     GetApiKeysRequestRequestTypeDef,
     GetAuthorizerRequestRequestTypeDef,
+    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
     GetAuthorizersRequestRequestTypeDef,
     GetBasePathMappingRequestRequestTypeDef,
+    GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef,
     GetBasePathMappingsRequestRequestTypeDef,
     GetClientCertificateRequestRequestTypeDef,
+    GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef,
     GetClientCertificatesRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
+    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDocumentationPartRequestRequestTypeDef,
+    GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef,
     GetDocumentationPartsRequestRequestTypeDef,
     GetDocumentationVersionRequestRequestTypeDef,
+    GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef,
     GetDocumentationVersionsRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
+    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
     GetDomainNamesRequestRequestTypeDef,
     GetExportRequestRequestTypeDef,
     GetGatewayResponseRequestRequestTypeDef,
+    GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef,
     GetGatewayResponsesRequestRequestTypeDef,
     GetIntegrationRequestRequestTypeDef,
     GetIntegrationResponseRequestRequestTypeDef,
     GetMethodRequestRequestTypeDef,
     GetMethodResponseRequestRequestTypeDef,
     GetModelRequestRequestTypeDef,
     GetModelTemplateRequestRequestTypeDef,
+    GetModelsRequestGetModelsPaginateTypeDef,
     GetModelsRequestRequestTypeDef,
     GetRequestValidatorRequestRequestTypeDef,
+    GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef,
     GetRequestValidatorsRequestRequestTypeDef,
     GetResourceRequestRequestTypeDef,
+    GetResourcesRequestGetResourcesPaginateTypeDef,
     GetResourcesRequestRequestTypeDef,
     GetRestApiRequestRequestTypeDef,
+    GetRestApisRequestGetRestApisPaginateTypeDef,
     GetRestApisRequestRequestTypeDef,
     GetSdkRequestRequestTypeDef,
     GetSdkTypeRequestRequestTypeDef,
+    GetSdkTypesRequestGetSdkTypesPaginateTypeDef,
     GetSdkTypesRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
     GetStagesRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
     GetUsagePlanKeyRequestRequestTypeDef,
+    GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef,
     GetUsagePlanKeysRequestRequestTypeDef,
     GetUsagePlanRequestRequestTypeDef,
+    GetUsagePlansRequestGetUsagePlansPaginateTypeDef,
     GetUsagePlansRequestRequestTypeDef,
+    GetUsageRequestGetUsagePaginateTypeDef,
     GetUsageRequestRequestTypeDef,
     GetVpcLinkRequestRequestTypeDef,
+    GetVpcLinksRequestGetVpcLinksPaginateTypeDef,
     GetVpcLinksRequestRequestTypeDef,
     ImportApiKeysRequestRequestTypeDef,
     ImportDocumentationPartsRequestRequestTypeDef,
     ImportRestApiRequestRequestTypeDef,
     IntegrationResponseTypeDef,
     TlsConfigTypeDef,
+    IntegrationResponseResponseMetadataTypeDef,
     MethodResponseTypeDef,
+    MethodResponseResponseMetadataTypeDef,
     MethodSettingTypeDef,
+    ModelResponseMetadataTypeDef,
     ModelTypeDef,
+    PaginatorConfigTypeDef,
     PatchOperationTypeDef,
     PutGatewayResponseRequestRequestTypeDef,
     PutIntegrationResponseRequestRequestTypeDef,
     PutMethodRequestRequestTypeDef,
     PutMethodResponseRequestRequestTypeDef,
     PutRestApiRequestRequestTypeDef,
+    RequestValidatorResponseMetadataTypeDef,
     RequestValidatorTypeDef,
+    ResponseMetadataTypeDef,
     SdkConfigurationPropertyTypeDef,
-    TagResourceRequestRequestTypeDef,
-    TestInvokeAuthorizerRequestRequestTypeDef,
-    TestInvokeMethodRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UsagePlanKeyTypeDef,
-    VpcLinkTypeDef,
-    ApiKeyIdsTypeDef,
-    ApiKeyResponseMetadataTypeDef,
-    AuthorizerResponseMetadataTypeDef,
-    BasePathMappingResponseMetadataTypeDef,
-    ClientCertificateResponseMetadataTypeDef,
-    DocumentationPartIdsTypeDef,
-    DocumentationVersionResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportResponseTypeDef,
-    GatewayResponseResponseMetadataTypeDef,
-    IntegrationResponseResponseMetadataTypeDef,
-    MethodResponseResponseMetadataTypeDef,
-    ModelResponseMetadataTypeDef,
-    RequestValidatorResponseMetadataTypeDef,
     SdkResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     TagsTypeDef,
     TemplateTypeDef,
+    TestInvokeAuthorizerRequestRequestTypeDef,
     TestInvokeAuthorizerResponseTypeDef,
+    TestInvokeMethodRequestRequestTypeDef,
     TestInvokeMethodResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
     UsagePlanKeyResponseMetadataTypeDef,
+    UsagePlanKeyTypeDef,
     UsageTypeDef,
     VpcLinkResponseMetadataTypeDef,
+    VpcLinkTypeDef,
     AccountTypeDef,
     ApiStageTypeDef,
     ApiKeysTypeDef,
     AuthorizersTypeDef,
     BasePathMappingsTypeDef,
     CreateStageRequestRequestTypeDef,
     ClientCertificatesTypeDef,
@@ -566,32 +584,14 @@
     CreateDomainNameRequestRequestTypeDef,
     DeploymentResponseMetadataTypeDef,
     DeploymentTypeDef,
     DocumentationVersionsTypeDef,
     DomainNameResponseMetadataTypeDef,
     DomainNameTypeDef,
     GatewayResponsesTypeDef,
-    GetApiKeysRequestGetApiKeysPaginateTypeDef,
-    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-    GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef,
-    GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef,
-    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-    GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef,
-    GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef,
-    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
-    GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef,
-    GetModelsRequestGetModelsPaginateTypeDef,
-    GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef,
-    GetResourcesRequestGetResourcesPaginateTypeDef,
-    GetRestApisRequestGetRestApisPaginateTypeDef,
-    GetSdkTypesRequestGetSdkTypesPaginateTypeDef,
-    GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef,
-    GetUsagePlansRequestGetUsagePlansPaginateTypeDef,
-    GetUsageRequestGetUsagePaginateTypeDef,
-    GetVpcLinksRequestGetVpcLinksPaginateTypeDef,
     IntegrationResponseMetadataTypeDef,
     IntegrationTypeDef,
     PutIntegrationRequestRequestTypeDef,
     StageResponseMetadataTypeDef,
     StageTypeDef,
     ModelsTypeDef,
     UpdateAccountRequestRequestTypeDef,
@@ -646,42 +646,42 @@
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

### Comparing `mypy-boto3-apigateway-1.26.40/README.md` & `mypy-boto3-apigateway-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-apigateway"></a>
 
 # mypy-boto3-apigateway
 
 [![PyPI - mypy-boto3-apigateway](https://img.shields.io/pypi/v/mypy-boto3-apigateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigateway)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apigateway?color=blue)](https://pypistats.org/packages/mypy-boto3-apigateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.APIGateway 1.26.40](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
+[boto3.APIGateway 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-apigateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -373,20 +373,24 @@
 
 `mypy_boto3_apigateway.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apigateway.type_defs import (
     AccessLogSettingsTypeDef,
-    ResponseMetadataTypeDef,
     ThrottleSettingsTypeDef,
+    ApiKeyIdsTypeDef,
+    ApiKeyResponseMetadataTypeDef,
     ApiKeyTypeDef,
+    AuthorizerResponseMetadataTypeDef,
     AuthorizerTypeDef,
+    BasePathMappingResponseMetadataTypeDef,
     BasePathMappingTypeDef,
     CanarySettingsTypeDef,
+    ClientCertificateResponseMetadataTypeDef,
     ClientCertificateTypeDef,
     StageKeyTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     CreateBasePathMappingRequestRequestTypeDef,
     DeploymentCanarySettingsTypeDef,
     DocumentationPartLocationTypeDef,
     CreateDocumentationVersionRequestRequestTypeDef,
@@ -416,110 +420,124 @@
     DeleteResourceRequestRequestTypeDef,
     DeleteRestApiRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteUsagePlanKeyRequestRequestTypeDef,
     DeleteUsagePlanRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     MethodSnapshotTypeDef,
+    DocumentationPartIdsTypeDef,
+    DocumentationVersionResponseMetadataTypeDef,
     DocumentationVersionTypeDef,
     MutualTlsAuthenticationTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportResponseTypeDef,
     FlushStageAuthorizersCacheRequestRequestTypeDef,
     FlushStageCacheRequestRequestTypeDef,
+    GatewayResponseResponseMetadataTypeDef,
     GatewayResponseTypeDef,
     GenerateClientCertificateRequestRequestTypeDef,
     GetApiKeyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetApiKeysRequestGetApiKeysPaginateTypeDef,
     GetApiKeysRequestRequestTypeDef,
     GetAuthorizerRequestRequestTypeDef,
+    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
     GetAuthorizersRequestRequestTypeDef,
     GetBasePathMappingRequestRequestTypeDef,
+    GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef,
     GetBasePathMappingsRequestRequestTypeDef,
     GetClientCertificateRequestRequestTypeDef,
+    GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef,
     GetClientCertificatesRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
+    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDocumentationPartRequestRequestTypeDef,
+    GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef,
     GetDocumentationPartsRequestRequestTypeDef,
     GetDocumentationVersionRequestRequestTypeDef,
+    GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef,
     GetDocumentationVersionsRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
+    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
     GetDomainNamesRequestRequestTypeDef,
     GetExportRequestRequestTypeDef,
     GetGatewayResponseRequestRequestTypeDef,
+    GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef,
     GetGatewayResponsesRequestRequestTypeDef,
     GetIntegrationRequestRequestTypeDef,
     GetIntegrationResponseRequestRequestTypeDef,
     GetMethodRequestRequestTypeDef,
     GetMethodResponseRequestRequestTypeDef,
     GetModelRequestRequestTypeDef,
     GetModelTemplateRequestRequestTypeDef,
+    GetModelsRequestGetModelsPaginateTypeDef,
     GetModelsRequestRequestTypeDef,
     GetRequestValidatorRequestRequestTypeDef,
+    GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef,
     GetRequestValidatorsRequestRequestTypeDef,
     GetResourceRequestRequestTypeDef,
+    GetResourcesRequestGetResourcesPaginateTypeDef,
     GetResourcesRequestRequestTypeDef,
     GetRestApiRequestRequestTypeDef,
+    GetRestApisRequestGetRestApisPaginateTypeDef,
     GetRestApisRequestRequestTypeDef,
     GetSdkRequestRequestTypeDef,
     GetSdkTypeRequestRequestTypeDef,
+    GetSdkTypesRequestGetSdkTypesPaginateTypeDef,
     GetSdkTypesRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
     GetStagesRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
     GetUsagePlanKeyRequestRequestTypeDef,
+    GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef,
     GetUsagePlanKeysRequestRequestTypeDef,
     GetUsagePlanRequestRequestTypeDef,
+    GetUsagePlansRequestGetUsagePlansPaginateTypeDef,
     GetUsagePlansRequestRequestTypeDef,
+    GetUsageRequestGetUsagePaginateTypeDef,
     GetUsageRequestRequestTypeDef,
     GetVpcLinkRequestRequestTypeDef,
+    GetVpcLinksRequestGetVpcLinksPaginateTypeDef,
     GetVpcLinksRequestRequestTypeDef,
     ImportApiKeysRequestRequestTypeDef,
     ImportDocumentationPartsRequestRequestTypeDef,
     ImportRestApiRequestRequestTypeDef,
     IntegrationResponseTypeDef,
     TlsConfigTypeDef,
+    IntegrationResponseResponseMetadataTypeDef,
     MethodResponseTypeDef,
+    MethodResponseResponseMetadataTypeDef,
     MethodSettingTypeDef,
+    ModelResponseMetadataTypeDef,
     ModelTypeDef,
+    PaginatorConfigTypeDef,
     PatchOperationTypeDef,
     PutGatewayResponseRequestRequestTypeDef,
     PutIntegrationResponseRequestRequestTypeDef,
     PutMethodRequestRequestTypeDef,
     PutMethodResponseRequestRequestTypeDef,
     PutRestApiRequestRequestTypeDef,
+    RequestValidatorResponseMetadataTypeDef,
     RequestValidatorTypeDef,
+    ResponseMetadataTypeDef,
     SdkConfigurationPropertyTypeDef,
-    TagResourceRequestRequestTypeDef,
-    TestInvokeAuthorizerRequestRequestTypeDef,
-    TestInvokeMethodRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UsagePlanKeyTypeDef,
-    VpcLinkTypeDef,
-    ApiKeyIdsTypeDef,
-    ApiKeyResponseMetadataTypeDef,
-    AuthorizerResponseMetadataTypeDef,
-    BasePathMappingResponseMetadataTypeDef,
-    ClientCertificateResponseMetadataTypeDef,
-    DocumentationPartIdsTypeDef,
-    DocumentationVersionResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportResponseTypeDef,
-    GatewayResponseResponseMetadataTypeDef,
-    IntegrationResponseResponseMetadataTypeDef,
-    MethodResponseResponseMetadataTypeDef,
-    ModelResponseMetadataTypeDef,
-    RequestValidatorResponseMetadataTypeDef,
     SdkResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     TagsTypeDef,
     TemplateTypeDef,
+    TestInvokeAuthorizerRequestRequestTypeDef,
     TestInvokeAuthorizerResponseTypeDef,
+    TestInvokeMethodRequestRequestTypeDef,
     TestInvokeMethodResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
     UsagePlanKeyResponseMetadataTypeDef,
+    UsagePlanKeyTypeDef,
     UsageTypeDef,
     VpcLinkResponseMetadataTypeDef,
+    VpcLinkTypeDef,
     AccountTypeDef,
     ApiStageTypeDef,
     ApiKeysTypeDef,
     AuthorizersTypeDef,
     BasePathMappingsTypeDef,
     CreateStageRequestRequestTypeDef,
     ClientCertificatesTypeDef,
@@ -534,32 +552,14 @@
     CreateDomainNameRequestRequestTypeDef,
     DeploymentResponseMetadataTypeDef,
     DeploymentTypeDef,
     DocumentationVersionsTypeDef,
     DomainNameResponseMetadataTypeDef,
     DomainNameTypeDef,
     GatewayResponsesTypeDef,
-    GetApiKeysRequestGetApiKeysPaginateTypeDef,
-    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-    GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef,
-    GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef,
-    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-    GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef,
-    GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef,
-    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
-    GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef,
-    GetModelsRequestGetModelsPaginateTypeDef,
-    GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef,
-    GetResourcesRequestGetResourcesPaginateTypeDef,
-    GetRestApisRequestGetRestApisPaginateTypeDef,
-    GetSdkTypesRequestGetSdkTypesPaginateTypeDef,
-    GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef,
-    GetUsagePlansRequestGetUsagePlansPaginateTypeDef,
-    GetUsageRequestGetUsagePaginateTypeDef,
-    GetVpcLinksRequestGetVpcLinksPaginateTypeDef,
     IntegrationResponseMetadataTypeDef,
     IntegrationTypeDef,
     PutIntegrationRequestRequestTypeDef,
     StageResponseMetadataTypeDef,
     StageTypeDef,
     ModelsTypeDef,
     UpdateAccountRequestRequestTypeDef,
@@ -614,42 +614,42 @@
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

### Comparing `mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/__init__.py` & `mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/__init__.pyi` & `mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/__main__.py` & `mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.APIGateway 1.26.40\nVersion:         1.26.40\nBuilder version:"
-        " 7.12.2\nDocs:           "
+        "Type annotations for boto3.APIGateway 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.40")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/client.py` & `mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/client.pyi` & `mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/literals.py` & `mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,15 @@
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
@@ -187,31 +188,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -290,14 +294,15 @@
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
@@ -308,18 +313,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -350,14 +357,15 @@
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
@@ -376,16 +384,19 @@
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
@@ -465,18 +476,21 @@
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
@@ -525,14 +539,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/literals.pyi` & `mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,15 @@
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
@@ -185,31 +186,34 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
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
@@ -288,14 +292,15 @@
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
@@ -306,18 +311,20 @@
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
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -348,14 +355,15 @@
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
@@ -374,16 +382,19 @@
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
@@ -463,18 +474,21 @@
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
@@ -523,14 +537,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/paginator.py` & `mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -97,312 +97,292 @@
     "GetSdkTypesPaginator",
     "GetUsagePaginator",
     "GetUsagePlanKeysPaginator",
     "GetUsagePlansPaginator",
     "GetVpcLinksPaginator",
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
 class GetApiKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetApiKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getapikeyspaginator)
     """
 
     def paginate(
         self,
         *,
         nameQuery: str = ...,
         customerId: str = ...,
         includeValues: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ApiKeysTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetApiKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getapikeyspaginator)
         """
 
-
 class GetAuthorizersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetAuthorizers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getauthorizerspaginator)
     """
 
     def paginate(
-        self, *, restApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, restApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[AuthorizersTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetAuthorizers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getauthorizerspaginator)
         """
 
-
 class GetBasePathMappingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetBasePathMappings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getbasepathmappingspaginator)
     """
 
     def paginate(
-        self, *, domainName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, domainName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[BasePathMappingsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetBasePathMappings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getbasepathmappingspaginator)
         """
 
-
 class GetClientCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetClientCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getclientcertificatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClientCertificatesTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetClientCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getclientcertificatespaginator)
         """
 
-
 class GetDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdeploymentspaginator)
     """
 
     def paginate(
-        self, *, restApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, restApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DeploymentsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdeploymentspaginator)
         """
 
-
 class GetDocumentationPartsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDocumentationParts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdocumentationpartspaginator)
     """
 
     def paginate(
         self,
         *,
         restApiId: str,
         type: DocumentationPartTypeType = ...,
         nameQuery: str = ...,
         path: str = ...,
         locationStatus: LocationStatusTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DocumentationPartsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDocumentationParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdocumentationpartspaginator)
         """
 
-
 class GetDocumentationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDocumentationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdocumentationversionspaginator)
     """
 
     def paginate(
-        self, *, restApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, restApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DocumentationVersionsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDocumentationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdocumentationversionspaginator)
         """
 
-
 class GetDomainNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDomainNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdomainnamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DomainNamesTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDomainNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdomainnamespaginator)
         """
 
-
 class GetGatewayResponsesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetGatewayResponses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getgatewayresponsespaginator)
     """
 
     def paginate(
-        self, *, restApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, restApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GatewayResponsesTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetGatewayResponses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getgatewayresponsespaginator)
         """
 
-
 class GetModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getmodelspaginator)
     """
 
     def paginate(
-        self, *, restApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, restApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ModelsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getmodelspaginator)
         """
 
-
 class GetRequestValidatorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetRequestValidators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getrequestvalidatorspaginator)
     """
 
     def paginate(
-        self, *, restApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, restApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[RequestValidatorsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetRequestValidators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getrequestvalidatorspaginator)
         """
 
-
 class GetResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         restApiId: str,
         embed: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ResourcesTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getresourcespaginator)
         """
 
-
 class GetRestApisPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetRestApis)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getrestapispaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[RestApisTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetRestApis.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getrestapispaginator)
         """
 
-
 class GetSdkTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetSdkTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getsdktypespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SdkTypesTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetSdkTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getsdktypespaginator)
         """
 
-
 class GetUsagePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsage)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getusagepaginator)
     """
 
     def paginate(
         self,
         *,
         usagePlanId: str,
         startDate: str,
         endDate: str,
         keyId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[UsageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsage.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getusagepaginator)
         """
 
-
 class GetUsagePlanKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsagePlanKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getusageplankeyspaginator)
     """
 
     def paginate(
         self,
         *,
         usagePlanId: str,
         nameQuery: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[UsagePlanKeysTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsagePlanKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getusageplankeyspaginator)
         """
 
-
 class GetUsagePlansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsagePlans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getusageplanspaginator)
     """
 
     def paginate(
-        self, *, keyId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, keyId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[UsagePlansTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsagePlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getusageplanspaginator)
         """
 
-
 class GetVpcLinksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetVpcLinks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getvpclinkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[VpcLinksTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetVpcLinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getvpclinkspaginator)
         """
```

### Comparing `mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/paginator.pyi` & `mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,292 +97,312 @@
     "GetSdkTypesPaginator",
     "GetUsagePaginator",
     "GetUsagePlanKeysPaginator",
     "GetUsagePlansPaginator",
     "GetVpcLinksPaginator",
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
 class GetApiKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetApiKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getapikeyspaginator)
     """
 
     def paginate(
         self,
         *,
         nameQuery: str = ...,
         customerId: str = ...,
         includeValues: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ApiKeysTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetApiKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getapikeyspaginator)
         """
 
+
 class GetAuthorizersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetAuthorizers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getauthorizerspaginator)
     """
 
     def paginate(
-        self, *, restApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, restApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[AuthorizersTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetAuthorizers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getauthorizerspaginator)
         """
 
+
 class GetBasePathMappingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetBasePathMappings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getbasepathmappingspaginator)
     """
 
     def paginate(
-        self, *, domainName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, domainName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[BasePathMappingsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetBasePathMappings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getbasepathmappingspaginator)
         """
 
+
 class GetClientCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetClientCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getclientcertificatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ClientCertificatesTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetClientCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getclientcertificatespaginator)
         """
 
+
 class GetDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdeploymentspaginator)
     """
 
     def paginate(
-        self, *, restApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, restApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DeploymentsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdeploymentspaginator)
         """
 
+
 class GetDocumentationPartsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDocumentationParts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdocumentationpartspaginator)
     """
 
     def paginate(
         self,
         *,
         restApiId: str,
         type: DocumentationPartTypeType = ...,
         nameQuery: str = ...,
         path: str = ...,
         locationStatus: LocationStatusTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DocumentationPartsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDocumentationParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdocumentationpartspaginator)
         """
 
+
 class GetDocumentationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDocumentationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdocumentationversionspaginator)
     """
 
     def paginate(
-        self, *, restApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, restApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DocumentationVersionsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDocumentationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdocumentationversionspaginator)
         """
 
+
 class GetDomainNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDomainNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdomainnamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DomainNamesTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDomainNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getdomainnamespaginator)
         """
 
+
 class GetGatewayResponsesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetGatewayResponses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getgatewayresponsespaginator)
     """
 
     def paginate(
-        self, *, restApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, restApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GatewayResponsesTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetGatewayResponses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getgatewayresponsespaginator)
         """
 
+
 class GetModelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetModels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getmodelspaginator)
     """
 
     def paginate(
-        self, *, restApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, restApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ModelsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetModels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getmodelspaginator)
         """
 
+
 class GetRequestValidatorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetRequestValidators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getrequestvalidatorspaginator)
     """
 
     def paginate(
-        self, *, restApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, restApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[RequestValidatorsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetRequestValidators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getrequestvalidatorspaginator)
         """
 
+
 class GetResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         restApiId: str,
         embed: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ResourcesTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getresourcespaginator)
         """
 
+
 class GetRestApisPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetRestApis)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getrestapispaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[RestApisTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetRestApis.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getrestapispaginator)
         """
 
+
 class GetSdkTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetSdkTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getsdktypespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[SdkTypesTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetSdkTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getsdktypespaginator)
         """
 
+
 class GetUsagePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsage)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getusagepaginator)
     """
 
     def paginate(
         self,
         *,
         usagePlanId: str,
         startDate: str,
         endDate: str,
         keyId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[UsageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsage.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getusagepaginator)
         """
 
+
 class GetUsagePlanKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsagePlanKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getusageplankeyspaginator)
     """
 
     def paginate(
         self,
         *,
         usagePlanId: str,
         nameQuery: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[UsagePlanKeysTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsagePlanKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getusageplankeyspaginator)
         """
 
+
 class GetUsagePlansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsagePlans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getusageplanspaginator)
     """
 
     def paginate(
-        self, *, keyId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, keyId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[UsagePlansTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsagePlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getusageplanspaginator)
         """
 
+
 class GetVpcLinksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetVpcLinks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getvpclinkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[VpcLinksTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetVpcLinks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/paginators/#getvpclinkspaginator)
         """
```

### Comparing `mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/type_defs.py` & `mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,20 +46,24 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessLogSettingsTypeDef",
-    "ResponseMetadataTypeDef",
     "ThrottleSettingsTypeDef",
+    "ApiKeyIdsTypeDef",
+    "ApiKeyResponseMetadataTypeDef",
     "ApiKeyTypeDef",
+    "AuthorizerResponseMetadataTypeDef",
     "AuthorizerTypeDef",
+    "BasePathMappingResponseMetadataTypeDef",
     "BasePathMappingTypeDef",
     "CanarySettingsTypeDef",
+    "ClientCertificateResponseMetadataTypeDef",
     "ClientCertificateTypeDef",
     "StageKeyTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
     "CreateBasePathMappingRequestRequestTypeDef",
     "DeploymentCanarySettingsTypeDef",
     "DocumentationPartLocationTypeDef",
     "CreateDocumentationVersionRequestRequestTypeDef",
@@ -89,110 +93,124 @@
     "DeleteResourceRequestRequestTypeDef",
     "DeleteRestApiRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeleteUsagePlanKeyRequestRequestTypeDef",
     "DeleteUsagePlanRequestRequestTypeDef",
     "DeleteVpcLinkRequestRequestTypeDef",
     "MethodSnapshotTypeDef",
+    "DocumentationPartIdsTypeDef",
+    "DocumentationVersionResponseMetadataTypeDef",
     "DocumentationVersionTypeDef",
     "MutualTlsAuthenticationTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportResponseTypeDef",
     "FlushStageAuthorizersCacheRequestRequestTypeDef",
     "FlushStageCacheRequestRequestTypeDef",
+    "GatewayResponseResponseMetadataTypeDef",
     "GatewayResponseTypeDef",
     "GenerateClientCertificateRequestRequestTypeDef",
     "GetApiKeyRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetApiKeysRequestGetApiKeysPaginateTypeDef",
     "GetApiKeysRequestRequestTypeDef",
     "GetAuthorizerRequestRequestTypeDef",
+    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
     "GetAuthorizersRequestRequestTypeDef",
     "GetBasePathMappingRequestRequestTypeDef",
+    "GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef",
     "GetBasePathMappingsRequestRequestTypeDef",
     "GetClientCertificateRequestRequestTypeDef",
+    "GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef",
     "GetClientCertificatesRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
+    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
     "GetDeploymentsRequestRequestTypeDef",
     "GetDocumentationPartRequestRequestTypeDef",
+    "GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef",
     "GetDocumentationPartsRequestRequestTypeDef",
     "GetDocumentationVersionRequestRequestTypeDef",
+    "GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef",
     "GetDocumentationVersionsRequestRequestTypeDef",
     "GetDomainNameRequestRequestTypeDef",
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
     "GetDomainNamesRequestRequestTypeDef",
     "GetExportRequestRequestTypeDef",
     "GetGatewayResponseRequestRequestTypeDef",
+    "GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef",
     "GetGatewayResponsesRequestRequestTypeDef",
     "GetIntegrationRequestRequestTypeDef",
     "GetIntegrationResponseRequestRequestTypeDef",
     "GetMethodRequestRequestTypeDef",
     "GetMethodResponseRequestRequestTypeDef",
     "GetModelRequestRequestTypeDef",
     "GetModelTemplateRequestRequestTypeDef",
+    "GetModelsRequestGetModelsPaginateTypeDef",
     "GetModelsRequestRequestTypeDef",
     "GetRequestValidatorRequestRequestTypeDef",
+    "GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef",
     "GetRequestValidatorsRequestRequestTypeDef",
     "GetResourceRequestRequestTypeDef",
+    "GetResourcesRequestGetResourcesPaginateTypeDef",
     "GetResourcesRequestRequestTypeDef",
     "GetRestApiRequestRequestTypeDef",
+    "GetRestApisRequestGetRestApisPaginateTypeDef",
     "GetRestApisRequestRequestTypeDef",
     "GetSdkRequestRequestTypeDef",
     "GetSdkTypeRequestRequestTypeDef",
+    "GetSdkTypesRequestGetSdkTypesPaginateTypeDef",
     "GetSdkTypesRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
     "GetStagesRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
     "GetUsagePlanKeyRequestRequestTypeDef",
+    "GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef",
     "GetUsagePlanKeysRequestRequestTypeDef",
     "GetUsagePlanRequestRequestTypeDef",
+    "GetUsagePlansRequestGetUsagePlansPaginateTypeDef",
     "GetUsagePlansRequestRequestTypeDef",
+    "GetUsageRequestGetUsagePaginateTypeDef",
     "GetUsageRequestRequestTypeDef",
     "GetVpcLinkRequestRequestTypeDef",
+    "GetVpcLinksRequestGetVpcLinksPaginateTypeDef",
     "GetVpcLinksRequestRequestTypeDef",
     "ImportApiKeysRequestRequestTypeDef",
     "ImportDocumentationPartsRequestRequestTypeDef",
     "ImportRestApiRequestRequestTypeDef",
     "IntegrationResponseTypeDef",
     "TlsConfigTypeDef",
+    "IntegrationResponseResponseMetadataTypeDef",
     "MethodResponseTypeDef",
+    "MethodResponseResponseMetadataTypeDef",
     "MethodSettingTypeDef",
+    "ModelResponseMetadataTypeDef",
     "ModelTypeDef",
+    "PaginatorConfigTypeDef",
     "PatchOperationTypeDef",
     "PutGatewayResponseRequestRequestTypeDef",
     "PutIntegrationResponseRequestRequestTypeDef",
     "PutMethodRequestRequestTypeDef",
     "PutMethodResponseRequestRequestTypeDef",
     "PutRestApiRequestRequestTypeDef",
+    "RequestValidatorResponseMetadataTypeDef",
     "RequestValidatorTypeDef",
+    "ResponseMetadataTypeDef",
     "SdkConfigurationPropertyTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "TestInvokeAuthorizerRequestRequestTypeDef",
-    "TestInvokeMethodRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "UsagePlanKeyTypeDef",
-    "VpcLinkTypeDef",
-    "ApiKeyIdsTypeDef",
-    "ApiKeyResponseMetadataTypeDef",
-    "AuthorizerResponseMetadataTypeDef",
-    "BasePathMappingResponseMetadataTypeDef",
-    "ClientCertificateResponseMetadataTypeDef",
-    "DocumentationPartIdsTypeDef",
-    "DocumentationVersionResponseMetadataTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExportResponseTypeDef",
-    "GatewayResponseResponseMetadataTypeDef",
-    "IntegrationResponseResponseMetadataTypeDef",
-    "MethodResponseResponseMetadataTypeDef",
-    "ModelResponseMetadataTypeDef",
-    "RequestValidatorResponseMetadataTypeDef",
     "SdkResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "TagsTypeDef",
     "TemplateTypeDef",
+    "TestInvokeAuthorizerRequestRequestTypeDef",
     "TestInvokeAuthorizerResponseTypeDef",
+    "TestInvokeMethodRequestRequestTypeDef",
     "TestInvokeMethodResponseTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "UsagePlanKeyResponseMetadataTypeDef",
+    "UsagePlanKeyTypeDef",
     "UsageTypeDef",
     "VpcLinkResponseMetadataTypeDef",
+    "VpcLinkTypeDef",
     "AccountTypeDef",
     "ApiStageTypeDef",
     "ApiKeysTypeDef",
     "AuthorizersTypeDef",
     "BasePathMappingsTypeDef",
     "CreateStageRequestRequestTypeDef",
     "ClientCertificatesTypeDef",
@@ -207,32 +225,14 @@
     "CreateDomainNameRequestRequestTypeDef",
     "DeploymentResponseMetadataTypeDef",
     "DeploymentTypeDef",
     "DocumentationVersionsTypeDef",
     "DomainNameResponseMetadataTypeDef",
     "DomainNameTypeDef",
     "GatewayResponsesTypeDef",
-    "GetApiKeysRequestGetApiKeysPaginateTypeDef",
-    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    "GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef",
-    "GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef",
-    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    "GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef",
-    "GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef",
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
-    "GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef",
-    "GetModelsRequestGetModelsPaginateTypeDef",
-    "GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef",
-    "GetResourcesRequestGetResourcesPaginateTypeDef",
-    "GetRestApisRequestGetRestApisPaginateTypeDef",
-    "GetSdkTypesRequestGetSdkTypesPaginateTypeDef",
-    "GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef",
-    "GetUsagePlansRequestGetUsagePlansPaginateTypeDef",
-    "GetUsageRequestGetUsagePaginateTypeDef",
-    "GetVpcLinksRequestGetVpcLinksPaginateTypeDef",
     "IntegrationResponseMetadataTypeDef",
     "IntegrationTypeDef",
     "PutIntegrationRequestRequestTypeDef",
     "StageResponseMetadataTypeDef",
     "StageTypeDef",
     "ModelsTypeDef",
     "UpdateAccountRequestRequestTypeDef",
@@ -284,34 +284,49 @@
     {
         "format": str,
         "destinationArn": str,
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
 ThrottleSettingsTypeDef = TypedDict(
     "ThrottleSettingsTypeDef",
     {
         "burstLimit": int,
         "rateLimit": float,
     },
     total=False,
 )
 
+ApiKeyIdsTypeDef = TypedDict(
+    "ApiKeyIdsTypeDef",
+    {
+        "ids": List[str],
+        "warnings": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ApiKeyResponseMetadataTypeDef = TypedDict(
+    "ApiKeyResponseMetadataTypeDef",
+    {
+        "id": str,
+        "value": str,
+        "name": str,
+        "customerId": str,
+        "description": str,
+        "enabled": bool,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "stageKeys": List[str],
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ApiKeyTypeDef = TypedDict(
     "ApiKeyTypeDef",
     {
         "id": str,
         "value": str,
         "name": str,
         "customerId": str,
@@ -321,14 +336,31 @@
         "lastUpdatedDate": datetime,
         "stageKeys": List[str],
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+AuthorizerResponseMetadataTypeDef = TypedDict(
+    "AuthorizerResponseMetadataTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "type": AuthorizerTypeType,
+        "providerARNs": List[str],
+        "authType": str,
+        "authorizerUri": str,
+        "authorizerCredentials": str,
+        "identitySource": str,
+        "identityValidationExpression": str,
+        "authorizerResultTtlInSeconds": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AuthorizerTypeDef = TypedDict(
     "AuthorizerTypeDef",
     {
         "id": str,
         "name": str,
         "type": AuthorizerTypeType,
         "providerARNs": List[str],
@@ -338,14 +370,24 @@
         "identitySource": str,
         "identityValidationExpression": str,
         "authorizerResultTtlInSeconds": int,
     },
     total=False,
 )
 
+BasePathMappingResponseMetadataTypeDef = TypedDict(
+    "BasePathMappingResponseMetadataTypeDef",
+    {
+        "basePath": str,
+        "restApiId": str,
+        "stage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BasePathMappingTypeDef = TypedDict(
     "BasePathMappingTypeDef",
     {
         "basePath": str,
         "restApiId": str,
         "stage": str,
     },
@@ -359,14 +401,27 @@
         "deploymentId": str,
         "stageVariableOverrides": Mapping[str, str],
         "useStageCache": bool,
     },
     total=False,
 )
 
+ClientCertificateResponseMetadataTypeDef = TypedDict(
+    "ClientCertificateResponseMetadataTypeDef",
+    {
+        "clientCertificateId": str,
+        "description": str,
+        "pemEncodedCertificate": str,
+        "createdDate": datetime,
+        "expirationDate": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ClientCertificateTypeDef = TypedDict(
     "ClientCertificateTypeDef",
     {
         "clientCertificateId": str,
         "description": str,
         "pemEncodedCertificate": str,
         "createdDate": datetime,
@@ -786,14 +841,33 @@
     {
         "authorizationType": str,
         "apiKeyRequired": bool,
     },
     total=False,
 )
 
+DocumentationPartIdsTypeDef = TypedDict(
+    "DocumentationPartIdsTypeDef",
+    {
+        "ids": List[str],
+        "warnings": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DocumentationVersionResponseMetadataTypeDef = TypedDict(
+    "DocumentationVersionResponseMetadataTypeDef",
+    {
+        "version": str,
+        "createdDate": datetime,
+        "description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DocumentationVersionTypeDef = TypedDict(
     "DocumentationVersionTypeDef",
     {
         "version": str,
         "createdDate": datetime,
         "description": str,
     },
@@ -806,14 +880,31 @@
         "truststoreUri": str,
         "truststoreVersion": str,
         "truststoreWarnings": List[str],
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
+ExportResponseTypeDef = TypedDict(
+    "ExportResponseTypeDef",
+    {
+        "contentType": str,
+        "contentDisposition": str,
+        "body": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FlushStageAuthorizersCacheRequestRequestTypeDef = TypedDict(
     "FlushStageAuthorizersCacheRequestRequestTypeDef",
     {
         "restApiId": str,
         "stageName": str,
     },
 )
@@ -822,14 +913,26 @@
     "FlushStageCacheRequestRequestTypeDef",
     {
         "restApiId": str,
         "stageName": str,
     },
 )
 
+GatewayResponseResponseMetadataTypeDef = TypedDict(
+    "GatewayResponseResponseMetadataTypeDef",
+    {
+        "responseType": GatewayResponseTypeType,
+        "statusCode": str,
+        "responseParameters": Dict[str, str],
+        "responseTemplates": Dict[str, str],
+        "defaultResponse": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GatewayResponseTypeDef = TypedDict(
     "GatewayResponseTypeDef",
     {
         "responseType": GatewayResponseTypeType,
         "statusCode": str,
         "responseParameters": Dict[str, str],
         "responseTemplates": Dict[str, str],
@@ -864,20 +967,21 @@
 
 class GetApiKeyRequestRequestTypeDef(
     _RequiredGetApiKeyRequestRequestTypeDef, _OptionalGetApiKeyRequestRequestTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetApiKeysRequestGetApiKeysPaginateTypeDef = TypedDict(
+    "GetApiKeysRequestGetApiKeysPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "nameQuery": str,
+        "customerId": str,
+        "includeValues": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetApiKeysRequestRequestTypeDef = TypedDict(
     "GetApiKeysRequestRequestTypeDef",
     {
@@ -894,14 +998,36 @@
     "GetAuthorizerRequestRequestTypeDef",
     {
         "restApiId": str,
         "authorizerId": str,
     },
 )
 
+_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
+    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetAuthorizersRequestRequestTypeDef = TypedDict(
     "_RequiredGetAuthorizersRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetAuthorizersRequestRequestTypeDef = TypedDict(
@@ -924,14 +1050,36 @@
     "GetBasePathMappingRequestRequestTypeDef",
     {
         "domainName": str,
         "basePath": str,
     },
 )
 
+_RequiredGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef = TypedDict(
+    "_RequiredGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef",
+    {
+        "domainName": str,
+    },
+)
+_OptionalGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef = TypedDict(
+    "_OptionalGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef(
+    _RequiredGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef,
+    _OptionalGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetBasePathMappingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBasePathMappingsRequestRequestTypeDef",
     {
         "domainName": str,
     },
 )
 _OptionalGetBasePathMappingsRequestRequestTypeDef = TypedDict(
@@ -954,14 +1102,22 @@
 GetClientCertificateRequestRequestTypeDef = TypedDict(
     "GetClientCertificateRequestRequestTypeDef",
     {
         "clientCertificateId": str,
     },
 )
 
+GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef = TypedDict(
+    "GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetClientCertificatesRequestRequestTypeDef = TypedDict(
     "GetClientCertificatesRequestRequestTypeDef",
     {
         "position": str,
         "limit": int,
     },
     total=False,
@@ -985,14 +1141,36 @@
 
 class GetDeploymentRequestRequestTypeDef(
     _RequiredGetDeploymentRequestRequestTypeDef, _OptionalGetDeploymentRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
+    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeploymentsRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetDeploymentsRequestRequestTypeDef = TypedDict(
@@ -1015,14 +1193,40 @@
     "GetDocumentationPartRequestRequestTypeDef",
     {
         "restApiId": str,
         "documentationPartId": str,
     },
 )
 
+_RequiredGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef = TypedDict(
+    "_RequiredGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef = TypedDict(
+    "_OptionalGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef",
+    {
+        "type": DocumentationPartTypeType,
+        "nameQuery": str,
+        "path": str,
+        "locationStatus": LocationStatusTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef(
+    _RequiredGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef,
+    _OptionalGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetDocumentationPartsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDocumentationPartsRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetDocumentationPartsRequestRequestTypeDef = TypedDict(
@@ -1050,14 +1254,36 @@
     "GetDocumentationVersionRequestRequestTypeDef",
     {
         "restApiId": str,
         "documentationVersion": str,
     },
 )
 
+_RequiredGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef(
+    _RequiredGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef,
+    _OptionalGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetDocumentationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDocumentationVersionsRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetDocumentationVersionsRequestRequestTypeDef = TypedDict(
@@ -1080,14 +1306,22 @@
 GetDomainNameRequestRequestTypeDef = TypedDict(
     "GetDomainNameRequestRequestTypeDef",
     {
         "domainName": str,
     },
 )
 
+GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetDomainNamesRequestRequestTypeDef = TypedDict(
     "GetDomainNamesRequestRequestTypeDef",
     {
         "position": str,
         "limit": int,
     },
     total=False,
@@ -1121,14 +1355,36 @@
     "GetGatewayResponseRequestRequestTypeDef",
     {
         "restApiId": str,
         "responseType": GatewayResponseTypeType,
     },
 )
 
+_RequiredGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef = TypedDict(
+    "_RequiredGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef = TypedDict(
+    "_OptionalGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef(
+    _RequiredGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef,
+    _OptionalGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetGatewayResponsesRequestRequestTypeDef = TypedDict(
     "_RequiredGetGatewayResponsesRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetGatewayResponsesRequestRequestTypeDef = TypedDict(
@@ -1212,14 +1468,36 @@
     "GetModelTemplateRequestRequestTypeDef",
     {
         "restApiId": str,
         "modelName": str,
     },
 )
 
+_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetModelsRequestGetModelsPaginateTypeDef(
+    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
+    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetModelsRequestRequestTypeDef = TypedDict(
     "_RequiredGetModelsRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetModelsRequestRequestTypeDef = TypedDict(
@@ -1242,14 +1520,36 @@
     "GetRequestValidatorRequestRequestTypeDef",
     {
         "restApiId": str,
         "requestValidatorId": str,
     },
 )
 
+_RequiredGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef = TypedDict(
+    "_RequiredGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef = TypedDict(
+    "_OptionalGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef(
+    _RequiredGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef,
+    _OptionalGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetRequestValidatorsRequestRequestTypeDef = TypedDict(
     "_RequiredGetRequestValidatorsRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetRequestValidatorsRequestRequestTypeDef = TypedDict(
@@ -1287,14 +1587,37 @@
 
 class GetResourceRequestRequestTypeDef(
     _RequiredGetResourceRequestRequestTypeDef, _OptionalGetResourceRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredGetResourcesRequestGetResourcesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcesRequestGetResourcesPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetResourcesRequestGetResourcesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcesRequestGetResourcesPaginateTypeDef",
+    {
+        "embed": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetResourcesRequestGetResourcesPaginateTypeDef(
+    _RequiredGetResourcesRequestGetResourcesPaginateTypeDef,
+    _OptionalGetResourcesRequestGetResourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcesRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetResourcesRequestRequestTypeDef = TypedDict(
@@ -1317,14 +1640,22 @@
 GetRestApiRequestRequestTypeDef = TypedDict(
     "GetRestApiRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 
+GetRestApisRequestGetRestApisPaginateTypeDef = TypedDict(
+    "GetRestApisRequestGetRestApisPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetRestApisRequestRequestTypeDef = TypedDict(
     "GetRestApisRequestRequestTypeDef",
     {
         "position": str,
         "limit": int,
     },
     total=False,
@@ -1356,14 +1687,22 @@
 GetSdkTypeRequestRequestTypeDef = TypedDict(
     "GetSdkTypeRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+GetSdkTypesRequestGetSdkTypesPaginateTypeDef = TypedDict(
+    "GetSdkTypesRequestGetSdkTypesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetSdkTypesRequestRequestTypeDef = TypedDict(
     "GetSdkTypesRequestRequestTypeDef",
     {
         "position": str,
         "limit": int,
     },
     total=False,
@@ -1424,14 +1763,37 @@
     "GetUsagePlanKeyRequestRequestTypeDef",
     {
         "usagePlanId": str,
         "keyId": str,
     },
 )
 
+_RequiredGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef = TypedDict(
+    "_RequiredGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef",
+    {
+        "usagePlanId": str,
+    },
+)
+_OptionalGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef = TypedDict(
+    "_OptionalGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef",
+    {
+        "nameQuery": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef(
+    _RequiredGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef,
+    _OptionalGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetUsagePlanKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetUsagePlanKeysRequestRequestTypeDef",
     {
         "usagePlanId": str,
     },
 )
 _OptionalGetUsagePlanKeysRequestRequestTypeDef = TypedDict(
@@ -1454,24 +1816,57 @@
 GetUsagePlanRequestRequestTypeDef = TypedDict(
     "GetUsagePlanRequestRequestTypeDef",
     {
         "usagePlanId": str,
     },
 )
 
+GetUsagePlansRequestGetUsagePlansPaginateTypeDef = TypedDict(
+    "GetUsagePlansRequestGetUsagePlansPaginateTypeDef",
+    {
+        "keyId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetUsagePlansRequestRequestTypeDef = TypedDict(
     "GetUsagePlansRequestRequestTypeDef",
     {
         "position": str,
         "keyId": str,
         "limit": int,
     },
     total=False,
 )
 
+_RequiredGetUsageRequestGetUsagePaginateTypeDef = TypedDict(
+    "_RequiredGetUsageRequestGetUsagePaginateTypeDef",
+    {
+        "usagePlanId": str,
+        "startDate": str,
+        "endDate": str,
+    },
+)
+_OptionalGetUsageRequestGetUsagePaginateTypeDef = TypedDict(
+    "_OptionalGetUsageRequestGetUsagePaginateTypeDef",
+    {
+        "keyId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetUsageRequestGetUsagePaginateTypeDef(
+    _RequiredGetUsageRequestGetUsagePaginateTypeDef, _OptionalGetUsageRequestGetUsagePaginateTypeDef
+):
+    pass
+
+
 _RequiredGetUsageRequestRequestTypeDef = TypedDict(
     "_RequiredGetUsageRequestRequestTypeDef",
     {
         "usagePlanId": str,
         "startDate": str,
         "endDate": str,
     },
@@ -1496,14 +1891,22 @@
 GetVpcLinkRequestRequestTypeDef = TypedDict(
     "GetVpcLinkRequestRequestTypeDef",
     {
         "vpcLinkId": str,
     },
 )
 
+GetVpcLinksRequestGetVpcLinksPaginateTypeDef = TypedDict(
+    "GetVpcLinksRequestGetVpcLinksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetVpcLinksRequestRequestTypeDef = TypedDict(
     "GetVpcLinksRequestRequestTypeDef",
     {
         "position": str,
         "limit": int,
     },
     total=False,
@@ -1593,24 +1996,46 @@
     "TlsConfigTypeDef",
     {
         "insecureSkipVerification": bool,
     },
     total=False,
 )
 
+IntegrationResponseResponseMetadataTypeDef = TypedDict(
+    "IntegrationResponseResponseMetadataTypeDef",
+    {
+        "statusCode": str,
+        "selectionPattern": str,
+        "responseParameters": Dict[str, str],
+        "responseTemplates": Dict[str, str],
+        "contentHandling": ContentHandlingStrategyType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MethodResponseTypeDef = TypedDict(
     "MethodResponseTypeDef",
     {
         "statusCode": str,
         "responseParameters": Dict[str, bool],
         "responseModels": Dict[str, str],
     },
     total=False,
 )
 
+MethodResponseResponseMetadataTypeDef = TypedDict(
+    "MethodResponseResponseMetadataTypeDef",
+    {
+        "statusCode": str,
+        "responseParameters": Dict[str, bool],
+        "responseModels": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MethodSettingTypeDef = TypedDict(
     "MethodSettingTypeDef",
     {
         "metricsEnabled": bool,
         "loggingLevel": str,
         "dataTraceEnabled": bool,
         "throttlingBurstLimit": int,
@@ -1620,26 +2045,48 @@
         "cacheDataEncrypted": bool,
         "requireAuthorizationForCacheControl": bool,
         "unauthorizedCacheControlHeaderStrategy": UnauthorizedCacheControlHeaderStrategyType,
     },
     total=False,
 )
 
+ModelResponseMetadataTypeDef = TypedDict(
+    "ModelResponseMetadataTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "description": str,
+        "schema": str,
+        "contentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ModelTypeDef = TypedDict(
     "ModelTypeDef",
     {
         "id": str,
         "name": str,
         "description": str,
         "schema": str,
         "contentType": str,
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
 PatchOperationTypeDef = TypedDict(
     "PatchOperationTypeDef",
     {
         "op": OpType,
         "path": str,
         "value": str,
         "from": str,
@@ -1775,45 +2222,93 @@
 
 class PutRestApiRequestRequestTypeDef(
     _RequiredPutRestApiRequestRequestTypeDef, _OptionalPutRestApiRequestRequestTypeDef
 ):
     pass
 
 
+RequestValidatorResponseMetadataTypeDef = TypedDict(
+    "RequestValidatorResponseMetadataTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "validateRequestBody": bool,
+        "validateRequestParameters": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RequestValidatorTypeDef = TypedDict(
     "RequestValidatorTypeDef",
     {
         "id": str,
         "name": str,
         "validateRequestBody": bool,
         "validateRequestParameters": bool,
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
 SdkConfigurationPropertyTypeDef = TypedDict(
     "SdkConfigurationPropertyTypeDef",
     {
         "name": str,
         "friendlyName": str,
         "description": str,
         "required": bool,
         "defaultValue": str,
     },
     total=False,
 )
 
+SdkResponseTypeDef = TypedDict(
+    "SdkResponseTypeDef",
+    {
+        "contentType": str,
+        "contentDisposition": str,
+        "body": StreamingBody,
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
 
+TagsTypeDef = TypedDict(
+    "TagsTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TemplateTypeDef = TypedDict(
+    "TemplateTypeDef",
+    {
+        "value": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredTestInvokeAuthorizerRequestRequestTypeDef",
     {
         "restApiId": str,
         "authorizerId": str,
     },
 )
@@ -1834,14 +2329,28 @@
 class TestInvokeAuthorizerRequestRequestTypeDef(
     _RequiredTestInvokeAuthorizerRequestRequestTypeDef,
     _OptionalTestInvokeAuthorizerRequestRequestTypeDef,
 ):
     pass
 
 
+TestInvokeAuthorizerResponseTypeDef = TypedDict(
+    "TestInvokeAuthorizerResponseTypeDef",
+    {
+        "clientStatus": int,
+        "log": str,
+        "latency": int,
+        "principalId": str,
+        "policy": str,
+        "authorization": Dict[str, List[str]],
+        "claims": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredTestInvokeMethodRequestRequestTypeDef = TypedDict(
     "_RequiredTestInvokeMethodRequestRequestTypeDef",
     {
         "restApiId": str,
         "resourceId": str,
         "httpMethod": str,
     },
@@ -1862,304 +2371,105 @@
 
 class TestInvokeMethodRequestRequestTypeDef(
     _RequiredTestInvokeMethodRequestRequestTypeDef, _OptionalTestInvokeMethodRequestRequestTypeDef
 ):
     pass
 
 
+TestInvokeMethodResponseTypeDef = TypedDict(
+    "TestInvokeMethodResponseTypeDef",
+    {
+        "status": int,
+        "body": str,
+        "headers": Dict[str, str],
+        "multiValueHeaders": Dict[str, List[str]],
+        "log": str,
+        "latency": int,
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
 
-UsagePlanKeyTypeDef = TypedDict(
-    "UsagePlanKeyTypeDef",
+UsagePlanKeyResponseMetadataTypeDef = TypedDict(
+    "UsagePlanKeyResponseMetadataTypeDef",
     {
         "id": str,
         "type": str,
         "value": str,
         "name": str,
-    },
-    total=False,
-)
-
-VpcLinkTypeDef = TypedDict(
-    "VpcLinkTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "description": str,
-        "targetArns": List[str],
-        "status": VpcLinkStatusType,
-        "statusMessage": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-ApiKeyIdsTypeDef = TypedDict(
-    "ApiKeyIdsTypeDef",
-    {
-        "ids": List[str],
-        "warnings": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ApiKeyResponseMetadataTypeDef = TypedDict(
-    "ApiKeyResponseMetadataTypeDef",
-    {
-        "id": str,
-        "value": str,
-        "name": str,
-        "customerId": str,
-        "description": str,
-        "enabled": bool,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "stageKeys": List[str],
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AuthorizerResponseMetadataTypeDef = TypedDict(
-    "AuthorizerResponseMetadataTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "type": AuthorizerTypeType,
-        "providerARNs": List[str],
-        "authType": str,
-        "authorizerUri": str,
-        "authorizerCredentials": str,
-        "identitySource": str,
-        "identityValidationExpression": str,
-        "authorizerResultTtlInSeconds": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BasePathMappingResponseMetadataTypeDef = TypedDict(
-    "BasePathMappingResponseMetadataTypeDef",
-    {
-        "basePath": str,
-        "restApiId": str,
-        "stage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ClientCertificateResponseMetadataTypeDef = TypedDict(
-    "ClientCertificateResponseMetadataTypeDef",
-    {
-        "clientCertificateId": str,
-        "description": str,
-        "pemEncodedCertificate": str,
-        "createdDate": datetime,
-        "expirationDate": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DocumentationPartIdsTypeDef = TypedDict(
-    "DocumentationPartIdsTypeDef",
-    {
-        "ids": List[str],
-        "warnings": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DocumentationVersionResponseMetadataTypeDef = TypedDict(
-    "DocumentationVersionResponseMetadataTypeDef",
-    {
-        "version": str,
-        "createdDate": datetime,
-        "description": str,
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
-ExportResponseTypeDef = TypedDict(
-    "ExportResponseTypeDef",
-    {
-        "contentType": str,
-        "contentDisposition": str,
-        "body": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GatewayResponseResponseMetadataTypeDef = TypedDict(
-    "GatewayResponseResponseMetadataTypeDef",
-    {
-        "responseType": GatewayResponseTypeType,
-        "statusCode": str,
-        "responseParameters": Dict[str, str],
-        "responseTemplates": Dict[str, str],
-        "defaultResponse": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-IntegrationResponseResponseMetadataTypeDef = TypedDict(
-    "IntegrationResponseResponseMetadataTypeDef",
-    {
-        "statusCode": str,
-        "selectionPattern": str,
-        "responseParameters": Dict[str, str],
-        "responseTemplates": Dict[str, str],
-        "contentHandling": ContentHandlingStrategyType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MethodResponseResponseMetadataTypeDef = TypedDict(
-    "MethodResponseResponseMetadataTypeDef",
-    {
-        "statusCode": str,
-        "responseParameters": Dict[str, bool],
-        "responseModels": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModelResponseMetadataTypeDef = TypedDict(
-    "ModelResponseMetadataTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "description": str,
-        "schema": str,
-        "contentType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RequestValidatorResponseMetadataTypeDef = TypedDict(
-    "RequestValidatorResponseMetadataTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "validateRequestBody": bool,
-        "validateRequestParameters": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SdkResponseTypeDef = TypedDict(
-    "SdkResponseTypeDef",
-    {
-        "contentType": str,
-        "contentDisposition": str,
-        "body": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagsTypeDef = TypedDict(
-    "TagsTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TemplateTypeDef = TypedDict(
-    "TemplateTypeDef",
-    {
-        "value": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TestInvokeAuthorizerResponseTypeDef = TypedDict(
-    "TestInvokeAuthorizerResponseTypeDef",
-    {
-        "clientStatus": int,
-        "log": str,
-        "latency": int,
-        "principalId": str,
-        "policy": str,
-        "authorization": Dict[str, List[str]],
-        "claims": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TestInvokeMethodResponseTypeDef = TypedDict(
-    "TestInvokeMethodResponseTypeDef",
-    {
-        "status": int,
-        "body": str,
-        "headers": Dict[str, str],
-        "multiValueHeaders": Dict[str, List[str]],
-        "log": str,
-        "latency": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UsagePlanKeyResponseMetadataTypeDef = TypedDict(
-    "UsagePlanKeyResponseMetadataTypeDef",
+UsagePlanKeyTypeDef = TypedDict(
+    "UsagePlanKeyTypeDef",
     {
         "id": str,
         "type": str,
         "value": str,
         "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
 UsageTypeDef = TypedDict(
     "UsageTypeDef",
     {
         "usagePlanId": str,
         "startDate": str,
         "endDate": str,
         "position": str,
         "items": Dict[str, List[List[int]]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VpcLinkResponseMetadataTypeDef = TypedDict(
     "VpcLinkResponseMetadataTypeDef",
     {
         "id": str,
         "name": str,
         "description": str,
         "targetArns": List[str],
         "status": VpcLinkStatusType,
         "statusMessage": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+VpcLinkTypeDef = TypedDict(
+    "VpcLinkTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "description": str,
+        "targetArns": List[str],
+        "status": VpcLinkStatusType,
+        "statusMessage": str,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
 AccountTypeDef = TypedDict(
     "AccountTypeDef",
     {
         "cloudwatchRoleArn": str,
         "throttleSettings": ThrottleSettingsTypeDef,
         "features": List[str],
         "apiKeyVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApiStageTypeDef = TypedDict(
     "ApiStageTypeDef",
     {
         "apiId": str,
@@ -2171,33 +2481,33 @@
 
 ApiKeysTypeDef = TypedDict(
     "ApiKeysTypeDef",
     {
         "warnings": List[str],
         "position": str,
         "items": List[ApiKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AuthorizersTypeDef = TypedDict(
     "AuthorizersTypeDef",
     {
         "position": str,
         "items": List[AuthorizerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BasePathMappingsTypeDef = TypedDict(
     "BasePathMappingsTypeDef",
     {
         "position": str,
         "items": List[BasePathMappingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateStageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStageRequestRequestTypeDef",
     {
         "restApiId": str,
@@ -2228,15 +2538,15 @@
 
 
 ClientCertificatesTypeDef = TypedDict(
     "ClientCertificatesTypeDef",
     {
         "position": str,
         "items": List[ClientCertificateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateApiKeyRequestRequestTypeDef = TypedDict(
     "CreateApiKeyRequestRequestTypeDef",
     {
         "name": str,
@@ -2290,15 +2600,15 @@
 
 DocumentationPartResponseMetadataTypeDef = TypedDict(
     "DocumentationPartResponseMetadataTypeDef",
     {
         "id": str,
         "location": DocumentationPartLocationTypeDef,
         "properties": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DocumentationPartTypeDef = TypedDict(
     "DocumentationPartTypeDef",
     {
         "id": str,
@@ -2350,15 +2660,15 @@
         "binaryMediaTypes": List[str],
         "minimumCompressionSize": int,
         "apiKeySource": ApiKeySourceTypeType,
         "endpointConfiguration": EndpointConfigurationTypeDef,
         "policy": str,
         "tags": Dict[str, str],
         "disableExecuteApiEndpoint": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestApiTypeDef = TypedDict(
     "RestApiTypeDef",
     {
         "id": str,
@@ -2413,15 +2723,15 @@
 DeploymentResponseMetadataTypeDef = TypedDict(
     "DeploymentResponseMetadataTypeDef",
     {
         "id": str,
         "description": str,
         "createdDate": datetime,
         "apiSummary": Dict[str, Dict[str, MethodSnapshotTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "id": str,
@@ -2433,15 +2743,15 @@
 )
 
 DocumentationVersionsTypeDef = TypedDict(
     "DocumentationVersionsTypeDef",
     {
         "position": str,
         "items": List[DocumentationVersionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainNameResponseMetadataTypeDef = TypedDict(
     "DomainNameResponseMetadataTypeDef",
     {
         "domainName": str,
@@ -2457,15 +2767,15 @@
         "endpointConfiguration": EndpointConfigurationTypeDef,
         "domainNameStatus": DomainNameStatusType,
         "domainNameStatusMessage": str,
         "securityPolicy": SecurityPolicyType,
         "tags": Dict[str, str],
         "mutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "ownershipVerificationCertificateArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainNameTypeDef = TypedDict(
     "DomainNameTypeDef",
     {
         "domainName": str,
@@ -2490,327 +2800,17 @@
 )
 
 GatewayResponsesTypeDef = TypedDict(
     "GatewayResponsesTypeDef",
     {
         "position": str,
         "items": List[GatewayResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetApiKeysRequestGetApiKeysPaginateTypeDef = TypedDict(
-    "GetApiKeysRequestGetApiKeysPaginateTypeDef",
-    {
-        "nameQuery": str,
-        "customerId": str,
-        "includeValues": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
-    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef = TypedDict(
-    "_RequiredGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef",
-    {
-        "domainName": str,
-    },
-)
-_OptionalGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef = TypedDict(
-    "_OptionalGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef(
-    _RequiredGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef,
-    _OptionalGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef,
-):
-    pass
-
-
-GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef = TypedDict(
-    "GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
-    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef = TypedDict(
-    "_RequiredGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef = TypedDict(
-    "_OptionalGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef",
-    {
-        "type": DocumentationPartTypeType,
-        "nameQuery": str,
-        "path": str,
-        "locationStatus": LocationStatusTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef(
-    _RequiredGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef,
-    _OptionalGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef(
-    _RequiredGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef,
-    _OptionalGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef,
-):
-    pass
-
-
-GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef = TypedDict(
-    "_RequiredGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef = TypedDict(
-    "_OptionalGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef(
-    _RequiredGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef,
-    _OptionalGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetModelsRequestGetModelsPaginateTypeDef(
-    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
-    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef = TypedDict(
-    "_RequiredGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef = TypedDict(
-    "_OptionalGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef(
-    _RequiredGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef,
-    _OptionalGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetResourcesRequestGetResourcesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcesRequestGetResourcesPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetResourcesRequestGetResourcesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcesRequestGetResourcesPaginateTypeDef",
-    {
-        "embed": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetResourcesRequestGetResourcesPaginateTypeDef(
-    _RequiredGetResourcesRequestGetResourcesPaginateTypeDef,
-    _OptionalGetResourcesRequestGetResourcesPaginateTypeDef,
-):
-    pass
-
-
-GetRestApisRequestGetRestApisPaginateTypeDef = TypedDict(
-    "GetRestApisRequestGetRestApisPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetSdkTypesRequestGetSdkTypesPaginateTypeDef = TypedDict(
-    "GetSdkTypesRequestGetSdkTypesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef = TypedDict(
-    "_RequiredGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef",
-    {
-        "usagePlanId": str,
-    },
-)
-_OptionalGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef = TypedDict(
-    "_OptionalGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef",
-    {
-        "nameQuery": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef(
-    _RequiredGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef,
-    _OptionalGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef,
-):
-    pass
-
-
-GetUsagePlansRequestGetUsagePlansPaginateTypeDef = TypedDict(
-    "GetUsagePlansRequestGetUsagePlansPaginateTypeDef",
-    {
-        "keyId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetUsageRequestGetUsagePaginateTypeDef = TypedDict(
-    "_RequiredGetUsageRequestGetUsagePaginateTypeDef",
-    {
-        "usagePlanId": str,
-        "startDate": str,
-        "endDate": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalGetUsageRequestGetUsagePaginateTypeDef = TypedDict(
-    "_OptionalGetUsageRequestGetUsagePaginateTypeDef",
-    {
-        "keyId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetUsageRequestGetUsagePaginateTypeDef(
-    _RequiredGetUsageRequestGetUsagePaginateTypeDef, _OptionalGetUsageRequestGetUsagePaginateTypeDef
-):
-    pass
-
-
-GetVpcLinksRequestGetVpcLinksPaginateTypeDef = TypedDict(
-    "GetVpcLinksRequestGetVpcLinksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
 IntegrationResponseMetadataTypeDef = TypedDict(
     "IntegrationResponseMetadataTypeDef",
     {
         "type": IntegrationTypeType,
         "httpMethod": str,
         "uri": str,
@@ -2822,15 +2822,15 @@
         "passthroughBehavior": str,
         "contentHandling": ContentHandlingStrategyType,
         "timeoutInMillis": int,
         "cacheNamespace": str,
         "cacheKeyParameters": List[str],
         "integrationResponses": Dict[str, IntegrationResponseTypeDef],
         "tlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IntegrationTypeDef = TypedDict(
     "IntegrationTypeDef",
     {
         "type": IntegrationTypeType,
@@ -2904,15 +2904,15 @@
         "accessLogSettings": AccessLogSettingsTypeDef,
         "canarySettings": CanarySettingsTypeDef,
         "tracingEnabled": bool,
         "webAclArn": str,
         "tags": Dict[str, str],
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StageTypeDef = TypedDict(
     "StageTypeDef",
     {
         "deploymentId": str,
@@ -2937,15 +2937,15 @@
 )
 
 ModelsTypeDef = TypedDict(
     "ModelsTypeDef",
     {
         "position": str,
         "items": List[ModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAccountRequestRequestTypeDef = TypedDict(
     "UpdateAccountRequestRequestTypeDef",
     {
         "patchOperations": Sequence[PatchOperationTypeDef],
@@ -3424,26 +3424,26 @@
 
 
 RequestValidatorsTypeDef = TypedDict(
     "RequestValidatorsTypeDef",
     {
         "position": str,
         "items": List[RequestValidatorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SdkTypeResponseMetadataTypeDef = TypedDict(
     "SdkTypeResponseMetadataTypeDef",
     {
         "id": str,
         "friendlyName": str,
         "description": str,
         "configurationProperties": List[SdkConfigurationPropertyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SdkTypeTypeDef = TypedDict(
     "SdkTypeTypeDef",
     {
         "id": str,
@@ -3455,24 +3455,24 @@
 )
 
 UsagePlanKeysTypeDef = TypedDict(
     "UsagePlanKeysTypeDef",
     {
         "position": str,
         "items": List[UsagePlanKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VpcLinksTypeDef = TypedDict(
     "VpcLinksTypeDef",
     {
         "position": str,
         "items": List[VpcLinkTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateUsagePlanRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUsagePlanRequestRequestTypeDef",
     {
         "name": str,
@@ -3504,15 +3504,15 @@
         "name": str,
         "description": str,
         "apiStages": List[ApiStageTypeDef],
         "throttle": ThrottleSettingsTypeDef,
         "quota": QuotaSettingsTypeDef,
         "productCode": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UsagePlanTypeDef = TypedDict(
     "UsagePlanTypeDef",
     {
         "id": str,
@@ -3528,42 +3528,42 @@
 )
 
 DocumentationPartsTypeDef = TypedDict(
     "DocumentationPartsTypeDef",
     {
         "position": str,
         "items": List[DocumentationPartTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestApisTypeDef = TypedDict(
     "RestApisTypeDef",
     {
         "position": str,
         "items": List[RestApiTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentsTypeDef = TypedDict(
     "DeploymentsTypeDef",
     {
         "position": str,
         "items": List[DeploymentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainNamesTypeDef = TypedDict(
     "DomainNamesTypeDef",
     {
         "position": str,
         "items": List[DomainNameTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MethodResponseMetadataTypeDef = TypedDict(
     "MethodResponseMetadataTypeDef",
     {
         "httpMethod": str,
@@ -3573,15 +3573,15 @@
         "requestValidatorId": str,
         "operationName": str,
         "requestParameters": Dict[str, bool],
         "requestModels": Dict[str, str],
         "methodResponses": Dict[str, MethodResponseTypeDef],
         "methodIntegration": IntegrationTypeDef,
         "authorizationScopes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MethodTypeDef = TypedDict(
     "MethodTypeDef",
     {
         "httpMethod": str,
@@ -3599,45 +3599,45 @@
     total=False,
 )
 
 StagesTypeDef = TypedDict(
     "StagesTypeDef",
     {
         "item": List[StageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SdkTypesTypeDef = TypedDict(
     "SdkTypesTypeDef",
     {
         "position": str,
         "items": List[SdkTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UsagePlansTypeDef = TypedDict(
     "UsagePlansTypeDef",
     {
         "position": str,
         "items": List[UsagePlanTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceResponseMetadataTypeDef = TypedDict(
     "ResourceResponseMetadataTypeDef",
     {
         "id": str,
         "parentId": str,
         "pathPart": str,
         "path": str,
         "resourceMethods": Dict[str, MethodTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "id": str,
@@ -3650,10 +3650,10 @@
 )
 
 ResourcesTypeDef = TypedDict(
     "ResourcesTypeDef",
     {
         "position": str,
         "items": List[ResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway/type_defs.pyi` & `mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,20 +45,24 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessLogSettingsTypeDef",
-    "ResponseMetadataTypeDef",
     "ThrottleSettingsTypeDef",
+    "ApiKeyIdsTypeDef",
+    "ApiKeyResponseMetadataTypeDef",
     "ApiKeyTypeDef",
+    "AuthorizerResponseMetadataTypeDef",
     "AuthorizerTypeDef",
+    "BasePathMappingResponseMetadataTypeDef",
     "BasePathMappingTypeDef",
     "CanarySettingsTypeDef",
+    "ClientCertificateResponseMetadataTypeDef",
     "ClientCertificateTypeDef",
     "StageKeyTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
     "CreateBasePathMappingRequestRequestTypeDef",
     "DeploymentCanarySettingsTypeDef",
     "DocumentationPartLocationTypeDef",
     "CreateDocumentationVersionRequestRequestTypeDef",
@@ -88,110 +92,124 @@
     "DeleteResourceRequestRequestTypeDef",
     "DeleteRestApiRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeleteUsagePlanKeyRequestRequestTypeDef",
     "DeleteUsagePlanRequestRequestTypeDef",
     "DeleteVpcLinkRequestRequestTypeDef",
     "MethodSnapshotTypeDef",
+    "DocumentationPartIdsTypeDef",
+    "DocumentationVersionResponseMetadataTypeDef",
     "DocumentationVersionTypeDef",
     "MutualTlsAuthenticationTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportResponseTypeDef",
     "FlushStageAuthorizersCacheRequestRequestTypeDef",
     "FlushStageCacheRequestRequestTypeDef",
+    "GatewayResponseResponseMetadataTypeDef",
     "GatewayResponseTypeDef",
     "GenerateClientCertificateRequestRequestTypeDef",
     "GetApiKeyRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetApiKeysRequestGetApiKeysPaginateTypeDef",
     "GetApiKeysRequestRequestTypeDef",
     "GetAuthorizerRequestRequestTypeDef",
+    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
     "GetAuthorizersRequestRequestTypeDef",
     "GetBasePathMappingRequestRequestTypeDef",
+    "GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef",
     "GetBasePathMappingsRequestRequestTypeDef",
     "GetClientCertificateRequestRequestTypeDef",
+    "GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef",
     "GetClientCertificatesRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
+    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
     "GetDeploymentsRequestRequestTypeDef",
     "GetDocumentationPartRequestRequestTypeDef",
+    "GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef",
     "GetDocumentationPartsRequestRequestTypeDef",
     "GetDocumentationVersionRequestRequestTypeDef",
+    "GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef",
     "GetDocumentationVersionsRequestRequestTypeDef",
     "GetDomainNameRequestRequestTypeDef",
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
     "GetDomainNamesRequestRequestTypeDef",
     "GetExportRequestRequestTypeDef",
     "GetGatewayResponseRequestRequestTypeDef",
+    "GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef",
     "GetGatewayResponsesRequestRequestTypeDef",
     "GetIntegrationRequestRequestTypeDef",
     "GetIntegrationResponseRequestRequestTypeDef",
     "GetMethodRequestRequestTypeDef",
     "GetMethodResponseRequestRequestTypeDef",
     "GetModelRequestRequestTypeDef",
     "GetModelTemplateRequestRequestTypeDef",
+    "GetModelsRequestGetModelsPaginateTypeDef",
     "GetModelsRequestRequestTypeDef",
     "GetRequestValidatorRequestRequestTypeDef",
+    "GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef",
     "GetRequestValidatorsRequestRequestTypeDef",
     "GetResourceRequestRequestTypeDef",
+    "GetResourcesRequestGetResourcesPaginateTypeDef",
     "GetResourcesRequestRequestTypeDef",
     "GetRestApiRequestRequestTypeDef",
+    "GetRestApisRequestGetRestApisPaginateTypeDef",
     "GetRestApisRequestRequestTypeDef",
     "GetSdkRequestRequestTypeDef",
     "GetSdkTypeRequestRequestTypeDef",
+    "GetSdkTypesRequestGetSdkTypesPaginateTypeDef",
     "GetSdkTypesRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
     "GetStagesRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
     "GetUsagePlanKeyRequestRequestTypeDef",
+    "GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef",
     "GetUsagePlanKeysRequestRequestTypeDef",
     "GetUsagePlanRequestRequestTypeDef",
+    "GetUsagePlansRequestGetUsagePlansPaginateTypeDef",
     "GetUsagePlansRequestRequestTypeDef",
+    "GetUsageRequestGetUsagePaginateTypeDef",
     "GetUsageRequestRequestTypeDef",
     "GetVpcLinkRequestRequestTypeDef",
+    "GetVpcLinksRequestGetVpcLinksPaginateTypeDef",
     "GetVpcLinksRequestRequestTypeDef",
     "ImportApiKeysRequestRequestTypeDef",
     "ImportDocumentationPartsRequestRequestTypeDef",
     "ImportRestApiRequestRequestTypeDef",
     "IntegrationResponseTypeDef",
     "TlsConfigTypeDef",
+    "IntegrationResponseResponseMetadataTypeDef",
     "MethodResponseTypeDef",
+    "MethodResponseResponseMetadataTypeDef",
     "MethodSettingTypeDef",
+    "ModelResponseMetadataTypeDef",
     "ModelTypeDef",
+    "PaginatorConfigTypeDef",
     "PatchOperationTypeDef",
     "PutGatewayResponseRequestRequestTypeDef",
     "PutIntegrationResponseRequestRequestTypeDef",
     "PutMethodRequestRequestTypeDef",
     "PutMethodResponseRequestRequestTypeDef",
     "PutRestApiRequestRequestTypeDef",
+    "RequestValidatorResponseMetadataTypeDef",
     "RequestValidatorTypeDef",
+    "ResponseMetadataTypeDef",
     "SdkConfigurationPropertyTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "TestInvokeAuthorizerRequestRequestTypeDef",
-    "TestInvokeMethodRequestRequestTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "UsagePlanKeyTypeDef",
-    "VpcLinkTypeDef",
-    "ApiKeyIdsTypeDef",
-    "ApiKeyResponseMetadataTypeDef",
-    "AuthorizerResponseMetadataTypeDef",
-    "BasePathMappingResponseMetadataTypeDef",
-    "ClientCertificateResponseMetadataTypeDef",
-    "DocumentationPartIdsTypeDef",
-    "DocumentationVersionResponseMetadataTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExportResponseTypeDef",
-    "GatewayResponseResponseMetadataTypeDef",
-    "IntegrationResponseResponseMetadataTypeDef",
-    "MethodResponseResponseMetadataTypeDef",
-    "ModelResponseMetadataTypeDef",
-    "RequestValidatorResponseMetadataTypeDef",
     "SdkResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "TagsTypeDef",
     "TemplateTypeDef",
+    "TestInvokeAuthorizerRequestRequestTypeDef",
     "TestInvokeAuthorizerResponseTypeDef",
+    "TestInvokeMethodRequestRequestTypeDef",
     "TestInvokeMethodResponseTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "UsagePlanKeyResponseMetadataTypeDef",
+    "UsagePlanKeyTypeDef",
     "UsageTypeDef",
     "VpcLinkResponseMetadataTypeDef",
+    "VpcLinkTypeDef",
     "AccountTypeDef",
     "ApiStageTypeDef",
     "ApiKeysTypeDef",
     "AuthorizersTypeDef",
     "BasePathMappingsTypeDef",
     "CreateStageRequestRequestTypeDef",
     "ClientCertificatesTypeDef",
@@ -206,32 +224,14 @@
     "CreateDomainNameRequestRequestTypeDef",
     "DeploymentResponseMetadataTypeDef",
     "DeploymentTypeDef",
     "DocumentationVersionsTypeDef",
     "DomainNameResponseMetadataTypeDef",
     "DomainNameTypeDef",
     "GatewayResponsesTypeDef",
-    "GetApiKeysRequestGetApiKeysPaginateTypeDef",
-    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    "GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef",
-    "GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef",
-    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    "GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef",
-    "GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef",
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
-    "GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef",
-    "GetModelsRequestGetModelsPaginateTypeDef",
-    "GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef",
-    "GetResourcesRequestGetResourcesPaginateTypeDef",
-    "GetRestApisRequestGetRestApisPaginateTypeDef",
-    "GetSdkTypesRequestGetSdkTypesPaginateTypeDef",
-    "GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef",
-    "GetUsagePlansRequestGetUsagePlansPaginateTypeDef",
-    "GetUsageRequestGetUsagePaginateTypeDef",
-    "GetVpcLinksRequestGetVpcLinksPaginateTypeDef",
     "IntegrationResponseMetadataTypeDef",
     "IntegrationTypeDef",
     "PutIntegrationRequestRequestTypeDef",
     "StageResponseMetadataTypeDef",
     "StageTypeDef",
     "ModelsTypeDef",
     "UpdateAccountRequestRequestTypeDef",
@@ -283,34 +283,49 @@
     {
         "format": str,
         "destinationArn": str,
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
 ThrottleSettingsTypeDef = TypedDict(
     "ThrottleSettingsTypeDef",
     {
         "burstLimit": int,
         "rateLimit": float,
     },
     total=False,
 )
 
+ApiKeyIdsTypeDef = TypedDict(
+    "ApiKeyIdsTypeDef",
+    {
+        "ids": List[str],
+        "warnings": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ApiKeyResponseMetadataTypeDef = TypedDict(
+    "ApiKeyResponseMetadataTypeDef",
+    {
+        "id": str,
+        "value": str,
+        "name": str,
+        "customerId": str,
+        "description": str,
+        "enabled": bool,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "stageKeys": List[str],
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ApiKeyTypeDef = TypedDict(
     "ApiKeyTypeDef",
     {
         "id": str,
         "value": str,
         "name": str,
         "customerId": str,
@@ -320,14 +335,31 @@
         "lastUpdatedDate": datetime,
         "stageKeys": List[str],
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+AuthorizerResponseMetadataTypeDef = TypedDict(
+    "AuthorizerResponseMetadataTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "type": AuthorizerTypeType,
+        "providerARNs": List[str],
+        "authType": str,
+        "authorizerUri": str,
+        "authorizerCredentials": str,
+        "identitySource": str,
+        "identityValidationExpression": str,
+        "authorizerResultTtlInSeconds": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AuthorizerTypeDef = TypedDict(
     "AuthorizerTypeDef",
     {
         "id": str,
         "name": str,
         "type": AuthorizerTypeType,
         "providerARNs": List[str],
@@ -337,14 +369,24 @@
         "identitySource": str,
         "identityValidationExpression": str,
         "authorizerResultTtlInSeconds": int,
     },
     total=False,
 )
 
+BasePathMappingResponseMetadataTypeDef = TypedDict(
+    "BasePathMappingResponseMetadataTypeDef",
+    {
+        "basePath": str,
+        "restApiId": str,
+        "stage": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BasePathMappingTypeDef = TypedDict(
     "BasePathMappingTypeDef",
     {
         "basePath": str,
         "restApiId": str,
         "stage": str,
     },
@@ -358,14 +400,27 @@
         "deploymentId": str,
         "stageVariableOverrides": Mapping[str, str],
         "useStageCache": bool,
     },
     total=False,
 )
 
+ClientCertificateResponseMetadataTypeDef = TypedDict(
+    "ClientCertificateResponseMetadataTypeDef",
+    {
+        "clientCertificateId": str,
+        "description": str,
+        "pemEncodedCertificate": str,
+        "createdDate": datetime,
+        "expirationDate": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ClientCertificateTypeDef = TypedDict(
     "ClientCertificateTypeDef",
     {
         "clientCertificateId": str,
         "description": str,
         "pemEncodedCertificate": str,
         "createdDate": datetime,
@@ -771,14 +826,33 @@
     {
         "authorizationType": str,
         "apiKeyRequired": bool,
     },
     total=False,
 )
 
+DocumentationPartIdsTypeDef = TypedDict(
+    "DocumentationPartIdsTypeDef",
+    {
+        "ids": List[str],
+        "warnings": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DocumentationVersionResponseMetadataTypeDef = TypedDict(
+    "DocumentationVersionResponseMetadataTypeDef",
+    {
+        "version": str,
+        "createdDate": datetime,
+        "description": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DocumentationVersionTypeDef = TypedDict(
     "DocumentationVersionTypeDef",
     {
         "version": str,
         "createdDate": datetime,
         "description": str,
     },
@@ -791,14 +865,31 @@
         "truststoreUri": str,
         "truststoreVersion": str,
         "truststoreWarnings": List[str],
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
+ExportResponseTypeDef = TypedDict(
+    "ExportResponseTypeDef",
+    {
+        "contentType": str,
+        "contentDisposition": str,
+        "body": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FlushStageAuthorizersCacheRequestRequestTypeDef = TypedDict(
     "FlushStageAuthorizersCacheRequestRequestTypeDef",
     {
         "restApiId": str,
         "stageName": str,
     },
 )
@@ -807,14 +898,26 @@
     "FlushStageCacheRequestRequestTypeDef",
     {
         "restApiId": str,
         "stageName": str,
     },
 )
 
+GatewayResponseResponseMetadataTypeDef = TypedDict(
+    "GatewayResponseResponseMetadataTypeDef",
+    {
+        "responseType": GatewayResponseTypeType,
+        "statusCode": str,
+        "responseParameters": Dict[str, str],
+        "responseTemplates": Dict[str, str],
+        "defaultResponse": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GatewayResponseTypeDef = TypedDict(
     "GatewayResponseTypeDef",
     {
         "responseType": GatewayResponseTypeType,
         "statusCode": str,
         "responseParameters": Dict[str, str],
         "responseTemplates": Dict[str, str],
@@ -847,20 +950,21 @@
 )
 
 class GetApiKeyRequestRequestTypeDef(
     _RequiredGetApiKeyRequestRequestTypeDef, _OptionalGetApiKeyRequestRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetApiKeysRequestGetApiKeysPaginateTypeDef = TypedDict(
+    "GetApiKeysRequestGetApiKeysPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "nameQuery": str,
+        "customerId": str,
+        "includeValues": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetApiKeysRequestRequestTypeDef = TypedDict(
     "GetApiKeysRequestRequestTypeDef",
     {
@@ -877,14 +981,34 @@
     "GetAuthorizerRequestRequestTypeDef",
     {
         "restApiId": str,
         "authorizerId": str,
     },
 )
 
+_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
+    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+):
+    pass
+
 _RequiredGetAuthorizersRequestRequestTypeDef = TypedDict(
     "_RequiredGetAuthorizersRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetAuthorizersRequestRequestTypeDef = TypedDict(
@@ -905,14 +1029,34 @@
     "GetBasePathMappingRequestRequestTypeDef",
     {
         "domainName": str,
         "basePath": str,
     },
 )
 
+_RequiredGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef = TypedDict(
+    "_RequiredGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef",
+    {
+        "domainName": str,
+    },
+)
+_OptionalGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef = TypedDict(
+    "_OptionalGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef(
+    _RequiredGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef,
+    _OptionalGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetBasePathMappingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBasePathMappingsRequestRequestTypeDef",
     {
         "domainName": str,
     },
 )
 _OptionalGetBasePathMappingsRequestRequestTypeDef = TypedDict(
@@ -933,14 +1077,22 @@
 GetClientCertificateRequestRequestTypeDef = TypedDict(
     "GetClientCertificateRequestRequestTypeDef",
     {
         "clientCertificateId": str,
     },
 )
 
+GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef = TypedDict(
+    "GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetClientCertificatesRequestRequestTypeDef = TypedDict(
     "GetClientCertificatesRequestRequestTypeDef",
     {
         "position": str,
         "limit": int,
     },
     total=False,
@@ -962,14 +1114,34 @@
 )
 
 class GetDeploymentRequestRequestTypeDef(
     _RequiredGetDeploymentRequestRequestTypeDef, _OptionalGetDeploymentRequestRequestTypeDef
 ):
     pass
 
+_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
+    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeploymentsRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetDeploymentsRequestRequestTypeDef = TypedDict(
@@ -990,14 +1162,38 @@
     "GetDocumentationPartRequestRequestTypeDef",
     {
         "restApiId": str,
         "documentationPartId": str,
     },
 )
 
+_RequiredGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef = TypedDict(
+    "_RequiredGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef = TypedDict(
+    "_OptionalGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef",
+    {
+        "type": DocumentationPartTypeType,
+        "nameQuery": str,
+        "path": str,
+        "locationStatus": LocationStatusTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef(
+    _RequiredGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef,
+    _OptionalGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetDocumentationPartsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDocumentationPartsRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetDocumentationPartsRequestRequestTypeDef = TypedDict(
@@ -1023,14 +1219,34 @@
     "GetDocumentationVersionRequestRequestTypeDef",
     {
         "restApiId": str,
         "documentationVersion": str,
     },
 )
 
+_RequiredGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef(
+    _RequiredGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef,
+    _OptionalGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetDocumentationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDocumentationVersionsRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetDocumentationVersionsRequestRequestTypeDef = TypedDict(
@@ -1051,14 +1267,22 @@
 GetDomainNameRequestRequestTypeDef = TypedDict(
     "GetDomainNameRequestRequestTypeDef",
     {
         "domainName": str,
     },
 )
 
+GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetDomainNamesRequestRequestTypeDef = TypedDict(
     "GetDomainNamesRequestRequestTypeDef",
     {
         "position": str,
         "limit": int,
     },
     total=False,
@@ -1090,14 +1314,34 @@
     "GetGatewayResponseRequestRequestTypeDef",
     {
         "restApiId": str,
         "responseType": GatewayResponseTypeType,
     },
 )
 
+_RequiredGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef = TypedDict(
+    "_RequiredGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef = TypedDict(
+    "_OptionalGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef(
+    _RequiredGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef,
+    _OptionalGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef,
+):
+    pass
+
 _RequiredGetGatewayResponsesRequestRequestTypeDef = TypedDict(
     "_RequiredGetGatewayResponsesRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetGatewayResponsesRequestRequestTypeDef = TypedDict(
@@ -1177,14 +1421,34 @@
     "GetModelTemplateRequestRequestTypeDef",
     {
         "restApiId": str,
         "modelName": str,
     },
 )
 
+_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetModelsRequestGetModelsPaginateTypeDef(
+    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
+    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetModelsRequestRequestTypeDef = TypedDict(
     "_RequiredGetModelsRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetModelsRequestRequestTypeDef = TypedDict(
@@ -1205,14 +1469,34 @@
     "GetRequestValidatorRequestRequestTypeDef",
     {
         "restApiId": str,
         "requestValidatorId": str,
     },
 )
 
+_RequiredGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef = TypedDict(
+    "_RequiredGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef = TypedDict(
+    "_OptionalGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef(
+    _RequiredGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef,
+    _OptionalGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetRequestValidatorsRequestRequestTypeDef = TypedDict(
     "_RequiredGetRequestValidatorsRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetRequestValidatorsRequestRequestTypeDef = TypedDict(
@@ -1246,14 +1530,35 @@
 )
 
 class GetResourceRequestRequestTypeDef(
     _RequiredGetResourceRequestRequestTypeDef, _OptionalGetResourceRequestRequestTypeDef
 ):
     pass
 
+_RequiredGetResourcesRequestGetResourcesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcesRequestGetResourcesPaginateTypeDef",
+    {
+        "restApiId": str,
+    },
+)
+_OptionalGetResourcesRequestGetResourcesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcesRequestGetResourcesPaginateTypeDef",
+    {
+        "embed": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetResourcesRequestGetResourcesPaginateTypeDef(
+    _RequiredGetResourcesRequestGetResourcesPaginateTypeDef,
+    _OptionalGetResourcesRequestGetResourcesPaginateTypeDef,
+):
+    pass
+
 _RequiredGetResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcesRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 _OptionalGetResourcesRequestRequestTypeDef = TypedDict(
@@ -1274,14 +1579,22 @@
 GetRestApiRequestRequestTypeDef = TypedDict(
     "GetRestApiRequestRequestTypeDef",
     {
         "restApiId": str,
     },
 )
 
+GetRestApisRequestGetRestApisPaginateTypeDef = TypedDict(
+    "GetRestApisRequestGetRestApisPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetRestApisRequestRequestTypeDef = TypedDict(
     "GetRestApisRequestRequestTypeDef",
     {
         "position": str,
         "limit": int,
     },
     total=False,
@@ -1311,14 +1624,22 @@
 GetSdkTypeRequestRequestTypeDef = TypedDict(
     "GetSdkTypeRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
+GetSdkTypesRequestGetSdkTypesPaginateTypeDef = TypedDict(
+    "GetSdkTypesRequestGetSdkTypesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetSdkTypesRequestRequestTypeDef = TypedDict(
     "GetSdkTypesRequestRequestTypeDef",
     {
         "position": str,
         "limit": int,
     },
     total=False,
@@ -1375,14 +1696,35 @@
     "GetUsagePlanKeyRequestRequestTypeDef",
     {
         "usagePlanId": str,
         "keyId": str,
     },
 )
 
+_RequiredGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef = TypedDict(
+    "_RequiredGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef",
+    {
+        "usagePlanId": str,
+    },
+)
+_OptionalGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef = TypedDict(
+    "_OptionalGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef",
+    {
+        "nameQuery": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef(
+    _RequiredGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef,
+    _OptionalGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef,
+):
+    pass
+
 _RequiredGetUsagePlanKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetUsagePlanKeysRequestRequestTypeDef",
     {
         "usagePlanId": str,
     },
 )
 _OptionalGetUsagePlanKeysRequestRequestTypeDef = TypedDict(
@@ -1403,24 +1745,55 @@
 GetUsagePlanRequestRequestTypeDef = TypedDict(
     "GetUsagePlanRequestRequestTypeDef",
     {
         "usagePlanId": str,
     },
 )
 
+GetUsagePlansRequestGetUsagePlansPaginateTypeDef = TypedDict(
+    "GetUsagePlansRequestGetUsagePlansPaginateTypeDef",
+    {
+        "keyId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetUsagePlansRequestRequestTypeDef = TypedDict(
     "GetUsagePlansRequestRequestTypeDef",
     {
         "position": str,
         "keyId": str,
         "limit": int,
     },
     total=False,
 )
 
+_RequiredGetUsageRequestGetUsagePaginateTypeDef = TypedDict(
+    "_RequiredGetUsageRequestGetUsagePaginateTypeDef",
+    {
+        "usagePlanId": str,
+        "startDate": str,
+        "endDate": str,
+    },
+)
+_OptionalGetUsageRequestGetUsagePaginateTypeDef = TypedDict(
+    "_OptionalGetUsageRequestGetUsagePaginateTypeDef",
+    {
+        "keyId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetUsageRequestGetUsagePaginateTypeDef(
+    _RequiredGetUsageRequestGetUsagePaginateTypeDef, _OptionalGetUsageRequestGetUsagePaginateTypeDef
+):
+    pass
+
 _RequiredGetUsageRequestRequestTypeDef = TypedDict(
     "_RequiredGetUsageRequestRequestTypeDef",
     {
         "usagePlanId": str,
         "startDate": str,
         "endDate": str,
     },
@@ -1443,14 +1816,22 @@
 GetVpcLinkRequestRequestTypeDef = TypedDict(
     "GetVpcLinkRequestRequestTypeDef",
     {
         "vpcLinkId": str,
     },
 )
 
+GetVpcLinksRequestGetVpcLinksPaginateTypeDef = TypedDict(
+    "GetVpcLinksRequestGetVpcLinksPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetVpcLinksRequestRequestTypeDef = TypedDict(
     "GetVpcLinksRequestRequestTypeDef",
     {
         "position": str,
         "limit": int,
     },
     total=False,
@@ -1534,24 +1915,46 @@
     "TlsConfigTypeDef",
     {
         "insecureSkipVerification": bool,
     },
     total=False,
 )
 
+IntegrationResponseResponseMetadataTypeDef = TypedDict(
+    "IntegrationResponseResponseMetadataTypeDef",
+    {
+        "statusCode": str,
+        "selectionPattern": str,
+        "responseParameters": Dict[str, str],
+        "responseTemplates": Dict[str, str],
+        "contentHandling": ContentHandlingStrategyType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MethodResponseTypeDef = TypedDict(
     "MethodResponseTypeDef",
     {
         "statusCode": str,
         "responseParameters": Dict[str, bool],
         "responseModels": Dict[str, str],
     },
     total=False,
 )
 
+MethodResponseResponseMetadataTypeDef = TypedDict(
+    "MethodResponseResponseMetadataTypeDef",
+    {
+        "statusCode": str,
+        "responseParameters": Dict[str, bool],
+        "responseModels": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MethodSettingTypeDef = TypedDict(
     "MethodSettingTypeDef",
     {
         "metricsEnabled": bool,
         "loggingLevel": str,
         "dataTraceEnabled": bool,
         "throttlingBurstLimit": int,
@@ -1561,26 +1964,48 @@
         "cacheDataEncrypted": bool,
         "requireAuthorizationForCacheControl": bool,
         "unauthorizedCacheControlHeaderStrategy": UnauthorizedCacheControlHeaderStrategyType,
     },
     total=False,
 )
 
+ModelResponseMetadataTypeDef = TypedDict(
+    "ModelResponseMetadataTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "description": str,
+        "schema": str,
+        "contentType": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ModelTypeDef = TypedDict(
     "ModelTypeDef",
     {
         "id": str,
         "name": str,
         "description": str,
         "schema": str,
         "contentType": str,
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
 PatchOperationTypeDef = TypedDict(
     "PatchOperationTypeDef",
     {
         "op": OpType,
         "path": str,
         "value": str,
         "from": str,
@@ -1706,45 +2131,93 @@
 )
 
 class PutRestApiRequestRequestTypeDef(
     _RequiredPutRestApiRequestRequestTypeDef, _OptionalPutRestApiRequestRequestTypeDef
 ):
     pass
 
+RequestValidatorResponseMetadataTypeDef = TypedDict(
+    "RequestValidatorResponseMetadataTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "validateRequestBody": bool,
+        "validateRequestParameters": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RequestValidatorTypeDef = TypedDict(
     "RequestValidatorTypeDef",
     {
         "id": str,
         "name": str,
         "validateRequestBody": bool,
         "validateRequestParameters": bool,
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
 SdkConfigurationPropertyTypeDef = TypedDict(
     "SdkConfigurationPropertyTypeDef",
     {
         "name": str,
         "friendlyName": str,
         "description": str,
         "required": bool,
         "defaultValue": str,
     },
     total=False,
 )
 
+SdkResponseTypeDef = TypedDict(
+    "SdkResponseTypeDef",
+    {
+        "contentType": str,
+        "contentDisposition": str,
+        "body": StreamingBody,
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
 
+TagsTypeDef = TypedDict(
+    "TagsTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TemplateTypeDef = TypedDict(
+    "TemplateTypeDef",
+    {
+        "value": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredTestInvokeAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredTestInvokeAuthorizerRequestRequestTypeDef",
     {
         "restApiId": str,
         "authorizerId": str,
     },
 )
@@ -1763,14 +2236,28 @@
 
 class TestInvokeAuthorizerRequestRequestTypeDef(
     _RequiredTestInvokeAuthorizerRequestRequestTypeDef,
     _OptionalTestInvokeAuthorizerRequestRequestTypeDef,
 ):
     pass
 
+TestInvokeAuthorizerResponseTypeDef = TypedDict(
+    "TestInvokeAuthorizerResponseTypeDef",
+    {
+        "clientStatus": int,
+        "log": str,
+        "latency": int,
+        "principalId": str,
+        "policy": str,
+        "authorization": Dict[str, List[str]],
+        "claims": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredTestInvokeMethodRequestRequestTypeDef = TypedDict(
     "_RequiredTestInvokeMethodRequestRequestTypeDef",
     {
         "restApiId": str,
         "resourceId": str,
         "httpMethod": str,
     },
@@ -1789,304 +2276,105 @@
 )
 
 class TestInvokeMethodRequestRequestTypeDef(
     _RequiredTestInvokeMethodRequestRequestTypeDef, _OptionalTestInvokeMethodRequestRequestTypeDef
 ):
     pass
 
+TestInvokeMethodResponseTypeDef = TypedDict(
+    "TestInvokeMethodResponseTypeDef",
+    {
+        "status": int,
+        "body": str,
+        "headers": Dict[str, str],
+        "multiValueHeaders": Dict[str, List[str]],
+        "log": str,
+        "latency": int,
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
 
-UsagePlanKeyTypeDef = TypedDict(
-    "UsagePlanKeyTypeDef",
+UsagePlanKeyResponseMetadataTypeDef = TypedDict(
+    "UsagePlanKeyResponseMetadataTypeDef",
     {
         "id": str,
         "type": str,
         "value": str,
         "name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-VpcLinkTypeDef = TypedDict(
-    "VpcLinkTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "description": str,
-        "targetArns": List[str],
-        "status": VpcLinkStatusType,
-        "statusMessage": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
 )
 
-ApiKeyIdsTypeDef = TypedDict(
-    "ApiKeyIdsTypeDef",
-    {
-        "ids": List[str],
-        "warnings": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ApiKeyResponseMetadataTypeDef = TypedDict(
-    "ApiKeyResponseMetadataTypeDef",
-    {
-        "id": str,
-        "value": str,
-        "name": str,
-        "customerId": str,
-        "description": str,
-        "enabled": bool,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "stageKeys": List[str],
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AuthorizerResponseMetadataTypeDef = TypedDict(
-    "AuthorizerResponseMetadataTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "type": AuthorizerTypeType,
-        "providerARNs": List[str],
-        "authType": str,
-        "authorizerUri": str,
-        "authorizerCredentials": str,
-        "identitySource": str,
-        "identityValidationExpression": str,
-        "authorizerResultTtlInSeconds": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BasePathMappingResponseMetadataTypeDef = TypedDict(
-    "BasePathMappingResponseMetadataTypeDef",
-    {
-        "basePath": str,
-        "restApiId": str,
-        "stage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ClientCertificateResponseMetadataTypeDef = TypedDict(
-    "ClientCertificateResponseMetadataTypeDef",
-    {
-        "clientCertificateId": str,
-        "description": str,
-        "pemEncodedCertificate": str,
-        "createdDate": datetime,
-        "expirationDate": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DocumentationPartIdsTypeDef = TypedDict(
-    "DocumentationPartIdsTypeDef",
-    {
-        "ids": List[str],
-        "warnings": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DocumentationVersionResponseMetadataTypeDef = TypedDict(
-    "DocumentationVersionResponseMetadataTypeDef",
-    {
-        "version": str,
-        "createdDate": datetime,
-        "description": str,
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
-ExportResponseTypeDef = TypedDict(
-    "ExportResponseTypeDef",
-    {
-        "contentType": str,
-        "contentDisposition": str,
-        "body": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GatewayResponseResponseMetadataTypeDef = TypedDict(
-    "GatewayResponseResponseMetadataTypeDef",
-    {
-        "responseType": GatewayResponseTypeType,
-        "statusCode": str,
-        "responseParameters": Dict[str, str],
-        "responseTemplates": Dict[str, str],
-        "defaultResponse": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-IntegrationResponseResponseMetadataTypeDef = TypedDict(
-    "IntegrationResponseResponseMetadataTypeDef",
-    {
-        "statusCode": str,
-        "selectionPattern": str,
-        "responseParameters": Dict[str, str],
-        "responseTemplates": Dict[str, str],
-        "contentHandling": ContentHandlingStrategyType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MethodResponseResponseMetadataTypeDef = TypedDict(
-    "MethodResponseResponseMetadataTypeDef",
-    {
-        "statusCode": str,
-        "responseParameters": Dict[str, bool],
-        "responseModels": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ModelResponseMetadataTypeDef = TypedDict(
-    "ModelResponseMetadataTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "description": str,
-        "schema": str,
-        "contentType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RequestValidatorResponseMetadataTypeDef = TypedDict(
-    "RequestValidatorResponseMetadataTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "validateRequestBody": bool,
-        "validateRequestParameters": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SdkResponseTypeDef = TypedDict(
-    "SdkResponseTypeDef",
-    {
-        "contentType": str,
-        "contentDisposition": str,
-        "body": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TagsTypeDef = TypedDict(
-    "TagsTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TemplateTypeDef = TypedDict(
-    "TemplateTypeDef",
-    {
-        "value": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TestInvokeAuthorizerResponseTypeDef = TypedDict(
-    "TestInvokeAuthorizerResponseTypeDef",
-    {
-        "clientStatus": int,
-        "log": str,
-        "latency": int,
-        "principalId": str,
-        "policy": str,
-        "authorization": Dict[str, List[str]],
-        "claims": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TestInvokeMethodResponseTypeDef = TypedDict(
-    "TestInvokeMethodResponseTypeDef",
-    {
-        "status": int,
-        "body": str,
-        "headers": Dict[str, str],
-        "multiValueHeaders": Dict[str, List[str]],
-        "log": str,
-        "latency": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UsagePlanKeyResponseMetadataTypeDef = TypedDict(
-    "UsagePlanKeyResponseMetadataTypeDef",
+UsagePlanKeyTypeDef = TypedDict(
+    "UsagePlanKeyTypeDef",
     {
         "id": str,
         "type": str,
         "value": str,
         "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
 UsageTypeDef = TypedDict(
     "UsageTypeDef",
     {
         "usagePlanId": str,
         "startDate": str,
         "endDate": str,
         "position": str,
         "items": Dict[str, List[List[int]]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VpcLinkResponseMetadataTypeDef = TypedDict(
     "VpcLinkResponseMetadataTypeDef",
     {
         "id": str,
         "name": str,
         "description": str,
         "targetArns": List[str],
         "status": VpcLinkStatusType,
         "statusMessage": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+VpcLinkTypeDef = TypedDict(
+    "VpcLinkTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "description": str,
+        "targetArns": List[str],
+        "status": VpcLinkStatusType,
+        "statusMessage": str,
+        "tags": Dict[str, str],
     },
+    total=False,
 )
 
 AccountTypeDef = TypedDict(
     "AccountTypeDef",
     {
         "cloudwatchRoleArn": str,
         "throttleSettings": ThrottleSettingsTypeDef,
         "features": List[str],
         "apiKeyVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApiStageTypeDef = TypedDict(
     "ApiStageTypeDef",
     {
         "apiId": str,
@@ -2098,33 +2386,33 @@
 
 ApiKeysTypeDef = TypedDict(
     "ApiKeysTypeDef",
     {
         "warnings": List[str],
         "position": str,
         "items": List[ApiKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AuthorizersTypeDef = TypedDict(
     "AuthorizersTypeDef",
     {
         "position": str,
         "items": List[AuthorizerTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BasePathMappingsTypeDef = TypedDict(
     "BasePathMappingsTypeDef",
     {
         "position": str,
         "items": List[BasePathMappingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateStageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStageRequestRequestTypeDef",
     {
         "restApiId": str,
@@ -2153,15 +2441,15 @@
     pass
 
 ClientCertificatesTypeDef = TypedDict(
     "ClientCertificatesTypeDef",
     {
         "position": str,
         "items": List[ClientCertificateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateApiKeyRequestRequestTypeDef = TypedDict(
     "CreateApiKeyRequestRequestTypeDef",
     {
         "name": str,
@@ -2213,15 +2501,15 @@
 
 DocumentationPartResponseMetadataTypeDef = TypedDict(
     "DocumentationPartResponseMetadataTypeDef",
     {
         "id": str,
         "location": DocumentationPartLocationTypeDef,
         "properties": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DocumentationPartTypeDef = TypedDict(
     "DocumentationPartTypeDef",
     {
         "id": str,
@@ -2271,15 +2559,15 @@
         "binaryMediaTypes": List[str],
         "minimumCompressionSize": int,
         "apiKeySource": ApiKeySourceTypeType,
         "endpointConfiguration": EndpointConfigurationTypeDef,
         "policy": str,
         "tags": Dict[str, str],
         "disableExecuteApiEndpoint": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestApiTypeDef = TypedDict(
     "RestApiTypeDef",
     {
         "id": str,
@@ -2332,15 +2620,15 @@
 DeploymentResponseMetadataTypeDef = TypedDict(
     "DeploymentResponseMetadataTypeDef",
     {
         "id": str,
         "description": str,
         "createdDate": datetime,
         "apiSummary": Dict[str, Dict[str, MethodSnapshotTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "id": str,
@@ -2352,15 +2640,15 @@
 )
 
 DocumentationVersionsTypeDef = TypedDict(
     "DocumentationVersionsTypeDef",
     {
         "position": str,
         "items": List[DocumentationVersionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainNameResponseMetadataTypeDef = TypedDict(
     "DomainNameResponseMetadataTypeDef",
     {
         "domainName": str,
@@ -2376,15 +2664,15 @@
         "endpointConfiguration": EndpointConfigurationTypeDef,
         "domainNameStatus": DomainNameStatusType,
         "domainNameStatusMessage": str,
         "securityPolicy": SecurityPolicyType,
         "tags": Dict[str, str],
         "mutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "ownershipVerificationCertificateArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainNameTypeDef = TypedDict(
     "DomainNameTypeDef",
     {
         "domainName": str,
@@ -2409,304 +2697,16 @@
 )
 
 GatewayResponsesTypeDef = TypedDict(
     "GatewayResponsesTypeDef",
     {
         "position": str,
         "items": List[GatewayResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetApiKeysRequestGetApiKeysPaginateTypeDef = TypedDict(
-    "GetApiKeysRequestGetApiKeysPaginateTypeDef",
-    {
-        "nameQuery": str,
-        "customerId": str,
-        "includeValues": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
-    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-):
-    pass
-
-_RequiredGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef = TypedDict(
-    "_RequiredGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef",
-    {
-        "domainName": str,
-    },
-)
-_OptionalGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef = TypedDict(
-    "_OptionalGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef(
-    _RequiredGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef,
-    _OptionalGetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef,
-):
-    pass
-
-GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef = TypedDict(
-    "GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
-    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-):
-    pass
-
-_RequiredGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef = TypedDict(
-    "_RequiredGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef = TypedDict(
-    "_OptionalGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef",
-    {
-        "type": DocumentationPartTypeType,
-        "nameQuery": str,
-        "path": str,
-        "locationStatus": LocationStatusTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef(
-    _RequiredGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef,
-    _OptionalGetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef,
-):
-    pass
-
-_RequiredGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef(
-    _RequiredGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef,
-    _OptionalGetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef,
-):
-    pass
-
-GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef = TypedDict(
-    "_RequiredGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef = TypedDict(
-    "_OptionalGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef(
-    _RequiredGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef,
-    _OptionalGetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef,
-):
-    pass
-
-_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetModelsRequestGetModelsPaginateTypeDef(
-    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
-    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
-):
-    pass
-
-_RequiredGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef = TypedDict(
-    "_RequiredGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef = TypedDict(
-    "_OptionalGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef(
-    _RequiredGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef,
-    _OptionalGetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef,
-):
-    pass
-
-_RequiredGetResourcesRequestGetResourcesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcesRequestGetResourcesPaginateTypeDef",
-    {
-        "restApiId": str,
-    },
-)
-_OptionalGetResourcesRequestGetResourcesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcesRequestGetResourcesPaginateTypeDef",
-    {
-        "embed": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetResourcesRequestGetResourcesPaginateTypeDef(
-    _RequiredGetResourcesRequestGetResourcesPaginateTypeDef,
-    _OptionalGetResourcesRequestGetResourcesPaginateTypeDef,
-):
-    pass
-
-GetRestApisRequestGetRestApisPaginateTypeDef = TypedDict(
-    "GetRestApisRequestGetRestApisPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetSdkTypesRequestGetSdkTypesPaginateTypeDef = TypedDict(
-    "GetSdkTypesRequestGetSdkTypesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef = TypedDict(
-    "_RequiredGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef",
-    {
-        "usagePlanId": str,
-    },
-)
-_OptionalGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef = TypedDict(
-    "_OptionalGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef",
-    {
-        "nameQuery": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef(
-    _RequiredGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef,
-    _OptionalGetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef,
-):
-    pass
-
-GetUsagePlansRequestGetUsagePlansPaginateTypeDef = TypedDict(
-    "GetUsagePlansRequestGetUsagePlansPaginateTypeDef",
-    {
-        "keyId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetUsageRequestGetUsagePaginateTypeDef = TypedDict(
-    "_RequiredGetUsageRequestGetUsagePaginateTypeDef",
-    {
-        "usagePlanId": str,
-        "startDate": str,
-        "endDate": str,
-    },
-)
-_OptionalGetUsageRequestGetUsagePaginateTypeDef = TypedDict(
-    "_OptionalGetUsageRequestGetUsagePaginateTypeDef",
-    {
-        "keyId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetUsageRequestGetUsagePaginateTypeDef(
-    _RequiredGetUsageRequestGetUsagePaginateTypeDef, _OptionalGetUsageRequestGetUsagePaginateTypeDef
-):
-    pass
-
-GetVpcLinksRequestGetVpcLinksPaginateTypeDef = TypedDict(
-    "GetVpcLinksRequestGetVpcLinksPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 IntegrationResponseMetadataTypeDef = TypedDict(
     "IntegrationResponseMetadataTypeDef",
     {
         "type": IntegrationTypeType,
         "httpMethod": str,
@@ -2719,15 +2719,15 @@
         "passthroughBehavior": str,
         "contentHandling": ContentHandlingStrategyType,
         "timeoutInMillis": int,
         "cacheNamespace": str,
         "cacheKeyParameters": List[str],
         "integrationResponses": Dict[str, IntegrationResponseTypeDef],
         "tlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IntegrationTypeDef = TypedDict(
     "IntegrationTypeDef",
     {
         "type": IntegrationTypeType,
@@ -2799,15 +2799,15 @@
         "accessLogSettings": AccessLogSettingsTypeDef,
         "canarySettings": CanarySettingsTypeDef,
         "tracingEnabled": bool,
         "webAclArn": str,
         "tags": Dict[str, str],
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StageTypeDef = TypedDict(
     "StageTypeDef",
     {
         "deploymentId": str,
@@ -2832,15 +2832,15 @@
 )
 
 ModelsTypeDef = TypedDict(
     "ModelsTypeDef",
     {
         "position": str,
         "items": List[ModelTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAccountRequestRequestTypeDef = TypedDict(
     "UpdateAccountRequestRequestTypeDef",
     {
         "patchOperations": Sequence[PatchOperationTypeDef],
@@ -3277,26 +3277,26 @@
     pass
 
 RequestValidatorsTypeDef = TypedDict(
     "RequestValidatorsTypeDef",
     {
         "position": str,
         "items": List[RequestValidatorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SdkTypeResponseMetadataTypeDef = TypedDict(
     "SdkTypeResponseMetadataTypeDef",
     {
         "id": str,
         "friendlyName": str,
         "description": str,
         "configurationProperties": List[SdkConfigurationPropertyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SdkTypeTypeDef = TypedDict(
     "SdkTypeTypeDef",
     {
         "id": str,
@@ -3308,24 +3308,24 @@
 )
 
 UsagePlanKeysTypeDef = TypedDict(
     "UsagePlanKeysTypeDef",
     {
         "position": str,
         "items": List[UsagePlanKeyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 VpcLinksTypeDef = TypedDict(
     "VpcLinksTypeDef",
     {
         "position": str,
         "items": List[VpcLinkTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateUsagePlanRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUsagePlanRequestRequestTypeDef",
     {
         "name": str,
@@ -3355,15 +3355,15 @@
         "name": str,
         "description": str,
         "apiStages": List[ApiStageTypeDef],
         "throttle": ThrottleSettingsTypeDef,
         "quota": QuotaSettingsTypeDef,
         "productCode": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UsagePlanTypeDef = TypedDict(
     "UsagePlanTypeDef",
     {
         "id": str,
@@ -3379,42 +3379,42 @@
 )
 
 DocumentationPartsTypeDef = TypedDict(
     "DocumentationPartsTypeDef",
     {
         "position": str,
         "items": List[DocumentationPartTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestApisTypeDef = TypedDict(
     "RestApisTypeDef",
     {
         "position": str,
         "items": List[RestApiTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeploymentsTypeDef = TypedDict(
     "DeploymentsTypeDef",
     {
         "position": str,
         "items": List[DeploymentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DomainNamesTypeDef = TypedDict(
     "DomainNamesTypeDef",
     {
         "position": str,
         "items": List[DomainNameTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MethodResponseMetadataTypeDef = TypedDict(
     "MethodResponseMetadataTypeDef",
     {
         "httpMethod": str,
@@ -3424,15 +3424,15 @@
         "requestValidatorId": str,
         "operationName": str,
         "requestParameters": Dict[str, bool],
         "requestModels": Dict[str, str],
         "methodResponses": Dict[str, MethodResponseTypeDef],
         "methodIntegration": IntegrationTypeDef,
         "authorizationScopes": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MethodTypeDef = TypedDict(
     "MethodTypeDef",
     {
         "httpMethod": str,
@@ -3450,45 +3450,45 @@
     total=False,
 )
 
 StagesTypeDef = TypedDict(
     "StagesTypeDef",
     {
         "item": List[StageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SdkTypesTypeDef = TypedDict(
     "SdkTypesTypeDef",
     {
         "position": str,
         "items": List[SdkTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UsagePlansTypeDef = TypedDict(
     "UsagePlansTypeDef",
     {
         "position": str,
         "items": List[UsagePlanTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceResponseMetadataTypeDef = TypedDict(
     "ResourceResponseMetadataTypeDef",
     {
         "id": str,
         "parentId": str,
         "pathPart": str,
         "path": str,
         "resourceMethods": Dict[str, MethodTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "id": str,
@@ -3501,10 +3501,10 @@
 )
 
 ResourcesTypeDef = TypedDict(
     "ResourcesTypeDef",
     {
         "position": str,
         "items": List[ResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway.egg-info/PKG-INFO` & `mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigateway
-Version: 1.26.40
-Summary: Type annotations for boto3.APIGateway 1.26.40 service generated with mypy-boto3-builder 7.12.2
+Version: 1.27.0
+Summary: Type annotations for boto3.APIGateway 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-apigateway"></a>
 
 # mypy-boto3-apigateway
 
 [![PyPI - mypy-boto3-apigateway](https://img.shields.io/pypi/v/mypy-boto3-apigateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigateway)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apigateway?color=blue)](https://pypistats.org/packages/mypy-boto3-apigateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.APIGateway 1.26.40](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
+[boto3.APIGateway 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-apigateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -405,20 +405,24 @@
 
 `mypy_boto3_apigateway.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apigateway.type_defs import (
     AccessLogSettingsTypeDef,
-    ResponseMetadataTypeDef,
     ThrottleSettingsTypeDef,
+    ApiKeyIdsTypeDef,
+    ApiKeyResponseMetadataTypeDef,
     ApiKeyTypeDef,
+    AuthorizerResponseMetadataTypeDef,
     AuthorizerTypeDef,
+    BasePathMappingResponseMetadataTypeDef,
     BasePathMappingTypeDef,
     CanarySettingsTypeDef,
+    ClientCertificateResponseMetadataTypeDef,
     ClientCertificateTypeDef,
     StageKeyTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     CreateBasePathMappingRequestRequestTypeDef,
     DeploymentCanarySettingsTypeDef,
     DocumentationPartLocationTypeDef,
     CreateDocumentationVersionRequestRequestTypeDef,
@@ -448,110 +452,124 @@
     DeleteResourceRequestRequestTypeDef,
     DeleteRestApiRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteUsagePlanKeyRequestRequestTypeDef,
     DeleteUsagePlanRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     MethodSnapshotTypeDef,
+    DocumentationPartIdsTypeDef,
+    DocumentationVersionResponseMetadataTypeDef,
     DocumentationVersionTypeDef,
     MutualTlsAuthenticationTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportResponseTypeDef,
     FlushStageAuthorizersCacheRequestRequestTypeDef,
     FlushStageCacheRequestRequestTypeDef,
+    GatewayResponseResponseMetadataTypeDef,
     GatewayResponseTypeDef,
     GenerateClientCertificateRequestRequestTypeDef,
     GetApiKeyRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetApiKeysRequestGetApiKeysPaginateTypeDef,
     GetApiKeysRequestRequestTypeDef,
     GetAuthorizerRequestRequestTypeDef,
+    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
     GetAuthorizersRequestRequestTypeDef,
     GetBasePathMappingRequestRequestTypeDef,
+    GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef,
     GetBasePathMappingsRequestRequestTypeDef,
     GetClientCertificateRequestRequestTypeDef,
+    GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef,
     GetClientCertificatesRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
+    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDocumentationPartRequestRequestTypeDef,
+    GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef,
     GetDocumentationPartsRequestRequestTypeDef,
     GetDocumentationVersionRequestRequestTypeDef,
+    GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef,
     GetDocumentationVersionsRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
+    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
     GetDomainNamesRequestRequestTypeDef,
     GetExportRequestRequestTypeDef,
     GetGatewayResponseRequestRequestTypeDef,
+    GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef,
     GetGatewayResponsesRequestRequestTypeDef,
     GetIntegrationRequestRequestTypeDef,
     GetIntegrationResponseRequestRequestTypeDef,
     GetMethodRequestRequestTypeDef,
     GetMethodResponseRequestRequestTypeDef,
     GetModelRequestRequestTypeDef,
     GetModelTemplateRequestRequestTypeDef,
+    GetModelsRequestGetModelsPaginateTypeDef,
     GetModelsRequestRequestTypeDef,
     GetRequestValidatorRequestRequestTypeDef,
+    GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef,
     GetRequestValidatorsRequestRequestTypeDef,
     GetResourceRequestRequestTypeDef,
+    GetResourcesRequestGetResourcesPaginateTypeDef,
     GetResourcesRequestRequestTypeDef,
     GetRestApiRequestRequestTypeDef,
+    GetRestApisRequestGetRestApisPaginateTypeDef,
     GetRestApisRequestRequestTypeDef,
     GetSdkRequestRequestTypeDef,
     GetSdkTypeRequestRequestTypeDef,
+    GetSdkTypesRequestGetSdkTypesPaginateTypeDef,
     GetSdkTypesRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
     GetStagesRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
     GetUsagePlanKeyRequestRequestTypeDef,
+    GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef,
     GetUsagePlanKeysRequestRequestTypeDef,
     GetUsagePlanRequestRequestTypeDef,
+    GetUsagePlansRequestGetUsagePlansPaginateTypeDef,
     GetUsagePlansRequestRequestTypeDef,
+    GetUsageRequestGetUsagePaginateTypeDef,
     GetUsageRequestRequestTypeDef,
     GetVpcLinkRequestRequestTypeDef,
+    GetVpcLinksRequestGetVpcLinksPaginateTypeDef,
     GetVpcLinksRequestRequestTypeDef,
     ImportApiKeysRequestRequestTypeDef,
     ImportDocumentationPartsRequestRequestTypeDef,
     ImportRestApiRequestRequestTypeDef,
     IntegrationResponseTypeDef,
     TlsConfigTypeDef,
+    IntegrationResponseResponseMetadataTypeDef,
     MethodResponseTypeDef,
+    MethodResponseResponseMetadataTypeDef,
     MethodSettingTypeDef,
+    ModelResponseMetadataTypeDef,
     ModelTypeDef,
+    PaginatorConfigTypeDef,
     PatchOperationTypeDef,
     PutGatewayResponseRequestRequestTypeDef,
     PutIntegrationResponseRequestRequestTypeDef,
     PutMethodRequestRequestTypeDef,
     PutMethodResponseRequestRequestTypeDef,
     PutRestApiRequestRequestTypeDef,
+    RequestValidatorResponseMetadataTypeDef,
     RequestValidatorTypeDef,
+    ResponseMetadataTypeDef,
     SdkConfigurationPropertyTypeDef,
-    TagResourceRequestRequestTypeDef,
-    TestInvokeAuthorizerRequestRequestTypeDef,
-    TestInvokeMethodRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UsagePlanKeyTypeDef,
-    VpcLinkTypeDef,
-    ApiKeyIdsTypeDef,
-    ApiKeyResponseMetadataTypeDef,
-    AuthorizerResponseMetadataTypeDef,
-    BasePathMappingResponseMetadataTypeDef,
-    ClientCertificateResponseMetadataTypeDef,
-    DocumentationPartIdsTypeDef,
-    DocumentationVersionResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportResponseTypeDef,
-    GatewayResponseResponseMetadataTypeDef,
-    IntegrationResponseResponseMetadataTypeDef,
-    MethodResponseResponseMetadataTypeDef,
-    ModelResponseMetadataTypeDef,
-    RequestValidatorResponseMetadataTypeDef,
     SdkResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     TagsTypeDef,
     TemplateTypeDef,
+    TestInvokeAuthorizerRequestRequestTypeDef,
     TestInvokeAuthorizerResponseTypeDef,
+    TestInvokeMethodRequestRequestTypeDef,
     TestInvokeMethodResponseTypeDef,
+    UntagResourceRequestRequestTypeDef,
     UsagePlanKeyResponseMetadataTypeDef,
+    UsagePlanKeyTypeDef,
     UsageTypeDef,
     VpcLinkResponseMetadataTypeDef,
+    VpcLinkTypeDef,
     AccountTypeDef,
     ApiStageTypeDef,
     ApiKeysTypeDef,
     AuthorizersTypeDef,
     BasePathMappingsTypeDef,
     CreateStageRequestRequestTypeDef,
     ClientCertificatesTypeDef,
@@ -566,32 +584,14 @@
     CreateDomainNameRequestRequestTypeDef,
     DeploymentResponseMetadataTypeDef,
     DeploymentTypeDef,
     DocumentationVersionsTypeDef,
     DomainNameResponseMetadataTypeDef,
     DomainNameTypeDef,
     GatewayResponsesTypeDef,
-    GetApiKeysRequestGetApiKeysPaginateTypeDef,
-    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-    GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef,
-    GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef,
-    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-    GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef,
-    GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef,
-    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
-    GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef,
-    GetModelsRequestGetModelsPaginateTypeDef,
-    GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef,
-    GetResourcesRequestGetResourcesPaginateTypeDef,
-    GetRestApisRequestGetRestApisPaginateTypeDef,
-    GetSdkTypesRequestGetSdkTypesPaginateTypeDef,
-    GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef,
-    GetUsagePlansRequestGetUsagePlansPaginateTypeDef,
-    GetUsageRequestGetUsagePaginateTypeDef,
-    GetVpcLinksRequestGetVpcLinksPaginateTypeDef,
     IntegrationResponseMetadataTypeDef,
     IntegrationTypeDef,
     PutIntegrationRequestRequestTypeDef,
     StageResponseMetadataTypeDef,
     StageTypeDef,
     ModelsTypeDef,
     UpdateAccountRequestRequestTypeDef,
@@ -646,42 +646,42 @@
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

### Comparing `mypy-boto3-apigateway-1.26.40/mypy_boto3_apigateway.egg-info/SOURCES.txt` & `mypy-boto3-apigateway-1.27.0/mypy_boto3_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.26.40/setup.py` & `mypy-boto3-apigateway-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-apigateway.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-apigateway",
-    version="1.26.40",
+    version="1.27.0",
     packages=["mypy_boto3_apigateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.APIGateway 1.26.40 service generated with mypy-boto3-builder"
-        " 7.12.2"
+        "Type annotations for boto3.APIGateway 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/",
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


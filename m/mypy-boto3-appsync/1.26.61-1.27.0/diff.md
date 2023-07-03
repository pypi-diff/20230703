# Comparing `tmp/mypy-boto3-appsync-1.26.61.tar.gz` & `tmp/mypy-boto3-appsync-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appsync-1.26.61.tar", last modified: Tue Jan 31 20:49:53 2023, max compression
+gzip compressed data, was "mypy-boto3-appsync-1.27.0.tar", last modified: Mon Jul  3 19:50:24 2023, max compression
```

## Comparing `mypy-boto3-appsync-1.26.61.tar` & `mypy-boto3-appsync-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:53.626128 mypy-boto3-appsync-1.26.61/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-01-31 20:49:53.626128 mypy-boto3-appsync-1.26.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17403 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:53.614128 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36769 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-01-31 20:47:21.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-01-31 20:47:21.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-01-31 20:47:21.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48122 2023-01-31 20:47:22.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48049 2023-01-31 20:47:21.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:53.626128 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-01-31 20:49:53.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-31 20:49:53.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:53.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:53.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 20:49:53.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-31 20:49:53.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 20:49:53.626128 mypy-boto3-appsync-1.26.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.610859 mypy-boto3-appsync-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:45.000000 mypy-boto3-appsync-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19974 2023-07-03 19:50:24.610859 mypy-boto3-appsync-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18489 2023-07-03 19:32:45.000000 mypy-boto3-appsync-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.610859 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-03 19:32:45.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-03 19:32:45.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:32:45.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43388 2023-07-03 19:32:45.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43314 2023-07-03 19:32:45.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-03 19:32:46.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-07-03 19:32:45.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-07-03 19:32:45.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-03 19:32:45.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:45.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57202 2023-07-03 19:32:47.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57119 2023-07-03 19:32:47.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:45.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.610859 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19974 2023-07-03 19:50:24.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-03 19:50:24.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:24.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:50:24.000000 mypy-boto3-appsync-1.27.0/mypy_boto3_appsync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:24.610859 mypy-boto3-appsync-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:32:45.000000 mypy-boto3-appsync-1.27.0/setup.py
```

### Comparing `mypy-boto3-appsync-1.26.61/LICENSE` & `mypy-boto3-appsync-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-appsync-1.26.61/PKG-INFO` & `mypy-boto3-appsync-1.27.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appsync
-Version: 1.26.61
-Summary: Type annotations for boto3.AppSync 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.AppSync 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-appsync"></a>
 
 # mypy-boto3-appsync
 
 [![PyPI - mypy-boto3-appsync](https://img.shields.io/pypi/v/mypy-boto3-appsync.svg?color=blue)](https://pypi.org/project/mypy-boto3-appsync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appsync.svg?color=blue)](https://pypi.org/project/mypy-boto3-appsync)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appsync?color=blue)](https://pypistats.org/packages/mypy-boto3-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppSync 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
+[boto3.AppSync 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appsync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,26 +323,31 @@
     AuthenticationTypeType,
     AuthorizationTypeType,
     ConflictDetectionTypeType,
     ConflictHandlerTypeType,
     DataSourceTypeType,
     DefaultActionType,
     FieldLogLevelType,
+    GraphQLApiTypeType,
+    GraphQLApiVisibilityType,
     ListApiKeysPaginatorName,
     ListDataSourcesPaginatorName,
     ListFunctionsPaginatorName,
     ListGraphqlApisPaginatorName,
     ListResolversByFunctionPaginatorName,
     ListResolversPaginatorName,
     ListTypesPaginatorName,
+    MergeTypeType,
     OutputTypeType,
+    OwnershipType,
     RelationalDatabaseSourceTypeType,
     ResolverKindType,
     RuntimeNameType,
     SchemaStatusType,
+    SourceApiAssociationStatusType,
     TypeDefinitionFormatType,
     AppSyncServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -365,15 +370,15 @@
     LambdaAuthorizerConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     ApiAssociationTypeDef,
     ApiCacheTypeDef,
     ApiKeyTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    SourceApiAssociationConfigTypeDef,
     AwsIamConfigTypeDef,
     CachingConfigTypeDef,
     CodeErrorLocationTypeDef,
     CreateApiCacheRequestRequestTypeDef,
     CreateApiKeyRequestRequestTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
     EventBridgeDataSourceConfigTypeDef,
@@ -392,84 +397,105 @@
     DeleteDomainNameRequestRequestTypeDef,
     DeleteFunctionRequestRequestTypeDef,
     DeleteGraphqlApiRequestRequestTypeDef,
     DeleteResolverRequestRequestTypeDef,
     DeleteTypeRequestRequestTypeDef,
     DeltaSyncConfigTypeDef,
     DisassociateApiRequestRequestTypeDef,
+    DisassociateMergedGraphqlApiRequestRequestTypeDef,
+    DisassociateMergedGraphqlApiResponseTypeDef,
+    DisassociateSourceGraphqlApiRequestRequestTypeDef,
+    DisassociateSourceGraphqlApiResponseTypeDef,
     ErrorDetailTypeDef,
     EvaluateMappingTemplateRequestRequestTypeDef,
     FlushApiCacheRequestRequestTypeDef,
     GetApiAssociationRequestRequestTypeDef,
     GetApiCacheRequestRequestTypeDef,
     GetDataSourceRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
     GetGraphqlApiRequestRequestTypeDef,
     GetIntrospectionSchemaRequestRequestTypeDef,
+    GetIntrospectionSchemaResponseTypeDef,
     GetResolverRequestRequestTypeDef,
     GetSchemaCreationStatusRequestRequestTypeDef,
+    GetSchemaCreationStatusResponseTypeDef,
+    GetSourceApiAssociationRequestRequestTypeDef,
     GetTypeRequestRequestTypeDef,
     LambdaConflictHandlerConfigTypeDef,
-    PaginatorConfigTypeDef,
+    ListApiKeysRequestListApiKeysPaginateTypeDef,
     ListApiKeysRequestRequestTypeDef,
+    ListDataSourcesRequestListDataSourcesPaginateTypeDef,
     ListDataSourcesRequestRequestTypeDef,
     ListDomainNamesRequestRequestTypeDef,
+    ListFunctionsRequestListFunctionsPaginateTypeDef,
     ListFunctionsRequestRequestTypeDef,
+    ListGraphqlApisRequestListGraphqlApisPaginateTypeDef,
     ListGraphqlApisRequestRequestTypeDef,
+    ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
     ListResolversByFunctionRequestRequestTypeDef,
+    ListResolversRequestListResolversPaginateTypeDef,
     ListResolversRequestRequestTypeDef,
+    ListSourceApiAssociationsRequestRequestTypeDef,
+    SourceApiAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTypesByAssociationRequestRequestTypeDef,
+    ListTypesRequestListTypesPaginateTypeDef,
     ListTypesRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     RdsHttpEndpointConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartSchemaCreationRequestRequestTypeDef,
+    StartSchemaCreationResponseTypeDef,
+    StartSchemaMergeRequestRequestTypeDef,
+    StartSchemaMergeResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiCacheRequestRequestTypeDef,
     UpdateApiKeyRequestRequestTypeDef,
     UpdateDomainNameRequestRequestTypeDef,
     UpdateTypeRequestRequestTypeDef,
     AdditionalAuthenticationProviderTypeDef,
-    EvaluateCodeRequestRequestTypeDef,
     AssociateApiResponseTypeDef,
-    CreateApiCacheResponseTypeDef,
-    CreateApiKeyResponseTypeDef,
     GetApiAssociationResponseTypeDef,
+    CreateApiCacheResponseTypeDef,
     GetApiCacheResponseTypeDef,
-    GetIntrospectionSchemaResponseTypeDef,
-    GetSchemaCreationStatusResponseTypeDef,
-    ListApiKeysResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartSchemaCreationResponseTypeDef,
     UpdateApiCacheResponseTypeDef,
+    CreateApiKeyResponseTypeDef,
+    ListApiKeysResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
+    EvaluateCodeRequestRequestTypeDef,
+    AssociateMergedGraphqlApiRequestRequestTypeDef,
+    AssociateSourceGraphqlApiRequestRequestTypeDef,
+    SourceApiAssociationTypeDef,
+    UpdateSourceApiAssociationRequestRequestTypeDef,
     AuthorizationConfigTypeDef,
     CodeErrorTypeDef,
     CreateDomainNameResponseTypeDef,
     GetDomainNameResponseTypeDef,
     ListDomainNamesResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateTypeResponseTypeDef,
     GetTypeResponseTypeDef,
+    ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     UpdateTypeResponseTypeDef,
     DynamodbDataSourceConfigTypeDef,
     EvaluateMappingTemplateResponseTypeDef,
     SyncConfigTypeDef,
-    ListApiKeysRequestListApiKeysPaginateTypeDef,
-    ListDataSourcesRequestListDataSourcesPaginateTypeDef,
-    ListFunctionsRequestListFunctionsPaginateTypeDef,
-    ListGraphqlApisRequestListGraphqlApisPaginateTypeDef,
-    ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
-    ListResolversRequestListResolversPaginateTypeDef,
-    ListTypesRequestListTypesPaginateTypeDef,
+    ListSourceApiAssociationsResponseTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     CreateGraphqlApiRequestRequestTypeDef,
     GraphqlApiTypeDef,
     UpdateGraphqlApiRequestRequestTypeDef,
+    AssociateMergedGraphqlApiResponseTypeDef,
+    AssociateSourceGraphqlApiResponseTypeDef,
+    GetSourceApiAssociationResponseTypeDef,
+    UpdateSourceApiAssociationResponseTypeDef,
     HttpDataSourceConfigTypeDef,
     EvaluateCodeErrorDetailTypeDef,
     CreateFunctionRequestRequestTypeDef,
     CreateResolverRequestRequestTypeDef,
     FunctionConfigurationTypeDef,
     ResolverTypeDef,
     UpdateFunctionRequestRequestTypeDef,
@@ -505,42 +531,42 @@
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

### Comparing `mypy-boto3-appsync-1.26.61/README.md` & `mypy-boto3-appsync-1.27.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-appsync"></a>
 
 # mypy-boto3-appsync
 
 [![PyPI - mypy-boto3-appsync](https://img.shields.io/pypi/v/mypy-boto3-appsync.svg?color=blue)](https://pypi.org/project/mypy-boto3-appsync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appsync.svg?color=blue)](https://pypi.org/project/mypy-boto3-appsync)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appsync?color=blue)](https://pypistats.org/packages/mypy-boto3-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppSync 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
+[boto3.AppSync 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appsync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,26 +291,31 @@
     AuthenticationTypeType,
     AuthorizationTypeType,
     ConflictDetectionTypeType,
     ConflictHandlerTypeType,
     DataSourceTypeType,
     DefaultActionType,
     FieldLogLevelType,
+    GraphQLApiTypeType,
+    GraphQLApiVisibilityType,
     ListApiKeysPaginatorName,
     ListDataSourcesPaginatorName,
     ListFunctionsPaginatorName,
     ListGraphqlApisPaginatorName,
     ListResolversByFunctionPaginatorName,
     ListResolversPaginatorName,
     ListTypesPaginatorName,
+    MergeTypeType,
     OutputTypeType,
+    OwnershipType,
     RelationalDatabaseSourceTypeType,
     ResolverKindType,
     RuntimeNameType,
     SchemaStatusType,
+    SourceApiAssociationStatusType,
     TypeDefinitionFormatType,
     AppSyncServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -333,15 +338,15 @@
     LambdaAuthorizerConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     ApiAssociationTypeDef,
     ApiCacheTypeDef,
     ApiKeyTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    SourceApiAssociationConfigTypeDef,
     AwsIamConfigTypeDef,
     CachingConfigTypeDef,
     CodeErrorLocationTypeDef,
     CreateApiCacheRequestRequestTypeDef,
     CreateApiKeyRequestRequestTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
     EventBridgeDataSourceConfigTypeDef,
@@ -360,84 +365,105 @@
     DeleteDomainNameRequestRequestTypeDef,
     DeleteFunctionRequestRequestTypeDef,
     DeleteGraphqlApiRequestRequestTypeDef,
     DeleteResolverRequestRequestTypeDef,
     DeleteTypeRequestRequestTypeDef,
     DeltaSyncConfigTypeDef,
     DisassociateApiRequestRequestTypeDef,
+    DisassociateMergedGraphqlApiRequestRequestTypeDef,
+    DisassociateMergedGraphqlApiResponseTypeDef,
+    DisassociateSourceGraphqlApiRequestRequestTypeDef,
+    DisassociateSourceGraphqlApiResponseTypeDef,
     ErrorDetailTypeDef,
     EvaluateMappingTemplateRequestRequestTypeDef,
     FlushApiCacheRequestRequestTypeDef,
     GetApiAssociationRequestRequestTypeDef,
     GetApiCacheRequestRequestTypeDef,
     GetDataSourceRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
     GetGraphqlApiRequestRequestTypeDef,
     GetIntrospectionSchemaRequestRequestTypeDef,
+    GetIntrospectionSchemaResponseTypeDef,
     GetResolverRequestRequestTypeDef,
     GetSchemaCreationStatusRequestRequestTypeDef,
+    GetSchemaCreationStatusResponseTypeDef,
+    GetSourceApiAssociationRequestRequestTypeDef,
     GetTypeRequestRequestTypeDef,
     LambdaConflictHandlerConfigTypeDef,
-    PaginatorConfigTypeDef,
+    ListApiKeysRequestListApiKeysPaginateTypeDef,
     ListApiKeysRequestRequestTypeDef,
+    ListDataSourcesRequestListDataSourcesPaginateTypeDef,
     ListDataSourcesRequestRequestTypeDef,
     ListDomainNamesRequestRequestTypeDef,
+    ListFunctionsRequestListFunctionsPaginateTypeDef,
     ListFunctionsRequestRequestTypeDef,
+    ListGraphqlApisRequestListGraphqlApisPaginateTypeDef,
     ListGraphqlApisRequestRequestTypeDef,
+    ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
     ListResolversByFunctionRequestRequestTypeDef,
+    ListResolversRequestListResolversPaginateTypeDef,
     ListResolversRequestRequestTypeDef,
+    ListSourceApiAssociationsRequestRequestTypeDef,
+    SourceApiAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTypesByAssociationRequestRequestTypeDef,
+    ListTypesRequestListTypesPaginateTypeDef,
     ListTypesRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     RdsHttpEndpointConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartSchemaCreationRequestRequestTypeDef,
+    StartSchemaCreationResponseTypeDef,
+    StartSchemaMergeRequestRequestTypeDef,
+    StartSchemaMergeResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiCacheRequestRequestTypeDef,
     UpdateApiKeyRequestRequestTypeDef,
     UpdateDomainNameRequestRequestTypeDef,
     UpdateTypeRequestRequestTypeDef,
     AdditionalAuthenticationProviderTypeDef,
-    EvaluateCodeRequestRequestTypeDef,
     AssociateApiResponseTypeDef,
-    CreateApiCacheResponseTypeDef,
-    CreateApiKeyResponseTypeDef,
     GetApiAssociationResponseTypeDef,
+    CreateApiCacheResponseTypeDef,
     GetApiCacheResponseTypeDef,
-    GetIntrospectionSchemaResponseTypeDef,
-    GetSchemaCreationStatusResponseTypeDef,
-    ListApiKeysResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartSchemaCreationResponseTypeDef,
     UpdateApiCacheResponseTypeDef,
+    CreateApiKeyResponseTypeDef,
+    ListApiKeysResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
+    EvaluateCodeRequestRequestTypeDef,
+    AssociateMergedGraphqlApiRequestRequestTypeDef,
+    AssociateSourceGraphqlApiRequestRequestTypeDef,
+    SourceApiAssociationTypeDef,
+    UpdateSourceApiAssociationRequestRequestTypeDef,
     AuthorizationConfigTypeDef,
     CodeErrorTypeDef,
     CreateDomainNameResponseTypeDef,
     GetDomainNameResponseTypeDef,
     ListDomainNamesResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateTypeResponseTypeDef,
     GetTypeResponseTypeDef,
+    ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     UpdateTypeResponseTypeDef,
     DynamodbDataSourceConfigTypeDef,
     EvaluateMappingTemplateResponseTypeDef,
     SyncConfigTypeDef,
-    ListApiKeysRequestListApiKeysPaginateTypeDef,
-    ListDataSourcesRequestListDataSourcesPaginateTypeDef,
-    ListFunctionsRequestListFunctionsPaginateTypeDef,
-    ListGraphqlApisRequestListGraphqlApisPaginateTypeDef,
-    ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
-    ListResolversRequestListResolversPaginateTypeDef,
-    ListTypesRequestListTypesPaginateTypeDef,
+    ListSourceApiAssociationsResponseTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     CreateGraphqlApiRequestRequestTypeDef,
     GraphqlApiTypeDef,
     UpdateGraphqlApiRequestRequestTypeDef,
+    AssociateMergedGraphqlApiResponseTypeDef,
+    AssociateSourceGraphqlApiResponseTypeDef,
+    GetSourceApiAssociationResponseTypeDef,
+    UpdateSourceApiAssociationResponseTypeDef,
     HttpDataSourceConfigTypeDef,
     EvaluateCodeErrorDetailTypeDef,
     CreateFunctionRequestRequestTypeDef,
     CreateResolverRequestRequestTypeDef,
     FunctionConfigurationTypeDef,
     ResolverTypeDef,
     UpdateFunctionRequestRequestTypeDef,
@@ -473,42 +499,42 @@
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

### Comparing `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/__init__.py` & `mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/__init__.pyi` & `mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/__main__.py` & `mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppSync 1.26.61\nVersion:         1.26.61\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.AppSync 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.61")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/client.py` & `mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 from botocore.response import StreamingBody
 
 from .literals import (
     ApiCacheTypeType,
     ApiCachingBehaviorType,
     AuthenticationTypeType,
     DataSourceTypeType,
+    GraphQLApiTypeType,
+    GraphQLApiVisibilityType,
     OutputTypeType,
+    OwnershipType,
     ResolverKindType,
     TypeDefinitionFormatType,
 )
 from .paginator import (
     ListApiKeysPaginator,
     ListDataSourcesPaginator,
     ListFunctionsPaginator,
@@ -37,64 +40,74 @@
     ListResolversPaginator,
     ListTypesPaginator,
 )
 from .type_defs import (
     AdditionalAuthenticationProviderTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiResponseTypeDef,
+    AssociateMergedGraphqlApiResponseTypeDef,
+    AssociateSourceGraphqlApiResponseTypeDef,
     CachingConfigTypeDef,
     CreateApiCacheResponseTypeDef,
     CreateApiKeyResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateFunctionResponseTypeDef,
     CreateGraphqlApiResponseTypeDef,
     CreateResolverResponseTypeDef,
     CreateTypeResponseTypeDef,
+    DisassociateMergedGraphqlApiResponseTypeDef,
+    DisassociateSourceGraphqlApiResponseTypeDef,
     DynamodbDataSourceConfigTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
     EvaluateCodeResponseTypeDef,
     EvaluateMappingTemplateResponseTypeDef,
     EventBridgeDataSourceConfigTypeDef,
     GetApiAssociationResponseTypeDef,
     GetApiCacheResponseTypeDef,
     GetDataSourceResponseTypeDef,
     GetDomainNameResponseTypeDef,
     GetFunctionResponseTypeDef,
     GetGraphqlApiResponseTypeDef,
     GetIntrospectionSchemaResponseTypeDef,
     GetResolverResponseTypeDef,
     GetSchemaCreationStatusResponseTypeDef,
+    GetSourceApiAssociationResponseTypeDef,
     GetTypeResponseTypeDef,
     HttpDataSourceConfigTypeDef,
     LambdaAuthorizerConfigTypeDef,
     LambdaDataSourceConfigTypeDef,
     ListApiKeysResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListDomainNamesResponseTypeDef,
     ListFunctionsResponseTypeDef,
     ListGraphqlApisResponseTypeDef,
     ListResolversByFunctionResponseTypeDef,
     ListResolversResponseTypeDef,
+    ListSourceApiAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     LogConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     OpenSearchServiceDataSourceConfigTypeDef,
     PipelineConfigTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
+    SourceApiAssociationConfigTypeDef,
     StartSchemaCreationResponseTypeDef,
+    StartSchemaMergeResponseTypeDef,
     SyncConfigTypeDef,
     UpdateApiCacheResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
     UpdateDataSourceResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     UpdateFunctionResponseTypeDef,
     UpdateGraphqlApiResponseTypeDef,
     UpdateResolverResponseTypeDef,
+    UpdateSourceApiAssociationResponseTypeDef,
     UpdateTypeResponseTypeDef,
     UserPoolConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -148,14 +161,46 @@
         """
         Maps an endpoint to your custom domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.associate_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#associate_api)
         """
 
+    def associate_merged_graphql_api(
+        self,
+        *,
+        sourceApiIdentifier: str,
+        mergedApiIdentifier: str,
+        description: str = ...,
+        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...
+    ) -> AssociateMergedGraphqlApiResponseTypeDef:
+        """
+        Creates an association between a Merged API and source API using the source
+        API's identifier.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.associate_merged_graphql_api)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#associate_merged_graphql_api)
+        """
+
+    def associate_source_graphql_api(
+        self,
+        *,
+        mergedApiIdentifier: str,
+        sourceApiIdentifier: str,
+        description: str = ...,
+        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...
+    ) -> AssociateSourceGraphqlApiResponseTypeDef:
+        """
+        Creates an association between a Merged API and source API using the Merged
+        API's identifier.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.associate_source_graphql_api)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#associate_source_graphql_api)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#can_paginate)
         """
@@ -257,15 +302,19 @@
         authenticationType: AuthenticationTypeType,
         logConfig: LogConfigTypeDef = ...,
         userPoolConfig: UserPoolConfigTypeDef = ...,
         openIDConnectConfig: OpenIDConnectConfigTypeDef = ...,
         tags: Mapping[str, str] = ...,
         additionalAuthenticationProviders: Sequence[AdditionalAuthenticationProviderTypeDef] = ...,
         xrayEnabled: bool = ...,
-        lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...
+        lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...,
+        visibility: GraphQLApiVisibilityType = ...,
+        apiType: GraphQLApiTypeType = ...,
+        mergedApiExecutionRoleArn: str = ...,
+        ownerContact: str = ...
     ) -> CreateGraphqlApiResponseTypeDef:
         """
         Creates a `GraphqlApi` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_graphql_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#create_graphql_api)
         """
@@ -334,15 +383,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.delete_domain_name)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#delete_domain_name)
         """
 
     def delete_function(self, *, apiId: str, functionId: str) -> Dict[str, Any]:
         """
-        Deletes a `Function` .
+        Deletes a `Function`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.delete_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#delete_function)
         """
 
     def delete_graphql_api(self, *, apiId: str) -> Dict[str, Any]:
         """
@@ -372,14 +421,36 @@
         """
         Removes an `ApiAssociation` object from a custom domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.disassociate_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#disassociate_api)
         """
 
+    def disassociate_merged_graphql_api(
+        self, *, sourceApiIdentifier: str, associationId: str
+    ) -> DisassociateMergedGraphqlApiResponseTypeDef:
+        """
+        Deletes an association between a Merged API and source API using the source
+        API's identifier and the association ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.disassociate_merged_graphql_api)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#disassociate_merged_graphql_api)
+        """
+
+    def disassociate_source_graphql_api(
+        self, *, mergedApiIdentifier: str, associationId: str
+    ) -> DisassociateSourceGraphqlApiResponseTypeDef:
+        """
+        Deletes an association between a Merged API and source API using the Merged
+        API's identifier and the association ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.disassociate_source_graphql_api)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#disassociate_source_graphql_api)
+        """
+
     def evaluate_code(
         self, *, runtime: AppSyncRuntimeTypeDef, code: str, context: str, function: str = ...
     ) -> EvaluateCodeResponseTypeDef:
         """
         Evaluates the given code and returns the response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.evaluate_code)
@@ -448,15 +519,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_domain_name)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#get_domain_name)
         """
 
     def get_function(self, *, apiId: str, functionId: str) -> GetFunctionResponseTypeDef:
         """
-        Get a `Function` .
+        Get a `Function`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#get_function)
         """
 
     def get_graphql_api(self, *, apiId: str) -> GetGraphqlApiResponseTypeDef:
         """
@@ -490,14 +561,24 @@
         """
         Retrieves the current status of a schema creation operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_schema_creation_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#get_schema_creation_status)
         """
 
+    def get_source_api_association(
+        self, *, mergedApiIdentifier: str, associationId: str
+    ) -> GetSourceApiAssociationResponseTypeDef:
+        """
+        Retrieves a `SourceApiAssociation` object.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_source_api_association)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#get_source_api_association)
+        """
+
     def get_type(
         self, *, apiId: str, typeName: str, format: TypeDefinitionFormatType
     ) -> GetTypeResponseTypeDef:
         """
         Retrieves a `Type` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_type)
@@ -541,15 +622,20 @@
         List multiple functions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_functions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_functions)
         """
 
     def list_graphql_apis(
-        self, *, nextToken: str = ..., maxResults: int = ...
+        self,
+        *,
+        nextToken: str = ...,
+        maxResults: int = ...,
+        apiType: GraphQLApiTypeType = ...,
+        owner: OwnershipType = ...
     ) -> ListGraphqlApisResponseTypeDef:
         """
         Lists your GraphQL APIs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_graphql_apis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_graphql_apis)
         """
@@ -570,14 +656,24 @@
         """
         List the resolvers that are associated with a specific function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_resolvers_by_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_resolvers_by_function)
         """
 
+    def list_source_api_associations(
+        self, *, apiId: str, nextToken: str = ..., maxResults: int = ...
+    ) -> ListSourceApiAssociationsResponseTypeDef:
+        """
+        Lists the `SourceApiAssociationSummary` data.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_source_api_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_source_api_associations)
+        """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_tags_for_resource)
         """
@@ -593,24 +689,50 @@
         """
         Lists the types for a given API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_types)
         """
 
+    def list_types_by_association(
+        self,
+        *,
+        mergedApiIdentifier: str,
+        associationId: str,
+        format: TypeDefinitionFormatType,
+        nextToken: str = ...,
+        maxResults: int = ...
+    ) -> ListTypesByAssociationResponseTypeDef:
+        """
+        Lists `Type` objects by the source API association ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_types_by_association)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_types_by_association)
+        """
+
     def start_schema_creation(
         self, *, apiId: str, definition: Union[str, bytes, IO[Any], StreamingBody]
     ) -> StartSchemaCreationResponseTypeDef:
         """
         Adds a new schema to your GraphQL API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.start_schema_creation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#start_schema_creation)
         """
 
+    def start_schema_merge(
+        self, *, associationId: str, mergedApiIdentifier: str
+    ) -> StartSchemaMergeResponseTypeDef:
+        """
+        Initiates a merge operation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.start_schema_merge)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#start_schema_merge)
+        """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Tags a resource with user-supplied tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#tag_resource)
         """
@@ -711,15 +833,17 @@
         name: str,
         logConfig: LogConfigTypeDef = ...,
         authenticationType: AuthenticationTypeType = ...,
         userPoolConfig: UserPoolConfigTypeDef = ...,
         openIDConnectConfig: OpenIDConnectConfigTypeDef = ...,
         additionalAuthenticationProviders: Sequence[AdditionalAuthenticationProviderTypeDef] = ...,
         xrayEnabled: bool = ...,
-        lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...
+        lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...,
+        mergedApiExecutionRoleArn: str = ...,
+        ownerContact: str = ...
     ) -> UpdateGraphqlApiResponseTypeDef:
         """
         Updates a `GraphqlApi` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_graphql_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#update_graphql_api)
         """
@@ -744,14 +868,30 @@
         """
         Updates a `Resolver` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_resolver)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#update_resolver)
         """
 
+    def update_source_api_association(
+        self,
+        *,
+        associationId: str,
+        mergedApiIdentifier: str,
+        description: str = ...,
+        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...
+    ) -> UpdateSourceApiAssociationResponseTypeDef:
+        """
+        Updates some of the configuration choices of a particular source API
+        association.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_source_api_association)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#update_source_api_association)
+        """
+
     def update_type(
         self, *, apiId: str, typeName: str, format: TypeDefinitionFormatType, definition: str = ...
     ) -> UpdateTypeResponseTypeDef:
         """
         Updates a `Type` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_type)
```

### Comparing `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/client.pyi` & `mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/client.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 from botocore.response import StreamingBody
 
 from .literals import (
     ApiCacheTypeType,
     ApiCachingBehaviorType,
     AuthenticationTypeType,
     DataSourceTypeType,
+    GraphQLApiTypeType,
+    GraphQLApiVisibilityType,
     OutputTypeType,
+    OwnershipType,
     ResolverKindType,
     TypeDefinitionFormatType,
 )
 from .paginator import (
     ListApiKeysPaginator,
     ListDataSourcesPaginator,
     ListFunctionsPaginator,
@@ -37,64 +40,74 @@
     ListResolversPaginator,
     ListTypesPaginator,
 )
 from .type_defs import (
     AdditionalAuthenticationProviderTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiResponseTypeDef,
+    AssociateMergedGraphqlApiResponseTypeDef,
+    AssociateSourceGraphqlApiResponseTypeDef,
     CachingConfigTypeDef,
     CreateApiCacheResponseTypeDef,
     CreateApiKeyResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateFunctionResponseTypeDef,
     CreateGraphqlApiResponseTypeDef,
     CreateResolverResponseTypeDef,
     CreateTypeResponseTypeDef,
+    DisassociateMergedGraphqlApiResponseTypeDef,
+    DisassociateSourceGraphqlApiResponseTypeDef,
     DynamodbDataSourceConfigTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
     EvaluateCodeResponseTypeDef,
     EvaluateMappingTemplateResponseTypeDef,
     EventBridgeDataSourceConfigTypeDef,
     GetApiAssociationResponseTypeDef,
     GetApiCacheResponseTypeDef,
     GetDataSourceResponseTypeDef,
     GetDomainNameResponseTypeDef,
     GetFunctionResponseTypeDef,
     GetGraphqlApiResponseTypeDef,
     GetIntrospectionSchemaResponseTypeDef,
     GetResolverResponseTypeDef,
     GetSchemaCreationStatusResponseTypeDef,
+    GetSourceApiAssociationResponseTypeDef,
     GetTypeResponseTypeDef,
     HttpDataSourceConfigTypeDef,
     LambdaAuthorizerConfigTypeDef,
     LambdaDataSourceConfigTypeDef,
     ListApiKeysResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListDomainNamesResponseTypeDef,
     ListFunctionsResponseTypeDef,
     ListGraphqlApisResponseTypeDef,
     ListResolversByFunctionResponseTypeDef,
     ListResolversResponseTypeDef,
+    ListSourceApiAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     LogConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     OpenSearchServiceDataSourceConfigTypeDef,
     PipelineConfigTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
+    SourceApiAssociationConfigTypeDef,
     StartSchemaCreationResponseTypeDef,
+    StartSchemaMergeResponseTypeDef,
     SyncConfigTypeDef,
     UpdateApiCacheResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
     UpdateDataSourceResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     UpdateFunctionResponseTypeDef,
     UpdateGraphqlApiResponseTypeDef,
     UpdateResolverResponseTypeDef,
+    UpdateSourceApiAssociationResponseTypeDef,
     UpdateTypeResponseTypeDef,
     UserPoolConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -142,14 +155,44 @@
     def associate_api(self, *, domainName: str, apiId: str) -> AssociateApiResponseTypeDef:
         """
         Maps an endpoint to your custom domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.associate_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#associate_api)
         """
+    def associate_merged_graphql_api(
+        self,
+        *,
+        sourceApiIdentifier: str,
+        mergedApiIdentifier: str,
+        description: str = ...,
+        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...
+    ) -> AssociateMergedGraphqlApiResponseTypeDef:
+        """
+        Creates an association between a Merged API and source API using the source
+        API's identifier.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.associate_merged_graphql_api)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#associate_merged_graphql_api)
+        """
+    def associate_source_graphql_api(
+        self,
+        *,
+        mergedApiIdentifier: str,
+        sourceApiIdentifier: str,
+        description: str = ...,
+        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...
+    ) -> AssociateSourceGraphqlApiResponseTypeDef:
+        """
+        Creates an association between a Merged API and source API using the Merged
+        API's identifier.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.associate_source_graphql_api)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#associate_source_graphql_api)
+        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#can_paginate)
         """
@@ -244,15 +287,19 @@
         authenticationType: AuthenticationTypeType,
         logConfig: LogConfigTypeDef = ...,
         userPoolConfig: UserPoolConfigTypeDef = ...,
         openIDConnectConfig: OpenIDConnectConfigTypeDef = ...,
         tags: Mapping[str, str] = ...,
         additionalAuthenticationProviders: Sequence[AdditionalAuthenticationProviderTypeDef] = ...,
         xrayEnabled: bool = ...,
-        lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...
+        lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...,
+        visibility: GraphQLApiVisibilityType = ...,
+        apiType: GraphQLApiTypeType = ...,
+        mergedApiExecutionRoleArn: str = ...,
+        ownerContact: str = ...
     ) -> CreateGraphqlApiResponseTypeDef:
         """
         Creates a `GraphqlApi` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_graphql_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#create_graphql_api)
         """
@@ -314,15 +361,15 @@
         Deletes a custom `DomainName` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.delete_domain_name)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#delete_domain_name)
         """
     def delete_function(self, *, apiId: str, functionId: str) -> Dict[str, Any]:
         """
-        Deletes a `Function` .
+        Deletes a `Function`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.delete_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#delete_function)
         """
     def delete_graphql_api(self, *, apiId: str) -> Dict[str, Any]:
         """
         Deletes a `GraphqlApi` object.
@@ -347,14 +394,34 @@
     def disassociate_api(self, *, domainName: str) -> Dict[str, Any]:
         """
         Removes an `ApiAssociation` object from a custom domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.disassociate_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#disassociate_api)
         """
+    def disassociate_merged_graphql_api(
+        self, *, sourceApiIdentifier: str, associationId: str
+    ) -> DisassociateMergedGraphqlApiResponseTypeDef:
+        """
+        Deletes an association between a Merged API and source API using the source
+        API's identifier and the association ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.disassociate_merged_graphql_api)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#disassociate_merged_graphql_api)
+        """
+    def disassociate_source_graphql_api(
+        self, *, mergedApiIdentifier: str, associationId: str
+    ) -> DisassociateSourceGraphqlApiResponseTypeDef:
+        """
+        Deletes an association between a Merged API and source API using the Merged
+        API's identifier and the association ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.disassociate_source_graphql_api)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#disassociate_source_graphql_api)
+        """
     def evaluate_code(
         self, *, runtime: AppSyncRuntimeTypeDef, code: str, context: str, function: str = ...
     ) -> EvaluateCodeResponseTypeDef:
         """
         Evaluates the given code and returns the response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.evaluate_code)
@@ -415,15 +482,15 @@
         Retrieves a custom `DomainName` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_domain_name)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#get_domain_name)
         """
     def get_function(self, *, apiId: str, functionId: str) -> GetFunctionResponseTypeDef:
         """
-        Get a `Function` .
+        Get a `Function`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#get_function)
         """
     def get_graphql_api(self, *, apiId: str) -> GetGraphqlApiResponseTypeDef:
         """
         Retrieves a `GraphqlApi` object.
@@ -452,14 +519,23 @@
     def get_schema_creation_status(self, *, apiId: str) -> GetSchemaCreationStatusResponseTypeDef:
         """
         Retrieves the current status of a schema creation operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_schema_creation_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#get_schema_creation_status)
         """
+    def get_source_api_association(
+        self, *, mergedApiIdentifier: str, associationId: str
+    ) -> GetSourceApiAssociationResponseTypeDef:
+        """
+        Retrieves a `SourceApiAssociation` object.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_source_api_association)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#get_source_api_association)
+        """
     def get_type(
         self, *, apiId: str, typeName: str, format: TypeDefinitionFormatType
     ) -> GetTypeResponseTypeDef:
         """
         Retrieves a `Type` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_type)
@@ -498,15 +574,20 @@
         """
         List multiple functions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_functions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_functions)
         """
     def list_graphql_apis(
-        self, *, nextToken: str = ..., maxResults: int = ...
+        self,
+        *,
+        nextToken: str = ...,
+        maxResults: int = ...,
+        apiType: GraphQLApiTypeType = ...,
+        owner: OwnershipType = ...
     ) -> ListGraphqlApisResponseTypeDef:
         """
         Lists your GraphQL APIs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_graphql_apis)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_graphql_apis)
         """
@@ -524,14 +605,23 @@
     ) -> ListResolversByFunctionResponseTypeDef:
         """
         List the resolvers that are associated with a specific function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_resolvers_by_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_resolvers_by_function)
         """
+    def list_source_api_associations(
+        self, *, apiId: str, nextToken: str = ..., maxResults: int = ...
+    ) -> ListSourceApiAssociationsResponseTypeDef:
+        """
+        Lists the `SourceApiAssociationSummary` data.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_source_api_associations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_source_api_associations)
+        """
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_tags_for_resource)
         """
@@ -545,23 +635,47 @@
     ) -> ListTypesResponseTypeDef:
         """
         Lists the types for a given API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_types)
         """
+    def list_types_by_association(
+        self,
+        *,
+        mergedApiIdentifier: str,
+        associationId: str,
+        format: TypeDefinitionFormatType,
+        nextToken: str = ...,
+        maxResults: int = ...
+    ) -> ListTypesByAssociationResponseTypeDef:
+        """
+        Lists `Type` objects by the source API association ID.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_types_by_association)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#list_types_by_association)
+        """
     def start_schema_creation(
         self, *, apiId: str, definition: Union[str, bytes, IO[Any], StreamingBody]
     ) -> StartSchemaCreationResponseTypeDef:
         """
         Adds a new schema to your GraphQL API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.start_schema_creation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#start_schema_creation)
         """
+    def start_schema_merge(
+        self, *, associationId: str, mergedApiIdentifier: str
+    ) -> StartSchemaMergeResponseTypeDef:
+        """
+        Initiates a merge operation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.start_schema_merge)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#start_schema_merge)
+        """
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Tags a resource with user-supplied tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#tag_resource)
         """
@@ -655,15 +769,17 @@
         name: str,
         logConfig: LogConfigTypeDef = ...,
         authenticationType: AuthenticationTypeType = ...,
         userPoolConfig: UserPoolConfigTypeDef = ...,
         openIDConnectConfig: OpenIDConnectConfigTypeDef = ...,
         additionalAuthenticationProviders: Sequence[AdditionalAuthenticationProviderTypeDef] = ...,
         xrayEnabled: bool = ...,
-        lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...
+        lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...,
+        mergedApiExecutionRoleArn: str = ...,
+        ownerContact: str = ...
     ) -> UpdateGraphqlApiResponseTypeDef:
         """
         Updates a `GraphqlApi` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_graphql_api)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#update_graphql_api)
         """
@@ -686,14 +802,29 @@
     ) -> UpdateResolverResponseTypeDef:
         """
         Updates a `Resolver` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_resolver)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#update_resolver)
         """
+    def update_source_api_association(
+        self,
+        *,
+        associationId: str,
+        mergedApiIdentifier: str,
+        description: str = ...,
+        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...
+    ) -> UpdateSourceApiAssociationResponseTypeDef:
+        """
+        Updates some of the configuration choices of a particular source API
+        association.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_source_api_association)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#update_source_api_association)
+        """
     def update_type(
         self, *, apiId: str, typeName: str, format: TypeDefinitionFormatType, definition: str = ...
     ) -> UpdateTypeResponseTypeDef:
         """
         Updates a `Type` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_type)
```

### Comparing `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/literals.py` & `mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,26 +27,31 @@
     "AuthenticationTypeType",
     "AuthorizationTypeType",
     "ConflictDetectionTypeType",
     "ConflictHandlerTypeType",
     "DataSourceTypeType",
     "DefaultActionType",
     "FieldLogLevelType",
+    "GraphQLApiTypeType",
+    "GraphQLApiVisibilityType",
     "ListApiKeysPaginatorName",
     "ListDataSourcesPaginatorName",
     "ListFunctionsPaginatorName",
     "ListGraphqlApisPaginatorName",
     "ListResolversByFunctionPaginatorName",
     "ListResolversPaginatorName",
     "ListTypesPaginatorName",
+    "MergeTypeType",
     "OutputTypeType",
+    "OwnershipType",
     "RelationalDatabaseSourceTypeType",
     "ResolverKindType",
     "RuntimeNameType",
     "SchemaStatusType",
+    "SourceApiAssociationStatusType",
     "TypeDefinitionFormatType",
     "AppSyncServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
@@ -86,28 +91,42 @@
     "AWS_LAMBDA",
     "HTTP",
     "NONE",
     "RELATIONAL_DATABASE",
 ]
 DefaultActionType = Literal["ALLOW", "DENY"]
 FieldLogLevelType = Literal["ALL", "ERROR", "NONE"]
+GraphQLApiTypeType = Literal["GRAPHQL", "MERGED"]
+GraphQLApiVisibilityType = Literal["GLOBAL", "PRIVATE"]
 ListApiKeysPaginatorName = Literal["list_api_keys"]
 ListDataSourcesPaginatorName = Literal["list_data_sources"]
 ListFunctionsPaginatorName = Literal["list_functions"]
 ListGraphqlApisPaginatorName = Literal["list_graphql_apis"]
 ListResolversByFunctionPaginatorName = Literal["list_resolvers_by_function"]
 ListResolversPaginatorName = Literal["list_resolvers"]
 ListTypesPaginatorName = Literal["list_types"]
+MergeTypeType = Literal["AUTO_MERGE", "MANUAL_MERGE"]
 OutputTypeType = Literal["JSON", "SDL"]
+OwnershipType = Literal["CURRENT_ACCOUNT", "OTHER_ACCOUNTS"]
 RelationalDatabaseSourceTypeType = Literal["RDS_HTTP_ENDPOINT"]
 ResolverKindType = Literal["PIPELINE", "UNIT"]
 RuntimeNameType = Literal["APPSYNC_JS"]
 SchemaStatusType = Literal[
     "ACTIVE", "DELETING", "FAILED", "NOT_APPLICABLE", "PROCESSING", "SUCCESS"
 ]
+SourceApiAssociationStatusType = Literal[
+    "AUTO_MERGE_SCHEDULE_FAILED",
+    "DELETION_FAILED",
+    "DELETION_IN_PROGRESS",
+    "DELETION_SCHEDULED",
+    "MERGE_FAILED",
+    "MERGE_IN_PROGRESS",
+    "MERGE_SCHEDULED",
+    "MERGE_SUCCESS",
+]
 TypeDefinitionFormatType = Literal["JSON", "SDL"]
 AppSyncServiceName = Literal["appsync"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -117,14 +136,15 @@
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
@@ -164,14 +184,15 @@
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
@@ -250,14 +271,15 @@
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
@@ -268,14 +290,15 @@
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
@@ -311,14 +334,15 @@
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
@@ -337,16 +361,19 @@
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
@@ -426,18 +453,21 @@
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
@@ -471,24 +501,28 @@
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
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/literals.pyi` & `mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -26,26 +26,31 @@
     "AuthenticationTypeType",
     "AuthorizationTypeType",
     "ConflictDetectionTypeType",
     "ConflictHandlerTypeType",
     "DataSourceTypeType",
     "DefaultActionType",
     "FieldLogLevelType",
+    "GraphQLApiTypeType",
+    "GraphQLApiVisibilityType",
     "ListApiKeysPaginatorName",
     "ListDataSourcesPaginatorName",
     "ListFunctionsPaginatorName",
     "ListGraphqlApisPaginatorName",
     "ListResolversByFunctionPaginatorName",
     "ListResolversPaginatorName",
     "ListTypesPaginatorName",
+    "MergeTypeType",
     "OutputTypeType",
+    "OwnershipType",
     "RelationalDatabaseSourceTypeType",
     "ResolverKindType",
     "RuntimeNameType",
     "SchemaStatusType",
+    "SourceApiAssociationStatusType",
     "TypeDefinitionFormatType",
     "AppSyncServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
@@ -84,28 +89,42 @@
     "AWS_LAMBDA",
     "HTTP",
     "NONE",
     "RELATIONAL_DATABASE",
 ]
 DefaultActionType = Literal["ALLOW", "DENY"]
 FieldLogLevelType = Literal["ALL", "ERROR", "NONE"]
+GraphQLApiTypeType = Literal["GRAPHQL", "MERGED"]
+GraphQLApiVisibilityType = Literal["GLOBAL", "PRIVATE"]
 ListApiKeysPaginatorName = Literal["list_api_keys"]
 ListDataSourcesPaginatorName = Literal["list_data_sources"]
 ListFunctionsPaginatorName = Literal["list_functions"]
 ListGraphqlApisPaginatorName = Literal["list_graphql_apis"]
 ListResolversByFunctionPaginatorName = Literal["list_resolvers_by_function"]
 ListResolversPaginatorName = Literal["list_resolvers"]
 ListTypesPaginatorName = Literal["list_types"]
+MergeTypeType = Literal["AUTO_MERGE", "MANUAL_MERGE"]
 OutputTypeType = Literal["JSON", "SDL"]
+OwnershipType = Literal["CURRENT_ACCOUNT", "OTHER_ACCOUNTS"]
 RelationalDatabaseSourceTypeType = Literal["RDS_HTTP_ENDPOINT"]
 ResolverKindType = Literal["PIPELINE", "UNIT"]
 RuntimeNameType = Literal["APPSYNC_JS"]
 SchemaStatusType = Literal[
     "ACTIVE", "DELETING", "FAILED", "NOT_APPLICABLE", "PROCESSING", "SUCCESS"
 ]
+SourceApiAssociationStatusType = Literal[
+    "AUTO_MERGE_SCHEDULE_FAILED",
+    "DELETION_FAILED",
+    "DELETION_IN_PROGRESS",
+    "DELETION_SCHEDULED",
+    "MERGE_FAILED",
+    "MERGE_IN_PROGRESS",
+    "MERGE_SCHEDULED",
+    "MERGE_SUCCESS",
+]
 TypeDefinitionFormatType = Literal["JSON", "SDL"]
 AppSyncServiceName = Literal["appsync"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -115,14 +134,15 @@
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
@@ -162,14 +182,15 @@
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
@@ -248,14 +269,15 @@
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
@@ -266,14 +288,15 @@
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
@@ -309,14 +332,15 @@
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
@@ -335,16 +359,19 @@
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
@@ -424,18 +451,21 @@
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
@@ -469,24 +499,28 @@
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
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/paginator.py` & `mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/paginator.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     list_types_paginator: ListTypesPaginator = client.get_paginator("list_types")
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
-from .literals import TypeDefinitionFormatType
+from .literals import GraphQLApiTypeType, OwnershipType, TypeDefinitionFormatType
 from .type_defs import (
     ListApiKeysResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListFunctionsResponseTypeDef,
     ListGraphqlApisResponseTypeDef,
     ListResolversByFunctionResponseTypeDef,
     ListResolversResponseTypeDef,
@@ -71,90 +71,94 @@
 class ListApiKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListApiKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listapikeyspaginator)
     """
 
     def paginate(
-        self, *, apiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, apiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApiKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListApiKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listapikeyspaginator)
         """
 
 
 class ListDataSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListDataSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listdatasourcespaginator)
     """
 
     def paginate(
-        self, *, apiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, apiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListDataSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listdatasourcespaginator)
         """
 
 
 class ListFunctionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListFunctions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listfunctionspaginator)
     """
 
     def paginate(
-        self, *, apiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, apiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFunctionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListFunctions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listfunctionspaginator)
         """
 
 
 class ListGraphqlApisPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListGraphqlApis)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listgraphqlapispaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        apiType: GraphQLApiTypeType = ...,
+        owner: OwnershipType = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGraphqlApisResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListGraphqlApis.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listgraphqlapispaginator)
         """
 
 
 class ListResolversPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolvers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolverspaginator)
     """
 
     def paginate(
-        self, *, apiId: str, typeName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, apiId: str, typeName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResolversResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolvers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolverspaginator)
         """
 
 
 class ListResolversByFunctionPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolversByFunction)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolversbyfunctionpaginator)
     """
 
     def paginate(
-        self, *, apiId: str, functionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, apiId: str, functionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResolversByFunctionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolversByFunction.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolversbyfunctionpaginator)
         """
 
 
@@ -165,13 +169,13 @@
     """
 
     def paginate(
         self,
         *,
         apiId: str,
         format: TypeDefinitionFormatType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listtypespaginator)
         """
```

### Comparing `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/paginator.pyi` & `mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/paginator.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     list_types_paginator: ListTypesPaginator = client.get_paginator("list_types")
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
-from .literals import TypeDefinitionFormatType
+from .literals import GraphQLApiTypeType, OwnershipType, TypeDefinitionFormatType
 from .type_defs import (
     ListApiKeysResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListFunctionsResponseTypeDef,
     ListGraphqlApisResponseTypeDef,
     ListResolversByFunctionResponseTypeDef,
     ListResolversResponseTypeDef,
@@ -68,85 +68,89 @@
 class ListApiKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListApiKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listapikeyspaginator)
     """
 
     def paginate(
-        self, *, apiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, apiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApiKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListApiKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listapikeyspaginator)
         """
 
 class ListDataSourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListDataSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listdatasourcespaginator)
     """
 
     def paginate(
-        self, *, apiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, apiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListDataSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listdatasourcespaginator)
         """
 
 class ListFunctionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListFunctions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listfunctionspaginator)
     """
 
     def paginate(
-        self, *, apiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, apiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFunctionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListFunctions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listfunctionspaginator)
         """
 
 class ListGraphqlApisPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListGraphqlApis)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listgraphqlapispaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        apiType: GraphQLApiTypeType = ...,
+        owner: OwnershipType = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListGraphqlApisResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListGraphqlApis.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listgraphqlapispaginator)
         """
 
 class ListResolversPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolvers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolverspaginator)
     """
 
     def paginate(
-        self, *, apiId: str, typeName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, apiId: str, typeName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResolversResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolvers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolverspaginator)
         """
 
 class ListResolversByFunctionPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolversByFunction)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolversbyfunctionpaginator)
     """
 
     def paginate(
-        self, *, apiId: str, functionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, apiId: str, functionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResolversByFunctionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolversByFunction.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listresolversbyfunctionpaginator)
         """
 
 class ListTypesPaginator(Paginator):
@@ -156,13 +160,13 @@
     """
 
     def paginate(
         self,
         *,
         apiId: str,
         format: TypeDefinitionFormatType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/paginators/#listtypespaginator)
         """
```

### Comparing `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/type_defs.py` & `mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ```python
     from mypy_boto3_appsync.type_defs import CognitoUserPoolConfigTypeDef
 
     data: CognitoUserPoolConfigTypeDef = {...}
     ```
 """
 import sys
+from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     ApiCacheStatusType,
     ApiCacheTypeType,
@@ -23,17 +24,22 @@
     AssociationStatusType,
     AuthenticationTypeType,
     ConflictDetectionTypeType,
     ConflictHandlerTypeType,
     DataSourceTypeType,
     DefaultActionType,
     FieldLogLevelType,
+    GraphQLApiTypeType,
+    GraphQLApiVisibilityType,
+    MergeTypeType,
     OutputTypeType,
+    OwnershipType,
     ResolverKindType,
     SchemaStatusType,
+    SourceApiAssociationStatusType,
     TypeDefinitionFormatType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -48,15 +54,15 @@
     "LambdaAuthorizerConfigTypeDef",
     "OpenIDConnectConfigTypeDef",
     "ApiAssociationTypeDef",
     "ApiCacheTypeDef",
     "ApiKeyTypeDef",
     "AppSyncRuntimeTypeDef",
     "AssociateApiRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "SourceApiAssociationConfigTypeDef",
     "AwsIamConfigTypeDef",
     "CachingConfigTypeDef",
     "CodeErrorLocationTypeDef",
     "CreateApiCacheRequestRequestTypeDef",
     "CreateApiKeyRequestRequestTypeDef",
     "ElasticsearchDataSourceConfigTypeDef",
     "EventBridgeDataSourceConfigTypeDef",
@@ -75,84 +81,105 @@
     "DeleteDomainNameRequestRequestTypeDef",
     "DeleteFunctionRequestRequestTypeDef",
     "DeleteGraphqlApiRequestRequestTypeDef",
     "DeleteResolverRequestRequestTypeDef",
     "DeleteTypeRequestRequestTypeDef",
     "DeltaSyncConfigTypeDef",
     "DisassociateApiRequestRequestTypeDef",
+    "DisassociateMergedGraphqlApiRequestRequestTypeDef",
+    "DisassociateMergedGraphqlApiResponseTypeDef",
+    "DisassociateSourceGraphqlApiRequestRequestTypeDef",
+    "DisassociateSourceGraphqlApiResponseTypeDef",
     "ErrorDetailTypeDef",
     "EvaluateMappingTemplateRequestRequestTypeDef",
     "FlushApiCacheRequestRequestTypeDef",
     "GetApiAssociationRequestRequestTypeDef",
     "GetApiCacheRequestRequestTypeDef",
     "GetDataSourceRequestRequestTypeDef",
     "GetDomainNameRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
     "GetGraphqlApiRequestRequestTypeDef",
     "GetIntrospectionSchemaRequestRequestTypeDef",
+    "GetIntrospectionSchemaResponseTypeDef",
     "GetResolverRequestRequestTypeDef",
     "GetSchemaCreationStatusRequestRequestTypeDef",
+    "GetSchemaCreationStatusResponseTypeDef",
+    "GetSourceApiAssociationRequestRequestTypeDef",
     "GetTypeRequestRequestTypeDef",
     "LambdaConflictHandlerConfigTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApiKeysRequestListApiKeysPaginateTypeDef",
     "ListApiKeysRequestRequestTypeDef",
+    "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     "ListDataSourcesRequestRequestTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
+    "ListFunctionsRequestListFunctionsPaginateTypeDef",
     "ListFunctionsRequestRequestTypeDef",
+    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
     "ListGraphqlApisRequestRequestTypeDef",
+    "ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
     "ListResolversByFunctionRequestRequestTypeDef",
+    "ListResolversRequestListResolversPaginateTypeDef",
     "ListResolversRequestRequestTypeDef",
+    "ListSourceApiAssociationsRequestRequestTypeDef",
+    "SourceApiAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTypesByAssociationRequestRequestTypeDef",
+    "ListTypesRequestListTypesPaginateTypeDef",
     "ListTypesRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "RdsHttpEndpointConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StartSchemaCreationRequestRequestTypeDef",
+    "StartSchemaCreationResponseTypeDef",
+    "StartSchemaMergeRequestRequestTypeDef",
+    "StartSchemaMergeResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiCacheRequestRequestTypeDef",
     "UpdateApiKeyRequestRequestTypeDef",
     "UpdateDomainNameRequestRequestTypeDef",
     "UpdateTypeRequestRequestTypeDef",
     "AdditionalAuthenticationProviderTypeDef",
-    "EvaluateCodeRequestRequestTypeDef",
     "AssociateApiResponseTypeDef",
-    "CreateApiCacheResponseTypeDef",
-    "CreateApiKeyResponseTypeDef",
     "GetApiAssociationResponseTypeDef",
+    "CreateApiCacheResponseTypeDef",
     "GetApiCacheResponseTypeDef",
-    "GetIntrospectionSchemaResponseTypeDef",
-    "GetSchemaCreationStatusResponseTypeDef",
-    "ListApiKeysResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartSchemaCreationResponseTypeDef",
     "UpdateApiCacheResponseTypeDef",
+    "CreateApiKeyResponseTypeDef",
+    "ListApiKeysResponseTypeDef",
     "UpdateApiKeyResponseTypeDef",
+    "EvaluateCodeRequestRequestTypeDef",
+    "AssociateMergedGraphqlApiRequestRequestTypeDef",
+    "AssociateSourceGraphqlApiRequestRequestTypeDef",
+    "SourceApiAssociationTypeDef",
+    "UpdateSourceApiAssociationRequestRequestTypeDef",
     "AuthorizationConfigTypeDef",
     "CodeErrorTypeDef",
     "CreateDomainNameResponseTypeDef",
     "GetDomainNameResponseTypeDef",
     "ListDomainNamesResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateTypeResponseTypeDef",
     "GetTypeResponseTypeDef",
+    "ListTypesByAssociationResponseTypeDef",
     "ListTypesResponseTypeDef",
     "UpdateTypeResponseTypeDef",
     "DynamodbDataSourceConfigTypeDef",
     "EvaluateMappingTemplateResponseTypeDef",
     "SyncConfigTypeDef",
-    "ListApiKeysRequestListApiKeysPaginateTypeDef",
-    "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
-    "ListFunctionsRequestListFunctionsPaginateTypeDef",
-    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
-    "ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
-    "ListResolversRequestListResolversPaginateTypeDef",
-    "ListTypesRequestListTypesPaginateTypeDef",
+    "ListSourceApiAssociationsResponseTypeDef",
     "RelationalDatabaseDataSourceConfigTypeDef",
     "CreateGraphqlApiRequestRequestTypeDef",
     "GraphqlApiTypeDef",
     "UpdateGraphqlApiRequestRequestTypeDef",
+    "AssociateMergedGraphqlApiResponseTypeDef",
+    "AssociateSourceGraphqlApiResponseTypeDef",
+    "GetSourceApiAssociationResponseTypeDef",
+    "UpdateSourceApiAssociationResponseTypeDef",
     "HttpDataSourceConfigTypeDef",
     "EvaluateCodeErrorDetailTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "CreateResolverRequestRequestTypeDef",
     "FunctionConfigurationTypeDef",
     "ResolverTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
@@ -294,23 +321,20 @@
     "AssociateApiRequestRequestTypeDef",
     {
         "domainName": str,
         "apiId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+SourceApiAssociationConfigTypeDef = TypedDict(
+    "SourceApiAssociationConfigTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "mergeType": MergeTypeType,
     },
+    total=False,
 )
 
 AwsIamConfigTypeDef = TypedDict(
     "AwsIamConfigTypeDef",
     {
         "signingRegion": str,
         "signingServiceName": str,
@@ -603,14 +627,46 @@
 DisassociateApiRequestRequestTypeDef = TypedDict(
     "DisassociateApiRequestRequestTypeDef",
     {
         "domainName": str,
     },
 )
 
+DisassociateMergedGraphqlApiRequestRequestTypeDef = TypedDict(
+    "DisassociateMergedGraphqlApiRequestRequestTypeDef",
+    {
+        "sourceApiIdentifier": str,
+        "associationId": str,
+    },
+)
+
+DisassociateMergedGraphqlApiResponseTypeDef = TypedDict(
+    "DisassociateMergedGraphqlApiResponseTypeDef",
+    {
+        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DisassociateSourceGraphqlApiRequestRequestTypeDef = TypedDict(
+    "DisassociateSourceGraphqlApiRequestRequestTypeDef",
+    {
+        "mergedApiIdentifier": str,
+        "associationId": str,
+    },
+)
+
+DisassociateSourceGraphqlApiResponseTypeDef = TypedDict(
+    "DisassociateSourceGraphqlApiResponseTypeDef",
+    {
+        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "message": str,
     },
     total=False,
 )
@@ -693,14 +749,22 @@
 class GetIntrospectionSchemaRequestRequestTypeDef(
     _RequiredGetIntrospectionSchemaRequestRequestTypeDef,
     _OptionalGetIntrospectionSchemaRequestRequestTypeDef,
 ):
     pass
 
 
+GetIntrospectionSchemaResponseTypeDef = TypedDict(
+    "GetIntrospectionSchemaResponseTypeDef",
+    {
+        "schema": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetResolverRequestRequestTypeDef = TypedDict(
     "GetResolverRequestRequestTypeDef",
     {
         "apiId": str,
         "typeName": str,
         "fieldName": str,
     },
@@ -709,14 +773,31 @@
 GetSchemaCreationStatusRequestRequestTypeDef = TypedDict(
     "GetSchemaCreationStatusRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 
+GetSchemaCreationStatusResponseTypeDef = TypedDict(
+    "GetSchemaCreationStatusResponseTypeDef",
+    {
+        "status": SchemaStatusType,
+        "details": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSourceApiAssociationRequestRequestTypeDef = TypedDict(
+    "GetSourceApiAssociationRequestRequestTypeDef",
+    {
+        "mergedApiIdentifier": str,
+        "associationId": str,
+    },
+)
+
 GetTypeRequestRequestTypeDef = TypedDict(
     "GetTypeRequestRequestTypeDef",
     {
         "apiId": str,
         "typeName": str,
         "format": TypeDefinitionFormatType,
     },
@@ -726,24 +807,36 @@
     "LambdaConflictHandlerConfigTypeDef",
     {
         "lambdaConflictHandlerArn": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
+    "_RequiredListApiKeysRequestListApiKeysPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "apiId": str,
+    },
+)
+_OptionalListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
+    "_OptionalListApiKeysRequestListApiKeysPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListApiKeysRequestListApiKeysPaginateTypeDef(
+    _RequiredListApiKeysRequestListApiKeysPaginateTypeDef,
+    _OptionalListApiKeysRequestListApiKeysPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListApiKeysRequestRequestTypeDef = TypedDict(
     "_RequiredListApiKeysRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 _OptionalListApiKeysRequestRequestTypeDef = TypedDict(
@@ -758,14 +851,36 @@
 
 class ListApiKeysRequestRequestTypeDef(
     _RequiredListApiKeysRequestRequestTypeDef, _OptionalListApiKeysRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef",
+    {
+        "apiId": str,
+    },
+)
+_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDataSourcesRequestListDataSourcesPaginateTypeDef(
+    _RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef,
+    _OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDataSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSourcesRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 _OptionalListDataSourcesRequestRequestTypeDef = TypedDict(
@@ -789,14 +904,36 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionsRequestListFunctionsPaginateTypeDef",
+    {
+        "apiId": str,
+    },
+)
+_OptionalListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionsRequestListFunctionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListFunctionsRequestListFunctionsPaginateTypeDef(
+    _RequiredListFunctionsRequestListFunctionsPaginateTypeDef,
+    _OptionalListFunctionsRequestListFunctionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionsRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 _OptionalListFunctionsRequestRequestTypeDef = TypedDict(
@@ -811,23 +948,58 @@
 
 class ListFunctionsRequestRequestTypeDef(
     _RequiredListFunctionsRequestRequestTypeDef, _OptionalListFunctionsRequestRequestTypeDef
 ):
     pass
 
 
+ListGraphqlApisRequestListGraphqlApisPaginateTypeDef = TypedDict(
+    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
+    {
+        "apiType": GraphQLApiTypeType,
+        "owner": OwnershipType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGraphqlApisRequestRequestTypeDef = TypedDict(
     "ListGraphqlApisRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
+        "apiType": GraphQLApiTypeType,
+        "owner": OwnershipType,
+    },
+    total=False,
+)
+
+_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
+    "_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
+    {
+        "apiId": str,
+        "functionId": str,
+    },
+)
+_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
+    "_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef(
+    _RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
+    _OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListResolversByFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredListResolversByFunctionRequestRequestTypeDef",
     {
         "apiId": str,
         "functionId": str,
     },
 )
@@ -844,14 +1016,37 @@
 class ListResolversByFunctionRequestRequestTypeDef(
     _RequiredListResolversByFunctionRequestRequestTypeDef,
     _OptionalListResolversByFunctionRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListResolversRequestListResolversPaginateTypeDef = TypedDict(
+    "_RequiredListResolversRequestListResolversPaginateTypeDef",
+    {
+        "apiId": str,
+        "typeName": str,
+    },
+)
+_OptionalListResolversRequestListResolversPaginateTypeDef = TypedDict(
+    "_OptionalListResolversRequestListResolversPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListResolversRequestListResolversPaginateTypeDef(
+    _RequiredListResolversRequestListResolversPaginateTypeDef,
+    _OptionalListResolversRequestListResolversPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListResolversRequestRequestTypeDef = TypedDict(
     "_RequiredListResolversRequestRequestTypeDef",
     {
         "apiId": str,
         "typeName": str,
     },
 )
@@ -867,21 +1062,114 @@
 
 class ListResolversRequestRequestTypeDef(
     _RequiredListResolversRequestRequestTypeDef, _OptionalListResolversRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListSourceApiAssociationsRequestRequestTypeDef = TypedDict(
+    "_RequiredListSourceApiAssociationsRequestRequestTypeDef",
+    {
+        "apiId": str,
+    },
+)
+_OptionalListSourceApiAssociationsRequestRequestTypeDef = TypedDict(
+    "_OptionalListSourceApiAssociationsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListSourceApiAssociationsRequestRequestTypeDef(
+    _RequiredListSourceApiAssociationsRequestRequestTypeDef,
+    _OptionalListSourceApiAssociationsRequestRequestTypeDef,
+):
+    pass
+
+
+SourceApiAssociationSummaryTypeDef = TypedDict(
+    "SourceApiAssociationSummaryTypeDef",
+    {
+        "associationId": str,
+        "associationArn": str,
+        "sourceApiId": str,
+        "sourceApiArn": str,
+        "mergedApiId": str,
+        "mergedApiArn": str,
+        "description": str,
+    },
+    total=False,
+)
+
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
+_RequiredListTypesByAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredListTypesByAssociationRequestRequestTypeDef",
+    {
+        "mergedApiIdentifier": str,
+        "associationId": str,
+        "format": TypeDefinitionFormatType,
+    },
+)
+_OptionalListTypesByAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalListTypesByAssociationRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListTypesByAssociationRequestRequestTypeDef(
+    _RequiredListTypesByAssociationRequestRequestTypeDef,
+    _OptionalListTypesByAssociationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListTypesRequestListTypesPaginateTypeDef = TypedDict(
+    "_RequiredListTypesRequestListTypesPaginateTypeDef",
+    {
+        "apiId": str,
+        "format": TypeDefinitionFormatType,
+    },
+)
+_OptionalListTypesRequestListTypesPaginateTypeDef = TypedDict(
+    "_OptionalListTypesRequestListTypesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTypesRequestListTypesPaginateTypeDef(
+    _RequiredListTypesRequestListTypesPaginateTypeDef,
+    _OptionalListTypesRequestListTypesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypesRequestRequestTypeDef",
     {
         "apiId": str,
         "format": TypeDefinitionFormatType,
     },
 )
@@ -897,34 +1185,79 @@
 
 class ListTypesRequestRequestTypeDef(
     _RequiredListTypesRequestRequestTypeDef, _OptionalListTypesRequestRequestTypeDef
 ):
     pass
 
 
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
 RdsHttpEndpointConfigTypeDef = TypedDict(
     "RdsHttpEndpointConfigTypeDef",
     {
         "awsRegion": str,
         "dbClusterIdentifier": str,
         "databaseName": str,
         "schema": str,
         "awsSecretStoreArn": str,
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
 StartSchemaCreationRequestRequestTypeDef = TypedDict(
     "StartSchemaCreationRequestRequestTypeDef",
     {
         "apiId": str,
         "definition": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
+StartSchemaCreationResponseTypeDef = TypedDict(
+    "StartSchemaCreationResponseTypeDef",
+    {
+        "status": SchemaStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartSchemaMergeRequestRequestTypeDef = TypedDict(
+    "StartSchemaMergeRequestRequestTypeDef",
+    {
+        "associationId": str,
+        "mergedApiIdentifier": str,
+    },
+)
+
+StartSchemaMergeResponseTypeDef = TypedDict(
+    "StartSchemaMergeResponseTypeDef",
+    {
+        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
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
@@ -1021,134 +1354,191 @@
         "openIDConnectConfig": OpenIDConnectConfigTypeDef,
         "userPoolConfig": CognitoUserPoolConfigTypeDef,
         "lambdaAuthorizerConfig": LambdaAuthorizerConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredEvaluateCodeRequestRequestTypeDef = TypedDict(
-    "_RequiredEvaluateCodeRequestRequestTypeDef",
+AssociateApiResponseTypeDef = TypedDict(
+    "AssociateApiResponseTypeDef",
     {
-        "runtime": AppSyncRuntimeTypeDef,
-        "code": str,
-        "context": str,
+        "apiAssociation": ApiAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalEvaluateCodeRequestRequestTypeDef = TypedDict(
-    "_OptionalEvaluateCodeRequestRequestTypeDef",
+
+GetApiAssociationResponseTypeDef = TypedDict(
+    "GetApiAssociationResponseTypeDef",
     {
-        "function": str,
+        "apiAssociation": ApiAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
+CreateApiCacheResponseTypeDef = TypedDict(
+    "CreateApiCacheResponseTypeDef",
+    {
+        "apiCache": ApiCacheTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-class EvaluateCodeRequestRequestTypeDef(
-    _RequiredEvaluateCodeRequestRequestTypeDef, _OptionalEvaluateCodeRequestRequestTypeDef
-):
-    pass
-
-
-AssociateApiResponseTypeDef = TypedDict(
-    "AssociateApiResponseTypeDef",
+GetApiCacheResponseTypeDef = TypedDict(
+    "GetApiCacheResponseTypeDef",
     {
-        "apiAssociation": ApiAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "apiCache": ApiCacheTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateApiCacheResponseTypeDef = TypedDict(
-    "CreateApiCacheResponseTypeDef",
+UpdateApiCacheResponseTypeDef = TypedDict(
+    "UpdateApiCacheResponseTypeDef",
     {
         "apiCache": ApiCacheTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateApiKeyResponseTypeDef = TypedDict(
     "CreateApiKeyResponseTypeDef",
     {
         "apiKey": ApiKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetApiAssociationResponseTypeDef = TypedDict(
-    "GetApiAssociationResponseTypeDef",
+ListApiKeysResponseTypeDef = TypedDict(
+    "ListApiKeysResponseTypeDef",
     {
-        "apiAssociation": ApiAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "apiKeys": List[ApiKeyTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetApiCacheResponseTypeDef = TypedDict(
-    "GetApiCacheResponseTypeDef",
+UpdateApiKeyResponseTypeDef = TypedDict(
+    "UpdateApiKeyResponseTypeDef",
     {
-        "apiCache": ApiCacheTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "apiKey": ApiKeyTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetIntrospectionSchemaResponseTypeDef = TypedDict(
-    "GetIntrospectionSchemaResponseTypeDef",
+_RequiredEvaluateCodeRequestRequestTypeDef = TypedDict(
+    "_RequiredEvaluateCodeRequestRequestTypeDef",
     {
-        "schema": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "runtime": AppSyncRuntimeTypeDef,
+        "code": str,
+        "context": str,
     },
 )
-
-GetSchemaCreationStatusResponseTypeDef = TypedDict(
-    "GetSchemaCreationStatusResponseTypeDef",
+_OptionalEvaluateCodeRequestRequestTypeDef = TypedDict(
+    "_OptionalEvaluateCodeRequestRequestTypeDef",
     {
-        "status": SchemaStatusType,
-        "details": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "function": str,
     },
+    total=False,
 )
 
-ListApiKeysResponseTypeDef = TypedDict(
-    "ListApiKeysResponseTypeDef",
+
+class EvaluateCodeRequestRequestTypeDef(
+    _RequiredEvaluateCodeRequestRequestTypeDef, _OptionalEvaluateCodeRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredAssociateMergedGraphqlApiRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateMergedGraphqlApiRequestRequestTypeDef",
     {
-        "apiKeys": List[ApiKeyTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "sourceApiIdentifier": str,
+        "mergedApiIdentifier": str,
     },
 )
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_OptionalAssociateMergedGraphqlApiRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateMergedGraphqlApiRequestRequestTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "description": str,
+        "sourceApiAssociationConfig": SourceApiAssociationConfigTypeDef,
     },
+    total=False,
 )
 
-StartSchemaCreationResponseTypeDef = TypedDict(
-    "StartSchemaCreationResponseTypeDef",
+
+class AssociateMergedGraphqlApiRequestRequestTypeDef(
+    _RequiredAssociateMergedGraphqlApiRequestRequestTypeDef,
+    _OptionalAssociateMergedGraphqlApiRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredAssociateSourceGraphqlApiRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateSourceGraphqlApiRequestRequestTypeDef",
     {
-        "status": SchemaStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "mergedApiIdentifier": str,
+        "sourceApiIdentifier": str,
     },
 )
+_OptionalAssociateSourceGraphqlApiRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateSourceGraphqlApiRequestRequestTypeDef",
+    {
+        "description": str,
+        "sourceApiAssociationConfig": SourceApiAssociationConfigTypeDef,
+    },
+    total=False,
+)
 
-UpdateApiCacheResponseTypeDef = TypedDict(
-    "UpdateApiCacheResponseTypeDef",
+
+class AssociateSourceGraphqlApiRequestRequestTypeDef(
+    _RequiredAssociateSourceGraphqlApiRequestRequestTypeDef,
+    _OptionalAssociateSourceGraphqlApiRequestRequestTypeDef,
+):
+    pass
+
+
+SourceApiAssociationTypeDef = TypedDict(
+    "SourceApiAssociationTypeDef",
     {
-        "apiCache": ApiCacheTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "associationId": str,
+        "associationArn": str,
+        "sourceApiId": str,
+        "sourceApiArn": str,
+        "mergedApiArn": str,
+        "mergedApiId": str,
+        "description": str,
+        "sourceApiAssociationConfig": SourceApiAssociationConfigTypeDef,
+        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
+        "sourceApiAssociationStatusDetail": str,
+        "lastSuccessfulMergeDate": datetime,
     },
+    total=False,
 )
 
-UpdateApiKeyResponseTypeDef = TypedDict(
-    "UpdateApiKeyResponseTypeDef",
+_RequiredUpdateSourceApiAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSourceApiAssociationRequestRequestTypeDef",
     {
-        "apiKey": ApiKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "associationId": str,
+        "mergedApiIdentifier": str,
     },
 )
+_OptionalUpdateSourceApiAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSourceApiAssociationRequestRequestTypeDef",
+    {
+        "description": str,
+        "sourceApiAssociationConfig": SourceApiAssociationConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateSourceApiAssociationRequestRequestTypeDef(
+    _RequiredUpdateSourceApiAssociationRequestRequestTypeDef,
+    _OptionalUpdateSourceApiAssociationRequestRequestTypeDef,
+):
+    pass
+
 
 _RequiredAuthorizationConfigTypeDef = TypedDict(
     "_RequiredAuthorizationConfigTypeDef",
     {
         "authorizationType": Literal["AWS_IAM"],
     },
 )
@@ -1177,73 +1567,82 @@
     total=False,
 )
 
 CreateDomainNameResponseTypeDef = TypedDict(
     "CreateDomainNameResponseTypeDef",
     {
         "domainNameConfig": DomainNameConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDomainNameResponseTypeDef = TypedDict(
     "GetDomainNameResponseTypeDef",
     {
         "domainNameConfig": DomainNameConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainNamesResponseTypeDef = TypedDict(
     "ListDomainNamesResponseTypeDef",
     {
         "domainNameConfigs": List[DomainNameConfigTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDomainNameResponseTypeDef = TypedDict(
     "UpdateDomainNameResponseTypeDef",
     {
         "domainNameConfig": DomainNameConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTypeResponseTypeDef = TypedDict(
     "CreateTypeResponseTypeDef",
     {
         "type": TypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTypeResponseTypeDef = TypedDict(
     "GetTypeResponseTypeDef",
     {
         "type": TypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTypesByAssociationResponseTypeDef = TypedDict(
+    "ListTypesByAssociationResponseTypeDef",
+    {
+        "types": List[TypeTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTypesResponseTypeDef = TypedDict(
     "ListTypesResponseTypeDef",
     {
         "types": List[TypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTypeResponseTypeDef = TypedDict(
     "UpdateTypeResponseTypeDef",
     {
         "type": TypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDynamodbDataSourceConfigTypeDef = TypedDict(
     "_RequiredDynamodbDataSourceConfigTypeDef",
     {
         "tableName": str,
@@ -1269,171 +1668,37 @@
 
 EvaluateMappingTemplateResponseTypeDef = TypedDict(
     "EvaluateMappingTemplateResponseTypeDef",
     {
         "evaluationResult": str,
         "error": ErrorDetailTypeDef,
         "logs": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SyncConfigTypeDef = TypedDict(
     "SyncConfigTypeDef",
     {
         "conflictHandler": ConflictHandlerTypeType,
         "conflictDetection": ConflictDetectionTypeType,
         "lambdaConflictHandlerConfig": LambdaConflictHandlerConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
-    "_RequiredListApiKeysRequestListApiKeysPaginateTypeDef",
+ListSourceApiAssociationsResponseTypeDef = TypedDict(
+    "ListSourceApiAssociationsResponseTypeDef",
     {
-        "apiId": str,
-    },
-)
-_OptionalListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
-    "_OptionalListApiKeysRequestListApiKeysPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListApiKeysRequestListApiKeysPaginateTypeDef(
-    _RequiredListApiKeysRequestListApiKeysPaginateTypeDef,
-    _OptionalListApiKeysRequestListApiKeysPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef",
-    {
-        "apiId": str,
-    },
-)
-_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDataSourcesRequestListDataSourcesPaginateTypeDef(
-    _RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef,
-    _OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionsRequestListFunctionsPaginateTypeDef",
-    {
-        "apiId": str,
-    },
-)
-_OptionalListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionsRequestListFunctionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListFunctionsRequestListFunctionsPaginateTypeDef(
-    _RequiredListFunctionsRequestListFunctionsPaginateTypeDef,
-    _OptionalListFunctionsRequestListFunctionsPaginateTypeDef,
-):
-    pass
-
-
-ListGraphqlApisRequestListGraphqlApisPaginateTypeDef = TypedDict(
-    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
-    "_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
-    {
-        "apiId": str,
-        "functionId": str,
-    },
-)
-_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
-    "_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef(
-    _RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
-    _OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListResolversRequestListResolversPaginateTypeDef = TypedDict(
-    "_RequiredListResolversRequestListResolversPaginateTypeDef",
-    {
-        "apiId": str,
-        "typeName": str,
-    },
-)
-_OptionalListResolversRequestListResolversPaginateTypeDef = TypedDict(
-    "_OptionalListResolversRequestListResolversPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListResolversRequestListResolversPaginateTypeDef(
-    _RequiredListResolversRequestListResolversPaginateTypeDef,
-    _OptionalListResolversRequestListResolversPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListTypesRequestListTypesPaginateTypeDef = TypedDict(
-    "_RequiredListTypesRequestListTypesPaginateTypeDef",
-    {
-        "apiId": str,
-        "format": TypeDefinitionFormatType,
-    },
-)
-_OptionalListTypesRequestListTypesPaginateTypeDef = TypedDict(
-    "_OptionalListTypesRequestListTypesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "sourceApiAssociationSummaries": List[SourceApiAssociationSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ListTypesRequestListTypesPaginateTypeDef(
-    _RequiredListTypesRequestListTypesPaginateTypeDef,
-    _OptionalListTypesRequestListTypesPaginateTypeDef,
-):
-    pass
-
-
 RelationalDatabaseDataSourceConfigTypeDef = TypedDict(
     "RelationalDatabaseDataSourceConfigTypeDef",
     {
         "relationalDatabaseSourceType": Literal["RDS_HTTP_ENDPOINT"],
         "rdsHttpEndpointConfig": RdsHttpEndpointConfigTypeDef,
     },
     total=False,
@@ -1452,14 +1717,18 @@
         "logConfig": LogConfigTypeDef,
         "userPoolConfig": UserPoolConfigTypeDef,
         "openIDConnectConfig": OpenIDConnectConfigTypeDef,
         "tags": Mapping[str, str],
         "additionalAuthenticationProviders": Sequence[AdditionalAuthenticationProviderTypeDef],
         "xrayEnabled": bool,
         "lambdaAuthorizerConfig": LambdaAuthorizerConfigTypeDef,
+        "visibility": GraphQLApiVisibilityType,
+        "apiType": GraphQLApiTypeType,
+        "mergedApiExecutionRoleArn": str,
+        "ownerContact": str,
     },
     total=False,
 )
 
 
 class CreateGraphqlApiRequestRequestTypeDef(
     _RequiredCreateGraphqlApiRequestRequestTypeDef, _OptionalCreateGraphqlApiRequestRequestTypeDef
@@ -1479,14 +1748,20 @@
         "arn": str,
         "uris": Dict[str, str],
         "tags": Dict[str, str],
         "additionalAuthenticationProviders": List[AdditionalAuthenticationProviderTypeDef],
         "xrayEnabled": bool,
         "wafWebAclArn": str,
         "lambdaAuthorizerConfig": LambdaAuthorizerConfigTypeDef,
+        "dns": Dict[str, str],
+        "visibility": GraphQLApiVisibilityType,
+        "apiType": GraphQLApiTypeType,
+        "mergedApiExecutionRoleArn": str,
+        "owner": str,
+        "ownerContact": str,
     },
     total=False,
 )
 
 _RequiredUpdateGraphqlApiRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGraphqlApiRequestRequestTypeDef",
     {
@@ -1500,25 +1775,59 @@
         "logConfig": LogConfigTypeDef,
         "authenticationType": AuthenticationTypeType,
         "userPoolConfig": UserPoolConfigTypeDef,
         "openIDConnectConfig": OpenIDConnectConfigTypeDef,
         "additionalAuthenticationProviders": Sequence[AdditionalAuthenticationProviderTypeDef],
         "xrayEnabled": bool,
         "lambdaAuthorizerConfig": LambdaAuthorizerConfigTypeDef,
+        "mergedApiExecutionRoleArn": str,
+        "ownerContact": str,
     },
     total=False,
 )
 
 
 class UpdateGraphqlApiRequestRequestTypeDef(
     _RequiredUpdateGraphqlApiRequestRequestTypeDef, _OptionalUpdateGraphqlApiRequestRequestTypeDef
 ):
     pass
 
 
+AssociateMergedGraphqlApiResponseTypeDef = TypedDict(
+    "AssociateMergedGraphqlApiResponseTypeDef",
+    {
+        "sourceApiAssociation": SourceApiAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AssociateSourceGraphqlApiResponseTypeDef = TypedDict(
+    "AssociateSourceGraphqlApiResponseTypeDef",
+    {
+        "sourceApiAssociation": SourceApiAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSourceApiAssociationResponseTypeDef = TypedDict(
+    "GetSourceApiAssociationResponseTypeDef",
+    {
+        "sourceApiAssociation": SourceApiAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSourceApiAssociationResponseTypeDef = TypedDict(
+    "UpdateSourceApiAssociationResponseTypeDef",
+    {
+        "sourceApiAssociation": SourceApiAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 HttpDataSourceConfigTypeDef = TypedDict(
     "HttpDataSourceConfigTypeDef",
     {
         "endpoint": str,
         "authorizationConfig": AuthorizationConfigTypeDef,
     },
     total=False,
@@ -1697,40 +2006,40 @@
     pass
 
 
 CreateGraphqlApiResponseTypeDef = TypedDict(
     "CreateGraphqlApiResponseTypeDef",
     {
         "graphqlApi": GraphqlApiTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGraphqlApiResponseTypeDef = TypedDict(
     "GetGraphqlApiResponseTypeDef",
     {
         "graphqlApi": GraphqlApiTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGraphqlApisResponseTypeDef = TypedDict(
     "ListGraphqlApisResponseTypeDef",
     {
         "graphqlApis": List[GraphqlApiTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGraphqlApiResponseTypeDef = TypedDict(
     "UpdateGraphqlApiResponseTypeDef",
     {
         "graphqlApi": GraphqlApiTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceRequestRequestTypeDef",
     {
         "apiId": str,
@@ -1813,118 +2122,118 @@
 
 EvaluateCodeResponseTypeDef = TypedDict(
     "EvaluateCodeResponseTypeDef",
     {
         "evaluationResult": str,
         "error": EvaluateCodeErrorDetailTypeDef,
         "logs": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFunctionResponseTypeDef = TypedDict(
     "CreateFunctionResponseTypeDef",
     {
         "functionConfiguration": FunctionConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFunctionResponseTypeDef = TypedDict(
     "GetFunctionResponseTypeDef",
     {
         "functionConfiguration": FunctionConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFunctionsResponseTypeDef = TypedDict(
     "ListFunctionsResponseTypeDef",
     {
         "functions": List[FunctionConfigurationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFunctionResponseTypeDef = TypedDict(
     "UpdateFunctionResponseTypeDef",
     {
         "functionConfiguration": FunctionConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateResolverResponseTypeDef = TypedDict(
     "CreateResolverResponseTypeDef",
     {
         "resolver": ResolverTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResolverResponseTypeDef = TypedDict(
     "GetResolverResponseTypeDef",
     {
         "resolver": ResolverTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResolversByFunctionResponseTypeDef = TypedDict(
     "ListResolversByFunctionResponseTypeDef",
     {
         "resolvers": List[ResolverTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResolversResponseTypeDef = TypedDict(
     "ListResolversResponseTypeDef",
     {
         "resolvers": List[ResolverTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateResolverResponseTypeDef = TypedDict(
     "UpdateResolverResponseTypeDef",
     {
         "resolver": ResolverTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDataSourceResponseTypeDef = TypedDict(
     "CreateDataSourceResponseTypeDef",
     {
         "dataSource": DataSourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDataSourceResponseTypeDef = TypedDict(
     "GetDataSourceResponseTypeDef",
     {
         "dataSource": DataSourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDataSourcesResponseTypeDef = TypedDict(
     "ListDataSourcesResponseTypeDef",
     {
         "dataSources": List[DataSourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDataSourceResponseTypeDef = TypedDict(
     "UpdateDataSourceResponseTypeDef",
     {
         "dataSource": DataSourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/type_defs.pyi` & `mypy-boto3-appsync-1.27.0/mypy_boto3_appsync/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ```python
     from mypy_boto3_appsync.type_defs import CognitoUserPoolConfigTypeDef
 
     data: CognitoUserPoolConfigTypeDef = {...}
     ```
 """
 import sys
+from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     ApiCacheStatusType,
     ApiCacheTypeType,
@@ -23,17 +24,22 @@
     AssociationStatusType,
     AuthenticationTypeType,
     ConflictDetectionTypeType,
     ConflictHandlerTypeType,
     DataSourceTypeType,
     DefaultActionType,
     FieldLogLevelType,
+    GraphQLApiTypeType,
+    GraphQLApiVisibilityType,
+    MergeTypeType,
     OutputTypeType,
+    OwnershipType,
     ResolverKindType,
     SchemaStatusType,
+    SourceApiAssociationStatusType,
     TypeDefinitionFormatType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -47,15 +53,15 @@
     "LambdaAuthorizerConfigTypeDef",
     "OpenIDConnectConfigTypeDef",
     "ApiAssociationTypeDef",
     "ApiCacheTypeDef",
     "ApiKeyTypeDef",
     "AppSyncRuntimeTypeDef",
     "AssociateApiRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "SourceApiAssociationConfigTypeDef",
     "AwsIamConfigTypeDef",
     "CachingConfigTypeDef",
     "CodeErrorLocationTypeDef",
     "CreateApiCacheRequestRequestTypeDef",
     "CreateApiKeyRequestRequestTypeDef",
     "ElasticsearchDataSourceConfigTypeDef",
     "EventBridgeDataSourceConfigTypeDef",
@@ -74,84 +80,105 @@
     "DeleteDomainNameRequestRequestTypeDef",
     "DeleteFunctionRequestRequestTypeDef",
     "DeleteGraphqlApiRequestRequestTypeDef",
     "DeleteResolverRequestRequestTypeDef",
     "DeleteTypeRequestRequestTypeDef",
     "DeltaSyncConfigTypeDef",
     "DisassociateApiRequestRequestTypeDef",
+    "DisassociateMergedGraphqlApiRequestRequestTypeDef",
+    "DisassociateMergedGraphqlApiResponseTypeDef",
+    "DisassociateSourceGraphqlApiRequestRequestTypeDef",
+    "DisassociateSourceGraphqlApiResponseTypeDef",
     "ErrorDetailTypeDef",
     "EvaluateMappingTemplateRequestRequestTypeDef",
     "FlushApiCacheRequestRequestTypeDef",
     "GetApiAssociationRequestRequestTypeDef",
     "GetApiCacheRequestRequestTypeDef",
     "GetDataSourceRequestRequestTypeDef",
     "GetDomainNameRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
     "GetGraphqlApiRequestRequestTypeDef",
     "GetIntrospectionSchemaRequestRequestTypeDef",
+    "GetIntrospectionSchemaResponseTypeDef",
     "GetResolverRequestRequestTypeDef",
     "GetSchemaCreationStatusRequestRequestTypeDef",
+    "GetSchemaCreationStatusResponseTypeDef",
+    "GetSourceApiAssociationRequestRequestTypeDef",
     "GetTypeRequestRequestTypeDef",
     "LambdaConflictHandlerConfigTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListApiKeysRequestListApiKeysPaginateTypeDef",
     "ListApiKeysRequestRequestTypeDef",
+    "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     "ListDataSourcesRequestRequestTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
+    "ListFunctionsRequestListFunctionsPaginateTypeDef",
     "ListFunctionsRequestRequestTypeDef",
+    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
     "ListGraphqlApisRequestRequestTypeDef",
+    "ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
     "ListResolversByFunctionRequestRequestTypeDef",
+    "ListResolversRequestListResolversPaginateTypeDef",
     "ListResolversRequestRequestTypeDef",
+    "ListSourceApiAssociationsRequestRequestTypeDef",
+    "SourceApiAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTypesByAssociationRequestRequestTypeDef",
+    "ListTypesRequestListTypesPaginateTypeDef",
     "ListTypesRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "RdsHttpEndpointConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "StartSchemaCreationRequestRequestTypeDef",
+    "StartSchemaCreationResponseTypeDef",
+    "StartSchemaMergeRequestRequestTypeDef",
+    "StartSchemaMergeResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiCacheRequestRequestTypeDef",
     "UpdateApiKeyRequestRequestTypeDef",
     "UpdateDomainNameRequestRequestTypeDef",
     "UpdateTypeRequestRequestTypeDef",
     "AdditionalAuthenticationProviderTypeDef",
-    "EvaluateCodeRequestRequestTypeDef",
     "AssociateApiResponseTypeDef",
-    "CreateApiCacheResponseTypeDef",
-    "CreateApiKeyResponseTypeDef",
     "GetApiAssociationResponseTypeDef",
+    "CreateApiCacheResponseTypeDef",
     "GetApiCacheResponseTypeDef",
-    "GetIntrospectionSchemaResponseTypeDef",
-    "GetSchemaCreationStatusResponseTypeDef",
-    "ListApiKeysResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartSchemaCreationResponseTypeDef",
     "UpdateApiCacheResponseTypeDef",
+    "CreateApiKeyResponseTypeDef",
+    "ListApiKeysResponseTypeDef",
     "UpdateApiKeyResponseTypeDef",
+    "EvaluateCodeRequestRequestTypeDef",
+    "AssociateMergedGraphqlApiRequestRequestTypeDef",
+    "AssociateSourceGraphqlApiRequestRequestTypeDef",
+    "SourceApiAssociationTypeDef",
+    "UpdateSourceApiAssociationRequestRequestTypeDef",
     "AuthorizationConfigTypeDef",
     "CodeErrorTypeDef",
     "CreateDomainNameResponseTypeDef",
     "GetDomainNameResponseTypeDef",
     "ListDomainNamesResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateTypeResponseTypeDef",
     "GetTypeResponseTypeDef",
+    "ListTypesByAssociationResponseTypeDef",
     "ListTypesResponseTypeDef",
     "UpdateTypeResponseTypeDef",
     "DynamodbDataSourceConfigTypeDef",
     "EvaluateMappingTemplateResponseTypeDef",
     "SyncConfigTypeDef",
-    "ListApiKeysRequestListApiKeysPaginateTypeDef",
-    "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
-    "ListFunctionsRequestListFunctionsPaginateTypeDef",
-    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
-    "ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
-    "ListResolversRequestListResolversPaginateTypeDef",
-    "ListTypesRequestListTypesPaginateTypeDef",
+    "ListSourceApiAssociationsResponseTypeDef",
     "RelationalDatabaseDataSourceConfigTypeDef",
     "CreateGraphqlApiRequestRequestTypeDef",
     "GraphqlApiTypeDef",
     "UpdateGraphqlApiRequestRequestTypeDef",
+    "AssociateMergedGraphqlApiResponseTypeDef",
+    "AssociateSourceGraphqlApiResponseTypeDef",
+    "GetSourceApiAssociationResponseTypeDef",
+    "UpdateSourceApiAssociationResponseTypeDef",
     "HttpDataSourceConfigTypeDef",
     "EvaluateCodeErrorDetailTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "CreateResolverRequestRequestTypeDef",
     "FunctionConfigurationTypeDef",
     "ResolverTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
@@ -287,23 +314,20 @@
     "AssociateApiRequestRequestTypeDef",
     {
         "domainName": str,
         "apiId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+SourceApiAssociationConfigTypeDef = TypedDict(
+    "SourceApiAssociationConfigTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "mergeType": MergeTypeType,
     },
+    total=False,
 )
 
 AwsIamConfigTypeDef = TypedDict(
     "AwsIamConfigTypeDef",
     {
         "signingRegion": str,
         "signingServiceName": str,
@@ -584,14 +608,46 @@
 DisassociateApiRequestRequestTypeDef = TypedDict(
     "DisassociateApiRequestRequestTypeDef",
     {
         "domainName": str,
     },
 )
 
+DisassociateMergedGraphqlApiRequestRequestTypeDef = TypedDict(
+    "DisassociateMergedGraphqlApiRequestRequestTypeDef",
+    {
+        "sourceApiIdentifier": str,
+        "associationId": str,
+    },
+)
+
+DisassociateMergedGraphqlApiResponseTypeDef = TypedDict(
+    "DisassociateMergedGraphqlApiResponseTypeDef",
+    {
+        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DisassociateSourceGraphqlApiRequestRequestTypeDef = TypedDict(
+    "DisassociateSourceGraphqlApiRequestRequestTypeDef",
+    {
+        "mergedApiIdentifier": str,
+        "associationId": str,
+    },
+)
+
+DisassociateSourceGraphqlApiResponseTypeDef = TypedDict(
+    "DisassociateSourceGraphqlApiResponseTypeDef",
+    {
+        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "message": str,
     },
     total=False,
 )
@@ -672,14 +728,22 @@
 
 class GetIntrospectionSchemaRequestRequestTypeDef(
     _RequiredGetIntrospectionSchemaRequestRequestTypeDef,
     _OptionalGetIntrospectionSchemaRequestRequestTypeDef,
 ):
     pass
 
+GetIntrospectionSchemaResponseTypeDef = TypedDict(
+    "GetIntrospectionSchemaResponseTypeDef",
+    {
+        "schema": StreamingBody,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetResolverRequestRequestTypeDef = TypedDict(
     "GetResolverRequestRequestTypeDef",
     {
         "apiId": str,
         "typeName": str,
         "fieldName": str,
     },
@@ -688,14 +752,31 @@
 GetSchemaCreationStatusRequestRequestTypeDef = TypedDict(
     "GetSchemaCreationStatusRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 
+GetSchemaCreationStatusResponseTypeDef = TypedDict(
+    "GetSchemaCreationStatusResponseTypeDef",
+    {
+        "status": SchemaStatusType,
+        "details": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSourceApiAssociationRequestRequestTypeDef = TypedDict(
+    "GetSourceApiAssociationRequestRequestTypeDef",
+    {
+        "mergedApiIdentifier": str,
+        "associationId": str,
+    },
+)
+
 GetTypeRequestRequestTypeDef = TypedDict(
     "GetTypeRequestRequestTypeDef",
     {
         "apiId": str,
         "typeName": str,
         "format": TypeDefinitionFormatType,
     },
@@ -705,24 +786,34 @@
     "LambdaConflictHandlerConfigTypeDef",
     {
         "lambdaConflictHandlerArn": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
+    "_RequiredListApiKeysRequestListApiKeysPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "apiId": str,
+    },
+)
+_OptionalListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
+    "_OptionalListApiKeysRequestListApiKeysPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListApiKeysRequestListApiKeysPaginateTypeDef(
+    _RequiredListApiKeysRequestListApiKeysPaginateTypeDef,
+    _OptionalListApiKeysRequestListApiKeysPaginateTypeDef,
+):
+    pass
+
 _RequiredListApiKeysRequestRequestTypeDef = TypedDict(
     "_RequiredListApiKeysRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 _OptionalListApiKeysRequestRequestTypeDef = TypedDict(
@@ -735,14 +826,34 @@
 )
 
 class ListApiKeysRequestRequestTypeDef(
     _RequiredListApiKeysRequestRequestTypeDef, _OptionalListApiKeysRequestRequestTypeDef
 ):
     pass
 
+_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef",
+    {
+        "apiId": str,
+    },
+)
+_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDataSourcesRequestListDataSourcesPaginateTypeDef(
+    _RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef,
+    _OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef,
+):
+    pass
+
 _RequiredListDataSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSourcesRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 _OptionalListDataSourcesRequestRequestTypeDef = TypedDict(
@@ -764,14 +875,34 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionsRequestListFunctionsPaginateTypeDef",
+    {
+        "apiId": str,
+    },
+)
+_OptionalListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionsRequestListFunctionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListFunctionsRequestListFunctionsPaginateTypeDef(
+    _RequiredListFunctionsRequestListFunctionsPaginateTypeDef,
+    _OptionalListFunctionsRequestListFunctionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionsRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 _OptionalListFunctionsRequestRequestTypeDef = TypedDict(
@@ -784,23 +915,56 @@
 )
 
 class ListFunctionsRequestRequestTypeDef(
     _RequiredListFunctionsRequestRequestTypeDef, _OptionalListFunctionsRequestRequestTypeDef
 ):
     pass
 
+ListGraphqlApisRequestListGraphqlApisPaginateTypeDef = TypedDict(
+    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
+    {
+        "apiType": GraphQLApiTypeType,
+        "owner": OwnershipType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListGraphqlApisRequestRequestTypeDef = TypedDict(
     "ListGraphqlApisRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
+        "apiType": GraphQLApiTypeType,
+        "owner": OwnershipType,
+    },
+    total=False,
+)
+
+_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
+    "_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
+    {
+        "apiId": str,
+        "functionId": str,
+    },
+)
+_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
+    "_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef(
+    _RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
+    _OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
+):
+    pass
+
 _RequiredListResolversByFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredListResolversByFunctionRequestRequestTypeDef",
     {
         "apiId": str,
         "functionId": str,
     },
 )
@@ -815,14 +979,35 @@
 
 class ListResolversByFunctionRequestRequestTypeDef(
     _RequiredListResolversByFunctionRequestRequestTypeDef,
     _OptionalListResolversByFunctionRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListResolversRequestListResolversPaginateTypeDef = TypedDict(
+    "_RequiredListResolversRequestListResolversPaginateTypeDef",
+    {
+        "apiId": str,
+        "typeName": str,
+    },
+)
+_OptionalListResolversRequestListResolversPaginateTypeDef = TypedDict(
+    "_OptionalListResolversRequestListResolversPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListResolversRequestListResolversPaginateTypeDef(
+    _RequiredListResolversRequestListResolversPaginateTypeDef,
+    _OptionalListResolversRequestListResolversPaginateTypeDef,
+):
+    pass
+
 _RequiredListResolversRequestRequestTypeDef = TypedDict(
     "_RequiredListResolversRequestRequestTypeDef",
     {
         "apiId": str,
         "typeName": str,
     },
 )
@@ -836,21 +1021,108 @@
 )
 
 class ListResolversRequestRequestTypeDef(
     _RequiredListResolversRequestRequestTypeDef, _OptionalListResolversRequestRequestTypeDef
 ):
     pass
 
+_RequiredListSourceApiAssociationsRequestRequestTypeDef = TypedDict(
+    "_RequiredListSourceApiAssociationsRequestRequestTypeDef",
+    {
+        "apiId": str,
+    },
+)
+_OptionalListSourceApiAssociationsRequestRequestTypeDef = TypedDict(
+    "_OptionalListSourceApiAssociationsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListSourceApiAssociationsRequestRequestTypeDef(
+    _RequiredListSourceApiAssociationsRequestRequestTypeDef,
+    _OptionalListSourceApiAssociationsRequestRequestTypeDef,
+):
+    pass
+
+SourceApiAssociationSummaryTypeDef = TypedDict(
+    "SourceApiAssociationSummaryTypeDef",
+    {
+        "associationId": str,
+        "associationArn": str,
+        "sourceApiId": str,
+        "sourceApiArn": str,
+        "mergedApiId": str,
+        "mergedApiArn": str,
+        "description": str,
+    },
+    total=False,
+)
+
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
+_RequiredListTypesByAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredListTypesByAssociationRequestRequestTypeDef",
+    {
+        "mergedApiIdentifier": str,
+        "associationId": str,
+        "format": TypeDefinitionFormatType,
+    },
+)
+_OptionalListTypesByAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalListTypesByAssociationRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListTypesByAssociationRequestRequestTypeDef(
+    _RequiredListTypesByAssociationRequestRequestTypeDef,
+    _OptionalListTypesByAssociationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListTypesRequestListTypesPaginateTypeDef = TypedDict(
+    "_RequiredListTypesRequestListTypesPaginateTypeDef",
+    {
+        "apiId": str,
+        "format": TypeDefinitionFormatType,
+    },
+)
+_OptionalListTypesRequestListTypesPaginateTypeDef = TypedDict(
+    "_OptionalListTypesRequestListTypesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTypesRequestListTypesPaginateTypeDef(
+    _RequiredListTypesRequestListTypesPaginateTypeDef,
+    _OptionalListTypesRequestListTypesPaginateTypeDef,
+):
+    pass
+
 _RequiredListTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypesRequestRequestTypeDef",
     {
         "apiId": str,
         "format": TypeDefinitionFormatType,
     },
 )
@@ -864,34 +1136,79 @@
 )
 
 class ListTypesRequestRequestTypeDef(
     _RequiredListTypesRequestRequestTypeDef, _OptionalListTypesRequestRequestTypeDef
 ):
     pass
 
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
 RdsHttpEndpointConfigTypeDef = TypedDict(
     "RdsHttpEndpointConfigTypeDef",
     {
         "awsRegion": str,
         "dbClusterIdentifier": str,
         "databaseName": str,
         "schema": str,
         "awsSecretStoreArn": str,
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
 StartSchemaCreationRequestRequestTypeDef = TypedDict(
     "StartSchemaCreationRequestRequestTypeDef",
     {
         "apiId": str,
         "definition": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
+StartSchemaCreationResponseTypeDef = TypedDict(
+    "StartSchemaCreationResponseTypeDef",
+    {
+        "status": SchemaStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartSchemaMergeRequestRequestTypeDef = TypedDict(
+    "StartSchemaMergeRequestRequestTypeDef",
+    {
+        "associationId": str,
+        "mergedApiIdentifier": str,
+    },
+)
+
+StartSchemaMergeResponseTypeDef = TypedDict(
+    "StartSchemaMergeResponseTypeDef",
+    {
+        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
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
@@ -982,132 +1299,183 @@
         "openIDConnectConfig": OpenIDConnectConfigTypeDef,
         "userPoolConfig": CognitoUserPoolConfigTypeDef,
         "lambdaAuthorizerConfig": LambdaAuthorizerConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredEvaluateCodeRequestRequestTypeDef = TypedDict(
-    "_RequiredEvaluateCodeRequestRequestTypeDef",
+AssociateApiResponseTypeDef = TypedDict(
+    "AssociateApiResponseTypeDef",
     {
-        "runtime": AppSyncRuntimeTypeDef,
-        "code": str,
-        "context": str,
+        "apiAssociation": ApiAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalEvaluateCodeRequestRequestTypeDef = TypedDict(
-    "_OptionalEvaluateCodeRequestRequestTypeDef",
+
+GetApiAssociationResponseTypeDef = TypedDict(
+    "GetApiAssociationResponseTypeDef",
     {
-        "function": str,
+        "apiAssociation": ApiAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class EvaluateCodeRequestRequestTypeDef(
-    _RequiredEvaluateCodeRequestRequestTypeDef, _OptionalEvaluateCodeRequestRequestTypeDef
-):
-    pass
+CreateApiCacheResponseTypeDef = TypedDict(
+    "CreateApiCacheResponseTypeDef",
+    {
+        "apiCache": ApiCacheTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-AssociateApiResponseTypeDef = TypedDict(
-    "AssociateApiResponseTypeDef",
+GetApiCacheResponseTypeDef = TypedDict(
+    "GetApiCacheResponseTypeDef",
     {
-        "apiAssociation": ApiAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "apiCache": ApiCacheTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateApiCacheResponseTypeDef = TypedDict(
-    "CreateApiCacheResponseTypeDef",
+UpdateApiCacheResponseTypeDef = TypedDict(
+    "UpdateApiCacheResponseTypeDef",
     {
         "apiCache": ApiCacheTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateApiKeyResponseTypeDef = TypedDict(
     "CreateApiKeyResponseTypeDef",
     {
         "apiKey": ApiKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetApiAssociationResponseTypeDef = TypedDict(
-    "GetApiAssociationResponseTypeDef",
+ListApiKeysResponseTypeDef = TypedDict(
+    "ListApiKeysResponseTypeDef",
     {
-        "apiAssociation": ApiAssociationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "apiKeys": List[ApiKeyTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetApiCacheResponseTypeDef = TypedDict(
-    "GetApiCacheResponseTypeDef",
+UpdateApiKeyResponseTypeDef = TypedDict(
+    "UpdateApiKeyResponseTypeDef",
     {
-        "apiCache": ApiCacheTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "apiKey": ApiKeyTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetIntrospectionSchemaResponseTypeDef = TypedDict(
-    "GetIntrospectionSchemaResponseTypeDef",
+_RequiredEvaluateCodeRequestRequestTypeDef = TypedDict(
+    "_RequiredEvaluateCodeRequestRequestTypeDef",
     {
-        "schema": StreamingBody,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "runtime": AppSyncRuntimeTypeDef,
+        "code": str,
+        "context": str,
     },
 )
-
-GetSchemaCreationStatusResponseTypeDef = TypedDict(
-    "GetSchemaCreationStatusResponseTypeDef",
+_OptionalEvaluateCodeRequestRequestTypeDef = TypedDict(
+    "_OptionalEvaluateCodeRequestRequestTypeDef",
     {
-        "status": SchemaStatusType,
-        "details": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "function": str,
     },
+    total=False,
 )
 
-ListApiKeysResponseTypeDef = TypedDict(
-    "ListApiKeysResponseTypeDef",
+class EvaluateCodeRequestRequestTypeDef(
+    _RequiredEvaluateCodeRequestRequestTypeDef, _OptionalEvaluateCodeRequestRequestTypeDef
+):
+    pass
+
+_RequiredAssociateMergedGraphqlApiRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateMergedGraphqlApiRequestRequestTypeDef",
     {
-        "apiKeys": List[ApiKeyTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "sourceApiIdentifier": str,
+        "mergedApiIdentifier": str,
     },
 )
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_OptionalAssociateMergedGraphqlApiRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateMergedGraphqlApiRequestRequestTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "description": str,
+        "sourceApiAssociationConfig": SourceApiAssociationConfigTypeDef,
     },
+    total=False,
 )
 
-StartSchemaCreationResponseTypeDef = TypedDict(
-    "StartSchemaCreationResponseTypeDef",
+class AssociateMergedGraphqlApiRequestRequestTypeDef(
+    _RequiredAssociateMergedGraphqlApiRequestRequestTypeDef,
+    _OptionalAssociateMergedGraphqlApiRequestRequestTypeDef,
+):
+    pass
+
+_RequiredAssociateSourceGraphqlApiRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateSourceGraphqlApiRequestRequestTypeDef",
     {
-        "status": SchemaStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "mergedApiIdentifier": str,
+        "sourceApiIdentifier": str,
+    },
+)
+_OptionalAssociateSourceGraphqlApiRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateSourceGraphqlApiRequestRequestTypeDef",
+    {
+        "description": str,
+        "sourceApiAssociationConfig": SourceApiAssociationConfigTypeDef,
     },
+    total=False,
 )
 
-UpdateApiCacheResponseTypeDef = TypedDict(
-    "UpdateApiCacheResponseTypeDef",
+class AssociateSourceGraphqlApiRequestRequestTypeDef(
+    _RequiredAssociateSourceGraphqlApiRequestRequestTypeDef,
+    _OptionalAssociateSourceGraphqlApiRequestRequestTypeDef,
+):
+    pass
+
+SourceApiAssociationTypeDef = TypedDict(
+    "SourceApiAssociationTypeDef",
     {
-        "apiCache": ApiCacheTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "associationId": str,
+        "associationArn": str,
+        "sourceApiId": str,
+        "sourceApiArn": str,
+        "mergedApiArn": str,
+        "mergedApiId": str,
+        "description": str,
+        "sourceApiAssociationConfig": SourceApiAssociationConfigTypeDef,
+        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
+        "sourceApiAssociationStatusDetail": str,
+        "lastSuccessfulMergeDate": datetime,
     },
+    total=False,
 )
 
-UpdateApiKeyResponseTypeDef = TypedDict(
-    "UpdateApiKeyResponseTypeDef",
+_RequiredUpdateSourceApiAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSourceApiAssociationRequestRequestTypeDef",
     {
-        "apiKey": ApiKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "associationId": str,
+        "mergedApiIdentifier": str,
     },
 )
+_OptionalUpdateSourceApiAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSourceApiAssociationRequestRequestTypeDef",
+    {
+        "description": str,
+        "sourceApiAssociationConfig": SourceApiAssociationConfigTypeDef,
+    },
+    total=False,
+)
+
+class UpdateSourceApiAssociationRequestRequestTypeDef(
+    _RequiredUpdateSourceApiAssociationRequestRequestTypeDef,
+    _OptionalUpdateSourceApiAssociationRequestRequestTypeDef,
+):
+    pass
 
 _RequiredAuthorizationConfigTypeDef = TypedDict(
     "_RequiredAuthorizationConfigTypeDef",
     {
         "authorizationType": Literal["AWS_IAM"],
     },
 )
@@ -1134,73 +1502,82 @@
     total=False,
 )
 
 CreateDomainNameResponseTypeDef = TypedDict(
     "CreateDomainNameResponseTypeDef",
     {
         "domainNameConfig": DomainNameConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDomainNameResponseTypeDef = TypedDict(
     "GetDomainNameResponseTypeDef",
     {
         "domainNameConfig": DomainNameConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainNamesResponseTypeDef = TypedDict(
     "ListDomainNamesResponseTypeDef",
     {
         "domainNameConfigs": List[DomainNameConfigTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDomainNameResponseTypeDef = TypedDict(
     "UpdateDomainNameResponseTypeDef",
     {
         "domainNameConfig": DomainNameConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTypeResponseTypeDef = TypedDict(
     "CreateTypeResponseTypeDef",
     {
         "type": TypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTypeResponseTypeDef = TypedDict(
     "GetTypeResponseTypeDef",
     {
         "type": TypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTypesByAssociationResponseTypeDef = TypedDict(
+    "ListTypesByAssociationResponseTypeDef",
+    {
+        "types": List[TypeTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTypesResponseTypeDef = TypedDict(
     "ListTypesResponseTypeDef",
     {
         "types": List[TypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTypeResponseTypeDef = TypedDict(
     "UpdateTypeResponseTypeDef",
     {
         "type": TypeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDynamodbDataSourceConfigTypeDef = TypedDict(
     "_RequiredDynamodbDataSourceConfigTypeDef",
     {
         "tableName": str,
@@ -1224,159 +1601,37 @@
 
 EvaluateMappingTemplateResponseTypeDef = TypedDict(
     "EvaluateMappingTemplateResponseTypeDef",
     {
         "evaluationResult": str,
         "error": ErrorDetailTypeDef,
         "logs": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SyncConfigTypeDef = TypedDict(
     "SyncConfigTypeDef",
     {
         "conflictHandler": ConflictHandlerTypeType,
         "conflictDetection": ConflictDetectionTypeType,
         "lambdaConflictHandlerConfig": LambdaConflictHandlerConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
-    "_RequiredListApiKeysRequestListApiKeysPaginateTypeDef",
-    {
-        "apiId": str,
-    },
-)
-_OptionalListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
-    "_OptionalListApiKeysRequestListApiKeysPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListApiKeysRequestListApiKeysPaginateTypeDef(
-    _RequiredListApiKeysRequestListApiKeysPaginateTypeDef,
-    _OptionalListApiKeysRequestListApiKeysPaginateTypeDef,
-):
-    pass
-
-_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef",
+ListSourceApiAssociationsResponseTypeDef = TypedDict(
+    "ListSourceApiAssociationsResponseTypeDef",
     {
-        "apiId": str,
-    },
-)
-_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDataSourcesRequestListDataSourcesPaginateTypeDef(
-    _RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef,
-    _OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef,
-):
-    pass
-
-_RequiredListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionsRequestListFunctionsPaginateTypeDef",
-    {
-        "apiId": str,
-    },
-)
-_OptionalListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionsRequestListFunctionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListFunctionsRequestListFunctionsPaginateTypeDef(
-    _RequiredListFunctionsRequestListFunctionsPaginateTypeDef,
-    _OptionalListFunctionsRequestListFunctionsPaginateTypeDef,
-):
-    pass
-
-ListGraphqlApisRequestListGraphqlApisPaginateTypeDef = TypedDict(
-    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
-    "_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
-    {
-        "apiId": str,
-        "functionId": str,
-    },
-)
-_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
-    "_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef(
-    _RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
-    _OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
-):
-    pass
-
-_RequiredListResolversRequestListResolversPaginateTypeDef = TypedDict(
-    "_RequiredListResolversRequestListResolversPaginateTypeDef",
-    {
-        "apiId": str,
-        "typeName": str,
-    },
-)
-_OptionalListResolversRequestListResolversPaginateTypeDef = TypedDict(
-    "_OptionalListResolversRequestListResolversPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListResolversRequestListResolversPaginateTypeDef(
-    _RequiredListResolversRequestListResolversPaginateTypeDef,
-    _OptionalListResolversRequestListResolversPaginateTypeDef,
-):
-    pass
-
-_RequiredListTypesRequestListTypesPaginateTypeDef = TypedDict(
-    "_RequiredListTypesRequestListTypesPaginateTypeDef",
-    {
-        "apiId": str,
-        "format": TypeDefinitionFormatType,
-    },
-)
-_OptionalListTypesRequestListTypesPaginateTypeDef = TypedDict(
-    "_OptionalListTypesRequestListTypesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "sourceApiAssociationSummaries": List[SourceApiAssociationSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class ListTypesRequestListTypesPaginateTypeDef(
-    _RequiredListTypesRequestListTypesPaginateTypeDef,
-    _OptionalListTypesRequestListTypesPaginateTypeDef,
-):
-    pass
-
 RelationalDatabaseDataSourceConfigTypeDef = TypedDict(
     "RelationalDatabaseDataSourceConfigTypeDef",
     {
         "relationalDatabaseSourceType": Literal["RDS_HTTP_ENDPOINT"],
         "rdsHttpEndpointConfig": RdsHttpEndpointConfigTypeDef,
     },
     total=False,
@@ -1395,14 +1650,18 @@
         "logConfig": LogConfigTypeDef,
         "userPoolConfig": UserPoolConfigTypeDef,
         "openIDConnectConfig": OpenIDConnectConfigTypeDef,
         "tags": Mapping[str, str],
         "additionalAuthenticationProviders": Sequence[AdditionalAuthenticationProviderTypeDef],
         "xrayEnabled": bool,
         "lambdaAuthorizerConfig": LambdaAuthorizerConfigTypeDef,
+        "visibility": GraphQLApiVisibilityType,
+        "apiType": GraphQLApiTypeType,
+        "mergedApiExecutionRoleArn": str,
+        "ownerContact": str,
     },
     total=False,
 )
 
 class CreateGraphqlApiRequestRequestTypeDef(
     _RequiredCreateGraphqlApiRequestRequestTypeDef, _OptionalCreateGraphqlApiRequestRequestTypeDef
 ):
@@ -1420,14 +1679,20 @@
         "arn": str,
         "uris": Dict[str, str],
         "tags": Dict[str, str],
         "additionalAuthenticationProviders": List[AdditionalAuthenticationProviderTypeDef],
         "xrayEnabled": bool,
         "wafWebAclArn": str,
         "lambdaAuthorizerConfig": LambdaAuthorizerConfigTypeDef,
+        "dns": Dict[str, str],
+        "visibility": GraphQLApiVisibilityType,
+        "apiType": GraphQLApiTypeType,
+        "mergedApiExecutionRoleArn": str,
+        "owner": str,
+        "ownerContact": str,
     },
     total=False,
 )
 
 _RequiredUpdateGraphqlApiRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGraphqlApiRequestRequestTypeDef",
     {
@@ -1441,23 +1706,57 @@
         "logConfig": LogConfigTypeDef,
         "authenticationType": AuthenticationTypeType,
         "userPoolConfig": UserPoolConfigTypeDef,
         "openIDConnectConfig": OpenIDConnectConfigTypeDef,
         "additionalAuthenticationProviders": Sequence[AdditionalAuthenticationProviderTypeDef],
         "xrayEnabled": bool,
         "lambdaAuthorizerConfig": LambdaAuthorizerConfigTypeDef,
+        "mergedApiExecutionRoleArn": str,
+        "ownerContact": str,
     },
     total=False,
 )
 
 class UpdateGraphqlApiRequestRequestTypeDef(
     _RequiredUpdateGraphqlApiRequestRequestTypeDef, _OptionalUpdateGraphqlApiRequestRequestTypeDef
 ):
     pass
 
+AssociateMergedGraphqlApiResponseTypeDef = TypedDict(
+    "AssociateMergedGraphqlApiResponseTypeDef",
+    {
+        "sourceApiAssociation": SourceApiAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AssociateSourceGraphqlApiResponseTypeDef = TypedDict(
+    "AssociateSourceGraphqlApiResponseTypeDef",
+    {
+        "sourceApiAssociation": SourceApiAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSourceApiAssociationResponseTypeDef = TypedDict(
+    "GetSourceApiAssociationResponseTypeDef",
+    {
+        "sourceApiAssociation": SourceApiAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSourceApiAssociationResponseTypeDef = TypedDict(
+    "UpdateSourceApiAssociationResponseTypeDef",
+    {
+        "sourceApiAssociation": SourceApiAssociationTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 HttpDataSourceConfigTypeDef = TypedDict(
     "HttpDataSourceConfigTypeDef",
     {
         "endpoint": str,
         "authorizationConfig": AuthorizationConfigTypeDef,
     },
     total=False,
@@ -1628,40 +1927,40 @@
 ):
     pass
 
 CreateGraphqlApiResponseTypeDef = TypedDict(
     "CreateGraphqlApiResponseTypeDef",
     {
         "graphqlApi": GraphqlApiTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetGraphqlApiResponseTypeDef = TypedDict(
     "GetGraphqlApiResponseTypeDef",
     {
         "graphqlApi": GraphqlApiTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListGraphqlApisResponseTypeDef = TypedDict(
     "ListGraphqlApisResponseTypeDef",
     {
         "graphqlApis": List[GraphqlApiTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGraphqlApiResponseTypeDef = TypedDict(
     "UpdateGraphqlApiResponseTypeDef",
     {
         "graphqlApi": GraphqlApiTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceRequestRequestTypeDef",
     {
         "apiId": str,
@@ -1740,118 +2039,118 @@
 
 EvaluateCodeResponseTypeDef = TypedDict(
     "EvaluateCodeResponseTypeDef",
     {
         "evaluationResult": str,
         "error": EvaluateCodeErrorDetailTypeDef,
         "logs": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateFunctionResponseTypeDef = TypedDict(
     "CreateFunctionResponseTypeDef",
     {
         "functionConfiguration": FunctionConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFunctionResponseTypeDef = TypedDict(
     "GetFunctionResponseTypeDef",
     {
         "functionConfiguration": FunctionConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFunctionsResponseTypeDef = TypedDict(
     "ListFunctionsResponseTypeDef",
     {
         "functions": List[FunctionConfigurationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFunctionResponseTypeDef = TypedDict(
     "UpdateFunctionResponseTypeDef",
     {
         "functionConfiguration": FunctionConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateResolverResponseTypeDef = TypedDict(
     "CreateResolverResponseTypeDef",
     {
         "resolver": ResolverTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetResolverResponseTypeDef = TypedDict(
     "GetResolverResponseTypeDef",
     {
         "resolver": ResolverTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResolversByFunctionResponseTypeDef = TypedDict(
     "ListResolversByFunctionResponseTypeDef",
     {
         "resolvers": List[ResolverTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListResolversResponseTypeDef = TypedDict(
     "ListResolversResponseTypeDef",
     {
         "resolvers": List[ResolverTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateResolverResponseTypeDef = TypedDict(
     "UpdateResolverResponseTypeDef",
     {
         "resolver": ResolverTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateDataSourceResponseTypeDef = TypedDict(
     "CreateDataSourceResponseTypeDef",
     {
         "dataSource": DataSourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDataSourceResponseTypeDef = TypedDict(
     "GetDataSourceResponseTypeDef",
     {
         "dataSource": DataSourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDataSourcesResponseTypeDef = TypedDict(
     "ListDataSourcesResponseTypeDef",
     {
         "dataSources": List[DataSourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDataSourceResponseTypeDef = TypedDict(
     "UpdateDataSourceResponseTypeDef",
     {
         "dataSource": DataSourceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/PKG-INFO` & `mypy-boto3-appsync-1.27.0/mypy_boto3_appsync.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appsync
-Version: 1.26.61
-Summary: Type annotations for boto3.AppSync 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.AppSync 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-appsync"></a>
 
 # mypy-boto3-appsync
 
 [![PyPI - mypy-boto3-appsync](https://img.shields.io/pypi/v/mypy-boto3-appsync.svg?color=blue)](https://pypi.org/project/mypy-boto3-appsync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appsync.svg?color=blue)](https://pypi.org/project/mypy-boto3-appsync)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appsync?color=blue)](https://pypistats.org/packages/mypy-boto3-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppSync 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
+[boto3.AppSync 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appsync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,26 +323,31 @@
     AuthenticationTypeType,
     AuthorizationTypeType,
     ConflictDetectionTypeType,
     ConflictHandlerTypeType,
     DataSourceTypeType,
     DefaultActionType,
     FieldLogLevelType,
+    GraphQLApiTypeType,
+    GraphQLApiVisibilityType,
     ListApiKeysPaginatorName,
     ListDataSourcesPaginatorName,
     ListFunctionsPaginatorName,
     ListGraphqlApisPaginatorName,
     ListResolversByFunctionPaginatorName,
     ListResolversPaginatorName,
     ListTypesPaginatorName,
+    MergeTypeType,
     OutputTypeType,
+    OwnershipType,
     RelationalDatabaseSourceTypeType,
     ResolverKindType,
     RuntimeNameType,
     SchemaStatusType,
+    SourceApiAssociationStatusType,
     TypeDefinitionFormatType,
     AppSyncServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -365,15 +370,15 @@
     LambdaAuthorizerConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     ApiAssociationTypeDef,
     ApiCacheTypeDef,
     ApiKeyTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    SourceApiAssociationConfigTypeDef,
     AwsIamConfigTypeDef,
     CachingConfigTypeDef,
     CodeErrorLocationTypeDef,
     CreateApiCacheRequestRequestTypeDef,
     CreateApiKeyRequestRequestTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
     EventBridgeDataSourceConfigTypeDef,
@@ -392,84 +397,105 @@
     DeleteDomainNameRequestRequestTypeDef,
     DeleteFunctionRequestRequestTypeDef,
     DeleteGraphqlApiRequestRequestTypeDef,
     DeleteResolverRequestRequestTypeDef,
     DeleteTypeRequestRequestTypeDef,
     DeltaSyncConfigTypeDef,
     DisassociateApiRequestRequestTypeDef,
+    DisassociateMergedGraphqlApiRequestRequestTypeDef,
+    DisassociateMergedGraphqlApiResponseTypeDef,
+    DisassociateSourceGraphqlApiRequestRequestTypeDef,
+    DisassociateSourceGraphqlApiResponseTypeDef,
     ErrorDetailTypeDef,
     EvaluateMappingTemplateRequestRequestTypeDef,
     FlushApiCacheRequestRequestTypeDef,
     GetApiAssociationRequestRequestTypeDef,
     GetApiCacheRequestRequestTypeDef,
     GetDataSourceRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
     GetGraphqlApiRequestRequestTypeDef,
     GetIntrospectionSchemaRequestRequestTypeDef,
+    GetIntrospectionSchemaResponseTypeDef,
     GetResolverRequestRequestTypeDef,
     GetSchemaCreationStatusRequestRequestTypeDef,
+    GetSchemaCreationStatusResponseTypeDef,
+    GetSourceApiAssociationRequestRequestTypeDef,
     GetTypeRequestRequestTypeDef,
     LambdaConflictHandlerConfigTypeDef,
-    PaginatorConfigTypeDef,
+    ListApiKeysRequestListApiKeysPaginateTypeDef,
     ListApiKeysRequestRequestTypeDef,
+    ListDataSourcesRequestListDataSourcesPaginateTypeDef,
     ListDataSourcesRequestRequestTypeDef,
     ListDomainNamesRequestRequestTypeDef,
+    ListFunctionsRequestListFunctionsPaginateTypeDef,
     ListFunctionsRequestRequestTypeDef,
+    ListGraphqlApisRequestListGraphqlApisPaginateTypeDef,
     ListGraphqlApisRequestRequestTypeDef,
+    ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
     ListResolversByFunctionRequestRequestTypeDef,
+    ListResolversRequestListResolversPaginateTypeDef,
     ListResolversRequestRequestTypeDef,
+    ListSourceApiAssociationsRequestRequestTypeDef,
+    SourceApiAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTypesByAssociationRequestRequestTypeDef,
+    ListTypesRequestListTypesPaginateTypeDef,
     ListTypesRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     RdsHttpEndpointConfigTypeDef,
+    ResponseMetadataTypeDef,
     StartSchemaCreationRequestRequestTypeDef,
+    StartSchemaCreationResponseTypeDef,
+    StartSchemaMergeRequestRequestTypeDef,
+    StartSchemaMergeResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiCacheRequestRequestTypeDef,
     UpdateApiKeyRequestRequestTypeDef,
     UpdateDomainNameRequestRequestTypeDef,
     UpdateTypeRequestRequestTypeDef,
     AdditionalAuthenticationProviderTypeDef,
-    EvaluateCodeRequestRequestTypeDef,
     AssociateApiResponseTypeDef,
-    CreateApiCacheResponseTypeDef,
-    CreateApiKeyResponseTypeDef,
     GetApiAssociationResponseTypeDef,
+    CreateApiCacheResponseTypeDef,
     GetApiCacheResponseTypeDef,
-    GetIntrospectionSchemaResponseTypeDef,
-    GetSchemaCreationStatusResponseTypeDef,
-    ListApiKeysResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartSchemaCreationResponseTypeDef,
     UpdateApiCacheResponseTypeDef,
+    CreateApiKeyResponseTypeDef,
+    ListApiKeysResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
+    EvaluateCodeRequestRequestTypeDef,
+    AssociateMergedGraphqlApiRequestRequestTypeDef,
+    AssociateSourceGraphqlApiRequestRequestTypeDef,
+    SourceApiAssociationTypeDef,
+    UpdateSourceApiAssociationRequestRequestTypeDef,
     AuthorizationConfigTypeDef,
     CodeErrorTypeDef,
     CreateDomainNameResponseTypeDef,
     GetDomainNameResponseTypeDef,
     ListDomainNamesResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateTypeResponseTypeDef,
     GetTypeResponseTypeDef,
+    ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     UpdateTypeResponseTypeDef,
     DynamodbDataSourceConfigTypeDef,
     EvaluateMappingTemplateResponseTypeDef,
     SyncConfigTypeDef,
-    ListApiKeysRequestListApiKeysPaginateTypeDef,
-    ListDataSourcesRequestListDataSourcesPaginateTypeDef,
-    ListFunctionsRequestListFunctionsPaginateTypeDef,
-    ListGraphqlApisRequestListGraphqlApisPaginateTypeDef,
-    ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
-    ListResolversRequestListResolversPaginateTypeDef,
-    ListTypesRequestListTypesPaginateTypeDef,
+    ListSourceApiAssociationsResponseTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     CreateGraphqlApiRequestRequestTypeDef,
     GraphqlApiTypeDef,
     UpdateGraphqlApiRequestRequestTypeDef,
+    AssociateMergedGraphqlApiResponseTypeDef,
+    AssociateSourceGraphqlApiResponseTypeDef,
+    GetSourceApiAssociationResponseTypeDef,
+    UpdateSourceApiAssociationResponseTypeDef,
     HttpDataSourceConfigTypeDef,
     EvaluateCodeErrorDetailTypeDef,
     CreateFunctionRequestRequestTypeDef,
     CreateResolverRequestRequestTypeDef,
     FunctionConfigurationTypeDef,
     ResolverTypeDef,
     UpdateFunctionRequestRequestTypeDef,
@@ -505,42 +531,42 @@
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

### Comparing `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/SOURCES.txt` & `mypy-boto3-appsync-1.27.0/mypy_boto3_appsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.26.61/setup.py` & `mypy-boto3-appsync-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 Setup script for mypy-boto3-appsync.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appsync",
-    version="1.26.61",
+    version="1.27.0",
     packages=["mypy_boto3_appsync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppSync 1.26.61 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.AppSync 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/",
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


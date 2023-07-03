# Comparing `tmp/mypy-boto3-lex-models-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-lex-models-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lex-models-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:38 2022, max compression
+gzip compressed data, was "mypy-boto3-lex-models-1.27.0.tar", last modified: Mon Jul  3 19:51:01 2023, max compression
```

## Comparing `mypy-boto3-lex-models-1.26.0.post1.tar` & `mypy-boto3-lex-models-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:38.900832 mypy-boto3-lex-models-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:36:58.000000 mypy-boto3-lex-models-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    19230 2022-11-01 21:43:38.900832 mypy-boto3-lex-models-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17764 2022-11-01 21:36:58.000000 mypy-boto3-lex-models-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:38.896832 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/
--rw-r--r--   0 runner    (1001) docker     (121)     2501 2022-11-01 21:36:58.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2500 2022-11-01 21:36:58.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-11-01 21:36:58.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    35095 2022-11-01 21:36:58.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    35036 2022-11-01 21:36:58.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10440 2022-11-01 21:36:59.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    10438 2022-11-01 21:36:59.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12097 2022-11-01 21:36:58.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    12085 2022-11-01 21:36:58.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:36:58.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    45986 2022-11-01 21:36:59.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    45933 2022-11-01 21:36:59.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:36:58.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:38.900832 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    19230 2022-11-01 21:43:38.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-11-01 21:43:38.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:38.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:38.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:38.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-01 21:43:38.000000 mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:38.900832 mypy-boto3-lex-models-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-11-01 21:36:58.000000 mypy-boto3-lex-models-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.387555 mypy-boto3-lex-models-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:40.000000 mypy-boto3-lex-models-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19255 2023-07-03 19:51:01.383556 mypy-boto3-lex-models-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17745 2023-07-03 19:40:40.000000 mypy-boto3-lex-models-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.383556 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-03 19:40:40.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-03 19:40:40.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 19:40:40.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35106 2023-07-03 19:40:42.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35047 2023-07-03 19:40:41.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-07-03 19:40:42.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-07-03 19:40:42.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-03 19:40:42.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-07-03 19:40:42.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:40.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46070 2023-07-03 19:40:43.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46017 2023-07-03 19:40:42.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:40.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.383556 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19255 2023-07-03 19:51:01.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:51:01.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:01.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:01.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:01.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:51:01.000000 mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:01.387555 mypy-boto3-lex-models-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-03 19:40:40.000000 mypy-boto3-lex-models-1.27.0/setup.py
```

### Comparing `mypy-boto3-lex-models-1.26.0.post1/LICENSE` & `mypy-boto3-lex-models-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-lex-models-1.26.0.post1/PKG-INFO` & `mypy-boto3-lex-models-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-models
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.LexModelBuildingService 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.LexModelBuildingService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/
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
 
 <a id="mypy-boto3-lex-models"></a>
 
 # mypy-boto3-lex-models
 
 [![PyPI - mypy-boto3-lex-models](https://img.shields.io/pypi/v/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lex-models?color=blue)](https://pypistats.org/packages/mypy-boto3-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelBuildingService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[boto3.LexModelBuildingService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [mypy-boto3-lex-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,15 +391,14 @@
     BuiltinIntentSlotTypeDef,
     BuiltinSlotTypeMetadataTypeDef,
     CodeHookTypeDef,
     LogSettingsRequestTypeDef,
     LogSettingsResponseTypeDef,
     CreateBotVersionRequestRequestTypeDef,
     IntentTypeDef,
-    ResponseMetadataTypeDef,
     CreateIntentVersionRequestRequestTypeDef,
     InputContextTypeDef,
     KendraConfigurationTypeDef,
     OutputContextTypeDef,
     CreateSlotTypeVersionRequestRequestTypeDef,
     EnumerationValueTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
@@ -406,72 +406,73 @@
     DeleteBotRequestRequestTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteIntentVersionRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteSlotTypeVersionRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetBotAliasRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
     GetBotAliasesRequestRequestTypeDef,
     GetBotChannelAssociationRequestRequestTypeDef,
+    GetBotChannelAssociationResponseTypeDef,
+    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     GetBotChannelAssociationsRequestRequestTypeDef,
     GetBotRequestRequestTypeDef,
+    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
     GetBotVersionsRequestRequestTypeDef,
+    GetBotsRequestGetBotsPaginateTypeDef,
     GetBotsRequestRequestTypeDef,
     GetBuiltinIntentRequestRequestTypeDef,
+    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
     GetBuiltinIntentsRequestRequestTypeDef,
+    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
     GetBuiltinSlotTypesRequestRequestTypeDef,
     GetExportRequestRequestTypeDef,
+    GetExportResponseTypeDef,
     GetImportRequestRequestTypeDef,
+    GetImportResponseTypeDef,
     GetIntentRequestRequestTypeDef,
+    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
     GetIntentVersionsRequestRequestTypeDef,
     IntentMetadataTypeDef,
+    GetIntentsRequestGetIntentsPaginateTypeDef,
     GetIntentsRequestRequestTypeDef,
     GetMigrationRequestRequestTypeDef,
     MigrationAlertTypeDef,
     GetMigrationsRequestRequestTypeDef,
     MigrationSummaryTypeDef,
     GetSlotTypeRequestRequestTypeDef,
+    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
     GetSlotTypeVersionsRequestRequestTypeDef,
     SlotTypeMetadataTypeDef,
+    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetSlotTypesRequestRequestTypeDef,
     GetUtterancesViewRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     MessageTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SlotDefaultValueTypeDef,
     SlotTypeRegexConfigurationTypeDef,
     StartMigrationRequestRequestTypeDef,
+    StartMigrationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UtteranceDataTypeDef,
-    FulfillmentActivityTypeDef,
-    ConversationLogsRequestTypeDef,
-    ConversationLogsResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotVersionsResponseTypeDef,
     GetBotsResponseTypeDef,
-    GetBuiltinIntentResponseTypeDef,
     GetBuiltinIntentsResponseTypeDef,
+    GetBuiltinIntentResponseTypeDef,
     GetBuiltinSlotTypesResponseTypeDef,
-    GetExportResponseTypeDef,
-    GetImportResponseTypeDef,
-    StartMigrationResponseTypeDef,
-    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
-    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
-    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
-    GetBotsRequestGetBotsPaginateTypeDef,
-    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
-    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
-    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
-    GetIntentsRequestGetIntentsPaginateTypeDef,
-    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
-    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
+    FulfillmentActivityTypeDef,
+    ConversationLogsRequestTypeDef,
+    ConversationLogsResponseTypeDef,
     GetIntentVersionsResponseTypeDef,
     GetIntentsResponseTypeDef,
     GetMigrationResponseTypeDef,
     GetMigrationsResponseTypeDef,
     GetSlotTypeVersionsResponseTypeDef,
     GetSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -513,42 +514,42 @@
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

### Comparing `mypy-boto3-lex-models-1.26.0.post1/README.md` & `mypy-boto3-lex-models-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lex-models"></a>
 
 # mypy-boto3-lex-models
 
 [![PyPI - mypy-boto3-lex-models](https://img.shields.io/pypi/v/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lex-models?color=blue)](https://pypistats.org/packages/mypy-boto3-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelBuildingService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[boto3.LexModelBuildingService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [mypy-boto3-lex-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,15 +359,14 @@
     BuiltinIntentSlotTypeDef,
     BuiltinSlotTypeMetadataTypeDef,
     CodeHookTypeDef,
     LogSettingsRequestTypeDef,
     LogSettingsResponseTypeDef,
     CreateBotVersionRequestRequestTypeDef,
     IntentTypeDef,
-    ResponseMetadataTypeDef,
     CreateIntentVersionRequestRequestTypeDef,
     InputContextTypeDef,
     KendraConfigurationTypeDef,
     OutputContextTypeDef,
     CreateSlotTypeVersionRequestRequestTypeDef,
     EnumerationValueTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
@@ -375,72 +374,73 @@
     DeleteBotRequestRequestTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteIntentVersionRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteSlotTypeVersionRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetBotAliasRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
     GetBotAliasesRequestRequestTypeDef,
     GetBotChannelAssociationRequestRequestTypeDef,
+    GetBotChannelAssociationResponseTypeDef,
+    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     GetBotChannelAssociationsRequestRequestTypeDef,
     GetBotRequestRequestTypeDef,
+    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
     GetBotVersionsRequestRequestTypeDef,
+    GetBotsRequestGetBotsPaginateTypeDef,
     GetBotsRequestRequestTypeDef,
     GetBuiltinIntentRequestRequestTypeDef,
+    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
     GetBuiltinIntentsRequestRequestTypeDef,
+    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
     GetBuiltinSlotTypesRequestRequestTypeDef,
     GetExportRequestRequestTypeDef,
+    GetExportResponseTypeDef,
     GetImportRequestRequestTypeDef,
+    GetImportResponseTypeDef,
     GetIntentRequestRequestTypeDef,
+    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
     GetIntentVersionsRequestRequestTypeDef,
     IntentMetadataTypeDef,
+    GetIntentsRequestGetIntentsPaginateTypeDef,
     GetIntentsRequestRequestTypeDef,
     GetMigrationRequestRequestTypeDef,
     MigrationAlertTypeDef,
     GetMigrationsRequestRequestTypeDef,
     MigrationSummaryTypeDef,
     GetSlotTypeRequestRequestTypeDef,
+    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
     GetSlotTypeVersionsRequestRequestTypeDef,
     SlotTypeMetadataTypeDef,
+    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetSlotTypesRequestRequestTypeDef,
     GetUtterancesViewRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     MessageTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SlotDefaultValueTypeDef,
     SlotTypeRegexConfigurationTypeDef,
     StartMigrationRequestRequestTypeDef,
+    StartMigrationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UtteranceDataTypeDef,
-    FulfillmentActivityTypeDef,
-    ConversationLogsRequestTypeDef,
-    ConversationLogsResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotVersionsResponseTypeDef,
     GetBotsResponseTypeDef,
-    GetBuiltinIntentResponseTypeDef,
     GetBuiltinIntentsResponseTypeDef,
+    GetBuiltinIntentResponseTypeDef,
     GetBuiltinSlotTypesResponseTypeDef,
-    GetExportResponseTypeDef,
-    GetImportResponseTypeDef,
-    StartMigrationResponseTypeDef,
-    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
-    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
-    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
-    GetBotsRequestGetBotsPaginateTypeDef,
-    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
-    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
-    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
-    GetIntentsRequestGetIntentsPaginateTypeDef,
-    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
-    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
+    FulfillmentActivityTypeDef,
+    ConversationLogsRequestTypeDef,
+    ConversationLogsResponseTypeDef,
     GetIntentVersionsResponseTypeDef,
     GetIntentsResponseTypeDef,
     GetMigrationResponseTypeDef,
     GetMigrationsResponseTypeDef,
     GetSlotTypeVersionsResponseTypeDef,
     GetSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -482,42 +482,42 @@
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

### Comparing `mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/__init__.py` & `mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/__init__.pyi` & `mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/__main__.py` & `mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LexModelBuildingService 1.26.0\nVersion:        "
-        " 1.26.0.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.LexModelBuildingService 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService\nOther"
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

### Comparing `mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/client.py` & `mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#get_bot_versions)
         """
 
     def get_bots(
         self, *, nextToken: str = ..., maxResults: int = ..., nameContains: str = ...
     ) -> GetBotsResponseTypeDef:
         """
-        Returns bot information as follows * If you provide the `nameContains` field,
+        Returns bot information as follows: * If you provide the `nameContains` field,
         the response includes information for the `$LATEST` version of all bots whose
         name contains the specified string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_bots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#get_bots)
         """
 
@@ -423,16 +423,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#get_intent_versions)
         """
 
     def get_intents(
         self, *, nextToken: str = ..., maxResults: int = ..., nameContains: str = ...
     ) -> GetIntentsResponseTypeDef:
         """
-        Returns intent information as follows * If you specify the `nameContains` field,
-        returns the `$LATEST` version of all intents that contain the specified string.
+        Returns intent information as follows: * If you specify the `nameContains`
+        field, returns the `$LATEST` version of all intents that contain the specified
+        string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_intents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#get_intents)
         """
 
     def get_migration(self, *, migrationId: str) -> GetMigrationResponseTypeDef:
         """
@@ -478,15 +479,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#get_slot_type_versions)
         """
 
     def get_slot_types(
         self, *, nextToken: str = ..., maxResults: int = ..., nameContains: str = ...
     ) -> GetSlotTypesResponseTypeDef:
         """
-        Returns slot type information as follows * If you specify the `nameContains`
+        Returns slot type information as follows: * If you specify the `nameContains`
         field, returns the `$LATEST` version of all slot types that contain the
         specified string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_slot_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#get_slot_types)
         """
```

### Comparing `mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/client.pyi` & `mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_bot_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#get_bot_versions)
         """
     def get_bots(
         self, *, nextToken: str = ..., maxResults: int = ..., nameContains: str = ...
     ) -> GetBotsResponseTypeDef:
         """
-        Returns bot information as follows * If you provide the `nameContains` field,
+        Returns bot information as follows: * If you provide the `nameContains` field,
         the response includes information for the `$LATEST` version of all bots whose
         name contains the specified string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_bots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#get_bots)
         """
     def get_builtin_intent(self, *, signature: str) -> GetBuiltinIntentResponseTypeDef:
@@ -389,16 +389,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_intent_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#get_intent_versions)
         """
     def get_intents(
         self, *, nextToken: str = ..., maxResults: int = ..., nameContains: str = ...
     ) -> GetIntentsResponseTypeDef:
         """
-        Returns intent information as follows * If you specify the `nameContains` field,
-        returns the `$LATEST` version of all intents that contain the specified string.
+        Returns intent information as follows: * If you specify the `nameContains`
+        field, returns the `$LATEST` version of all intents that contain the specified
+        string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_intents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#get_intents)
         """
     def get_migration(self, *, migrationId: str) -> GetMigrationResponseTypeDef:
         """
         Provides details about an ongoing or complete migration from an Amazon Lex V1
@@ -439,15 +440,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_slot_type_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#get_slot_type_versions)
         """
     def get_slot_types(
         self, *, nextToken: str = ..., maxResults: int = ..., nameContains: str = ...
     ) -> GetSlotTypesResponseTypeDef:
         """
-        Returns slot type information as follows * If you specify the `nameContains`
+        Returns slot type information as follows: * If you specify the `nameContains`
         field, returns the `$LATEST` version of all slot types that contain the
         specified string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.get_slot_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#get_slot_types)
         """
     def get_utterances_view(
```

### Comparing `mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/literals.py` & `mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/literals.py`

 * *Files 8% similar despite different names*

```diff
@@ -120,23 +120,25 @@
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
@@ -146,30 +148,35 @@
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
@@ -195,14 +202,15 @@
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
@@ -247,51 +255,57 @@
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
@@ -304,14 +318,15 @@
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
@@ -323,28 +338,35 @@
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
@@ -353,14 +375,15 @@
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
@@ -371,55 +394,64 @@
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

### Comparing `mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/literals.pyi` & `mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/literals.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -118,23 +118,25 @@
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
@@ -144,30 +146,35 @@
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
@@ -193,14 +200,15 @@
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
@@ -245,51 +253,57 @@
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
@@ -302,14 +316,15 @@
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
@@ -321,28 +336,35 @@
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
@@ -351,14 +373,15 @@
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
@@ -369,55 +392,64 @@
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

### Comparing `mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/paginator.py` & `mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -65,183 +65,171 @@
     "GetBuiltinSlotTypesPaginator",
     "GetIntentVersionsPaginator",
     "GetIntentsPaginator",
     "GetSlotTypeVersionsPaginator",
     "GetSlotTypesPaginator",
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
 class GetBotAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotaliasespaginator)
     """
 
     def paginate(
         self,
         *,
         botName: str,
         nameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBotAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotaliasespaginator)
         """
 
-
 class GetBotChannelAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotChannelAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotchannelassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         botName: str,
         botAlias: str,
         nameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBotChannelAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotChannelAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotchannelassociationspaginator)
         """
 
-
 class GetBotVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBotVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotversionspaginator)
         """
 
-
 class GetBotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotspaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotspaginator)
         """
 
-
 class GetBuiltinIntentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinIntents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbuiltinintentspaginator)
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBuiltinIntentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinIntents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbuiltinintentspaginator)
         """
 
-
 class GetBuiltinSlotTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinSlotTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbuiltinslottypespaginator)
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBuiltinSlotTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinSlotTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbuiltinslottypespaginator)
         """
 
-
 class GetIntentVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntentVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetIntentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentversionspaginator)
         """
 
-
 class GetIntentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentspaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetIntentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentspaginator)
         """
 
-
 class GetSlotTypeVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypeVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypeversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetSlotTypeVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypeVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypeversionspaginator)
         """
 
-
 class GetSlotTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypespaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetSlotTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypespaginator)
         """
```

### Comparing `mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/paginator.pyi` & `mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,171 +65,183 @@
     "GetBuiltinSlotTypesPaginator",
     "GetIntentVersionsPaginator",
     "GetIntentsPaginator",
     "GetSlotTypeVersionsPaginator",
     "GetSlotTypesPaginator",
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
 class GetBotAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotaliasespaginator)
     """
 
     def paginate(
         self,
         *,
         botName: str,
         nameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBotAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotaliasespaginator)
         """
 
+
 class GetBotChannelAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotChannelAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotchannelassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         botName: str,
         botAlias: str,
         nameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBotChannelAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotChannelAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotchannelassociationspaginator)
         """
 
+
 class GetBotVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBotVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotversionspaginator)
         """
 
+
 class GetBotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotspaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotspaginator)
         """
 
+
 class GetBuiltinIntentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinIntents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbuiltinintentspaginator)
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBuiltinIntentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinIntents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbuiltinintentspaginator)
         """
 
+
 class GetBuiltinSlotTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinSlotTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbuiltinslottypespaginator)
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetBuiltinSlotTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinSlotTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbuiltinslottypespaginator)
         """
 
+
 class GetIntentVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntentVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetIntentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentversionspaginator)
         """
 
+
 class GetIntentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentspaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetIntentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentspaginator)
         """
 
+
 class GetSlotTypeVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypeVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypeversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetSlotTypeVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypeVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypeversionspaginator)
         """
 
+
 class GetSlotTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypespaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetSlotTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypespaginator)
         """
```

### Comparing `mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/type_defs.py` & `mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     "BuiltinIntentSlotTypeDef",
     "BuiltinSlotTypeMetadataTypeDef",
     "CodeHookTypeDef",
     "LogSettingsRequestTypeDef",
     "LogSettingsResponseTypeDef",
     "CreateBotVersionRequestRequestTypeDef",
     "IntentTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateIntentVersionRequestRequestTypeDef",
     "InputContextTypeDef",
     "KendraConfigurationTypeDef",
     "OutputContextTypeDef",
     "CreateSlotTypeVersionRequestRequestTypeDef",
     "EnumerationValueTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
@@ -72,72 +71,73 @@
     "DeleteBotRequestRequestTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
     "DeleteIntentRequestRequestTypeDef",
     "DeleteIntentVersionRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteSlotTypeVersionRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetBotAliasRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     "GetBotAliasesRequestRequestTypeDef",
     "GetBotChannelAssociationRequestRequestTypeDef",
+    "GetBotChannelAssociationResponseTypeDef",
+    "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     "GetBotChannelAssociationsRequestRequestTypeDef",
     "GetBotRequestRequestTypeDef",
+    "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
     "GetBotVersionsRequestRequestTypeDef",
+    "GetBotsRequestGetBotsPaginateTypeDef",
     "GetBotsRequestRequestTypeDef",
     "GetBuiltinIntentRequestRequestTypeDef",
+    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
     "GetBuiltinIntentsRequestRequestTypeDef",
+    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
     "GetBuiltinSlotTypesRequestRequestTypeDef",
     "GetExportRequestRequestTypeDef",
+    "GetExportResponseTypeDef",
     "GetImportRequestRequestTypeDef",
+    "GetImportResponseTypeDef",
     "GetIntentRequestRequestTypeDef",
+    "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
     "GetIntentVersionsRequestRequestTypeDef",
     "IntentMetadataTypeDef",
+    "GetIntentsRequestGetIntentsPaginateTypeDef",
     "GetIntentsRequestRequestTypeDef",
     "GetMigrationRequestRequestTypeDef",
     "MigrationAlertTypeDef",
     "GetMigrationsRequestRequestTypeDef",
     "MigrationSummaryTypeDef",
     "GetSlotTypeRequestRequestTypeDef",
+    "GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
     "GetSlotTypeVersionsRequestRequestTypeDef",
     "SlotTypeMetadataTypeDef",
+    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
     "GetSlotTypesRequestRequestTypeDef",
     "GetUtterancesViewRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "MessageTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "SlotDefaultValueTypeDef",
     "SlotTypeRegexConfigurationTypeDef",
     "StartMigrationRequestRequestTypeDef",
+    "StartMigrationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UtteranceDataTypeDef",
-    "FulfillmentActivityTypeDef",
-    "ConversationLogsRequestTypeDef",
-    "ConversationLogsResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetBotChannelAssociationResponseTypeDef",
     "GetBotChannelAssociationsResponseTypeDef",
     "GetBotVersionsResponseTypeDef",
     "GetBotsResponseTypeDef",
-    "GetBuiltinIntentResponseTypeDef",
     "GetBuiltinIntentsResponseTypeDef",
+    "GetBuiltinIntentResponseTypeDef",
     "GetBuiltinSlotTypesResponseTypeDef",
-    "GetExportResponseTypeDef",
-    "GetImportResponseTypeDef",
-    "StartMigrationResponseTypeDef",
-    "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
-    "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
-    "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
-    "GetBotsRequestGetBotsPaginateTypeDef",
-    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
-    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
-    "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
-    "GetIntentsRequestGetIntentsPaginateTypeDef",
-    "GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
-    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
+    "FulfillmentActivityTypeDef",
+    "ConversationLogsRequestTypeDef",
+    "ConversationLogsResponseTypeDef",
     "GetIntentVersionsResponseTypeDef",
     "GetIntentsResponseTypeDef",
     "GetMigrationResponseTypeDef",
     "GetMigrationsResponseTypeDef",
     "GetSlotTypeVersionsResponseTypeDef",
     "GetSlotTypesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
@@ -294,25 +294,14 @@
     "IntentTypeDef",
     {
         "intentName": str,
         "intentVersion": str,
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
 _RequiredCreateIntentVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntentVersionRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateIntentVersionRequestRequestTypeDef = TypedDict(
@@ -476,32 +465,52 @@
     "DeleteUtterancesRequestRequestTypeDef",
     {
         "botName": str,
         "userId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBotAliasRequestRequestTypeDef = TypedDict(
     "GetBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
+    "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "botName": str,
+    },
+)
+_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
+    "_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class GetBotAliasesRequestGetBotAliasesPaginateTypeDef(
+    _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetBotAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotAliasesRequestRequestTypeDef",
     {
         "botName": str,
     },
 )
 _OptionalGetBotAliasesRequestRequestTypeDef = TypedDict(
@@ -526,14 +535,54 @@
     {
         "name": str,
         "botName": str,
         "botAlias": str,
     },
 )
 
+GetBotChannelAssociationResponseTypeDef = TypedDict(
+    "GetBotChannelAssociationResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "botAlias": str,
+        "botName": str,
+        "createdDate": datetime,
+        "type": ChannelTypeType,
+        "botConfiguration": Dict[str, str],
+        "status": ChannelStatusType,
+        "failureReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
+    {
+        "botName": str,
+        "botAlias": str,
+    },
+)
+_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef(
+    _RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+    _OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetBotChannelAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotChannelAssociationsRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
     },
 )
@@ -559,14 +608,36 @@
     "GetBotRequestRequestTypeDef",
     {
         "name": str,
         "versionOrAlias": str,
     },
 )
 
+_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetBotVersionsRequestGetBotVersionsPaginateTypeDef(
+    _RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+    _OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetBotVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetBotVersionsRequestRequestTypeDef = TypedDict(
@@ -581,14 +652,23 @@
 
 class GetBotVersionsRequestRequestTypeDef(
     _RequiredGetBotVersionsRequestRequestTypeDef, _OptionalGetBotVersionsRequestRequestTypeDef
 ):
     pass
 
 
+GetBotsRequestGetBotsPaginateTypeDef = TypedDict(
+    "GetBotsRequestGetBotsPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetBotsRequestRequestTypeDef = TypedDict(
     "GetBotsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -598,25 +678,45 @@
 GetBuiltinIntentRequestRequestTypeDef = TypedDict(
     "GetBuiltinIntentRequestRequestTypeDef",
     {
         "signature": str,
     },
 )
 
+GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef = TypedDict(
+    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
+    {
+        "locale": LocaleType,
+        "signatureContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetBuiltinIntentsRequestRequestTypeDef = TypedDict(
     "GetBuiltinIntentsRequestRequestTypeDef",
     {
         "locale": LocaleType,
         "signatureContains": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef = TypedDict(
+    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
+    {
+        "locale": LocaleType,
+        "signatureContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetBuiltinSlotTypesRequestRequestTypeDef = TypedDict(
     "GetBuiltinSlotTypesRequestRequestTypeDef",
     {
         "locale": LocaleType,
         "signatureContains": str,
         "nextToken": str,
         "maxResults": int,
@@ -630,29 +730,79 @@
         "name": str,
         "version": str,
         "resourceType": ResourceTypeType,
         "exportType": ExportTypeType,
     },
 )
 
+GetExportResponseTypeDef = TypedDict(
+    "GetExportResponseTypeDef",
+    {
+        "name": str,
+        "version": str,
+        "resourceType": ResourceTypeType,
+        "exportType": ExportTypeType,
+        "exportStatus": ExportStatusType,
+        "failureReason": str,
+        "url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetImportRequestRequestTypeDef = TypedDict(
     "GetImportRequestRequestTypeDef",
     {
         "importId": str,
     },
 )
 
+GetImportResponseTypeDef = TypedDict(
+    "GetImportResponseTypeDef",
+    {
+        "name": str,
+        "resourceType": ResourceTypeType,
+        "mergeStrategy": MergeStrategyType,
+        "importId": str,
+        "importStatus": ImportStatusType,
+        "failureReason": List[str],
+        "createdDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetIntentRequestRequestTypeDef = TypedDict(
     "GetIntentRequestRequestTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
+_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef(
+    _RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+    _OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetIntentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntentVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetIntentVersionsRequestRequestTypeDef = TypedDict(
@@ -679,14 +829,23 @@
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
     },
     total=False,
 )
 
+GetIntentsRequestGetIntentsPaginateTypeDef = TypedDict(
+    "GetIntentsRequestGetIntentsPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetIntentsRequestRequestTypeDef = TypedDict(
     "GetIntentsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -744,14 +903,36 @@
     "GetSlotTypeRequestRequestTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
+_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef(
+    _RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+    _OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSlotTypeVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
@@ -779,14 +960,23 @@
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
     },
     total=False,
 )
 
+GetSlotTypesRequestGetSlotTypesPaginateTypeDef = TypedDict(
+    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetSlotTypesRequestRequestTypeDef = TypedDict(
     "GetSlotTypesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -833,14 +1023,35 @@
 )
 
 
 class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
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
 SlotDefaultValueTypeDef = TypedDict(
     "SlotDefaultValueTypeDef",
     {
         "defaultValue": str,
     },
 )
 
@@ -858,14 +1069,29 @@
         "v1BotVersion": str,
         "v2BotName": str,
         "v2BotRole": str,
         "migrationStrategy": MigrationStrategyType,
     },
 )
 
+StartMigrationResponseTypeDef = TypedDict(
+    "StartMigrationResponseTypeDef",
+    {
+        "v1BotName": str,
+        "v1BotVersion": str,
+        "v1BotLocale": LocaleType,
+        "v2BotId": str,
+        "v2BotRole": str,
+        "migrationId": str,
+        "migrationStrategy": MigrationStrategyType,
+        "migrationTimestamp": datetime,
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
@@ -878,348 +1104,122 @@
         "distinctUsers": int,
         "firstUtteredDate": datetime,
         "lastUtteredDate": datetime,
     },
     total=False,
 )
 
-_RequiredFulfillmentActivityTypeDef = TypedDict(
-    "_RequiredFulfillmentActivityTypeDef",
-    {
-        "type": FulfillmentActivityTypeType,
-    },
-)
-_OptionalFulfillmentActivityTypeDef = TypedDict(
-    "_OptionalFulfillmentActivityTypeDef",
-    {
-        "codeHook": CodeHookTypeDef,
-    },
-    total=False,
-)
-
-
-class FulfillmentActivityTypeDef(
-    _RequiredFulfillmentActivityTypeDef, _OptionalFulfillmentActivityTypeDef
-):
-    pass
-
-
-ConversationLogsRequestTypeDef = TypedDict(
-    "ConversationLogsRequestTypeDef",
-    {
-        "logSettings": Sequence[LogSettingsRequestTypeDef],
-        "iamRoleArn": str,
-    },
-)
-
-ConversationLogsResponseTypeDef = TypedDict(
-    "ConversationLogsResponseTypeDef",
-    {
-        "logSettings": List[LogSettingsResponseTypeDef],
-        "iamRoleArn": str,
-    },
-    total=False,
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBotChannelAssociationResponseTypeDef = TypedDict(
-    "GetBotChannelAssociationResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "botAlias": str,
-        "botName": str,
-        "createdDate": datetime,
-        "type": ChannelTypeType,
-        "botConfiguration": Dict[str, str],
-        "status": ChannelStatusType,
-        "failureReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetBotChannelAssociationsResponseTypeDef = TypedDict(
     "GetBotChannelAssociationsResponseTypeDef",
     {
         "botChannelAssociations": List[BotChannelAssociationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBotVersionsResponseTypeDef = TypedDict(
     "GetBotVersionsResponseTypeDef",
     {
         "bots": List[BotMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBotsResponseTypeDef = TypedDict(
     "GetBotsResponseTypeDef",
     {
         "bots": List[BotMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetBuiltinIntentsResponseTypeDef = TypedDict(
+    "GetBuiltinIntentsResponseTypeDef",
+    {
+        "intents": List[BuiltinIntentMetadataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBuiltinIntentResponseTypeDef = TypedDict(
     "GetBuiltinIntentResponseTypeDef",
     {
         "signature": str,
         "supportedLocales": List[LocaleType],
         "slots": List[BuiltinIntentSlotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBuiltinIntentsResponseTypeDef = TypedDict(
-    "GetBuiltinIntentsResponseTypeDef",
-    {
-        "intents": List[BuiltinIntentMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBuiltinSlotTypesResponseTypeDef = TypedDict(
     "GetBuiltinSlotTypesResponseTypeDef",
     {
         "slotTypes": List[BuiltinSlotTypeMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetExportResponseTypeDef = TypedDict(
-    "GetExportResponseTypeDef",
-    {
-        "name": str,
-        "version": str,
-        "resourceType": ResourceTypeType,
-        "exportType": ExportTypeType,
-        "exportStatus": ExportStatusType,
-        "failureReason": str,
-        "url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetImportResponseTypeDef = TypedDict(
-    "GetImportResponseTypeDef",
-    {
-        "name": str,
-        "resourceType": ResourceTypeType,
-        "mergeStrategy": MergeStrategyType,
-        "importId": str,
-        "importStatus": ImportStatusType,
-        "failureReason": List[str],
-        "createdDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartMigrationResponseTypeDef = TypedDict(
-    "StartMigrationResponseTypeDef",
-    {
-        "v1BotName": str,
-        "v1BotVersion": str,
-        "v1BotLocale": LocaleType,
-        "v2BotId": str,
-        "v2BotRole": str,
-        "migrationId": str,
-        "migrationStrategy": MigrationStrategyType,
-        "migrationTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
-    "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
-    {
-        "botName": str,
-    },
-)
-_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
-    "_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetBotAliasesRequestGetBotAliasesPaginateTypeDef(
-    _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
-    _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
-    {
-        "botName": str,
-        "botAlias": str,
-    },
-)
-_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef(
-    _RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
-    _OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetBotVersionsRequestGetBotVersionsPaginateTypeDef(
-    _RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
-    _OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
-):
-    pass
-
-
-GetBotsRequestGetBotsPaginateTypeDef = TypedDict(
-    "GetBotsRequestGetBotsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef = TypedDict(
-    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
-    {
-        "locale": LocaleType,
-        "signatureContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef = TypedDict(
-    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
-    {
-        "locale": LocaleType,
-        "signatureContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+_RequiredFulfillmentActivityTypeDef = TypedDict(
+    "_RequiredFulfillmentActivityTypeDef",
     {
-        "name": str,
+        "type": FulfillmentActivityTypeType,
     },
 )
-_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+_OptionalFulfillmentActivityTypeDef = TypedDict(
+    "_OptionalFulfillmentActivityTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "codeHook": CodeHookTypeDef,
     },
     total=False,
 )
 
 
-class GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef(
-    _RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
-    _OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+class FulfillmentActivityTypeDef(
+    _RequiredFulfillmentActivityTypeDef, _OptionalFulfillmentActivityTypeDef
 ):
     pass
 
 
-GetIntentsRequestGetIntentsPaginateTypeDef = TypedDict(
-    "GetIntentsRequestGetIntentsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
+ConversationLogsRequestTypeDef = TypedDict(
+    "ConversationLogsRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "logSettings": Sequence[LogSettingsRequestTypeDef],
+        "iamRoleArn": str,
     },
-    total=False,
 )
 
-
-class GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef(
-    _RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
-    _OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
-):
-    pass
-
-
-GetSlotTypesRequestGetSlotTypesPaginateTypeDef = TypedDict(
-    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
+ConversationLogsResponseTypeDef = TypedDict(
+    "ConversationLogsResponseTypeDef",
     {
-        "nameContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "logSettings": List[LogSettingsResponseTypeDef],
+        "iamRoleArn": str,
     },
     total=False,
 )
 
 GetIntentVersionsResponseTypeDef = TypedDict(
     "GetIntentVersionsResponseTypeDef",
     {
         "intents": List[IntentMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIntentsResponseTypeDef = TypedDict(
     "GetIntentsResponseTypeDef",
     {
         "intents": List[IntentMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMigrationResponseTypeDef = TypedDict(
     "GetMigrationResponseTypeDef",
     {
         "migrationId": str,
@@ -1228,50 +1228,50 @@
         "v1BotLocale": LocaleType,
         "v2BotId": str,
         "v2BotRole": str,
         "migrationStatus": MigrationStatusType,
         "migrationStrategy": MigrationStrategyType,
         "migrationTimestamp": datetime,
         "alerts": List[MigrationAlertTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMigrationsResponseTypeDef = TypedDict(
     "GetMigrationsResponseTypeDef",
     {
         "migrationSummaries": List[MigrationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSlotTypeVersionsResponseTypeDef = TypedDict(
     "GetSlotTypeVersionsResponseTypeDef",
     {
         "slotTypes": List[SlotTypeMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSlotTypesResponseTypeDef = TypedDict(
     "GetSlotTypesResponseTypeDef",
     {
         "slotTypes": List[SlotTypeMetadataTypeDef],
         "nextToken": str,
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
 
 _RequiredStartImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportRequestRequestTypeDef",
     {
         "payload": Union[str, bytes, IO[Any], StreamingBody],
@@ -1300,15 +1300,15 @@
         "name": str,
         "resourceType": ResourceTypeType,
         "mergeStrategy": MergeStrategyType,
         "importId": str,
         "importStatus": ImportStatusType,
         "tags": List[TagTypeDef],
         "createdDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1427,15 +1427,15 @@
         "description": str,
         "botVersion": str,
         "botName": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutBotAliasResponseTypeDef = TypedDict(
     "PutBotAliasResponseTypeDef",
     {
         "name": str,
@@ -1443,15 +1443,15 @@
         "botVersion": str,
         "botName": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "name": str,
@@ -1467,15 +1467,15 @@
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "enableModelImprovements": bool,
         "detectSentiment": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FollowUpPromptTypeDef = TypedDict(
     "FollowUpPromptTypeDef",
     {
         "prompt": PromptTypeDef,
@@ -1500,15 +1500,15 @@
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "detectSentiment": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBotRequestRequestTypeDef = TypedDict(
     "_RequiredPutBotRequestRequestTypeDef",
     {
         "name": str,
@@ -1562,15 +1562,15 @@
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "createVersion": bool,
         "detectSentiment": bool,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSlotTypeDef = TypedDict(
     "_RequiredSlotTypeDef",
     {
         "name": str,
@@ -1607,15 +1607,15 @@
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSlotTypeResponseTypeDef = TypedDict(
     "GetSlotTypeResponseTypeDef",
     {
         "name": str,
@@ -1624,15 +1624,15 @@
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutSlotTypeRequestRequestTypeDef",
     {
         "name": str,
@@ -1669,33 +1669,33 @@
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUtterancesViewResponseTypeDef = TypedDict(
     "GetUtterancesViewResponseTypeDef",
     {
         "botName": str,
         "utterances": List[UtteranceListTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBotAliasesResponseTypeDef = TypedDict(
     "GetBotAliasesResponseTypeDef",
     {
         "BotAliases": List[BotAliasMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateIntentVersionResponseTypeDef = TypedDict(
     "CreateIntentVersionResponseTypeDef",
     {
         "name": str,
@@ -1712,15 +1712,15 @@
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIntentResponseTypeDef = TypedDict(
     "GetIntentResponseTypeDef",
     {
         "name": str,
@@ -1737,15 +1737,15 @@
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutIntentRequestRequestTypeDef = TypedDict(
     "_RequiredPutIntentRequestRequestTypeDef",
     {
         "name": str,
@@ -1798,10 +1798,10 @@
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "createVersion": bool,
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models/type_defs.pyi` & `mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,14 @@
     "BuiltinIntentSlotTypeDef",
     "BuiltinSlotTypeMetadataTypeDef",
     "CodeHookTypeDef",
     "LogSettingsRequestTypeDef",
     "LogSettingsResponseTypeDef",
     "CreateBotVersionRequestRequestTypeDef",
     "IntentTypeDef",
-    "ResponseMetadataTypeDef",
     "CreateIntentVersionRequestRequestTypeDef",
     "InputContextTypeDef",
     "KendraConfigurationTypeDef",
     "OutputContextTypeDef",
     "CreateSlotTypeVersionRequestRequestTypeDef",
     "EnumerationValueTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
@@ -71,72 +70,73 @@
     "DeleteBotRequestRequestTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
     "DeleteIntentRequestRequestTypeDef",
     "DeleteIntentVersionRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteSlotTypeVersionRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetBotAliasRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     "GetBotAliasesRequestRequestTypeDef",
     "GetBotChannelAssociationRequestRequestTypeDef",
+    "GetBotChannelAssociationResponseTypeDef",
+    "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     "GetBotChannelAssociationsRequestRequestTypeDef",
     "GetBotRequestRequestTypeDef",
+    "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
     "GetBotVersionsRequestRequestTypeDef",
+    "GetBotsRequestGetBotsPaginateTypeDef",
     "GetBotsRequestRequestTypeDef",
     "GetBuiltinIntentRequestRequestTypeDef",
+    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
     "GetBuiltinIntentsRequestRequestTypeDef",
+    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
     "GetBuiltinSlotTypesRequestRequestTypeDef",
     "GetExportRequestRequestTypeDef",
+    "GetExportResponseTypeDef",
     "GetImportRequestRequestTypeDef",
+    "GetImportResponseTypeDef",
     "GetIntentRequestRequestTypeDef",
+    "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
     "GetIntentVersionsRequestRequestTypeDef",
     "IntentMetadataTypeDef",
+    "GetIntentsRequestGetIntentsPaginateTypeDef",
     "GetIntentsRequestRequestTypeDef",
     "GetMigrationRequestRequestTypeDef",
     "MigrationAlertTypeDef",
     "GetMigrationsRequestRequestTypeDef",
     "MigrationSummaryTypeDef",
     "GetSlotTypeRequestRequestTypeDef",
+    "GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
     "GetSlotTypeVersionsRequestRequestTypeDef",
     "SlotTypeMetadataTypeDef",
+    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
     "GetSlotTypesRequestRequestTypeDef",
     "GetUtterancesViewRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "MessageTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "SlotDefaultValueTypeDef",
     "SlotTypeRegexConfigurationTypeDef",
     "StartMigrationRequestRequestTypeDef",
+    "StartMigrationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UtteranceDataTypeDef",
-    "FulfillmentActivityTypeDef",
-    "ConversationLogsRequestTypeDef",
-    "ConversationLogsResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetBotChannelAssociationResponseTypeDef",
     "GetBotChannelAssociationsResponseTypeDef",
     "GetBotVersionsResponseTypeDef",
     "GetBotsResponseTypeDef",
-    "GetBuiltinIntentResponseTypeDef",
     "GetBuiltinIntentsResponseTypeDef",
+    "GetBuiltinIntentResponseTypeDef",
     "GetBuiltinSlotTypesResponseTypeDef",
-    "GetExportResponseTypeDef",
-    "GetImportResponseTypeDef",
-    "StartMigrationResponseTypeDef",
-    "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
-    "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
-    "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
-    "GetBotsRequestGetBotsPaginateTypeDef",
-    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
-    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
-    "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
-    "GetIntentsRequestGetIntentsPaginateTypeDef",
-    "GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
-    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
+    "FulfillmentActivityTypeDef",
+    "ConversationLogsRequestTypeDef",
+    "ConversationLogsResponseTypeDef",
     "GetIntentVersionsResponseTypeDef",
     "GetIntentsResponseTypeDef",
     "GetMigrationResponseTypeDef",
     "GetMigrationsResponseTypeDef",
     "GetSlotTypeVersionsResponseTypeDef",
     "GetSlotTypesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
@@ -289,25 +289,14 @@
     "IntentTypeDef",
     {
         "intentName": str,
         "intentVersion": str,
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
 _RequiredCreateIntentVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntentVersionRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateIntentVersionRequestRequestTypeDef = TypedDict(
@@ -463,32 +452,50 @@
     "DeleteUtterancesRequestRequestTypeDef",
     {
         "botName": str,
         "userId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBotAliasRequestRequestTypeDef = TypedDict(
     "GetBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
+    "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "botName": str,
+    },
+)
+_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
+    "_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class GetBotAliasesRequestGetBotAliasesPaginateTypeDef(
+    _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+):
+    pass
+
 _RequiredGetBotAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotAliasesRequestRequestTypeDef",
     {
         "botName": str,
     },
 )
 _OptionalGetBotAliasesRequestRequestTypeDef = TypedDict(
@@ -511,14 +518,52 @@
     {
         "name": str,
         "botName": str,
         "botAlias": str,
     },
 )
 
+GetBotChannelAssociationResponseTypeDef = TypedDict(
+    "GetBotChannelAssociationResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "botAlias": str,
+        "botName": str,
+        "createdDate": datetime,
+        "type": ChannelTypeType,
+        "botConfiguration": Dict[str, str],
+        "status": ChannelStatusType,
+        "failureReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
+    {
+        "botName": str,
+        "botAlias": str,
+    },
+)
+_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef(
+    _RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+    _OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetBotChannelAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotChannelAssociationsRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
     },
 )
@@ -542,14 +587,34 @@
     "GetBotRequestRequestTypeDef",
     {
         "name": str,
         "versionOrAlias": str,
     },
 )
 
+_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetBotVersionsRequestGetBotVersionsPaginateTypeDef(
+    _RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+    _OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetBotVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetBotVersionsRequestRequestTypeDef = TypedDict(
@@ -562,14 +627,23 @@
 )
 
 class GetBotVersionsRequestRequestTypeDef(
     _RequiredGetBotVersionsRequestRequestTypeDef, _OptionalGetBotVersionsRequestRequestTypeDef
 ):
     pass
 
+GetBotsRequestGetBotsPaginateTypeDef = TypedDict(
+    "GetBotsRequestGetBotsPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetBotsRequestRequestTypeDef = TypedDict(
     "GetBotsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -579,25 +653,45 @@
 GetBuiltinIntentRequestRequestTypeDef = TypedDict(
     "GetBuiltinIntentRequestRequestTypeDef",
     {
         "signature": str,
     },
 )
 
+GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef = TypedDict(
+    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
+    {
+        "locale": LocaleType,
+        "signatureContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetBuiltinIntentsRequestRequestTypeDef = TypedDict(
     "GetBuiltinIntentsRequestRequestTypeDef",
     {
         "locale": LocaleType,
         "signatureContains": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef = TypedDict(
+    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
+    {
+        "locale": LocaleType,
+        "signatureContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetBuiltinSlotTypesRequestRequestTypeDef = TypedDict(
     "GetBuiltinSlotTypesRequestRequestTypeDef",
     {
         "locale": LocaleType,
         "signatureContains": str,
         "nextToken": str,
         "maxResults": int,
@@ -611,29 +705,77 @@
         "name": str,
         "version": str,
         "resourceType": ResourceTypeType,
         "exportType": ExportTypeType,
     },
 )
 
+GetExportResponseTypeDef = TypedDict(
+    "GetExportResponseTypeDef",
+    {
+        "name": str,
+        "version": str,
+        "resourceType": ResourceTypeType,
+        "exportType": ExportTypeType,
+        "exportStatus": ExportStatusType,
+        "failureReason": str,
+        "url": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetImportRequestRequestTypeDef = TypedDict(
     "GetImportRequestRequestTypeDef",
     {
         "importId": str,
     },
 )
 
+GetImportResponseTypeDef = TypedDict(
+    "GetImportResponseTypeDef",
+    {
+        "name": str,
+        "resourceType": ResourceTypeType,
+        "mergeStrategy": MergeStrategyType,
+        "importId": str,
+        "importStatus": ImportStatusType,
+        "failureReason": List[str],
+        "createdDate": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetIntentRequestRequestTypeDef = TypedDict(
     "GetIntentRequestRequestTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
+_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef(
+    _RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+    _OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetIntentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntentVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetIntentVersionsRequestRequestTypeDef = TypedDict(
@@ -658,14 +800,23 @@
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
     },
     total=False,
 )
 
+GetIntentsRequestGetIntentsPaginateTypeDef = TypedDict(
+    "GetIntentsRequestGetIntentsPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetIntentsRequestRequestTypeDef = TypedDict(
     "GetIntentsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -723,14 +874,34 @@
     "GetSlotTypeRequestRequestTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
+_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef(
+    _RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+    _OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSlotTypeVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
@@ -756,14 +927,23 @@
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
     },
     total=False,
 )
 
+GetSlotTypesRequestGetSlotTypesPaginateTypeDef = TypedDict(
+    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetSlotTypesRequestRequestTypeDef = TypedDict(
     "GetSlotTypesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -808,14 +988,35 @@
     },
     total=False,
 )
 
 class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
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
 SlotDefaultValueTypeDef = TypedDict(
     "SlotDefaultValueTypeDef",
     {
         "defaultValue": str,
     },
 )
 
@@ -833,14 +1034,29 @@
         "v1BotVersion": str,
         "v2BotName": str,
         "v2BotRole": str,
         "migrationStrategy": MigrationStrategyType,
     },
 )
 
+StartMigrationResponseTypeDef = TypedDict(
+    "StartMigrationResponseTypeDef",
+    {
+        "v1BotName": str,
+        "v1BotVersion": str,
+        "v1BotLocale": LocaleType,
+        "v2BotId": str,
+        "v2BotRole": str,
+        "migrationId": str,
+        "migrationStrategy": MigrationStrategyType,
+        "migrationTimestamp": datetime,
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
@@ -853,336 +1069,120 @@
         "distinctUsers": int,
         "firstUtteredDate": datetime,
         "lastUtteredDate": datetime,
     },
     total=False,
 )
 
-_RequiredFulfillmentActivityTypeDef = TypedDict(
-    "_RequiredFulfillmentActivityTypeDef",
-    {
-        "type": FulfillmentActivityTypeType,
-    },
-)
-_OptionalFulfillmentActivityTypeDef = TypedDict(
-    "_OptionalFulfillmentActivityTypeDef",
-    {
-        "codeHook": CodeHookTypeDef,
-    },
-    total=False,
-)
-
-class FulfillmentActivityTypeDef(
-    _RequiredFulfillmentActivityTypeDef, _OptionalFulfillmentActivityTypeDef
-):
-    pass
-
-ConversationLogsRequestTypeDef = TypedDict(
-    "ConversationLogsRequestTypeDef",
-    {
-        "logSettings": Sequence[LogSettingsRequestTypeDef],
-        "iamRoleArn": str,
-    },
-)
-
-ConversationLogsResponseTypeDef = TypedDict(
-    "ConversationLogsResponseTypeDef",
-    {
-        "logSettings": List[LogSettingsResponseTypeDef],
-        "iamRoleArn": str,
-    },
-    total=False,
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBotChannelAssociationResponseTypeDef = TypedDict(
-    "GetBotChannelAssociationResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "botAlias": str,
-        "botName": str,
-        "createdDate": datetime,
-        "type": ChannelTypeType,
-        "botConfiguration": Dict[str, str],
-        "status": ChannelStatusType,
-        "failureReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetBotChannelAssociationsResponseTypeDef = TypedDict(
     "GetBotChannelAssociationsResponseTypeDef",
     {
         "botChannelAssociations": List[BotChannelAssociationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBotVersionsResponseTypeDef = TypedDict(
     "GetBotVersionsResponseTypeDef",
     {
         "bots": List[BotMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBotsResponseTypeDef = TypedDict(
     "GetBotsResponseTypeDef",
     {
         "bots": List[BotMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetBuiltinIntentsResponseTypeDef = TypedDict(
+    "GetBuiltinIntentsResponseTypeDef",
+    {
+        "intents": List[BuiltinIntentMetadataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBuiltinIntentResponseTypeDef = TypedDict(
     "GetBuiltinIntentResponseTypeDef",
     {
         "signature": str,
         "supportedLocales": List[LocaleType],
         "slots": List[BuiltinIntentSlotTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetBuiltinIntentsResponseTypeDef = TypedDict(
-    "GetBuiltinIntentsResponseTypeDef",
-    {
-        "intents": List[BuiltinIntentMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBuiltinSlotTypesResponseTypeDef = TypedDict(
     "GetBuiltinSlotTypesResponseTypeDef",
     {
         "slotTypes": List[BuiltinSlotTypeMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetExportResponseTypeDef = TypedDict(
-    "GetExportResponseTypeDef",
-    {
-        "name": str,
-        "version": str,
-        "resourceType": ResourceTypeType,
-        "exportType": ExportTypeType,
-        "exportStatus": ExportStatusType,
-        "failureReason": str,
-        "url": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetImportResponseTypeDef = TypedDict(
-    "GetImportResponseTypeDef",
-    {
-        "name": str,
-        "resourceType": ResourceTypeType,
-        "mergeStrategy": MergeStrategyType,
-        "importId": str,
-        "importStatus": ImportStatusType,
-        "failureReason": List[str],
-        "createdDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartMigrationResponseTypeDef = TypedDict(
-    "StartMigrationResponseTypeDef",
-    {
-        "v1BotName": str,
-        "v1BotVersion": str,
-        "v1BotLocale": LocaleType,
-        "v2BotId": str,
-        "v2BotRole": str,
-        "migrationId": str,
-        "migrationStrategy": MigrationStrategyType,
-        "migrationTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
-    "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
-    {
-        "botName": str,
-    },
-)
-_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
-    "_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetBotAliasesRequestGetBotAliasesPaginateTypeDef(
-    _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
-    _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
-):
-    pass
-
-_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
-    {
-        "botName": str,
-        "botAlias": str,
-    },
-)
-_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef(
-    _RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
-    _OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
-):
-    pass
-
-_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class GetBotVersionsRequestGetBotVersionsPaginateTypeDef(
-    _RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
-    _OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
-):
-    pass
-
-GetBotsRequestGetBotsPaginateTypeDef = TypedDict(
-    "GetBotsRequestGetBotsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef = TypedDict(
-    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
-    {
-        "locale": LocaleType,
-        "signatureContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef = TypedDict(
-    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
-    {
-        "locale": LocaleType,
-        "signatureContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+_RequiredFulfillmentActivityTypeDef = TypedDict(
+    "_RequiredFulfillmentActivityTypeDef",
     {
-        "name": str,
+        "type": FulfillmentActivityTypeType,
     },
 )
-_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+_OptionalFulfillmentActivityTypeDef = TypedDict(
+    "_OptionalFulfillmentActivityTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "codeHook": CodeHookTypeDef,
     },
     total=False,
 )
 
-class GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef(
-    _RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
-    _OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+class FulfillmentActivityTypeDef(
+    _RequiredFulfillmentActivityTypeDef, _OptionalFulfillmentActivityTypeDef
 ):
     pass
 
-GetIntentsRequestGetIntentsPaginateTypeDef = TypedDict(
-    "GetIntentsRequestGetIntentsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
+ConversationLogsRequestTypeDef = TypedDict(
+    "ConversationLogsRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "logSettings": Sequence[LogSettingsRequestTypeDef],
+        "iamRoleArn": str,
     },
-    total=False,
 )
 
-class GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef(
-    _RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
-    _OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
-):
-    pass
-
-GetSlotTypesRequestGetSlotTypesPaginateTypeDef = TypedDict(
-    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
+ConversationLogsResponseTypeDef = TypedDict(
+    "ConversationLogsResponseTypeDef",
     {
-        "nameContains": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "logSettings": List[LogSettingsResponseTypeDef],
+        "iamRoleArn": str,
     },
     total=False,
 )
 
 GetIntentVersionsResponseTypeDef = TypedDict(
     "GetIntentVersionsResponseTypeDef",
     {
         "intents": List[IntentMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIntentsResponseTypeDef = TypedDict(
     "GetIntentsResponseTypeDef",
     {
         "intents": List[IntentMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMigrationResponseTypeDef = TypedDict(
     "GetMigrationResponseTypeDef",
     {
         "migrationId": str,
@@ -1191,50 +1191,50 @@
         "v1BotLocale": LocaleType,
         "v2BotId": str,
         "v2BotRole": str,
         "migrationStatus": MigrationStatusType,
         "migrationStrategy": MigrationStrategyType,
         "migrationTimestamp": datetime,
         "alerts": List[MigrationAlertTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMigrationsResponseTypeDef = TypedDict(
     "GetMigrationsResponseTypeDef",
     {
         "migrationSummaries": List[MigrationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSlotTypeVersionsResponseTypeDef = TypedDict(
     "GetSlotTypeVersionsResponseTypeDef",
     {
         "slotTypes": List[SlotTypeMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSlotTypesResponseTypeDef = TypedDict(
     "GetSlotTypesResponseTypeDef",
     {
         "slotTypes": List[SlotTypeMetadataTypeDef],
         "nextToken": str,
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
 
 _RequiredStartImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportRequestRequestTypeDef",
     {
         "payload": Union[str, bytes, IO[Any], StreamingBody],
@@ -1261,15 +1261,15 @@
         "name": str,
         "resourceType": ResourceTypeType,
         "mergeStrategy": MergeStrategyType,
         "importId": str,
         "importStatus": ImportStatusType,
         "tags": List[TagTypeDef],
         "createdDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1382,15 +1382,15 @@
         "description": str,
         "botVersion": str,
         "botName": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutBotAliasResponseTypeDef = TypedDict(
     "PutBotAliasResponseTypeDef",
     {
         "name": str,
@@ -1398,15 +1398,15 @@
         "botVersion": str,
         "botName": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "name": str,
@@ -1422,15 +1422,15 @@
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "enableModelImprovements": bool,
         "detectSentiment": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FollowUpPromptTypeDef = TypedDict(
     "FollowUpPromptTypeDef",
     {
         "prompt": PromptTypeDef,
@@ -1455,15 +1455,15 @@
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "detectSentiment": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBotRequestRequestTypeDef = TypedDict(
     "_RequiredPutBotRequestRequestTypeDef",
     {
         "name": str,
@@ -1515,15 +1515,15 @@
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "createVersion": bool,
         "detectSentiment": bool,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSlotTypeDef = TypedDict(
     "_RequiredSlotTypeDef",
     {
         "name": str,
@@ -1558,15 +1558,15 @@
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSlotTypeResponseTypeDef = TypedDict(
     "GetSlotTypeResponseTypeDef",
     {
         "name": str,
@@ -1575,15 +1575,15 @@
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutSlotTypeRequestRequestTypeDef",
     {
         "name": str,
@@ -1618,33 +1618,33 @@
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUtterancesViewResponseTypeDef = TypedDict(
     "GetUtterancesViewResponseTypeDef",
     {
         "botName": str,
         "utterances": List[UtteranceListTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBotAliasesResponseTypeDef = TypedDict(
     "GetBotAliasesResponseTypeDef",
     {
         "BotAliases": List[BotAliasMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateIntentVersionResponseTypeDef = TypedDict(
     "CreateIntentVersionResponseTypeDef",
     {
         "name": str,
@@ -1661,15 +1661,15 @@
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIntentResponseTypeDef = TypedDict(
     "GetIntentResponseTypeDef",
     {
         "name": str,
@@ -1686,15 +1686,15 @@
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutIntentRequestRequestTypeDef = TypedDict(
     "_RequiredPutIntentRequestRequestTypeDef",
     {
         "name": str,
@@ -1745,10 +1745,10 @@
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "createVersion": bool,
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models.egg-info/PKG-INFO` & `mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-models
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.LexModelBuildingService 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.LexModelBuildingService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/
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
 
 <a id="mypy-boto3-lex-models"></a>
 
 # mypy-boto3-lex-models
 
 [![PyPI - mypy-boto3-lex-models](https://img.shields.io/pypi/v/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lex-models?color=blue)](https://pypistats.org/packages/mypy-boto3-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelBuildingService 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[boto3.LexModelBuildingService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [mypy-boto3-lex-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,15 +391,14 @@
     BuiltinIntentSlotTypeDef,
     BuiltinSlotTypeMetadataTypeDef,
     CodeHookTypeDef,
     LogSettingsRequestTypeDef,
     LogSettingsResponseTypeDef,
     CreateBotVersionRequestRequestTypeDef,
     IntentTypeDef,
-    ResponseMetadataTypeDef,
     CreateIntentVersionRequestRequestTypeDef,
     InputContextTypeDef,
     KendraConfigurationTypeDef,
     OutputContextTypeDef,
     CreateSlotTypeVersionRequestRequestTypeDef,
     EnumerationValueTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
@@ -406,72 +406,73 @@
     DeleteBotRequestRequestTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteIntentVersionRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteSlotTypeVersionRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetBotAliasRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
     GetBotAliasesRequestRequestTypeDef,
     GetBotChannelAssociationRequestRequestTypeDef,
+    GetBotChannelAssociationResponseTypeDef,
+    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     GetBotChannelAssociationsRequestRequestTypeDef,
     GetBotRequestRequestTypeDef,
+    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
     GetBotVersionsRequestRequestTypeDef,
+    GetBotsRequestGetBotsPaginateTypeDef,
     GetBotsRequestRequestTypeDef,
     GetBuiltinIntentRequestRequestTypeDef,
+    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
     GetBuiltinIntentsRequestRequestTypeDef,
+    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
     GetBuiltinSlotTypesRequestRequestTypeDef,
     GetExportRequestRequestTypeDef,
+    GetExportResponseTypeDef,
     GetImportRequestRequestTypeDef,
+    GetImportResponseTypeDef,
     GetIntentRequestRequestTypeDef,
+    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
     GetIntentVersionsRequestRequestTypeDef,
     IntentMetadataTypeDef,
+    GetIntentsRequestGetIntentsPaginateTypeDef,
     GetIntentsRequestRequestTypeDef,
     GetMigrationRequestRequestTypeDef,
     MigrationAlertTypeDef,
     GetMigrationsRequestRequestTypeDef,
     MigrationSummaryTypeDef,
     GetSlotTypeRequestRequestTypeDef,
+    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
     GetSlotTypeVersionsRequestRequestTypeDef,
     SlotTypeMetadataTypeDef,
+    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetSlotTypesRequestRequestTypeDef,
     GetUtterancesViewRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     MessageTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     SlotDefaultValueTypeDef,
     SlotTypeRegexConfigurationTypeDef,
     StartMigrationRequestRequestTypeDef,
+    StartMigrationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UtteranceDataTypeDef,
-    FulfillmentActivityTypeDef,
-    ConversationLogsRequestTypeDef,
-    ConversationLogsResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotVersionsResponseTypeDef,
     GetBotsResponseTypeDef,
-    GetBuiltinIntentResponseTypeDef,
     GetBuiltinIntentsResponseTypeDef,
+    GetBuiltinIntentResponseTypeDef,
     GetBuiltinSlotTypesResponseTypeDef,
-    GetExportResponseTypeDef,
-    GetImportResponseTypeDef,
-    StartMigrationResponseTypeDef,
-    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
-    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
-    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
-    GetBotsRequestGetBotsPaginateTypeDef,
-    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
-    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
-    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
-    GetIntentsRequestGetIntentsPaginateTypeDef,
-    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
-    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
+    FulfillmentActivityTypeDef,
+    ConversationLogsRequestTypeDef,
+    ConversationLogsResponseTypeDef,
     GetIntentVersionsResponseTypeDef,
     GetIntentsResponseTypeDef,
     GetMigrationResponseTypeDef,
     GetMigrationsResponseTypeDef,
     GetSlotTypeVersionsResponseTypeDef,
     GetSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -513,42 +514,42 @@
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

### Comparing `mypy-boto3-lex-models-1.26.0.post1/mypy_boto3_lex_models.egg-info/SOURCES.txt` & `mypy-boto3-lex-models-1.27.0/mypy_boto3_lex_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.26.0.post1/setup.py` & `mypy-boto3-lex-models-1.27.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-lex-models.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lex-models",
-    version="1.26.0.post1",
+    version="1.27.0",
     packages=["mypy_boto3_lex_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LexModelBuildingService 1.26.0 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.LexModelBuildingService 1.27.0 service generated with"
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
     keywords="boto3 lex-models type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_lex_models": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_lex_models": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/",
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


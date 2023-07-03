# Comparing `tmp/mypy-boto3-cloudtrail-1.26.72.tar.gz` & `tmp/mypy-boto3-cloudtrail-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudtrail-1.26.72.tar", last modified: Wed Feb 15 22:27:56 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudtrail-1.27.0.tar", last modified: Mon Jul  3 19:50:31 2023, max compression
```

## Comparing `mypy-boto3-cloudtrail-1.26.72.tar` & `mypy-boto3-cloudtrail-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.846127 mypy-boto3-cloudtrail-1.26.72/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-02-15 22:27:56.842126 mypy-boto3-cloudtrail-1.26.72/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16189 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.834126 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37753 2023-02-15 22:27:03.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37696 2023-02-15 22:27:03.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-02-15 22:27:03.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-02-15 22:27:03.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-02-15 22:27:03.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-02-15 22:27:03.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39728 2023-02-15 22:27:05.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39689 2023-02-15 22:27:04.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.842126 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-02-15 22:27:56.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-15 22:27:56.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 22:27:56.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-15 22:27:56.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 22:27:56.846127 mypy-boto3-cloudtrail-1.26.72/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.378978 mypy-boto3-cloudtrail-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:59.000000 mypy-boto3-cloudtrail-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-07-03 19:50:31.370977 mypy-boto3-cloudtrail-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-07-03 19:33:59.000000 mypy-boto3-cloudtrail-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.370977 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-03 19:33:59.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-03 19:33:59.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:33:59.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39076 2023-07-03 19:33:59.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39017 2023-07-03 19:33:59.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10111 2023-07-03 19:33:59.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-07-03 19:33:59.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-07-03 19:33:59.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-07-03 19:33:59.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:59.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39814 2023-07-03 19:34:01.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39779 2023-07-03 19:34:01.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:59.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.370977 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-07-03 19:50:31.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:50:31.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:31.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:50:31.000000 mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:31.378978 mypy-boto3-cloudtrail-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:33:59.000000 mypy-boto3-cloudtrail-1.27.0/setup.py
```

### Comparing `mypy-boto3-cloudtrail-1.26.72/LICENSE` & `mypy-boto3-cloudtrail-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-cloudtrail-1.26.72/PKG-INFO` & `mypy-boto3-cloudtrail-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudtrail
-Version: 1.26.72
-Summary: Type annotations for boto3.CloudTrail 1.26.72 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudTrail 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-cloudtrail"></a>
 
 # mypy-boto3-cloudtrail
 
 [![PyPI - mypy-boto3-cloudtrail](https://img.shields.io/pypi/v/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudtrail?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [mypy-boto3-cloudtrail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,17 +350,18 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudtrail.type_defs import (
     TagTypeDef,
     AdvancedFieldSelectorTypeDef,
     CancelQueryRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelQueryResponseTypeDef,
     ChannelTypeDef,
     DestinationTypeDef,
+    CreateTrailResponseTypeDef,
     DataResourceTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteEventDataStoreRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteTrailRequestRequestTypeDef,
     DeregisterOrganizationDelegatedAdminRequestRequestTypeDef,
     DescribeQueryRequestRequestTypeDef,
@@ -375,52 +376,58 @@
     GetImportRequestRequestTypeDef,
     ImportStatisticsTypeDef,
     GetInsightSelectorsRequestRequestTypeDef,
     InsightSelectorTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
     GetTrailRequestRequestTypeDef,
     GetTrailStatusRequestRequestTypeDef,
+    GetTrailStatusResponseTypeDef,
     ImportFailureListItemTypeDef,
     S3ImportSourceTypeDef,
     ImportsListItemTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListEventDataStoresRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
     ListImportFailuresRequestRequestTypeDef,
+    ListImportsRequestListImportsPaginateTypeDef,
     ListImportsRequestRequestTypeDef,
+    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     PublicKeyTypeDef,
     ListQueriesRequestRequestTypeDef,
     QueryTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
+    ListTrailsRequestListTrailsPaginateTypeDef,
     ListTrailsRequestRequestTypeDef,
     TrailInfoTypeDef,
     LookupAttributeTypeDef,
+    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    PutResourcePolicyResponseTypeDef,
     RegisterOrganizationDelegatedAdminRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RestoreEventDataStoreRequestRequestTypeDef,
+    StartEventDataStoreIngestionRequestRequestTypeDef,
     StartLoggingRequestRequestTypeDef,
     StartQueryRequestRequestTypeDef,
+    StartQueryResponseTypeDef,
+    StopEventDataStoreIngestionRequestRequestTypeDef,
     StopImportRequestRequestTypeDef,
     StopLoggingRequestRequestTypeDef,
     UpdateTrailRequestRequestTypeDef,
+    UpdateTrailResponseTypeDef,
     AddTagsRequestRequestTypeDef,
     CreateTrailRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
     ResourceTagTypeDef,
     AdvancedEventSelectorTypeDef,
-    CancelQueryResponseTypeDef,
-    CreateTrailResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetTrailStatusResponseTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    StartQueryResponseTypeDef,
-    UpdateTrailResponseTypeDef,
     ListChannelsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     CreateChannelResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
     EventSelectorTypeDef,
     DescribeQueryResponseTypeDef,
@@ -430,19 +437,14 @@
     GetInsightSelectorsResponseTypeDef,
     PutInsightSelectorsRequestRequestTypeDef,
     PutInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     ListImportFailuresResponseTypeDef,
     ImportSourceTypeDef,
     ListImportsResponseTypeDef,
-    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
-    ListImportsRequestListImportsPaginateTypeDef,
-    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
-    ListTrailsRequestListTrailsPaginateTypeDef,
     ListPublicKeysResponseTypeDef,
     ListQueriesResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupEventsRequestLookupEventsPaginateTypeDef,
     LookupEventsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     CreateEventDataStoreRequestRequestTypeDef,
@@ -473,42 +475,42 @@
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

### Comparing `mypy-boto3-cloudtrail-1.26.72/README.md` & `mypy-boto3-cloudtrail-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cloudtrail"></a>
 
 # mypy-boto3-cloudtrail
 
 [![PyPI - mypy-boto3-cloudtrail](https://img.shields.io/pypi/v/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudtrail?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [mypy-boto3-cloudtrail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,17 +318,18 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudtrail.type_defs import (
     TagTypeDef,
     AdvancedFieldSelectorTypeDef,
     CancelQueryRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelQueryResponseTypeDef,
     ChannelTypeDef,
     DestinationTypeDef,
+    CreateTrailResponseTypeDef,
     DataResourceTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteEventDataStoreRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteTrailRequestRequestTypeDef,
     DeregisterOrganizationDelegatedAdminRequestRequestTypeDef,
     DescribeQueryRequestRequestTypeDef,
@@ -343,52 +344,58 @@
     GetImportRequestRequestTypeDef,
     ImportStatisticsTypeDef,
     GetInsightSelectorsRequestRequestTypeDef,
     InsightSelectorTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
     GetTrailRequestRequestTypeDef,
     GetTrailStatusRequestRequestTypeDef,
+    GetTrailStatusResponseTypeDef,
     ImportFailureListItemTypeDef,
     S3ImportSourceTypeDef,
     ImportsListItemTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListEventDataStoresRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
     ListImportFailuresRequestRequestTypeDef,
+    ListImportsRequestListImportsPaginateTypeDef,
     ListImportsRequestRequestTypeDef,
+    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     PublicKeyTypeDef,
     ListQueriesRequestRequestTypeDef,
     QueryTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
+    ListTrailsRequestListTrailsPaginateTypeDef,
     ListTrailsRequestRequestTypeDef,
     TrailInfoTypeDef,
     LookupAttributeTypeDef,
+    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    PutResourcePolicyResponseTypeDef,
     RegisterOrganizationDelegatedAdminRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RestoreEventDataStoreRequestRequestTypeDef,
+    StartEventDataStoreIngestionRequestRequestTypeDef,
     StartLoggingRequestRequestTypeDef,
     StartQueryRequestRequestTypeDef,
+    StartQueryResponseTypeDef,
+    StopEventDataStoreIngestionRequestRequestTypeDef,
     StopImportRequestRequestTypeDef,
     StopLoggingRequestRequestTypeDef,
     UpdateTrailRequestRequestTypeDef,
+    UpdateTrailResponseTypeDef,
     AddTagsRequestRequestTypeDef,
     CreateTrailRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
     ResourceTagTypeDef,
     AdvancedEventSelectorTypeDef,
-    CancelQueryResponseTypeDef,
-    CreateTrailResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetTrailStatusResponseTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    StartQueryResponseTypeDef,
-    UpdateTrailResponseTypeDef,
     ListChannelsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     CreateChannelResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
     EventSelectorTypeDef,
     DescribeQueryResponseTypeDef,
@@ -398,19 +405,14 @@
     GetInsightSelectorsResponseTypeDef,
     PutInsightSelectorsRequestRequestTypeDef,
     PutInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     ListImportFailuresResponseTypeDef,
     ImportSourceTypeDef,
     ListImportsResponseTypeDef,
-    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
-    ListImportsRequestListImportsPaginateTypeDef,
-    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
-    ListTrailsRequestListTrailsPaginateTypeDef,
     ListPublicKeysResponseTypeDef,
     ListQueriesResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupEventsRequestLookupEventsPaginateTypeDef,
     LookupEventsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     CreateEventDataStoreRequestRequestTypeDef,
@@ -441,42 +443,42 @@
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

### Comparing `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/__init__.py` & `mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/__init__.pyi` & `mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/__main__.py` & `mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudTrail 1.26.72\nVersion:         1.26.72\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.CloudTrail 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.72")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/client.py` & `mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,16 +206,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#can_paginate)
         """
 
     def cancel_query(
         self, *, QueryId: str, EventDataStore: str = ...
     ) -> CancelQueryResponseTypeDef:
         """
-        Cancels a query if the query is not in a terminated state, such as `CANCELLED` ,
-        `FAILED` , `TIMED_OUT` , or `FINISHED`.
+        Cancels a query if the query is not in a terminated state, such as `CANCELLED`,
+        `FAILED`, `TIMED_OUT`, or `FINISHED`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.cancel_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#cancel_query)
         """
 
     def close(self) -> None:
         """
@@ -247,15 +247,16 @@
         Name: str,
         AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         TagsList: Sequence[TagTypeDef] = ...,
-        KmsKeyId: str = ...
+        KmsKeyId: str = ...,
+        StartIngestion: bool = ...
     ) -> CreateEventDataStoreResponseTypeDef:
         """
         Creates a new event data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#create_event_data_store)
         """
@@ -290,15 +291,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#delete_channel)
         """
 
     def delete_event_data_store(self, *, EventDataStore: str) -> Dict[str, Any]:
         """
-        Disables the event data store specified by `EventDataStore` , which accepts an
+        Disables the event data store specified by `EventDataStore`, which accepts an
         event data store ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#delete_event_data_store)
         """
 
     def delete_resource_policy(self, *, ResourceArn: str) -> Dict[str, Any]:
@@ -325,29 +326,29 @@
         an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.deregister_organization_delegated_admin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#deregister_organization_delegated_admin)
         """
 
     def describe_query(
-        self, *, QueryId: str, EventDataStore: str = ...
+        self, *, EventDataStore: str = ..., QueryId: str = ..., QueryAlias: str = ...
     ) -> DescribeQueryResponseTypeDef:
         """
         Returns metadata about a query, including query run time in milliseconds, number
         of events scanned and matched, and query status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.describe_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#describe_query)
         """
 
     def describe_trails(
         self, *, trailNameList: Sequence[str] = ..., includeShadowTrails: bool = ...
     ) -> DescribeTrailsResponseTypeDef:
         """
-        Retrieves settings for one or more trails associated with the current region for
+        Retrieves settings for one or more trails associated with the current Region for
         your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.describe_trails)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#describe_trails)
         """
 
     def generate_presigned_url(
@@ -458,15 +459,15 @@
         """
 
     def list_event_data_stores(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListEventDataStoresResponseTypeDef:
         """
         Returns information about all event data stores in the account, in the current
-        region.
+        Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_event_data_stores)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_event_data_stores)
         """
 
     def list_import_failures(
         self, *, ImportId: str, MaxResults: int = ..., NextToken: str = ...
@@ -484,15 +485,15 @@
         MaxResults: int = ...,
         Destination: str = ...,
         ImportStatus: ImportStatusType = ...,
         NextToken: str = ...
     ) -> ListImportsResponseTypeDef:
         """
         Returns information on all imports, or a select set of imports by `ImportStatus`
-        or `Destination` .
+        or `Destination`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_imports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_imports)
         """
 
     def list_public_keys(
         self,
@@ -526,16 +527,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_queries)
         """
 
     def list_tags(
         self, *, ResourceIdList: Sequence[str], NextToken: str = ...
     ) -> ListTagsResponseTypeDef:
         """
-        Lists the tags for the trail, event data store, or channel in the current
-        region.
+        Lists the tags for the specified trails, event data stores, or channels in the
+        current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_tags)
         """
 
     def list_trails(self, *, NextToken: str = ...) -> ListTrailsResponseTypeDef:
         """
@@ -619,21 +620,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#remove_tags)
         """
 
     def restore_event_data_store(
         self, *, EventDataStore: str
     ) -> RestoreEventDataStoreResponseTypeDef:
         """
-        Restores a deleted event data store specified by `EventDataStore` , which
-        accepts an event data store ARN.
+        Restores a deleted event data store specified by `EventDataStore`, which accepts
+        an event data store ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.restore_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#restore_event_data_store)
         """
 
+    def start_event_data_store_ingestion(self, *, EventDataStore: str) -> Dict[str, Any]:
+        """
+        Starts the ingestion of live events on an event data store specified as either
+        an ARN or the ID portion of the ARN.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_event_data_store_ingestion)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#start_event_data_store_ingestion)
+        """
+
     def start_import(
         self,
         *,
         Destinations: Sequence[str] = ...,
         ImportSource: ImportSourceTypeDef = ...,
         StartEventTime: Union[datetime, str] = ...,
         EndEventTime: Union[datetime, str] = ...,
@@ -653,23 +663,37 @@
         a trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_logging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#start_logging)
         """
 
     def start_query(
-        self, *, QueryStatement: str, DeliveryS3Uri: str = ...
+        self,
+        *,
+        QueryStatement: str = ...,
+        DeliveryS3Uri: str = ...,
+        QueryAlias: str = ...,
+        QueryParameters: Sequence[str] = ...
     ) -> StartQueryResponseTypeDef:
         """
         Starts a CloudTrail Lake query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#start_query)
         """
 
+    def stop_event_data_store_ingestion(self, *, EventDataStore: str) -> Dict[str, Any]:
+        """
+        Stops the ingestion of live events on an event data store specified as either an
+        ARN or the ID portion of the ARN.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.stop_event_data_store_ingestion)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#stop_event_data_store_ingestion)
+        """
+
     def stop_import(self, *, ImportId: str) -> StopImportResponseTypeDef:
         """
         Stops a specified import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.stop_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#stop_import)
         """
```

### Comparing `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/client.pyi` & `mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -199,16 +199,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#can_paginate)
         """
     def cancel_query(
         self, *, QueryId: str, EventDataStore: str = ...
     ) -> CancelQueryResponseTypeDef:
         """
-        Cancels a query if the query is not in a terminated state, such as `CANCELLED` ,
-        `FAILED` , `TIMED_OUT` , or `FINISHED`.
+        Cancels a query if the query is not in a terminated state, such as `CANCELLED`,
+        `FAILED`, `TIMED_OUT`, or `FINISHED`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.cancel_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#cancel_query)
         """
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
@@ -237,15 +237,16 @@
         Name: str,
         AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         TagsList: Sequence[TagTypeDef] = ...,
-        KmsKeyId: str = ...
+        KmsKeyId: str = ...,
+        StartIngestion: bool = ...
     ) -> CreateEventDataStoreResponseTypeDef:
         """
         Creates a new event data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#create_event_data_store)
         """
@@ -277,15 +278,15 @@
         Deletes a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#delete_channel)
         """
     def delete_event_data_store(self, *, EventDataStore: str) -> Dict[str, Any]:
         """
-        Disables the event data store specified by `EventDataStore` , which accepts an
+        Disables the event data store specified by `EventDataStore`, which accepts an
         event data store ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#delete_event_data_store)
         """
     def delete_resource_policy(self, *, ResourceArn: str) -> Dict[str, Any]:
         """
@@ -308,28 +309,28 @@
         Removes CloudTrail delegated administrator permissions from a member account in
         an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.deregister_organization_delegated_admin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#deregister_organization_delegated_admin)
         """
     def describe_query(
-        self, *, QueryId: str, EventDataStore: str = ...
+        self, *, EventDataStore: str = ..., QueryId: str = ..., QueryAlias: str = ...
     ) -> DescribeQueryResponseTypeDef:
         """
         Returns metadata about a query, including query run time in milliseconds, number
         of events scanned and matched, and query status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.describe_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#describe_query)
         """
     def describe_trails(
         self, *, trailNameList: Sequence[str] = ..., includeShadowTrails: bool = ...
     ) -> DescribeTrailsResponseTypeDef:
         """
-        Retrieves settings for one or more trails associated with the current region for
+        Retrieves settings for one or more trails associated with the current Region for
         your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.describe_trails)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#describe_trails)
         """
     def generate_presigned_url(
         self,
@@ -428,15 +429,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_channels)
         """
     def list_event_data_stores(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListEventDataStoresResponseTypeDef:
         """
         Returns information about all event data stores in the account, in the current
-        region.
+        Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_event_data_stores)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_event_data_stores)
         """
     def list_import_failures(
         self, *, ImportId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListImportFailuresResponseTypeDef:
@@ -452,15 +453,15 @@
         MaxResults: int = ...,
         Destination: str = ...,
         ImportStatus: ImportStatusType = ...,
         NextToken: str = ...
     ) -> ListImportsResponseTypeDef:
         """
         Returns information on all imports, or a select set of imports by `ImportStatus`
-        or `Destination` .
+        or `Destination`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_imports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_imports)
         """
     def list_public_keys(
         self,
         *,
@@ -491,16 +492,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_queries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_queries)
         """
     def list_tags(
         self, *, ResourceIdList: Sequence[str], NextToken: str = ...
     ) -> ListTagsResponseTypeDef:
         """
-        Lists the tags for the trail, event data store, or channel in the current
-        region.
+        Lists the tags for the specified trails, event data stores, or channels in the
+        current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_tags)
         """
     def list_trails(self, *, NextToken: str = ...) -> ListTrailsResponseTypeDef:
         """
         Lists trails that are in the current account.
@@ -576,20 +577,28 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.remove_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#remove_tags)
         """
     def restore_event_data_store(
         self, *, EventDataStore: str
     ) -> RestoreEventDataStoreResponseTypeDef:
         """
-        Restores a deleted event data store specified by `EventDataStore` , which
-        accepts an event data store ARN.
+        Restores a deleted event data store specified by `EventDataStore`, which accepts
+        an event data store ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.restore_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#restore_event_data_store)
         """
+    def start_event_data_store_ingestion(self, *, EventDataStore: str) -> Dict[str, Any]:
+        """
+        Starts the ingestion of live events on an event data store specified as either
+        an ARN or the ID portion of the ARN.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_event_data_store_ingestion)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#start_event_data_store_ingestion)
+        """
     def start_import(
         self,
         *,
         Destinations: Sequence[str] = ...,
         ImportSource: ImportSourceTypeDef = ...,
         StartEventTime: Union[datetime, str] = ...,
         EndEventTime: Union[datetime, str] = ...,
@@ -607,22 +616,35 @@
         Starts the recording of Amazon Web Services API calls and log file delivery for
         a trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_logging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#start_logging)
         """
     def start_query(
-        self, *, QueryStatement: str, DeliveryS3Uri: str = ...
+        self,
+        *,
+        QueryStatement: str = ...,
+        DeliveryS3Uri: str = ...,
+        QueryAlias: str = ...,
+        QueryParameters: Sequence[str] = ...
     ) -> StartQueryResponseTypeDef:
         """
         Starts a CloudTrail Lake query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#start_query)
         """
+    def stop_event_data_store_ingestion(self, *, EventDataStore: str) -> Dict[str, Any]:
+        """
+        Stops the ingestion of live events on an event data store specified as either an
+        ARN or the ID portion of the ARN.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.stop_event_data_store_ingestion)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#stop_event_data_store_ingestion)
+        """
     def stop_import(self, *, ImportId: str) -> StopImportResponseTypeDef:
         """
         Stops a specified import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.stop_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#stop_import)
         """
```

### Comparing `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/literals.py` & `mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,22 @@
     "PENDING",
     "RESOURCE_NOT_FOUND",
     "SUCCESS",
     "UNKNOWN",
 ]
 DestinationTypeType = Literal["AWS_SERVICE", "EVENT_DATA_STORE"]
 EventCategoryType = Literal["insight"]
-EventDataStoreStatusType = Literal["CREATED", "ENABLED", "PENDING_DELETION"]
+EventDataStoreStatusType = Literal[
+    "CREATED",
+    "ENABLED",
+    "PENDING_DELETION",
+    "STARTING_INGESTION",
+    "STOPPED_INGESTION",
+    "STOPPING_INGESTION",
+]
 ImportFailureStatusType = Literal["FAILED", "RETRY", "SUCCEEDED"]
 ImportStatusType = Literal["COMPLETED", "FAILED", "INITIALIZING", "IN_PROGRESS", "STOPPED"]
 InsightTypeType = Literal["ApiCallRateInsight", "ApiErrorRateInsight"]
 ListImportFailuresPaginatorName = Literal["list_import_failures"]
 ListImportsPaginatorName = Literal["list_imports"]
 ListPublicKeysPaginatorName = Literal["list_public_keys"]
 ListTagsPaginatorName = Literal["list_tags"]
@@ -91,14 +98,15 @@
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
@@ -138,14 +146,15 @@
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
@@ -224,14 +233,15 @@
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
@@ -242,14 +252,15 @@
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
@@ -285,14 +296,15 @@
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
@@ -311,16 +323,19 @@
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
@@ -400,18 +415,21 @@
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

### Comparing `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/literals.pyi` & `mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,22 @@
     "PENDING",
     "RESOURCE_NOT_FOUND",
     "SUCCESS",
     "UNKNOWN",
 ]
 DestinationTypeType = Literal["AWS_SERVICE", "EVENT_DATA_STORE"]
 EventCategoryType = Literal["insight"]
-EventDataStoreStatusType = Literal["CREATED", "ENABLED", "PENDING_DELETION"]
+EventDataStoreStatusType = Literal[
+    "CREATED",
+    "ENABLED",
+    "PENDING_DELETION",
+    "STARTING_INGESTION",
+    "STOPPED_INGESTION",
+    "STOPPING_INGESTION",
+]
 ImportFailureStatusType = Literal["FAILED", "RETRY", "SUCCEEDED"]
 ImportStatusType = Literal["COMPLETED", "FAILED", "INITIALIZING", "IN_PROGRESS", "STOPPED"]
 InsightTypeType = Literal["ApiCallRateInsight", "ApiErrorRateInsight"]
 ListImportFailuresPaginatorName = Literal["list_import_failures"]
 ListImportsPaginatorName = Literal["list_imports"]
 ListPublicKeysPaginatorName = Literal["list_public_keys"]
 ListTagsPaginatorName = Literal["list_tags"]
@@ -89,14 +96,15 @@
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
@@ -136,14 +144,15 @@
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
@@ -222,14 +231,15 @@
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
@@ -240,14 +250,15 @@
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
@@ -283,14 +294,15 @@
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
@@ -309,16 +321,19 @@
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
@@ -398,18 +413,21 @@
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

### Comparing `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/paginator.py` & `mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 class ListImportFailuresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImportFailures)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listimportfailurespaginator)
     """
 
     def paginate(
-        self, *, ImportId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ImportId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListImportFailuresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImportFailures.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listimportfailurespaginator)
         """
 
 
@@ -95,15 +95,15 @@
     """
 
     def paginate(
         self,
         *,
         Destination: str = ...,
         ImportStatus: ImportStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listimportspaginator)
         """
 
 
@@ -114,45 +114,45 @@
     """
 
     def paginate(
         self,
         *,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPublicKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listpublickeyspaginator)
         """
 
 
 class ListTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtagspaginator)
     """
 
     def paginate(
-        self, *, ResourceIdList: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceIdList: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtagspaginator)
         """
 
 
 class ListTrailsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTrails)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtrailspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTrailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTrails.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtrailspaginator)
         """
 
 
@@ -165,13 +165,13 @@
     def paginate(
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         EventCategory: Literal["insight"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[LookupEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.LookupEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#lookupeventspaginator)
         """
```

### Comparing `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/paginator.pyi` & `mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 class ListImportFailuresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImportFailures)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listimportfailurespaginator)
     """
 
     def paginate(
-        self, *, ImportId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ImportId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListImportFailuresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImportFailures.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listimportfailurespaginator)
         """
 
 class ListImportsPaginator(Paginator):
@@ -90,15 +90,15 @@
     """
 
     def paginate(
         self,
         *,
         Destination: str = ...,
         ImportStatus: ImportStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListImportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListImports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listimportspaginator)
         """
 
 class ListPublicKeysPaginator(Paginator):
@@ -108,43 +108,43 @@
     """
 
     def paginate(
         self,
         *,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPublicKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listpublickeyspaginator)
         """
 
 class ListTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtagspaginator)
     """
 
     def paginate(
-        self, *, ResourceIdList: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceIdList: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtagspaginator)
         """
 
 class ListTrailsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTrails)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtrailspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTrailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListTrails.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listtrailspaginator)
         """
 
 class LookupEventsPaginator(Paginator):
@@ -156,13 +156,13 @@
     def paginate(
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         EventCategory: Literal["insight"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[LookupEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.LookupEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#lookupeventspaginator)
         """
```

### Comparing `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/type_defs.py` & `mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,18 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
     "AdvancedFieldSelectorTypeDef",
     "CancelQueryRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelQueryResponseTypeDef",
     "ChannelTypeDef",
     "DestinationTypeDef",
+    "CreateTrailResponseTypeDef",
     "DataResourceTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteEventDataStoreRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteTrailRequestRequestTypeDef",
     "DeregisterOrganizationDelegatedAdminRequestRequestTypeDef",
     "DescribeQueryRequestRequestTypeDef",
@@ -62,52 +63,58 @@
     "GetImportRequestRequestTypeDef",
     "ImportStatisticsTypeDef",
     "GetInsightSelectorsRequestRequestTypeDef",
     "InsightSelectorTypeDef",
     "GetQueryResultsRequestRequestTypeDef",
     "QueryStatisticsTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
+    "GetResourcePolicyResponseTypeDef",
     "GetTrailRequestRequestTypeDef",
     "GetTrailStatusRequestRequestTypeDef",
+    "GetTrailStatusResponseTypeDef",
     "ImportFailureListItemTypeDef",
     "S3ImportSourceTypeDef",
     "ImportsListItemTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListEventDataStoresRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
     "ListImportFailuresRequestRequestTypeDef",
+    "ListImportsRequestListImportsPaginateTypeDef",
     "ListImportsRequestRequestTypeDef",
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
     "ListPublicKeysRequestRequestTypeDef",
     "PublicKeyTypeDef",
     "ListQueriesRequestRequestTypeDef",
     "QueryTypeDef",
+    "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "ListTrailsRequestListTrailsPaginateTypeDef",
     "ListTrailsRequestRequestTypeDef",
     "TrailInfoTypeDef",
     "LookupAttributeTypeDef",
+    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "PutResourcePolicyResponseTypeDef",
     "RegisterOrganizationDelegatedAdminRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreEventDataStoreRequestRequestTypeDef",
+    "StartEventDataStoreIngestionRequestRequestTypeDef",
     "StartLoggingRequestRequestTypeDef",
     "StartQueryRequestRequestTypeDef",
+    "StartQueryResponseTypeDef",
+    "StopEventDataStoreIngestionRequestRequestTypeDef",
     "StopImportRequestRequestTypeDef",
     "StopLoggingRequestRequestTypeDef",
     "UpdateTrailRequestRequestTypeDef",
+    "UpdateTrailResponseTypeDef",
     "AddTagsRequestRequestTypeDef",
     "CreateTrailRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
     "ResourceTagTypeDef",
     "AdvancedEventSelectorTypeDef",
-    "CancelQueryResponseTypeDef",
-    "CreateTrailResponseTypeDef",
-    "GetResourcePolicyResponseTypeDef",
-    "GetTrailStatusResponseTypeDef",
-    "PutResourcePolicyResponseTypeDef",
-    "StartQueryResponseTypeDef",
-    "UpdateTrailResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdateChannelResponseTypeDef",
     "EventSelectorTypeDef",
     "DescribeQueryResponseTypeDef",
@@ -117,19 +124,14 @@
     "GetInsightSelectorsResponseTypeDef",
     "PutInsightSelectorsRequestRequestTypeDef",
     "PutInsightSelectorsResponseTypeDef",
     "GetQueryResultsResponseTypeDef",
     "ListImportFailuresResponseTypeDef",
     "ImportSourceTypeDef",
     "ListImportsResponseTypeDef",
-    "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
-    "ListImportsRequestListImportsPaginateTypeDef",
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
-    "ListTagsRequestListTagsPaginateTypeDef",
-    "ListTrailsRequestListTrailsPaginateTypeDef",
     "ListPublicKeysResponseTypeDef",
     "ListQueriesResponseTypeDef",
     "ListTrailsResponseTypeDef",
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     "LookupEventsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "CreateEventDataStoreRequestRequestTypeDef",
@@ -214,22 +216,20 @@
 
 class CancelQueryRequestRequestTypeDef(
     _RequiredCancelQueryRequestRequestTypeDef, _OptionalCancelQueryRequestRequestTypeDef
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelQueryResponseTypeDef = TypedDict(
+    "CancelQueryResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "QueryId": str,
+        "QueryStatus": QueryStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "ChannelArn": str,
@@ -242,14 +242,34 @@
     "DestinationTypeDef",
     {
         "Type": DestinationTypeType,
         "Location": str,
     },
 )
 
+CreateTrailResponseTypeDef = TypedDict(
+    "CreateTrailResponseTypeDef",
+    {
+        "Name": str,
+        "S3BucketName": str,
+        "S3KeyPrefix": str,
+        "SnsTopicName": str,
+        "SnsTopicARN": str,
+        "IncludeGlobalServiceEvents": bool,
+        "IsMultiRegionTrail": bool,
+        "TrailARN": str,
+        "LogFileValidationEnabled": bool,
+        "CloudWatchLogsLogGroupArn": str,
+        "CloudWatchLogsRoleArn": str,
+        "KmsKeyId": str,
+        "IsOrganizationTrail": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataResourceTypeDef = TypedDict(
     "DataResourceTypeDef",
     {
         "Type": str,
         "Values": List[str],
     },
     total=False,
@@ -286,35 +306,24 @@
 DeregisterOrganizationDelegatedAdminRequestRequestTypeDef = TypedDict(
     "DeregisterOrganizationDelegatedAdminRequestRequestTypeDef",
     {
         "DelegatedAdminAccountId": str,
     },
 )
 
-_RequiredDescribeQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeQueryRequestRequestTypeDef",
-    {
-        "QueryId": str,
-    },
-)
-_OptionalDescribeQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeQueryRequestRequestTypeDef",
+DescribeQueryRequestRequestTypeDef = TypedDict(
+    "DescribeQueryRequestRequestTypeDef",
     {
         "EventDataStore": str,
+        "QueryId": str,
+        "QueryAlias": str,
     },
     total=False,
 )
 
-
-class DescribeQueryRequestRequestTypeDef(
-    _RequiredDescribeQueryRequestRequestTypeDef, _OptionalDescribeQueryRequestRequestTypeDef
-):
-    pass
-
-
 QueryStatisticsForDescribeQueryTypeDef = TypedDict(
     "QueryStatisticsForDescribeQueryTypeDef",
     {
         "EventsMatched": int,
         "EventsScanned": int,
         "BytesScanned": int,
         "ExecutionTimeInMillis": int,
@@ -467,28 +476,61 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourcePolicy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTrailRequestRequestTypeDef = TypedDict(
     "GetTrailRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 GetTrailStatusRequestRequestTypeDef = TypedDict(
     "GetTrailStatusRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+GetTrailStatusResponseTypeDef = TypedDict(
+    "GetTrailStatusResponseTypeDef",
+    {
+        "IsLogging": bool,
+        "LatestDeliveryError": str,
+        "LatestNotificationError": str,
+        "LatestDeliveryTime": datetime,
+        "LatestNotificationTime": datetime,
+        "StartLoggingTime": datetime,
+        "StopLoggingTime": datetime,
+        "LatestCloudWatchLogsDeliveryError": str,
+        "LatestCloudWatchLogsDeliveryTime": datetime,
+        "LatestDigestDeliveryTime": datetime,
+        "LatestDigestDeliveryError": str,
+        "LatestDeliveryAttemptTime": str,
+        "LatestNotificationAttemptTime": str,
+        "LatestNotificationAttemptSucceeded": str,
+        "LatestDeliveryAttemptSucceeded": str,
+        "TimeLoggingStarted": str,
+        "TimeLoggingStopped": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ImportFailureListItemTypeDef = TypedDict(
     "ImportFailureListItemTypeDef",
     {
         "Location": str,
         "Status": ImportFailureStatusType,
         "ErrorType": str,
         "ErrorMessage": str,
@@ -532,24 +574,36 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
+    "_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ImportId": str,
+    },
+)
+_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
+    "_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListImportFailuresRequestListImportFailuresPaginateTypeDef(
+    _RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    _OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListImportFailuresRequestRequestTypeDef = TypedDict(
     "_RequiredListImportFailuresRequestRequestTypeDef",
     {
         "ImportId": str,
     },
 )
 _OptionalListImportFailuresRequestRequestTypeDef = TypedDict(
@@ -565,25 +619,45 @@
 class ListImportFailuresRequestRequestTypeDef(
     _RequiredListImportFailuresRequestRequestTypeDef,
     _OptionalListImportFailuresRequestRequestTypeDef,
 ):
     pass
 
 
+ListImportsRequestListImportsPaginateTypeDef = TypedDict(
+    "ListImportsRequestListImportsPaginateTypeDef",
+    {
+        "Destination": str,
+        "ImportStatus": ImportStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListImportsRequestRequestTypeDef = TypedDict(
     "ListImportsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "Destination": str,
         "ImportStatus": ImportStatusType,
         "NextToken": str,
     },
     total=False,
 )
 
+ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPublicKeysRequestRequestTypeDef = TypedDict(
     "ListPublicKeysRequestRequestTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "NextToken": str,
     },
@@ -632,14 +706,35 @@
         "QueryId": str,
         "QueryStatus": QueryStatusType,
         "CreationTime": datetime,
     },
     total=False,
 )
 
+_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_RequiredListTagsRequestListTagsPaginateTypeDef",
+    {
+        "ResourceIdList": Sequence[str],
+    },
+)
+_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_OptionalListTagsRequestListTagsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTagsRequestListTagsPaginateTypeDef(
+    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
+):
+    pass
+
+
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceIdList": Sequence[str],
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
@@ -653,14 +748,22 @@
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
 
+ListTrailsRequestListTrailsPaginateTypeDef = TypedDict(
+    "ListTrailsRequestListTrailsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTrailsRequestRequestTypeDef = TypedDict(
     "ListTrailsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -679,63 +782,105 @@
     "LookupAttributeTypeDef",
     {
         "AttributeKey": LookupAttributeKeyType,
         "AttributeValue": str,
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourcePolicy": str,
     },
 )
 
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourcePolicy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterOrganizationDelegatedAdminRequestRequestTypeDef = TypedDict(
     "RegisterOrganizationDelegatedAdminRequestRequestTypeDef",
     {
         "MemberAccountId": str,
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
 RestoreEventDataStoreRequestRequestTypeDef = TypedDict(
     "RestoreEventDataStoreRequestRequestTypeDef",
     {
         "EventDataStore": str,
     },
 )
 
+StartEventDataStoreIngestionRequestRequestTypeDef = TypedDict(
+    "StartEventDataStoreIngestionRequestRequestTypeDef",
+    {
+        "EventDataStore": str,
+    },
+)
+
 StartLoggingRequestRequestTypeDef = TypedDict(
     "StartLoggingRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-_RequiredStartQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredStartQueryRequestRequestTypeDef",
+StartQueryRequestRequestTypeDef = TypedDict(
+    "StartQueryRequestRequestTypeDef",
     {
         "QueryStatement": str,
-    },
-)
-_OptionalStartQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalStartQueryRequestRequestTypeDef",
-    {
         "DeliveryS3Uri": str,
+        "QueryAlias": str,
+        "QueryParameters": Sequence[str],
     },
     total=False,
 )
 
+StartQueryResponseTypeDef = TypedDict(
+    "StartQueryResponseTypeDef",
+    {
+        "QueryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
-class StartQueryRequestRequestTypeDef(
-    _RequiredStartQueryRequestRequestTypeDef, _OptionalStartQueryRequestRequestTypeDef
-):
-    pass
-
+StopEventDataStoreIngestionRequestRequestTypeDef = TypedDict(
+    "StopEventDataStoreIngestionRequestRequestTypeDef",
+    {
+        "EventDataStore": str,
+    },
+)
 
 StopImportRequestRequestTypeDef = TypedDict(
     "StopImportRequestRequestTypeDef",
     {
         "ImportId": str,
     },
 )
@@ -773,14 +918,34 @@
 
 class UpdateTrailRequestRequestTypeDef(
     _RequiredUpdateTrailRequestRequestTypeDef, _OptionalUpdateTrailRequestRequestTypeDef
 ):
     pass
 
 
+UpdateTrailResponseTypeDef = TypedDict(
+    "UpdateTrailResponseTypeDef",
+    {
+        "Name": str,
+        "S3BucketName": str,
+        "S3KeyPrefix": str,
+        "SnsTopicName": str,
+        "SnsTopicARN": str,
+        "IncludeGlobalServiceEvents": bool,
+        "IsMultiRegionTrail": bool,
+        "TrailARN": str,
+        "LogFileValidationEnabled": bool,
+        "CloudWatchLogsLogGroupArn": str,
+        "CloudWatchLogsRoleArn": str,
+        "KmsKeyId": str,
+        "IsOrganizationTrail": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AddTagsRequestRequestTypeDef = TypedDict(
     "AddTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagsList": Sequence[TagTypeDef],
     },
 )
@@ -850,119 +1015,20 @@
 
 class AdvancedEventSelectorTypeDef(
     _RequiredAdvancedEventSelectorTypeDef, _OptionalAdvancedEventSelectorTypeDef
 ):
     pass
 
 
-CancelQueryResponseTypeDef = TypedDict(
-    "CancelQueryResponseTypeDef",
-    {
-        "QueryId": str,
-        "QueryStatus": QueryStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTrailResponseTypeDef = TypedDict(
-    "CreateTrailResponseTypeDef",
-    {
-        "Name": str,
-        "S3BucketName": str,
-        "S3KeyPrefix": str,
-        "SnsTopicName": str,
-        "SnsTopicARN": str,
-        "IncludeGlobalServiceEvents": bool,
-        "IsMultiRegionTrail": bool,
-        "TrailARN": str,
-        "LogFileValidationEnabled": bool,
-        "CloudWatchLogsLogGroupArn": str,
-        "CloudWatchLogsRoleArn": str,
-        "KmsKeyId": str,
-        "IsOrganizationTrail": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourcePolicy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTrailStatusResponseTypeDef = TypedDict(
-    "GetTrailStatusResponseTypeDef",
-    {
-        "IsLogging": bool,
-        "LatestDeliveryError": str,
-        "LatestNotificationError": str,
-        "LatestDeliveryTime": datetime,
-        "LatestNotificationTime": datetime,
-        "StartLoggingTime": datetime,
-        "StopLoggingTime": datetime,
-        "LatestCloudWatchLogsDeliveryError": str,
-        "LatestCloudWatchLogsDeliveryTime": datetime,
-        "LatestDigestDeliveryTime": datetime,
-        "LatestDigestDeliveryError": str,
-        "LatestDeliveryAttemptTime": str,
-        "LatestNotificationAttemptTime": str,
-        "LatestNotificationAttemptSucceeded": str,
-        "LatestDeliveryAttemptSucceeded": str,
-        "TimeLoggingStarted": str,
-        "TimeLoggingStopped": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourcePolicy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartQueryResponseTypeDef = TypedDict(
-    "StartQueryResponseTypeDef",
-    {
-        "QueryId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTrailResponseTypeDef = TypedDict(
-    "UpdateTrailResponseTypeDef",
-    {
-        "Name": str,
-        "S3BucketName": str,
-        "S3KeyPrefix": str,
-        "SnsTopicName": str,
-        "SnsTopicARN": str,
-        "IncludeGlobalServiceEvents": bool,
-        "IsMultiRegionTrail": bool,
-        "TrailARN": str,
-        "LogFileValidationEnabled": bool,
-        "CloudWatchLogsLogGroupArn": str,
-        "CloudWatchLogsRoleArn": str,
-        "KmsKeyId": str,
-        "IsOrganizationTrail": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "Name": str,
@@ -989,15 +1055,15 @@
     "CreateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "Destinations": List[DestinationTypeDef],
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "Channel": str,
@@ -1022,15 +1088,15 @@
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "Destinations": List[DestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventSelectorTypeDef = TypedDict(
     "EventSelectorTypeDef",
     {
         "ReadWriteType": ReadWriteTypeType,
@@ -1047,31 +1113,31 @@
         "QueryId": str,
         "QueryString": str,
         "QueryStatus": QueryStatusType,
         "QueryStatistics": QueryStatisticsForDescribeQueryTypeDef,
         "ErrorMessage": str,
         "DeliveryS3Uri": str,
         "DeliveryStatus": DeliveryStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTrailsResponseTypeDef = TypedDict(
     "DescribeTrailsResponseTypeDef",
     {
         "trailList": List[TrailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTrailResponseTypeDef = TypedDict(
     "GetTrailResponseTypeDef",
     {
         "Trail": TrailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "EventId": str,
@@ -1088,15 +1154,15 @@
 )
 
 GetInsightSelectorsResponseTypeDef = TypedDict(
     "GetInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "InsightSelectors": List[InsightSelectorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutInsightSelectorsRequestRequestTypeDef = TypedDict(
     "PutInsightSelectorsRequestRequestTypeDef",
     {
         "TrailName": str,
@@ -1105,36 +1171,36 @@
 )
 
 PutInsightSelectorsResponseTypeDef = TypedDict(
     "PutInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "InsightSelectors": List[InsightSelectorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueryResultsResponseTypeDef = TypedDict(
     "GetQueryResultsResponseTypeDef",
     {
         "QueryStatus": QueryStatusType,
         "QueryStatistics": QueryStatisticsTypeDef,
         "QueryResultRows": List[List[Dict[str, str]]],
         "NextToken": str,
         "ErrorMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListImportFailuresResponseTypeDef = TypedDict(
     "ListImportFailuresResponseTypeDef",
     {
         "Failures": List[ImportFailureListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportSourceTypeDef = TypedDict(
     "ImportSourceTypeDef",
     {
         "S3": S3ImportSourceTypeDef,
@@ -1142,124 +1208,53 @@
 )
 
 ListImportsResponseTypeDef = TypedDict(
     "ListImportsResponseTypeDef",
     {
         "Imports": List[ImportsListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
-    "_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef",
-    {
-        "ImportId": str,
-    },
-)
-_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
-    "_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListImportFailuresRequestListImportFailuresPaginateTypeDef(
-    _RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef,
-    _OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef,
-):
-    pass
-
-
-ListImportsRequestListImportsPaginateTypeDef = TypedDict(
-    "ListImportsRequestListImportsPaginateTypeDef",
-    {
-        "Destination": str,
-        "ImportStatus": ImportStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_RequiredListTagsRequestListTagsPaginateTypeDef",
-    {
-        "ResourceIdList": Sequence[str],
-    },
-)
-_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_OptionalListTagsRequestListTagsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTagsRequestListTagsPaginateTypeDef(
-    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
-):
-    pass
-
-
-ListTrailsRequestListTrailsPaginateTypeDef = TypedDict(
-    "ListTrailsRequestListTrailsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListPublicKeysResponseTypeDef = TypedDict(
     "ListPublicKeysResponseTypeDef",
     {
         "PublicKeyList": List[PublicKeyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListQueriesResponseTypeDef = TypedDict(
     "ListQueriesResponseTypeDef",
     {
         "Queries": List[QueryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrailsResponseTypeDef = TypedDict(
     "ListTrailsResponseTypeDef",
     {
         "Trails": List[TrailInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LookupEventsRequestLookupEventsPaginateTypeDef = TypedDict(
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     {
         "LookupAttributes": Sequence[LookupAttributeTypeDef],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "EventCategory": Literal["insight"],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 LookupEventsRequestRequestTypeDef = TypedDict(
     "LookupEventsRequestRequestTypeDef",
     {
@@ -1274,15 +1269,15 @@
 )
 
 ListTagsResponseTypeDef = TypedDict(
     "ListTagsResponseTypeDef",
     {
         "ResourceTagList": List[ResourceTagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventDataStoreRequestRequestTypeDef",
     {
         "Name": str,
@@ -1294,14 +1289,15 @@
         "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "TagsList": Sequence[TagTypeDef],
         "KmsKeyId": str,
+        "StartIngestion": bool,
     },
     total=False,
 )
 
 
 class CreateEventDataStoreRequestRequestTypeDef(
     _RequiredCreateEventDataStoreRequestRequestTypeDef,
@@ -1321,15 +1317,15 @@
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "TagsList": List[TagTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventDataStoreTypeDef = TypedDict(
     "EventDataStoreTypeDef",
     {
         "EventDataStoreArn": str,
@@ -1356,15 +1352,15 @@
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreEventDataStoreResponseTypeDef = TypedDict(
     "RestoreEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
@@ -1374,15 +1370,15 @@
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceConfigTypeDef = TypedDict(
     "SourceConfigTypeDef",
     {
         "ApplyToAllRegions": bool,
@@ -1429,25 +1425,25 @@
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEventSelectorsResponseTypeDef = TypedDict(
     "GetEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "EventSelectors": List[EventSelectorTypeDef],
         "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
     "_RequiredPutEventSelectorsRequestRequestTypeDef",
     {
         "TrailName": str,
@@ -1471,24 +1467,24 @@
 
 PutEventSelectorsResponseTypeDef = TypedDict(
     "PutEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "EventSelectors": List[EventSelectorTypeDef],
         "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LookupEventsResponseTypeDef = TypedDict(
     "LookupEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetImportResponseTypeDef = TypedDict(
     "GetImportResponseTypeDef",
     {
         "ImportId": str,
@@ -1496,15 +1492,15 @@
         "ImportSource": ImportSourceTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartImportRequestRequestTypeDef = TypedDict(
     "StartImportRequestRequestTypeDef",
     {
         "Destinations": Sequence[str],
@@ -1523,15 +1519,15 @@
         "Destinations": List[str],
         "ImportSource": ImportSourceTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopImportResponseTypeDef = TypedDict(
     "StopImportResponseTypeDef",
     {
         "ImportId": str,
@@ -1539,32 +1535,32 @@
         "Destinations": List[str],
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventDataStoresResponseTypeDef = TypedDict(
     "ListEventDataStoresResponseTypeDef",
     {
         "EventDataStores": List[EventDataStoreTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "SourceConfig": SourceConfigTypeDef,
         "Destinations": List[DestinationTypeDef],
         "IngestionStatus": IngestionStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/type_defs.pyi` & `mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,18 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
     "AdvancedFieldSelectorTypeDef",
     "CancelQueryRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelQueryResponseTypeDef",
     "ChannelTypeDef",
     "DestinationTypeDef",
+    "CreateTrailResponseTypeDef",
     "DataResourceTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteEventDataStoreRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteTrailRequestRequestTypeDef",
     "DeregisterOrganizationDelegatedAdminRequestRequestTypeDef",
     "DescribeQueryRequestRequestTypeDef",
@@ -61,52 +62,58 @@
     "GetImportRequestRequestTypeDef",
     "ImportStatisticsTypeDef",
     "GetInsightSelectorsRequestRequestTypeDef",
     "InsightSelectorTypeDef",
     "GetQueryResultsRequestRequestTypeDef",
     "QueryStatisticsTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
+    "GetResourcePolicyResponseTypeDef",
     "GetTrailRequestRequestTypeDef",
     "GetTrailStatusRequestRequestTypeDef",
+    "GetTrailStatusResponseTypeDef",
     "ImportFailureListItemTypeDef",
     "S3ImportSourceTypeDef",
     "ImportsListItemTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListEventDataStoresRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
     "ListImportFailuresRequestRequestTypeDef",
+    "ListImportsRequestListImportsPaginateTypeDef",
     "ListImportsRequestRequestTypeDef",
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
     "ListPublicKeysRequestRequestTypeDef",
     "PublicKeyTypeDef",
     "ListQueriesRequestRequestTypeDef",
     "QueryTypeDef",
+    "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "ListTrailsRequestListTrailsPaginateTypeDef",
     "ListTrailsRequestRequestTypeDef",
     "TrailInfoTypeDef",
     "LookupAttributeTypeDef",
+    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "PutResourcePolicyResponseTypeDef",
     "RegisterOrganizationDelegatedAdminRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RestoreEventDataStoreRequestRequestTypeDef",
+    "StartEventDataStoreIngestionRequestRequestTypeDef",
     "StartLoggingRequestRequestTypeDef",
     "StartQueryRequestRequestTypeDef",
+    "StartQueryResponseTypeDef",
+    "StopEventDataStoreIngestionRequestRequestTypeDef",
     "StopImportRequestRequestTypeDef",
     "StopLoggingRequestRequestTypeDef",
     "UpdateTrailRequestRequestTypeDef",
+    "UpdateTrailResponseTypeDef",
     "AddTagsRequestRequestTypeDef",
     "CreateTrailRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
     "ResourceTagTypeDef",
     "AdvancedEventSelectorTypeDef",
-    "CancelQueryResponseTypeDef",
-    "CreateTrailResponseTypeDef",
-    "GetResourcePolicyResponseTypeDef",
-    "GetTrailStatusResponseTypeDef",
-    "PutResourcePolicyResponseTypeDef",
-    "StartQueryResponseTypeDef",
-    "UpdateTrailResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdateChannelResponseTypeDef",
     "EventSelectorTypeDef",
     "DescribeQueryResponseTypeDef",
@@ -116,19 +123,14 @@
     "GetInsightSelectorsResponseTypeDef",
     "PutInsightSelectorsRequestRequestTypeDef",
     "PutInsightSelectorsResponseTypeDef",
     "GetQueryResultsResponseTypeDef",
     "ListImportFailuresResponseTypeDef",
     "ImportSourceTypeDef",
     "ListImportsResponseTypeDef",
-    "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
-    "ListImportsRequestListImportsPaginateTypeDef",
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
-    "ListTagsRequestListTagsPaginateTypeDef",
-    "ListTrailsRequestListTrailsPaginateTypeDef",
     "ListPublicKeysResponseTypeDef",
     "ListQueriesResponseTypeDef",
     "ListTrailsResponseTypeDef",
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     "LookupEventsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "CreateEventDataStoreRequestRequestTypeDef",
@@ -207,22 +209,20 @@
 )
 
 class CancelQueryRequestRequestTypeDef(
     _RequiredCancelQueryRequestRequestTypeDef, _OptionalCancelQueryRequestRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelQueryResponseTypeDef = TypedDict(
+    "CancelQueryResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "QueryId": str,
+        "QueryStatus": QueryStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "ChannelArn": str,
@@ -235,14 +235,34 @@
     "DestinationTypeDef",
     {
         "Type": DestinationTypeType,
         "Location": str,
     },
 )
 
+CreateTrailResponseTypeDef = TypedDict(
+    "CreateTrailResponseTypeDef",
+    {
+        "Name": str,
+        "S3BucketName": str,
+        "S3KeyPrefix": str,
+        "SnsTopicName": str,
+        "SnsTopicARN": str,
+        "IncludeGlobalServiceEvents": bool,
+        "IsMultiRegionTrail": bool,
+        "TrailARN": str,
+        "LogFileValidationEnabled": bool,
+        "CloudWatchLogsLogGroupArn": str,
+        "CloudWatchLogsRoleArn": str,
+        "KmsKeyId": str,
+        "IsOrganizationTrail": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DataResourceTypeDef = TypedDict(
     "DataResourceTypeDef",
     {
         "Type": str,
         "Values": List[str],
     },
     total=False,
@@ -279,33 +299,24 @@
 DeregisterOrganizationDelegatedAdminRequestRequestTypeDef = TypedDict(
     "DeregisterOrganizationDelegatedAdminRequestRequestTypeDef",
     {
         "DelegatedAdminAccountId": str,
     },
 )
 
-_RequiredDescribeQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeQueryRequestRequestTypeDef",
-    {
-        "QueryId": str,
-    },
-)
-_OptionalDescribeQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeQueryRequestRequestTypeDef",
+DescribeQueryRequestRequestTypeDef = TypedDict(
+    "DescribeQueryRequestRequestTypeDef",
     {
         "EventDataStore": str,
+        "QueryId": str,
+        "QueryAlias": str,
     },
     total=False,
 )
 
-class DescribeQueryRequestRequestTypeDef(
-    _RequiredDescribeQueryRequestRequestTypeDef, _OptionalDescribeQueryRequestRequestTypeDef
-):
-    pass
-
 QueryStatisticsForDescribeQueryTypeDef = TypedDict(
     "QueryStatisticsForDescribeQueryTypeDef",
     {
         "EventsMatched": int,
         "EventsScanned": int,
         "BytesScanned": int,
         "ExecutionTimeInMillis": int,
@@ -456,28 +467,61 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourcePolicy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTrailRequestRequestTypeDef = TypedDict(
     "GetTrailRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 GetTrailStatusRequestRequestTypeDef = TypedDict(
     "GetTrailStatusRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+GetTrailStatusResponseTypeDef = TypedDict(
+    "GetTrailStatusResponseTypeDef",
+    {
+        "IsLogging": bool,
+        "LatestDeliveryError": str,
+        "LatestNotificationError": str,
+        "LatestDeliveryTime": datetime,
+        "LatestNotificationTime": datetime,
+        "StartLoggingTime": datetime,
+        "StopLoggingTime": datetime,
+        "LatestCloudWatchLogsDeliveryError": str,
+        "LatestCloudWatchLogsDeliveryTime": datetime,
+        "LatestDigestDeliveryTime": datetime,
+        "LatestDigestDeliveryError": str,
+        "LatestDeliveryAttemptTime": str,
+        "LatestNotificationAttemptTime": str,
+        "LatestNotificationAttemptSucceeded": str,
+        "LatestDeliveryAttemptSucceeded": str,
+        "TimeLoggingStarted": str,
+        "TimeLoggingStopped": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ImportFailureListItemTypeDef = TypedDict(
     "ImportFailureListItemTypeDef",
     {
         "Location": str,
         "Status": ImportFailureStatusType,
         "ErrorType": str,
         "ErrorMessage": str,
@@ -521,24 +565,34 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
+    "_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ImportId": str,
+    },
+)
+_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
+    "_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListImportFailuresRequestListImportFailuresPaginateTypeDef(
+    _RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef,
+    _OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef,
+):
+    pass
+
 _RequiredListImportFailuresRequestRequestTypeDef = TypedDict(
     "_RequiredListImportFailuresRequestRequestTypeDef",
     {
         "ImportId": str,
     },
 )
 _OptionalListImportFailuresRequestRequestTypeDef = TypedDict(
@@ -552,25 +606,45 @@
 
 class ListImportFailuresRequestRequestTypeDef(
     _RequiredListImportFailuresRequestRequestTypeDef,
     _OptionalListImportFailuresRequestRequestTypeDef,
 ):
     pass
 
+ListImportsRequestListImportsPaginateTypeDef = TypedDict(
+    "ListImportsRequestListImportsPaginateTypeDef",
+    {
+        "Destination": str,
+        "ImportStatus": ImportStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListImportsRequestRequestTypeDef = TypedDict(
     "ListImportsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "Destination": str,
         "ImportStatus": ImportStatusType,
         "NextToken": str,
     },
     total=False,
 )
 
+ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPublicKeysRequestRequestTypeDef = TypedDict(
     "ListPublicKeysRequestRequestTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "NextToken": str,
     },
@@ -617,14 +691,33 @@
         "QueryId": str,
         "QueryStatus": QueryStatusType,
         "CreationTime": datetime,
     },
     total=False,
 )
 
+_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_RequiredListTagsRequestListTagsPaginateTypeDef",
+    {
+        "ResourceIdList": Sequence[str],
+    },
+)
+_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_OptionalListTagsRequestListTagsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTagsRequestListTagsPaginateTypeDef(
+    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
+):
+    pass
+
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceIdList": Sequence[str],
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
@@ -636,14 +729,22 @@
 )
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
+ListTrailsRequestListTrailsPaginateTypeDef = TypedDict(
+    "ListTrailsRequestListTrailsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTrailsRequestRequestTypeDef = TypedDict(
     "ListTrailsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -662,61 +763,105 @@
     "LookupAttributeTypeDef",
     {
         "AttributeKey": LookupAttributeKeyType,
         "AttributeValue": str,
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourcePolicy": str,
     },
 )
 
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourcePolicy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegisterOrganizationDelegatedAdminRequestRequestTypeDef = TypedDict(
     "RegisterOrganizationDelegatedAdminRequestRequestTypeDef",
     {
         "MemberAccountId": str,
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
 RestoreEventDataStoreRequestRequestTypeDef = TypedDict(
     "RestoreEventDataStoreRequestRequestTypeDef",
     {
         "EventDataStore": str,
     },
 )
 
+StartEventDataStoreIngestionRequestRequestTypeDef = TypedDict(
+    "StartEventDataStoreIngestionRequestRequestTypeDef",
+    {
+        "EventDataStore": str,
+    },
+)
+
 StartLoggingRequestRequestTypeDef = TypedDict(
     "StartLoggingRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-_RequiredStartQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredStartQueryRequestRequestTypeDef",
+StartQueryRequestRequestTypeDef = TypedDict(
+    "StartQueryRequestRequestTypeDef",
     {
         "QueryStatement": str,
+        "DeliveryS3Uri": str,
+        "QueryAlias": str,
+        "QueryParameters": Sequence[str],
     },
+    total=False,
 )
-_OptionalStartQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalStartQueryRequestRequestTypeDef",
+
+StartQueryResponseTypeDef = TypedDict(
+    "StartQueryResponseTypeDef",
     {
-        "DeliveryS3Uri": str,
+        "QueryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class StartQueryRequestRequestTypeDef(
-    _RequiredStartQueryRequestRequestTypeDef, _OptionalStartQueryRequestRequestTypeDef
-):
-    pass
+StopEventDataStoreIngestionRequestRequestTypeDef = TypedDict(
+    "StopEventDataStoreIngestionRequestRequestTypeDef",
+    {
+        "EventDataStore": str,
+    },
+)
 
 StopImportRequestRequestTypeDef = TypedDict(
     "StopImportRequestRequestTypeDef",
     {
         "ImportId": str,
     },
 )
@@ -752,14 +897,34 @@
 )
 
 class UpdateTrailRequestRequestTypeDef(
     _RequiredUpdateTrailRequestRequestTypeDef, _OptionalUpdateTrailRequestRequestTypeDef
 ):
     pass
 
+UpdateTrailResponseTypeDef = TypedDict(
+    "UpdateTrailResponseTypeDef",
+    {
+        "Name": str,
+        "S3BucketName": str,
+        "S3KeyPrefix": str,
+        "SnsTopicName": str,
+        "SnsTopicARN": str,
+        "IncludeGlobalServiceEvents": bool,
+        "IsMultiRegionTrail": bool,
+        "TrailARN": str,
+        "LogFileValidationEnabled": bool,
+        "CloudWatchLogsLogGroupArn": str,
+        "CloudWatchLogsRoleArn": str,
+        "KmsKeyId": str,
+        "IsOrganizationTrail": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AddTagsRequestRequestTypeDef = TypedDict(
     "AddTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagsList": Sequence[TagTypeDef],
     },
 )
@@ -825,119 +990,20 @@
 )
 
 class AdvancedEventSelectorTypeDef(
     _RequiredAdvancedEventSelectorTypeDef, _OptionalAdvancedEventSelectorTypeDef
 ):
     pass
 
-CancelQueryResponseTypeDef = TypedDict(
-    "CancelQueryResponseTypeDef",
-    {
-        "QueryId": str,
-        "QueryStatus": QueryStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTrailResponseTypeDef = TypedDict(
-    "CreateTrailResponseTypeDef",
-    {
-        "Name": str,
-        "S3BucketName": str,
-        "S3KeyPrefix": str,
-        "SnsTopicName": str,
-        "SnsTopicARN": str,
-        "IncludeGlobalServiceEvents": bool,
-        "IsMultiRegionTrail": bool,
-        "TrailARN": str,
-        "LogFileValidationEnabled": bool,
-        "CloudWatchLogsLogGroupArn": str,
-        "CloudWatchLogsRoleArn": str,
-        "KmsKeyId": str,
-        "IsOrganizationTrail": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourcePolicy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTrailStatusResponseTypeDef = TypedDict(
-    "GetTrailStatusResponseTypeDef",
-    {
-        "IsLogging": bool,
-        "LatestDeliveryError": str,
-        "LatestNotificationError": str,
-        "LatestDeliveryTime": datetime,
-        "LatestNotificationTime": datetime,
-        "StartLoggingTime": datetime,
-        "StopLoggingTime": datetime,
-        "LatestCloudWatchLogsDeliveryError": str,
-        "LatestCloudWatchLogsDeliveryTime": datetime,
-        "LatestDigestDeliveryTime": datetime,
-        "LatestDigestDeliveryError": str,
-        "LatestDeliveryAttemptTime": str,
-        "LatestNotificationAttemptTime": str,
-        "LatestNotificationAttemptSucceeded": str,
-        "LatestDeliveryAttemptSucceeded": str,
-        "TimeLoggingStarted": str,
-        "TimeLoggingStopped": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourcePolicy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartQueryResponseTypeDef = TypedDict(
-    "StartQueryResponseTypeDef",
-    {
-        "QueryId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateTrailResponseTypeDef = TypedDict(
-    "UpdateTrailResponseTypeDef",
-    {
-        "Name": str,
-        "S3BucketName": str,
-        "S3KeyPrefix": str,
-        "SnsTopicName": str,
-        "SnsTopicARN": str,
-        "IncludeGlobalServiceEvents": bool,
-        "IsMultiRegionTrail": bool,
-        "TrailARN": str,
-        "LogFileValidationEnabled": bool,
-        "CloudWatchLogsLogGroupArn": str,
-        "CloudWatchLogsRoleArn": str,
-        "KmsKeyId": str,
-        "IsOrganizationTrail": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "Name": str,
@@ -962,15 +1028,15 @@
     "CreateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "Destinations": List[DestinationTypeDef],
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "Channel": str,
@@ -993,15 +1059,15 @@
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "Destinations": List[DestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventSelectorTypeDef = TypedDict(
     "EventSelectorTypeDef",
     {
         "ReadWriteType": ReadWriteTypeType,
@@ -1018,31 +1084,31 @@
         "QueryId": str,
         "QueryString": str,
         "QueryStatus": QueryStatusType,
         "QueryStatistics": QueryStatisticsForDescribeQueryTypeDef,
         "ErrorMessage": str,
         "DeliveryS3Uri": str,
         "DeliveryStatus": DeliveryStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTrailsResponseTypeDef = TypedDict(
     "DescribeTrailsResponseTypeDef",
     {
         "trailList": List[TrailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTrailResponseTypeDef = TypedDict(
     "GetTrailResponseTypeDef",
     {
         "Trail": TrailTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "EventId": str,
@@ -1059,15 +1125,15 @@
 )
 
 GetInsightSelectorsResponseTypeDef = TypedDict(
     "GetInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "InsightSelectors": List[InsightSelectorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutInsightSelectorsRequestRequestTypeDef = TypedDict(
     "PutInsightSelectorsRequestRequestTypeDef",
     {
         "TrailName": str,
@@ -1076,36 +1142,36 @@
 )
 
 PutInsightSelectorsResponseTypeDef = TypedDict(
     "PutInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "InsightSelectors": List[InsightSelectorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueryResultsResponseTypeDef = TypedDict(
     "GetQueryResultsResponseTypeDef",
     {
         "QueryStatus": QueryStatusType,
         "QueryStatistics": QueryStatisticsTypeDef,
         "QueryResultRows": List[List[Dict[str, str]]],
         "NextToken": str,
         "ErrorMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListImportFailuresResponseTypeDef = TypedDict(
     "ListImportFailuresResponseTypeDef",
     {
         "Failures": List[ImportFailureListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportSourceTypeDef = TypedDict(
     "ImportSourceTypeDef",
     {
         "S3": S3ImportSourceTypeDef,
@@ -1113,120 +1179,53 @@
 )
 
 ListImportsResponseTypeDef = TypedDict(
     "ListImportsResponseTypeDef",
     {
         "Imports": List[ImportsListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
-    "_RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef",
-    {
-        "ImportId": str,
-    },
-)
-_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef = TypedDict(
-    "_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-class ListImportFailuresRequestListImportFailuresPaginateTypeDef(
-    _RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef,
-    _OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef,
-):
-    pass
-
-ListImportsRequestListImportsPaginateTypeDef = TypedDict(
-    "ListImportsRequestListImportsPaginateTypeDef",
-    {
-        "Destination": str,
-        "ImportStatus": ImportStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_RequiredListTagsRequestListTagsPaginateTypeDef",
-    {
-        "ResourceIdList": Sequence[str],
-    },
-)
-_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_OptionalListTagsRequestListTagsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTagsRequestListTagsPaginateTypeDef(
-    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
-):
-    pass
-
-ListTrailsRequestListTrailsPaginateTypeDef = TypedDict(
-    "ListTrailsRequestListTrailsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
 ListPublicKeysResponseTypeDef = TypedDict(
     "ListPublicKeysResponseTypeDef",
     {
         "PublicKeyList": List[PublicKeyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListQueriesResponseTypeDef = TypedDict(
     "ListQueriesResponseTypeDef",
     {
         "Queries": List[QueryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTrailsResponseTypeDef = TypedDict(
     "ListTrailsResponseTypeDef",
     {
         "Trails": List[TrailInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LookupEventsRequestLookupEventsPaginateTypeDef = TypedDict(
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     {
         "LookupAttributes": Sequence[LookupAttributeTypeDef],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "EventCategory": Literal["insight"],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 LookupEventsRequestRequestTypeDef = TypedDict(
     "LookupEventsRequestRequestTypeDef",
     {
@@ -1241,15 +1240,15 @@
 )
 
 ListTagsResponseTypeDef = TypedDict(
     "ListTagsResponseTypeDef",
     {
         "ResourceTagList": List[ResourceTagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventDataStoreRequestRequestTypeDef",
     {
         "Name": str,
@@ -1261,14 +1260,15 @@
         "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "TagsList": Sequence[TagTypeDef],
         "KmsKeyId": str,
+        "StartIngestion": bool,
     },
     total=False,
 )
 
 class CreateEventDataStoreRequestRequestTypeDef(
     _RequiredCreateEventDataStoreRequestRequestTypeDef,
     _OptionalCreateEventDataStoreRequestRequestTypeDef,
@@ -1286,15 +1286,15 @@
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "TagsList": List[TagTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventDataStoreTypeDef = TypedDict(
     "EventDataStoreTypeDef",
     {
         "EventDataStoreArn": str,
@@ -1321,15 +1321,15 @@
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreEventDataStoreResponseTypeDef = TypedDict(
     "RestoreEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
@@ -1339,15 +1339,15 @@
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SourceConfigTypeDef = TypedDict(
     "SourceConfigTypeDef",
     {
         "ApplyToAllRegions": bool,
@@ -1392,25 +1392,25 @@
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEventSelectorsResponseTypeDef = TypedDict(
     "GetEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "EventSelectors": List[EventSelectorTypeDef],
         "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
     "_RequiredPutEventSelectorsRequestRequestTypeDef",
     {
         "TrailName": str,
@@ -1432,24 +1432,24 @@
 
 PutEventSelectorsResponseTypeDef = TypedDict(
     "PutEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "EventSelectors": List[EventSelectorTypeDef],
         "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LookupEventsResponseTypeDef = TypedDict(
     "LookupEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetImportResponseTypeDef = TypedDict(
     "GetImportResponseTypeDef",
     {
         "ImportId": str,
@@ -1457,15 +1457,15 @@
         "ImportSource": ImportSourceTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartImportRequestRequestTypeDef = TypedDict(
     "StartImportRequestRequestTypeDef",
     {
         "Destinations": Sequence[str],
@@ -1484,15 +1484,15 @@
         "Destinations": List[str],
         "ImportSource": ImportSourceTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopImportResponseTypeDef = TypedDict(
     "StopImportResponseTypeDef",
     {
         "ImportId": str,
@@ -1500,32 +1500,32 @@
         "Destinations": List[str],
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventDataStoresResponseTypeDef = TypedDict(
     "ListEventDataStoresResponseTypeDef",
     {
         "EventDataStores": List[EventDataStoreTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "SourceConfig": SourceConfigTypeDef,
         "Destinations": List[DestinationTypeDef],
         "IngestionStatus": IngestionStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/PKG-INFO` & `mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudtrail
-Version: 1.26.72
-Summary: Type annotations for boto3.CloudTrail 1.26.72 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudTrail 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-cloudtrail"></a>
 
 # mypy-boto3-cloudtrail
 
 [![PyPI - mypy-boto3-cloudtrail](https://img.shields.io/pypi/v/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudtrail?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [mypy-boto3-cloudtrail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,17 +350,18 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudtrail.type_defs import (
     TagTypeDef,
     AdvancedFieldSelectorTypeDef,
     CancelQueryRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelQueryResponseTypeDef,
     ChannelTypeDef,
     DestinationTypeDef,
+    CreateTrailResponseTypeDef,
     DataResourceTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteEventDataStoreRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteTrailRequestRequestTypeDef,
     DeregisterOrganizationDelegatedAdminRequestRequestTypeDef,
     DescribeQueryRequestRequestTypeDef,
@@ -375,52 +376,58 @@
     GetImportRequestRequestTypeDef,
     ImportStatisticsTypeDef,
     GetInsightSelectorsRequestRequestTypeDef,
     InsightSelectorTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
     GetTrailRequestRequestTypeDef,
     GetTrailStatusRequestRequestTypeDef,
+    GetTrailStatusResponseTypeDef,
     ImportFailureListItemTypeDef,
     S3ImportSourceTypeDef,
     ImportsListItemTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListEventDataStoresRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
     ListImportFailuresRequestRequestTypeDef,
+    ListImportsRequestListImportsPaginateTypeDef,
     ListImportsRequestRequestTypeDef,
+    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     PublicKeyTypeDef,
     ListQueriesRequestRequestTypeDef,
     QueryTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
+    ListTrailsRequestListTrailsPaginateTypeDef,
     ListTrailsRequestRequestTypeDef,
     TrailInfoTypeDef,
     LookupAttributeTypeDef,
+    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    PutResourcePolicyResponseTypeDef,
     RegisterOrganizationDelegatedAdminRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RestoreEventDataStoreRequestRequestTypeDef,
+    StartEventDataStoreIngestionRequestRequestTypeDef,
     StartLoggingRequestRequestTypeDef,
     StartQueryRequestRequestTypeDef,
+    StartQueryResponseTypeDef,
+    StopEventDataStoreIngestionRequestRequestTypeDef,
     StopImportRequestRequestTypeDef,
     StopLoggingRequestRequestTypeDef,
     UpdateTrailRequestRequestTypeDef,
+    UpdateTrailResponseTypeDef,
     AddTagsRequestRequestTypeDef,
     CreateTrailRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
     ResourceTagTypeDef,
     AdvancedEventSelectorTypeDef,
-    CancelQueryResponseTypeDef,
-    CreateTrailResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetTrailStatusResponseTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    StartQueryResponseTypeDef,
-    UpdateTrailResponseTypeDef,
     ListChannelsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     CreateChannelResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
     EventSelectorTypeDef,
     DescribeQueryResponseTypeDef,
@@ -430,19 +437,14 @@
     GetInsightSelectorsResponseTypeDef,
     PutInsightSelectorsRequestRequestTypeDef,
     PutInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     ListImportFailuresResponseTypeDef,
     ImportSourceTypeDef,
     ListImportsResponseTypeDef,
-    ListImportFailuresRequestListImportFailuresPaginateTypeDef,
-    ListImportsRequestListImportsPaginateTypeDef,
-    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
-    ListTrailsRequestListTrailsPaginateTypeDef,
     ListPublicKeysResponseTypeDef,
     ListQueriesResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupEventsRequestLookupEventsPaginateTypeDef,
     LookupEventsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     CreateEventDataStoreRequestRequestTypeDef,
@@ -473,42 +475,42 @@
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

### Comparing `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/SOURCES.txt` & `mypy-boto3-cloudtrail-1.27.0/mypy_boto3_cloudtrail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.26.72/setup.py` & `mypy-boto3-cloudtrail-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-cloudtrail.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudtrail",
-    version="1.26.72",
+    version="1.27.0",
     packages=["mypy_boto3_cloudtrail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudTrail 1.26.72 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.CloudTrail 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/",
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


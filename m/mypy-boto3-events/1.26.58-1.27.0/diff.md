# Comparing `tmp/mypy-boto3-events-1.26.58.tar.gz` & `tmp/mypy-boto3-events-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-events-1.26.58.tar", last modified: Thu Jan 26 20:25:02 2023, max compression
+gzip compressed data, was "mypy-boto3-events-1.27.0.tar", last modified: Mon Jul  3 19:50:45 2023, max compression
```

## Comparing `mypy-boto3-events-1.26.58.tar` & `mypy-boto3-events-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 20:25:02.559779 mypy-boto3-events-1.26.58/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-26 20:24:32.000000 mypy-boto3-events-1.26.58/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-01-26 20:25:02.559779 mypy-boto3-events-1.26.58/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18296 2023-01-26 20:24:32.000000 mypy-boto3-events-1.26.58/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 20:25:02.559779 mypy-boto3-events-1.26.58/mypy_boto3_events/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-01-26 20:24:32.000000 mypy-boto3-events-1.26.58/mypy_boto3_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-01-26 20:24:32.000000 mypy-boto3-events-1.26.58/mypy_boto3_events/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-01-26 20:24:32.000000 mypy-boto3-events-1.26.58/mypy_boto3_events/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37779 2023-01-26 20:24:33.000000 mypy-boto3-events-1.26.58/mypy_boto3_events/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37713 2023-01-26 20:24:32.000000 mypy-boto3-events-1.26.58/mypy_boto3_events/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-01-26 20:24:33.000000 mypy-boto3-events-1.26.58/mypy_boto3_events/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-01-26 20:24:33.000000 mypy-boto3-events-1.26.58/mypy_boto3_events/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-01-26 20:24:33.000000 mypy-boto3-events-1.26.58/mypy_boto3_events/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-01-26 20:24:33.000000 mypy-boto3-events-1.26.58/mypy_boto3_events/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-26 20:24:32.000000 mypy-boto3-events-1.26.58/mypy_boto3_events/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    58931 2023-01-26 20:24:35.000000 mypy-boto3-events-1.26.58/mypy_boto3_events/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58862 2023-01-26 20:24:34.000000 mypy-boto3-events-1.26.58/mypy_boto3_events/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-26 20:24:32.000000 mypy-boto3-events-1.26.58/mypy_boto3_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 20:25:02.559779 mypy-boto3-events-1.26.58/mypy_boto3_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-01-26 20:25:02.000000 mypy-boto3-events-1.26.58/mypy_boto3_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-26 20:25:02.000000 mypy-boto3-events-1.26.58/mypy_boto3_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 20:25:02.000000 mypy-boto3-events-1.26.58/mypy_boto3_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 20:25:02.000000 mypy-boto3-events-1.26.58/mypy_boto3_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-26 20:25:02.000000 mypy-boto3-events-1.26.58/mypy_boto3_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-26 20:25:02.000000 mypy-boto3-events-1.26.58/mypy_boto3_events.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-26 20:25:02.559779 mypy-boto3-events-1.26.58/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-01-26 20:24:32.000000 mypy-boto3-events-1.26.58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.811239 mypy-boto3-events-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:37.000000 mypy-boto3-events-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19759 2023-07-03 19:50:45.811239 mypy-boto3-events-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-07-03 19:37:37.000000 mypy-boto3-events-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.807239 mypy-boto3-events-1.27.0/mypy_boto3_events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-03 19:37:37.000000 mypy-boto3-events-1.27.0/mypy_boto3_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 19:37:37.000000 mypy-boto3-events-1.27.0/mypy_boto3_events/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-03 19:37:37.000000 mypy-boto3-events-1.27.0/mypy_boto3_events/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37779 2023-07-03 19:37:38.000000 mypy-boto3-events-1.27.0/mypy_boto3_events/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37713 2023-07-03 19:37:37.000000 mypy-boto3-events-1.27.0/mypy_boto3_events/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-07-03 19:37:38.000000 mypy-boto3-events-1.27.0/mypy_boto3_events/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-07-03 19:37:38.000000 mypy-boto3-events-1.27.0/mypy_boto3_events/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-03 19:37:38.000000 mypy-boto3-events-1.27.0/mypy_boto3_events/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-07-03 19:37:38.000000 mypy-boto3-events-1.27.0/mypy_boto3_events/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:37.000000 mypy-boto3-events-1.27.0/mypy_boto3_events/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59050 2023-07-03 19:37:39.000000 mypy-boto3-events-1.27.0/mypy_boto3_events/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58981 2023-07-03 19:37:38.000000 mypy-boto3-events-1.27.0/mypy_boto3_events/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:37.000000 mypy-boto3-events-1.27.0/mypy_boto3_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.811239 mypy-boto3-events-1.27.0/mypy_boto3_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19759 2023-07-03 19:50:45.000000 mypy-boto3-events-1.27.0/mypy_boto3_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 19:50:45.000000 mypy-boto3-events-1.27.0/mypy_boto3_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:45.000000 mypy-boto3-events-1.27.0/mypy_boto3_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:45.000000 mypy-boto3-events-1.27.0/mypy_boto3_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:45.000000 mypy-boto3-events-1.27.0/mypy_boto3_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 19:50:45.000000 mypy-boto3-events-1.27.0/mypy_boto3_events.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:45.811239 mypy-boto3-events-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-03 19:37:37.000000 mypy-boto3-events-1.27.0/setup.py
```

### Comparing `mypy-boto3-events-1.26.58/LICENSE` & `mypy-boto3-events-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-events-1.26.58/PKG-INFO` & `mypy-boto3-events-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-events
-Version: 1.26.58
-Summary: Type annotations for boto3.EventBridge 1.26.58 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.EventBridge 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-events"></a>
 
 # mypy-boto3-events
 
 [![PyPI - mypy-boto3-events](https://img.shields.io/pypi/v/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-events?color=blue)](https://pypistats.org/packages/mypy-boto3-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridge 1.26.58](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[boto3.EventBridge 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
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
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,56 +353,70 @@
     ActivateEventSourceRequestRequestTypeDef,
     ApiDestinationTypeDef,
     ArchiveTypeDef,
     AwsVpcConfigurationTypeDef,
     BatchArrayPropertiesTypeDef,
     BatchRetryStrategyTypeDef,
     CancelReplayRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelReplayResponseTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ConditionTypeDef,
     ConnectionApiKeyAuthResponseParametersTypeDef,
     ConnectionBasicAuthResponseParametersTypeDef,
     ConnectionBodyParameterTypeDef,
     ConnectionHeaderParameterTypeDef,
     ConnectionQueryStringParameterTypeDef,
     ConnectionOAuthClientResponseParametersTypeDef,
     ConnectionTypeDef,
     CreateApiDestinationRequestRequestTypeDef,
+    CreateApiDestinationResponseTypeDef,
     CreateArchiveRequestRequestTypeDef,
+    CreateArchiveResponseTypeDef,
     CreateConnectionApiKeyAuthRequestParametersTypeDef,
     CreateConnectionBasicAuthRequestParametersTypeDef,
     CreateConnectionOAuthClientRequestParametersTypeDef,
+    CreateConnectionResponseTypeDef,
     EndpointEventBusTypeDef,
     ReplicationConfigTypeDef,
     TagTypeDef,
+    CreateEventBusResponseTypeDef,
     CreatePartnerEventSourceRequestRequestTypeDef,
+    CreatePartnerEventSourceResponseTypeDef,
     DeactivateEventSourceRequestRequestTypeDef,
     DeadLetterConfigTypeDef,
     DeauthorizeConnectionRequestRequestTypeDef,
+    DeauthorizeConnectionResponseTypeDef,
     DeleteApiDestinationRequestRequestTypeDef,
     DeleteArchiveRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
+    DeleteConnectionResponseTypeDef,
     DeleteEndpointRequestRequestTypeDef,
     DeleteEventBusRequestRequestTypeDef,
     DeletePartnerEventSourceRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DescribeApiDestinationRequestRequestTypeDef,
+    DescribeApiDestinationResponseTypeDef,
     DescribeArchiveRequestRequestTypeDef,
+    DescribeArchiveResponseTypeDef,
     DescribeConnectionRequestRequestTypeDef,
     DescribeEndpointRequestRequestTypeDef,
     DescribeEventBusRequestRequestTypeDef,
+    DescribeEventBusResponseTypeDef,
     DescribeEventSourceRequestRequestTypeDef,
+    DescribeEventSourceResponseTypeDef,
     DescribePartnerEventSourceRequestRequestTypeDef,
+    DescribePartnerEventSourceResponseTypeDef,
     DescribeReplayRequestRequestTypeDef,
     ReplayDestinationTypeDef,
     DescribeRuleRequestRequestTypeDef,
+    DescribeRuleResponseTypeDef,
     DisableRuleRequestRequestTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableRuleRequestRequestTypeDef,
     EventBusTypeDef,
     EventSourceTypeDef,
     PrimaryTypeDef,
     SecondaryTypeDef,
     HttpParametersTypeDef,
     InputTransformerTypeDef,
@@ -415,66 +429,55 @@
     ListEventSourcesRequestRequestTypeDef,
     ListPartnerEventSourceAccountsRequestRequestTypeDef,
     PartnerEventSourceAccountTypeDef,
     ListPartnerEventSourcesRequestRequestTypeDef,
     PartnerEventSourceTypeDef,
     ListReplaysRequestRequestTypeDef,
     ReplayTypeDef,
-    PaginatorConfigTypeDef,
+    ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
     ListRuleNamesByTargetRequestRequestTypeDef,
+    ListRuleNamesByTargetResponseTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
     ListTargetsByRuleRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutEventsRequestEntryTypeDef,
     PutEventsResultEntryTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResultEntryTypeDef,
+    PutRuleResponseTypeDef,
     PutTargetsResultEntryTypeDef,
     RedshiftDataParametersTypeDef,
     RemovePermissionRequestRequestTypeDef,
     RemoveTargetsRequestRequestTypeDef,
     RemoveTargetsResultEntryTypeDef,
+    ResponseMetadataTypeDef,
     RetryPolicyTypeDef,
     RunCommandTargetTypeDef,
     SageMakerPipelineParameterTypeDef,
     SqsParametersTypeDef,
+    StartReplayResponseTypeDef,
     TestEventPatternRequestRequestTypeDef,
+    TestEventPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiDestinationRequestRequestTypeDef,
+    UpdateApiDestinationResponseTypeDef,
     UpdateArchiveRequestRequestTypeDef,
+    UpdateArchiveResponseTypeDef,
     UpdateConnectionApiKeyAuthRequestParametersTypeDef,
     UpdateConnectionBasicAuthRequestParametersTypeDef,
     UpdateConnectionOAuthClientRequestParametersTypeDef,
-    NetworkConfigurationTypeDef,
-    BatchParametersTypeDef,
-    CancelReplayResponseTypeDef,
-    CreateApiDestinationResponseTypeDef,
-    CreateArchiveResponseTypeDef,
-    CreateConnectionResponseTypeDef,
-    CreateEventBusResponseTypeDef,
-    CreatePartnerEventSourceResponseTypeDef,
-    DeauthorizeConnectionResponseTypeDef,
-    DeleteConnectionResponseTypeDef,
-    DescribeApiDestinationResponseTypeDef,
-    DescribeArchiveResponseTypeDef,
-    DescribeEventBusResponseTypeDef,
-    DescribeEventSourceResponseTypeDef,
-    DescribePartnerEventSourceResponseTypeDef,
-    DescribeRuleResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
+    UpdateConnectionResponseTypeDef,
     ListApiDestinationsResponseTypeDef,
     ListArchivesResponseTypeDef,
-    ListRuleNamesByTargetResponseTypeDef,
-    PutRuleResponseTypeDef,
-    StartReplayResponseTypeDef,
-    TestEventPatternResponseTypeDef,
-    UpdateApiDestinationResponseTypeDef,
-    UpdateArchiveResponseTypeDef,
-    UpdateConnectionResponseTypeDef,
+    NetworkConfigurationTypeDef,
+    BatchParametersTypeDef,
     PutPermissionRequestRequestTypeDef,
     ConnectionHttpParametersTypeDef,
     ListConnectionsResponseTypeDef,
     CreateEventBusRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutRuleRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -482,17 +485,14 @@
     StartReplayRequestRequestTypeDef,
     ListEventBusesResponseTypeDef,
     ListEventSourcesResponseTypeDef,
     FailoverConfigTypeDef,
     ListPartnerEventSourceAccountsResponseTypeDef,
     ListPartnerEventSourcesResponseTypeDef,
     ListReplaysResponseTypeDef,
-    ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
-    ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
     ListRulesResponseTypeDef,
     PutEventsRequestRequestTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestRequestTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
@@ -529,42 +529,42 @@
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

### Comparing `mypy-boto3-events-1.26.58/README.md` & `mypy-boto3-events-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-events"></a>
 
 # mypy-boto3-events
 
 [![PyPI - mypy-boto3-events](https://img.shields.io/pypi/v/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-events?color=blue)](https://pypistats.org/packages/mypy-boto3-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridge 1.26.58](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[boto3.EventBridge 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
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
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,56 +321,70 @@
     ActivateEventSourceRequestRequestTypeDef,
     ApiDestinationTypeDef,
     ArchiveTypeDef,
     AwsVpcConfigurationTypeDef,
     BatchArrayPropertiesTypeDef,
     BatchRetryStrategyTypeDef,
     CancelReplayRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelReplayResponseTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ConditionTypeDef,
     ConnectionApiKeyAuthResponseParametersTypeDef,
     ConnectionBasicAuthResponseParametersTypeDef,
     ConnectionBodyParameterTypeDef,
     ConnectionHeaderParameterTypeDef,
     ConnectionQueryStringParameterTypeDef,
     ConnectionOAuthClientResponseParametersTypeDef,
     ConnectionTypeDef,
     CreateApiDestinationRequestRequestTypeDef,
+    CreateApiDestinationResponseTypeDef,
     CreateArchiveRequestRequestTypeDef,
+    CreateArchiveResponseTypeDef,
     CreateConnectionApiKeyAuthRequestParametersTypeDef,
     CreateConnectionBasicAuthRequestParametersTypeDef,
     CreateConnectionOAuthClientRequestParametersTypeDef,
+    CreateConnectionResponseTypeDef,
     EndpointEventBusTypeDef,
     ReplicationConfigTypeDef,
     TagTypeDef,
+    CreateEventBusResponseTypeDef,
     CreatePartnerEventSourceRequestRequestTypeDef,
+    CreatePartnerEventSourceResponseTypeDef,
     DeactivateEventSourceRequestRequestTypeDef,
     DeadLetterConfigTypeDef,
     DeauthorizeConnectionRequestRequestTypeDef,
+    DeauthorizeConnectionResponseTypeDef,
     DeleteApiDestinationRequestRequestTypeDef,
     DeleteArchiveRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
+    DeleteConnectionResponseTypeDef,
     DeleteEndpointRequestRequestTypeDef,
     DeleteEventBusRequestRequestTypeDef,
     DeletePartnerEventSourceRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DescribeApiDestinationRequestRequestTypeDef,
+    DescribeApiDestinationResponseTypeDef,
     DescribeArchiveRequestRequestTypeDef,
+    DescribeArchiveResponseTypeDef,
     DescribeConnectionRequestRequestTypeDef,
     DescribeEndpointRequestRequestTypeDef,
     DescribeEventBusRequestRequestTypeDef,
+    DescribeEventBusResponseTypeDef,
     DescribeEventSourceRequestRequestTypeDef,
+    DescribeEventSourceResponseTypeDef,
     DescribePartnerEventSourceRequestRequestTypeDef,
+    DescribePartnerEventSourceResponseTypeDef,
     DescribeReplayRequestRequestTypeDef,
     ReplayDestinationTypeDef,
     DescribeRuleRequestRequestTypeDef,
+    DescribeRuleResponseTypeDef,
     DisableRuleRequestRequestTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableRuleRequestRequestTypeDef,
     EventBusTypeDef,
     EventSourceTypeDef,
     PrimaryTypeDef,
     SecondaryTypeDef,
     HttpParametersTypeDef,
     InputTransformerTypeDef,
@@ -383,66 +397,55 @@
     ListEventSourcesRequestRequestTypeDef,
     ListPartnerEventSourceAccountsRequestRequestTypeDef,
     PartnerEventSourceAccountTypeDef,
     ListPartnerEventSourcesRequestRequestTypeDef,
     PartnerEventSourceTypeDef,
     ListReplaysRequestRequestTypeDef,
     ReplayTypeDef,
-    PaginatorConfigTypeDef,
+    ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
     ListRuleNamesByTargetRequestRequestTypeDef,
+    ListRuleNamesByTargetResponseTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
     ListTargetsByRuleRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutEventsRequestEntryTypeDef,
     PutEventsResultEntryTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResultEntryTypeDef,
+    PutRuleResponseTypeDef,
     PutTargetsResultEntryTypeDef,
     RedshiftDataParametersTypeDef,
     RemovePermissionRequestRequestTypeDef,
     RemoveTargetsRequestRequestTypeDef,
     RemoveTargetsResultEntryTypeDef,
+    ResponseMetadataTypeDef,
     RetryPolicyTypeDef,
     RunCommandTargetTypeDef,
     SageMakerPipelineParameterTypeDef,
     SqsParametersTypeDef,
+    StartReplayResponseTypeDef,
     TestEventPatternRequestRequestTypeDef,
+    TestEventPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiDestinationRequestRequestTypeDef,
+    UpdateApiDestinationResponseTypeDef,
     UpdateArchiveRequestRequestTypeDef,
+    UpdateArchiveResponseTypeDef,
     UpdateConnectionApiKeyAuthRequestParametersTypeDef,
     UpdateConnectionBasicAuthRequestParametersTypeDef,
     UpdateConnectionOAuthClientRequestParametersTypeDef,
-    NetworkConfigurationTypeDef,
-    BatchParametersTypeDef,
-    CancelReplayResponseTypeDef,
-    CreateApiDestinationResponseTypeDef,
-    CreateArchiveResponseTypeDef,
-    CreateConnectionResponseTypeDef,
-    CreateEventBusResponseTypeDef,
-    CreatePartnerEventSourceResponseTypeDef,
-    DeauthorizeConnectionResponseTypeDef,
-    DeleteConnectionResponseTypeDef,
-    DescribeApiDestinationResponseTypeDef,
-    DescribeArchiveResponseTypeDef,
-    DescribeEventBusResponseTypeDef,
-    DescribeEventSourceResponseTypeDef,
-    DescribePartnerEventSourceResponseTypeDef,
-    DescribeRuleResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
+    UpdateConnectionResponseTypeDef,
     ListApiDestinationsResponseTypeDef,
     ListArchivesResponseTypeDef,
-    ListRuleNamesByTargetResponseTypeDef,
-    PutRuleResponseTypeDef,
-    StartReplayResponseTypeDef,
-    TestEventPatternResponseTypeDef,
-    UpdateApiDestinationResponseTypeDef,
-    UpdateArchiveResponseTypeDef,
-    UpdateConnectionResponseTypeDef,
+    NetworkConfigurationTypeDef,
+    BatchParametersTypeDef,
     PutPermissionRequestRequestTypeDef,
     ConnectionHttpParametersTypeDef,
     ListConnectionsResponseTypeDef,
     CreateEventBusRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutRuleRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -450,17 +453,14 @@
     StartReplayRequestRequestTypeDef,
     ListEventBusesResponseTypeDef,
     ListEventSourcesResponseTypeDef,
     FailoverConfigTypeDef,
     ListPartnerEventSourceAccountsResponseTypeDef,
     ListPartnerEventSourcesResponseTypeDef,
     ListReplaysResponseTypeDef,
-    ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
-    ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
     ListRulesResponseTypeDef,
     PutEventsRequestRequestTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestRequestTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
@@ -497,42 +497,42 @@
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

### Comparing `mypy-boto3-events-1.26.58/mypy_boto3_events/__init__.py` & `mypy-boto3-events-1.27.0/mypy_boto3_events/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.26.58/mypy_boto3_events/__init__.pyi` & `mypy-boto3-events-1.27.0/mypy_boto3_events/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.26.58/mypy_boto3_events/__main__.py` & `mypy-boto3-events-1.27.0/mypy_boto3_events/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridge 1.26.58\nVersion:         1.26.58\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.EventBridge 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.58")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-events-1.26.58/mypy_boto3_events/client.py` & `mypy-boto3-events-1.27.0/mypy_boto3_events/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.26.58/mypy_boto3_events/client.pyi` & `mypy-boto3-events-1.27.0/mypy_boto3_events/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.26.58/mypy_boto3_events/literals.py` & `mypy-boto3-events-1.27.0/mypy_boto3_events/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApiDestinationHttpMethodType",
     "ApiDestinationStateType",
     "ArchiveStateType",
     "AssignPublicIpType",
     "ConnectionAuthorizationTypeType",
     "ConnectionOAuthHttpMethodType",
@@ -42,15 +41,14 @@
     "EventBridgeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApiDestinationHttpMethodType = Literal["DELETE", "GET", "HEAD", "OPTIONS", "PATCH", "POST", "PUT"]
 ApiDestinationStateType = Literal["ACTIVE", "INACTIVE"]
 ArchiveStateType = Literal[
     "CREATE_FAILED", "CREATING", "DISABLED", "ENABLED", "UPDATE_FAILED", "UPDATING"
 ]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 ConnectionAuthorizationTypeType = Literal["API_KEY", "BASIC", "OAUTH_CLIENT_CREDENTIALS"]
@@ -84,14 +82,15 @@
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
@@ -123,21 +122,23 @@
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
@@ -216,14 +217,15 @@
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
@@ -234,14 +236,15 @@
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
@@ -277,14 +280,15 @@
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
@@ -303,16 +307,19 @@
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
@@ -392,18 +399,21 @@
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

### Comparing `mypy-boto3-events-1.26.58/mypy_boto3_events/literals.pyi` & `mypy-boto3-events-1.27.0/mypy_boto3_events/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ApiDestinationHttpMethodType",
     "ApiDestinationStateType",
     "ArchiveStateType",
     "AssignPublicIpType",
     "ConnectionAuthorizationTypeType",
     "ConnectionOAuthHttpMethodType",
@@ -41,14 +42,15 @@
     "EventBridgeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ApiDestinationHttpMethodType = Literal["DELETE", "GET", "HEAD", "OPTIONS", "PATCH", "POST", "PUT"]
 ApiDestinationStateType = Literal["ACTIVE", "INACTIVE"]
 ArchiveStateType = Literal[
     "CREATE_FAILED", "CREATING", "DISABLED", "ENABLED", "UPDATE_FAILED", "UPDATING"
 ]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 ConnectionAuthorizationTypeType = Literal["API_KEY", "BASIC", "OAUTH_CLIENT_CREDENTIALS"]
@@ -82,14 +84,15 @@
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
@@ -121,21 +124,23 @@
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
@@ -214,14 +219,15 @@
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
@@ -232,14 +238,15 @@
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
@@ -275,14 +282,15 @@
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
@@ -301,16 +309,19 @@
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
@@ -390,18 +401,21 @@
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

### Comparing `mypy-boto3-events-1.26.58/mypy_boto3_events/paginator.py` & `mypy-boto3-events-1.27.0/mypy_boto3_events/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """
 
     def paginate(
         self,
         *,
         TargetArn: str,
         EventBusName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRuleNamesByTargetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListRuleNamesByTarget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listrulenamesbytargetpaginator)
         """
 
 
@@ -73,28 +73,32 @@
     """
 
     def paginate(
         self,
         *,
         NamePrefix: str = ...,
         EventBusName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listrulespaginator)
         """
 
 
 class ListTargetsByRulePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListTargetsByRule)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listtargetsbyrulepaginator)
     """
 
     def paginate(
-        self, *, Rule: str, EventBusName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        Rule: str,
+        EventBusName: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTargetsByRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListTargetsByRule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listtargetsbyrulepaginator)
         """
```

### Comparing `mypy-boto3-events-1.26.58/mypy_boto3_events/paginator.pyi` & `mypy-boto3-events-1.27.0/mypy_boto3_events/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     """
 
     def paginate(
         self,
         *,
         TargetArn: str,
         EventBusName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRuleNamesByTargetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListRuleNamesByTarget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listrulenamesbytargetpaginator)
         """
 
 class ListRulesPaginator(Paginator):
@@ -69,27 +69,31 @@
     """
 
     def paginate(
         self,
         *,
         NamePrefix: str = ...,
         EventBusName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listrulespaginator)
         """
 
 class ListTargetsByRulePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListTargetsByRule)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listtargetsbyrulepaginator)
     """
 
     def paginate(
-        self, *, Rule: str, EventBusName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        Rule: str,
+        EventBusName: str = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTargetsByRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListTargetsByRule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/paginators/#listtargetsbyrulepaginator)
         """
```

### Comparing `mypy-boto3-events-1.26.58/mypy_boto3_events/type_defs.py` & `mypy-boto3-events-1.27.0/mypy_boto3_events/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,56 +47,70 @@
     "ActivateEventSourceRequestRequestTypeDef",
     "ApiDestinationTypeDef",
     "ArchiveTypeDef",
     "AwsVpcConfigurationTypeDef",
     "BatchArrayPropertiesTypeDef",
     "BatchRetryStrategyTypeDef",
     "CancelReplayRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelReplayResponseTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "ConditionTypeDef",
     "ConnectionApiKeyAuthResponseParametersTypeDef",
     "ConnectionBasicAuthResponseParametersTypeDef",
     "ConnectionBodyParameterTypeDef",
     "ConnectionHeaderParameterTypeDef",
     "ConnectionQueryStringParameterTypeDef",
     "ConnectionOAuthClientResponseParametersTypeDef",
     "ConnectionTypeDef",
     "CreateApiDestinationRequestRequestTypeDef",
+    "CreateApiDestinationResponseTypeDef",
     "CreateArchiveRequestRequestTypeDef",
+    "CreateArchiveResponseTypeDef",
     "CreateConnectionApiKeyAuthRequestParametersTypeDef",
     "CreateConnectionBasicAuthRequestParametersTypeDef",
     "CreateConnectionOAuthClientRequestParametersTypeDef",
+    "CreateConnectionResponseTypeDef",
     "EndpointEventBusTypeDef",
     "ReplicationConfigTypeDef",
     "TagTypeDef",
+    "CreateEventBusResponseTypeDef",
     "CreatePartnerEventSourceRequestRequestTypeDef",
+    "CreatePartnerEventSourceResponseTypeDef",
     "DeactivateEventSourceRequestRequestTypeDef",
     "DeadLetterConfigTypeDef",
     "DeauthorizeConnectionRequestRequestTypeDef",
+    "DeauthorizeConnectionResponseTypeDef",
     "DeleteApiDestinationRequestRequestTypeDef",
     "DeleteArchiveRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
+    "DeleteConnectionResponseTypeDef",
     "DeleteEndpointRequestRequestTypeDef",
     "DeleteEventBusRequestRequestTypeDef",
     "DeletePartnerEventSourceRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DescribeApiDestinationRequestRequestTypeDef",
+    "DescribeApiDestinationResponseTypeDef",
     "DescribeArchiveRequestRequestTypeDef",
+    "DescribeArchiveResponseTypeDef",
     "DescribeConnectionRequestRequestTypeDef",
     "DescribeEndpointRequestRequestTypeDef",
     "DescribeEventBusRequestRequestTypeDef",
+    "DescribeEventBusResponseTypeDef",
     "DescribeEventSourceRequestRequestTypeDef",
+    "DescribeEventSourceResponseTypeDef",
     "DescribePartnerEventSourceRequestRequestTypeDef",
+    "DescribePartnerEventSourceResponseTypeDef",
     "DescribeReplayRequestRequestTypeDef",
     "ReplayDestinationTypeDef",
     "DescribeRuleRequestRequestTypeDef",
+    "DescribeRuleResponseTypeDef",
     "DisableRuleRequestRequestTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableRuleRequestRequestTypeDef",
     "EventBusTypeDef",
     "EventSourceTypeDef",
     "PrimaryTypeDef",
     "SecondaryTypeDef",
     "HttpParametersTypeDef",
     "InputTransformerTypeDef",
@@ -109,66 +123,55 @@
     "ListEventSourcesRequestRequestTypeDef",
     "ListPartnerEventSourceAccountsRequestRequestTypeDef",
     "PartnerEventSourceAccountTypeDef",
     "ListPartnerEventSourcesRequestRequestTypeDef",
     "PartnerEventSourceTypeDef",
     "ListReplaysRequestRequestTypeDef",
     "ReplayTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
     "ListRuleNamesByTargetRequestRequestTypeDef",
+    "ListRuleNamesByTargetResponseTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
     "ListTargetsByRuleRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutEventsRequestEntryTypeDef",
     "PutEventsResultEntryTypeDef",
     "PutPartnerEventsRequestEntryTypeDef",
     "PutPartnerEventsResultEntryTypeDef",
+    "PutRuleResponseTypeDef",
     "PutTargetsResultEntryTypeDef",
     "RedshiftDataParametersTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "RemoveTargetsRequestRequestTypeDef",
     "RemoveTargetsResultEntryTypeDef",
+    "ResponseMetadataTypeDef",
     "RetryPolicyTypeDef",
     "RunCommandTargetTypeDef",
     "SageMakerPipelineParameterTypeDef",
     "SqsParametersTypeDef",
+    "StartReplayResponseTypeDef",
     "TestEventPatternRequestRequestTypeDef",
+    "TestEventPatternResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiDestinationRequestRequestTypeDef",
+    "UpdateApiDestinationResponseTypeDef",
     "UpdateArchiveRequestRequestTypeDef",
+    "UpdateArchiveResponseTypeDef",
     "UpdateConnectionApiKeyAuthRequestParametersTypeDef",
     "UpdateConnectionBasicAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthClientRequestParametersTypeDef",
-    "NetworkConfigurationTypeDef",
-    "BatchParametersTypeDef",
-    "CancelReplayResponseTypeDef",
-    "CreateApiDestinationResponseTypeDef",
-    "CreateArchiveResponseTypeDef",
-    "CreateConnectionResponseTypeDef",
-    "CreateEventBusResponseTypeDef",
-    "CreatePartnerEventSourceResponseTypeDef",
-    "DeauthorizeConnectionResponseTypeDef",
-    "DeleteConnectionResponseTypeDef",
-    "DescribeApiDestinationResponseTypeDef",
-    "DescribeArchiveResponseTypeDef",
-    "DescribeEventBusResponseTypeDef",
-    "DescribeEventSourceResponseTypeDef",
-    "DescribePartnerEventSourceResponseTypeDef",
-    "DescribeRuleResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "UpdateConnectionResponseTypeDef",
     "ListApiDestinationsResponseTypeDef",
     "ListArchivesResponseTypeDef",
-    "ListRuleNamesByTargetResponseTypeDef",
-    "PutRuleResponseTypeDef",
-    "StartReplayResponseTypeDef",
-    "TestEventPatternResponseTypeDef",
-    "UpdateApiDestinationResponseTypeDef",
-    "UpdateArchiveResponseTypeDef",
-    "UpdateConnectionResponseTypeDef",
+    "NetworkConfigurationTypeDef",
+    "BatchParametersTypeDef",
     "PutPermissionRequestRequestTypeDef",
     "ConnectionHttpParametersTypeDef",
     "ListConnectionsResponseTypeDef",
     "CreateEventBusRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutRuleRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -176,17 +179,14 @@
     "StartReplayRequestRequestTypeDef",
     "ListEventBusesResponseTypeDef",
     "ListEventSourcesResponseTypeDef",
     "FailoverConfigTypeDef",
     "ListPartnerEventSourceAccountsResponseTypeDef",
     "ListPartnerEventSourcesResponseTypeDef",
     "ListReplaysResponseTypeDef",
-    "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
-    "ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
     "ListRulesResponseTypeDef",
     "PutEventsRequestRequestTypeDef",
     "PutEventsResponseTypeDef",
     "PutPartnerEventsRequestRequestTypeDef",
     "PutPartnerEventsResponseTypeDef",
     "PutTargetsResponseTypeDef",
     "RemoveTargetsResponseTypeDef",
@@ -294,22 +294,21 @@
 CancelReplayRequestRequestTypeDef = TypedDict(
     "CancelReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelReplayResponseTypeDef = TypedDict(
+    "CancelReplayResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ReplayArn": str,
+        "State": ReplayStateType,
+        "StateReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
@@ -431,14 +430,25 @@
 class CreateApiDestinationRequestRequestTypeDef(
     _RequiredCreateApiDestinationRequestRequestTypeDef,
     _OptionalCreateApiDestinationRequestRequestTypeDef,
 ):
     pass
 
 
+CreateApiDestinationResponseTypeDef = TypedDict(
+    "CreateApiDestinationResponseTypeDef",
+    {
+        "ApiDestinationArn": str,
+        "ApiDestinationState": ApiDestinationStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateArchiveRequestRequestTypeDef = TypedDict(
     "_RequiredCreateArchiveRequestRequestTypeDef",
     {
         "ArchiveName": str,
         "EventSourceArn": str,
     },
 )
@@ -455,14 +465,25 @@
 
 class CreateArchiveRequestRequestTypeDef(
     _RequiredCreateArchiveRequestRequestTypeDef, _OptionalCreateArchiveRequestRequestTypeDef
 ):
     pass
 
 
+CreateArchiveResponseTypeDef = TypedDict(
+    "CreateArchiveResponseTypeDef",
+    {
+        "ArchiveArn": str,
+        "State": ArchiveStateType,
+        "StateReason": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateConnectionApiKeyAuthRequestParametersTypeDef = TypedDict(
     "CreateConnectionApiKeyAuthRequestParametersTypeDef",
     {
         "ApiKeyName": str,
         "ApiKeyValue": str,
     },
 )
@@ -479,14 +500,25 @@
     "CreateConnectionOAuthClientRequestParametersTypeDef",
     {
         "ClientID": str,
         "ClientSecret": str,
     },
 )
 
+CreateConnectionResponseTypeDef = TypedDict(
+    "CreateConnectionResponseTypeDef",
+    {
+        "ConnectionArn": str,
+        "ConnectionState": ConnectionStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EndpointEventBusTypeDef = TypedDict(
     "EndpointEventBusTypeDef",
     {
         "EventBusArn": str,
     },
 )
 
@@ -502,22 +534,38 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateEventBusResponseTypeDef = TypedDict(
+    "CreateEventBusResponseTypeDef",
+    {
+        "EventBusArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreatePartnerEventSourceRequestRequestTypeDef = TypedDict(
     "CreatePartnerEventSourceRequestRequestTypeDef",
     {
         "Name": str,
         "Account": str,
     },
 )
 
+CreatePartnerEventSourceResponseTypeDef = TypedDict(
+    "CreatePartnerEventSourceResponseTypeDef",
+    {
+        "EventSourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeactivateEventSourceRequestRequestTypeDef = TypedDict(
     "DeactivateEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -532,14 +580,26 @@
 DeauthorizeConnectionRequestRequestTypeDef = TypedDict(
     "DeauthorizeConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeauthorizeConnectionResponseTypeDef = TypedDict(
+    "DeauthorizeConnectionResponseTypeDef",
+    {
+        "ConnectionArn": str,
+        "ConnectionState": ConnectionStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "LastAuthorizedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteApiDestinationRequestRequestTypeDef = TypedDict(
     "DeleteApiDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -553,14 +613,26 @@
 DeleteConnectionRequestRequestTypeDef = TypedDict(
     "DeleteConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteConnectionResponseTypeDef = TypedDict(
+    "DeleteConnectionResponseTypeDef",
+    {
+        "ConnectionArn": str,
+        "ConnectionState": ConnectionStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "LastAuthorizedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteEndpointRequestRequestTypeDef = TypedDict(
     "DeleteEndpointRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -604,21 +676,56 @@
 DescribeApiDestinationRequestRequestTypeDef = TypedDict(
     "DescribeApiDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DescribeApiDestinationResponseTypeDef = TypedDict(
+    "DescribeApiDestinationResponseTypeDef",
+    {
+        "ApiDestinationArn": str,
+        "Name": str,
+        "Description": str,
+        "ApiDestinationState": ApiDestinationStateType,
+        "ConnectionArn": str,
+        "InvocationEndpoint": str,
+        "HttpMethod": ApiDestinationHttpMethodType,
+        "InvocationRateLimitPerSecond": int,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeArchiveRequestRequestTypeDef = TypedDict(
     "DescribeArchiveRequestRequestTypeDef",
     {
         "ArchiveName": str,
     },
 )
 
+DescribeArchiveResponseTypeDef = TypedDict(
+    "DescribeArchiveResponseTypeDef",
+    {
+        "ArchiveArn": str,
+        "ArchiveName": str,
+        "EventSourceArn": str,
+        "Description": str,
+        "EventPattern": str,
+        "State": ArchiveStateType,
+        "StateReason": str,
+        "RetentionDays": int,
+        "SizeBytes": int,
+        "EventCount": int,
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeConnectionRequestRequestTypeDef = TypedDict(
     "DescribeConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -647,28 +754,60 @@
     "DescribeEventBusRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+DescribeEventBusResponseTypeDef = TypedDict(
+    "DescribeEventBusResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeEventSourceRequestRequestTypeDef = TypedDict(
     "DescribeEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DescribeEventSourceResponseTypeDef = TypedDict(
+    "DescribeEventSourceResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedBy": str,
+        "CreationTime": datetime,
+        "ExpirationTime": datetime,
+        "Name": str,
+        "State": EventSourceStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribePartnerEventSourceRequestRequestTypeDef = TypedDict(
     "DescribePartnerEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DescribePartnerEventSourceResponseTypeDef = TypedDict(
+    "DescribePartnerEventSourceResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeReplayRequestRequestTypeDef = TypedDict(
     "DescribeReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
     },
 )
 
@@ -710,14 +849,31 @@
 
 class DescribeRuleRequestRequestTypeDef(
     _RequiredDescribeRuleRequestRequestTypeDef, _OptionalDescribeRuleRequestRequestTypeDef
 ):
     pass
 
 
+DescribeRuleResponseTypeDef = TypedDict(
+    "DescribeRuleResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "EventPattern": str,
+        "ScheduleExpression": str,
+        "State": RuleStateType,
+        "Description": str,
+        "RoleArn": str,
+        "ManagedBy": str,
+        "EventBusName": str,
+        "CreatedBy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDisableRuleRequestRequestTypeDef = TypedDict(
     "_RequiredDisableRuleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDisableRuleRequestRequestTypeDef = TypedDict(
@@ -749,14 +905,21 @@
     {
         "type": PlacementStrategyTypeType,
         "field": str,
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
 _RequiredEnableRuleRequestRequestTypeDef = TypedDict(
     "_RequiredEnableRuleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalEnableRuleRequestRequestTypeDef = TypedDict(
@@ -1002,24 +1165,37 @@
         "EventLastReplayedTime": datetime,
         "ReplayStartTime": datetime,
         "ReplayEndTime": datetime,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
+    "_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TargetArn": str,
+    },
+)
+_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
+    "_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
+    {
+        "EventBusName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef(
+    _RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
+    _OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRuleNamesByTargetRequestRequestTypeDef = TypedDict(
     "_RequiredListRuleNamesByTargetRequestRequestTypeDef",
     {
         "TargetArn": str,
     },
 )
 _OptionalListRuleNamesByTargetRequestRequestTypeDef = TypedDict(
@@ -1036,14 +1212,33 @@
 class ListRuleNamesByTargetRequestRequestTypeDef(
     _RequiredListRuleNamesByTargetRequestRequestTypeDef,
     _OptionalListRuleNamesByTargetRequestRequestTypeDef,
 ):
     pass
 
 
+ListRuleNamesByTargetResponseTypeDef = TypedDict(
+    "ListRuleNamesByTargetResponseTypeDef",
+    {
+        "RuleNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "ListRulesRequestListRulesPaginateTypeDef",
+    {
+        "NamePrefix": str,
+        "EventBusName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRulesRequestRequestTypeDef = TypedDict(
     "ListRulesRequestRequestTypeDef",
     {
         "NamePrefix": str,
         "EventBusName": str,
         "NextToken": str,
         "Limit": int,
@@ -1070,14 +1265,37 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
+    "_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
+    {
+        "Rule": str,
+    },
+)
+_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
+    "_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
+    {
+        "EventBusName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef(
+    _RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
+    _OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTargetsByRuleRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsByRuleRequestRequestTypeDef",
     {
         "Rule": str,
     },
 )
 _OptionalListTargetsByRuleRequestRequestTypeDef = TypedDict(
@@ -1093,14 +1311,24 @@
 
 class ListTargetsByRuleRequestRequestTypeDef(
     _RequiredListTargetsByRuleRequestRequestTypeDef, _OptionalListTargetsByRuleRequestRequestTypeDef
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
 PutEventsRequestEntryTypeDef = TypedDict(
     "PutEventsRequestEntryTypeDef",
     {
         "Time": Union[datetime, str],
         "Source": str,
         "Resources": Sequence[str],
         "DetailType": str,
@@ -1139,38 +1367,47 @@
         "EventId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+PutRuleResponseTypeDef = TypedDict(
+    "PutRuleResponseTypeDef",
+    {
+        "RuleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutTargetsResultEntryTypeDef = TypedDict(
     "PutTargetsResultEntryTypeDef",
     {
         "TargetId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
 _RequiredRedshiftDataParametersTypeDef = TypedDict(
     "_RequiredRedshiftDataParametersTypeDef",
     {
         "Database": str,
-        "Sql": str,
     },
 )
 _OptionalRedshiftDataParametersTypeDef = TypedDict(
     "_OptionalRedshiftDataParametersTypeDef",
     {
         "SecretManagerArn": str,
         "DbUser": str,
+        "Sql": str,
         "StatementName": str,
         "WithEvent": bool,
+        "Sqls": List[str],
     },
     total=False,
 )
 
 
 class RedshiftDataParametersTypeDef(
     _RequiredRedshiftDataParametersTypeDef, _OptionalRedshiftDataParametersTypeDef
@@ -1217,14 +1454,25 @@
         "TargetId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
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
 RetryPolicyTypeDef = TypedDict(
     "RetryPolicyTypeDef",
     {
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
     },
     total=False,
@@ -1250,22 +1498,41 @@
     "SqsParametersTypeDef",
     {
         "MessageGroupId": str,
     },
     total=False,
 )
 
+StartReplayResponseTypeDef = TypedDict(
+    "StartReplayResponseTypeDef",
+    {
+        "ReplayArn": str,
+        "State": ReplayStateType,
+        "StateReason": str,
+        "ReplayStartTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TestEventPatternRequestRequestTypeDef = TypedDict(
     "TestEventPatternRequestRequestTypeDef",
     {
         "EventPattern": str,
         "Event": str,
     },
 )
 
+TestEventPatternResponseTypeDef = TypedDict(
+    "TestEventPatternResponseTypeDef",
+    {
+        "Result": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1292,14 +1559,25 @@
 class UpdateApiDestinationRequestRequestTypeDef(
     _RequiredUpdateApiDestinationRequestRequestTypeDef,
     _OptionalUpdateApiDestinationRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateApiDestinationResponseTypeDef = TypedDict(
+    "UpdateApiDestinationResponseTypeDef",
+    {
+        "ApiDestinationArn": str,
+        "ApiDestinationState": ApiDestinationStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateArchiveRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateArchiveRequestRequestTypeDef",
     {
         "ArchiveName": str,
     },
 )
 _OptionalUpdateArchiveRequestRequestTypeDef = TypedDict(
@@ -1315,14 +1593,25 @@
 
 class UpdateArchiveRequestRequestTypeDef(
     _RequiredUpdateArchiveRequestRequestTypeDef, _OptionalUpdateArchiveRequestRequestTypeDef
 ):
     pass
 
 
+UpdateArchiveResponseTypeDef = TypedDict(
+    "UpdateArchiveResponseTypeDef",
+    {
+        "ArchiveArn": str,
+        "State": ArchiveStateType,
+        "StateReason": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateConnectionApiKeyAuthRequestParametersTypeDef = TypedDict(
     "UpdateConnectionApiKeyAuthRequestParametersTypeDef",
     {
         "ApiKeyName": str,
         "ApiKeyValue": str,
     },
     total=False,
@@ -1342,304 +1631,72 @@
     {
         "ClientID": str,
         "ClientSecret": str,
     },
     total=False,
 )
 
-NetworkConfigurationTypeDef = TypedDict(
-    "NetworkConfigurationTypeDef",
-    {
-        "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-_RequiredBatchParametersTypeDef = TypedDict(
-    "_RequiredBatchParametersTypeDef",
-    {
-        "JobDefinition": str,
-        "JobName": str,
-    },
-)
-_OptionalBatchParametersTypeDef = TypedDict(
-    "_OptionalBatchParametersTypeDef",
-    {
-        "ArrayProperties": BatchArrayPropertiesTypeDef,
-        "RetryStrategy": BatchRetryStrategyTypeDef,
-    },
-    total=False,
-)
-
-
-class BatchParametersTypeDef(_RequiredBatchParametersTypeDef, _OptionalBatchParametersTypeDef):
-    pass
-
-
-CancelReplayResponseTypeDef = TypedDict(
-    "CancelReplayResponseTypeDef",
-    {
-        "ReplayArn": str,
-        "State": ReplayStateType,
-        "StateReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateApiDestinationResponseTypeDef = TypedDict(
-    "CreateApiDestinationResponseTypeDef",
-    {
-        "ApiDestinationArn": str,
-        "ApiDestinationState": ApiDestinationStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateArchiveResponseTypeDef = TypedDict(
-    "CreateArchiveResponseTypeDef",
-    {
-        "ArchiveArn": str,
-        "State": ArchiveStateType,
-        "StateReason": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateConnectionResponseTypeDef = TypedDict(
-    "CreateConnectionResponseTypeDef",
-    {
-        "ConnectionArn": str,
-        "ConnectionState": ConnectionStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEventBusResponseTypeDef = TypedDict(
-    "CreateEventBusResponseTypeDef",
-    {
-        "EventBusArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePartnerEventSourceResponseTypeDef = TypedDict(
-    "CreatePartnerEventSourceResponseTypeDef",
-    {
-        "EventSourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeauthorizeConnectionResponseTypeDef = TypedDict(
-    "DeauthorizeConnectionResponseTypeDef",
-    {
-        "ConnectionArn": str,
-        "ConnectionState": ConnectionStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LastAuthorizedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteConnectionResponseTypeDef = TypedDict(
-    "DeleteConnectionResponseTypeDef",
+UpdateConnectionResponseTypeDef = TypedDict(
+    "UpdateConnectionResponseTypeDef",
     {
         "ConnectionArn": str,
         "ConnectionState": ConnectionStateType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LastAuthorizedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeApiDestinationResponseTypeDef = TypedDict(
-    "DescribeApiDestinationResponseTypeDef",
-    {
-        "ApiDestinationArn": str,
-        "Name": str,
-        "Description": str,
-        "ApiDestinationState": ApiDestinationStateType,
-        "ConnectionArn": str,
-        "InvocationEndpoint": str,
-        "HttpMethod": ApiDestinationHttpMethodType,
-        "InvocationRateLimitPerSecond": int,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeArchiveResponseTypeDef = TypedDict(
-    "DescribeArchiveResponseTypeDef",
-    {
-        "ArchiveArn": str,
-        "ArchiveName": str,
-        "EventSourceArn": str,
-        "Description": str,
-        "EventPattern": str,
-        "State": ArchiveStateType,
-        "StateReason": str,
-        "RetentionDays": int,
-        "SizeBytes": int,
-        "EventCount": int,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeEventBusResponseTypeDef = TypedDict(
-    "DescribeEventBusResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeEventSourceResponseTypeDef = TypedDict(
-    "DescribeEventSourceResponseTypeDef",
-    {
-        "Arn": str,
-        "CreatedBy": str,
-        "CreationTime": datetime,
-        "ExpirationTime": datetime,
-        "Name": str,
-        "State": EventSourceStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribePartnerEventSourceResponseTypeDef = TypedDict(
-    "DescribePartnerEventSourceResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRuleResponseTypeDef = TypedDict(
-    "DescribeRuleResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "EventPattern": str,
-        "ScheduleExpression": str,
-        "State": RuleStateType,
-        "Description": str,
-        "RoleArn": str,
-        "ManagedBy": str,
-        "EventBusName": str,
-        "CreatedBy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApiDestinationsResponseTypeDef = TypedDict(
     "ListApiDestinationsResponseTypeDef",
     {
         "ApiDestinations": List[ApiDestinationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListArchivesResponseTypeDef = TypedDict(
     "ListArchivesResponseTypeDef",
     {
         "Archives": List[ArchiveTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRuleNamesByTargetResponseTypeDef = TypedDict(
-    "ListRuleNamesByTargetResponseTypeDef",
+NetworkConfigurationTypeDef = TypedDict(
+    "NetworkConfigurationTypeDef",
     {
-        "RuleNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
+    total=False,
 )
 
-PutRuleResponseTypeDef = TypedDict(
-    "PutRuleResponseTypeDef",
+_RequiredBatchParametersTypeDef = TypedDict(
+    "_RequiredBatchParametersTypeDef",
     {
-        "RuleArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobDefinition": str,
+        "JobName": str,
     },
 )
-
-StartReplayResponseTypeDef = TypedDict(
-    "StartReplayResponseTypeDef",
+_OptionalBatchParametersTypeDef = TypedDict(
+    "_OptionalBatchParametersTypeDef",
     {
-        "ReplayArn": str,
-        "State": ReplayStateType,
-        "StateReason": str,
-        "ReplayStartTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ArrayProperties": BatchArrayPropertiesTypeDef,
+        "RetryStrategy": BatchRetryStrategyTypeDef,
     },
+    total=False,
 )
 
-TestEventPatternResponseTypeDef = TypedDict(
-    "TestEventPatternResponseTypeDef",
-    {
-        "Result": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpdateApiDestinationResponseTypeDef = TypedDict(
-    "UpdateApiDestinationResponseTypeDef",
-    {
-        "ApiDestinationArn": str,
-        "ApiDestinationState": ApiDestinationStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateArchiveResponseTypeDef = TypedDict(
-    "UpdateArchiveResponseTypeDef",
-    {
-        "ArchiveArn": str,
-        "State": ArchiveStateType,
-        "StateReason": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class BatchParametersTypeDef(_RequiredBatchParametersTypeDef, _OptionalBatchParametersTypeDef):
+    pass
 
-UpdateConnectionResponseTypeDef = TypedDict(
-    "UpdateConnectionResponseTypeDef",
-    {
-        "ConnectionArn": str,
-        "ConnectionState": ConnectionStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LastAuthorizedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 PutPermissionRequestRequestTypeDef = TypedDict(
     "PutPermissionRequestRequestTypeDef",
     {
         "EventBusName": str,
         "Action": str,
         "Principal": str,
@@ -1661,15 +1718,15 @@
 )
 
 ListConnectionsResponseTypeDef = TypedDict(
     "ListConnectionsResponseTypeDef",
     {
         "Connections": List[ConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEventBusRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventBusRequestRequestTypeDef",
     {
         "Name": str,
@@ -1691,15 +1748,15 @@
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutRuleRequestRequestTypeDef",
     {
         "Name": str,
@@ -1745,15 +1802,15 @@
         "EventSourceArn": str,
         "Destination": ReplayDestinationTypeDef,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
         "EventLastReplayedTime": datetime,
         "ReplayStartTime": datetime,
         "ReplayEndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartReplayRequestRequestTypeDef = TypedDict(
     "_RequiredStartReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
@@ -1779,24 +1836,24 @@
 
 
 ListEventBusesResponseTypeDef = TypedDict(
     "ListEventBusesResponseTypeDef",
     {
         "EventBuses": List[EventBusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventSourcesResponseTypeDef = TypedDict(
     "ListEventSourcesResponseTypeDef",
     {
         "EventSources": List[EventSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FailoverConfigTypeDef = TypedDict(
     "FailoverConfigTypeDef",
     {
         "Primary": PrimaryTypeDef,
@@ -1805,98 +1862,42 @@
 )
 
 ListPartnerEventSourceAccountsResponseTypeDef = TypedDict(
     "ListPartnerEventSourceAccountsResponseTypeDef",
     {
         "PartnerEventSourceAccounts": List[PartnerEventSourceAccountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPartnerEventSourcesResponseTypeDef = TypedDict(
     "ListPartnerEventSourcesResponseTypeDef",
     {
         "PartnerEventSources": List[PartnerEventSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReplaysResponseTypeDef = TypedDict(
     "ListReplaysResponseTypeDef",
     {
         "Replays": List[ReplayTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
-    "_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
-    {
-        "TargetArn": str,
-    },
-)
-_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
-    "_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
-    {
-        "EventBusName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
-)
-
-
-class ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef(
-    _RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
-    _OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
-):
-    pass
-
-
-ListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "ListRulesRequestListRulesPaginateTypeDef",
-    {
-        "NamePrefix": str,
-        "EventBusName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
-    "_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
-    {
-        "Rule": str,
-    },
-)
-_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
-    "_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
-    {
-        "EventBusName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
 )
 
-
-class ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef(
-    _RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
-    _OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
-):
-    pass
-
-
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "Rules": List[RuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutEventsRequestRequestTypeDef = TypedDict(
     "_RequiredPutEventsRequestRequestTypeDef",
     {
         "Entries": Sequence[PutEventsRequestEntryTypeDef],
@@ -1918,15 +1919,15 @@
 
 
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "Entries": List[PutEventsResultEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutPartnerEventsRequestRequestTypeDef = TypedDict(
     "PutPartnerEventsRequestRequestTypeDef",
     {
         "Entries": Sequence[PutPartnerEventsRequestEntryTypeDef],
@@ -1934,33 +1935,33 @@
 )
 
 PutPartnerEventsResponseTypeDef = TypedDict(
     "PutPartnerEventsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "Entries": List[PutPartnerEventsResultEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutTargetsResponseTypeDef = TypedDict(
     "PutTargetsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "FailedEntries": List[PutTargetsResultEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RemoveTargetsResponseTypeDef = TypedDict(
     "RemoveTargetsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "FailedEntries": List[RemoveTargetsResultEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RunCommandParametersTypeDef = TypedDict(
     "RunCommandParametersTypeDef",
     {
         "RunCommandTargets": List[RunCommandTargetTypeDef],
@@ -2156,15 +2157,15 @@
         "Name": str,
         "Arn": str,
         "RoutingConfig": RoutingConfigTypeDef,
         "ReplicationConfig": ReplicationConfigTypeDef,
         "EventBuses": List[EndpointEventBusTypeDef],
         "RoleArn": str,
         "State": EndpointStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointResponseTypeDef = TypedDict(
     "DescribeEndpointResponseTypeDef",
     {
         "Name": str,
@@ -2176,15 +2177,15 @@
         "RoleArn": str,
         "EndpointId": str,
         "EndpointUrl": str,
         "State": EndpointStateType,
         "StateReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Name": str,
@@ -2237,24 +2238,24 @@
         "RoutingConfig": RoutingConfigTypeDef,
         "ReplicationConfig": ReplicationConfigTypeDef,
         "EventBuses": List[EndpointEventBusTypeDef],
         "RoleArn": str,
         "EndpointId": str,
         "EndpointUrl": str,
         "State": EndpointStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTargetsByRuleResponseTypeDef = TypedDict(
     "ListTargetsByRuleResponseTypeDef",
     {
         "Targets": List[TargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredPutTargetsRequestRequestTypeDef",
     {
         "Rule": str,
@@ -2286,15 +2287,15 @@
         "StateReason": str,
         "AuthorizationType": ConnectionAuthorizationTypeType,
         "SecretArn": str,
         "AuthParameters": ConnectionAuthResponseParametersTypeDef,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LastAuthorizedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionRequestRequestTypeDef",
     {
         "Name": str,
@@ -2341,10 +2342,10 @@
 
 
 ListEndpointsResponseTypeDef = TypedDict(
     "ListEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-events-1.26.58/mypy_boto3_events/type_defs.pyi` & `mypy-boto3-events-1.27.0/mypy_boto3_events/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -46,56 +46,70 @@
     "ActivateEventSourceRequestRequestTypeDef",
     "ApiDestinationTypeDef",
     "ArchiveTypeDef",
     "AwsVpcConfigurationTypeDef",
     "BatchArrayPropertiesTypeDef",
     "BatchRetryStrategyTypeDef",
     "CancelReplayRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CancelReplayResponseTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "ConditionTypeDef",
     "ConnectionApiKeyAuthResponseParametersTypeDef",
     "ConnectionBasicAuthResponseParametersTypeDef",
     "ConnectionBodyParameterTypeDef",
     "ConnectionHeaderParameterTypeDef",
     "ConnectionQueryStringParameterTypeDef",
     "ConnectionOAuthClientResponseParametersTypeDef",
     "ConnectionTypeDef",
     "CreateApiDestinationRequestRequestTypeDef",
+    "CreateApiDestinationResponseTypeDef",
     "CreateArchiveRequestRequestTypeDef",
+    "CreateArchiveResponseTypeDef",
     "CreateConnectionApiKeyAuthRequestParametersTypeDef",
     "CreateConnectionBasicAuthRequestParametersTypeDef",
     "CreateConnectionOAuthClientRequestParametersTypeDef",
+    "CreateConnectionResponseTypeDef",
     "EndpointEventBusTypeDef",
     "ReplicationConfigTypeDef",
     "TagTypeDef",
+    "CreateEventBusResponseTypeDef",
     "CreatePartnerEventSourceRequestRequestTypeDef",
+    "CreatePartnerEventSourceResponseTypeDef",
     "DeactivateEventSourceRequestRequestTypeDef",
     "DeadLetterConfigTypeDef",
     "DeauthorizeConnectionRequestRequestTypeDef",
+    "DeauthorizeConnectionResponseTypeDef",
     "DeleteApiDestinationRequestRequestTypeDef",
     "DeleteArchiveRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
+    "DeleteConnectionResponseTypeDef",
     "DeleteEndpointRequestRequestTypeDef",
     "DeleteEventBusRequestRequestTypeDef",
     "DeletePartnerEventSourceRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DescribeApiDestinationRequestRequestTypeDef",
+    "DescribeApiDestinationResponseTypeDef",
     "DescribeArchiveRequestRequestTypeDef",
+    "DescribeArchiveResponseTypeDef",
     "DescribeConnectionRequestRequestTypeDef",
     "DescribeEndpointRequestRequestTypeDef",
     "DescribeEventBusRequestRequestTypeDef",
+    "DescribeEventBusResponseTypeDef",
     "DescribeEventSourceRequestRequestTypeDef",
+    "DescribeEventSourceResponseTypeDef",
     "DescribePartnerEventSourceRequestRequestTypeDef",
+    "DescribePartnerEventSourceResponseTypeDef",
     "DescribeReplayRequestRequestTypeDef",
     "ReplayDestinationTypeDef",
     "DescribeRuleRequestRequestTypeDef",
+    "DescribeRuleResponseTypeDef",
     "DisableRuleRequestRequestTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableRuleRequestRequestTypeDef",
     "EventBusTypeDef",
     "EventSourceTypeDef",
     "PrimaryTypeDef",
     "SecondaryTypeDef",
     "HttpParametersTypeDef",
     "InputTransformerTypeDef",
@@ -108,66 +122,55 @@
     "ListEventSourcesRequestRequestTypeDef",
     "ListPartnerEventSourceAccountsRequestRequestTypeDef",
     "PartnerEventSourceAccountTypeDef",
     "ListPartnerEventSourcesRequestRequestTypeDef",
     "PartnerEventSourceTypeDef",
     "ListReplaysRequestRequestTypeDef",
     "ReplayTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
     "ListRuleNamesByTargetRequestRequestTypeDef",
+    "ListRuleNamesByTargetResponseTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
     "ListTargetsByRuleRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PutEventsRequestEntryTypeDef",
     "PutEventsResultEntryTypeDef",
     "PutPartnerEventsRequestEntryTypeDef",
     "PutPartnerEventsResultEntryTypeDef",
+    "PutRuleResponseTypeDef",
     "PutTargetsResultEntryTypeDef",
     "RedshiftDataParametersTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "RemoveTargetsRequestRequestTypeDef",
     "RemoveTargetsResultEntryTypeDef",
+    "ResponseMetadataTypeDef",
     "RetryPolicyTypeDef",
     "RunCommandTargetTypeDef",
     "SageMakerPipelineParameterTypeDef",
     "SqsParametersTypeDef",
+    "StartReplayResponseTypeDef",
     "TestEventPatternRequestRequestTypeDef",
+    "TestEventPatternResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiDestinationRequestRequestTypeDef",
+    "UpdateApiDestinationResponseTypeDef",
     "UpdateArchiveRequestRequestTypeDef",
+    "UpdateArchiveResponseTypeDef",
     "UpdateConnectionApiKeyAuthRequestParametersTypeDef",
     "UpdateConnectionBasicAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthClientRequestParametersTypeDef",
-    "NetworkConfigurationTypeDef",
-    "BatchParametersTypeDef",
-    "CancelReplayResponseTypeDef",
-    "CreateApiDestinationResponseTypeDef",
-    "CreateArchiveResponseTypeDef",
-    "CreateConnectionResponseTypeDef",
-    "CreateEventBusResponseTypeDef",
-    "CreatePartnerEventSourceResponseTypeDef",
-    "DeauthorizeConnectionResponseTypeDef",
-    "DeleteConnectionResponseTypeDef",
-    "DescribeApiDestinationResponseTypeDef",
-    "DescribeArchiveResponseTypeDef",
-    "DescribeEventBusResponseTypeDef",
-    "DescribeEventSourceResponseTypeDef",
-    "DescribePartnerEventSourceResponseTypeDef",
-    "DescribeRuleResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "UpdateConnectionResponseTypeDef",
     "ListApiDestinationsResponseTypeDef",
     "ListArchivesResponseTypeDef",
-    "ListRuleNamesByTargetResponseTypeDef",
-    "PutRuleResponseTypeDef",
-    "StartReplayResponseTypeDef",
-    "TestEventPatternResponseTypeDef",
-    "UpdateApiDestinationResponseTypeDef",
-    "UpdateArchiveResponseTypeDef",
-    "UpdateConnectionResponseTypeDef",
+    "NetworkConfigurationTypeDef",
+    "BatchParametersTypeDef",
     "PutPermissionRequestRequestTypeDef",
     "ConnectionHttpParametersTypeDef",
     "ListConnectionsResponseTypeDef",
     "CreateEventBusRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutRuleRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -175,17 +178,14 @@
     "StartReplayRequestRequestTypeDef",
     "ListEventBusesResponseTypeDef",
     "ListEventSourcesResponseTypeDef",
     "FailoverConfigTypeDef",
     "ListPartnerEventSourceAccountsResponseTypeDef",
     "ListPartnerEventSourcesResponseTypeDef",
     "ListReplaysResponseTypeDef",
-    "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
-    "ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
     "ListRulesResponseTypeDef",
     "PutEventsRequestRequestTypeDef",
     "PutEventsResponseTypeDef",
     "PutPartnerEventsRequestRequestTypeDef",
     "PutPartnerEventsResponseTypeDef",
     "PutTargetsResponseTypeDef",
     "RemoveTargetsResponseTypeDef",
@@ -291,22 +291,21 @@
 CancelReplayRequestRequestTypeDef = TypedDict(
     "CancelReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelReplayResponseTypeDef = TypedDict(
+    "CancelReplayResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ReplayArn": str,
+        "State": ReplayStateType,
+        "StateReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
@@ -424,14 +423,25 @@
 
 class CreateApiDestinationRequestRequestTypeDef(
     _RequiredCreateApiDestinationRequestRequestTypeDef,
     _OptionalCreateApiDestinationRequestRequestTypeDef,
 ):
     pass
 
+CreateApiDestinationResponseTypeDef = TypedDict(
+    "CreateApiDestinationResponseTypeDef",
+    {
+        "ApiDestinationArn": str,
+        "ApiDestinationState": ApiDestinationStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateArchiveRequestRequestTypeDef = TypedDict(
     "_RequiredCreateArchiveRequestRequestTypeDef",
     {
         "ArchiveName": str,
         "EventSourceArn": str,
     },
 )
@@ -446,14 +456,25 @@
 )
 
 class CreateArchiveRequestRequestTypeDef(
     _RequiredCreateArchiveRequestRequestTypeDef, _OptionalCreateArchiveRequestRequestTypeDef
 ):
     pass
 
+CreateArchiveResponseTypeDef = TypedDict(
+    "CreateArchiveResponseTypeDef",
+    {
+        "ArchiveArn": str,
+        "State": ArchiveStateType,
+        "StateReason": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateConnectionApiKeyAuthRequestParametersTypeDef = TypedDict(
     "CreateConnectionApiKeyAuthRequestParametersTypeDef",
     {
         "ApiKeyName": str,
         "ApiKeyValue": str,
     },
 )
@@ -470,14 +491,25 @@
     "CreateConnectionOAuthClientRequestParametersTypeDef",
     {
         "ClientID": str,
         "ClientSecret": str,
     },
 )
 
+CreateConnectionResponseTypeDef = TypedDict(
+    "CreateConnectionResponseTypeDef",
+    {
+        "ConnectionArn": str,
+        "ConnectionState": ConnectionStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EndpointEventBusTypeDef = TypedDict(
     "EndpointEventBusTypeDef",
     {
         "EventBusArn": str,
     },
 )
 
@@ -493,22 +525,38 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateEventBusResponseTypeDef = TypedDict(
+    "CreateEventBusResponseTypeDef",
+    {
+        "EventBusArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreatePartnerEventSourceRequestRequestTypeDef = TypedDict(
     "CreatePartnerEventSourceRequestRequestTypeDef",
     {
         "Name": str,
         "Account": str,
     },
 )
 
+CreatePartnerEventSourceResponseTypeDef = TypedDict(
+    "CreatePartnerEventSourceResponseTypeDef",
+    {
+        "EventSourceArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeactivateEventSourceRequestRequestTypeDef = TypedDict(
     "DeactivateEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -523,14 +571,26 @@
 DeauthorizeConnectionRequestRequestTypeDef = TypedDict(
     "DeauthorizeConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeauthorizeConnectionResponseTypeDef = TypedDict(
+    "DeauthorizeConnectionResponseTypeDef",
+    {
+        "ConnectionArn": str,
+        "ConnectionState": ConnectionStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "LastAuthorizedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteApiDestinationRequestRequestTypeDef = TypedDict(
     "DeleteApiDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -544,14 +604,26 @@
 DeleteConnectionRequestRequestTypeDef = TypedDict(
     "DeleteConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteConnectionResponseTypeDef = TypedDict(
+    "DeleteConnectionResponseTypeDef",
+    {
+        "ConnectionArn": str,
+        "ConnectionState": ConnectionStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "LastAuthorizedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteEndpointRequestRequestTypeDef = TypedDict(
     "DeleteEndpointRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -593,21 +665,56 @@
 DescribeApiDestinationRequestRequestTypeDef = TypedDict(
     "DescribeApiDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DescribeApiDestinationResponseTypeDef = TypedDict(
+    "DescribeApiDestinationResponseTypeDef",
+    {
+        "ApiDestinationArn": str,
+        "Name": str,
+        "Description": str,
+        "ApiDestinationState": ApiDestinationStateType,
+        "ConnectionArn": str,
+        "InvocationEndpoint": str,
+        "HttpMethod": ApiDestinationHttpMethodType,
+        "InvocationRateLimitPerSecond": int,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeArchiveRequestRequestTypeDef = TypedDict(
     "DescribeArchiveRequestRequestTypeDef",
     {
         "ArchiveName": str,
     },
 )
 
+DescribeArchiveResponseTypeDef = TypedDict(
+    "DescribeArchiveResponseTypeDef",
+    {
+        "ArchiveArn": str,
+        "ArchiveName": str,
+        "EventSourceArn": str,
+        "Description": str,
+        "EventPattern": str,
+        "State": ArchiveStateType,
+        "StateReason": str,
+        "RetentionDays": int,
+        "SizeBytes": int,
+        "EventCount": int,
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeConnectionRequestRequestTypeDef = TypedDict(
     "DescribeConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -634,28 +741,60 @@
     "DescribeEventBusRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+DescribeEventBusResponseTypeDef = TypedDict(
+    "DescribeEventBusResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "Policy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeEventSourceRequestRequestTypeDef = TypedDict(
     "DescribeEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DescribeEventSourceResponseTypeDef = TypedDict(
+    "DescribeEventSourceResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedBy": str,
+        "CreationTime": datetime,
+        "ExpirationTime": datetime,
+        "Name": str,
+        "State": EventSourceStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribePartnerEventSourceRequestRequestTypeDef = TypedDict(
     "DescribePartnerEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DescribePartnerEventSourceResponseTypeDef = TypedDict(
+    "DescribePartnerEventSourceResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeReplayRequestRequestTypeDef = TypedDict(
     "DescribeReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
     },
 )
 
@@ -693,14 +832,31 @@
 )
 
 class DescribeRuleRequestRequestTypeDef(
     _RequiredDescribeRuleRequestRequestTypeDef, _OptionalDescribeRuleRequestRequestTypeDef
 ):
     pass
 
+DescribeRuleResponseTypeDef = TypedDict(
+    "DescribeRuleResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "EventPattern": str,
+        "ScheduleExpression": str,
+        "State": RuleStateType,
+        "Description": str,
+        "RoleArn": str,
+        "ManagedBy": str,
+        "EventBusName": str,
+        "CreatedBy": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDisableRuleRequestRequestTypeDef = TypedDict(
     "_RequiredDisableRuleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDisableRuleRequestRequestTypeDef = TypedDict(
@@ -730,14 +886,21 @@
     {
         "type": PlacementStrategyTypeType,
         "field": str,
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
 _RequiredEnableRuleRequestRequestTypeDef = TypedDict(
     "_RequiredEnableRuleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalEnableRuleRequestRequestTypeDef = TypedDict(
@@ -975,24 +1138,35 @@
         "EventLastReplayedTime": datetime,
         "ReplayStartTime": datetime,
         "ReplayEndTime": datetime,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
+    "_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TargetArn": str,
+    },
+)
+_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
+    "_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
+    {
+        "EventBusName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef(
+    _RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
+    _OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
+):
+    pass
+
 _RequiredListRuleNamesByTargetRequestRequestTypeDef = TypedDict(
     "_RequiredListRuleNamesByTargetRequestRequestTypeDef",
     {
         "TargetArn": str,
     },
 )
 _OptionalListRuleNamesByTargetRequestRequestTypeDef = TypedDict(
@@ -1007,14 +1181,33 @@
 
 class ListRuleNamesByTargetRequestRequestTypeDef(
     _RequiredListRuleNamesByTargetRequestRequestTypeDef,
     _OptionalListRuleNamesByTargetRequestRequestTypeDef,
 ):
     pass
 
+ListRuleNamesByTargetResponseTypeDef = TypedDict(
+    "ListRuleNamesByTargetResponseTypeDef",
+    {
+        "RuleNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "ListRulesRequestListRulesPaginateTypeDef",
+    {
+        "NamePrefix": str,
+        "EventBusName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRulesRequestRequestTypeDef = TypedDict(
     "ListRulesRequestRequestTypeDef",
     {
         "NamePrefix": str,
         "EventBusName": str,
         "NextToken": str,
         "Limit": int,
@@ -1041,14 +1234,35 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
+    "_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
+    {
+        "Rule": str,
+    },
+)
+_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
+    "_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
+    {
+        "EventBusName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef(
+    _RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
+    _OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
+):
+    pass
+
 _RequiredListTargetsByRuleRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsByRuleRequestRequestTypeDef",
     {
         "Rule": str,
     },
 )
 _OptionalListTargetsByRuleRequestRequestTypeDef = TypedDict(
@@ -1062,14 +1276,24 @@
 )
 
 class ListTargetsByRuleRequestRequestTypeDef(
     _RequiredListTargetsByRuleRequestRequestTypeDef, _OptionalListTargetsByRuleRequestRequestTypeDef
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
 PutEventsRequestEntryTypeDef = TypedDict(
     "PutEventsRequestEntryTypeDef",
     {
         "Time": Union[datetime, str],
         "Source": str,
         "Resources": Sequence[str],
         "DetailType": str,
@@ -1108,38 +1332,47 @@
         "EventId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+PutRuleResponseTypeDef = TypedDict(
+    "PutRuleResponseTypeDef",
+    {
+        "RuleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutTargetsResultEntryTypeDef = TypedDict(
     "PutTargetsResultEntryTypeDef",
     {
         "TargetId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
 _RequiredRedshiftDataParametersTypeDef = TypedDict(
     "_RequiredRedshiftDataParametersTypeDef",
     {
         "Database": str,
-        "Sql": str,
     },
 )
 _OptionalRedshiftDataParametersTypeDef = TypedDict(
     "_OptionalRedshiftDataParametersTypeDef",
     {
         "SecretManagerArn": str,
         "DbUser": str,
+        "Sql": str,
         "StatementName": str,
         "WithEvent": bool,
+        "Sqls": List[str],
     },
     total=False,
 )
 
 class RedshiftDataParametersTypeDef(
     _RequiredRedshiftDataParametersTypeDef, _OptionalRedshiftDataParametersTypeDef
 ):
@@ -1182,14 +1415,25 @@
         "TargetId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
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
 RetryPolicyTypeDef = TypedDict(
     "RetryPolicyTypeDef",
     {
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
     },
     total=False,
@@ -1215,22 +1459,41 @@
     "SqsParametersTypeDef",
     {
         "MessageGroupId": str,
     },
     total=False,
 )
 
+StartReplayResponseTypeDef = TypedDict(
+    "StartReplayResponseTypeDef",
+    {
+        "ReplayArn": str,
+        "State": ReplayStateType,
+        "StateReason": str,
+        "ReplayStartTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TestEventPatternRequestRequestTypeDef = TypedDict(
     "TestEventPatternRequestRequestTypeDef",
     {
         "EventPattern": str,
         "Event": str,
     },
 )
 
+TestEventPatternResponseTypeDef = TypedDict(
+    "TestEventPatternResponseTypeDef",
+    {
+        "Result": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1255,14 +1518,25 @@
 
 class UpdateApiDestinationRequestRequestTypeDef(
     _RequiredUpdateApiDestinationRequestRequestTypeDef,
     _OptionalUpdateApiDestinationRequestRequestTypeDef,
 ):
     pass
 
+UpdateApiDestinationResponseTypeDef = TypedDict(
+    "UpdateApiDestinationResponseTypeDef",
+    {
+        "ApiDestinationArn": str,
+        "ApiDestinationState": ApiDestinationStateType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateArchiveRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateArchiveRequestRequestTypeDef",
     {
         "ArchiveName": str,
     },
 )
 _OptionalUpdateArchiveRequestRequestTypeDef = TypedDict(
@@ -1276,14 +1550,25 @@
 )
 
 class UpdateArchiveRequestRequestTypeDef(
     _RequiredUpdateArchiveRequestRequestTypeDef, _OptionalUpdateArchiveRequestRequestTypeDef
 ):
     pass
 
+UpdateArchiveResponseTypeDef = TypedDict(
+    "UpdateArchiveResponseTypeDef",
+    {
+        "ArchiveArn": str,
+        "State": ArchiveStateType,
+        "StateReason": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateConnectionApiKeyAuthRequestParametersTypeDef = TypedDict(
     "UpdateConnectionApiKeyAuthRequestParametersTypeDef",
     {
         "ApiKeyName": str,
         "ApiKeyValue": str,
     },
     total=False,
@@ -1303,302 +1588,70 @@
     {
         "ClientID": str,
         "ClientSecret": str,
     },
     total=False,
 )
 
-NetworkConfigurationTypeDef = TypedDict(
-    "NetworkConfigurationTypeDef",
-    {
-        "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-_RequiredBatchParametersTypeDef = TypedDict(
-    "_RequiredBatchParametersTypeDef",
-    {
-        "JobDefinition": str,
-        "JobName": str,
-    },
-)
-_OptionalBatchParametersTypeDef = TypedDict(
-    "_OptionalBatchParametersTypeDef",
-    {
-        "ArrayProperties": BatchArrayPropertiesTypeDef,
-        "RetryStrategy": BatchRetryStrategyTypeDef,
-    },
-    total=False,
-)
-
-class BatchParametersTypeDef(_RequiredBatchParametersTypeDef, _OptionalBatchParametersTypeDef):
-    pass
-
-CancelReplayResponseTypeDef = TypedDict(
-    "CancelReplayResponseTypeDef",
-    {
-        "ReplayArn": str,
-        "State": ReplayStateType,
-        "StateReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateApiDestinationResponseTypeDef = TypedDict(
-    "CreateApiDestinationResponseTypeDef",
-    {
-        "ApiDestinationArn": str,
-        "ApiDestinationState": ApiDestinationStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateArchiveResponseTypeDef = TypedDict(
-    "CreateArchiveResponseTypeDef",
-    {
-        "ArchiveArn": str,
-        "State": ArchiveStateType,
-        "StateReason": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateConnectionResponseTypeDef = TypedDict(
-    "CreateConnectionResponseTypeDef",
-    {
-        "ConnectionArn": str,
-        "ConnectionState": ConnectionStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEventBusResponseTypeDef = TypedDict(
-    "CreateEventBusResponseTypeDef",
-    {
-        "EventBusArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePartnerEventSourceResponseTypeDef = TypedDict(
-    "CreatePartnerEventSourceResponseTypeDef",
-    {
-        "EventSourceArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeauthorizeConnectionResponseTypeDef = TypedDict(
-    "DeauthorizeConnectionResponseTypeDef",
-    {
-        "ConnectionArn": str,
-        "ConnectionState": ConnectionStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LastAuthorizedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteConnectionResponseTypeDef = TypedDict(
-    "DeleteConnectionResponseTypeDef",
+UpdateConnectionResponseTypeDef = TypedDict(
+    "UpdateConnectionResponseTypeDef",
     {
         "ConnectionArn": str,
         "ConnectionState": ConnectionStateType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LastAuthorizedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeApiDestinationResponseTypeDef = TypedDict(
-    "DescribeApiDestinationResponseTypeDef",
-    {
-        "ApiDestinationArn": str,
-        "Name": str,
-        "Description": str,
-        "ApiDestinationState": ApiDestinationStateType,
-        "ConnectionArn": str,
-        "InvocationEndpoint": str,
-        "HttpMethod": ApiDestinationHttpMethodType,
-        "InvocationRateLimitPerSecond": int,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeArchiveResponseTypeDef = TypedDict(
-    "DescribeArchiveResponseTypeDef",
-    {
-        "ArchiveArn": str,
-        "ArchiveName": str,
-        "EventSourceArn": str,
-        "Description": str,
-        "EventPattern": str,
-        "State": ArchiveStateType,
-        "StateReason": str,
-        "RetentionDays": int,
-        "SizeBytes": int,
-        "EventCount": int,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeEventBusResponseTypeDef = TypedDict(
-    "DescribeEventBusResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Policy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeEventSourceResponseTypeDef = TypedDict(
-    "DescribeEventSourceResponseTypeDef",
-    {
-        "Arn": str,
-        "CreatedBy": str,
-        "CreationTime": datetime,
-        "ExpirationTime": datetime,
-        "Name": str,
-        "State": EventSourceStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribePartnerEventSourceResponseTypeDef = TypedDict(
-    "DescribePartnerEventSourceResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeRuleResponseTypeDef = TypedDict(
-    "DescribeRuleResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "EventPattern": str,
-        "ScheduleExpression": str,
-        "State": RuleStateType,
-        "Description": str,
-        "RoleArn": str,
-        "ManagedBy": str,
-        "EventBusName": str,
-        "CreatedBy": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListApiDestinationsResponseTypeDef = TypedDict(
     "ListApiDestinationsResponseTypeDef",
     {
         "ApiDestinations": List[ApiDestinationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListArchivesResponseTypeDef = TypedDict(
     "ListArchivesResponseTypeDef",
     {
         "Archives": List[ArchiveTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListRuleNamesByTargetResponseTypeDef = TypedDict(
-    "ListRuleNamesByTargetResponseTypeDef",
-    {
-        "RuleNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutRuleResponseTypeDef = TypedDict(
-    "PutRuleResponseTypeDef",
-    {
-        "RuleArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartReplayResponseTypeDef = TypedDict(
-    "StartReplayResponseTypeDef",
-    {
-        "ReplayArn": str,
-        "State": ReplayStateType,
-        "StateReason": str,
-        "ReplayStartTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TestEventPatternResponseTypeDef = TypedDict(
-    "TestEventPatternResponseTypeDef",
+NetworkConfigurationTypeDef = TypedDict(
+    "NetworkConfigurationTypeDef",
     {
-        "Result": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
+    total=False,
 )
 
-UpdateApiDestinationResponseTypeDef = TypedDict(
-    "UpdateApiDestinationResponseTypeDef",
+_RequiredBatchParametersTypeDef = TypedDict(
+    "_RequiredBatchParametersTypeDef",
     {
-        "ApiDestinationArn": str,
-        "ApiDestinationState": ApiDestinationStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "JobDefinition": str,
+        "JobName": str,
     },
 )
-
-UpdateArchiveResponseTypeDef = TypedDict(
-    "UpdateArchiveResponseTypeDef",
+_OptionalBatchParametersTypeDef = TypedDict(
+    "_OptionalBatchParametersTypeDef",
     {
-        "ArchiveArn": str,
-        "State": ArchiveStateType,
-        "StateReason": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ArrayProperties": BatchArrayPropertiesTypeDef,
+        "RetryStrategy": BatchRetryStrategyTypeDef,
     },
+    total=False,
 )
 
-UpdateConnectionResponseTypeDef = TypedDict(
-    "UpdateConnectionResponseTypeDef",
-    {
-        "ConnectionArn": str,
-        "ConnectionState": ConnectionStateType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LastAuthorizedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class BatchParametersTypeDef(_RequiredBatchParametersTypeDef, _OptionalBatchParametersTypeDef):
+    pass
 
 PutPermissionRequestRequestTypeDef = TypedDict(
     "PutPermissionRequestRequestTypeDef",
     {
         "EventBusName": str,
         "Action": str,
         "Principal": str,
@@ -1620,15 +1673,15 @@
 )
 
 ListConnectionsResponseTypeDef = TypedDict(
     "ListConnectionsResponseTypeDef",
     {
         "Connections": List[ConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEventBusRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventBusRequestRequestTypeDef",
     {
         "Name": str,
@@ -1648,15 +1701,15 @@
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutRuleRequestRequestTypeDef",
     {
         "Name": str,
@@ -1700,15 +1753,15 @@
         "EventSourceArn": str,
         "Destination": ReplayDestinationTypeDef,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
         "EventLastReplayedTime": datetime,
         "ReplayStartTime": datetime,
         "ReplayEndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartReplayRequestRequestTypeDef = TypedDict(
     "_RequiredStartReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
@@ -1732,24 +1785,24 @@
     pass
 
 ListEventBusesResponseTypeDef = TypedDict(
     "ListEventBusesResponseTypeDef",
     {
         "EventBuses": List[EventBusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventSourcesResponseTypeDef = TypedDict(
     "ListEventSourcesResponseTypeDef",
     {
         "EventSources": List[EventSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FailoverConfigTypeDef = TypedDict(
     "FailoverConfigTypeDef",
     {
         "Primary": PrimaryTypeDef,
@@ -1758,94 +1811,42 @@
 )
 
 ListPartnerEventSourceAccountsResponseTypeDef = TypedDict(
     "ListPartnerEventSourceAccountsResponseTypeDef",
     {
         "PartnerEventSourceAccounts": List[PartnerEventSourceAccountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPartnerEventSourcesResponseTypeDef = TypedDict(
     "ListPartnerEventSourcesResponseTypeDef",
     {
         "PartnerEventSources": List[PartnerEventSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListReplaysResponseTypeDef = TypedDict(
     "ListReplaysResponseTypeDef",
     {
         "Replays": List[ReplayTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
-    "_RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
-    {
-        "TargetArn": str,
-    },
-)
-_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
-    "_OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
-    {
-        "EventBusName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef(
-    _RequiredListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
-    _OptionalListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
-):
-    pass
-
-ListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "ListRulesRequestListRulesPaginateTypeDef",
-    {
-        "NamePrefix": str,
-        "EventBusName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
-    "_RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
-    {
-        "Rule": str,
-    },
-)
-_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef = TypedDict(
-    "_OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
-    {
-        "EventBusName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef(
-    _RequiredListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
-    _OptionalListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
-):
-    pass
-
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "Rules": List[RuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutEventsRequestRequestTypeDef = TypedDict(
     "_RequiredPutEventsRequestRequestTypeDef",
     {
         "Entries": Sequence[PutEventsRequestEntryTypeDef],
@@ -1865,15 +1866,15 @@
     pass
 
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "Entries": List[PutEventsResultEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutPartnerEventsRequestRequestTypeDef = TypedDict(
     "PutPartnerEventsRequestRequestTypeDef",
     {
         "Entries": Sequence[PutPartnerEventsRequestEntryTypeDef],
@@ -1881,33 +1882,33 @@
 )
 
 PutPartnerEventsResponseTypeDef = TypedDict(
     "PutPartnerEventsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "Entries": List[PutPartnerEventsResultEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutTargetsResponseTypeDef = TypedDict(
     "PutTargetsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "FailedEntries": List[PutTargetsResultEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RemoveTargetsResponseTypeDef = TypedDict(
     "RemoveTargetsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "FailedEntries": List[RemoveTargetsResultEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RunCommandParametersTypeDef = TypedDict(
     "RunCommandParametersTypeDef",
     {
         "RunCommandTargets": List[RunCommandTargetTypeDef],
@@ -2095,15 +2096,15 @@
         "Name": str,
         "Arn": str,
         "RoutingConfig": RoutingConfigTypeDef,
         "ReplicationConfig": ReplicationConfigTypeDef,
         "EventBuses": List[EndpointEventBusTypeDef],
         "RoleArn": str,
         "State": EndpointStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointResponseTypeDef = TypedDict(
     "DescribeEndpointResponseTypeDef",
     {
         "Name": str,
@@ -2115,15 +2116,15 @@
         "RoleArn": str,
         "EndpointId": str,
         "EndpointUrl": str,
         "State": EndpointStateType,
         "StateReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Name": str,
@@ -2174,24 +2175,24 @@
         "RoutingConfig": RoutingConfigTypeDef,
         "ReplicationConfig": ReplicationConfigTypeDef,
         "EventBuses": List[EndpointEventBusTypeDef],
         "RoleArn": str,
         "EndpointId": str,
         "EndpointUrl": str,
         "State": EndpointStateType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTargetsByRuleResponseTypeDef = TypedDict(
     "ListTargetsByRuleResponseTypeDef",
     {
         "Targets": List[TargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredPutTargetsRequestRequestTypeDef",
     {
         "Rule": str,
@@ -2221,15 +2222,15 @@
         "StateReason": str,
         "AuthorizationType": ConnectionAuthorizationTypeType,
         "SecretArn": str,
         "AuthParameters": ConnectionAuthResponseParametersTypeDef,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LastAuthorizedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionRequestRequestTypeDef",
     {
         "Name": str,
@@ -2272,10 +2273,10 @@
     pass
 
 ListEndpointsResponseTypeDef = TypedDict(
     "ListEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-events-1.26.58/mypy_boto3_events.egg-info/PKG-INFO` & `mypy-boto3-events-1.27.0/mypy_boto3_events.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-events
-Version: 1.26.58
-Summary: Type annotations for boto3.EventBridge 1.26.58 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.EventBridge 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-events"></a>
 
 # mypy-boto3-events
 
 [![PyPI - mypy-boto3-events](https://img.shields.io/pypi/v/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-events?color=blue)](https://pypistats.org/packages/mypy-boto3-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridge 1.26.58](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[boto3.EventBridge 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
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
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,56 +353,70 @@
     ActivateEventSourceRequestRequestTypeDef,
     ApiDestinationTypeDef,
     ArchiveTypeDef,
     AwsVpcConfigurationTypeDef,
     BatchArrayPropertiesTypeDef,
     BatchRetryStrategyTypeDef,
     CancelReplayRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CancelReplayResponseTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ConditionTypeDef,
     ConnectionApiKeyAuthResponseParametersTypeDef,
     ConnectionBasicAuthResponseParametersTypeDef,
     ConnectionBodyParameterTypeDef,
     ConnectionHeaderParameterTypeDef,
     ConnectionQueryStringParameterTypeDef,
     ConnectionOAuthClientResponseParametersTypeDef,
     ConnectionTypeDef,
     CreateApiDestinationRequestRequestTypeDef,
+    CreateApiDestinationResponseTypeDef,
     CreateArchiveRequestRequestTypeDef,
+    CreateArchiveResponseTypeDef,
     CreateConnectionApiKeyAuthRequestParametersTypeDef,
     CreateConnectionBasicAuthRequestParametersTypeDef,
     CreateConnectionOAuthClientRequestParametersTypeDef,
+    CreateConnectionResponseTypeDef,
     EndpointEventBusTypeDef,
     ReplicationConfigTypeDef,
     TagTypeDef,
+    CreateEventBusResponseTypeDef,
     CreatePartnerEventSourceRequestRequestTypeDef,
+    CreatePartnerEventSourceResponseTypeDef,
     DeactivateEventSourceRequestRequestTypeDef,
     DeadLetterConfigTypeDef,
     DeauthorizeConnectionRequestRequestTypeDef,
+    DeauthorizeConnectionResponseTypeDef,
     DeleteApiDestinationRequestRequestTypeDef,
     DeleteArchiveRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
+    DeleteConnectionResponseTypeDef,
     DeleteEndpointRequestRequestTypeDef,
     DeleteEventBusRequestRequestTypeDef,
     DeletePartnerEventSourceRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DescribeApiDestinationRequestRequestTypeDef,
+    DescribeApiDestinationResponseTypeDef,
     DescribeArchiveRequestRequestTypeDef,
+    DescribeArchiveResponseTypeDef,
     DescribeConnectionRequestRequestTypeDef,
     DescribeEndpointRequestRequestTypeDef,
     DescribeEventBusRequestRequestTypeDef,
+    DescribeEventBusResponseTypeDef,
     DescribeEventSourceRequestRequestTypeDef,
+    DescribeEventSourceResponseTypeDef,
     DescribePartnerEventSourceRequestRequestTypeDef,
+    DescribePartnerEventSourceResponseTypeDef,
     DescribeReplayRequestRequestTypeDef,
     ReplayDestinationTypeDef,
     DescribeRuleRequestRequestTypeDef,
+    DescribeRuleResponseTypeDef,
     DisableRuleRequestRequestTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableRuleRequestRequestTypeDef,
     EventBusTypeDef,
     EventSourceTypeDef,
     PrimaryTypeDef,
     SecondaryTypeDef,
     HttpParametersTypeDef,
     InputTransformerTypeDef,
@@ -415,66 +429,55 @@
     ListEventSourcesRequestRequestTypeDef,
     ListPartnerEventSourceAccountsRequestRequestTypeDef,
     PartnerEventSourceAccountTypeDef,
     ListPartnerEventSourcesRequestRequestTypeDef,
     PartnerEventSourceTypeDef,
     ListReplaysRequestRequestTypeDef,
     ReplayTypeDef,
-    PaginatorConfigTypeDef,
+    ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
     ListRuleNamesByTargetRequestRequestTypeDef,
+    ListRuleNamesByTargetResponseTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
     ListTargetsByRuleRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PutEventsRequestEntryTypeDef,
     PutEventsResultEntryTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResultEntryTypeDef,
+    PutRuleResponseTypeDef,
     PutTargetsResultEntryTypeDef,
     RedshiftDataParametersTypeDef,
     RemovePermissionRequestRequestTypeDef,
     RemoveTargetsRequestRequestTypeDef,
     RemoveTargetsResultEntryTypeDef,
+    ResponseMetadataTypeDef,
     RetryPolicyTypeDef,
     RunCommandTargetTypeDef,
     SageMakerPipelineParameterTypeDef,
     SqsParametersTypeDef,
+    StartReplayResponseTypeDef,
     TestEventPatternRequestRequestTypeDef,
+    TestEventPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiDestinationRequestRequestTypeDef,
+    UpdateApiDestinationResponseTypeDef,
     UpdateArchiveRequestRequestTypeDef,
+    UpdateArchiveResponseTypeDef,
     UpdateConnectionApiKeyAuthRequestParametersTypeDef,
     UpdateConnectionBasicAuthRequestParametersTypeDef,
     UpdateConnectionOAuthClientRequestParametersTypeDef,
-    NetworkConfigurationTypeDef,
-    BatchParametersTypeDef,
-    CancelReplayResponseTypeDef,
-    CreateApiDestinationResponseTypeDef,
-    CreateArchiveResponseTypeDef,
-    CreateConnectionResponseTypeDef,
-    CreateEventBusResponseTypeDef,
-    CreatePartnerEventSourceResponseTypeDef,
-    DeauthorizeConnectionResponseTypeDef,
-    DeleteConnectionResponseTypeDef,
-    DescribeApiDestinationResponseTypeDef,
-    DescribeArchiveResponseTypeDef,
-    DescribeEventBusResponseTypeDef,
-    DescribeEventSourceResponseTypeDef,
-    DescribePartnerEventSourceResponseTypeDef,
-    DescribeRuleResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
+    UpdateConnectionResponseTypeDef,
     ListApiDestinationsResponseTypeDef,
     ListArchivesResponseTypeDef,
-    ListRuleNamesByTargetResponseTypeDef,
-    PutRuleResponseTypeDef,
-    StartReplayResponseTypeDef,
-    TestEventPatternResponseTypeDef,
-    UpdateApiDestinationResponseTypeDef,
-    UpdateArchiveResponseTypeDef,
-    UpdateConnectionResponseTypeDef,
+    NetworkConfigurationTypeDef,
+    BatchParametersTypeDef,
     PutPermissionRequestRequestTypeDef,
     ConnectionHttpParametersTypeDef,
     ListConnectionsResponseTypeDef,
     CreateEventBusRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutRuleRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -482,17 +485,14 @@
     StartReplayRequestRequestTypeDef,
     ListEventBusesResponseTypeDef,
     ListEventSourcesResponseTypeDef,
     FailoverConfigTypeDef,
     ListPartnerEventSourceAccountsResponseTypeDef,
     ListPartnerEventSourcesResponseTypeDef,
     ListReplaysResponseTypeDef,
-    ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
-    ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
     ListRulesResponseTypeDef,
     PutEventsRequestRequestTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestRequestTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
@@ -529,42 +529,42 @@
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

### Comparing `mypy-boto3-events-1.26.58/mypy_boto3_events.egg-info/SOURCES.txt` & `mypy-boto3-events-1.27.0/mypy_boto3_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.26.58/setup.py` & `mypy-boto3-events-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-events.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-events",
-    version="1.26.58",
+    version="1.27.0",
     packages=["mypy_boto3_events"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EventBridge 1.26.58 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.EventBridge 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/",
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


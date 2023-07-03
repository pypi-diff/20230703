# Comparing `tmp/mypy-boto3-logs-1.26.53.tar.gz` & `tmp/mypy-boto3-logs-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-logs-1.26.53.tar", last modified: Thu Jan 19 22:27:41 2023, max compression
+gzip compressed data, was "mypy-boto3-logs-1.27.0.tar", last modified: Mon Jul  3 19:51:03 2023, max compression
```

## Comparing `mypy-boto3-logs-1.26.53.tar` & `mypy-boto3-logs-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:27:41.081137 mypy-boto3-logs-1.26.53/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-19 22:26:56.000000 mypy-boto3-logs-1.26.53/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-01-19 22:27:41.077136 mypy-boto3-logs-1.26.53/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17093 2023-01-19 22:26:56.000000 mypy-boto3-logs-1.26.53/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:27:41.073136 mypy-boto3-logs-1.26.53/mypy_boto3_logs/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-01-19 22:26:56.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-01-19 22:26:56.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-19 22:26:56.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36150 2023-01-19 22:26:56.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36086 2023-01-19 22:26:56.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-01-19 22:26:56.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-01-19 22:26:56.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-01-19 22:26:56.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11803 2023-01-19 22:26:56.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 22:26:56.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34106 2023-01-19 22:26:57.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34079 2023-01-19 22:26:57.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-19 22:26:56.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:27:41.077136 mypy-boto3-logs-1.26.53/mypy_boto3_logs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-01-19 22:27:40.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-01-19 22:27:40.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 22:27:40.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 22:27:40.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-19 22:27:40.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-19 22:27:40.000000 mypy-boto3-logs-1.26.53/mypy_boto3_logs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 22:27:41.081137 mypy-boto3-logs-1.26.53/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-01-19 22:26:56.000000 mypy-boto3-logs-1.26.53/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.523594 mypy-boto3-logs-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:16.000000 mypy-boto3-logs-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18843 2023-07-03 19:51:03.523594 mypy-boto3-logs-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17360 2023-07-03 19:41:16.000000 mypy-boto3-logs-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.511594 mypy-boto3-logs-1.27.0/mypy_boto3_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-03 19:41:16.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-03 19:41:16.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:41:16.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38072 2023-07-03 19:41:17.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38005 2023-07-03 19:41:16.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-03 19:41:17.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-07-03 19:41:17.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-07-03 19:41:17.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-07-03 19:41:17.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:16.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36719 2023-07-03 19:41:18.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36688 2023-07-03 19:41:17.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:16.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:03.523594 mypy-boto3-logs-1.27.0/mypy_boto3_logs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18843 2023-07-03 19:51:03.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-03 19:51:03.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:03.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:03.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 19:51:03.000000 mypy-boto3-logs-1.27.0/mypy_boto3_logs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:03.523594 mypy-boto3-logs-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:41:16.000000 mypy-boto3-logs-1.27.0/setup.py
```

### Comparing `mypy-boto3-logs-1.26.53/LICENSE` & `mypy-boto3-logs-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-logs-1.26.53/PKG-INFO` & `mypy-boto3-logs-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-logs
-Version: 1.26.53
-Summary: Type annotations for boto3.CloudWatchLogs 1.26.53 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudWatchLogs 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-logs"></a>
 
 # mypy-boto3-logs
 
 [![PyPI - mypy-boto3-logs](https://img.shields.io/pypi/v/mypy-boto3-logs.svg?color=blue)](https://pypi.org/project/mypy-boto3-logs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-logs.svg?color=blue)](https://pypi.org/project/mypy-boto3-logs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-logs?color=blue)](https://pypistats.org/packages/mypy-boto3-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchLogs 1.26.53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[boto3.CloudWatchLogs 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
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
 [mypy-boto3-logs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,16 +340,19 @@
     DescribeMetricFiltersPaginatorName,
     DescribeQueriesPaginatorName,
     DescribeResourcePoliciesPaginatorName,
     DescribeSubscriptionFiltersPaginatorName,
     DistributionType,
     ExportTaskStatusCodeType,
     FilterLogEventsPaginatorName,
+    InheritedPropertyType,
     OrderByType,
+    PolicyTypeType,
     QueryStatusType,
+    ScopeType,
     StandardUnitType,
     CloudWatchLogsServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -364,101 +367,107 @@
 ### Typed dictionaries
 
 `mypy_boto3_logs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_logs.type_defs import (
+    AccountPolicyTypeDef,
     AssociateKmsKeyRequestRequestTypeDef,
     CancelExportTaskRequestRequestTypeDef,
     CreateExportTaskRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateExportTaskResponseTypeDef,
     CreateLogGroupRequestRequestTypeDef,
     CreateLogStreamRequestRequestTypeDef,
+    DeleteAccountPolicyRequestRequestTypeDef,
     DeleteDataProtectionPolicyRequestRequestTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteLogGroupRequestRequestTypeDef,
     DeleteLogStreamRequestRequestTypeDef,
     DeleteMetricFilterRequestRequestTypeDef,
     DeleteQueryDefinitionRequestRequestTypeDef,
+    DeleteQueryDefinitionResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRetentionPolicyRequestRequestTypeDef,
     DeleteSubscriptionFilterRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAccountPoliciesRequestRequestTypeDef,
+    DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef,
     DescribeDestinationsRequestRequestTypeDef,
     DestinationTypeDef,
+    DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
     DescribeExportTasksRequestRequestTypeDef,
+    DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef,
     DescribeLogGroupsRequestRequestTypeDef,
     LogGroupTypeDef,
+    DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef,
     DescribeLogStreamsRequestRequestTypeDef,
     LogStreamTypeDef,
+    DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef,
     DescribeMetricFiltersRequestRequestTypeDef,
+    DescribeQueriesRequestDescribeQueriesPaginateTypeDef,
     DescribeQueriesRequestRequestTypeDef,
     QueryInfoTypeDef,
     DescribeQueryDefinitionsRequestRequestTypeDef,
     QueryDefinitionTypeDef,
+    DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef,
     DescribeResourcePoliciesRequestRequestTypeDef,
     ResourcePolicyTypeDef,
+    DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
     DescribeSubscriptionFiltersRequestRequestTypeDef,
     SubscriptionFilterTypeDef,
     DisassociateKmsKeyRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportTaskExecutionInfoTypeDef,
     ExportTaskStatusTypeDef,
+    FilterLogEventsRequestFilterLogEventsPaginateTypeDef,
     FilterLogEventsRequestRequestTypeDef,
     FilteredLogEventTypeDef,
     SearchedLogStreamTypeDef,
     GetDataProtectionPolicyRequestRequestTypeDef,
+    GetDataProtectionPolicyResponseTypeDef,
     GetLogEventsRequestRequestTypeDef,
     OutputLogEventTypeDef,
     GetLogGroupFieldsRequestRequestTypeDef,
     LogGroupFieldTypeDef,
     GetLogRecordRequestRequestTypeDef,
+    GetLogRecordResponseTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     ResultFieldTypeDef,
     InputLogEventTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTagsLogGroupRequestRequestTypeDef,
+    ListTagsLogGroupResponseTypeDef,
     MetricFilterMatchRecordTypeDef,
     MetricTransformationTypeDef,
+    PaginatorConfigTypeDef,
+    PutAccountPolicyRequestRequestTypeDef,
     PutDataProtectionPolicyRequestRequestTypeDef,
+    PutDataProtectionPolicyResponseTypeDef,
     PutDestinationPolicyRequestRequestTypeDef,
     PutDestinationRequestRequestTypeDef,
     RejectedLogEventsInfoTypeDef,
     PutQueryDefinitionRequestRequestTypeDef,
+    PutQueryDefinitionResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutRetentionPolicyRequestRequestTypeDef,
     PutSubscriptionFilterRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     StartQueryRequestRequestTypeDef,
+    StartQueryResponseTypeDef,
     StopQueryRequestRequestTypeDef,
+    StopQueryResponseTypeDef,
     TagLogGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestMetricFilterRequestRequestTypeDef,
     UntagLogGroupRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateExportTaskResponseTypeDef,
-    DeleteQueryDefinitionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDataProtectionPolicyResponseTypeDef,
-    GetLogRecordResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTagsLogGroupResponseTypeDef,
-    PutDataProtectionPolicyResponseTypeDef,
-    PutQueryDefinitionResponseTypeDef,
-    StartQueryResponseTypeDef,
-    StopQueryResponseTypeDef,
-    DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef,
-    DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
-    DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef,
-    DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef,
-    DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef,
-    DescribeQueriesRequestDescribeQueriesPaginateTypeDef,
-    DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef,
-    DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
-    FilterLogEventsRequestFilterLogEventsPaginateTypeDef,
+    DescribeAccountPoliciesResponseTypeDef,
+    PutAccountPolicyResponseTypeDef,
     DescribeDestinationsResponseTypeDef,
     PutDestinationResponseTypeDef,
     DescribeLogGroupsResponseTypeDef,
     DescribeLogStreamsResponseTypeDef,
     DescribeQueriesResponseTypeDef,
     DescribeQueryDefinitionsResponseTypeDef,
     DescribeResourcePoliciesResponseTypeDef,
@@ -475,53 +484,53 @@
     PutMetricFilterRequestRequestTypeDef,
     PutLogEventsResponseTypeDef,
     DescribeExportTasksResponseTypeDef,
     DescribeMetricFiltersResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateKmsKeyRequestRequestTypeDef:
+def get_structure() -> AccountPolicyTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-logs-1.26.53/README.md` & `mypy-boto3-logs-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-logs"></a>
 
 # mypy-boto3-logs
 
 [![PyPI - mypy-boto3-logs](https://img.shields.io/pypi/v/mypy-boto3-logs.svg?color=blue)](https://pypi.org/project/mypy-boto3-logs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-logs.svg?color=blue)](https://pypi.org/project/mypy-boto3-logs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-logs?color=blue)](https://pypistats.org/packages/mypy-boto3-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchLogs 1.26.53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[boto3.CloudWatchLogs 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
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
 [mypy-boto3-logs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -308,16 +308,19 @@
     DescribeMetricFiltersPaginatorName,
     DescribeQueriesPaginatorName,
     DescribeResourcePoliciesPaginatorName,
     DescribeSubscriptionFiltersPaginatorName,
     DistributionType,
     ExportTaskStatusCodeType,
     FilterLogEventsPaginatorName,
+    InheritedPropertyType,
     OrderByType,
+    PolicyTypeType,
     QueryStatusType,
+    ScopeType,
     StandardUnitType,
     CloudWatchLogsServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -332,101 +335,107 @@
 ### Typed dictionaries
 
 `mypy_boto3_logs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_logs.type_defs import (
+    AccountPolicyTypeDef,
     AssociateKmsKeyRequestRequestTypeDef,
     CancelExportTaskRequestRequestTypeDef,
     CreateExportTaskRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateExportTaskResponseTypeDef,
     CreateLogGroupRequestRequestTypeDef,
     CreateLogStreamRequestRequestTypeDef,
+    DeleteAccountPolicyRequestRequestTypeDef,
     DeleteDataProtectionPolicyRequestRequestTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteLogGroupRequestRequestTypeDef,
     DeleteLogStreamRequestRequestTypeDef,
     DeleteMetricFilterRequestRequestTypeDef,
     DeleteQueryDefinitionRequestRequestTypeDef,
+    DeleteQueryDefinitionResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRetentionPolicyRequestRequestTypeDef,
     DeleteSubscriptionFilterRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAccountPoliciesRequestRequestTypeDef,
+    DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef,
     DescribeDestinationsRequestRequestTypeDef,
     DestinationTypeDef,
+    DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
     DescribeExportTasksRequestRequestTypeDef,
+    DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef,
     DescribeLogGroupsRequestRequestTypeDef,
     LogGroupTypeDef,
+    DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef,
     DescribeLogStreamsRequestRequestTypeDef,
     LogStreamTypeDef,
+    DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef,
     DescribeMetricFiltersRequestRequestTypeDef,
+    DescribeQueriesRequestDescribeQueriesPaginateTypeDef,
     DescribeQueriesRequestRequestTypeDef,
     QueryInfoTypeDef,
     DescribeQueryDefinitionsRequestRequestTypeDef,
     QueryDefinitionTypeDef,
+    DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef,
     DescribeResourcePoliciesRequestRequestTypeDef,
     ResourcePolicyTypeDef,
+    DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
     DescribeSubscriptionFiltersRequestRequestTypeDef,
     SubscriptionFilterTypeDef,
     DisassociateKmsKeyRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportTaskExecutionInfoTypeDef,
     ExportTaskStatusTypeDef,
+    FilterLogEventsRequestFilterLogEventsPaginateTypeDef,
     FilterLogEventsRequestRequestTypeDef,
     FilteredLogEventTypeDef,
     SearchedLogStreamTypeDef,
     GetDataProtectionPolicyRequestRequestTypeDef,
+    GetDataProtectionPolicyResponseTypeDef,
     GetLogEventsRequestRequestTypeDef,
     OutputLogEventTypeDef,
     GetLogGroupFieldsRequestRequestTypeDef,
     LogGroupFieldTypeDef,
     GetLogRecordRequestRequestTypeDef,
+    GetLogRecordResponseTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     ResultFieldTypeDef,
     InputLogEventTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTagsLogGroupRequestRequestTypeDef,
+    ListTagsLogGroupResponseTypeDef,
     MetricFilterMatchRecordTypeDef,
     MetricTransformationTypeDef,
+    PaginatorConfigTypeDef,
+    PutAccountPolicyRequestRequestTypeDef,
     PutDataProtectionPolicyRequestRequestTypeDef,
+    PutDataProtectionPolicyResponseTypeDef,
     PutDestinationPolicyRequestRequestTypeDef,
     PutDestinationRequestRequestTypeDef,
     RejectedLogEventsInfoTypeDef,
     PutQueryDefinitionRequestRequestTypeDef,
+    PutQueryDefinitionResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutRetentionPolicyRequestRequestTypeDef,
     PutSubscriptionFilterRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     StartQueryRequestRequestTypeDef,
+    StartQueryResponseTypeDef,
     StopQueryRequestRequestTypeDef,
+    StopQueryResponseTypeDef,
     TagLogGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestMetricFilterRequestRequestTypeDef,
     UntagLogGroupRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateExportTaskResponseTypeDef,
-    DeleteQueryDefinitionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDataProtectionPolicyResponseTypeDef,
-    GetLogRecordResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTagsLogGroupResponseTypeDef,
-    PutDataProtectionPolicyResponseTypeDef,
-    PutQueryDefinitionResponseTypeDef,
-    StartQueryResponseTypeDef,
-    StopQueryResponseTypeDef,
-    DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef,
-    DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
-    DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef,
-    DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef,
-    DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef,
-    DescribeQueriesRequestDescribeQueriesPaginateTypeDef,
-    DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef,
-    DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
-    FilterLogEventsRequestFilterLogEventsPaginateTypeDef,
+    DescribeAccountPoliciesResponseTypeDef,
+    PutAccountPolicyResponseTypeDef,
     DescribeDestinationsResponseTypeDef,
     PutDestinationResponseTypeDef,
     DescribeLogGroupsResponseTypeDef,
     DescribeLogStreamsResponseTypeDef,
     DescribeQueriesResponseTypeDef,
     DescribeQueryDefinitionsResponseTypeDef,
     DescribeResourcePoliciesResponseTypeDef,
@@ -443,53 +452,53 @@
     PutMetricFilterRequestRequestTypeDef,
     PutLogEventsResponseTypeDef,
     DescribeExportTasksResponseTypeDef,
     DescribeMetricFiltersResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateKmsKeyRequestRequestTypeDef:
+def get_structure() -> AccountPolicyTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-logs-1.26.53/mypy_boto3_logs/__init__.py` & `mypy-boto3-logs-1.27.0/mypy_boto3_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.26.53/mypy_boto3_logs/__init__.pyi` & `mypy-boto3-logs-1.27.0/mypy_boto3_logs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.26.53/mypy_boto3_logs/__main__.py` & `mypy-boto3-logs-1.27.0/mypy_boto3_logs/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchLogs 1.26.53\nVersion:         1.26.53\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.CloudWatchLogs 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.53")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-logs-1.26.53/mypy_boto3_logs/client.py` & `mypy-boto3-logs-1.27.0/mypy_boto3_logs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     DescribeResourcePoliciesPaginator,
     DescribeSubscriptionFiltersPaginator,
     FilterLogEventsPaginator,
 )
 from .type_defs import (
     CreateExportTaskResponseTypeDef,
     DeleteQueryDefinitionResponseTypeDef,
+    DescribeAccountPoliciesResponseTypeDef,
     DescribeDestinationsResponseTypeDef,
     DescribeExportTasksResponseTypeDef,
     DescribeLogGroupsResponseTypeDef,
     DescribeLogStreamsResponseTypeDef,
     DescribeMetricFiltersResponseTypeDef,
     DescribeQueriesResponseTypeDef,
     DescribeQueryDefinitionsResponseTypeDef,
@@ -49,14 +50,15 @@
     GetLogGroupFieldsResponseTypeDef,
     GetLogRecordResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     InputLogEventTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTagsLogGroupResponseTypeDef,
     MetricTransformationTypeDef,
+    PutAccountPolicyResponseTypeDef,
     PutDataProtectionPolicyResponseTypeDef,
     PutDestinationResponseTypeDef,
     PutLogEventsResponseTypeDef,
     PutQueryDefinitionResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     StartQueryResponseTypeDef,
     StopQueryResponseTypeDef,
@@ -182,14 +184,24 @@
         """
         Creates a log stream for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_log_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#create_log_stream)
         """
 
+    def delete_account_policy(
+        self, *, policyName: str, policyType: Literal["DATA_PROTECTION_POLICY"]
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes a CloudWatch Logs account policy.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_account_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#delete_account_policy)
+        """
+
     def delete_data_protection_policy(
         self, *, logGroupIdentifier: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the data protection policy from the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_data_protection_policy)
@@ -267,14 +279,28 @@
         """
         Deletes the specified subscription filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_subscription_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#delete_subscription_filter)
         """
 
+    def describe_account_policies(
+        self,
+        *,
+        policyType: Literal["DATA_PROTECTION_POLICY"],
+        policyName: str = ...,
+        accountIdentifiers: Sequence[str] = ...
+    ) -> DescribeAccountPoliciesResponseTypeDef:
+        """
+        Returns a list of all CloudWatch Logs account policies in the account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_account_policies)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#describe_account_policies)
+        """
+
     def describe_destinations(
         self, *, DestinationNamePrefix: str = ..., nextToken: str = ..., limit: int = ...
     ) -> DescribeDestinationsResponseTypeDef:
         """
         Lists all your destinations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_destinations)
@@ -515,14 +541,30 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.list_tags_log_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#list_tags_log_group)
         """
 
+    def put_account_policy(
+        self,
+        *,
+        policyName: str,
+        policyDocument: str,
+        policyType: Literal["DATA_PROTECTION_POLICY"],
+        scope: Literal["ALL"] = ...
+    ) -> PutAccountPolicyResponseTypeDef:
+        """
+        Creates an account-level data protection policy that applies to all log groups
+        in the account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_account_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#put_account_policy)
+        """
+
     def put_data_protection_policy(
         self, *, logGroupIdentifier: str, policyDocument: str
     ) -> PutDataProtectionPolicyResponseTypeDef:
         """
         Creates a data protection policy for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_data_protection_policy)
```

### Comparing `mypy-boto3-logs-1.26.53/mypy_boto3_logs/client.pyi` & `mypy-boto3-logs-1.27.0/mypy_boto3_logs/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     DescribeResourcePoliciesPaginator,
     DescribeSubscriptionFiltersPaginator,
     FilterLogEventsPaginator,
 )
 from .type_defs import (
     CreateExportTaskResponseTypeDef,
     DeleteQueryDefinitionResponseTypeDef,
+    DescribeAccountPoliciesResponseTypeDef,
     DescribeDestinationsResponseTypeDef,
     DescribeExportTasksResponseTypeDef,
     DescribeLogGroupsResponseTypeDef,
     DescribeLogStreamsResponseTypeDef,
     DescribeMetricFiltersResponseTypeDef,
     DescribeQueriesResponseTypeDef,
     DescribeQueryDefinitionsResponseTypeDef,
@@ -49,14 +50,15 @@
     GetLogGroupFieldsResponseTypeDef,
     GetLogRecordResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     InputLogEventTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTagsLogGroupResponseTypeDef,
     MetricTransformationTypeDef,
+    PutAccountPolicyResponseTypeDef,
     PutDataProtectionPolicyResponseTypeDef,
     PutDestinationResponseTypeDef,
     PutLogEventsResponseTypeDef,
     PutQueryDefinitionResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     StartQueryResponseTypeDef,
     StopQueryResponseTypeDef,
@@ -170,14 +172,23 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a log stream for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_log_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#create_log_stream)
         """
+    def delete_account_policy(
+        self, *, policyName: str, policyType: Literal["DATA_PROTECTION_POLICY"]
+    ) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes a CloudWatch Logs account policy.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_account_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#delete_account_policy)
+        """
     def delete_data_protection_policy(
         self, *, logGroupIdentifier: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the data protection policy from the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_data_protection_policy)
@@ -246,14 +257,27 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified subscription filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.delete_subscription_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#delete_subscription_filter)
         """
+    def describe_account_policies(
+        self,
+        *,
+        policyType: Literal["DATA_PROTECTION_POLICY"],
+        policyName: str = ...,
+        accountIdentifiers: Sequence[str] = ...
+    ) -> DescribeAccountPoliciesResponseTypeDef:
+        """
+        Returns a list of all CloudWatch Logs account policies in the account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_account_policies)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#describe_account_policies)
+        """
     def describe_destinations(
         self, *, DestinationNamePrefix: str = ..., nextToken: str = ..., limit: int = ...
     ) -> DescribeDestinationsResponseTypeDef:
         """
         Lists all your destinations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_destinations)
@@ -475,14 +499,29 @@
     def list_tags_log_group(self, *, logGroupName: str) -> ListTagsLogGroupResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.list_tags_log_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#list_tags_log_group)
         """
+    def put_account_policy(
+        self,
+        *,
+        policyName: str,
+        policyDocument: str,
+        policyType: Literal["DATA_PROTECTION_POLICY"],
+        scope: Literal["ALL"] = ...
+    ) -> PutAccountPolicyResponseTypeDef:
+        """
+        Creates an account-level data protection policy that applies to all log groups
+        in the account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_account_policy)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/client/#put_account_policy)
+        """
     def put_data_protection_policy(
         self, *, logGroupIdentifier: str, policyDocument: str
     ) -> PutDataProtectionPolicyResponseTypeDef:
         """
         Creates a data protection policy for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_data_protection_policy)
```

### Comparing `mypy-boto3-logs-1.26.53/mypy_boto3_logs/literals.py` & `mypy-boto3-logs-1.27.0/mypy_boto3_logs/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,57 +14,61 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DataProtectionStatusType",
     "DescribeDestinationsPaginatorName",
     "DescribeExportTasksPaginatorName",
     "DescribeLogGroupsPaginatorName",
     "DescribeLogStreamsPaginatorName",
     "DescribeMetricFiltersPaginatorName",
     "DescribeQueriesPaginatorName",
     "DescribeResourcePoliciesPaginatorName",
     "DescribeSubscriptionFiltersPaginatorName",
     "DistributionType",
     "ExportTaskStatusCodeType",
     "FilterLogEventsPaginatorName",
+    "InheritedPropertyType",
     "OrderByType",
+    "PolicyTypeType",
     "QueryStatusType",
+    "ScopeType",
     "StandardUnitType",
     "CloudWatchLogsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DataProtectionStatusType = Literal["ACTIVATED", "ARCHIVED", "DELETED", "DISABLED"]
 DescribeDestinationsPaginatorName = Literal["describe_destinations"]
 DescribeExportTasksPaginatorName = Literal["describe_export_tasks"]
 DescribeLogGroupsPaginatorName = Literal["describe_log_groups"]
 DescribeLogStreamsPaginatorName = Literal["describe_log_streams"]
 DescribeMetricFiltersPaginatorName = Literal["describe_metric_filters"]
 DescribeQueriesPaginatorName = Literal["describe_queries"]
 DescribeResourcePoliciesPaginatorName = Literal["describe_resource_policies"]
 DescribeSubscriptionFiltersPaginatorName = Literal["describe_subscription_filters"]
 DistributionType = Literal["ByLogStream", "Random"]
 ExportTaskStatusCodeType = Literal[
     "CANCELLED", "COMPLETED", "FAILED", "PENDING", "PENDING_CANCEL", "RUNNING"
 ]
 FilterLogEventsPaginatorName = Literal["filter_log_events"]
+InheritedPropertyType = Literal["ACCOUNT_DATA_PROTECTION"]
 OrderByType = Literal["LastEventTime", "LogStreamName"]
+PolicyTypeType = Literal["DATA_PROTECTION_POLICY"]
 QueryStatusType = Literal[
     "Cancelled", "Complete", "Failed", "Running", "Scheduled", "Timeout", "Unknown"
 ]
+ScopeType = Literal["ALL"]
 StandardUnitType = Literal[
     "Bits",
     "Bits/Second",
     "Bytes",
     "Bytes/Second",
     "Count",
     "Count/Second",
@@ -102,14 +106,15 @@
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
@@ -141,21 +146,23 @@
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
@@ -234,14 +241,15 @@
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
@@ -252,14 +260,15 @@
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
@@ -295,14 +304,15 @@
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
@@ -321,16 +331,19 @@
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
@@ -410,18 +423,21 @@
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
@@ -461,14 +477,15 @@
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

### Comparing `mypy-boto3-logs-1.26.53/mypy_boto3_logs/literals.pyi` & `mypy-boto3-logs-1.27.0/mypy_boto3_logs/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,55 +14,63 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DataProtectionStatusType",
     "DescribeDestinationsPaginatorName",
     "DescribeExportTasksPaginatorName",
     "DescribeLogGroupsPaginatorName",
     "DescribeLogStreamsPaginatorName",
     "DescribeMetricFiltersPaginatorName",
     "DescribeQueriesPaginatorName",
     "DescribeResourcePoliciesPaginatorName",
     "DescribeSubscriptionFiltersPaginatorName",
     "DistributionType",
     "ExportTaskStatusCodeType",
     "FilterLogEventsPaginatorName",
+    "InheritedPropertyType",
     "OrderByType",
+    "PolicyTypeType",
     "QueryStatusType",
+    "ScopeType",
     "StandardUnitType",
     "CloudWatchLogsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DataProtectionStatusType = Literal["ACTIVATED", "ARCHIVED", "DELETED", "DISABLED"]
 DescribeDestinationsPaginatorName = Literal["describe_destinations"]
 DescribeExportTasksPaginatorName = Literal["describe_export_tasks"]
 DescribeLogGroupsPaginatorName = Literal["describe_log_groups"]
 DescribeLogStreamsPaginatorName = Literal["describe_log_streams"]
 DescribeMetricFiltersPaginatorName = Literal["describe_metric_filters"]
 DescribeQueriesPaginatorName = Literal["describe_queries"]
 DescribeResourcePoliciesPaginatorName = Literal["describe_resource_policies"]
 DescribeSubscriptionFiltersPaginatorName = Literal["describe_subscription_filters"]
 DistributionType = Literal["ByLogStream", "Random"]
 ExportTaskStatusCodeType = Literal[
     "CANCELLED", "COMPLETED", "FAILED", "PENDING", "PENDING_CANCEL", "RUNNING"
 ]
 FilterLogEventsPaginatorName = Literal["filter_log_events"]
+InheritedPropertyType = Literal["ACCOUNT_DATA_PROTECTION"]
 OrderByType = Literal["LastEventTime", "LogStreamName"]
+PolicyTypeType = Literal["DATA_PROTECTION_POLICY"]
 QueryStatusType = Literal[
     "Cancelled", "Complete", "Failed", "Running", "Scheduled", "Timeout", "Unknown"
 ]
+ScopeType = Literal["ALL"]
 StandardUnitType = Literal[
     "Bits",
     "Bits/Second",
     "Bytes",
     "Bytes/Second",
     "Count",
     "Count/Second",
@@ -100,14 +108,15 @@
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
@@ -139,21 +148,23 @@
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
@@ -232,14 +243,15 @@
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
@@ -250,14 +262,15 @@
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
@@ -293,14 +306,15 @@
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
@@ -319,16 +333,19 @@
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
@@ -408,18 +425,21 @@
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
@@ -459,14 +479,15 @@
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

### Comparing `mypy-boto3-logs-1.26.53/mypy_boto3_logs/paginator.py` & `mypy-boto3-logs-1.27.0/mypy_boto3_logs/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,176 +61,165 @@
     "DescribeMetricFiltersPaginator",
     "DescribeQueriesPaginator",
     "DescribeResourcePoliciesPaginator",
     "DescribeSubscriptionFiltersPaginator",
     "FilterLogEventsPaginator",
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
 class DescribeDestinationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeDestinations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describedestinationspaginator)
     """
 
     def paginate(
-        self, *, DestinationNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DestinationNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describedestinationspaginator)
         """
 
-
 class DescribeExportTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeExportTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeexporttaskspaginator)
     """
 
     def paginate(
         self,
         *,
         taskId: str = ...,
         statusCode: ExportTaskStatusCodeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeExportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeExportTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeexporttaskspaginator)
         """
 
-
 class DescribeLogGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeloggroupspaginator)
     """
 
     def paginate(
         self,
         *,
         accountIdentifiers: Sequence[str] = ...,
         logGroupNamePrefix: str = ...,
         logGroupNamePattern: str = ...,
         includeLinkedAccounts: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLogGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeloggroupspaginator)
         """
 
-
 class DescribeLogStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describelogstreamspaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         logStreamNamePrefix: str = ...,
         orderBy: OrderByType = ...,
         descending: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLogStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describelogstreamspaginator)
         """
 
-
 class DescribeMetricFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeMetricFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describemetricfilterspaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         filterNamePrefix: str = ...,
         metricName: str = ...,
         metricNamespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMetricFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeMetricFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describemetricfilterspaginator)
         """
 
-
 class DescribeQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describequeriespaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         status: QueryStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeQueriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describequeriespaginator)
         """
 
-
 class DescribeResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeresourcepoliciespaginator)
         """
 
-
 class DescribeSubscriptionFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeSubscriptionFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describesubscriptionfilterspaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str,
         filterNamePrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSubscriptionFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeSubscriptionFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describesubscriptionfilterspaginator)
         """
 
-
 class FilterLogEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.FilterLogEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#filterlogeventspaginator)
     """
 
     def paginate(
@@ -241,13 +230,13 @@
         logStreamNames: Sequence[str] = ...,
         logStreamNamePrefix: str = ...,
         startTime: int = ...,
         endTime: int = ...,
         filterPattern: str = ...,
         interleaved: bool = ...,
         unmask: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[FilterLogEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.FilterLogEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#filterlogeventspaginator)
         """
```

### Comparing `mypy-boto3-logs-1.26.53/mypy_boto3_logs/paginator.pyi` & `mypy-boto3-logs-1.27.0/mypy_boto3_logs/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,165 +61,176 @@
     "DescribeMetricFiltersPaginator",
     "DescribeQueriesPaginator",
     "DescribeResourcePoliciesPaginator",
     "DescribeSubscriptionFiltersPaginator",
     "FilterLogEventsPaginator",
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
 class DescribeDestinationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeDestinations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describedestinationspaginator)
     """
 
     def paginate(
-        self, *, DestinationNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DestinationNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describedestinationspaginator)
         """
 
+
 class DescribeExportTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeExportTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeexporttaskspaginator)
     """
 
     def paginate(
         self,
         *,
         taskId: str = ...,
         statusCode: ExportTaskStatusCodeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeExportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeExportTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeexporttaskspaginator)
         """
 
+
 class DescribeLogGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeloggroupspaginator)
     """
 
     def paginate(
         self,
         *,
         accountIdentifiers: Sequence[str] = ...,
         logGroupNamePrefix: str = ...,
         logGroupNamePattern: str = ...,
         includeLinkedAccounts: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLogGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeloggroupspaginator)
         """
 
+
 class DescribeLogStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describelogstreamspaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         logStreamNamePrefix: str = ...,
         orderBy: OrderByType = ...,
         descending: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeLogStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describelogstreamspaginator)
         """
 
+
 class DescribeMetricFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeMetricFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describemetricfilterspaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         filterNamePrefix: str = ...,
         metricName: str = ...,
         metricNamespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeMetricFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeMetricFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describemetricfilterspaginator)
         """
 
+
 class DescribeQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describequeriespaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         status: QueryStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeQueriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describequeriespaginator)
         """
 
+
 class DescribeResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describeresourcepoliciespaginator)
         """
 
+
 class DescribeSubscriptionFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeSubscriptionFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describesubscriptionfilterspaginator)
     """
 
     def paginate(
         self,
         *,
         logGroupName: str,
         filterNamePrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSubscriptionFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeSubscriptionFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#describesubscriptionfilterspaginator)
         """
 
+
 class FilterLogEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.FilterLogEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#filterlogeventspaginator)
     """
 
     def paginate(
@@ -230,13 +241,13 @@
         logStreamNames: Sequence[str] = ...,
         logStreamNamePrefix: str = ...,
         startTime: int = ...,
         endTime: int = ...,
         filterPattern: str = ...,
         interleaved: bool = ...,
         unmask: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[FilterLogEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.FilterLogEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/paginators/#filterlogeventspaginator)
         """
```

### Comparing `mypy-boto3-logs-1.26.53/mypy_boto3_logs/type_defs.py` & `mypy-boto3-logs-1.27.0/mypy_boto3_logs/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for logs service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_logs.type_defs import AssociateKmsKeyRequestRequestTypeDef
+    from mypy_boto3_logs.type_defs import AccountPolicyTypeDef
 
-    data: AssociateKmsKeyRequestRequestTypeDef = {...}
+    data: AccountPolicyTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     DataProtectionStatusType,
@@ -20,107 +20,117 @@
     ExportTaskStatusCodeType,
     OrderByType,
     QueryStatusType,
     StandardUnitType,
 )
 
 if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AccountPolicyTypeDef",
     "AssociateKmsKeyRequestRequestTypeDef",
     "CancelExportTaskRequestRequestTypeDef",
     "CreateExportTaskRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateExportTaskResponseTypeDef",
     "CreateLogGroupRequestRequestTypeDef",
     "CreateLogStreamRequestRequestTypeDef",
+    "DeleteAccountPolicyRequestRequestTypeDef",
     "DeleteDataProtectionPolicyRequestRequestTypeDef",
     "DeleteDestinationRequestRequestTypeDef",
     "DeleteLogGroupRequestRequestTypeDef",
     "DeleteLogStreamRequestRequestTypeDef",
     "DeleteMetricFilterRequestRequestTypeDef",
     "DeleteQueryDefinitionRequestRequestTypeDef",
+    "DeleteQueryDefinitionResponseTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRetentionPolicyRequestRequestTypeDef",
     "DeleteSubscriptionFilterRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAccountPoliciesRequestRequestTypeDef",
+    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
     "DescribeDestinationsRequestRequestTypeDef",
     "DestinationTypeDef",
+    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
     "DescribeExportTasksRequestRequestTypeDef",
+    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
     "DescribeLogGroupsRequestRequestTypeDef",
     "LogGroupTypeDef",
+    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
     "DescribeLogStreamsRequestRequestTypeDef",
     "LogStreamTypeDef",
+    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
     "DescribeMetricFiltersRequestRequestTypeDef",
+    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
     "DescribeQueriesRequestRequestTypeDef",
     "QueryInfoTypeDef",
     "DescribeQueryDefinitionsRequestRequestTypeDef",
     "QueryDefinitionTypeDef",
+    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
     "DescribeResourcePoliciesRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
+    "DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
     "DescribeSubscriptionFiltersRequestRequestTypeDef",
     "SubscriptionFilterTypeDef",
     "DisassociateKmsKeyRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportTaskExecutionInfoTypeDef",
     "ExportTaskStatusTypeDef",
+    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
     "FilterLogEventsRequestRequestTypeDef",
     "FilteredLogEventTypeDef",
     "SearchedLogStreamTypeDef",
     "GetDataProtectionPolicyRequestRequestTypeDef",
+    "GetDataProtectionPolicyResponseTypeDef",
     "GetLogEventsRequestRequestTypeDef",
     "OutputLogEventTypeDef",
     "GetLogGroupFieldsRequestRequestTypeDef",
     "LogGroupFieldTypeDef",
     "GetLogRecordRequestRequestTypeDef",
+    "GetLogRecordResponseTypeDef",
     "GetQueryResultsRequestRequestTypeDef",
     "QueryStatisticsTypeDef",
     "ResultFieldTypeDef",
     "InputLogEventTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTagsLogGroupRequestRequestTypeDef",
+    "ListTagsLogGroupResponseTypeDef",
     "MetricFilterMatchRecordTypeDef",
     "MetricTransformationTypeDef",
+    "PaginatorConfigTypeDef",
+    "PutAccountPolicyRequestRequestTypeDef",
     "PutDataProtectionPolicyRequestRequestTypeDef",
+    "PutDataProtectionPolicyResponseTypeDef",
     "PutDestinationPolicyRequestRequestTypeDef",
     "PutDestinationRequestRequestTypeDef",
     "RejectedLogEventsInfoTypeDef",
     "PutQueryDefinitionRequestRequestTypeDef",
+    "PutQueryDefinitionResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutRetentionPolicyRequestRequestTypeDef",
     "PutSubscriptionFilterRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "StartQueryRequestRequestTypeDef",
+    "StartQueryResponseTypeDef",
     "StopQueryRequestRequestTypeDef",
+    "StopQueryResponseTypeDef",
     "TagLogGroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestMetricFilterRequestRequestTypeDef",
     "UntagLogGroupRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "CreateExportTaskResponseTypeDef",
-    "DeleteQueryDefinitionResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetDataProtectionPolicyResponseTypeDef",
-    "GetLogRecordResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTagsLogGroupResponseTypeDef",
-    "PutDataProtectionPolicyResponseTypeDef",
-    "PutQueryDefinitionResponseTypeDef",
-    "StartQueryResponseTypeDef",
-    "StopQueryResponseTypeDef",
-    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
-    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
-    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
-    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
-    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
-    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
-    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
-    "DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
-    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
+    "DescribeAccountPoliciesResponseTypeDef",
+    "PutAccountPolicyResponseTypeDef",
     "DescribeDestinationsResponseTypeDef",
     "PutDestinationResponseTypeDef",
     "DescribeLogGroupsResponseTypeDef",
     "DescribeLogStreamsResponseTypeDef",
     "DescribeQueriesResponseTypeDef",
     "DescribeQueryDefinitionsResponseTypeDef",
     "DescribeResourcePoliciesResponseTypeDef",
@@ -136,14 +146,27 @@
     "MetricFilterTypeDef",
     "PutMetricFilterRequestRequestTypeDef",
     "PutLogEventsResponseTypeDef",
     "DescribeExportTasksResponseTypeDef",
     "DescribeMetricFiltersResponseTypeDef",
 )
 
+AccountPolicyTypeDef = TypedDict(
+    "AccountPolicyTypeDef",
+    {
+        "policyName": str,
+        "policyDocument": str,
+        "lastUpdatedTime": int,
+        "policyType": Literal["DATA_PROTECTION_POLICY"],
+        "scope": Literal["ALL"],
+        "accountId": str,
+    },
+    total=False,
+)
+
 AssociateKmsKeyRequestRequestTypeDef = TypedDict(
     "AssociateKmsKeyRequestRequestTypeDef",
     {
         "logGroupName": str,
         "kmsKeyId": str,
     },
 )
@@ -177,22 +200,19 @@
 
 class CreateExportTaskRequestRequestTypeDef(
     _RequiredCreateExportTaskRequestRequestTypeDef, _OptionalCreateExportTaskRequestRequestTypeDef
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateExportTaskResponseTypeDef = TypedDict(
+    "CreateExportTaskResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLogGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLogGroupRequestRequestTypeDef",
     {
         "logGroupName": str,
@@ -218,14 +238,22 @@
     "CreateLogStreamRequestRequestTypeDef",
     {
         "logGroupName": str,
         "logStreamName": str,
     },
 )
 
+DeleteAccountPolicyRequestRequestTypeDef = TypedDict(
+    "DeleteAccountPolicyRequestRequestTypeDef",
+    {
+        "policyName": str,
+        "policyType": Literal["DATA_PROTECTION_POLICY"],
+    },
+)
+
 DeleteDataProtectionPolicyRequestRequestTypeDef = TypedDict(
     "DeleteDataProtectionPolicyRequestRequestTypeDef",
     {
         "logGroupIdentifier": str,
     },
 )
 
@@ -262,14 +290,22 @@
 DeleteQueryDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteQueryDefinitionRequestRequestTypeDef",
     {
         "queryDefinitionId": str,
     },
 )
 
+DeleteQueryDefinitionResponseTypeDef = TypedDict(
+    "DeleteQueryDefinitionResponseTypeDef",
+    {
+        "success": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "policyName": str,
     },
     total=False,
 )
@@ -285,20 +321,42 @@
     "DeleteSubscriptionFilterRequestRequestTypeDef",
     {
         "logGroupName": str,
         "filterName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeAccountPoliciesRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeAccountPoliciesRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "policyType": Literal["DATA_PROTECTION_POLICY"],
+    },
+)
+_OptionalDescribeAccountPoliciesRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeAccountPoliciesRequestRequestTypeDef",
+    {
+        "policyName": str,
+        "accountIdentifiers": Sequence[str],
+    },
+    total=False,
+)
+
+
+class DescribeAccountPoliciesRequestRequestTypeDef(
+    _RequiredDescribeAccountPoliciesRequestRequestTypeDef,
+    _OptionalDescribeAccountPoliciesRequestRequestTypeDef,
+):
+    pass
+
+
+DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef = TypedDict(
+    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
+    {
+        "DestinationNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeDestinationsRequestRequestTypeDef = TypedDict(
     "DescribeDestinationsRequestRequestTypeDef",
     {
@@ -318,25 +376,47 @@
         "accessPolicy": str,
         "arn": str,
         "creationTime": int,
     },
     total=False,
 )
 
+DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef = TypedDict(
+    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
+    {
+        "taskId": str,
+        "statusCode": ExportTaskStatusCodeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeExportTasksRequestRequestTypeDef = TypedDict(
     "DescribeExportTasksRequestRequestTypeDef",
     {
         "taskId": str,
         "statusCode": ExportTaskStatusCodeType,
         "nextToken": str,
         "limit": int,
     },
     total=False,
 )
 
+DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef = TypedDict(
+    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
+    {
+        "accountIdentifiers": Sequence[str],
+        "logGroupNamePrefix": str,
+        "logGroupNamePattern": str,
+        "includeLinkedAccounts": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeLogGroupsRequestRequestTypeDef = TypedDict(
     "DescribeLogGroupsRequestRequestTypeDef",
     {
         "accountIdentifiers": Sequence[str],
         "logGroupNamePrefix": str,
         "logGroupNamePattern": str,
         "nextToken": str,
@@ -353,14 +433,28 @@
         "creationTime": int,
         "retentionInDays": int,
         "metricFilterCount": int,
         "arn": str,
         "storedBytes": int,
         "kmsKeyId": str,
         "dataProtectionStatus": DataProtectionStatusType,
+        "inheritedProperties": List[Literal["ACCOUNT_DATA_PROTECTION"]],
+    },
+    total=False,
+)
+
+DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef = TypedDict(
+    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "logGroupIdentifier": str,
+        "logStreamNamePrefix": str,
+        "orderBy": OrderByType,
+        "descending": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeLogStreamsRequestRequestTypeDef = TypedDict(
     "DescribeLogStreamsRequestRequestTypeDef",
     {
@@ -386,27 +480,49 @@
         "uploadSequenceToken": str,
         "arn": str,
         "storedBytes": int,
     },
     total=False,
 )
 
+DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef = TypedDict(
+    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "filterNamePrefix": str,
+        "metricName": str,
+        "metricNamespace": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeMetricFiltersRequestRequestTypeDef = TypedDict(
     "DescribeMetricFiltersRequestRequestTypeDef",
     {
         "logGroupName": str,
         "filterNamePrefix": str,
         "nextToken": str,
         "limit": int,
         "metricName": str,
         "metricNamespace": str,
     },
     total=False,
 )
 
+DescribeQueriesRequestDescribeQueriesPaginateTypeDef = TypedDict(
+    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "status": QueryStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeQueriesRequestRequestTypeDef = TypedDict(
     "DescribeQueriesRequestRequestTypeDef",
     {
         "logGroupName": str,
         "status": QueryStatusType,
         "maxResults": int,
         "nextToken": str,
@@ -444,14 +560,22 @@
         "queryString": str,
         "lastModified": int,
         "logGroupNames": List[str],
     },
     total=False,
 )
 
+DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef = TypedDict(
+    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeResourcePoliciesRequestRequestTypeDef = TypedDict(
     "DescribeResourcePoliciesRequestRequestTypeDef",
     {
         "nextToken": str,
         "limit": int,
     },
     total=False,
@@ -463,14 +587,37 @@
         "policyName": str,
         "policyDocument": str,
         "lastUpdatedTime": int,
     },
     total=False,
 )
 
+_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
+    {
+        "logGroupName": str,
+    },
+)
+_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
+    {
+        "filterNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef(
+    _RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
+    _OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeSubscriptionFiltersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSubscriptionFiltersRequestRequestTypeDef",
     {
         "logGroupName": str,
     },
 )
 _OptionalDescribeSubscriptionFiltersRequestRequestTypeDef = TypedDict(
@@ -508,14 +655,21 @@
 DisassociateKmsKeyRequestRequestTypeDef = TypedDict(
     "DisassociateKmsKeyRequestRequestTypeDef",
     {
         "logGroupName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExportTaskExecutionInfoTypeDef = TypedDict(
     "ExportTaskExecutionInfoTypeDef",
     {
         "creationTime": int,
         "completionTime": int,
     },
     total=False,
@@ -526,14 +680,31 @@
     {
         "code": ExportTaskStatusCodeType,
         "message": str,
     },
     total=False,
 )
 
+FilterLogEventsRequestFilterLogEventsPaginateTypeDef = TypedDict(
+    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "logGroupIdentifier": str,
+        "logStreamNames": Sequence[str],
+        "logStreamNamePrefix": str,
+        "startTime": int,
+        "endTime": int,
+        "filterPattern": str,
+        "interleaved": bool,
+        "unmask": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 FilterLogEventsRequestRequestTypeDef = TypedDict(
     "FilterLogEventsRequestRequestTypeDef",
     {
         "logGroupName": str,
         "logGroupIdentifier": str,
         "logStreamNames": Sequence[str],
         "logStreamNamePrefix": str,
@@ -572,14 +743,24 @@
 GetDataProtectionPolicyRequestRequestTypeDef = TypedDict(
     "GetDataProtectionPolicyRequestRequestTypeDef",
     {
         "logGroupIdentifier": str,
     },
 )
 
+GetDataProtectionPolicyResponseTypeDef = TypedDict(
+    "GetDataProtectionPolicyResponseTypeDef",
+    {
+        "logGroupIdentifier": str,
+        "policyDocument": str,
+        "lastUpdatedTime": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetLogEventsRequestRequestTypeDef = TypedDict(
     "_RequiredGetLogEventsRequestRequestTypeDef",
     {
         "logStreamName": str,
     },
 )
 _OptionalGetLogEventsRequestRequestTypeDef = TypedDict(
@@ -650,14 +831,22 @@
 
 class GetLogRecordRequestRequestTypeDef(
     _RequiredGetLogRecordRequestRequestTypeDef, _OptionalGetLogRecordRequestRequestTypeDef
 ):
     pass
 
 
+GetLogRecordResponseTypeDef = TypedDict(
+    "GetLogRecordResponseTypeDef",
+    {
+        "logRecord": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetQueryResultsRequestRequestTypeDef = TypedDict(
     "GetQueryResultsRequestRequestTypeDef",
     {
         "queryId": str,
     },
 )
 
@@ -691,21 +880,37 @@
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
 ListTagsLogGroupRequestRequestTypeDef = TypedDict(
     "ListTagsLogGroupRequestRequestTypeDef",
     {
         "logGroupName": str,
     },
 )
 
+ListTagsLogGroupResponseTypeDef = TypedDict(
+    "ListTagsLogGroupResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MetricFilterMatchRecordTypeDef = TypedDict(
     "MetricFilterMatchRecordTypeDef",
     {
         "eventNumber": int,
         "eventMessage": str,
         "extractedValues": Dict[str, str],
     },
@@ -733,22 +938,65 @@
 
 class MetricTransformationTypeDef(
     _RequiredMetricTransformationTypeDef, _OptionalMetricTransformationTypeDef
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
+_RequiredPutAccountPolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredPutAccountPolicyRequestRequestTypeDef",
+    {
+        "policyName": str,
+        "policyDocument": str,
+        "policyType": Literal["DATA_PROTECTION_POLICY"],
+    },
+)
+_OptionalPutAccountPolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalPutAccountPolicyRequestRequestTypeDef",
+    {
+        "scope": Literal["ALL"],
+    },
+    total=False,
+)
+
+
+class PutAccountPolicyRequestRequestTypeDef(
+    _RequiredPutAccountPolicyRequestRequestTypeDef, _OptionalPutAccountPolicyRequestRequestTypeDef
+):
+    pass
+
+
 PutDataProtectionPolicyRequestRequestTypeDef = TypedDict(
     "PutDataProtectionPolicyRequestRequestTypeDef",
     {
         "logGroupIdentifier": str,
         "policyDocument": str,
     },
 )
 
+PutDataProtectionPolicyResponseTypeDef = TypedDict(
+    "PutDataProtectionPolicyResponseTypeDef",
+    {
+        "logGroupIdentifier": str,
+        "policyDocument": str,
+        "lastUpdatedTime": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutDestinationPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutDestinationPolicyRequestRequestTypeDef",
     {
         "destinationName": str,
         "accessPolicy": str,
     },
 )
@@ -821,14 +1069,22 @@
 class PutQueryDefinitionRequestRequestTypeDef(
     _RequiredPutQueryDefinitionRequestRequestTypeDef,
     _OptionalPutQueryDefinitionRequestRequestTypeDef,
 ):
     pass
 
 
+PutQueryDefinitionResponseTypeDef = TypedDict(
+    "PutQueryDefinitionResponseTypeDef",
+    {
+        "queryDefinitionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policyName": str,
         "policyDocument": str,
     },
     total=False,
@@ -864,14 +1120,25 @@
 class PutSubscriptionFilterRequestRequestTypeDef(
     _RequiredPutSubscriptionFilterRequestRequestTypeDef,
     _OptionalPutSubscriptionFilterRequestRequestTypeDef,
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
 _RequiredStartQueryRequestRequestTypeDef = TypedDict(
     "_RequiredStartQueryRequestRequestTypeDef",
     {
         "startTime": int,
         "endTime": int,
         "queryString": str,
     },
@@ -890,21 +1157,37 @@
 
 class StartQueryRequestRequestTypeDef(
     _RequiredStartQueryRequestRequestTypeDef, _OptionalStartQueryRequestRequestTypeDef
 ):
     pass
 
 
+StartQueryResponseTypeDef = TypedDict(
+    "StartQueryResponseTypeDef",
+    {
+        "queryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopQueryRequestRequestTypeDef = TypedDict(
     "StopQueryRequestRequestTypeDef",
     {
         "queryId": str,
     },
 )
 
+StopQueryResponseTypeDef = TypedDict(
+    "StopQueryResponseTypeDef",
+    {
+        "success": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagLogGroupRequestRequestTypeDef = TypedDict(
     "TagLogGroupRequestRequestTypeDef",
     {
         "logGroupName": str,
         "tags": Mapping[str, str],
     },
 )
@@ -937,295 +1220,106 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-CreateExportTaskResponseTypeDef = TypedDict(
-    "CreateExportTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteQueryDefinitionResponseTypeDef = TypedDict(
-    "DeleteQueryDefinitionResponseTypeDef",
-    {
-        "success": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+DescribeAccountPoliciesResponseTypeDef = TypedDict(
+    "DescribeAccountPoliciesResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "accountPolicies": List[AccountPolicyTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetDataProtectionPolicyResponseTypeDef = TypedDict(
-    "GetDataProtectionPolicyResponseTypeDef",
+PutAccountPolicyResponseTypeDef = TypedDict(
+    "PutAccountPolicyResponseTypeDef",
     {
-        "logGroupIdentifier": str,
-        "policyDocument": str,
-        "lastUpdatedTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "accountPolicy": AccountPolicyTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetLogRecordResponseTypeDef = TypedDict(
-    "GetLogRecordResponseTypeDef",
-    {
-        "logRecord": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsLogGroupResponseTypeDef = TypedDict(
-    "ListTagsLogGroupResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutDataProtectionPolicyResponseTypeDef = TypedDict(
-    "PutDataProtectionPolicyResponseTypeDef",
-    {
-        "logGroupIdentifier": str,
-        "policyDocument": str,
-        "lastUpdatedTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutQueryDefinitionResponseTypeDef = TypedDict(
-    "PutQueryDefinitionResponseTypeDef",
-    {
-        "queryDefinitionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartQueryResponseTypeDef = TypedDict(
-    "StartQueryResponseTypeDef",
-    {
-        "queryId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopQueryResponseTypeDef = TypedDict(
-    "StopQueryResponseTypeDef",
-    {
-        "success": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef = TypedDict(
-    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
-    {
-        "DestinationNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef = TypedDict(
-    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
-    {
-        "taskId": str,
-        "statusCode": ExportTaskStatusCodeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef = TypedDict(
-    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
-    {
-        "accountIdentifiers": Sequence[str],
-        "logGroupNamePrefix": str,
-        "logGroupNamePattern": str,
-        "includeLinkedAccounts": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef = TypedDict(
-    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "logGroupIdentifier": str,
-        "logStreamNamePrefix": str,
-        "orderBy": OrderByType,
-        "descending": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef = TypedDict(
-    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "filterNamePrefix": str,
-        "metricName": str,
-        "metricNamespace": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeQueriesRequestDescribeQueriesPaginateTypeDef = TypedDict(
-    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "status": QueryStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef = TypedDict(
-    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
-    {
-        "logGroupName": str,
-    },
-)
-_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
-    {
-        "filterNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef(
-    _RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
-    _OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
-):
-    pass
-
-
-FilterLogEventsRequestFilterLogEventsPaginateTypeDef = TypedDict(
-    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "logGroupIdentifier": str,
-        "logStreamNames": Sequence[str],
-        "logStreamNamePrefix": str,
-        "startTime": int,
-        "endTime": int,
-        "filterPattern": str,
-        "interleaved": bool,
-        "unmask": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeDestinationsResponseTypeDef = TypedDict(
     "DescribeDestinationsResponseTypeDef",
     {
         "destinations": List[DestinationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutDestinationResponseTypeDef = TypedDict(
     "PutDestinationResponseTypeDef",
     {
         "destination": DestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLogGroupsResponseTypeDef = TypedDict(
     "DescribeLogGroupsResponseTypeDef",
     {
         "logGroups": List[LogGroupTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLogStreamsResponseTypeDef = TypedDict(
     "DescribeLogStreamsResponseTypeDef",
     {
         "logStreams": List[LogStreamTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQueriesResponseTypeDef = TypedDict(
     "DescribeQueriesResponseTypeDef",
     {
         "queries": List[QueryInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQueryDefinitionsResponseTypeDef = TypedDict(
     "DescribeQueryDefinitionsResponseTypeDef",
     {
         "queryDefinitions": List[QueryDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeResourcePoliciesResponseTypeDef = TypedDict(
     "DescribeResourcePoliciesResponseTypeDef",
     {
         "resourcePolicies": List[ResourcePolicyTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutResourcePolicyResponseTypeDef = TypedDict(
     "PutResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSubscriptionFiltersResponseTypeDef = TypedDict(
     "DescribeSubscriptionFiltersResponseTypeDef",
     {
         "subscriptionFilters": List[SubscriptionFilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportTaskTypeDef = TypedDict(
     "ExportTaskTypeDef",
     {
         "taskId": str,
@@ -1243,43 +1337,43 @@
 
 FilterLogEventsResponseTypeDef = TypedDict(
     "FilterLogEventsResponseTypeDef",
     {
         "events": List[FilteredLogEventTypeDef],
         "searchedLogStreams": List[SearchedLogStreamTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLogEventsResponseTypeDef = TypedDict(
     "GetLogEventsResponseTypeDef",
     {
         "events": List[OutputLogEventTypeDef],
         "nextForwardToken": str,
         "nextBackwardToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLogGroupFieldsResponseTypeDef = TypedDict(
     "GetLogGroupFieldsResponseTypeDef",
     {
         "logGroupFields": List[LogGroupFieldTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueryResultsResponseTypeDef = TypedDict(
     "GetQueryResultsResponseTypeDef",
     {
         "results": List[List[ResultFieldTypeDef]],
         "statistics": QueryStatisticsTypeDef,
         "status": QueryStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutLogEventsRequestRequestTypeDef = TypedDict(
     "_RequiredPutLogEventsRequestRequestTypeDef",
     {
         "logGroupName": str,
@@ -1302,15 +1396,15 @@
     pass
 
 
 TestMetricFilterResponseTypeDef = TypedDict(
     "TestMetricFilterResponseTypeDef",
     {
         "matches": List[MetricFilterMatchRecordTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricFilterTypeDef = TypedDict(
     "MetricFilterTypeDef",
     {
         "filterName": str,
@@ -1333,28 +1427,28 @@
 )
 
 PutLogEventsResponseTypeDef = TypedDict(
     "PutLogEventsResponseTypeDef",
     {
         "nextSequenceToken": str,
         "rejectedLogEventsInfo": RejectedLogEventsInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExportTasksResponseTypeDef = TypedDict(
     "DescribeExportTasksResponseTypeDef",
     {
         "exportTasks": List[ExportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMetricFiltersResponseTypeDef = TypedDict(
     "DescribeMetricFiltersResponseTypeDef",
     {
         "metricFilters": List[MetricFilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-logs-1.26.53/mypy_boto3_logs/type_defs.pyi` & `mypy-boto3-logs-1.27.0/mypy_boto3_logs/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for logs service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_logs.type_defs import AssociateKmsKeyRequestRequestTypeDef
+    from mypy_boto3_logs.type_defs import AccountPolicyTypeDef
 
-    data: AssociateKmsKeyRequestRequestTypeDef = {...}
+    data: AccountPolicyTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     DataProtectionStatusType,
@@ -20,106 +20,116 @@
     ExportTaskStatusCodeType,
     OrderByType,
     QueryStatusType,
     StandardUnitType,
 )
 
 if sys.version_info >= (3, 9):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AccountPolicyTypeDef",
     "AssociateKmsKeyRequestRequestTypeDef",
     "CancelExportTaskRequestRequestTypeDef",
     "CreateExportTaskRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateExportTaskResponseTypeDef",
     "CreateLogGroupRequestRequestTypeDef",
     "CreateLogStreamRequestRequestTypeDef",
+    "DeleteAccountPolicyRequestRequestTypeDef",
     "DeleteDataProtectionPolicyRequestRequestTypeDef",
     "DeleteDestinationRequestRequestTypeDef",
     "DeleteLogGroupRequestRequestTypeDef",
     "DeleteLogStreamRequestRequestTypeDef",
     "DeleteMetricFilterRequestRequestTypeDef",
     "DeleteQueryDefinitionRequestRequestTypeDef",
+    "DeleteQueryDefinitionResponseTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRetentionPolicyRequestRequestTypeDef",
     "DeleteSubscriptionFilterRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeAccountPoliciesRequestRequestTypeDef",
+    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
     "DescribeDestinationsRequestRequestTypeDef",
     "DestinationTypeDef",
+    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
     "DescribeExportTasksRequestRequestTypeDef",
+    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
     "DescribeLogGroupsRequestRequestTypeDef",
     "LogGroupTypeDef",
+    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
     "DescribeLogStreamsRequestRequestTypeDef",
     "LogStreamTypeDef",
+    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
     "DescribeMetricFiltersRequestRequestTypeDef",
+    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
     "DescribeQueriesRequestRequestTypeDef",
     "QueryInfoTypeDef",
     "DescribeQueryDefinitionsRequestRequestTypeDef",
     "QueryDefinitionTypeDef",
+    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
     "DescribeResourcePoliciesRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
+    "DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
     "DescribeSubscriptionFiltersRequestRequestTypeDef",
     "SubscriptionFilterTypeDef",
     "DisassociateKmsKeyRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportTaskExecutionInfoTypeDef",
     "ExportTaskStatusTypeDef",
+    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
     "FilterLogEventsRequestRequestTypeDef",
     "FilteredLogEventTypeDef",
     "SearchedLogStreamTypeDef",
     "GetDataProtectionPolicyRequestRequestTypeDef",
+    "GetDataProtectionPolicyResponseTypeDef",
     "GetLogEventsRequestRequestTypeDef",
     "OutputLogEventTypeDef",
     "GetLogGroupFieldsRequestRequestTypeDef",
     "LogGroupFieldTypeDef",
     "GetLogRecordRequestRequestTypeDef",
+    "GetLogRecordResponseTypeDef",
     "GetQueryResultsRequestRequestTypeDef",
     "QueryStatisticsTypeDef",
     "ResultFieldTypeDef",
     "InputLogEventTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTagsLogGroupRequestRequestTypeDef",
+    "ListTagsLogGroupResponseTypeDef",
     "MetricFilterMatchRecordTypeDef",
     "MetricTransformationTypeDef",
+    "PaginatorConfigTypeDef",
+    "PutAccountPolicyRequestRequestTypeDef",
     "PutDataProtectionPolicyRequestRequestTypeDef",
+    "PutDataProtectionPolicyResponseTypeDef",
     "PutDestinationPolicyRequestRequestTypeDef",
     "PutDestinationRequestRequestTypeDef",
     "RejectedLogEventsInfoTypeDef",
     "PutQueryDefinitionRequestRequestTypeDef",
+    "PutQueryDefinitionResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutRetentionPolicyRequestRequestTypeDef",
     "PutSubscriptionFilterRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "StartQueryRequestRequestTypeDef",
+    "StartQueryResponseTypeDef",
     "StopQueryRequestRequestTypeDef",
+    "StopQueryResponseTypeDef",
     "TagLogGroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestMetricFilterRequestRequestTypeDef",
     "UntagLogGroupRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "CreateExportTaskResponseTypeDef",
-    "DeleteQueryDefinitionResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetDataProtectionPolicyResponseTypeDef",
-    "GetLogRecordResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTagsLogGroupResponseTypeDef",
-    "PutDataProtectionPolicyResponseTypeDef",
-    "PutQueryDefinitionResponseTypeDef",
-    "StartQueryResponseTypeDef",
-    "StopQueryResponseTypeDef",
-    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
-    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
-    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
-    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
-    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
-    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
-    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
-    "DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
-    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
+    "DescribeAccountPoliciesResponseTypeDef",
+    "PutAccountPolicyResponseTypeDef",
     "DescribeDestinationsResponseTypeDef",
     "PutDestinationResponseTypeDef",
     "DescribeLogGroupsResponseTypeDef",
     "DescribeLogStreamsResponseTypeDef",
     "DescribeQueriesResponseTypeDef",
     "DescribeQueryDefinitionsResponseTypeDef",
     "DescribeResourcePoliciesResponseTypeDef",
@@ -135,14 +145,27 @@
     "MetricFilterTypeDef",
     "PutMetricFilterRequestRequestTypeDef",
     "PutLogEventsResponseTypeDef",
     "DescribeExportTasksResponseTypeDef",
     "DescribeMetricFiltersResponseTypeDef",
 )
 
+AccountPolicyTypeDef = TypedDict(
+    "AccountPolicyTypeDef",
+    {
+        "policyName": str,
+        "policyDocument": str,
+        "lastUpdatedTime": int,
+        "policyType": Literal["DATA_PROTECTION_POLICY"],
+        "scope": Literal["ALL"],
+        "accountId": str,
+    },
+    total=False,
+)
+
 AssociateKmsKeyRequestRequestTypeDef = TypedDict(
     "AssociateKmsKeyRequestRequestTypeDef",
     {
         "logGroupName": str,
         "kmsKeyId": str,
     },
 )
@@ -174,22 +197,19 @@
 )
 
 class CreateExportTaskRequestRequestTypeDef(
     _RequiredCreateExportTaskRequestRequestTypeDef, _OptionalCreateExportTaskRequestRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateExportTaskResponseTypeDef = TypedDict(
+    "CreateExportTaskResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLogGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLogGroupRequestRequestTypeDef",
     {
         "logGroupName": str,
@@ -213,14 +233,22 @@
     "CreateLogStreamRequestRequestTypeDef",
     {
         "logGroupName": str,
         "logStreamName": str,
     },
 )
 
+DeleteAccountPolicyRequestRequestTypeDef = TypedDict(
+    "DeleteAccountPolicyRequestRequestTypeDef",
+    {
+        "policyName": str,
+        "policyType": Literal["DATA_PROTECTION_POLICY"],
+    },
+)
+
 DeleteDataProtectionPolicyRequestRequestTypeDef = TypedDict(
     "DeleteDataProtectionPolicyRequestRequestTypeDef",
     {
         "logGroupIdentifier": str,
     },
 )
 
@@ -257,14 +285,22 @@
 DeleteQueryDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteQueryDefinitionRequestRequestTypeDef",
     {
         "queryDefinitionId": str,
     },
 )
 
+DeleteQueryDefinitionResponseTypeDef = TypedDict(
+    "DeleteQueryDefinitionResponseTypeDef",
+    {
+        "success": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "policyName": str,
     },
     total=False,
 )
@@ -280,20 +316,40 @@
     "DeleteSubscriptionFilterRequestRequestTypeDef",
     {
         "logGroupName": str,
         "filterName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredDescribeAccountPoliciesRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeAccountPoliciesRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "policyType": Literal["DATA_PROTECTION_POLICY"],
+    },
+)
+_OptionalDescribeAccountPoliciesRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeAccountPoliciesRequestRequestTypeDef",
+    {
+        "policyName": str,
+        "accountIdentifiers": Sequence[str],
+    },
+    total=False,
+)
+
+class DescribeAccountPoliciesRequestRequestTypeDef(
+    _RequiredDescribeAccountPoliciesRequestRequestTypeDef,
+    _OptionalDescribeAccountPoliciesRequestRequestTypeDef,
+):
+    pass
+
+DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef = TypedDict(
+    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
+    {
+        "DestinationNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeDestinationsRequestRequestTypeDef = TypedDict(
     "DescribeDestinationsRequestRequestTypeDef",
     {
@@ -313,25 +369,47 @@
         "accessPolicy": str,
         "arn": str,
         "creationTime": int,
     },
     total=False,
 )
 
+DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef = TypedDict(
+    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
+    {
+        "taskId": str,
+        "statusCode": ExportTaskStatusCodeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeExportTasksRequestRequestTypeDef = TypedDict(
     "DescribeExportTasksRequestRequestTypeDef",
     {
         "taskId": str,
         "statusCode": ExportTaskStatusCodeType,
         "nextToken": str,
         "limit": int,
     },
     total=False,
 )
 
+DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef = TypedDict(
+    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
+    {
+        "accountIdentifiers": Sequence[str],
+        "logGroupNamePrefix": str,
+        "logGroupNamePattern": str,
+        "includeLinkedAccounts": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeLogGroupsRequestRequestTypeDef = TypedDict(
     "DescribeLogGroupsRequestRequestTypeDef",
     {
         "accountIdentifiers": Sequence[str],
         "logGroupNamePrefix": str,
         "logGroupNamePattern": str,
         "nextToken": str,
@@ -348,14 +426,28 @@
         "creationTime": int,
         "retentionInDays": int,
         "metricFilterCount": int,
         "arn": str,
         "storedBytes": int,
         "kmsKeyId": str,
         "dataProtectionStatus": DataProtectionStatusType,
+        "inheritedProperties": List[Literal["ACCOUNT_DATA_PROTECTION"]],
+    },
+    total=False,
+)
+
+DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef = TypedDict(
+    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "logGroupIdentifier": str,
+        "logStreamNamePrefix": str,
+        "orderBy": OrderByType,
+        "descending": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeLogStreamsRequestRequestTypeDef = TypedDict(
     "DescribeLogStreamsRequestRequestTypeDef",
     {
@@ -381,27 +473,49 @@
         "uploadSequenceToken": str,
         "arn": str,
         "storedBytes": int,
     },
     total=False,
 )
 
+DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef = TypedDict(
+    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "filterNamePrefix": str,
+        "metricName": str,
+        "metricNamespace": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeMetricFiltersRequestRequestTypeDef = TypedDict(
     "DescribeMetricFiltersRequestRequestTypeDef",
     {
         "logGroupName": str,
         "filterNamePrefix": str,
         "nextToken": str,
         "limit": int,
         "metricName": str,
         "metricNamespace": str,
     },
     total=False,
 )
 
+DescribeQueriesRequestDescribeQueriesPaginateTypeDef = TypedDict(
+    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "status": QueryStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeQueriesRequestRequestTypeDef = TypedDict(
     "DescribeQueriesRequestRequestTypeDef",
     {
         "logGroupName": str,
         "status": QueryStatusType,
         "maxResults": int,
         "nextToken": str,
@@ -439,14 +553,22 @@
         "queryString": str,
         "lastModified": int,
         "logGroupNames": List[str],
     },
     total=False,
 )
 
+DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef = TypedDict(
+    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeResourcePoliciesRequestRequestTypeDef = TypedDict(
     "DescribeResourcePoliciesRequestRequestTypeDef",
     {
         "nextToken": str,
         "limit": int,
     },
     total=False,
@@ -458,14 +580,35 @@
         "policyName": str,
         "policyDocument": str,
         "lastUpdatedTime": int,
     },
     total=False,
 )
 
+_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
+    {
+        "logGroupName": str,
+    },
+)
+_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
+    {
+        "filterNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef(
+    _RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
+    _OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeSubscriptionFiltersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSubscriptionFiltersRequestRequestTypeDef",
     {
         "logGroupName": str,
     },
 )
 _OptionalDescribeSubscriptionFiltersRequestRequestTypeDef = TypedDict(
@@ -501,14 +644,21 @@
 DisassociateKmsKeyRequestRequestTypeDef = TypedDict(
     "DisassociateKmsKeyRequestRequestTypeDef",
     {
         "logGroupName": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExportTaskExecutionInfoTypeDef = TypedDict(
     "ExportTaskExecutionInfoTypeDef",
     {
         "creationTime": int,
         "completionTime": int,
     },
     total=False,
@@ -519,14 +669,31 @@
     {
         "code": ExportTaskStatusCodeType,
         "message": str,
     },
     total=False,
 )
 
+FilterLogEventsRequestFilterLogEventsPaginateTypeDef = TypedDict(
+    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
+    {
+        "logGroupName": str,
+        "logGroupIdentifier": str,
+        "logStreamNames": Sequence[str],
+        "logStreamNamePrefix": str,
+        "startTime": int,
+        "endTime": int,
+        "filterPattern": str,
+        "interleaved": bool,
+        "unmask": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 FilterLogEventsRequestRequestTypeDef = TypedDict(
     "FilterLogEventsRequestRequestTypeDef",
     {
         "logGroupName": str,
         "logGroupIdentifier": str,
         "logStreamNames": Sequence[str],
         "logStreamNamePrefix": str,
@@ -565,14 +732,24 @@
 GetDataProtectionPolicyRequestRequestTypeDef = TypedDict(
     "GetDataProtectionPolicyRequestRequestTypeDef",
     {
         "logGroupIdentifier": str,
     },
 )
 
+GetDataProtectionPolicyResponseTypeDef = TypedDict(
+    "GetDataProtectionPolicyResponseTypeDef",
+    {
+        "logGroupIdentifier": str,
+        "policyDocument": str,
+        "lastUpdatedTime": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetLogEventsRequestRequestTypeDef = TypedDict(
     "_RequiredGetLogEventsRequestRequestTypeDef",
     {
         "logStreamName": str,
     },
 )
 _OptionalGetLogEventsRequestRequestTypeDef = TypedDict(
@@ -639,14 +816,22 @@
 )
 
 class GetLogRecordRequestRequestTypeDef(
     _RequiredGetLogRecordRequestRequestTypeDef, _OptionalGetLogRecordRequestRequestTypeDef
 ):
     pass
 
+GetLogRecordResponseTypeDef = TypedDict(
+    "GetLogRecordResponseTypeDef",
+    {
+        "logRecord": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetQueryResultsRequestRequestTypeDef = TypedDict(
     "GetQueryResultsRequestRequestTypeDef",
     {
         "queryId": str,
     },
 )
 
@@ -680,21 +865,37 @@
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
 ListTagsLogGroupRequestRequestTypeDef = TypedDict(
     "ListTagsLogGroupRequestRequestTypeDef",
     {
         "logGroupName": str,
     },
 )
 
+ListTagsLogGroupResponseTypeDef = TypedDict(
+    "ListTagsLogGroupResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MetricFilterMatchRecordTypeDef = TypedDict(
     "MetricFilterMatchRecordTypeDef",
     {
         "eventNumber": int,
         "eventMessage": str,
         "extractedValues": Dict[str, str],
     },
@@ -720,22 +921,63 @@
 )
 
 class MetricTransformationTypeDef(
     _RequiredMetricTransformationTypeDef, _OptionalMetricTransformationTypeDef
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
+_RequiredPutAccountPolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredPutAccountPolicyRequestRequestTypeDef",
+    {
+        "policyName": str,
+        "policyDocument": str,
+        "policyType": Literal["DATA_PROTECTION_POLICY"],
+    },
+)
+_OptionalPutAccountPolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalPutAccountPolicyRequestRequestTypeDef",
+    {
+        "scope": Literal["ALL"],
+    },
+    total=False,
+)
+
+class PutAccountPolicyRequestRequestTypeDef(
+    _RequiredPutAccountPolicyRequestRequestTypeDef, _OptionalPutAccountPolicyRequestRequestTypeDef
+):
+    pass
+
 PutDataProtectionPolicyRequestRequestTypeDef = TypedDict(
     "PutDataProtectionPolicyRequestRequestTypeDef",
     {
         "logGroupIdentifier": str,
         "policyDocument": str,
     },
 )
 
+PutDataProtectionPolicyResponseTypeDef = TypedDict(
+    "PutDataProtectionPolicyResponseTypeDef",
+    {
+        "logGroupIdentifier": str,
+        "policyDocument": str,
+        "lastUpdatedTime": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutDestinationPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutDestinationPolicyRequestRequestTypeDef",
     {
         "destinationName": str,
         "accessPolicy": str,
     },
 )
@@ -802,14 +1044,22 @@
 
 class PutQueryDefinitionRequestRequestTypeDef(
     _RequiredPutQueryDefinitionRequestRequestTypeDef,
     _OptionalPutQueryDefinitionRequestRequestTypeDef,
 ):
     pass
 
+PutQueryDefinitionResponseTypeDef = TypedDict(
+    "PutQueryDefinitionResponseTypeDef",
+    {
+        "queryDefinitionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policyName": str,
         "policyDocument": str,
     },
     total=False,
@@ -843,14 +1093,25 @@
 
 class PutSubscriptionFilterRequestRequestTypeDef(
     _RequiredPutSubscriptionFilterRequestRequestTypeDef,
     _OptionalPutSubscriptionFilterRequestRequestTypeDef,
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
 _RequiredStartQueryRequestRequestTypeDef = TypedDict(
     "_RequiredStartQueryRequestRequestTypeDef",
     {
         "startTime": int,
         "endTime": int,
         "queryString": str,
     },
@@ -867,21 +1128,37 @@
 )
 
 class StartQueryRequestRequestTypeDef(
     _RequiredStartQueryRequestRequestTypeDef, _OptionalStartQueryRequestRequestTypeDef
 ):
     pass
 
+StartQueryResponseTypeDef = TypedDict(
+    "StartQueryResponseTypeDef",
+    {
+        "queryId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopQueryRequestRequestTypeDef = TypedDict(
     "StopQueryRequestRequestTypeDef",
     {
         "queryId": str,
     },
 )
 
+StopQueryResponseTypeDef = TypedDict(
+    "StopQueryResponseTypeDef",
+    {
+        "success": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagLogGroupRequestRequestTypeDef = TypedDict(
     "TagLogGroupRequestRequestTypeDef",
     {
         "logGroupName": str,
         "tags": Mapping[str, str],
     },
 )
@@ -914,293 +1191,106 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-CreateExportTaskResponseTypeDef = TypedDict(
-    "CreateExportTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteQueryDefinitionResponseTypeDef = TypedDict(
-    "DeleteQueryDefinitionResponseTypeDef",
-    {
-        "success": bool,
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
-GetDataProtectionPolicyResponseTypeDef = TypedDict(
-    "GetDataProtectionPolicyResponseTypeDef",
-    {
-        "logGroupIdentifier": str,
-        "policyDocument": str,
-        "lastUpdatedTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLogRecordResponseTypeDef = TypedDict(
-    "GetLogRecordResponseTypeDef",
+DescribeAccountPoliciesResponseTypeDef = TypedDict(
+    "DescribeAccountPoliciesResponseTypeDef",
     {
-        "logRecord": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "accountPolicies": List[AccountPolicyTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+PutAccountPolicyResponseTypeDef = TypedDict(
+    "PutAccountPolicyResponseTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "accountPolicy": AccountPolicyTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsLogGroupResponseTypeDef = TypedDict(
-    "ListTagsLogGroupResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutDataProtectionPolicyResponseTypeDef = TypedDict(
-    "PutDataProtectionPolicyResponseTypeDef",
-    {
-        "logGroupIdentifier": str,
-        "policyDocument": str,
-        "lastUpdatedTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutQueryDefinitionResponseTypeDef = TypedDict(
-    "PutQueryDefinitionResponseTypeDef",
-    {
-        "queryDefinitionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartQueryResponseTypeDef = TypedDict(
-    "StartQueryResponseTypeDef",
-    {
-        "queryId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopQueryResponseTypeDef = TypedDict(
-    "StopQueryResponseTypeDef",
-    {
-        "success": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef = TypedDict(
-    "DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef",
-    {
-        "DestinationNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef = TypedDict(
-    "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
-    {
-        "taskId": str,
-        "statusCode": ExportTaskStatusCodeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef = TypedDict(
-    "DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef",
-    {
-        "accountIdentifiers": Sequence[str],
-        "logGroupNamePrefix": str,
-        "logGroupNamePattern": str,
-        "includeLinkedAccounts": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef = TypedDict(
-    "DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "logGroupIdentifier": str,
-        "logStreamNamePrefix": str,
-        "orderBy": OrderByType,
-        "descending": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef = TypedDict(
-    "DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "filterNamePrefix": str,
-        "metricName": str,
-        "metricNamespace": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeQueriesRequestDescribeQueriesPaginateTypeDef = TypedDict(
-    "DescribeQueriesRequestDescribeQueriesPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "status": QueryStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef = TypedDict(
-    "DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
-    {
-        "logGroupName": str,
-    },
-)
-_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef",
-    {
-        "filterNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef(
-    _RequiredDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
-    _OptionalDescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
-):
-    pass
-
-FilterLogEventsRequestFilterLogEventsPaginateTypeDef = TypedDict(
-    "FilterLogEventsRequestFilterLogEventsPaginateTypeDef",
-    {
-        "logGroupName": str,
-        "logGroupIdentifier": str,
-        "logStreamNames": Sequence[str],
-        "logStreamNamePrefix": str,
-        "startTime": int,
-        "endTime": int,
-        "filterPattern": str,
-        "interleaved": bool,
-        "unmask": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeDestinationsResponseTypeDef = TypedDict(
     "DescribeDestinationsResponseTypeDef",
     {
         "destinations": List[DestinationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutDestinationResponseTypeDef = TypedDict(
     "PutDestinationResponseTypeDef",
     {
         "destination": DestinationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLogGroupsResponseTypeDef = TypedDict(
     "DescribeLogGroupsResponseTypeDef",
     {
         "logGroups": List[LogGroupTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeLogStreamsResponseTypeDef = TypedDict(
     "DescribeLogStreamsResponseTypeDef",
     {
         "logStreams": List[LogStreamTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQueriesResponseTypeDef = TypedDict(
     "DescribeQueriesResponseTypeDef",
     {
         "queries": List[QueryInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeQueryDefinitionsResponseTypeDef = TypedDict(
     "DescribeQueryDefinitionsResponseTypeDef",
     {
         "queryDefinitions": List[QueryDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeResourcePoliciesResponseTypeDef = TypedDict(
     "DescribeResourcePoliciesResponseTypeDef",
     {
         "resourcePolicies": List[ResourcePolicyTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutResourcePolicyResponseTypeDef = TypedDict(
     "PutResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSubscriptionFiltersResponseTypeDef = TypedDict(
     "DescribeSubscriptionFiltersResponseTypeDef",
     {
         "subscriptionFilters": List[SubscriptionFilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportTaskTypeDef = TypedDict(
     "ExportTaskTypeDef",
     {
         "taskId": str,
@@ -1218,43 +1308,43 @@
 
 FilterLogEventsResponseTypeDef = TypedDict(
     "FilterLogEventsResponseTypeDef",
     {
         "events": List[FilteredLogEventTypeDef],
         "searchedLogStreams": List[SearchedLogStreamTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLogEventsResponseTypeDef = TypedDict(
     "GetLogEventsResponseTypeDef",
     {
         "events": List[OutputLogEventTypeDef],
         "nextForwardToken": str,
         "nextBackwardToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLogGroupFieldsResponseTypeDef = TypedDict(
     "GetLogGroupFieldsResponseTypeDef",
     {
         "logGroupFields": List[LogGroupFieldTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueryResultsResponseTypeDef = TypedDict(
     "GetQueryResultsResponseTypeDef",
     {
         "results": List[List[ResultFieldTypeDef]],
         "statistics": QueryStatisticsTypeDef,
         "status": QueryStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutLogEventsRequestRequestTypeDef = TypedDict(
     "_RequiredPutLogEventsRequestRequestTypeDef",
     {
         "logGroupName": str,
@@ -1275,15 +1365,15 @@
 ):
     pass
 
 TestMetricFilterResponseTypeDef = TypedDict(
     "TestMetricFilterResponseTypeDef",
     {
         "matches": List[MetricFilterMatchRecordTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MetricFilterTypeDef = TypedDict(
     "MetricFilterTypeDef",
     {
         "filterName": str,
@@ -1306,28 +1396,28 @@
 )
 
 PutLogEventsResponseTypeDef = TypedDict(
     "PutLogEventsResponseTypeDef",
     {
         "nextSequenceToken": str,
         "rejectedLogEventsInfo": RejectedLogEventsInfoTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExportTasksResponseTypeDef = TypedDict(
     "DescribeExportTasksResponseTypeDef",
     {
         "exportTasks": List[ExportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeMetricFiltersResponseTypeDef = TypedDict(
     "DescribeMetricFiltersResponseTypeDef",
     {
         "metricFilters": List[MetricFilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-logs-1.26.53/mypy_boto3_logs.egg-info/PKG-INFO` & `mypy-boto3-logs-1.27.0/mypy_boto3_logs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-logs
-Version: 1.26.53
-Summary: Type annotations for boto3.CloudWatchLogs 1.26.53 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.CloudWatchLogs 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-logs"></a>
 
 # mypy-boto3-logs
 
 [![PyPI - mypy-boto3-logs](https://img.shields.io/pypi/v/mypy-boto3-logs.svg?color=blue)](https://pypi.org/project/mypy-boto3-logs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-logs.svg?color=blue)](https://pypi.org/project/mypy-boto3-logs)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-logs?color=blue)](https://pypistats.org/packages/mypy-boto3-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchLogs 1.26.53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[boto3.CloudWatchLogs 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
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
 [mypy-boto3-logs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,16 +340,19 @@
     DescribeMetricFiltersPaginatorName,
     DescribeQueriesPaginatorName,
     DescribeResourcePoliciesPaginatorName,
     DescribeSubscriptionFiltersPaginatorName,
     DistributionType,
     ExportTaskStatusCodeType,
     FilterLogEventsPaginatorName,
+    InheritedPropertyType,
     OrderByType,
+    PolicyTypeType,
     QueryStatusType,
+    ScopeType,
     StandardUnitType,
     CloudWatchLogsServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
@@ -364,101 +367,107 @@
 ### Typed dictionaries
 
 `mypy_boto3_logs.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_logs.type_defs import (
+    AccountPolicyTypeDef,
     AssociateKmsKeyRequestRequestTypeDef,
     CancelExportTaskRequestRequestTypeDef,
     CreateExportTaskRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    CreateExportTaskResponseTypeDef,
     CreateLogGroupRequestRequestTypeDef,
     CreateLogStreamRequestRequestTypeDef,
+    DeleteAccountPolicyRequestRequestTypeDef,
     DeleteDataProtectionPolicyRequestRequestTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteLogGroupRequestRequestTypeDef,
     DeleteLogStreamRequestRequestTypeDef,
     DeleteMetricFilterRequestRequestTypeDef,
     DeleteQueryDefinitionRequestRequestTypeDef,
+    DeleteQueryDefinitionResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRetentionPolicyRequestRequestTypeDef,
     DeleteSubscriptionFilterRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeAccountPoliciesRequestRequestTypeDef,
+    DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef,
     DescribeDestinationsRequestRequestTypeDef,
     DestinationTypeDef,
+    DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
     DescribeExportTasksRequestRequestTypeDef,
+    DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef,
     DescribeLogGroupsRequestRequestTypeDef,
     LogGroupTypeDef,
+    DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef,
     DescribeLogStreamsRequestRequestTypeDef,
     LogStreamTypeDef,
+    DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef,
     DescribeMetricFiltersRequestRequestTypeDef,
+    DescribeQueriesRequestDescribeQueriesPaginateTypeDef,
     DescribeQueriesRequestRequestTypeDef,
     QueryInfoTypeDef,
     DescribeQueryDefinitionsRequestRequestTypeDef,
     QueryDefinitionTypeDef,
+    DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef,
     DescribeResourcePoliciesRequestRequestTypeDef,
     ResourcePolicyTypeDef,
+    DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
     DescribeSubscriptionFiltersRequestRequestTypeDef,
     SubscriptionFilterTypeDef,
     DisassociateKmsKeyRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportTaskExecutionInfoTypeDef,
     ExportTaskStatusTypeDef,
+    FilterLogEventsRequestFilterLogEventsPaginateTypeDef,
     FilterLogEventsRequestRequestTypeDef,
     FilteredLogEventTypeDef,
     SearchedLogStreamTypeDef,
     GetDataProtectionPolicyRequestRequestTypeDef,
+    GetDataProtectionPolicyResponseTypeDef,
     GetLogEventsRequestRequestTypeDef,
     OutputLogEventTypeDef,
     GetLogGroupFieldsRequestRequestTypeDef,
     LogGroupFieldTypeDef,
     GetLogRecordRequestRequestTypeDef,
+    GetLogRecordResponseTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     ResultFieldTypeDef,
     InputLogEventTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTagsLogGroupRequestRequestTypeDef,
+    ListTagsLogGroupResponseTypeDef,
     MetricFilterMatchRecordTypeDef,
     MetricTransformationTypeDef,
+    PaginatorConfigTypeDef,
+    PutAccountPolicyRequestRequestTypeDef,
     PutDataProtectionPolicyRequestRequestTypeDef,
+    PutDataProtectionPolicyResponseTypeDef,
     PutDestinationPolicyRequestRequestTypeDef,
     PutDestinationRequestRequestTypeDef,
     RejectedLogEventsInfoTypeDef,
     PutQueryDefinitionRequestRequestTypeDef,
+    PutQueryDefinitionResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutRetentionPolicyRequestRequestTypeDef,
     PutSubscriptionFilterRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     StartQueryRequestRequestTypeDef,
+    StartQueryResponseTypeDef,
     StopQueryRequestRequestTypeDef,
+    StopQueryResponseTypeDef,
     TagLogGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestMetricFilterRequestRequestTypeDef,
     UntagLogGroupRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    CreateExportTaskResponseTypeDef,
-    DeleteQueryDefinitionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDataProtectionPolicyResponseTypeDef,
-    GetLogRecordResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTagsLogGroupResponseTypeDef,
-    PutDataProtectionPolicyResponseTypeDef,
-    PutQueryDefinitionResponseTypeDef,
-    StartQueryResponseTypeDef,
-    StopQueryResponseTypeDef,
-    DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef,
-    DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
-    DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef,
-    DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef,
-    DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef,
-    DescribeQueriesRequestDescribeQueriesPaginateTypeDef,
-    DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef,
-    DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef,
-    FilterLogEventsRequestFilterLogEventsPaginateTypeDef,
+    DescribeAccountPoliciesResponseTypeDef,
+    PutAccountPolicyResponseTypeDef,
     DescribeDestinationsResponseTypeDef,
     PutDestinationResponseTypeDef,
     DescribeLogGroupsResponseTypeDef,
     DescribeLogStreamsResponseTypeDef,
     DescribeQueriesResponseTypeDef,
     DescribeQueryDefinitionsResponseTypeDef,
     DescribeResourcePoliciesResponseTypeDef,
@@ -475,53 +484,53 @@
     PutMetricFilterRequestRequestTypeDef,
     PutLogEventsResponseTypeDef,
     DescribeExportTasksResponseTypeDef,
     DescribeMetricFiltersResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateKmsKeyRequestRequestTypeDef:
+def get_structure() -> AccountPolicyTypeDef:
     return {...}
 ```
 
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

### Comparing `mypy-boto3-logs-1.26.53/mypy_boto3_logs.egg-info/SOURCES.txt` & `mypy-boto3-logs-1.27.0/mypy_boto3_logs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-logs-1.26.53/setup.py` & `mypy-boto3-logs-1.27.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-logs.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-logs",
-    version="1.26.53",
+    version="1.27.0",
     packages=["mypy_boto3_logs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchLogs 1.26.53 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.CloudWatchLogs 1.27.0 service generated with mypy-boto3-builder"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_logs/",
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


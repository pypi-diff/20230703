# Comparing `tmp/mypy-boto3-ssm-incidents-1.26.8.tar.gz` & `tmp/mypy-boto3-ssm-incidents-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-incidents-1.26.8.tar", last modified: Fri Nov 11 21:07:54 2022, max compression
+gzip compressed data, was "mypy-boto3-ssm-incidents-1.27.0.tar", last modified: Mon Jul  3 19:51:30 2023, max compression
```

## Comparing `mypy-boto3-ssm-incidents-1.26.8.tar` & `mypy-boto3-ssm-incidents-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.062122 mypy-boto3-ssm-incidents-1.26.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    18120 2022-11-11 21:07:54.058122 mypy-boto3-ssm-incidents-1.26.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16662 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.058122 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/
--rw-r--r--   0 runner    (1001) docker     (121)     2281 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25547 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    25503 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9337 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9335 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7893 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7884 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    32544 2022-11-11 21:07:45.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    32482 2022-11-11 21:07:45.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2645 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2643 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.058122 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18120 2022-11-11 21:07:53.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-11-11 21:07:53.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-11 21:07:53.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-11 21:07:53.000000 mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 21:07:54.062122 mypy-boto3-ssm-incidents-1.26.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-11-11 21:07:44.000000 mypy-boto3-ssm-incidents-1.26.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:30.512049 mypy-boto3-ssm-incidents-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18292 2023-07-03 19:51:30.512049 mypy-boto3-ssm-incidents-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16784 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:30.512049 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25687 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25643 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33935 2023-07-03 19:48:42.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33871 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-03 19:48:41.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:30.512049 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18292 2023-07-03 19:51:30.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-03 19:51:30.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:30.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:30.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:30.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 19:51:30.000000 mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:30.512049 mypy-boto3-ssm-incidents-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-03 19:48:40.000000 mypy-boto3-ssm-incidents-1.27.0/setup.py
```

### Comparing `mypy-boto3-ssm-incidents-1.26.8/LICENSE` & `mypy-boto3-ssm-incidents-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-ssm-incidents-1.26.8/PKG-INFO` & `mypy-boto3-ssm-incidents-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-incidents
-Version: 1.26.8
-Summary: Type annotations for boto3.SSMIncidents 1.26.8 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.SSMIncidents 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/
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
 
 <a id="mypy-boto3-ssm-incidents"></a>
 
 # mypy-boto3-ssm-incidents
 
 [![PyPI - mypy-boto3-ssm-incidents](https://img.shields.io/pypi/v/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-incidents?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMIncidents 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[boto3.SSMIncidents 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
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
 [mypy-boto3-ssm-incidents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,87 +391,91 @@
 ```python
 from mypy_boto3_ssm_incidents.type_defs import (
     AddRegionActionTypeDef,
     AttributeValueListTypeDef,
     AutomationExecutionTypeDef,
     ChatChannelTypeDef,
     RegionMapInputValueTypeDef,
-    ResponseMetadataTypeDef,
+    CreateReplicationSetOutputTypeDef,
+    CreateResponsePlanOutputTypeDef,
     EventReferenceTypeDef,
+    CreateTimelineEventOutputTypeDef,
     DeleteIncidentRecordInputRequestTypeDef,
     DeleteRegionActionTypeDef,
     DeleteReplicationSetInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteResponsePlanInputRequestTypeDef,
     DeleteTimelineEventInputRequestTypeDef,
     DynamicSsmParameterValueTypeDef,
     GetIncidentRecordInputRequestTypeDef,
     GetReplicationSetInputRequestTypeDef,
     WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
+    GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
     GetResourcePoliciesInputRequestTypeDef,
     ResourcePolicyTypeDef,
     GetResponsePlanInputRequestTypeDef,
     GetTimelineEventInputRequestTypeDef,
     IncidentRecordSourceTypeDef,
     NotificationTargetItemTypeDef,
-    ItemValueTypeDef,
+    PagerDutyIncidentDetailTypeDef,
+    ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
     ListRelatedItemsInputRequestTypeDef,
+    ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
     ListReplicationSetsInputRequestTypeDef,
+    ListReplicationSetsOutputTypeDef,
+    ListResponsePlansInputListResponsePlansPaginateTypeDef,
     ListResponsePlansInputRequestTypeDef,
     ResponsePlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PagerDutyIncidentConfigurationTypeDef,
+    PaginatorConfigTypeDef,
     PutResourcePolicyInputRequestTypeDef,
+    PutResourcePolicyOutputTypeDef,
     RegionInfoTypeDef,
+    ResponseMetadataTypeDef,
     TriggerDetailsTypeDef,
+    StartIncidentOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeletionProtectionInputRequestTypeDef,
     ConditionTypeDef,
     CreateReplicationSetInputRequestTypeDef,
-    CreateReplicationSetOutputTypeDef,
-    CreateResponsePlanOutputTypeDef,
-    CreateTimelineEventOutputTypeDef,
-    ListReplicationSetsOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutResourcePolicyOutputTypeDef,
-    StartIncidentOutputTypeDef,
     CreateTimelineEventInputRequestTypeDef,
     EventSummaryTypeDef,
     TimelineEventTypeDef,
     UpdateTimelineEventInputRequestTypeDef,
     UpdateReplicationSetActionTypeDef,
     SsmAutomationTypeDef,
     GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
     GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
-    GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
-    ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
-    ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
-    ListResponsePlansInputListResponsePlansPaginateTypeDef,
     GetResourcePoliciesOutputTypeDef,
     IncidentRecordSummaryTypeDef,
     IncidentRecordTypeDef,
     IncidentTemplateTypeDef,
     UpdateIncidentRecordInputRequestTypeDef,
-    ItemIdentifierTypeDef,
+    ItemValueTypeDef,
     ListResponsePlansOutputTypeDef,
+    PagerDutyConfigurationTypeDef,
     ReplicationSetTypeDef,
     FilterTypeDef,
     ListTimelineEventsOutputTypeDef,
     GetTimelineEventOutputTypeDef,
     UpdateReplicationSetInputRequestTypeDef,
     ActionTypeDef,
     ListIncidentRecordsOutputTypeDef,
     GetIncidentRecordOutputTypeDef,
-    RelatedItemTypeDef,
+    ItemIdentifierTypeDef,
+    IntegrationTypeDef,
     GetReplicationSetOutputTypeDef,
     ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef,
     ListIncidentRecordsInputRequestTypeDef,
     ListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     ListTimelineEventsInputRequestTypeDef,
+    RelatedItemTypeDef,
     CreateResponsePlanInputRequestTypeDef,
     GetResponsePlanOutputTypeDef,
     UpdateResponsePlanInputRequestTypeDef,
     ListRelatedItemsOutputTypeDef,
     RelatedItemsUpdateTypeDef,
     StartIncidentInputRequestTypeDef,
     UpdateRelatedItemsInputRequestTypeDef,
@@ -484,42 +489,42 @@
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

### Comparing `mypy-boto3-ssm-incidents-1.26.8/README.md` & `mypy-boto3-ssm-incidents-1.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ssm-incidents"></a>
 
 # mypy-boto3-ssm-incidents
 
 [![PyPI - mypy-boto3-ssm-incidents](https://img.shields.io/pypi/v/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-incidents?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMIncidents 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[boto3.SSMIncidents 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
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
 [mypy-boto3-ssm-incidents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,87 +359,91 @@
 ```python
 from mypy_boto3_ssm_incidents.type_defs import (
     AddRegionActionTypeDef,
     AttributeValueListTypeDef,
     AutomationExecutionTypeDef,
     ChatChannelTypeDef,
     RegionMapInputValueTypeDef,
-    ResponseMetadataTypeDef,
+    CreateReplicationSetOutputTypeDef,
+    CreateResponsePlanOutputTypeDef,
     EventReferenceTypeDef,
+    CreateTimelineEventOutputTypeDef,
     DeleteIncidentRecordInputRequestTypeDef,
     DeleteRegionActionTypeDef,
     DeleteReplicationSetInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteResponsePlanInputRequestTypeDef,
     DeleteTimelineEventInputRequestTypeDef,
     DynamicSsmParameterValueTypeDef,
     GetIncidentRecordInputRequestTypeDef,
     GetReplicationSetInputRequestTypeDef,
     WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
+    GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
     GetResourcePoliciesInputRequestTypeDef,
     ResourcePolicyTypeDef,
     GetResponsePlanInputRequestTypeDef,
     GetTimelineEventInputRequestTypeDef,
     IncidentRecordSourceTypeDef,
     NotificationTargetItemTypeDef,
-    ItemValueTypeDef,
+    PagerDutyIncidentDetailTypeDef,
+    ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
     ListRelatedItemsInputRequestTypeDef,
+    ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
     ListReplicationSetsInputRequestTypeDef,
+    ListReplicationSetsOutputTypeDef,
+    ListResponsePlansInputListResponsePlansPaginateTypeDef,
     ListResponsePlansInputRequestTypeDef,
     ResponsePlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PagerDutyIncidentConfigurationTypeDef,
+    PaginatorConfigTypeDef,
     PutResourcePolicyInputRequestTypeDef,
+    PutResourcePolicyOutputTypeDef,
     RegionInfoTypeDef,
+    ResponseMetadataTypeDef,
     TriggerDetailsTypeDef,
+    StartIncidentOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeletionProtectionInputRequestTypeDef,
     ConditionTypeDef,
     CreateReplicationSetInputRequestTypeDef,
-    CreateReplicationSetOutputTypeDef,
-    CreateResponsePlanOutputTypeDef,
-    CreateTimelineEventOutputTypeDef,
-    ListReplicationSetsOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutResourcePolicyOutputTypeDef,
-    StartIncidentOutputTypeDef,
     CreateTimelineEventInputRequestTypeDef,
     EventSummaryTypeDef,
     TimelineEventTypeDef,
     UpdateTimelineEventInputRequestTypeDef,
     UpdateReplicationSetActionTypeDef,
     SsmAutomationTypeDef,
     GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
     GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
-    GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
-    ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
-    ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
-    ListResponsePlansInputListResponsePlansPaginateTypeDef,
     GetResourcePoliciesOutputTypeDef,
     IncidentRecordSummaryTypeDef,
     IncidentRecordTypeDef,
     IncidentTemplateTypeDef,
     UpdateIncidentRecordInputRequestTypeDef,
-    ItemIdentifierTypeDef,
+    ItemValueTypeDef,
     ListResponsePlansOutputTypeDef,
+    PagerDutyConfigurationTypeDef,
     ReplicationSetTypeDef,
     FilterTypeDef,
     ListTimelineEventsOutputTypeDef,
     GetTimelineEventOutputTypeDef,
     UpdateReplicationSetInputRequestTypeDef,
     ActionTypeDef,
     ListIncidentRecordsOutputTypeDef,
     GetIncidentRecordOutputTypeDef,
-    RelatedItemTypeDef,
+    ItemIdentifierTypeDef,
+    IntegrationTypeDef,
     GetReplicationSetOutputTypeDef,
     ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef,
     ListIncidentRecordsInputRequestTypeDef,
     ListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     ListTimelineEventsInputRequestTypeDef,
+    RelatedItemTypeDef,
     CreateResponsePlanInputRequestTypeDef,
     GetResponsePlanOutputTypeDef,
     UpdateResponsePlanInputRequestTypeDef,
     ListRelatedItemsOutputTypeDef,
     RelatedItemsUpdateTypeDef,
     StartIncidentInputRequestTypeDef,
     UpdateRelatedItemsInputRequestTypeDef,
@@ -453,42 +457,42 @@
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

### Comparing `mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/__init__.py` & `mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/__init__.pyi` & `mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/__main__.py` & `mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSMIncidents 1.26.8\nVersion:         1.26.8\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.SSMIncidents 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.8")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/client.py` & `mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     FilterTypeDef,
     GetIncidentRecordOutputTypeDef,
     GetReplicationSetOutputTypeDef,
     GetResourcePoliciesOutputTypeDef,
     GetResponsePlanOutputTypeDef,
     GetTimelineEventOutputTypeDef,
     IncidentTemplateTypeDef,
+    IntegrationTypeDef,
     ListIncidentRecordsOutputTypeDef,
     ListRelatedItemsOutputTypeDef,
     ListReplicationSetsOutputTypeDef,
     ListResponsePlansOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTimelineEventsOutputTypeDef,
     NotificationTargetItemTypeDef,
@@ -141,14 +142,15 @@
         incidentTemplate: IncidentTemplateTypeDef,
         name: str,
         actions: Sequence[ActionTypeDef] = ...,
         chatChannel: ChatChannelTypeDef = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
+        integrations: Sequence[IntegrationTypeDef] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateResponsePlanOutputTypeDef:
         """
         Creates a response plan that automates the initial response to incidents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_response_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#create_response_plan)
@@ -448,15 +450,16 @@
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         incidentTemplateDedupeString: str = ...,
         incidentTemplateImpact: int = ...,
         incidentTemplateNotificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         incidentTemplateSummary: str = ...,
         incidentTemplateTags: Mapping[str, str] = ...,
-        incidentTemplateTitle: str = ...
+        incidentTemplateTitle: str = ...,
+        integrations: Sequence[IntegrationTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_response_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#update_response_plan)
         """
```

### Comparing `mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/client.pyi` & `mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     FilterTypeDef,
     GetIncidentRecordOutputTypeDef,
     GetReplicationSetOutputTypeDef,
     GetResourcePoliciesOutputTypeDef,
     GetResponsePlanOutputTypeDef,
     GetTimelineEventOutputTypeDef,
     IncidentTemplateTypeDef,
+    IntegrationTypeDef,
     ListIncidentRecordsOutputTypeDef,
     ListRelatedItemsOutputTypeDef,
     ListReplicationSetsOutputTypeDef,
     ListResponsePlansOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTimelineEventsOutputTypeDef,
     NotificationTargetItemTypeDef,
@@ -133,14 +134,15 @@
         incidentTemplate: IncidentTemplateTypeDef,
         name: str,
         actions: Sequence[ActionTypeDef] = ...,
         chatChannel: ChatChannelTypeDef = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
+        integrations: Sequence[IntegrationTypeDef] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateResponsePlanOutputTypeDef:
         """
         Creates a response plan that automates the initial response to incidents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_response_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#create_response_plan)
@@ -413,15 +415,16 @@
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         incidentTemplateDedupeString: str = ...,
         incidentTemplateImpact: int = ...,
         incidentTemplateNotificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         incidentTemplateSummary: str = ...,
         incidentTemplateTags: Mapping[str, str] = ...,
-        incidentTemplateTitle: str = ...
+        incidentTemplateTitle: str = ...,
+        integrations: Sequence[IntegrationTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified response plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_response_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#update_response_plan)
         """
```

### Comparing `mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/literals.py` & `mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/literals.py`

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
@@ -335,56 +357,64 @@
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
     "scheduler",
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

### Comparing `mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/literals.pyi` & `mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -81,23 +81,25 @@
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
@@ -107,30 +109,35 @@
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
@@ -156,14 +163,15 @@
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
@@ -208,51 +216,57 @@
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
@@ -265,14 +279,15 @@
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
@@ -284,28 +299,35 @@
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
@@ -333,56 +355,64 @@
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
     "scheduler",
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

### Comparing `mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/paginator.py` & `mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 class GetResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.GetResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#getresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourcePoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.GetResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#getresourcepoliciespaginator)
         """
 
 
@@ -93,60 +93,60 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listincidentrecordspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIncidentRecordsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListIncidentRecords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listincidentrecordspaginator)
         """
 
 
 class ListRelatedItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListRelatedItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listrelateditemspaginator)
     """
 
     def paginate(
-        self, *, incidentRecordArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, incidentRecordArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRelatedItemsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListRelatedItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listrelateditemspaginator)
         """
 
 
 class ListReplicationSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListReplicationSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listreplicationsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReplicationSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListReplicationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listreplicationsetspaginator)
         """
 
 
 class ListResponsePlansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListResponsePlans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listresponseplanspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResponsePlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListResponsePlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listresponseplanspaginator)
         """
 
 
@@ -159,13 +159,13 @@
     def paginate(
         self,
         *,
         incidentRecordArn: str,
         filters: Sequence[FilterTypeDef] = ...,
         sortBy: Literal["EVENT_TIME"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTimelineEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListTimelineEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listtimelineeventspaginator)
         """
```

### Comparing `mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/paginator.pyi` & `mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 class GetResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.GetResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#getresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourcePoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.GetResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#getresourcepoliciespaginator)
         """
 
 class ListIncidentRecordsPaginator(Paginator):
@@ -88,57 +88,57 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listincidentrecordspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListIncidentRecordsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListIncidentRecords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listincidentrecordspaginator)
         """
 
 class ListRelatedItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListRelatedItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listrelateditemspaginator)
     """
 
     def paginate(
-        self, *, incidentRecordArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, incidentRecordArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRelatedItemsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListRelatedItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listrelateditemspaginator)
         """
 
 class ListReplicationSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListReplicationSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listreplicationsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListReplicationSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListReplicationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listreplicationsetspaginator)
         """
 
 class ListResponsePlansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListResponsePlans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listresponseplanspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResponsePlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListResponsePlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listresponseplanspaginator)
         """
 
 class ListTimelineEventsPaginator(Paginator):
@@ -150,13 +150,13 @@
     def paginate(
         self,
         *,
         incidentRecordArn: str,
         filters: Sequence[FilterTypeDef] = ...,
         sortBy: Literal["EVENT_TIME"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTimelineEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListTimelineEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listtimelineeventspaginator)
         """
```

### Comparing `mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/type_defs.py` & `mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,87 +37,91 @@
 
 __all__ = (
     "AddRegionActionTypeDef",
     "AttributeValueListTypeDef",
     "AutomationExecutionTypeDef",
     "ChatChannelTypeDef",
     "RegionMapInputValueTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateReplicationSetOutputTypeDef",
+    "CreateResponsePlanOutputTypeDef",
     "EventReferenceTypeDef",
+    "CreateTimelineEventOutputTypeDef",
     "DeleteIncidentRecordInputRequestTypeDef",
     "DeleteRegionActionTypeDef",
     "DeleteReplicationSetInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteResponsePlanInputRequestTypeDef",
     "DeleteTimelineEventInputRequestTypeDef",
     "DynamicSsmParameterValueTypeDef",
     "GetIncidentRecordInputRequestTypeDef",
     "GetReplicationSetInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     "GetResourcePoliciesInputRequestTypeDef",
     "ResourcePolicyTypeDef",
     "GetResponsePlanInputRequestTypeDef",
     "GetTimelineEventInputRequestTypeDef",
     "IncidentRecordSourceTypeDef",
     "NotificationTargetItemTypeDef",
-    "ItemValueTypeDef",
+    "PagerDutyIncidentDetailTypeDef",
+    "ListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     "ListRelatedItemsInputRequestTypeDef",
+    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
     "ListReplicationSetsInputRequestTypeDef",
+    "ListReplicationSetsOutputTypeDef",
+    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
     "ListResponsePlansInputRequestTypeDef",
     "ResponsePlanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PagerDutyIncidentConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
+    "PutResourcePolicyOutputTypeDef",
     "RegionInfoTypeDef",
+    "ResponseMetadataTypeDef",
     "TriggerDetailsTypeDef",
+    "StartIncidentOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeletionProtectionInputRequestTypeDef",
     "ConditionTypeDef",
     "CreateReplicationSetInputRequestTypeDef",
-    "CreateReplicationSetOutputTypeDef",
-    "CreateResponsePlanOutputTypeDef",
-    "CreateTimelineEventOutputTypeDef",
-    "ListReplicationSetsOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutResourcePolicyOutputTypeDef",
-    "StartIncidentOutputTypeDef",
     "CreateTimelineEventInputRequestTypeDef",
     "EventSummaryTypeDef",
     "TimelineEventTypeDef",
     "UpdateTimelineEventInputRequestTypeDef",
     "UpdateReplicationSetActionTypeDef",
     "SsmAutomationTypeDef",
     "GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     "GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
-    "GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
-    "ListRelatedItemsInputListRelatedItemsPaginateTypeDef",
-    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
-    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
     "GetResourcePoliciesOutputTypeDef",
     "IncidentRecordSummaryTypeDef",
     "IncidentRecordTypeDef",
     "IncidentTemplateTypeDef",
     "UpdateIncidentRecordInputRequestTypeDef",
-    "ItemIdentifierTypeDef",
+    "ItemValueTypeDef",
     "ListResponsePlansOutputTypeDef",
+    "PagerDutyConfigurationTypeDef",
     "ReplicationSetTypeDef",
     "FilterTypeDef",
     "ListTimelineEventsOutputTypeDef",
     "GetTimelineEventOutputTypeDef",
     "UpdateReplicationSetInputRequestTypeDef",
     "ActionTypeDef",
     "ListIncidentRecordsOutputTypeDef",
     "GetIncidentRecordOutputTypeDef",
-    "RelatedItemTypeDef",
+    "ItemIdentifierTypeDef",
+    "IntegrationTypeDef",
     "GetReplicationSetOutputTypeDef",
     "ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef",
     "ListIncidentRecordsInputRequestTypeDef",
     "ListTimelineEventsInputListTimelineEventsPaginateTypeDef",
     "ListTimelineEventsInputRequestTypeDef",
+    "RelatedItemTypeDef",
     "CreateResponsePlanInputRequestTypeDef",
     "GetResponsePlanOutputTypeDef",
     "UpdateResponsePlanInputRequestTypeDef",
     "ListRelatedItemsOutputTypeDef",
     "RelatedItemsUpdateTypeDef",
     "StartIncidentInputRequestTypeDef",
     "UpdateRelatedItemsInputRequestTypeDef",
@@ -172,34 +176,48 @@
     "RegionMapInputValueTypeDef",
     {
         "sseKmsKeyId": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateReplicationSetOutputTypeDef = TypedDict(
+    "CreateReplicationSetOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateResponsePlanOutputTypeDef = TypedDict(
+    "CreateResponsePlanOutputTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventReferenceTypeDef = TypedDict(
     "EventReferenceTypeDef",
     {
         "relatedItemId": str,
         "resource": str,
     },
     total=False,
 )
 
+CreateTimelineEventOutputTypeDef = TypedDict(
+    "CreateTimelineEventOutputTypeDef",
+    {
+        "eventId": str,
+        "incidentRecordArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteIncidentRecordInputRequestTypeDef = TypedDict(
     "DeleteIncidentRecordInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -267,24 +285,36 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "resourceArn": str,
+    },
+)
+_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef(
+    _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
+    _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetResourcePoliciesInputRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesInputRequestTypeDef = TypedDict(
@@ -354,24 +384,58 @@
     "NotificationTargetItemTypeDef",
     {
         "snsTopicArn": str,
     },
     total=False,
 )
 
-ItemValueTypeDef = TypedDict(
-    "ItemValueTypeDef",
+_RequiredPagerDutyIncidentDetailTypeDef = TypedDict(
+    "_RequiredPagerDutyIncidentDetailTypeDef",
     {
-        "arn": str,
-        "metricDefinition": str,
-        "url": str,
+        "id": str,
+    },
+)
+_OptionalPagerDutyIncidentDetailTypeDef = TypedDict(
+    "_OptionalPagerDutyIncidentDetailTypeDef",
+    {
+        "autoResolve": bool,
+        "secretId": str,
+    },
+    total=False,
+)
+
+
+class PagerDutyIncidentDetailTypeDef(
+    _RequiredPagerDutyIncidentDetailTypeDef, _OptionalPagerDutyIncidentDetailTypeDef
+):
+    pass
+
+
+_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
+    "_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef",
+    {
+        "incidentRecordArn": str,
+    },
+)
+_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
+    "_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListRelatedItemsInputListRelatedItemsPaginateTypeDef(
+    _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef,
+    _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListRelatedItemsInputRequestTypeDef = TypedDict(
     "_RequiredListRelatedItemsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListRelatedItemsInputRequestTypeDef = TypedDict(
@@ -386,23 +450,48 @@
 
 class ListRelatedItemsInputRequestTypeDef(
     _RequiredListRelatedItemsInputRequestTypeDef, _OptionalListRelatedItemsInputRequestTypeDef
 ):
     pass
 
 
+ListReplicationSetsInputListReplicationSetsPaginateTypeDef = TypedDict(
+    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReplicationSetsInputRequestTypeDef = TypedDict(
     "ListReplicationSetsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListReplicationSetsOutputTypeDef = TypedDict(
+    "ListReplicationSetsOutputTypeDef",
+    {
+        "nextToken": str,
+        "replicationSetArns": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListResponsePlansInputListResponsePlansPaginateTypeDef = TypedDict(
+    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListResponsePlansInputRequestTypeDef = TypedDict(
     "ListResponsePlansInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -433,22 +522,55 @@
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
+PagerDutyIncidentConfigurationTypeDef = TypedDict(
+    "PagerDutyIncidentConfigurationTypeDef",
+    {
+        "serviceId": str,
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
 PutResourcePolicyInputRequestTypeDef = TypedDict(
     "PutResourcePolicyInputRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
     },
 )
 
+PutResourcePolicyOutputTypeDef = TypedDict(
+    "PutResourcePolicyOutputTypeDef",
+    {
+        "policyId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRegionInfoTypeDef = TypedDict(
     "_RequiredRegionInfoTypeDef",
     {
         "status": RegionStatusType,
         "statusUpdateDateTime": datetime,
     },
 )
@@ -462,14 +584,25 @@
 )
 
 
 class RegionInfoTypeDef(_RequiredRegionInfoTypeDef, _OptionalRegionInfoTypeDef):
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
 _RequiredTriggerDetailsTypeDef = TypedDict(
     "_RequiredTriggerDetailsTypeDef",
     {
         "source": str,
         "timestamp": Union[datetime, str],
     },
 )
@@ -483,14 +616,22 @@
 )
 
 
 class TriggerDetailsTypeDef(_RequiredTriggerDetailsTypeDef, _OptionalTriggerDetailsTypeDef):
     pass
 
 
+StartIncidentOutputTypeDef = TypedDict(
+    "StartIncidentOutputTypeDef",
+    {
+        "incidentRecordArn": str,
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
@@ -555,72 +696,14 @@
 class CreateReplicationSetInputRequestTypeDef(
     _RequiredCreateReplicationSetInputRequestTypeDef,
     _OptionalCreateReplicationSetInputRequestTypeDef,
 ):
     pass
 
 
-CreateReplicationSetOutputTypeDef = TypedDict(
-    "CreateReplicationSetOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateResponsePlanOutputTypeDef = TypedDict(
-    "CreateResponsePlanOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTimelineEventOutputTypeDef = TypedDict(
-    "CreateTimelineEventOutputTypeDef",
-    {
-        "eventId": str,
-        "incidentRecordArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListReplicationSetsOutputTypeDef = TypedDict(
-    "ListReplicationSetsOutputTypeDef",
-    {
-        "nextToken": str,
-        "replicationSetArns": List[str],
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
-PutResourcePolicyOutputTypeDef = TypedDict(
-    "PutResourcePolicyOutputTypeDef",
-    {
-        "policyId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartIncidentOutputTypeDef = TypedDict(
-    "StartIncidentOutputTypeDef",
-    {
-        "incidentRecordArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateTimelineEventInputRequestTypeDef = TypedDict(
     "_RequiredCreateTimelineEventInputRequestTypeDef",
     {
         "eventData": str,
         "eventTime": Union[datetime, str],
         "eventType": str,
         "incidentRecordArn": str,
@@ -787,80 +870,20 @@
 class GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef(
     _RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
     _OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
 ):
     pass
 
 
-_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef(
-    _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
-    _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
-    "_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef",
-    {
-        "incidentRecordArn": str,
-    },
-)
-_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
-    "_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListRelatedItemsInputListRelatedItemsPaginateTypeDef(
-    _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef,
-    _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef,
-):
-    pass
-
-
-ListReplicationSetsInputListReplicationSetsPaginateTypeDef = TypedDict(
-    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListResponsePlansInputListResponsePlansPaginateTypeDef = TypedDict(
-    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 GetResourcePoliciesOutputTypeDef = TypedDict(
     "GetResourcePoliciesOutputTypeDef",
     {
         "nextToken": str,
         "resourcePolicies": List[ResourcePolicyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredIncidentRecordSummaryTypeDef = TypedDict(
     "_RequiredIncidentRecordSummaryTypeDef",
     {
         "arn": str,
@@ -964,28 +987,40 @@
 class UpdateIncidentRecordInputRequestTypeDef(
     _RequiredUpdateIncidentRecordInputRequestTypeDef,
     _OptionalUpdateIncidentRecordInputRequestTypeDef,
 ):
     pass
 
 
-ItemIdentifierTypeDef = TypedDict(
-    "ItemIdentifierTypeDef",
+ItemValueTypeDef = TypedDict(
+    "ItemValueTypeDef",
     {
-        "type": ItemTypeType,
-        "value": ItemValueTypeDef,
+        "arn": str,
+        "metricDefinition": str,
+        "pagerDutyIncidentDetail": PagerDutyIncidentDetailTypeDef,
+        "url": str,
     },
+    total=False,
 )
 
 ListResponsePlansOutputTypeDef = TypedDict(
     "ListResponsePlansOutputTypeDef",
     {
         "nextToken": str,
         "responsePlanSummaries": List[ResponsePlanSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PagerDutyConfigurationTypeDef = TypedDict(
+    "PagerDutyConfigurationTypeDef",
+    {
+        "name": str,
+        "pagerDutyIncidentConfiguration": PagerDutyIncidentConfigurationTypeDef,
+        "secretId": str,
     },
 )
 
 _RequiredReplicationSetTypeDef = TypedDict(
     "_RequiredReplicationSetTypeDef",
     {
         "createdBy": str,
@@ -1019,23 +1054,23 @@
 )
 
 ListTimelineEventsOutputTypeDef = TypedDict(
     "ListTimelineEventsOutputTypeDef",
     {
         "eventSummaries": List[EventSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTimelineEventOutputTypeDef = TypedDict(
     "GetTimelineEventOutputTypeDef",
     {
         "event": TimelineEventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateReplicationSetInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationSetInputRequestTypeDef",
     {
         "actions": Sequence[UpdateReplicationSetActionTypeDef],
@@ -1067,59 +1102,55 @@
 )
 
 ListIncidentRecordsOutputTypeDef = TypedDict(
     "ListIncidentRecordsOutputTypeDef",
     {
         "incidentRecordSummaries": List[IncidentRecordSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIncidentRecordOutputTypeDef = TypedDict(
     "GetIncidentRecordOutputTypeDef",
     {
         "incidentRecord": IncidentRecordTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredRelatedItemTypeDef = TypedDict(
-    "_RequiredRelatedItemTypeDef",
+ItemIdentifierTypeDef = TypedDict(
+    "ItemIdentifierTypeDef",
     {
-        "identifier": ItemIdentifierTypeDef,
+        "type": ItemTypeType,
+        "value": ItemValueTypeDef,
     },
 )
-_OptionalRelatedItemTypeDef = TypedDict(
-    "_OptionalRelatedItemTypeDef",
+
+IntegrationTypeDef = TypedDict(
+    "IntegrationTypeDef",
     {
-        "generatedId": str,
-        "title": str,
+        "pagerDutyConfiguration": PagerDutyConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class RelatedItemTypeDef(_RequiredRelatedItemTypeDef, _OptionalRelatedItemTypeDef):
-    pass
-
-
 GetReplicationSetOutputTypeDef = TypedDict(
     "GetReplicationSetOutputTypeDef",
     {
         "replicationSet": ReplicationSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef = TypedDict(
     "ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListIncidentRecordsInputRequestTypeDef = TypedDict(
     "ListIncidentRecordsInputRequestTypeDef",
     {
@@ -1138,15 +1169,15 @@
 )
 _OptionalListTimelineEventsInputListTimelineEventsPaginateTypeDef = TypedDict(
     "_OptionalListTimelineEventsInputListTimelineEventsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
         "sortBy": Literal["EVENT_TIME"],
         "sortOrder": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListTimelineEventsInputListTimelineEventsPaginateTypeDef(
     _RequiredListTimelineEventsInputListTimelineEventsPaginateTypeDef,
@@ -1176,14 +1207,34 @@
 
 class ListTimelineEventsInputRequestTypeDef(
     _RequiredListTimelineEventsInputRequestTypeDef, _OptionalListTimelineEventsInputRequestTypeDef
 ):
     pass
 
 
+_RequiredRelatedItemTypeDef = TypedDict(
+    "_RequiredRelatedItemTypeDef",
+    {
+        "identifier": ItemIdentifierTypeDef,
+    },
+)
+_OptionalRelatedItemTypeDef = TypedDict(
+    "_OptionalRelatedItemTypeDef",
+    {
+        "generatedId": str,
+        "title": str,
+    },
+    total=False,
+)
+
+
+class RelatedItemTypeDef(_RequiredRelatedItemTypeDef, _OptionalRelatedItemTypeDef):
+    pass
+
+
 _RequiredCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateResponsePlanInputRequestTypeDef",
     {
         "incidentTemplate": IncidentTemplateTypeDef,
         "name": str,
     },
 )
@@ -1191,14 +1242,15 @@
     "_OptionalCreateResponsePlanInputRequestTypeDef",
     {
         "actions": Sequence[ActionTypeDef],
         "chatChannel": ChatChannelTypeDef,
         "clientToken": str,
         "displayName": str,
         "engagements": Sequence[str],
+        "integrations": Sequence[IntegrationTypeDef],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class CreateResponsePlanInputRequestTypeDef(
@@ -1212,16 +1264,17 @@
     {
         "actions": List[ActionTypeDef],
         "arn": str,
         "chatChannel": ChatChannelTypeDef,
         "displayName": str,
         "engagements": List[str],
         "incidentTemplate": IncidentTemplateTypeDef,
+        "integrations": List[IntegrationTypeDef],
         "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResponsePlanInputRequestTypeDef",
     {
         "arn": str,
@@ -1237,14 +1290,15 @@
         "engagements": Sequence[str],
         "incidentTemplateDedupeString": str,
         "incidentTemplateImpact": int,
         "incidentTemplateNotificationTargets": Sequence[NotificationTargetItemTypeDef],
         "incidentTemplateSummary": str,
         "incidentTemplateTags": Mapping[str, str],
         "incidentTemplateTitle": str,
+        "integrations": Sequence[IntegrationTypeDef],
     },
     total=False,
 )
 
 
 class UpdateResponsePlanInputRequestTypeDef(
     _RequiredUpdateResponsePlanInputRequestTypeDef, _OptionalUpdateResponsePlanInputRequestTypeDef
@@ -1253,15 +1307,15 @@
 
 
 ListRelatedItemsOutputTypeDef = TypedDict(
     "ListRelatedItemsOutputTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[RelatedItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RelatedItemsUpdateTypeDef = TypedDict(
     "RelatedItemsUpdateTypeDef",
     {
         "itemToAdd": RelatedItemTypeDef,
```

### Comparing `mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/type_defs.pyi` & `mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -36,87 +36,91 @@
 
 __all__ = (
     "AddRegionActionTypeDef",
     "AttributeValueListTypeDef",
     "AutomationExecutionTypeDef",
     "ChatChannelTypeDef",
     "RegionMapInputValueTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateReplicationSetOutputTypeDef",
+    "CreateResponsePlanOutputTypeDef",
     "EventReferenceTypeDef",
+    "CreateTimelineEventOutputTypeDef",
     "DeleteIncidentRecordInputRequestTypeDef",
     "DeleteRegionActionTypeDef",
     "DeleteReplicationSetInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteResponsePlanInputRequestTypeDef",
     "DeleteTimelineEventInputRequestTypeDef",
     "DynamicSsmParameterValueTypeDef",
     "GetIncidentRecordInputRequestTypeDef",
     "GetReplicationSetInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     "GetResourcePoliciesInputRequestTypeDef",
     "ResourcePolicyTypeDef",
     "GetResponsePlanInputRequestTypeDef",
     "GetTimelineEventInputRequestTypeDef",
     "IncidentRecordSourceTypeDef",
     "NotificationTargetItemTypeDef",
-    "ItemValueTypeDef",
+    "PagerDutyIncidentDetailTypeDef",
+    "ListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     "ListRelatedItemsInputRequestTypeDef",
+    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
     "ListReplicationSetsInputRequestTypeDef",
+    "ListReplicationSetsOutputTypeDef",
+    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
     "ListResponsePlansInputRequestTypeDef",
     "ResponsePlanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PagerDutyIncidentConfigurationTypeDef",
+    "PaginatorConfigTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
+    "PutResourcePolicyOutputTypeDef",
     "RegionInfoTypeDef",
+    "ResponseMetadataTypeDef",
     "TriggerDetailsTypeDef",
+    "StartIncidentOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeletionProtectionInputRequestTypeDef",
     "ConditionTypeDef",
     "CreateReplicationSetInputRequestTypeDef",
-    "CreateReplicationSetOutputTypeDef",
-    "CreateResponsePlanOutputTypeDef",
-    "CreateTimelineEventOutputTypeDef",
-    "ListReplicationSetsOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutResourcePolicyOutputTypeDef",
-    "StartIncidentOutputTypeDef",
     "CreateTimelineEventInputRequestTypeDef",
     "EventSummaryTypeDef",
     "TimelineEventTypeDef",
     "UpdateTimelineEventInputRequestTypeDef",
     "UpdateReplicationSetActionTypeDef",
     "SsmAutomationTypeDef",
     "GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     "GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
-    "GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
-    "ListRelatedItemsInputListRelatedItemsPaginateTypeDef",
-    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
-    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
     "GetResourcePoliciesOutputTypeDef",
     "IncidentRecordSummaryTypeDef",
     "IncidentRecordTypeDef",
     "IncidentTemplateTypeDef",
     "UpdateIncidentRecordInputRequestTypeDef",
-    "ItemIdentifierTypeDef",
+    "ItemValueTypeDef",
     "ListResponsePlansOutputTypeDef",
+    "PagerDutyConfigurationTypeDef",
     "ReplicationSetTypeDef",
     "FilterTypeDef",
     "ListTimelineEventsOutputTypeDef",
     "GetTimelineEventOutputTypeDef",
     "UpdateReplicationSetInputRequestTypeDef",
     "ActionTypeDef",
     "ListIncidentRecordsOutputTypeDef",
     "GetIncidentRecordOutputTypeDef",
-    "RelatedItemTypeDef",
+    "ItemIdentifierTypeDef",
+    "IntegrationTypeDef",
     "GetReplicationSetOutputTypeDef",
     "ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef",
     "ListIncidentRecordsInputRequestTypeDef",
     "ListTimelineEventsInputListTimelineEventsPaginateTypeDef",
     "ListTimelineEventsInputRequestTypeDef",
+    "RelatedItemTypeDef",
     "CreateResponsePlanInputRequestTypeDef",
     "GetResponsePlanOutputTypeDef",
     "UpdateResponsePlanInputRequestTypeDef",
     "ListRelatedItemsOutputTypeDef",
     "RelatedItemsUpdateTypeDef",
     "StartIncidentInputRequestTypeDef",
     "UpdateRelatedItemsInputRequestTypeDef",
@@ -169,34 +173,48 @@
     "RegionMapInputValueTypeDef",
     {
         "sseKmsKeyId": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateReplicationSetOutputTypeDef = TypedDict(
+    "CreateReplicationSetOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateResponsePlanOutputTypeDef = TypedDict(
+    "CreateResponsePlanOutputTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventReferenceTypeDef = TypedDict(
     "EventReferenceTypeDef",
     {
         "relatedItemId": str,
         "resource": str,
     },
     total=False,
 )
 
+CreateTimelineEventOutputTypeDef = TypedDict(
+    "CreateTimelineEventOutputTypeDef",
+    {
+        "eventId": str,
+        "incidentRecordArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteIncidentRecordInputRequestTypeDef = TypedDict(
     "DeleteIncidentRecordInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -264,24 +282,34 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "resourceArn": str,
+    },
+)
+_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef(
+    _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
+    _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
+):
+    pass
+
 _RequiredGetResourcePoliciesInputRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesInputRequestTypeDef = TypedDict(
@@ -347,24 +375,54 @@
     "NotificationTargetItemTypeDef",
     {
         "snsTopicArn": str,
     },
     total=False,
 )
 
-ItemValueTypeDef = TypedDict(
-    "ItemValueTypeDef",
+_RequiredPagerDutyIncidentDetailTypeDef = TypedDict(
+    "_RequiredPagerDutyIncidentDetailTypeDef",
     {
-        "arn": str,
-        "metricDefinition": str,
-        "url": str,
+        "id": str,
+    },
+)
+_OptionalPagerDutyIncidentDetailTypeDef = TypedDict(
+    "_OptionalPagerDutyIncidentDetailTypeDef",
+    {
+        "autoResolve": bool,
+        "secretId": str,
     },
     total=False,
 )
 
+class PagerDutyIncidentDetailTypeDef(
+    _RequiredPagerDutyIncidentDetailTypeDef, _OptionalPagerDutyIncidentDetailTypeDef
+):
+    pass
+
+_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
+    "_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef",
+    {
+        "incidentRecordArn": str,
+    },
+)
+_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
+    "_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListRelatedItemsInputListRelatedItemsPaginateTypeDef(
+    _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef,
+    _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef,
+):
+    pass
+
 _RequiredListRelatedItemsInputRequestTypeDef = TypedDict(
     "_RequiredListRelatedItemsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListRelatedItemsInputRequestTypeDef = TypedDict(
@@ -377,23 +435,48 @@
 )
 
 class ListRelatedItemsInputRequestTypeDef(
     _RequiredListRelatedItemsInputRequestTypeDef, _OptionalListRelatedItemsInputRequestTypeDef
 ):
     pass
 
+ListReplicationSetsInputListReplicationSetsPaginateTypeDef = TypedDict(
+    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListReplicationSetsInputRequestTypeDef = TypedDict(
     "ListReplicationSetsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListReplicationSetsOutputTypeDef = TypedDict(
+    "ListReplicationSetsOutputTypeDef",
+    {
+        "nextToken": str,
+        "replicationSetArns": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListResponsePlansInputListResponsePlansPaginateTypeDef = TypedDict(
+    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListResponsePlansInputRequestTypeDef = TypedDict(
     "ListResponsePlansInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -422,22 +505,55 @@
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
+PagerDutyIncidentConfigurationTypeDef = TypedDict(
+    "PagerDutyIncidentConfigurationTypeDef",
+    {
+        "serviceId": str,
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
 PutResourcePolicyInputRequestTypeDef = TypedDict(
     "PutResourcePolicyInputRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
     },
 )
 
+PutResourcePolicyOutputTypeDef = TypedDict(
+    "PutResourcePolicyOutputTypeDef",
+    {
+        "policyId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRegionInfoTypeDef = TypedDict(
     "_RequiredRegionInfoTypeDef",
     {
         "status": RegionStatusType,
         "statusUpdateDateTime": datetime,
     },
 )
@@ -449,14 +565,25 @@
     },
     total=False,
 )
 
 class RegionInfoTypeDef(_RequiredRegionInfoTypeDef, _OptionalRegionInfoTypeDef):
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
 _RequiredTriggerDetailsTypeDef = TypedDict(
     "_RequiredTriggerDetailsTypeDef",
     {
         "source": str,
         "timestamp": Union[datetime, str],
     },
 )
@@ -468,14 +595,22 @@
     },
     total=False,
 )
 
 class TriggerDetailsTypeDef(_RequiredTriggerDetailsTypeDef, _OptionalTriggerDetailsTypeDef):
     pass
 
+StartIncidentOutputTypeDef = TypedDict(
+    "StartIncidentOutputTypeDef",
+    {
+        "incidentRecordArn": str,
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
@@ -536,72 +671,14 @@
 
 class CreateReplicationSetInputRequestTypeDef(
     _RequiredCreateReplicationSetInputRequestTypeDef,
     _OptionalCreateReplicationSetInputRequestTypeDef,
 ):
     pass
 
-CreateReplicationSetOutputTypeDef = TypedDict(
-    "CreateReplicationSetOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateResponsePlanOutputTypeDef = TypedDict(
-    "CreateResponsePlanOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTimelineEventOutputTypeDef = TypedDict(
-    "CreateTimelineEventOutputTypeDef",
-    {
-        "eventId": str,
-        "incidentRecordArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListReplicationSetsOutputTypeDef = TypedDict(
-    "ListReplicationSetsOutputTypeDef",
-    {
-        "nextToken": str,
-        "replicationSetArns": List[str],
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
-PutResourcePolicyOutputTypeDef = TypedDict(
-    "PutResourcePolicyOutputTypeDef",
-    {
-        "policyId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartIncidentOutputTypeDef = TypedDict(
-    "StartIncidentOutputTypeDef",
-    {
-        "incidentRecordArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateTimelineEventInputRequestTypeDef = TypedDict(
     "_RequiredCreateTimelineEventInputRequestTypeDef",
     {
         "eventData": str,
         "eventTime": Union[datetime, str],
         "eventType": str,
         "incidentRecordArn": str,
@@ -754,76 +831,20 @@
 
 class GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef(
     _RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
     _OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
 ):
     pass
 
-_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef(
-    _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
-    _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
-):
-    pass
-
-_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
-    "_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef",
-    {
-        "incidentRecordArn": str,
-    },
-)
-_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
-    "_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListRelatedItemsInputListRelatedItemsPaginateTypeDef(
-    _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef,
-    _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef,
-):
-    pass
-
-ListReplicationSetsInputListReplicationSetsPaginateTypeDef = TypedDict(
-    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListResponsePlansInputListResponsePlansPaginateTypeDef = TypedDict(
-    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 GetResourcePoliciesOutputTypeDef = TypedDict(
     "GetResourcePoliciesOutputTypeDef",
     {
         "nextToken": str,
         "resourcePolicies": List[ResourcePolicyTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredIncidentRecordSummaryTypeDef = TypedDict(
     "_RequiredIncidentRecordSummaryTypeDef",
     {
         "arn": str,
@@ -919,28 +940,40 @@
 
 class UpdateIncidentRecordInputRequestTypeDef(
     _RequiredUpdateIncidentRecordInputRequestTypeDef,
     _OptionalUpdateIncidentRecordInputRequestTypeDef,
 ):
     pass
 
-ItemIdentifierTypeDef = TypedDict(
-    "ItemIdentifierTypeDef",
+ItemValueTypeDef = TypedDict(
+    "ItemValueTypeDef",
     {
-        "type": ItemTypeType,
-        "value": ItemValueTypeDef,
+        "arn": str,
+        "metricDefinition": str,
+        "pagerDutyIncidentDetail": PagerDutyIncidentDetailTypeDef,
+        "url": str,
     },
+    total=False,
 )
 
 ListResponsePlansOutputTypeDef = TypedDict(
     "ListResponsePlansOutputTypeDef",
     {
         "nextToken": str,
         "responsePlanSummaries": List[ResponsePlanSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PagerDutyConfigurationTypeDef = TypedDict(
+    "PagerDutyConfigurationTypeDef",
+    {
+        "name": str,
+        "pagerDutyIncidentConfiguration": PagerDutyIncidentConfigurationTypeDef,
+        "secretId": str,
     },
 )
 
 _RequiredReplicationSetTypeDef = TypedDict(
     "_RequiredReplicationSetTypeDef",
     {
         "createdBy": str,
@@ -972,23 +1005,23 @@
 )
 
 ListTimelineEventsOutputTypeDef = TypedDict(
     "ListTimelineEventsOutputTypeDef",
     {
         "eventSummaries": List[EventSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTimelineEventOutputTypeDef = TypedDict(
     "GetTimelineEventOutputTypeDef",
     {
         "event": TimelineEventTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateReplicationSetInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationSetInputRequestTypeDef",
     {
         "actions": Sequence[UpdateReplicationSetActionTypeDef],
@@ -1018,57 +1051,55 @@
 )
 
 ListIncidentRecordsOutputTypeDef = TypedDict(
     "ListIncidentRecordsOutputTypeDef",
     {
         "incidentRecordSummaries": List[IncidentRecordSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetIncidentRecordOutputTypeDef = TypedDict(
     "GetIncidentRecordOutputTypeDef",
     {
         "incidentRecord": IncidentRecordTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredRelatedItemTypeDef = TypedDict(
-    "_RequiredRelatedItemTypeDef",
+ItemIdentifierTypeDef = TypedDict(
+    "ItemIdentifierTypeDef",
     {
-        "identifier": ItemIdentifierTypeDef,
+        "type": ItemTypeType,
+        "value": ItemValueTypeDef,
     },
 )
-_OptionalRelatedItemTypeDef = TypedDict(
-    "_OptionalRelatedItemTypeDef",
+
+IntegrationTypeDef = TypedDict(
+    "IntegrationTypeDef",
     {
-        "generatedId": str,
-        "title": str,
+        "pagerDutyConfiguration": PagerDutyConfigurationTypeDef,
     },
     total=False,
 )
 
-class RelatedItemTypeDef(_RequiredRelatedItemTypeDef, _OptionalRelatedItemTypeDef):
-    pass
-
 GetReplicationSetOutputTypeDef = TypedDict(
     "GetReplicationSetOutputTypeDef",
     {
         "replicationSet": ReplicationSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef = TypedDict(
     "ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListIncidentRecordsInputRequestTypeDef = TypedDict(
     "ListIncidentRecordsInputRequestTypeDef",
     {
@@ -1087,15 +1118,15 @@
 )
 _OptionalListTimelineEventsInputListTimelineEventsPaginateTypeDef = TypedDict(
     "_OptionalListTimelineEventsInputListTimelineEventsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
         "sortBy": Literal["EVENT_TIME"],
         "sortOrder": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListTimelineEventsInputListTimelineEventsPaginateTypeDef(
     _RequiredListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     _OptionalListTimelineEventsInputListTimelineEventsPaginateTypeDef,
@@ -1121,14 +1152,32 @@
 )
 
 class ListTimelineEventsInputRequestTypeDef(
     _RequiredListTimelineEventsInputRequestTypeDef, _OptionalListTimelineEventsInputRequestTypeDef
 ):
     pass
 
+_RequiredRelatedItemTypeDef = TypedDict(
+    "_RequiredRelatedItemTypeDef",
+    {
+        "identifier": ItemIdentifierTypeDef,
+    },
+)
+_OptionalRelatedItemTypeDef = TypedDict(
+    "_OptionalRelatedItemTypeDef",
+    {
+        "generatedId": str,
+        "title": str,
+    },
+    total=False,
+)
+
+class RelatedItemTypeDef(_RequiredRelatedItemTypeDef, _OptionalRelatedItemTypeDef):
+    pass
+
 _RequiredCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateResponsePlanInputRequestTypeDef",
     {
         "incidentTemplate": IncidentTemplateTypeDef,
         "name": str,
     },
 )
@@ -1136,14 +1185,15 @@
     "_OptionalCreateResponsePlanInputRequestTypeDef",
     {
         "actions": Sequence[ActionTypeDef],
         "chatChannel": ChatChannelTypeDef,
         "clientToken": str,
         "displayName": str,
         "engagements": Sequence[str],
+        "integrations": Sequence[IntegrationTypeDef],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateResponsePlanInputRequestTypeDef(
     _RequiredCreateResponsePlanInputRequestTypeDef, _OptionalCreateResponsePlanInputRequestTypeDef
@@ -1155,16 +1205,17 @@
     {
         "actions": List[ActionTypeDef],
         "arn": str,
         "chatChannel": ChatChannelTypeDef,
         "displayName": str,
         "engagements": List[str],
         "incidentTemplate": IncidentTemplateTypeDef,
+        "integrations": List[IntegrationTypeDef],
         "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResponsePlanInputRequestTypeDef",
     {
         "arn": str,
@@ -1180,29 +1231,30 @@
         "engagements": Sequence[str],
         "incidentTemplateDedupeString": str,
         "incidentTemplateImpact": int,
         "incidentTemplateNotificationTargets": Sequence[NotificationTargetItemTypeDef],
         "incidentTemplateSummary": str,
         "incidentTemplateTags": Mapping[str, str],
         "incidentTemplateTitle": str,
+        "integrations": Sequence[IntegrationTypeDef],
     },
     total=False,
 )
 
 class UpdateResponsePlanInputRequestTypeDef(
     _RequiredUpdateResponsePlanInputRequestTypeDef, _OptionalUpdateResponsePlanInputRequestTypeDef
 ):
     pass
 
 ListRelatedItemsOutputTypeDef = TypedDict(
     "ListRelatedItemsOutputTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[RelatedItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RelatedItemsUpdateTypeDef = TypedDict(
     "RelatedItemsUpdateTypeDef",
     {
         "itemToAdd": RelatedItemTypeDef,
```

### Comparing `mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/waiter.py` & `mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents/waiter.pyi` & `mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents.egg-info/PKG-INFO` & `mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-incidents
-Version: 1.26.8
-Summary: Type annotations for boto3.SSMIncidents 1.26.8 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.SSMIncidents 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/
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
 
 <a id="mypy-boto3-ssm-incidents"></a>
 
 # mypy-boto3-ssm-incidents
 
 [![PyPI - mypy-boto3-ssm-incidents](https://img.shields.io/pypi/v/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-incidents?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMIncidents 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[boto3.SSMIncidents 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
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
 [mypy-boto3-ssm-incidents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,87 +391,91 @@
 ```python
 from mypy_boto3_ssm_incidents.type_defs import (
     AddRegionActionTypeDef,
     AttributeValueListTypeDef,
     AutomationExecutionTypeDef,
     ChatChannelTypeDef,
     RegionMapInputValueTypeDef,
-    ResponseMetadataTypeDef,
+    CreateReplicationSetOutputTypeDef,
+    CreateResponsePlanOutputTypeDef,
     EventReferenceTypeDef,
+    CreateTimelineEventOutputTypeDef,
     DeleteIncidentRecordInputRequestTypeDef,
     DeleteRegionActionTypeDef,
     DeleteReplicationSetInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteResponsePlanInputRequestTypeDef,
     DeleteTimelineEventInputRequestTypeDef,
     DynamicSsmParameterValueTypeDef,
     GetIncidentRecordInputRequestTypeDef,
     GetReplicationSetInputRequestTypeDef,
     WaiterConfigTypeDef,
-    PaginatorConfigTypeDef,
+    GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
     GetResourcePoliciesInputRequestTypeDef,
     ResourcePolicyTypeDef,
     GetResponsePlanInputRequestTypeDef,
     GetTimelineEventInputRequestTypeDef,
     IncidentRecordSourceTypeDef,
     NotificationTargetItemTypeDef,
-    ItemValueTypeDef,
+    PagerDutyIncidentDetailTypeDef,
+    ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
     ListRelatedItemsInputRequestTypeDef,
+    ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
     ListReplicationSetsInputRequestTypeDef,
+    ListReplicationSetsOutputTypeDef,
+    ListResponsePlansInputListResponsePlansPaginateTypeDef,
     ListResponsePlansInputRequestTypeDef,
     ResponsePlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PagerDutyIncidentConfigurationTypeDef,
+    PaginatorConfigTypeDef,
     PutResourcePolicyInputRequestTypeDef,
+    PutResourcePolicyOutputTypeDef,
     RegionInfoTypeDef,
+    ResponseMetadataTypeDef,
     TriggerDetailsTypeDef,
+    StartIncidentOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeletionProtectionInputRequestTypeDef,
     ConditionTypeDef,
     CreateReplicationSetInputRequestTypeDef,
-    CreateReplicationSetOutputTypeDef,
-    CreateResponsePlanOutputTypeDef,
-    CreateTimelineEventOutputTypeDef,
-    ListReplicationSetsOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutResourcePolicyOutputTypeDef,
-    StartIncidentOutputTypeDef,
     CreateTimelineEventInputRequestTypeDef,
     EventSummaryTypeDef,
     TimelineEventTypeDef,
     UpdateTimelineEventInputRequestTypeDef,
     UpdateReplicationSetActionTypeDef,
     SsmAutomationTypeDef,
     GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
     GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
-    GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
-    ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
-    ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
-    ListResponsePlansInputListResponsePlansPaginateTypeDef,
     GetResourcePoliciesOutputTypeDef,
     IncidentRecordSummaryTypeDef,
     IncidentRecordTypeDef,
     IncidentTemplateTypeDef,
     UpdateIncidentRecordInputRequestTypeDef,
-    ItemIdentifierTypeDef,
+    ItemValueTypeDef,
     ListResponsePlansOutputTypeDef,
+    PagerDutyConfigurationTypeDef,
     ReplicationSetTypeDef,
     FilterTypeDef,
     ListTimelineEventsOutputTypeDef,
     GetTimelineEventOutputTypeDef,
     UpdateReplicationSetInputRequestTypeDef,
     ActionTypeDef,
     ListIncidentRecordsOutputTypeDef,
     GetIncidentRecordOutputTypeDef,
-    RelatedItemTypeDef,
+    ItemIdentifierTypeDef,
+    IntegrationTypeDef,
     GetReplicationSetOutputTypeDef,
     ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef,
     ListIncidentRecordsInputRequestTypeDef,
     ListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     ListTimelineEventsInputRequestTypeDef,
+    RelatedItemTypeDef,
     CreateResponsePlanInputRequestTypeDef,
     GetResponsePlanOutputTypeDef,
     UpdateResponsePlanInputRequestTypeDef,
     ListRelatedItemsOutputTypeDef,
     RelatedItemsUpdateTypeDef,
     StartIncidentInputRequestTypeDef,
     UpdateRelatedItemsInputRequestTypeDef,
@@ -484,42 +489,42 @@
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

### Comparing `mypy-boto3-ssm-incidents-1.26.8/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt` & `mypy-boto3-ssm-incidents-1.27.0/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.26.8/setup.py` & `mypy-boto3-ssm-incidents-1.27.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-ssm-incidents.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm-incidents",
-    version="1.26.8",
+    version="1.27.0",
     packages=["mypy_boto3_ssm_incidents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSMIncidents 1.26.8 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.SSMIncidents 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
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
     keywords="boto3 ssm-incidents type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_ssm_incidents": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_ssm_incidents": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/",
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


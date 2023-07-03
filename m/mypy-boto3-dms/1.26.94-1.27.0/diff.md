# Comparing `tmp/mypy-boto3-dms-1.26.94.tar.gz` & `tmp/mypy-boto3-dms-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dms-1.26.94.tar", last modified: Fri Mar 17 19:32:19 2023, max compression
+gzip compressed data, was "mypy-boto3-dms-1.27.0.tar", last modified: Mon Jul  3 19:50:40 2023, max compression
```

## Comparing `mypy-boto3-dms-1.26.94.tar` & `mypy-boto3-dms-1.27.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:32:19.877378 mypy-boto3-dms-1.26.94/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-17 19:32:05.000000 mypy-boto3-dms-1.26.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28357 2023-03-17 19:32:19.877378 mypy-boto3-dms-1.26.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26865 2023-03-17 19:32:05.000000 mypy-boto3-dms-1.26.94/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:32:19.873377 mypy-boto3-dms-1.26.94/mypy_boto3_dms/
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-03-17 19:32:05.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-03-17 19:32:05.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-17 19:32:05.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66105 2023-03-17 19:32:06.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    66008 2023-03-17 19:32:05.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14621 2023-03-17 19:32:07.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-03-17 19:32:07.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-03-17 19:32:06.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17089 2023-03-17 19:32:06.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 19:32:05.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    92801 2023-03-17 19:32:09.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    92750 2023-03-17 19:32:08.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-17 19:32:05.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-03-17 19:32:06.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-03-17 19:32:06.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:32:19.877378 mypy-boto3-dms-1.26.94/mypy_boto3_dms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28357 2023-03-17 19:32:19.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-17 19:32:19.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 19:32:19.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 19:32:19.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-17 19:32:19.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-17 19:32:19.000000 mypy-boto3-dms-1.26.94/mypy_boto3_dms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 19:32:19.877378 mypy-boto3-dms-1.26.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-17 19:32:05.000000 mypy-boto3-dms-1.26.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.351140 mypy-boto3-dms-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28329 2023-07-03 19:50:40.351140 mypy-boto3-dms-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26839 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.339140 mypy-boto3-dms-1.27.0/mypy_boto3_dms/
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66105 2023-07-03 19:35:42.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66008 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-03 19:35:42.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-07-03 19:35:42.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-07-03 19:35:42.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-07-03 19:35:42.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    92957 2023-07-03 19:35:45.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92906 2023-07-03 19:35:44.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-07-03 19:35:42.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-03 19:35:42.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.351140 mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28329 2023-07-03 19:50:40.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 19:50:40.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:40.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:40.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:40.351140 mypy-boto3-dms-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/setup.py
```

### Comparing `mypy-boto3-dms-1.26.94/LICENSE` & `mypy-boto3-dms-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-dms-1.26.94/PKG-INFO` & `mypy-boto3-dms-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dms
-Version: 1.26.94
-Summary: Type annotations for boto3.DatabaseMigrationService 1.26.94 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.DatabaseMigrationService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-dms"></a>
 
 # mypy-boto3-dms
 
 [![PyPI - mypy-boto3-dms](https://img.shields.io/pypi/v/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dms?color=blue)](https://pypistats.org/packages/mypy-boto3-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DatabaseMigrationService 1.26.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[boto3.DatabaseMigrationService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
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
 [mypy-boto3-dms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -472,15 +472,14 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dms.type_defs import (
     AccountQuotaTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     AvailabilityZoneTypeDef,
     BatchStartRecommendationsErrorEntryTypeDef,
     CancelReplicationTaskAssessmentRunMessageRequestTypeDef,
     CertificateTypeDef,
     CollectorHealthCheckTypeDef,
     InventoryDataTypeDef,
     CollectorShortInfoResponseTypeDef,
@@ -501,92 +500,96 @@
     PostgreSQLSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     S3SettingsTypeDef,
     SybaseSettingsTypeDef,
     EventSubscriptionTypeDef,
     CreateFleetAdvisorCollectorRequestRequestTypeDef,
+    CreateFleetAdvisorCollectorResponseTypeDef,
     DatabaseInstanceSoftwareDetailsResponseTypeDef,
     ServerShortInfoResponseTypeDef,
     DatabaseShortInfoResponseTypeDef,
     DeleteCertificateMessageRequestTypeDef,
     DeleteCollectorRequestRequestTypeDef,
     DeleteConnectionMessageRequestTypeDef,
     DeleteEndpointMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteFleetAdvisorDatabasesRequestRequestTypeDef,
+    DeleteFleetAdvisorDatabasesResponseTypeDef,
     DeleteReplicationInstanceMessageRequestTypeDef,
     DeleteReplicationSubnetGroupMessageRequestTypeDef,
     DeleteReplicationTaskAssessmentRunMessageRequestTypeDef,
     DeleteReplicationTaskMessageRequestTypeDef,
     DescribeApplicableIndividualAssessmentsMessageRequestTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeEndpointSettingsMessageRequestTypeDef,
     EndpointSettingTypeDef,
     SupportedEndpointTypeTypeDef,
     EventCategoryGroupTypeDef,
     EventTypeDef,
     DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef,
     FleetAdvisorLsaAnalysisResponseTypeDef,
     FleetAdvisorSchemaObjectResponseTypeDef,
+    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
     DescribeOrderableReplicationInstancesMessageRequestTypeDef,
     OrderableReplicationInstanceTypeDef,
     LimitationTypeDef,
     DescribeRefreshSchemasStatusMessageRequestTypeDef,
     RefreshSchemasStatusTypeDef,
     DescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
     ReplicationInstanceTaskLogTypeDef,
+    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef,
     ReplicationTaskAssessmentResultTypeDef,
     ReplicationTaskIndividualAssessmentTypeDef,
+    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeSchemasMessageRequestTypeDef,
+    DescribeSchemasResponseTypeDef,
     TableStatisticsTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyReplicationInstanceMessageRequestTypeDef,
     ModifyReplicationSubnetGroupMessageRequestTypeDef,
     ModifyReplicationTaskMessageRequestTypeDef,
     MoveReplicationTaskMessageRequestTypeDef,
+    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     RdsConfigurationTypeDef,
     RdsRequirementsTypeDef,
     RebootReplicationInstanceMessageRequestTypeDef,
     RecommendationSettingsTypeDef,
     RefreshSchemasMessageRequestTypeDef,
     TableToReloadTypeDef,
+    ReloadTablesResponseTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     ReplicationPendingModifiedValuesTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ReplicationTaskAssessmentRunProgressTypeDef,
     ReplicationTaskStatsTypeDef,
+    ResponseMetadataTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseTypeDef,
     SchemaShortInfoResponseTypeDef,
     StartReplicationTaskAssessmentMessageRequestTypeDef,
     StartReplicationTaskAssessmentRunMessageRequestTypeDef,
     StartReplicationTaskMessageRequestTypeDef,
     StopReplicationTaskMessageRequestTypeDef,
     TestConnectionMessageRequestTypeDef,
     UpdateSubscriptionsToEventBridgeMessageRequestTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateReplicationInstanceMessageRequestTypeDef,
     CreateReplicationSubnetGroupMessageRequestTypeDef,
     CreateReplicationTaskMessageRequestTypeDef,
     ImportCertificateMessageRequestTypeDef,
-    CreateFleetAdvisorCollectorResponseTypeDef,
-    DeleteFleetAdvisorDatabasesResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseTypeDef,
-    DescribeSchemasResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ReloadTablesResponseTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseTypeDef,
     SubnetTypeDef,
     BatchStartRecommendationsResponseTypeDef,
     DeleteCertificateResponseTypeDef,
     DescribeCertificatesResponseTypeDef,
     ImportCertificateResponseTypeDef,
     CollectorResponseTypeDef,
     DeleteConnectionResponseTypeDef,
@@ -596,47 +599,44 @@
     EndpointTypeDef,
     ModifyEndpointMessageRequestTypeDef,
     CreateEventSubscriptionResponseTypeDef,
     DeleteEventSubscriptionResponseTypeDef,
     DescribeEventSubscriptionsResponseTypeDef,
     ModifyEventSubscriptionResponseTypeDef,
     DatabaseResponseTypeDef,
+    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
+    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
     DescribeConnectionsMessageRequestTypeDef,
+    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
     DescribeEndpointTypesMessageRequestTypeDef,
+    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
     DescribeEndpointsMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeFleetAdvisorCollectorsRequestRequestTypeDef,
     DescribeFleetAdvisorDatabasesRequestRequestTypeDef,
     DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef,
     DescribeFleetAdvisorSchemasRequestRequestTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     DescribeRecommendationLimitationsRequestRequestTypeDef,
     DescribeRecommendationsRequestRequestTypeDef,
+    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
     DescribeReplicationInstancesMessageRequestTypeDef,
+    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
     DescribeReplicationSubnetGroupsMessageRequestTypeDef,
     DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef,
     DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef,
-    DescribeReplicationTasksMessageRequestTypeDef,
-    DescribeTableStatisticsMessageRequestTypeDef,
-    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
-    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
-    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
-    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
-    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
-    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
-    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef,
-    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+    DescribeReplicationTasksMessageRequestTypeDef,
     DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+    DescribeTableStatisticsMessageRequestTypeDef,
     DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef,
     DescribeEndpointsMessageEndpointDeletedWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef,
@@ -708,42 +708,42 @@
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

### Comparing `mypy-boto3-dms-1.26.94/README.md` & `mypy-boto3-dms-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-dms"></a>
 
 # mypy-boto3-dms
 
 [![PyPI - mypy-boto3-dms](https://img.shields.io/pypi/v/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dms?color=blue)](https://pypistats.org/packages/mypy-boto3-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DatabaseMigrationService 1.26.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[boto3.DatabaseMigrationService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
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
 [mypy-boto3-dms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -440,15 +440,14 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dms.type_defs import (
     AccountQuotaTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     AvailabilityZoneTypeDef,
     BatchStartRecommendationsErrorEntryTypeDef,
     CancelReplicationTaskAssessmentRunMessageRequestTypeDef,
     CertificateTypeDef,
     CollectorHealthCheckTypeDef,
     InventoryDataTypeDef,
     CollectorShortInfoResponseTypeDef,
@@ -469,92 +468,96 @@
     PostgreSQLSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     S3SettingsTypeDef,
     SybaseSettingsTypeDef,
     EventSubscriptionTypeDef,
     CreateFleetAdvisorCollectorRequestRequestTypeDef,
+    CreateFleetAdvisorCollectorResponseTypeDef,
     DatabaseInstanceSoftwareDetailsResponseTypeDef,
     ServerShortInfoResponseTypeDef,
     DatabaseShortInfoResponseTypeDef,
     DeleteCertificateMessageRequestTypeDef,
     DeleteCollectorRequestRequestTypeDef,
     DeleteConnectionMessageRequestTypeDef,
     DeleteEndpointMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteFleetAdvisorDatabasesRequestRequestTypeDef,
+    DeleteFleetAdvisorDatabasesResponseTypeDef,
     DeleteReplicationInstanceMessageRequestTypeDef,
     DeleteReplicationSubnetGroupMessageRequestTypeDef,
     DeleteReplicationTaskAssessmentRunMessageRequestTypeDef,
     DeleteReplicationTaskMessageRequestTypeDef,
     DescribeApplicableIndividualAssessmentsMessageRequestTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeEndpointSettingsMessageRequestTypeDef,
     EndpointSettingTypeDef,
     SupportedEndpointTypeTypeDef,
     EventCategoryGroupTypeDef,
     EventTypeDef,
     DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef,
     FleetAdvisorLsaAnalysisResponseTypeDef,
     FleetAdvisorSchemaObjectResponseTypeDef,
+    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
     DescribeOrderableReplicationInstancesMessageRequestTypeDef,
     OrderableReplicationInstanceTypeDef,
     LimitationTypeDef,
     DescribeRefreshSchemasStatusMessageRequestTypeDef,
     RefreshSchemasStatusTypeDef,
     DescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
     ReplicationInstanceTaskLogTypeDef,
+    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef,
     ReplicationTaskAssessmentResultTypeDef,
     ReplicationTaskIndividualAssessmentTypeDef,
+    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeSchemasMessageRequestTypeDef,
+    DescribeSchemasResponseTypeDef,
     TableStatisticsTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyReplicationInstanceMessageRequestTypeDef,
     ModifyReplicationSubnetGroupMessageRequestTypeDef,
     ModifyReplicationTaskMessageRequestTypeDef,
     MoveReplicationTaskMessageRequestTypeDef,
+    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     RdsConfigurationTypeDef,
     RdsRequirementsTypeDef,
     RebootReplicationInstanceMessageRequestTypeDef,
     RecommendationSettingsTypeDef,
     RefreshSchemasMessageRequestTypeDef,
     TableToReloadTypeDef,
+    ReloadTablesResponseTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     ReplicationPendingModifiedValuesTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ReplicationTaskAssessmentRunProgressTypeDef,
     ReplicationTaskStatsTypeDef,
+    ResponseMetadataTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseTypeDef,
     SchemaShortInfoResponseTypeDef,
     StartReplicationTaskAssessmentMessageRequestTypeDef,
     StartReplicationTaskAssessmentRunMessageRequestTypeDef,
     StartReplicationTaskMessageRequestTypeDef,
     StopReplicationTaskMessageRequestTypeDef,
     TestConnectionMessageRequestTypeDef,
     UpdateSubscriptionsToEventBridgeMessageRequestTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateReplicationInstanceMessageRequestTypeDef,
     CreateReplicationSubnetGroupMessageRequestTypeDef,
     CreateReplicationTaskMessageRequestTypeDef,
     ImportCertificateMessageRequestTypeDef,
-    CreateFleetAdvisorCollectorResponseTypeDef,
-    DeleteFleetAdvisorDatabasesResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseTypeDef,
-    DescribeSchemasResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ReloadTablesResponseTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseTypeDef,
     SubnetTypeDef,
     BatchStartRecommendationsResponseTypeDef,
     DeleteCertificateResponseTypeDef,
     DescribeCertificatesResponseTypeDef,
     ImportCertificateResponseTypeDef,
     CollectorResponseTypeDef,
     DeleteConnectionResponseTypeDef,
@@ -564,47 +567,44 @@
     EndpointTypeDef,
     ModifyEndpointMessageRequestTypeDef,
     CreateEventSubscriptionResponseTypeDef,
     DeleteEventSubscriptionResponseTypeDef,
     DescribeEventSubscriptionsResponseTypeDef,
     ModifyEventSubscriptionResponseTypeDef,
     DatabaseResponseTypeDef,
+    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
+    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
     DescribeConnectionsMessageRequestTypeDef,
+    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
     DescribeEndpointTypesMessageRequestTypeDef,
+    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
     DescribeEndpointsMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeFleetAdvisorCollectorsRequestRequestTypeDef,
     DescribeFleetAdvisorDatabasesRequestRequestTypeDef,
     DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef,
     DescribeFleetAdvisorSchemasRequestRequestTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     DescribeRecommendationLimitationsRequestRequestTypeDef,
     DescribeRecommendationsRequestRequestTypeDef,
+    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
     DescribeReplicationInstancesMessageRequestTypeDef,
+    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
     DescribeReplicationSubnetGroupsMessageRequestTypeDef,
     DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef,
     DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef,
-    DescribeReplicationTasksMessageRequestTypeDef,
-    DescribeTableStatisticsMessageRequestTypeDef,
-    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
-    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
-    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
-    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
-    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
-    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
-    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef,
-    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+    DescribeReplicationTasksMessageRequestTypeDef,
     DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+    DescribeTableStatisticsMessageRequestTypeDef,
     DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef,
     DescribeEndpointsMessageEndpointDeletedWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef,
@@ -676,42 +676,42 @@
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

### Comparing `mypy-boto3-dms-1.26.94/mypy_boto3_dms/__init__.py` & `mypy-boto3-dms-1.27.0/mypy_boto3_dms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.26.94/mypy_boto3_dms/__init__.pyi` & `mypy-boto3-dms-1.27.0/mypy_boto3_dms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.26.94/mypy_boto3_dms/__main__.py` & `mypy-boto3-dms-1.27.0/mypy_boto3_dms/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DatabaseMigrationService 1.26.94\nVersion:        "
-        " 1.26.94\nBuilder version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.DatabaseMigrationService 1.27.0\nVersion:        "
+        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.94")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-dms-1.26.94/mypy_boto3_dms/client.py` & `mypy-boto3-dms-1.27.0/mypy_boto3_dms/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.26.94/mypy_boto3_dms/client.pyi` & `mypy-boto3-dms-1.27.0/mypy_boto3_dms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.26.94/mypy_boto3_dms/literals.py` & `mypy-boto3-dms-1.27.0/mypy_boto3_dms/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AuthMechanismValueType",
     "AuthTypeValueType",
     "CannedAclForObjectsValueType",
     "CharLengthSemanticsType",
     "CollectorStatusType",
     "CompressionTypeValueType",
@@ -77,15 +76,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AuthMechanismValueType = Literal["default", "mongodb_cr", "scram_sha_1"]
 AuthTypeValueType = Literal["no", "password"]
 CannedAclForObjectsValueType = Literal[
     "authenticated-read",
     "aws-exec-read",
     "bucket-owner-full-control",
     "bucket-owner-read",
@@ -166,14 +164,15 @@
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
@@ -213,14 +212,15 @@
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
@@ -318,14 +318,15 @@
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
@@ -361,14 +362,15 @@
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
@@ -387,16 +389,19 @@
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
@@ -480,15 +485,17 @@
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

### Comparing `mypy-boto3-dms-1.26.94/mypy_boto3_dms/literals.pyi` & `mypy-boto3-dms-1.27.0/mypy_boto3_dms/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AuthMechanismValueType",
     "AuthTypeValueType",
     "CannedAclForObjectsValueType",
     "CharLengthSemanticsType",
     "CollectorStatusType",
     "CompressionTypeValueType",
@@ -76,14 +77,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AuthMechanismValueType = Literal["default", "mongodb_cr", "scram_sha_1"]
 AuthTypeValueType = Literal["no", "password"]
 CannedAclForObjectsValueType = Literal[
     "authenticated-read",
     "aws-exec-read",
     "bucket-owner-full-control",
     "bucket-owner-read",
@@ -164,14 +166,15 @@
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
@@ -211,14 +214,15 @@
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
@@ -316,14 +320,15 @@
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
@@ -359,14 +364,15 @@
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
@@ -385,16 +391,19 @@
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
@@ -478,15 +487,17 @@
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

### Comparing `mypy-boto3-dms-1.26.94/mypy_boto3_dms/paginator.py` & `mypy-boto3-dms-1.27.0/mypy_boto3_dms/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describecertificatespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describecertificatespaginator)
         """
 
 
@@ -124,15 +124,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeconnectionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeconnectionspaginator)
         """
 
 
@@ -142,15 +142,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEndpointTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointtypespaginator)
         """
 
 
@@ -160,15 +160,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointspaginator)
         """
 
 
@@ -179,15 +179,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventsubscriptionspaginator)
         """
 
 
@@ -203,30 +203,30 @@
         SourceIdentifier: str = ...,
         SourceType: Literal["replication-instance"] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventspaginator)
         """
 
 
 class DescribeOrderableReplicationInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeOrderableReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
         """
 
 
@@ -236,15 +236,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationinstancespaginator)
         """
 
 
@@ -254,30 +254,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationsubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationsubnetgroupspaginator)
         """
 
 
 class DescribeReplicationTaskAssessmentResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
     """
 
     def paginate(
-        self, *, ReplicationTaskArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ReplicationTaskArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationTaskAssessmentResultsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
         """
 
 
@@ -288,30 +288,30 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         WithoutSettings: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskspaginator)
         """
 
 
 class DescribeSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
     """
 
     def paginate(
-        self, *, EndpointArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, EndpointArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
         """
 
 
@@ -322,13 +322,13 @@
     """
 
     def paginate(
         self,
         *,
         ReplicationTaskArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTableStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describetablestatisticspaginator)
         """
```

### Comparing `mypy-boto3-dms-1.26.94/mypy_boto3_dms/paginator.pyi` & `mypy-boto3-dms-1.27.0/mypy_boto3_dms/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describecertificatespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describecertificatespaginator)
         """
 
 class DescribeConnectionsPaginator(Paginator):
@@ -119,15 +119,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeconnectionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeconnectionspaginator)
         """
 
 class DescribeEndpointTypesPaginator(Paginator):
@@ -136,15 +136,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEndpointTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointtypespaginator)
         """
 
 class DescribeEndpointsPaginator(Paginator):
@@ -153,15 +153,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeendpointspaginator)
         """
 
 class DescribeEventSubscriptionsPaginator(Paginator):
@@ -171,15 +171,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventsubscriptionspaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
@@ -194,29 +194,29 @@
         SourceIdentifier: str = ...,
         SourceType: Literal["replication-instance"] = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeeventspaginator)
         """
 
 class DescribeOrderableReplicationInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeOrderableReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeorderablereplicationinstancespaginator)
         """
 
 class DescribeReplicationInstancesPaginator(Paginator):
@@ -225,15 +225,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationinstancespaginator)
         """
 
 class DescribeReplicationSubnetGroupsPaginator(Paginator):
@@ -242,29 +242,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationsubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationsubnetgroupspaginator)
         """
 
 class DescribeReplicationTaskAssessmentResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
     """
 
     def paginate(
-        self, *, ReplicationTaskArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ReplicationTaskArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationTaskAssessmentResultsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskassessmentresultspaginator)
         """
 
 class DescribeReplicationTasksPaginator(Paginator):
@@ -274,29 +274,29 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         WithoutSettings: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeReplicationTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describereplicationtaskspaginator)
         """
 
 class DescribeSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
     """
 
     def paginate(
-        self, *, EndpointArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, EndpointArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describeschemaspaginator)
         """
 
 class DescribeTableStatisticsPaginator(Paginator):
@@ -306,13 +306,13 @@
     """
 
     def paginate(
         self,
         *,
         ReplicationTaskArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeTableStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/paginators/#describetablestatisticspaginator)
         """
```

### Comparing `mypy-boto3-dms-1.26.94/mypy_boto3_dms/type_defs.py` & `mypy-boto3-dms-1.27.0/mypy_boto3_dms/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountQuotaTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchStartRecommendationsErrorEntryTypeDef",
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     "CertificateTypeDef",
     "CollectorHealthCheckTypeDef",
     "InventoryDataTypeDef",
     "CollectorShortInfoResponseTypeDef",
@@ -90,92 +89,96 @@
     "PostgreSQLSettingsTypeDef",
     "RedisSettingsTypeDef",
     "RedshiftSettingsTypeDef",
     "S3SettingsTypeDef",
     "SybaseSettingsTypeDef",
     "EventSubscriptionTypeDef",
     "CreateFleetAdvisorCollectorRequestRequestTypeDef",
+    "CreateFleetAdvisorCollectorResponseTypeDef",
     "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     "ServerShortInfoResponseTypeDef",
     "DatabaseShortInfoResponseTypeDef",
     "DeleteCertificateMessageRequestTypeDef",
     "DeleteCollectorRequestRequestTypeDef",
     "DeleteConnectionMessageRequestTypeDef",
     "DeleteEndpointMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
     "DeleteReplicationInstanceMessageRequestTypeDef",
     "DeleteReplicationSubnetGroupMessageRequestTypeDef",
     "DeleteReplicationTaskAssessmentRunMessageRequestTypeDef",
     "DeleteReplicationTaskMessageRequestTypeDef",
     "DescribeApplicableIndividualAssessmentsMessageRequestTypeDef",
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     "FilterTypeDef",
-    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEndpointSettingsMessageRequestTypeDef",
     "EndpointSettingTypeDef",
     "SupportedEndpointTypeTypeDef",
     "EventCategoryGroupTypeDef",
     "EventTypeDef",
     "DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef",
     "FleetAdvisorLsaAnalysisResponseTypeDef",
     "FleetAdvisorSchemaObjectResponseTypeDef",
+    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
     "OrderableReplicationInstanceTypeDef",
     "LimitationTypeDef",
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
     "RefreshSchemasStatusTypeDef",
     "DescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
     "ReplicationInstanceTaskLogTypeDef",
+    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     "ReplicationTaskAssessmentResultTypeDef",
     "ReplicationTaskIndividualAssessmentTypeDef",
+    "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
     "DescribeSchemasMessageRequestTypeDef",
+    "DescribeSchemasResponseTypeDef",
     "TableStatisticsTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyReplicationInstanceMessageRequestTypeDef",
     "ModifyReplicationSubnetGroupMessageRequestTypeDef",
     "ModifyReplicationTaskMessageRequestTypeDef",
     "MoveReplicationTaskMessageRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "RdsConfigurationTypeDef",
     "RdsRequirementsTypeDef",
     "RebootReplicationInstanceMessageRequestTypeDef",
     "RecommendationSettingsTypeDef",
     "RefreshSchemasMessageRequestTypeDef",
     "TableToReloadTypeDef",
+    "ReloadTablesResponseTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "ReplicationPendingModifiedValuesTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ReplicationTaskAssessmentRunProgressTypeDef",
     "ReplicationTaskStatsTypeDef",
+    "ResponseMetadataTypeDef",
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
     "SchemaShortInfoResponseTypeDef",
     "StartReplicationTaskAssessmentMessageRequestTypeDef",
     "StartReplicationTaskAssessmentRunMessageRequestTypeDef",
     "StartReplicationTaskMessageRequestTypeDef",
     "StopReplicationTaskMessageRequestTypeDef",
     "TestConnectionMessageRequestTypeDef",
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
+    "DescribeAccountAttributesResponseTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateReplicationInstanceMessageRequestTypeDef",
     "CreateReplicationSubnetGroupMessageRequestTypeDef",
     "CreateReplicationTaskMessageRequestTypeDef",
     "ImportCertificateMessageRequestTypeDef",
-    "CreateFleetAdvisorCollectorResponseTypeDef",
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
-    "DescribeAccountAttributesResponseTypeDef",
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
-    "DescribeSchemasResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ReloadTablesResponseTypeDef",
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
     "SubnetTypeDef",
     "BatchStartRecommendationsResponseTypeDef",
     "DeleteCertificateResponseTypeDef",
     "DescribeCertificatesResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "CollectorResponseTypeDef",
     "DeleteConnectionResponseTypeDef",
@@ -185,47 +188,44 @@
     "EndpointTypeDef",
     "ModifyEndpointMessageRequestTypeDef",
     "CreateEventSubscriptionResponseTypeDef",
     "DeleteEventSubscriptionResponseTypeDef",
     "DescribeEventSubscriptionsResponseTypeDef",
     "ModifyEventSubscriptionResponseTypeDef",
     "DatabaseResponseTypeDef",
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
+    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
     "DescribeConnectionsMessageRequestTypeDef",
+    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
     "DescribeEndpointTypesMessageRequestTypeDef",
+    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
     "DescribeEndpointsMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
     "DescribeFleetAdvisorCollectorsRequestRequestTypeDef",
     "DescribeFleetAdvisorDatabasesRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemasRequestRequestTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "DescribeRecommendationLimitationsRequestRequestTypeDef",
     "DescribeRecommendationsRequestRequestTypeDef",
+    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
     "DescribeReplicationInstancesMessageRequestTypeDef",
+    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
     "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
     "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
-    "DescribeReplicationTasksMessageRequestTypeDef",
-    "DescribeTableStatisticsMessageRequestTypeDef",
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
-    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
-    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
-    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
-    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
-    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
-    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
     "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
-    "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    "DescribeReplicationTasksMessageRequestTypeDef",
     "DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+    "DescribeTableStatisticsMessageRequestTypeDef",
     "DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef",
     "DescribeEndpointsMessageEndpointDeletedWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef",
@@ -314,25 +314,14 @@
     {
         "ReplicationInstanceArn": str,
         "ApplyAction": str,
         "OptInType": str,
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
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -878,14 +867,26 @@
 class CreateFleetAdvisorCollectorRequestRequestTypeDef(
     _RequiredCreateFleetAdvisorCollectorRequestRequestTypeDef,
     _OptionalCreateFleetAdvisorCollectorRequestRequestTypeDef,
 ):
     pass
 
 
+CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
+    "CreateFleetAdvisorCollectorResponseTypeDef",
+    {
+        "CollectorReferencedId": str,
+        "CollectorName": str,
+        "Description": str,
+        "ServiceAccessRoleArn": str,
+        "S3BucketName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DatabaseInstanceSoftwareDetailsResponseTypeDef = TypedDict(
     "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "EngineEdition": str,
         "ServicePack": str,
@@ -956,14 +957,22 @@
 DeleteFleetAdvisorDatabasesRequestRequestTypeDef = TypedDict(
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
     {
         "DatabaseIds": Sequence[str],
     },
 )
 
+DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
+    {
+        "DatabaseIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteReplicationInstanceMessageRequestTypeDef = TypedDict(
     "DeleteReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceArn": str,
     },
 )
 
@@ -998,30 +1007,29 @@
         "MigrationType": MigrationTypeValueType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-FilterTypeDef = TypedDict(
-    "FilterTypeDef",
+DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     {
-        "Name": str,
-        "Values": Sequence[str],
+        "IndividualAssessmentNames": List[str],
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+FilterTypeDef = TypedDict(
+    "FilterTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Name": str,
+        "Values": Sequence[str],
     },
-    total=False,
 )
 
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
@@ -1127,14 +1135,22 @@
         "NumberOfObjects": int,
         "CodeLineCount": int,
         "CodeSize": int,
     },
     total=False,
 )
 
+DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef = TypedDict(
+    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeOrderableReplicationInstancesMessageRequestTypeDef = TypedDict(
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
@@ -1217,14 +1233,23 @@
         "ReplicationTaskName": str,
         "ReplicationTaskArn": str,
         "ReplicationInstanceTaskLogSize": int,
     },
     total=False,
 )
 
+DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
+    {
+        "ReplicationTaskArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1253,14 +1278,36 @@
         "IndividualAssessmentName": str,
         "Status": str,
         "ReplicationTaskIndividualAssessmentStartDate": datetime,
     },
     total=False,
 )
 
+_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    {
+        "EndpointArn": str,
+    },
+)
+_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeSchemasMessageDescribeSchemasPaginateTypeDef(
+    _RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+    _OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+):
+    pass
+
+
 _RequiredDescribeSchemasMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeSchemasMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 _OptionalDescribeSchemasMessageRequestTypeDef = TypedDict(
@@ -1275,14 +1322,23 @@
 
 class DescribeSchemasMessageRequestTypeDef(
     _RequiredDescribeSchemasMessageRequestTypeDef, _OptionalDescribeSchemasMessageRequestTypeDef
 ):
     pass
 
 
+DescribeSchemasResponseTypeDef = TypedDict(
+    "DescribeSchemasResponseTypeDef",
+    {
+        "Marker": str,
+        "Schemas": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TableStatisticsTypeDef = TypedDict(
     "TableStatisticsTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
         "Inserts": int,
         "Deletes": int,
@@ -1305,14 +1361,21 @@
         "ValidationSuspendedRecords": int,
         "ValidationState": str,
         "ValidationStateDetails": str,
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
 ListTagsForResourceMessageRequestTypeDef = TypedDict(
     "ListTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceArnList": Sequence[str],
     },
     total=False,
@@ -1431,14 +1494,24 @@
     "MoveReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "TargetReplicationInstanceArn": str,
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
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
@@ -1519,14 +1592,22 @@
     "TableToReloadTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
     },
 )
 
+ReloadTablesResponseTypeDef = TypedDict(
+    "ReloadTablesResponseTypeDef",
+    {
+        "ReplicationTaskArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveTagsFromResourceMessageRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1575,14 +1656,34 @@
         "StopDate": datetime,
         "FullLoadStartDate": datetime,
         "FullLoadFinishDate": datetime,
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
+RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
+    {
+        "LsaAnalysisId": str,
+        "Status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SchemaShortInfoResponseTypeDef = TypedDict(
     "SchemaShortInfoResponseTypeDef",
     {
         "SchemaId": str,
         "SchemaName": str,
         "DatabaseId": str,
         "DatabaseName": str,
@@ -1671,14 +1772,31 @@
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
     {
         "ForceMove": bool,
     },
     total=False,
 )
 
+UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAccountAttributesResponseTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseTypeDef",
+    {
+        "AccountQuotas": List[AccountQuotaTypeDef],
+        "UniqueAccountIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1822,98 +1940,19 @@
 
 class ImportCertificateMessageRequestTypeDef(
     _RequiredImportCertificateMessageRequestTypeDef, _OptionalImportCertificateMessageRequestTypeDef
 ):
     pass
 
 
-CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
-    "CreateFleetAdvisorCollectorResponseTypeDef",
-    {
-        "CollectorReferencedId": str,
-        "CollectorName": str,
-        "Description": str,
-        "ServiceAccessRoleArn": str,
-        "S3BucketName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
-    {
-        "DatabaseIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountAttributesResponseTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseTypeDef",
-    {
-        "AccountQuotas": List[AccountQuotaTypeDef],
-        "UniqueAccountIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
-    {
-        "IndividualAssessmentNames": List[str],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSchemasResponseTypeDef = TypedDict(
-    "DescribeSchemasResponseTypeDef",
-    {
-        "Marker": str,
-        "Schemas": List[str],
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
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReloadTablesResponseTypeDef = TypedDict(
-    "ReloadTablesResponseTypeDef",
-    {
-        "ReplicationTaskArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
-    {
-        "LsaAnalysisId": str,
-        "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
-    {
-        "Result": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
@@ -1923,40 +1962,40 @@
     total=False,
 )
 
 BatchStartRecommendationsResponseTypeDef = TypedDict(
     "BatchStartRecommendationsResponseTypeDef",
     {
         "ErrorEntries": List[BatchStartRecommendationsErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCertificateResponseTypeDef = TypedDict(
     "DeleteCertificateResponseTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCertificatesResponseTypeDef = TypedDict(
     "DescribeCertificatesResponseTypeDef",
     {
         "Marker": str,
         "Certificates": List[CertificateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportCertificateResponseTypeDef = TypedDict(
     "ImportCertificateResponseTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CollectorResponseTypeDef = TypedDict(
     "CollectorResponseTypeDef",
     {
         "CollectorReferencedId": str,
@@ -1976,32 +2015,32 @@
     total=False,
 )
 
 DeleteConnectionResponseTypeDef = TypedDict(
     "DeleteConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConnectionsResponseTypeDef = TypedDict(
     "DescribeConnectionsResponseTypeDef",
     {
         "Marker": str,
         "Connections": List[ConnectionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestConnectionResponseTypeDef = TypedDict(
     "TestConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointMessageRequestTypeDef",
     {
         "EndpointIdentifier": str,
@@ -2148,40 +2187,40 @@
     pass
 
 
 CreateEventSubscriptionResponseTypeDef = TypedDict(
     "CreateEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEventSubscriptionResponseTypeDef = TypedDict(
     "DeleteEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventSubscriptionsResponseTypeDef = TypedDict(
     "DescribeEventSubscriptionsResponseTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyEventSubscriptionResponseTypeDef = TypedDict(
     "ModifyEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatabaseResponseTypeDef = TypedDict(
     "DatabaseResponseTypeDef",
     {
         "DatabaseId": str,
@@ -2191,44 +2230,80 @@
         "Server": ServerShortInfoResponseTypeDef,
         "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseTypeDef,
         "Collectors": List[CollectorShortInfoResponseTypeDef],
     },
     total=False,
 )
 
+DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeCertificatesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef = TypedDict(
+    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeConnectionsMessageRequestTypeDef = TypedDict(
     "DescribeConnectionsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef = TypedDict(
+    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEndpointTypesMessageRequestTypeDef = TypedDict(
     "DescribeEndpointTypesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef = TypedDict(
+    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEndpointsMessageRequestTypeDef = TypedDict(
     "DescribeEndpointsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
@@ -2240,25 +2315,50 @@
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": Literal["replication-instance"],
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": Literal["replication-instance"],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -2338,236 +2438,136 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeReplicationInstancesMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationInstancesMessageRequestTypeDef",
+DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef = TypedDict(
+    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeReplicationSubnetGroupsMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
+DescribeReplicationInstancesMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationInstancesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
+DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
+DescribeReplicationSubnetGroupsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReplicationTasksMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationTasksMessageRequestTypeDef",
+DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
-        "WithoutSettings": bool,
     },
     total=False,
 )
 
-_RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
-    {
-        "ReplicationTaskArn": str,
-    },
-)
-_OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeTableStatisticsMessageRequestTypeDef",
+DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
     {
+        "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
-        "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-
-class DescribeTableStatisticsMessageRequestTypeDef(
-    _RequiredDescribeTableStatisticsMessageRequestTypeDef,
-    _OptionalDescribeTableStatisticsMessageRequestTypeDef,
-):
-    pass
-
-
-DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef = TypedDict(
-    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef = TypedDict(
-    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef = TypedDict(
-    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": Literal["replication-instance"],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef = TypedDict(
-    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef = TypedDict(
-    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
+DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef = TypedDict(
+    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "WithoutSettings": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
+DescribeReplicationTasksMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationTasksMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "MaxRecords": int,
+        "Marker": str,
+        "WithoutSettings": bool,
     },
     total=False,
 )
 
-DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
+_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
     {
         "ReplicationTaskArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
-    total=False,
 )
-
-DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef = TypedDict(
-    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
+_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "WithoutSettings": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
-    {
-        "EndpointArn": str,
-    },
-)
-_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class DescribeSchemasMessageDescribeSchemasPaginateTypeDef(
-    _RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
-    _OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+class DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef(
+    _RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+    _OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+_RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
-_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+_OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeTableStatisticsMessageRequestTypeDef",
     {
+        "MaxRecords": int,
+        "Marker": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef(
-    _RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
-    _OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+class DescribeTableStatisticsMessageRequestTypeDef(
+    _RequiredDescribeTableStatisticsMessageRequestTypeDef,
+    _OptionalDescribeTableStatisticsMessageRequestTypeDef,
 ):
     pass
 
 
 DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef = TypedDict(
     "DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef",
     {
@@ -2661,132 +2661,132 @@
 )
 
 DescribeEndpointSettingsResponseTypeDef = TypedDict(
     "DescribeEndpointSettingsResponseTypeDef",
     {
         "Marker": str,
         "EndpointSettings": List[EndpointSettingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointTypesResponseTypeDef = TypedDict(
     "DescribeEndpointTypesResponseTypeDef",
     {
         "Marker": str,
         "SupportedEndpointTypes": List[SupportedEndpointTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventCategoriesResponseTypeDef = TypedDict(
     "DescribeEventCategoriesResponseTypeDef",
     {
         "EventCategoryGroupList": List[EventCategoryGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
     {
         "Analysis": List[FleetAdvisorLsaAnalysisResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
     {
         "FleetAdvisorSchemaObjects": List[FleetAdvisorSchemaObjectResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOrderableReplicationInstancesResponseTypeDef = TypedDict(
     "DescribeOrderableReplicationInstancesResponseTypeDef",
     {
         "OrderableReplicationInstances": List[OrderableReplicationInstanceTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRecommendationLimitationsResponseTypeDef = TypedDict(
     "DescribeRecommendationLimitationsResponseTypeDef",
     {
         "NextToken": str,
         "Limitations": List[LimitationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRefreshSchemasStatusResponseTypeDef = TypedDict(
     "DescribeRefreshSchemasStatusResponseTypeDef",
     {
         "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RefreshSchemasResponseTypeDef = TypedDict(
     "RefreshSchemasResponseTypeDef",
     {
         "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationInstanceTaskLogsResponseTypeDef = TypedDict(
     "DescribeReplicationInstanceTaskLogsResponseTypeDef",
     {
         "ReplicationInstanceArn": str,
         "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTaskAssessmentResultsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     {
         "Marker": str,
         "BucketName": str,
         "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTaskIndividualAssessmentsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTaskIndividualAssessments": List[ReplicationTaskIndividualAssessmentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTableStatisticsResponseTypeDef = TypedDict(
     "DescribeTableStatisticsResponseTypeDef",
     {
         "ReplicationTaskArn": str,
         "TableStatistics": List[TableStatisticsTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
@@ -2917,74 +2917,74 @@
 )
 
 DescribeFleetAdvisorCollectorsResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorCollectorsResponseTypeDef",
     {
         "Collectors": List[CollectorResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEndpointResponseTypeDef = TypedDict(
     "CreateEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Marker": str,
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyEndpointResponseTypeDef = TypedDict(
     "ModifyEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorDatabasesResponseTypeDef",
     {
         "Databases": List[DatabaseResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplyPendingMaintenanceActionResponseTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResponseTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePendingMaintenanceActionsResponseTypeDef = TypedDict(
     "DescribePendingMaintenanceActionsResponseTypeDef",
     {
         "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommendationDataTypeDef = TypedDict(
     "RecommendationDataTypeDef",
     {
         "RdsEngine": RdsRecommendationTypeDef,
@@ -3000,139 +3000,139 @@
     total=False,
 )
 
 CancelReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "DeleteReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTaskAssessmentRunsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTaskAssessmentRuns": List[ReplicationTaskAssessmentRunTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "StartReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateReplicationTaskResponseTypeDef = TypedDict(
     "CreateReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationTaskResponseTypeDef = TypedDict(
     "DeleteReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTasksResponseTypeDef = TypedDict(
     "DescribeReplicationTasksResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTasks": List[ReplicationTaskTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationTaskResponseTypeDef = TypedDict(
     "ModifyReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MoveReplicationTaskResponseTypeDef = TypedDict(
     "MoveReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationTaskAssessmentResponseTypeDef = TypedDict(
     "StartReplicationTaskAssessmentResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationTaskResponseTypeDef = TypedDict(
     "StartReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopReplicationTaskResponseTypeDef = TypedDict(
     "StopReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorSchemasResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorSchemasResponseTypeDef",
     {
         "FleetAdvisorSchemas": List[SchemaResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateReplicationSubnetGroupResponseTypeDef = TypedDict(
     "CreateReplicationSubnetGroupResponseTypeDef",
     {
         "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationSubnetGroupsResponseTypeDef = TypedDict(
     "DescribeReplicationSubnetGroupsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationSubnetGroups": List[ReplicationSubnetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationSubnetGroupResponseTypeDef = TypedDict(
     "ModifyReplicationSubnetGroupResponseTypeDef",
     {
         "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicationInstanceTypeDef = TypedDict(
     "ReplicationInstanceTypeDef",
     {
         "ReplicationInstanceIdentifier": str,
@@ -3178,52 +3178,52 @@
     total=False,
 )
 
 CreateReplicationInstanceResponseTypeDef = TypedDict(
     "CreateReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationInstanceResponseTypeDef = TypedDict(
     "DeleteReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationInstancesResponseTypeDef = TypedDict(
     "DescribeReplicationInstancesResponseTypeDef",
     {
         "Marker": str,
         "ReplicationInstances": List[ReplicationInstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationInstanceResponseTypeDef = TypedDict(
     "ModifyReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootReplicationInstanceResponseTypeDef = TypedDict(
     "RebootReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRecommendationsResponseTypeDef = TypedDict(
     "DescribeRecommendationsResponseTypeDef",
     {
         "NextToken": str,
         "Recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dms-1.26.94/mypy_boto3_dms/type_defs.pyi` & `mypy-boto3-dms-1.27.0/mypy_boto3_dms/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountQuotaTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchStartRecommendationsErrorEntryTypeDef",
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     "CertificateTypeDef",
     "CollectorHealthCheckTypeDef",
     "InventoryDataTypeDef",
     "CollectorShortInfoResponseTypeDef",
@@ -89,92 +88,96 @@
     "PostgreSQLSettingsTypeDef",
     "RedisSettingsTypeDef",
     "RedshiftSettingsTypeDef",
     "S3SettingsTypeDef",
     "SybaseSettingsTypeDef",
     "EventSubscriptionTypeDef",
     "CreateFleetAdvisorCollectorRequestRequestTypeDef",
+    "CreateFleetAdvisorCollectorResponseTypeDef",
     "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     "ServerShortInfoResponseTypeDef",
     "DatabaseShortInfoResponseTypeDef",
     "DeleteCertificateMessageRequestTypeDef",
     "DeleteCollectorRequestRequestTypeDef",
     "DeleteConnectionMessageRequestTypeDef",
     "DeleteEndpointMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
     "DeleteReplicationInstanceMessageRequestTypeDef",
     "DeleteReplicationSubnetGroupMessageRequestTypeDef",
     "DeleteReplicationTaskAssessmentRunMessageRequestTypeDef",
     "DeleteReplicationTaskMessageRequestTypeDef",
     "DescribeApplicableIndividualAssessmentsMessageRequestTypeDef",
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     "FilterTypeDef",
-    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEndpointSettingsMessageRequestTypeDef",
     "EndpointSettingTypeDef",
     "SupportedEndpointTypeTypeDef",
     "EventCategoryGroupTypeDef",
     "EventTypeDef",
     "DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef",
     "FleetAdvisorLsaAnalysisResponseTypeDef",
     "FleetAdvisorSchemaObjectResponseTypeDef",
+    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
     "OrderableReplicationInstanceTypeDef",
     "LimitationTypeDef",
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
     "RefreshSchemasStatusTypeDef",
     "DescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
     "ReplicationInstanceTaskLogTypeDef",
+    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     "ReplicationTaskAssessmentResultTypeDef",
     "ReplicationTaskIndividualAssessmentTypeDef",
+    "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
     "DescribeSchemasMessageRequestTypeDef",
+    "DescribeSchemasResponseTypeDef",
     "TableStatisticsTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyReplicationInstanceMessageRequestTypeDef",
     "ModifyReplicationSubnetGroupMessageRequestTypeDef",
     "ModifyReplicationTaskMessageRequestTypeDef",
     "MoveReplicationTaskMessageRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "RdsConfigurationTypeDef",
     "RdsRequirementsTypeDef",
     "RebootReplicationInstanceMessageRequestTypeDef",
     "RecommendationSettingsTypeDef",
     "RefreshSchemasMessageRequestTypeDef",
     "TableToReloadTypeDef",
+    "ReloadTablesResponseTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "ReplicationPendingModifiedValuesTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ReplicationTaskAssessmentRunProgressTypeDef",
     "ReplicationTaskStatsTypeDef",
+    "ResponseMetadataTypeDef",
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
     "SchemaShortInfoResponseTypeDef",
     "StartReplicationTaskAssessmentMessageRequestTypeDef",
     "StartReplicationTaskAssessmentRunMessageRequestTypeDef",
     "StartReplicationTaskMessageRequestTypeDef",
     "StopReplicationTaskMessageRequestTypeDef",
     "TestConnectionMessageRequestTypeDef",
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
+    "DescribeAccountAttributesResponseTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateReplicationInstanceMessageRequestTypeDef",
     "CreateReplicationSubnetGroupMessageRequestTypeDef",
     "CreateReplicationTaskMessageRequestTypeDef",
     "ImportCertificateMessageRequestTypeDef",
-    "CreateFleetAdvisorCollectorResponseTypeDef",
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
-    "DescribeAccountAttributesResponseTypeDef",
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
-    "DescribeSchemasResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ReloadTablesResponseTypeDef",
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
     "SubnetTypeDef",
     "BatchStartRecommendationsResponseTypeDef",
     "DeleteCertificateResponseTypeDef",
     "DescribeCertificatesResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "CollectorResponseTypeDef",
     "DeleteConnectionResponseTypeDef",
@@ -184,47 +187,44 @@
     "EndpointTypeDef",
     "ModifyEndpointMessageRequestTypeDef",
     "CreateEventSubscriptionResponseTypeDef",
     "DeleteEventSubscriptionResponseTypeDef",
     "DescribeEventSubscriptionsResponseTypeDef",
     "ModifyEventSubscriptionResponseTypeDef",
     "DatabaseResponseTypeDef",
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
+    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
     "DescribeConnectionsMessageRequestTypeDef",
+    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
     "DescribeEndpointTypesMessageRequestTypeDef",
+    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
     "DescribeEndpointsMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
     "DescribeFleetAdvisorCollectorsRequestRequestTypeDef",
     "DescribeFleetAdvisorDatabasesRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemasRequestRequestTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "DescribeRecommendationLimitationsRequestRequestTypeDef",
     "DescribeRecommendationsRequestRequestTypeDef",
+    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
     "DescribeReplicationInstancesMessageRequestTypeDef",
+    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
     "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
     "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
-    "DescribeReplicationTasksMessageRequestTypeDef",
-    "DescribeTableStatisticsMessageRequestTypeDef",
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
-    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
-    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
-    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
-    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
-    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
-    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
     "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
-    "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    "DescribeReplicationTasksMessageRequestTypeDef",
     "DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+    "DescribeTableStatisticsMessageRequestTypeDef",
     "DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef",
     "DescribeEndpointsMessageEndpointDeletedWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef",
@@ -313,25 +313,14 @@
     {
         "ReplicationInstanceArn": str,
         "ApplyAction": str,
         "OptInType": str,
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
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -869,14 +858,26 @@
 
 class CreateFleetAdvisorCollectorRequestRequestTypeDef(
     _RequiredCreateFleetAdvisorCollectorRequestRequestTypeDef,
     _OptionalCreateFleetAdvisorCollectorRequestRequestTypeDef,
 ):
     pass
 
+CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
+    "CreateFleetAdvisorCollectorResponseTypeDef",
+    {
+        "CollectorReferencedId": str,
+        "CollectorName": str,
+        "Description": str,
+        "ServiceAccessRoleArn": str,
+        "S3BucketName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DatabaseInstanceSoftwareDetailsResponseTypeDef = TypedDict(
     "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "EngineEdition": str,
         "ServicePack": str,
@@ -947,14 +948,22 @@
 DeleteFleetAdvisorDatabasesRequestRequestTypeDef = TypedDict(
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
     {
         "DatabaseIds": Sequence[str],
     },
 )
 
+DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
+    {
+        "DatabaseIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteReplicationInstanceMessageRequestTypeDef = TypedDict(
     "DeleteReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceArn": str,
     },
 )
 
@@ -989,30 +998,29 @@
         "MigrationType": MigrationTypeValueType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-FilterTypeDef = TypedDict(
-    "FilterTypeDef",
+DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     {
-        "Name": str,
-        "Values": Sequence[str],
+        "IndividualAssessmentNames": List[str],
+        "Marker": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+FilterTypeDef = TypedDict(
+    "FilterTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Name": str,
+        "Values": Sequence[str],
     },
-    total=False,
 )
 
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
@@ -1116,14 +1124,22 @@
         "NumberOfObjects": int,
         "CodeLineCount": int,
         "CodeSize": int,
     },
     total=False,
 )
 
+DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef = TypedDict(
+    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeOrderableReplicationInstancesMessageRequestTypeDef = TypedDict(
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
@@ -1204,14 +1220,23 @@
         "ReplicationTaskName": str,
         "ReplicationTaskArn": str,
         "ReplicationInstanceTaskLogSize": int,
     },
     total=False,
 )
 
+DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
+    {
+        "ReplicationTaskArn": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1240,14 +1265,34 @@
         "IndividualAssessmentName": str,
         "Status": str,
         "ReplicationTaskIndividualAssessmentStartDate": datetime,
     },
     total=False,
 )
 
+_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    {
+        "EndpointArn": str,
+    },
+)
+_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeSchemasMessageDescribeSchemasPaginateTypeDef(
+    _RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+    _OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+):
+    pass
+
 _RequiredDescribeSchemasMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeSchemasMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 _OptionalDescribeSchemasMessageRequestTypeDef = TypedDict(
@@ -1260,14 +1305,23 @@
 )
 
 class DescribeSchemasMessageRequestTypeDef(
     _RequiredDescribeSchemasMessageRequestTypeDef, _OptionalDescribeSchemasMessageRequestTypeDef
 ):
     pass
 
+DescribeSchemasResponseTypeDef = TypedDict(
+    "DescribeSchemasResponseTypeDef",
+    {
+        "Marker": str,
+        "Schemas": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TableStatisticsTypeDef = TypedDict(
     "TableStatisticsTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
         "Inserts": int,
         "Deletes": int,
@@ -1290,14 +1344,21 @@
         "ValidationSuspendedRecords": int,
         "ValidationState": str,
         "ValidationStateDetails": str,
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
 ListTagsForResourceMessageRequestTypeDef = TypedDict(
     "ListTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceArnList": Sequence[str],
     },
     total=False,
@@ -1408,14 +1469,24 @@
     "MoveReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "TargetReplicationInstanceArn": str,
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
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
@@ -1494,14 +1565,22 @@
     "TableToReloadTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
     },
 )
 
+ReloadTablesResponseTypeDef = TypedDict(
+    "ReloadTablesResponseTypeDef",
+    {
+        "ReplicationTaskArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveTagsFromResourceMessageRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1550,14 +1629,34 @@
         "StopDate": datetime,
         "FullLoadStartDate": datetime,
         "FullLoadFinishDate": datetime,
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
+RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
+    {
+        "LsaAnalysisId": str,
+        "Status": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SchemaShortInfoResponseTypeDef = TypedDict(
     "SchemaShortInfoResponseTypeDef",
     {
         "SchemaId": str,
         "SchemaName": str,
         "DatabaseId": str,
         "DatabaseName": str,
@@ -1642,14 +1741,31 @@
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
     {
         "ForceMove": bool,
     },
     total=False,
 )
 
+UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeAccountAttributesResponseTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseTypeDef",
+    {
+        "AccountQuotas": List[AccountQuotaTypeDef],
+        "UniqueAccountIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1783,98 +1899,19 @@
 )
 
 class ImportCertificateMessageRequestTypeDef(
     _RequiredImportCertificateMessageRequestTypeDef, _OptionalImportCertificateMessageRequestTypeDef
 ):
     pass
 
-CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
-    "CreateFleetAdvisorCollectorResponseTypeDef",
-    {
-        "CollectorReferencedId": str,
-        "CollectorName": str,
-        "Description": str,
-        "ServiceAccessRoleArn": str,
-        "S3BucketName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
-    {
-        "DatabaseIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAccountAttributesResponseTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseTypeDef",
-    {
-        "AccountQuotas": List[AccountQuotaTypeDef],
-        "UniqueAccountIdentifier": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
-    {
-        "IndividualAssessmentNames": List[str],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSchemasResponseTypeDef = TypedDict(
-    "DescribeSchemasResponseTypeDef",
-    {
-        "Marker": str,
-        "Schemas": List[str],
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
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReloadTablesResponseTypeDef = TypedDict(
-    "ReloadTablesResponseTypeDef",
-    {
-        "ReplicationTaskArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
-    {
-        "LsaAnalysisId": str,
-        "Status": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
-    {
-        "Result": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
@@ -1884,40 +1921,40 @@
     total=False,
 )
 
 BatchStartRecommendationsResponseTypeDef = TypedDict(
     "BatchStartRecommendationsResponseTypeDef",
     {
         "ErrorEntries": List[BatchStartRecommendationsErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteCertificateResponseTypeDef = TypedDict(
     "DeleteCertificateResponseTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCertificatesResponseTypeDef = TypedDict(
     "DescribeCertificatesResponseTypeDef",
     {
         "Marker": str,
         "Certificates": List[CertificateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportCertificateResponseTypeDef = TypedDict(
     "ImportCertificateResponseTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CollectorResponseTypeDef = TypedDict(
     "CollectorResponseTypeDef",
     {
         "CollectorReferencedId": str,
@@ -1937,32 +1974,32 @@
     total=False,
 )
 
 DeleteConnectionResponseTypeDef = TypedDict(
     "DeleteConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeConnectionsResponseTypeDef = TypedDict(
     "DescribeConnectionsResponseTypeDef",
     {
         "Marker": str,
         "Connections": List[ConnectionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TestConnectionResponseTypeDef = TypedDict(
     "TestConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointMessageRequestTypeDef",
     {
         "EndpointIdentifier": str,
@@ -2105,40 +2142,40 @@
 ):
     pass
 
 CreateEventSubscriptionResponseTypeDef = TypedDict(
     "CreateEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEventSubscriptionResponseTypeDef = TypedDict(
     "DeleteEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventSubscriptionsResponseTypeDef = TypedDict(
     "DescribeEventSubscriptionsResponseTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyEventSubscriptionResponseTypeDef = TypedDict(
     "ModifyEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DatabaseResponseTypeDef = TypedDict(
     "DatabaseResponseTypeDef",
     {
         "DatabaseId": str,
@@ -2148,44 +2185,80 @@
         "Server": ServerShortInfoResponseTypeDef,
         "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseTypeDef,
         "Collectors": List[CollectorShortInfoResponseTypeDef],
     },
     total=False,
 )
 
+DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeCertificatesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef = TypedDict(
+    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeConnectionsMessageRequestTypeDef = TypedDict(
     "DescribeConnectionsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef = TypedDict(
+    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEndpointTypesMessageRequestTypeDef = TypedDict(
     "DescribeEndpointTypesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef = TypedDict(
+    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEndpointsMessageRequestTypeDef = TypedDict(
     "DescribeEndpointsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
@@ -2197,25 +2270,50 @@
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": Literal["replication-instance"],
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": Literal["replication-instance"],
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -2295,231 +2393,133 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeReplicationInstancesMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationInstancesMessageRequestTypeDef",
+DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef = TypedDict(
+    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeReplicationSubnetGroupsMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
+DescribeReplicationInstancesMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationInstancesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
+DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
+DescribeReplicationSubnetGroupsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReplicationTasksMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationTasksMessageRequestTypeDef",
+DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
-        "WithoutSettings": bool,
     },
     total=False,
 )
 
-_RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
-    {
-        "ReplicationTaskArn": str,
-    },
-)
-_OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeTableStatisticsMessageRequestTypeDef",
+DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
     {
+        "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
-        "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-class DescribeTableStatisticsMessageRequestTypeDef(
-    _RequiredDescribeTableStatisticsMessageRequestTypeDef,
-    _OptionalDescribeTableStatisticsMessageRequestTypeDef,
-):
-    pass
-
-DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef = TypedDict(
-    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef = TypedDict(
-    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef = TypedDict(
-    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": Literal["replication-instance"],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef = TypedDict(
-    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef = TypedDict(
-    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
+DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef = TypedDict(
+    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "WithoutSettings": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
+DescribeReplicationTasksMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationTasksMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "MaxRecords": int,
+        "Marker": str,
+        "WithoutSettings": bool,
     },
     total=False,
 )
 
-DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
+_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
     {
         "ReplicationTaskArn": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
-    total=False,
 )
-
-DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef = TypedDict(
-    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
+_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "WithoutSettings": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
-    {
-        "EndpointArn": str,
-    },
-)
-_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class DescribeSchemasMessageDescribeSchemasPaginateTypeDef(
-    _RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
-    _OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+class DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef(
+    _RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+    _OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
 ):
     pass
 
-_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+_RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
-_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+_OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeTableStatisticsMessageRequestTypeDef",
     {
+        "MaxRecords": int,
+        "Marker": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef(
-    _RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
-    _OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+class DescribeTableStatisticsMessageRequestTypeDef(
+    _RequiredDescribeTableStatisticsMessageRequestTypeDef,
+    _OptionalDescribeTableStatisticsMessageRequestTypeDef,
 ):
     pass
 
 DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef = TypedDict(
     "DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -2612,132 +2612,132 @@
 )
 
 DescribeEndpointSettingsResponseTypeDef = TypedDict(
     "DescribeEndpointSettingsResponseTypeDef",
     {
         "Marker": str,
         "EndpointSettings": List[EndpointSettingTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointTypesResponseTypeDef = TypedDict(
     "DescribeEndpointTypesResponseTypeDef",
     {
         "Marker": str,
         "SupportedEndpointTypes": List[SupportedEndpointTypeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventCategoriesResponseTypeDef = TypedDict(
     "DescribeEventCategoriesResponseTypeDef",
     {
         "EventCategoryGroupList": List[EventCategoryGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
     {
         "Analysis": List[FleetAdvisorLsaAnalysisResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
     {
         "FleetAdvisorSchemaObjects": List[FleetAdvisorSchemaObjectResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeOrderableReplicationInstancesResponseTypeDef = TypedDict(
     "DescribeOrderableReplicationInstancesResponseTypeDef",
     {
         "OrderableReplicationInstances": List[OrderableReplicationInstanceTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRecommendationLimitationsResponseTypeDef = TypedDict(
     "DescribeRecommendationLimitationsResponseTypeDef",
     {
         "NextToken": str,
         "Limitations": List[LimitationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRefreshSchemasStatusResponseTypeDef = TypedDict(
     "DescribeRefreshSchemasStatusResponseTypeDef",
     {
         "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RefreshSchemasResponseTypeDef = TypedDict(
     "RefreshSchemasResponseTypeDef",
     {
         "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationInstanceTaskLogsResponseTypeDef = TypedDict(
     "DescribeReplicationInstanceTaskLogsResponseTypeDef",
     {
         "ReplicationInstanceArn": str,
         "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTaskAssessmentResultsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     {
         "Marker": str,
         "BucketName": str,
         "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTaskIndividualAssessmentsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTaskIndividualAssessments": List[ReplicationTaskIndividualAssessmentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTableStatisticsResponseTypeDef = TypedDict(
     "DescribeTableStatisticsResponseTypeDef",
     {
         "ReplicationTaskArn": str,
         "TableStatistics": List[TableStatisticsTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
@@ -2866,74 +2866,74 @@
 )
 
 DescribeFleetAdvisorCollectorsResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorCollectorsResponseTypeDef",
     {
         "Collectors": List[CollectorResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateEndpointResponseTypeDef = TypedDict(
     "CreateEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Marker": str,
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyEndpointResponseTypeDef = TypedDict(
     "ModifyEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorDatabasesResponseTypeDef",
     {
         "Databases": List[DatabaseResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ApplyPendingMaintenanceActionResponseTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResponseTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePendingMaintenanceActionsResponseTypeDef = TypedDict(
     "DescribePendingMaintenanceActionsResponseTypeDef",
     {
         "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
         "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommendationDataTypeDef = TypedDict(
     "RecommendationDataTypeDef",
     {
         "RdsEngine": RdsRecommendationTypeDef,
@@ -2949,139 +2949,139 @@
     total=False,
 )
 
 CancelReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "DeleteReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTaskAssessmentRunsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTaskAssessmentRuns": List[ReplicationTaskAssessmentRunTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "StartReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateReplicationTaskResponseTypeDef = TypedDict(
     "CreateReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationTaskResponseTypeDef = TypedDict(
     "DeleteReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationTasksResponseTypeDef = TypedDict(
     "DescribeReplicationTasksResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTasks": List[ReplicationTaskTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationTaskResponseTypeDef = TypedDict(
     "ModifyReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MoveReplicationTaskResponseTypeDef = TypedDict(
     "MoveReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationTaskAssessmentResponseTypeDef = TypedDict(
     "StartReplicationTaskAssessmentResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartReplicationTaskResponseTypeDef = TypedDict(
     "StartReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopReplicationTaskResponseTypeDef = TypedDict(
     "StopReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeFleetAdvisorSchemasResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorSchemasResponseTypeDef",
     {
         "FleetAdvisorSchemas": List[SchemaResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateReplicationSubnetGroupResponseTypeDef = TypedDict(
     "CreateReplicationSubnetGroupResponseTypeDef",
     {
         "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationSubnetGroupsResponseTypeDef = TypedDict(
     "DescribeReplicationSubnetGroupsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationSubnetGroups": List[ReplicationSubnetGroupTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationSubnetGroupResponseTypeDef = TypedDict(
     "ModifyReplicationSubnetGroupResponseTypeDef",
     {
         "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicationInstanceTypeDef = TypedDict(
     "ReplicationInstanceTypeDef",
     {
         "ReplicationInstanceIdentifier": str,
@@ -3127,52 +3127,52 @@
     total=False,
 )
 
 CreateReplicationInstanceResponseTypeDef = TypedDict(
     "CreateReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteReplicationInstanceResponseTypeDef = TypedDict(
     "DeleteReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeReplicationInstancesResponseTypeDef = TypedDict(
     "DescribeReplicationInstancesResponseTypeDef",
     {
         "Marker": str,
         "ReplicationInstances": List[ReplicationInstanceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReplicationInstanceResponseTypeDef = TypedDict(
     "ModifyReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RebootReplicationInstanceResponseTypeDef = TypedDict(
     "RebootReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRecommendationsResponseTypeDef = TypedDict(
     "DescribeRecommendationsResponseTypeDef",
     {
         "NextToken": str,
         "Recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dms-1.26.94/mypy_boto3_dms/waiter.py` & `mypy-boto3-dms-1.27.0/mypy_boto3_dms/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.26.94/mypy_boto3_dms/waiter.pyi` & `mypy-boto3-dms-1.27.0/mypy_boto3_dms/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.26.94/mypy_boto3_dms.egg-info/PKG-INFO` & `mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dms
-Version: 1.26.94
-Summary: Type annotations for boto3.DatabaseMigrationService 1.26.94 service generated with mypy-boto3-builder 7.13.0
+Version: 1.27.0
+Summary: Type annotations for boto3.DatabaseMigrationService 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-dms"></a>
 
 # mypy-boto3-dms
 
 [![PyPI - mypy-boto3-dms](https://img.shields.io/pypi/v/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dms?color=blue)](https://pypistats.org/packages/mypy-boto3-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DatabaseMigrationService 1.26.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[boto3.DatabaseMigrationService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
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
 [mypy-boto3-dms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -472,15 +472,14 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dms.type_defs import (
     AccountQuotaTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     AvailabilityZoneTypeDef,
     BatchStartRecommendationsErrorEntryTypeDef,
     CancelReplicationTaskAssessmentRunMessageRequestTypeDef,
     CertificateTypeDef,
     CollectorHealthCheckTypeDef,
     InventoryDataTypeDef,
     CollectorShortInfoResponseTypeDef,
@@ -501,92 +500,96 @@
     PostgreSQLSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     S3SettingsTypeDef,
     SybaseSettingsTypeDef,
     EventSubscriptionTypeDef,
     CreateFleetAdvisorCollectorRequestRequestTypeDef,
+    CreateFleetAdvisorCollectorResponseTypeDef,
     DatabaseInstanceSoftwareDetailsResponseTypeDef,
     ServerShortInfoResponseTypeDef,
     DatabaseShortInfoResponseTypeDef,
     DeleteCertificateMessageRequestTypeDef,
     DeleteCollectorRequestRequestTypeDef,
     DeleteConnectionMessageRequestTypeDef,
     DeleteEndpointMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteFleetAdvisorDatabasesRequestRequestTypeDef,
+    DeleteFleetAdvisorDatabasesResponseTypeDef,
     DeleteReplicationInstanceMessageRequestTypeDef,
     DeleteReplicationSubnetGroupMessageRequestTypeDef,
     DeleteReplicationTaskAssessmentRunMessageRequestTypeDef,
     DeleteReplicationTaskMessageRequestTypeDef,
     DescribeApplicableIndividualAssessmentsMessageRequestTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseTypeDef,
     FilterTypeDef,
-    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeEndpointSettingsMessageRequestTypeDef,
     EndpointSettingTypeDef,
     SupportedEndpointTypeTypeDef,
     EventCategoryGroupTypeDef,
     EventTypeDef,
     DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef,
     FleetAdvisorLsaAnalysisResponseTypeDef,
     FleetAdvisorSchemaObjectResponseTypeDef,
+    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
     DescribeOrderableReplicationInstancesMessageRequestTypeDef,
     OrderableReplicationInstanceTypeDef,
     LimitationTypeDef,
     DescribeRefreshSchemasStatusMessageRequestTypeDef,
     RefreshSchemasStatusTypeDef,
     DescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
     ReplicationInstanceTaskLogTypeDef,
+    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef,
     ReplicationTaskAssessmentResultTypeDef,
     ReplicationTaskIndividualAssessmentTypeDef,
+    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeSchemasMessageRequestTypeDef,
+    DescribeSchemasResponseTypeDef,
     TableStatisticsTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyReplicationInstanceMessageRequestTypeDef,
     ModifyReplicationSubnetGroupMessageRequestTypeDef,
     ModifyReplicationTaskMessageRequestTypeDef,
     MoveReplicationTaskMessageRequestTypeDef,
+    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     RdsConfigurationTypeDef,
     RdsRequirementsTypeDef,
     RebootReplicationInstanceMessageRequestTypeDef,
     RecommendationSettingsTypeDef,
     RefreshSchemasMessageRequestTypeDef,
     TableToReloadTypeDef,
+    ReloadTablesResponseTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     ReplicationPendingModifiedValuesTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ReplicationTaskAssessmentRunProgressTypeDef,
     ReplicationTaskStatsTypeDef,
+    ResponseMetadataTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseTypeDef,
     SchemaShortInfoResponseTypeDef,
     StartReplicationTaskAssessmentMessageRequestTypeDef,
     StartReplicationTaskAssessmentRunMessageRequestTypeDef,
     StartReplicationTaskMessageRequestTypeDef,
     StopReplicationTaskMessageRequestTypeDef,
     TestConnectionMessageRequestTypeDef,
     UpdateSubscriptionsToEventBridgeMessageRequestTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateReplicationInstanceMessageRequestTypeDef,
     CreateReplicationSubnetGroupMessageRequestTypeDef,
     CreateReplicationTaskMessageRequestTypeDef,
     ImportCertificateMessageRequestTypeDef,
-    CreateFleetAdvisorCollectorResponseTypeDef,
-    DeleteFleetAdvisorDatabasesResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseTypeDef,
-    DescribeSchemasResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ReloadTablesResponseTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseTypeDef,
     SubnetTypeDef,
     BatchStartRecommendationsResponseTypeDef,
     DeleteCertificateResponseTypeDef,
     DescribeCertificatesResponseTypeDef,
     ImportCertificateResponseTypeDef,
     CollectorResponseTypeDef,
     DeleteConnectionResponseTypeDef,
@@ -596,47 +599,44 @@
     EndpointTypeDef,
     ModifyEndpointMessageRequestTypeDef,
     CreateEventSubscriptionResponseTypeDef,
     DeleteEventSubscriptionResponseTypeDef,
     DescribeEventSubscriptionsResponseTypeDef,
     ModifyEventSubscriptionResponseTypeDef,
     DatabaseResponseTypeDef,
+    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
+    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
     DescribeConnectionsMessageRequestTypeDef,
+    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
     DescribeEndpointTypesMessageRequestTypeDef,
+    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
     DescribeEndpointsMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeFleetAdvisorCollectorsRequestRequestTypeDef,
     DescribeFleetAdvisorDatabasesRequestRequestTypeDef,
     DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef,
     DescribeFleetAdvisorSchemasRequestRequestTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     DescribeRecommendationLimitationsRequestRequestTypeDef,
     DescribeRecommendationsRequestRequestTypeDef,
+    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
     DescribeReplicationInstancesMessageRequestTypeDef,
+    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
     DescribeReplicationSubnetGroupsMessageRequestTypeDef,
     DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef,
     DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef,
-    DescribeReplicationTasksMessageRequestTypeDef,
-    DescribeTableStatisticsMessageRequestTypeDef,
-    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
-    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
-    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
-    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
-    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
-    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
-    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef,
-    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+    DescribeReplicationTasksMessageRequestTypeDef,
     DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+    DescribeTableStatisticsMessageRequestTypeDef,
     DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef,
     DescribeEndpointsMessageEndpointDeletedWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef,
@@ -708,42 +708,42 @@
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

### Comparing `mypy-boto3-dms-1.26.94/mypy_boto3_dms.egg-info/SOURCES.txt` & `mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.26.94/setup.py` & `mypy-boto3-dms-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-dms.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dms",
-    version="1.26.94",
+    version="1.27.0",
     packages=["mypy_boto3_dms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DatabaseMigrationService 1.26.94 service generated with"
-        " mypy-boto3-builder 7.13.0"
+        "Type annotations for boto3.DatabaseMigrationService 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/",
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


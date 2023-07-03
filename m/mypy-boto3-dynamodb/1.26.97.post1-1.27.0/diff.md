# Comparing `tmp/mypy-boto3-dynamodb-1.26.97.post1.tar.gz` & `tmp/mypy-boto3-dynamodb-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dynamodb-1.26.97.post1.tar", last modified: Thu Mar 23 01:30:37 2023, max compression
+gzip compressed data, was "mypy-boto3-dynamodb-1.27.0.tar", last modified: Mon Jul  3 19:50:41 2023, max compression
```

## Comparing `mypy-boto3-dynamodb-1.26.97.post1.tar` & `mypy-boto3-dynamodb-1.27.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-23 01:30:37.291124 mypy-boto3-dynamodb-1.26.97.post1/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1070 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/LICENSE
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    28241 2023-03-23 01:30:37.291124 mypy-boto3-dynamodb-1.26.97.post1/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    26744 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/README.md
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-23 01:30:37.287124 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1858 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/__init__.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1856 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/__init__.pyi
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      923 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/__main__.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    53968 2023-03-23 01:29:17.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/client.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    53901 2023-03-23 01:29:17.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/client.pyi
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    12660 2023-03-23 01:29:18.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/literals.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    12658 2023-03-23 01:29:18.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/literals.pyi
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     8360 2023-03-23 01:29:18.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/paginator.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     8353 2023-03-23 01:29:18.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/paginator.pyi
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/py.typed
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    27133 2023-03-23 01:29:17.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/service_resource.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    27106 2023-03-23 01:29:17.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/service_resource.pyi
--rw-rw-r--   0 vlad      (1000) vlad      (1000)   151904 2023-03-23 01:29:21.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/type_defs.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)   151751 2023-03-23 01:29:20.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/type_defs.pyi
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       67 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/version.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     2258 2023-03-23 01:29:18.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/waiter.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     2256 2023-03-23 01:29:18.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/waiter.pyi
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-23 01:30:37.291124 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    28241 2023-03-23 01:30:37.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      841 2023-03-23 01:30:37.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/SOURCES.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-03-23 01:30:37.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/dependency_links.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-03-23 01:30:37.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/not-zip-safe
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       52 2023-03-23 01:30:37.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/requires.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       20 2023-03-23 01:30:37.000000 mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/top_level.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-03-23 01:30:37.291124 mypy-boto3-dynamodb-1.26.97.post1/setup.cfg
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     2009 2023-03-23 01:29:16.000000 mypy-boto3-dynamodb-1.26.97.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:41.075153 mypy-boto3-dynamodb-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-07-03 19:50:41.071153 mypy-boto3-dynamodb-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26772 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:41.067153 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54381 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12863 2023-07-03 19:36:00.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-07-03 19:36:00.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-07-03 19:36:00.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-03 19:36:00.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27454 2023-07-03 19:36:00.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   152926 2023-07-03 19:36:04.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152773 2023-07-03 19:36:02.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-03 19:36:00.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-03 19:36:00.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:41.067153 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-07-03 19:50:40.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 19:50:40.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:40.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:50:40.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:41.075153 mypy-boto3-dynamodb-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/setup.py
```

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/LICENSE` & `mypy-boto3-dynamodb-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/PKG-INFO` & `mypy-boto3-dynamodb-1.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.26.97.post1
-Summary: Type annotations for boto3.DynamoDB 1.26.97 service generated with mypy-boto3-builder 7.14.1
+Version: 1.27.0
+Summary: Type annotations for boto3.DynamoDB 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-dynamodb"></a>
 
 # mypy-boto3-dynamodb
 
 [![PyPI - mypy-boto3-dynamodb](https://img.shields.io/pypi/v/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dynamodb?color=blue)](https://pypistats.org/packages/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -481,30 +481,30 @@
 ### Typed dictionaries
 
 `mypy_boto3_dynamodb.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodb.type_defs import (
-    ResponseMetadataTypeDef,
+    ArchivalSummaryResponseMetadataTypeDef,
     ArchivalSummaryTableTypeDef,
     ArchivalSummaryTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
     AttributeValueTypeDef,
     AttributeValueUpdateTableTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
     BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
-    BatchStatementErrorTypeDef,
     ItemCollectionMetricsServiceResourceTypeDef,
+    BillingModeSummaryResponseMetadataTypeDef,
     BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
     CapacityServiceResourceTypeDef,
     CapacityTableTypeDef,
     CapacityTypeDef,
     ConditionTableTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
@@ -547,64 +547,67 @@
     DescribeExportInputRequestTypeDef,
     ExportDescriptionTypeDef,
     DescribeGlobalTableInputRequestTypeDef,
     DescribeGlobalTableSettingsInputRequestTypeDef,
     DescribeImportInputRequestTypeDef,
     DescribeKinesisStreamingDestinationInputRequestTypeDef,
     KinesisDataStreamDestinationTypeDef,
+    DescribeLimitsOutputTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportSummaryTypeDef,
     ExportTableToPointInTimeInputRequestTypeDef,
     GetItemInputTableGetItemTypeDef,
     ProvisionedThroughputDescriptionTableTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
     ProjectionServiceResourceTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    KinesisStreamingDestinationOutputTypeDef,
+    ListBackupsInputListBackupsPaginateTypeDef,
     ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
+    ListTablesInputListTablesPaginateTypeDef,
     ListTablesInputRequestTypeDef,
+    ListTablesOutputTableTypeDef,
+    ListTablesOutputTypeDef,
+    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
     TagTableTypeDef,
+    PaginatorConfigTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
+    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
     PutRequestServiceResourceTypeDef,
     TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
+    ResponseMetadataTypeDef,
+    RestoreSummaryResponseMetadataTypeDef,
     RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
+    SSEDescriptionResponseMetadataTypeDef,
     SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
     SSESpecificationTableTypeDef,
+    StreamSpecificationResponseMetadataTypeDef,
     StreamSpecificationTableTypeDef,
     TableBatchWriterRequestTypeDef,
+    TableClassSummaryResponseMetadataTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
-    ArchivalSummaryResponseMetadataTypeDef,
-    BillingModeSummaryResponseMetadataTypeDef,
-    DescribeLimitsOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    KinesisStreamingDestinationOutputTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTablesOutputTypeDef,
-    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
-    RestoreSummaryResponseMetadataTypeDef,
-    SSEDescriptionResponseMetadataTypeDef,
-    StreamSpecificationResponseMetadataTypeDef,
-    TableClassSummaryResponseMetadataTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     AttributeValueUpdateTypeDef,
+    BatchStatementErrorTypeDef,
     BatchStatementRequestTypeDef,
     ConditionCheckTypeDef,
     ConditionTypeDef,
     DeleteRequestTypeDef,
     DeleteTypeDef,
     ExecuteStatementInputRequestTypeDef,
     ExpectedAttributeValueTypeDef,
@@ -619,19 +622,20 @@
     UpdateTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyUpdateTypeDef,
     CreateBackupOutputTypeDef,
     ListBackupsOutputTableTypeDef,
     ListBackupsOutputTypeDef,
     BatchGetItemInputServiceResourceBatchGetItemTypeDef,
-    BatchStatementResponseTypeDef,
     ConsumedCapacityServiceResourceTypeDef,
     ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
+    QueryInputQueryPaginateTypeDef,
     QueryInputTableQueryTypeDef,
+    ScanInputScanPaginateTypeDef,
     ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
     LocalSecondaryIndexDescriptionTableTypeDef,
     CreateGlobalSecondaryIndexActionTableTypeDef,
     UpdateGlobalSecondaryIndexActionTableTypeDef,
     LocalSecondaryIndexDescriptionTypeDef,
@@ -665,24 +669,20 @@
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
     GlobalSecondaryIndexDescriptionTableTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
     ImportSummaryTypeDef,
-    ListBackupsInputListBackupsPaginateTypeDef,
-    ListTablesInputListTablesPaginateTypeDef,
-    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    QueryInputQueryPaginateTypeDef,
-    ScanInputScanPaginateTypeDef,
     ListTagsOfResourceOutputTableTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
     WriteRequestServiceResourceTypeDef,
     UpdateTimeToLiveInputRequestTypeDef,
     UpdateTimeToLiveOutputTypeDef,
+    BatchStatementResponseTypeDef,
     BatchExecuteStatementInputRequestTypeDef,
     QueryInputRequestTypeDef,
     ScanInputRequestTypeDef,
     DeleteItemInputRequestTypeDef,
     PutItemInputRequestTypeDef,
     UpdateItemInputRequestTypeDef,
     TransactGetItemTypeDef,
@@ -695,15 +695,14 @@
     BatchGetItemOutputServiceResourceTypeDef,
     DeleteItemOutputTableTypeDef,
     GetItemOutputTableTypeDef,
     PutItemOutputTableTypeDef,
     QueryOutputTableTypeDef,
     ScanOutputTableTypeDef,
     UpdateItemOutputTableTypeDef,
-    BatchExecuteStatementOutputTypeDef,
     BatchGetItemOutputTypeDef,
     DeleteItemOutputTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     GetItemOutputTypeDef,
     PutItemOutputTypeDef,
     QueryOutputTypeDef,
@@ -728,14 +727,15 @@
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
     CreateTableInputServiceResourceCreateTableTypeDef,
     ListImportsOutputTypeDef,
     BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     BatchWriteItemOutputServiceResourceTypeDef,
+    BatchExecuteStatementOutputTypeDef,
     TransactGetItemsInputRequestTypeDef,
     BatchWriteItemInputRequestTypeDef,
     BatchWriteItemOutputTypeDef,
     TransactWriteItemsInputRequestTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
@@ -776,15 +776,15 @@
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> ArchivalSummaryResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/README.md` & `mypy-boto3-dynamodb-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-dynamodb"></a>
 
 # mypy-boto3-dynamodb
 
 [![PyPI - mypy-boto3-dynamodb](https://img.shields.io/pypi/v/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dynamodb?color=blue)](https://pypistats.org/packages/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -449,30 +449,30 @@
 ### Typed dictionaries
 
 `mypy_boto3_dynamodb.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodb.type_defs import (
-    ResponseMetadataTypeDef,
+    ArchivalSummaryResponseMetadataTypeDef,
     ArchivalSummaryTableTypeDef,
     ArchivalSummaryTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
     AttributeValueTypeDef,
     AttributeValueUpdateTableTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
     BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
-    BatchStatementErrorTypeDef,
     ItemCollectionMetricsServiceResourceTypeDef,
+    BillingModeSummaryResponseMetadataTypeDef,
     BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
     CapacityServiceResourceTypeDef,
     CapacityTableTypeDef,
     CapacityTypeDef,
     ConditionTableTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
@@ -515,64 +515,67 @@
     DescribeExportInputRequestTypeDef,
     ExportDescriptionTypeDef,
     DescribeGlobalTableInputRequestTypeDef,
     DescribeGlobalTableSettingsInputRequestTypeDef,
     DescribeImportInputRequestTypeDef,
     DescribeKinesisStreamingDestinationInputRequestTypeDef,
     KinesisDataStreamDestinationTypeDef,
+    DescribeLimitsOutputTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportSummaryTypeDef,
     ExportTableToPointInTimeInputRequestTypeDef,
     GetItemInputTableGetItemTypeDef,
     ProvisionedThroughputDescriptionTableTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
     ProjectionServiceResourceTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    KinesisStreamingDestinationOutputTypeDef,
+    ListBackupsInputListBackupsPaginateTypeDef,
     ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
+    ListTablesInputListTablesPaginateTypeDef,
     ListTablesInputRequestTypeDef,
+    ListTablesOutputTableTypeDef,
+    ListTablesOutputTypeDef,
+    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
     TagTableTypeDef,
+    PaginatorConfigTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
+    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
     PutRequestServiceResourceTypeDef,
     TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
+    ResponseMetadataTypeDef,
+    RestoreSummaryResponseMetadataTypeDef,
     RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
+    SSEDescriptionResponseMetadataTypeDef,
     SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
     SSESpecificationTableTypeDef,
+    StreamSpecificationResponseMetadataTypeDef,
     StreamSpecificationTableTypeDef,
     TableBatchWriterRequestTypeDef,
+    TableClassSummaryResponseMetadataTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
-    ArchivalSummaryResponseMetadataTypeDef,
-    BillingModeSummaryResponseMetadataTypeDef,
-    DescribeLimitsOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    KinesisStreamingDestinationOutputTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTablesOutputTypeDef,
-    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
-    RestoreSummaryResponseMetadataTypeDef,
-    SSEDescriptionResponseMetadataTypeDef,
-    StreamSpecificationResponseMetadataTypeDef,
-    TableClassSummaryResponseMetadataTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     AttributeValueUpdateTypeDef,
+    BatchStatementErrorTypeDef,
     BatchStatementRequestTypeDef,
     ConditionCheckTypeDef,
     ConditionTypeDef,
     DeleteRequestTypeDef,
     DeleteTypeDef,
     ExecuteStatementInputRequestTypeDef,
     ExpectedAttributeValueTypeDef,
@@ -587,19 +590,20 @@
     UpdateTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyUpdateTypeDef,
     CreateBackupOutputTypeDef,
     ListBackupsOutputTableTypeDef,
     ListBackupsOutputTypeDef,
     BatchGetItemInputServiceResourceBatchGetItemTypeDef,
-    BatchStatementResponseTypeDef,
     ConsumedCapacityServiceResourceTypeDef,
     ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
+    QueryInputQueryPaginateTypeDef,
     QueryInputTableQueryTypeDef,
+    ScanInputScanPaginateTypeDef,
     ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
     LocalSecondaryIndexDescriptionTableTypeDef,
     CreateGlobalSecondaryIndexActionTableTypeDef,
     UpdateGlobalSecondaryIndexActionTableTypeDef,
     LocalSecondaryIndexDescriptionTypeDef,
@@ -633,24 +637,20 @@
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
     GlobalSecondaryIndexDescriptionTableTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
     ImportSummaryTypeDef,
-    ListBackupsInputListBackupsPaginateTypeDef,
-    ListTablesInputListTablesPaginateTypeDef,
-    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    QueryInputQueryPaginateTypeDef,
-    ScanInputScanPaginateTypeDef,
     ListTagsOfResourceOutputTableTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
     WriteRequestServiceResourceTypeDef,
     UpdateTimeToLiveInputRequestTypeDef,
     UpdateTimeToLiveOutputTypeDef,
+    BatchStatementResponseTypeDef,
     BatchExecuteStatementInputRequestTypeDef,
     QueryInputRequestTypeDef,
     ScanInputRequestTypeDef,
     DeleteItemInputRequestTypeDef,
     PutItemInputRequestTypeDef,
     UpdateItemInputRequestTypeDef,
     TransactGetItemTypeDef,
@@ -663,15 +663,14 @@
     BatchGetItemOutputServiceResourceTypeDef,
     DeleteItemOutputTableTypeDef,
     GetItemOutputTableTypeDef,
     PutItemOutputTableTypeDef,
     QueryOutputTableTypeDef,
     ScanOutputTableTypeDef,
     UpdateItemOutputTableTypeDef,
-    BatchExecuteStatementOutputTypeDef,
     BatchGetItemOutputTypeDef,
     DeleteItemOutputTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     GetItemOutputTypeDef,
     PutItemOutputTypeDef,
     QueryOutputTypeDef,
@@ -696,14 +695,15 @@
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
     CreateTableInputServiceResourceCreateTableTypeDef,
     ListImportsOutputTypeDef,
     BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     BatchWriteItemOutputServiceResourceTypeDef,
+    BatchExecuteStatementOutputTypeDef,
     TransactGetItemsInputRequestTypeDef,
     BatchWriteItemInputRequestTypeDef,
     BatchWriteItemOutputTypeDef,
     TransactWriteItemsInputRequestTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
@@ -744,15 +744,15 @@
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> ArchivalSummaryResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/__init__.py` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/__init__.pyi` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/__main__.py` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DynamoDB 1.26.97\nVersion:         1.26.97.post1\nBuilder"
-        " version: 7.14.1\nDocs:           "
+        "Type annotations for boto3.DynamoDB 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.97.post1")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/client.py` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     ConditionalOperatorType,
     ContributorInsightsActionType,
     ExportFormatType,
     InputCompressionTypeType,
     InputFormatType,
     ReturnConsumedCapacityType,
     ReturnItemCollectionMetricsType,
+    ReturnValuesOnConditionCheckFailureType,
     ReturnValueType,
     S3SseAlgorithmType,
     SelectType,
     TableClassType,
 )
 from .paginator import (
     ListBackupsPaginator,
@@ -356,15 +357,16 @@
                     Set[bytes],
                     Set[bytearray],
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ],
-        ] = ...
+        ] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.delete_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#delete_item)
         """
@@ -541,15 +543,16 @@
                     None,
                 ],
             ]
         ] = ...,
         ConsistentRead: bool = ...,
         NextToken: str = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
-        Limit: int = ...
+        Limit: int = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> ExecuteStatementOutputTypeDef:
         """
         This operation allows you to perform reads and singleton writes on data stored
         in DynamoDB, using PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.execute_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#execute_statement)
@@ -790,15 +793,16 @@
                     Set[bytes],
                     Set[bytearray],
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ],
-        ] = ...
+        ] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.put_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#put_item)
         """
@@ -1144,15 +1148,16 @@
                     Set[bytes],
                     Set[bytearray],
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ],
-        ] = ...
+        ] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#update_item)
```

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/client.pyi` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     ConditionalOperatorType,
     ContributorInsightsActionType,
     ExportFormatType,
     InputCompressionTypeType,
     InputFormatType,
     ReturnConsumedCapacityType,
     ReturnItemCollectionMetricsType,
+    ReturnValuesOnConditionCheckFailureType,
     ReturnValueType,
     S3SseAlgorithmType,
     SelectType,
     TableClassType,
 )
 from .paginator import (
     ListBackupsPaginator,
@@ -342,15 +343,16 @@
                     Set[bytes],
                     Set[bytearray],
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ],
-        ] = ...
+        ] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.delete_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#delete_item)
         """
@@ -510,15 +512,16 @@
                     None,
                 ],
             ]
         ] = ...,
         ConsistentRead: bool = ...,
         NextToken: str = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
-        Limit: int = ...
+        Limit: int = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> ExecuteStatementOutputTypeDef:
         """
         This operation allows you to perform reads and singleton writes on data stored
         in DynamoDB, using PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.execute_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#execute_statement)
@@ -746,15 +749,16 @@
                     Set[bytes],
                     Set[bytearray],
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ],
-        ] = ...
+        ] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.put_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#put_item)
         """
@@ -1087,15 +1091,16 @@
                     Set[bytes],
                     Set[bytearray],
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ],
-        ] = ...
+        ] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/client/#update_item)
```

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/literals.py` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,15 @@
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
@@ -216,14 +217,15 @@
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
@@ -321,14 +323,15 @@
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
@@ -364,14 +367,15 @@
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
@@ -390,16 +394,19 @@
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
@@ -483,15 +490,17 @@
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

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/literals.pyi` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,15 @@
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
@@ -214,14 +215,15 @@
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
@@ -319,14 +321,15 @@
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
@@ -362,14 +365,15 @@
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
@@ -388,16 +392,19 @@
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
@@ -481,15 +488,17 @@
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

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/paginator.py` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,45 +77,45 @@
     def paginate(
         self,
         *,
         TableName: str = ...,
         TimeRangeLowerBound: Union[datetime, str] = ...,
         TimeRangeUpperBound: Union[datetime, str] = ...,
         BackupType: BackupTypeFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupsOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listbackupspaginator)
         """
 
 
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTablesOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtablespaginator)
         """
 
 
 class ListTagsOfResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtagsofresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsOfResourceOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtagsofresourcepaginator)
         """
 
 
@@ -157,15 +157,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[QueryOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#querypaginator)
         """
 
 
@@ -206,13 +206,13 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ConsistentRead: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ScanOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/paginator.pyi` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -74,43 +74,43 @@
     def paginate(
         self,
         *,
         TableName: str = ...,
         TimeRangeLowerBound: Union[datetime, str] = ...,
         TimeRangeUpperBound: Union[datetime, str] = ...,
         BackupType: BackupTypeFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBackupsOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listbackupspaginator)
         """
 
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTablesOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtablespaginator)
         """
 
 class ListTagsOfResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtagsofresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListTagsOfResourceOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#listtagsofresourcepaginator)
         """
 
 class QueryPaginator(Paginator):
@@ -151,15 +151,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[QueryOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#querypaginator)
         """
 
 class ScanPaginator(Paginator):
@@ -199,13 +199,13 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ] = ...,
         ConsistentRead: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ScanOutputTableTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/service_resource.py` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/service_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 from .client import DynamoDBClient
 from .literals import (
     BillingModeType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
     ReturnItemCollectionMetricsType,
+    ReturnValuesOnConditionCheckFailureType,
     ReturnValueType,
     SelectType,
     TableClassType,
     TableStatusType,
 )
 from .type_defs import (
     ArchivalSummaryResponseMetadataTypeDef,
@@ -229,15 +230,16 @@
                 Set[str],
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
-        ] = ...
+        ] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> DeleteItemOutputTableTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tabledelete_item-method)
         """
@@ -338,15 +340,16 @@
                 Set[str],
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
-        ] = ...
+        ] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> PutItemOutputTableTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.put_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableput_item-method)
         """
@@ -553,15 +556,16 @@
                 Set[str],
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
-        ] = ...
+        ] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> UpdateItemOutputTableTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableupdate_item-method)
```

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/service_resource.pyi` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/service_resource.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 from .client import DynamoDBClient
 from .literals import (
     BillingModeType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
     ReturnItemCollectionMetricsType,
+    ReturnValuesOnConditionCheckFailureType,
     ReturnValueType,
     SelectType,
     TableClassType,
     TableStatusType,
 )
 from .type_defs import (
     ArchivalSummaryResponseMetadataTypeDef,
@@ -220,15 +221,16 @@
                 Set[str],
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
-        ] = ...
+        ] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> DeleteItemOutputTableTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tabledelete_item-method)
         """
@@ -325,15 +327,16 @@
                 Set[str],
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
-        ] = ...
+        ] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> PutItemOutputTableTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.put_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableput_item-method)
         """
@@ -535,15 +538,16 @@
                 Set[str],
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
-        ] = ...
+        ] = ...,
+        ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...
     ) -> UpdateItemOutputTableTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/service_resource/#tableupdate_item-method)
```

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/type_defs.py` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for dynamodb service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_dynamodb.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_dynamodb.type_defs import ArchivalSummaryResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ArchivalSummaryResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from decimal import Decimal
 from typing import Any, Dict, List, Mapping, Sequence, Set, Union
 
@@ -60,30 +60,30 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ResponseMetadataTypeDef",
+    "ArchivalSummaryResponseMetadataTypeDef",
     "ArchivalSummaryTableTypeDef",
     "ArchivalSummaryTypeDef",
     "AttributeDefinitionServiceResourceTypeDef",
     "AttributeDefinitionTableTypeDef",
     "AttributeDefinitionTypeDef",
     "AttributeValueTypeDef",
     "AttributeValueUpdateTableTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
     "BackupSummaryTableTypeDef",
     "BackupSummaryTypeDef",
     "KeysAndAttributesServiceResourceTypeDef",
-    "BatchStatementErrorTypeDef",
     "ItemCollectionMetricsServiceResourceTypeDef",
+    "BillingModeSummaryResponseMetadataTypeDef",
     "BillingModeSummaryTableTypeDef",
     "BillingModeSummaryTypeDef",
     "CapacityServiceResourceTypeDef",
     "CapacityTableTypeDef",
     "CapacityTypeDef",
     "ConditionTableTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
@@ -126,64 +126,67 @@
     "DescribeExportInputRequestTypeDef",
     "ExportDescriptionTypeDef",
     "DescribeGlobalTableInputRequestTypeDef",
     "DescribeGlobalTableSettingsInputRequestTypeDef",
     "DescribeImportInputRequestTypeDef",
     "DescribeKinesisStreamingDestinationInputRequestTypeDef",
     "KinesisDataStreamDestinationTypeDef",
+    "DescribeLimitsOutputTypeDef",
     "DescribeTableInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTableReplicaAutoScalingInputRequestTypeDef",
     "DescribeTimeToLiveInputRequestTypeDef",
     "TimeToLiveDescriptionTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportSummaryTypeDef",
     "ExportTableToPointInTimeInputRequestTypeDef",
     "GetItemInputTableGetItemTypeDef",
     "ProvisionedThroughputDescriptionTableTypeDef",
     "ProvisionedThroughputDescriptionTypeDef",
     "ProjectionServiceResourceTypeDef",
     "S3BucketSourceTypeDef",
     "KinesisStreamingDestinationInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "KinesisStreamingDestinationOutputTypeDef",
+    "ListBackupsInputListBackupsPaginateTypeDef",
     "ListBackupsInputRequestTypeDef",
     "ListContributorInsightsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListGlobalTablesInputRequestTypeDef",
     "ListImportsInputRequestTypeDef",
+    "ListTablesInputListTablesPaginateTypeDef",
     "ListTablesInputRequestTypeDef",
+    "ListTablesOutputTableTypeDef",
+    "ListTablesOutputTypeDef",
+    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     "ListTagsOfResourceInputRequestTypeDef",
     "TagTableTypeDef",
+    "PaginatorConfigTypeDef",
     "PointInTimeRecoverySpecificationTypeDef",
+    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
     "PutRequestServiceResourceTypeDef",
     "TableClassSummaryTableTypeDef",
     "TableClassSummaryTypeDef",
+    "ResponseMetadataTypeDef",
+    "RestoreSummaryResponseMetadataTypeDef",
     "RestoreSummaryTableTypeDef",
     "RestoreSummaryTypeDef",
+    "SSEDescriptionResponseMetadataTypeDef",
     "SSEDescriptionTableTypeDef",
     "SSEDescriptionTypeDef",
     "SSESpecificationTableTypeDef",
+    "StreamSpecificationResponseMetadataTypeDef",
     "StreamSpecificationTableTypeDef",
     "TableBatchWriterRequestTypeDef",
+    "TableClassSummaryResponseMetadataTypeDef",
     "TimeToLiveSpecificationTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateContributorInsightsInputRequestTypeDef",
-    "ArchivalSummaryResponseMetadataTypeDef",
-    "BillingModeSummaryResponseMetadataTypeDef",
-    "DescribeLimitsOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "KinesisStreamingDestinationOutputTypeDef",
-    "ListTablesOutputTableTypeDef",
-    "ListTablesOutputTypeDef",
-    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
-    "RestoreSummaryResponseMetadataTypeDef",
-    "SSEDescriptionResponseMetadataTypeDef",
-    "StreamSpecificationResponseMetadataTypeDef",
-    "TableClassSummaryResponseMetadataTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
     "AttributeValueUpdateTypeDef",
+    "BatchStatementErrorTypeDef",
     "BatchStatementRequestTypeDef",
     "ConditionCheckTypeDef",
     "ConditionTypeDef",
     "DeleteRequestTypeDef",
     "DeleteTypeDef",
     "ExecuteStatementInputRequestTypeDef",
     "ExpectedAttributeValueTypeDef",
@@ -198,19 +201,20 @@
     "UpdateTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyUpdateTypeDef",
     "CreateBackupOutputTypeDef",
     "ListBackupsOutputTableTypeDef",
     "ListBackupsOutputTypeDef",
     "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
-    "BatchStatementResponseTypeDef",
     "ConsumedCapacityServiceResourceTypeDef",
     "ConsumedCapacityTableTypeDef",
     "ConsumedCapacityTypeDef",
+    "QueryInputQueryPaginateTypeDef",
     "QueryInputTableQueryTypeDef",
+    "ScanInputScanPaginateTypeDef",
     "ScanInputTableScanTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
     "LocalSecondaryIndexDescriptionTableTypeDef",
     "CreateGlobalSecondaryIndexActionTableTypeDef",
     "UpdateGlobalSecondaryIndexActionTableTypeDef",
     "LocalSecondaryIndexDescriptionTypeDef",
@@ -244,24 +248,20 @@
     "DescribeTimeToLiveOutputTypeDef",
     "ListExportsOutputTypeDef",
     "GlobalSecondaryIndexDescriptionTableTypeDef",
     "GlobalSecondaryIndexDescriptionTypeDef",
     "GlobalSecondaryIndexServiceResourceTypeDef",
     "LocalSecondaryIndexServiceResourceTypeDef",
     "ImportSummaryTypeDef",
-    "ListBackupsInputListBackupsPaginateTypeDef",
-    "ListTablesInputListTablesPaginateTypeDef",
-    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    "QueryInputQueryPaginateTypeDef",
-    "ScanInputScanPaginateTypeDef",
     "ListTagsOfResourceOutputTableTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
     "WriteRequestServiceResourceTypeDef",
     "UpdateTimeToLiveInputRequestTypeDef",
     "UpdateTimeToLiveOutputTypeDef",
+    "BatchStatementResponseTypeDef",
     "BatchExecuteStatementInputRequestTypeDef",
     "QueryInputRequestTypeDef",
     "ScanInputRequestTypeDef",
     "DeleteItemInputRequestTypeDef",
     "PutItemInputRequestTypeDef",
     "UpdateItemInputRequestTypeDef",
     "TransactGetItemTypeDef",
@@ -274,15 +274,14 @@
     "BatchGetItemOutputServiceResourceTypeDef",
     "DeleteItemOutputTableTypeDef",
     "GetItemOutputTableTypeDef",
     "PutItemOutputTableTypeDef",
     "QueryOutputTableTypeDef",
     "ScanOutputTableTypeDef",
     "UpdateItemOutputTableTypeDef",
-    "BatchExecuteStatementOutputTypeDef",
     "BatchGetItemOutputTypeDef",
     "DeleteItemOutputTypeDef",
     "ExecuteStatementOutputTypeDef",
     "ExecuteTransactionOutputTypeDef",
     "GetItemOutputTypeDef",
     "PutItemOutputTypeDef",
     "QueryOutputTypeDef",
@@ -307,14 +306,15 @@
     "CreateReplicationGroupMemberActionTypeDef",
     "UpdateReplicationGroupMemberActionTypeDef",
     "UpdateGlobalTableInputRequestTypeDef",
     "CreateTableInputServiceResourceCreateTableTypeDef",
     "ListImportsOutputTypeDef",
     "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     "BatchWriteItemOutputServiceResourceTypeDef",
+    "BatchExecuteStatementOutputTypeDef",
     "TransactGetItemsInputRequestTypeDef",
     "BatchWriteItemInputRequestTypeDef",
     "BatchWriteItemOutputTypeDef",
     "TransactWriteItemsInputRequestTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
@@ -354,22 +354,21 @@
     "UpdateGlobalTableSettingsOutputTypeDef",
     "UpdateTableReplicaAutoScalingInputRequestTypeDef",
     "UpdateGlobalTableSettingsInputRequestTypeDef",
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     "UpdateTableReplicaAutoScalingOutputTypeDef",
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ArchivalSummaryResponseMetadataTypeDef = TypedDict(
+    "ArchivalSummaryResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ArchivalDateTime": datetime,
+        "ArchivalReason": str,
+        "ArchivalBackupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ArchivalSummaryTableTypeDef = TypedDict(
     "ArchivalSummaryTableTypeDef",
     {
         "ArchivalDateTime": datetime,
@@ -601,23 +600,14 @@
 class KeysAndAttributesServiceResourceTypeDef(
     _RequiredKeysAndAttributesServiceResourceTypeDef,
     _OptionalKeysAndAttributesServiceResourceTypeDef,
 ):
     pass
 
 
-BatchStatementErrorTypeDef = TypedDict(
-    "BatchStatementErrorTypeDef",
-    {
-        "Code": BatchStatementErrorCodeEnumType,
-        "Message": str,
-    },
-    total=False,
-)
-
 ItemCollectionMetricsServiceResourceTypeDef = TypedDict(
     "ItemCollectionMetricsServiceResourceTypeDef",
     {
         "ItemCollectionKey": Dict[
             str,
             Union[
                 bytes,
@@ -637,14 +627,23 @@
             ],
         ],
         "SizeEstimateRangeGB": List[float],
     },
     total=False,
 )
 
+BillingModeSummaryResponseMetadataTypeDef = TypedDict(
+    "BillingModeSummaryResponseMetadataTypeDef",
+    {
+        "BillingMode": BillingModeType,
+        "LastUpdateToPayPerRequestDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BillingModeSummaryTableTypeDef = TypedDict(
     "BillingModeSummaryTableTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
     total=False,
@@ -1202,14 +1201,25 @@
         "StreamArn": str,
         "DestinationStatus": DestinationStatusType,
         "DestinationStatusDescription": str,
     },
     total=False,
 )
 
+DescribeLimitsOutputTypeDef = TypedDict(
+    "DescribeLimitsOutputTypeDef",
+    {
+        "AccountMaxReadCapacityUnits": int,
+        "AccountMaxWriteCapacityUnits": int,
+        "TableMaxReadCapacityUnits": int,
+        "TableMaxWriteCapacityUnits": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeTableInputRequestTypeDef = TypedDict(
     "DescribeTableInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 
@@ -1241,14 +1251,21 @@
     {
         "TimeToLiveStatus": TimeToLiveStatusType,
         "AttributeName": str,
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
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "ExportArn": str,
         "ExportStatus": ExportStatusType,
     },
     total=False,
@@ -1383,20 +1400,32 @@
     "KinesisStreamingDestinationInputRequestTypeDef",
     {
         "TableName": str,
         "StreamArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+KinesisStreamingDestinationOutputTypeDef = TypedDict(
+    "KinesisStreamingDestinationOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TableName": str,
+        "StreamArn": str,
+        "DestinationStatus": DestinationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
+    "ListBackupsInputListBackupsPaginateTypeDef",
+    {
+        "TableName": str,
+        "TimeRangeLowerBound": Union[datetime, str],
+        "TimeRangeUpperBound": Union[datetime, str],
+        "BackupType": BackupTypeFilterType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBackupsInputRequestTypeDef = TypedDict(
     "ListBackupsInputRequestTypeDef",
     {
@@ -1446,23 +1475,71 @@
         "TableArn": str,
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListTablesInputListTablesPaginateTypeDef = TypedDict(
+    "ListTablesInputListTablesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTablesInputRequestTypeDef = TypedDict(
     "ListTablesInputRequestTypeDef",
     {
         "ExclusiveStartTableName": str,
         "Limit": int,
     },
     total=False,
 )
 
+ListTablesOutputTableTypeDef = TypedDict(
+    "ListTablesOutputTableTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTablesOutputTypeDef = TypedDict(
+    "ListTablesOutputTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
+    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListTagsOfResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsOfResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsOfResourceInputRequestTypeDef = TypedDict(
@@ -1484,21 +1561,43 @@
     "TagTableTypeDef",
     {
         "Key": str,
         "Value": str,
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
 PointInTimeRecoverySpecificationTypeDef = TypedDict(
     "PointInTimeRecoverySpecificationTypeDef",
     {
         "PointInTimeRecoveryEnabled": bool,
     },
 )
 
+ProvisionedThroughputDescriptionResponseMetadataTypeDef = TypedDict(
+    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
+    {
+        "LastIncreaseDateTime": datetime,
+        "LastDecreaseDateTime": datetime,
+        "NumberOfDecreasesToday": int,
+        "ReadCapacityUnits": int,
+        "WriteCapacityUnits": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutRequestServiceResourceTypeDef = TypedDict(
     "PutRequestServiceResourceTypeDef",
     {
         "Item": Mapping[
             str,
             Union[
                 bytes,
@@ -1534,14 +1633,36 @@
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
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
+RestoreSummaryResponseMetadataTypeDef = TypedDict(
+    "RestoreSummaryResponseMetadataTypeDef",
+    {
+        "SourceBackupArn": str,
+        "SourceTableArn": str,
+        "RestoreDateTime": datetime,
+        "RestoreInProgress": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRestoreSummaryTableTypeDef = TypedDict(
     "_RequiredRestoreSummaryTableTypeDef",
     {
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
     },
 )
@@ -1578,14 +1699,25 @@
 )
 
 
 class RestoreSummaryTypeDef(_RequiredRestoreSummaryTypeDef, _OptionalRestoreSummaryTypeDef):
     pass
 
 
+SSEDescriptionResponseMetadataTypeDef = TypedDict(
+    "SSEDescriptionResponseMetadataTypeDef",
+    {
+        "Status": SSEStatusType,
+        "SSEType": SSETypeType,
+        "KMSMasterKeyArn": str,
+        "InaccessibleEncryptionDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SSEDescriptionTableTypeDef = TypedDict(
     "SSEDescriptionTableTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
@@ -1610,14 +1742,23 @@
         "Enabled": bool,
         "SSEType": SSETypeType,
         "KMSMasterKeyId": str,
     },
     total=False,
 )
 
+StreamSpecificationResponseMetadataTypeDef = TypedDict(
+    "StreamSpecificationResponseMetadataTypeDef",
+    {
+        "StreamEnabled": bool,
+        "StreamViewType": StreamViewTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStreamSpecificationTableTypeDef = TypedDict(
     "_RequiredStreamSpecificationTableTypeDef",
     {
         "StreamEnabled": bool,
     },
 )
 _OptionalStreamSpecificationTableTypeDef = TypedDict(
@@ -1639,14 +1780,23 @@
     "TableBatchWriterRequestTypeDef",
     {
         "overwrite_by_pkeys": List[str],
     },
     total=False,
 )
 
+TableClassSummaryResponseMetadataTypeDef = TypedDict(
+    "TableClassSummaryResponseMetadataTypeDef",
+    {
+        "TableClass": TableClassType,
+        "LastUpdateDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TimeToLiveSpecificationTypeDef = TypedDict(
     "TimeToLiveSpecificationTypeDef",
     {
         "Enabled": bool,
         "AttributeName": str,
     },
 )
@@ -1678,138 +1828,21 @@
 class UpdateContributorInsightsInputRequestTypeDef(
     _RequiredUpdateContributorInsightsInputRequestTypeDef,
     _OptionalUpdateContributorInsightsInputRequestTypeDef,
 ):
     pass
 
 
-ArchivalSummaryResponseMetadataTypeDef = TypedDict(
-    "ArchivalSummaryResponseMetadataTypeDef",
-    {
-        "ArchivalDateTime": datetime,
-        "ArchivalReason": str,
-        "ArchivalBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BillingModeSummaryResponseMetadataTypeDef = TypedDict(
-    "BillingModeSummaryResponseMetadataTypeDef",
-    {
-        "BillingMode": BillingModeType,
-        "LastUpdateToPayPerRequestDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeLimitsOutputTypeDef = TypedDict(
-    "DescribeLimitsOutputTypeDef",
-    {
-        "AccountMaxReadCapacityUnits": int,
-        "AccountMaxWriteCapacityUnits": int,
-        "TableMaxReadCapacityUnits": int,
-        "TableMaxWriteCapacityUnits": int,
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
-KinesisStreamingDestinationOutputTypeDef = TypedDict(
-    "KinesisStreamingDestinationOutputTypeDef",
-    {
-        "TableName": str,
-        "StreamArn": str,
-        "DestinationStatus": DestinationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTablesOutputTableTypeDef = TypedDict(
-    "ListTablesOutputTableTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTablesOutputTypeDef = TypedDict(
-    "ListTablesOutputTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ProvisionedThroughputDescriptionResponseMetadataTypeDef = TypedDict(
-    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
-    {
-        "LastIncreaseDateTime": datetime,
-        "LastDecreaseDateTime": datetime,
-        "NumberOfDecreasesToday": int,
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RestoreSummaryResponseMetadataTypeDef = TypedDict(
-    "RestoreSummaryResponseMetadataTypeDef",
-    {
-        "SourceBackupArn": str,
-        "SourceTableArn": str,
-        "RestoreDateTime": datetime,
-        "RestoreInProgress": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SSEDescriptionResponseMetadataTypeDef = TypedDict(
-    "SSEDescriptionResponseMetadataTypeDef",
-    {
-        "Status": SSEStatusType,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyArn": str,
-        "InaccessibleEncryptionDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StreamSpecificationResponseMetadataTypeDef = TypedDict(
-    "StreamSpecificationResponseMetadataTypeDef",
-    {
-        "StreamEnabled": bool,
-        "StreamViewType": StreamViewTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TableClassSummaryResponseMetadataTypeDef = TypedDict(
-    "TableClassSummaryResponseMetadataTypeDef",
-    {
-        "TableClass": TableClassType,
-        "LastUpdateDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateContributorInsightsOutputTypeDef = TypedDict(
     "UpdateContributorInsightsOutputTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttributeValueUpdateTypeDef = TypedDict(
     "AttributeValueUpdateTypeDef",
     {
         "Value": Union[
@@ -1832,14 +1865,24 @@
             ],
         ],
         "Action": AttributeActionType,
     },
     total=False,
 )
 
+BatchStatementErrorTypeDef = TypedDict(
+    "BatchStatementErrorTypeDef",
+    {
+        "Code": BatchStatementErrorCodeEnumType,
+        "Message": str,
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+    total=False,
+)
+
 _RequiredBatchStatementRequestTypeDef = TypedDict(
     "_RequiredBatchStatementRequestTypeDef",
     {
         "Statement": str,
     },
 )
 _OptionalBatchStatementRequestTypeDef = TypedDict(
@@ -1863,14 +1906,15 @@
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ]
         ],
         "ConsistentRead": bool,
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class BatchStatementRequestTypeDef(
     _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
@@ -2105,14 +2149,15 @@
                 ],
             ]
         ],
         "ConsistentRead": bool,
         "NextToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "Limit": int,
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class ExecuteStatementInputRequestTypeDef(
     _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
@@ -2348,14 +2393,15 @@
                     Set[bytearray],
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ]
         ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class ParameterizedStatementTypeDef(
     _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
@@ -2556,33 +2602,33 @@
     pass
 
 
 CreateBackupOutputTypeDef = TypedDict(
     "CreateBackupOutputTypeDef",
     {
         "BackupDetails": BackupDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBackupsOutputTableTypeDef = TypedDict(
     "ListBackupsOutputTableTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTableTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBackupsOutputTypeDef = TypedDict(
     "ListBackupsOutputTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
     "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
     {
         "RequestItems": Mapping[str, KeysAndAttributesServiceResourceTypeDef],
@@ -2600,24 +2646,14 @@
 class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
     _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
     _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
 ):
     pass
 
 
-BatchStatementResponseTypeDef = TypedDict(
-    "BatchStatementResponseTypeDef",
-    {
-        "Error": BatchStatementErrorTypeDef,
-        "TableName": str,
-        "Item": Dict[str, AttributeValueTypeDef],
-    },
-    total=False,
-)
-
 ConsumedCapacityServiceResourceTypeDef = TypedDict(
     "ConsumedCapacityServiceResourceTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
@@ -2652,14 +2688,67 @@
         "Table": CapacityTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTypeDef],
     },
     total=False,
 )
 
+_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryInputQueryPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryInputQueryPaginateTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTableTypeDef],
+        "QueryFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class QueryInputQueryPaginateTypeDef(
+    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
+):
+    pass
+
+
 QueryInputTableQueryTypeDef = TypedDict(
     "QueryInputTableQueryTypeDef",
     {
         "IndexName": str,
         "Select": SelectType,
         "AttributesToGet": Sequence[str],
         "Limit": int,
@@ -2711,14 +2800,66 @@
                 None,
             ],
         ],
     },
     total=False,
 )
 
+_RequiredScanInputScanPaginateTypeDef = TypedDict(
+    "_RequiredScanInputScanPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalScanInputScanPaginateTypeDef = TypedDict(
+    "_OptionalScanInputScanPaginateTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "ConsistentRead": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ScanInputScanPaginateTypeDef(
+    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
+):
+    pass
+
+
 ScanInputTableScanTypeDef = TypedDict(
     "ScanInputTableScanTypeDef",
     {
         "IndexName": str,
         "AttributesToGet": Sequence[str],
         "Limit": int,
         "Select": SelectType,
@@ -2795,15 +2936,15 @@
 
 
 ListContributorInsightsOutputTypeDef = TypedDict(
     "ListContributorInsightsOutputTypeDef",
     {
         "ContributorInsightsSummaries": List[ContributorInsightsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
     "LocalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
@@ -3053,15 +3194,15 @@
 
 
 ListTagsOfResourceOutputTypeDef = TypedDict(
     "ListTagsOfResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
@@ -3126,14 +3267,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class DeleteItemInputTableDeleteItemTypeDef(
     _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
@@ -3190,14 +3332,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class PutItemInputTablePutItemTypeDef(
     _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
@@ -3256,14 +3399,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class UpdateItemInputTableUpdateItemTypeDef(
     _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
@@ -3285,48 +3429,48 @@
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsRuleList": List[str],
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "LastUpdateDateTime": datetime,
         "FailureException": FailureExceptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExportOutputTypeDef = TypedDict(
     "DescribeExportOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportTableToPointInTimeOutputTypeDef = TypedDict(
     "ExportTableToPointInTimeOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeKinesisStreamingDestinationOutputTypeDef = TypedDict(
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     {
         "TableName": str,
         "KinesisDataStreamDestinations": List[KinesisDataStreamDestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeTableInputTableExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeTableInputTableExistsWaitTypeDef",
     {
         "TableName": str,
@@ -3370,24 +3514,24 @@
     pass
 
 
 DescribeTimeToLiveOutputTypeDef = TypedDict(
     "DescribeTimeToLiveOutputTypeDef",
     {
         "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "ExportSummaries": List[ExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
@@ -3463,167 +3607,20 @@
         "InputFormat": InputFormatType,
         "StartTime": datetime,
         "EndTime": datetime,
     },
     total=False,
 )
 
-ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
-    "ListBackupsInputListBackupsPaginateTypeDef",
-    {
-        "TableName": str,
-        "TimeRangeLowerBound": Union[datetime, str],
-        "TimeRangeUpperBound": Union[datetime, str],
-        "BackupType": BackupTypeFilterType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTablesInputListTablesPaginateTypeDef = TypedDict(
-    "ListTablesInputListTablesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
-    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-):
-    pass
-
-
-_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryInputQueryPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryInputQueryPaginateTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTableTypeDef],
-        "QueryFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class QueryInputQueryPaginateTypeDef(
-    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
-):
-    pass
-
-
-_RequiredScanInputScanPaginateTypeDef = TypedDict(
-    "_RequiredScanInputScanPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalScanInputScanPaginateTypeDef = TypedDict(
-    "_OptionalScanInputScanPaginateTypeDef",
-    {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ConsistentRead": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ScanInputScanPaginateTypeDef(
-    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
-):
-    pass
-
-
 ListTagsOfResourceOutputTableTypeDef = TypedDict(
     "ListTagsOfResourceOutputTableTypeDef",
     {
         "Tags": List[TagTableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContinuousBackupsInputRequestTypeDef = TypedDict(
     "UpdateContinuousBackupsInputRequestTypeDef",
     {
         "TableName": str,
@@ -3648,18 +3645,28 @@
     },
 )
 
 UpdateTimeToLiveOutputTypeDef = TypedDict(
     "UpdateTimeToLiveOutputTypeDef",
     {
         "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+BatchStatementResponseTypeDef = TypedDict(
+    "BatchStatementResponseTypeDef",
+    {
+        "Error": BatchStatementErrorTypeDef,
+        "TableName": str,
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+    total=False,
+)
+
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
     {
         "Statements": Sequence[BatchStatementRequestTypeDef],
     },
 )
 _OptionalBatchExecuteStatementInputRequestTypeDef = TypedDict(
@@ -3887,14 +3894,15 @@
                     Set[bytearray],
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ],
         ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class DeleteItemInputRequestTypeDef(
     _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
@@ -3958,14 +3966,15 @@
                     Set[bytearray],
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ],
         ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class PutItemInputRequestTypeDef(
     _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
@@ -4031,14 +4040,15 @@
                     Set[bytearray],
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ],
         ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
 class UpdateItemInputRequestTypeDef(
     _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
@@ -4165,15 +4175,15 @@
                         None,
                     ],
                 ]
             ],
         ],
         "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteItemOutputTableTypeDef = TypedDict(
     "DeleteItemOutputTableTypeDef",
     {
         "Attributes": Dict[
@@ -4193,15 +4203,15 @@
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetItemOutputTableTypeDef = TypedDict(
     "GetItemOutputTableTypeDef",
     {
         "Item": Dict[
@@ -4220,15 +4230,15 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutItemOutputTableTypeDef = TypedDict(
     "PutItemOutputTableTypeDef",
     {
         "Attributes": Dict[
@@ -4248,15 +4258,15 @@
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryOutputTableTypeDef = TypedDict(
     "QueryOutputTableTypeDef",
     {
         "Items": List[
@@ -4298,15 +4308,15 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScanOutputTableTypeDef = TypedDict(
     "ScanOutputTableTypeDef",
     {
         "Items": List[
@@ -4348,15 +4358,15 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateItemOutputTableTypeDef = TypedDict(
     "UpdateItemOutputTableTypeDef",
     {
         "Attributes": Dict[
@@ -4376,151 +4386,142 @@
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchExecuteStatementOutputTypeDef = TypedDict(
-    "BatchExecuteStatementOutputTypeDef",
-    {
-        "Responses": List[BatchStatementResponseTypeDef],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetItemOutputTypeDef = TypedDict(
     "BatchGetItemOutputTypeDef",
     {
         "Responses": Dict[str, List[Dict[str, AttributeValueTypeDef]]],
         "UnprocessedKeys": Dict[str, KeysAndAttributesTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteItemOutputTypeDef = TypedDict(
     "DeleteItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExecuteStatementOutputTypeDef = TypedDict(
     "ExecuteStatementOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "NextToken": str,
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExecuteTransactionOutputTypeDef = TypedDict(
     "ExecuteTransactionOutputTypeDef",
     {
         "Responses": List[ItemResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetItemOutputTypeDef = TypedDict(
     "GetItemOutputTypeDef",
     {
         "Item": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutItemOutputTypeDef = TypedDict(
     "PutItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryOutputTypeDef = TypedDict(
     "QueryOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScanOutputTypeDef = TypedDict(
     "ScanOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TransactGetItemsOutputTypeDef = TypedDict(
     "TransactGetItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "Responses": List[ItemResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TransactWriteItemsOutputTypeDef = TypedDict(
     "TransactWriteItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateItemOutputTypeDef = TypedDict(
     "UpdateItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContinuousBackupsOutputTypeDef = TypedDict(
     "DescribeContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContinuousBackupsOutputTypeDef = TypedDict(
     "UpdateContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GlobalSecondaryIndexUpdateTableTypeDef = TypedDict(
     "GlobalSecondaryIndexUpdateTableTypeDef",
     {
         "Update": UpdateGlobalSecondaryIndexActionTableTypeDef,
@@ -4667,15 +4668,15 @@
 )
 
 ListGlobalTablesOutputTypeDef = TypedDict(
     "ListGlobalTablesOutputTypeDef",
     {
         "GlobalTables": List[GlobalTableTypeDef],
         "LastEvaluatedGlobalTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicaDescriptionTableTypeDef = TypedDict(
     "ReplicaDescriptionTableTypeDef",
     {
         "RegionName": str,
@@ -4848,15 +4849,15 @@
 
 
 ListImportsOutputTypeDef = TypedDict(
     "ListImportsOutputTypeDef",
     {
         "ImportSummaryList": List[ImportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
     "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     {
         "RequestItems": Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
@@ -4881,15 +4882,24 @@
 
 BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
     "BatchWriteItemOutputServiceResourceTypeDef",
     {
         "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceTypeDef]],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
         "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchExecuteStatementOutputTypeDef = TypedDict(
+    "BatchExecuteStatementOutputTypeDef",
+    {
+        "Responses": List[BatchStatementResponseTypeDef],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactGetItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactGetItemTypeDef],
@@ -4934,15 +4944,15 @@
 
 BatchWriteItemOutputTypeDef = TypedDict(
     "BatchWriteItemOutputTypeDef",
     {
         "UnprocessedItems": Dict[str, List[WriteRequestTypeDef]],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTransactWriteItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactWriteItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactWriteItemTypeDef],
@@ -5311,47 +5321,47 @@
     pass
 
 
 DeleteBackupOutputTypeDef = TypedDict(
     "DeleteBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBackupOutputTypeDef = TypedDict(
     "DescribeBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImportOutputTypeDef = TypedDict(
     "DescribeImportOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportTableOutputTypeDef = TypedDict(
     "ImportTableOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteTableOutputTableTypeDef = TypedDict(
     "DeleteTableOutputTableTypeDef",
     {
         "TableDescription": TableDescriptionTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTableInputTableUpdateTypeDef = TypedDict(
     "UpdateTableInputTableUpdateTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionTableTypeDef],
@@ -5367,79 +5377,79 @@
     total=False,
 )
 
 CreateGlobalTableOutputTypeDef = TypedDict(
     "CreateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeGlobalTableOutputTypeDef = TypedDict(
     "DescribeGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGlobalTableOutputTypeDef = TypedDict(
     "UpdateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTableOutputTypeDef = TypedDict(
     "CreateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteTableOutputTypeDef = TypedDict(
     "DeleteTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTableOutputTypeDef = TypedDict(
     "DescribeTableOutputTypeDef",
     {
         "Table": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreTableFromBackupOutputTypeDef = TypedDict(
     "RestoreTableFromBackupOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreTableToPointInTimeOutputTypeDef = TypedDict(
     "RestoreTableToPointInTimeOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTableOutputTypeDef = TypedDict(
     "UpdateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateTableInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTableInputRequestTypeDef",
     {
         "TableName": str,
@@ -5479,24 +5489,24 @@
 )
 
 DescribeGlobalTableSettingsOutputTypeDef = TypedDict(
     "DescribeGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGlobalTableSettingsOutputTypeDef = TypedDict(
     "UpdateGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef",
     {
         "TableName": str,
@@ -5550,18 +5560,18 @@
     pass
 
 
 DescribeTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "UpdateTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/type_defs.pyi` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for dynamodb service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_dynamodb.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_dynamodb.type_defs import ArchivalSummaryResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ArchivalSummaryResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from decimal import Decimal
 from typing import Any, Dict, List, Mapping, Sequence, Set, Union
 
@@ -59,30 +59,30 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ResponseMetadataTypeDef",
+    "ArchivalSummaryResponseMetadataTypeDef",
     "ArchivalSummaryTableTypeDef",
     "ArchivalSummaryTypeDef",
     "AttributeDefinitionServiceResourceTypeDef",
     "AttributeDefinitionTableTypeDef",
     "AttributeDefinitionTypeDef",
     "AttributeValueTypeDef",
     "AttributeValueUpdateTableTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
     "BackupSummaryTableTypeDef",
     "BackupSummaryTypeDef",
     "KeysAndAttributesServiceResourceTypeDef",
-    "BatchStatementErrorTypeDef",
     "ItemCollectionMetricsServiceResourceTypeDef",
+    "BillingModeSummaryResponseMetadataTypeDef",
     "BillingModeSummaryTableTypeDef",
     "BillingModeSummaryTypeDef",
     "CapacityServiceResourceTypeDef",
     "CapacityTableTypeDef",
     "CapacityTypeDef",
     "ConditionTableTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
@@ -125,64 +125,67 @@
     "DescribeExportInputRequestTypeDef",
     "ExportDescriptionTypeDef",
     "DescribeGlobalTableInputRequestTypeDef",
     "DescribeGlobalTableSettingsInputRequestTypeDef",
     "DescribeImportInputRequestTypeDef",
     "DescribeKinesisStreamingDestinationInputRequestTypeDef",
     "KinesisDataStreamDestinationTypeDef",
+    "DescribeLimitsOutputTypeDef",
     "DescribeTableInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTableReplicaAutoScalingInputRequestTypeDef",
     "DescribeTimeToLiveInputRequestTypeDef",
     "TimeToLiveDescriptionTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ExportSummaryTypeDef",
     "ExportTableToPointInTimeInputRequestTypeDef",
     "GetItemInputTableGetItemTypeDef",
     "ProvisionedThroughputDescriptionTableTypeDef",
     "ProvisionedThroughputDescriptionTypeDef",
     "ProjectionServiceResourceTypeDef",
     "S3BucketSourceTypeDef",
     "KinesisStreamingDestinationInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "KinesisStreamingDestinationOutputTypeDef",
+    "ListBackupsInputListBackupsPaginateTypeDef",
     "ListBackupsInputRequestTypeDef",
     "ListContributorInsightsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListGlobalTablesInputRequestTypeDef",
     "ListImportsInputRequestTypeDef",
+    "ListTablesInputListTablesPaginateTypeDef",
     "ListTablesInputRequestTypeDef",
+    "ListTablesOutputTableTypeDef",
+    "ListTablesOutputTypeDef",
+    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
     "ListTagsOfResourceInputRequestTypeDef",
     "TagTableTypeDef",
+    "PaginatorConfigTypeDef",
     "PointInTimeRecoverySpecificationTypeDef",
+    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
     "PutRequestServiceResourceTypeDef",
     "TableClassSummaryTableTypeDef",
     "TableClassSummaryTypeDef",
+    "ResponseMetadataTypeDef",
+    "RestoreSummaryResponseMetadataTypeDef",
     "RestoreSummaryTableTypeDef",
     "RestoreSummaryTypeDef",
+    "SSEDescriptionResponseMetadataTypeDef",
     "SSEDescriptionTableTypeDef",
     "SSEDescriptionTypeDef",
     "SSESpecificationTableTypeDef",
+    "StreamSpecificationResponseMetadataTypeDef",
     "StreamSpecificationTableTypeDef",
     "TableBatchWriterRequestTypeDef",
+    "TableClassSummaryResponseMetadataTypeDef",
     "TimeToLiveSpecificationTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateContributorInsightsInputRequestTypeDef",
-    "ArchivalSummaryResponseMetadataTypeDef",
-    "BillingModeSummaryResponseMetadataTypeDef",
-    "DescribeLimitsOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "KinesisStreamingDestinationOutputTypeDef",
-    "ListTablesOutputTableTypeDef",
-    "ListTablesOutputTypeDef",
-    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
-    "RestoreSummaryResponseMetadataTypeDef",
-    "SSEDescriptionResponseMetadataTypeDef",
-    "StreamSpecificationResponseMetadataTypeDef",
-    "TableClassSummaryResponseMetadataTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
     "AttributeValueUpdateTypeDef",
+    "BatchStatementErrorTypeDef",
     "BatchStatementRequestTypeDef",
     "ConditionCheckTypeDef",
     "ConditionTypeDef",
     "DeleteRequestTypeDef",
     "DeleteTypeDef",
     "ExecuteStatementInputRequestTypeDef",
     "ExpectedAttributeValueTypeDef",
@@ -197,19 +200,20 @@
     "UpdateTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyUpdateTypeDef",
     "CreateBackupOutputTypeDef",
     "ListBackupsOutputTableTypeDef",
     "ListBackupsOutputTypeDef",
     "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
-    "BatchStatementResponseTypeDef",
     "ConsumedCapacityServiceResourceTypeDef",
     "ConsumedCapacityTableTypeDef",
     "ConsumedCapacityTypeDef",
+    "QueryInputQueryPaginateTypeDef",
     "QueryInputTableQueryTypeDef",
+    "ScanInputScanPaginateTypeDef",
     "ScanInputTableScanTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
     "LocalSecondaryIndexDescriptionTableTypeDef",
     "CreateGlobalSecondaryIndexActionTableTypeDef",
     "UpdateGlobalSecondaryIndexActionTableTypeDef",
     "LocalSecondaryIndexDescriptionTypeDef",
@@ -243,24 +247,20 @@
     "DescribeTimeToLiveOutputTypeDef",
     "ListExportsOutputTypeDef",
     "GlobalSecondaryIndexDescriptionTableTypeDef",
     "GlobalSecondaryIndexDescriptionTypeDef",
     "GlobalSecondaryIndexServiceResourceTypeDef",
     "LocalSecondaryIndexServiceResourceTypeDef",
     "ImportSummaryTypeDef",
-    "ListBackupsInputListBackupsPaginateTypeDef",
-    "ListTablesInputListTablesPaginateTypeDef",
-    "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    "QueryInputQueryPaginateTypeDef",
-    "ScanInputScanPaginateTypeDef",
     "ListTagsOfResourceOutputTableTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
     "WriteRequestServiceResourceTypeDef",
     "UpdateTimeToLiveInputRequestTypeDef",
     "UpdateTimeToLiveOutputTypeDef",
+    "BatchStatementResponseTypeDef",
     "BatchExecuteStatementInputRequestTypeDef",
     "QueryInputRequestTypeDef",
     "ScanInputRequestTypeDef",
     "DeleteItemInputRequestTypeDef",
     "PutItemInputRequestTypeDef",
     "UpdateItemInputRequestTypeDef",
     "TransactGetItemTypeDef",
@@ -273,15 +273,14 @@
     "BatchGetItemOutputServiceResourceTypeDef",
     "DeleteItemOutputTableTypeDef",
     "GetItemOutputTableTypeDef",
     "PutItemOutputTableTypeDef",
     "QueryOutputTableTypeDef",
     "ScanOutputTableTypeDef",
     "UpdateItemOutputTableTypeDef",
-    "BatchExecuteStatementOutputTypeDef",
     "BatchGetItemOutputTypeDef",
     "DeleteItemOutputTypeDef",
     "ExecuteStatementOutputTypeDef",
     "ExecuteTransactionOutputTypeDef",
     "GetItemOutputTypeDef",
     "PutItemOutputTypeDef",
     "QueryOutputTypeDef",
@@ -306,14 +305,15 @@
     "CreateReplicationGroupMemberActionTypeDef",
     "UpdateReplicationGroupMemberActionTypeDef",
     "UpdateGlobalTableInputRequestTypeDef",
     "CreateTableInputServiceResourceCreateTableTypeDef",
     "ListImportsOutputTypeDef",
     "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     "BatchWriteItemOutputServiceResourceTypeDef",
+    "BatchExecuteStatementOutputTypeDef",
     "TransactGetItemsInputRequestTypeDef",
     "BatchWriteItemInputRequestTypeDef",
     "BatchWriteItemOutputTypeDef",
     "TransactWriteItemsInputRequestTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
@@ -353,22 +353,21 @@
     "UpdateGlobalTableSettingsOutputTypeDef",
     "UpdateTableReplicaAutoScalingInputRequestTypeDef",
     "UpdateGlobalTableSettingsInputRequestTypeDef",
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     "UpdateTableReplicaAutoScalingOutputTypeDef",
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ArchivalSummaryResponseMetadataTypeDef = TypedDict(
+    "ArchivalSummaryResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ArchivalDateTime": datetime,
+        "ArchivalReason": str,
+        "ArchivalBackupArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ArchivalSummaryTableTypeDef = TypedDict(
     "ArchivalSummaryTableTypeDef",
     {
         "ArchivalDateTime": datetime,
@@ -592,23 +591,14 @@
 
 class KeysAndAttributesServiceResourceTypeDef(
     _RequiredKeysAndAttributesServiceResourceTypeDef,
     _OptionalKeysAndAttributesServiceResourceTypeDef,
 ):
     pass
 
-BatchStatementErrorTypeDef = TypedDict(
-    "BatchStatementErrorTypeDef",
-    {
-        "Code": BatchStatementErrorCodeEnumType,
-        "Message": str,
-    },
-    total=False,
-)
-
 ItemCollectionMetricsServiceResourceTypeDef = TypedDict(
     "ItemCollectionMetricsServiceResourceTypeDef",
     {
         "ItemCollectionKey": Dict[
             str,
             Union[
                 bytes,
@@ -628,14 +618,23 @@
             ],
         ],
         "SizeEstimateRangeGB": List[float],
     },
     total=False,
 )
 
+BillingModeSummaryResponseMetadataTypeDef = TypedDict(
+    "BillingModeSummaryResponseMetadataTypeDef",
+    {
+        "BillingMode": BillingModeType,
+        "LastUpdateToPayPerRequestDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BillingModeSummaryTableTypeDef = TypedDict(
     "BillingModeSummaryTableTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
     total=False,
@@ -1185,14 +1184,25 @@
         "StreamArn": str,
         "DestinationStatus": DestinationStatusType,
         "DestinationStatusDescription": str,
     },
     total=False,
 )
 
+DescribeLimitsOutputTypeDef = TypedDict(
+    "DescribeLimitsOutputTypeDef",
+    {
+        "AccountMaxReadCapacityUnits": int,
+        "AccountMaxWriteCapacityUnits": int,
+        "TableMaxReadCapacityUnits": int,
+        "TableMaxWriteCapacityUnits": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeTableInputRequestTypeDef = TypedDict(
     "DescribeTableInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 
@@ -1224,14 +1234,21 @@
     {
         "TimeToLiveStatus": TimeToLiveStatusType,
         "AttributeName": str,
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
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "ExportArn": str,
         "ExportStatus": ExportStatusType,
     },
     total=False,
@@ -1360,20 +1377,32 @@
     "KinesisStreamingDestinationInputRequestTypeDef",
     {
         "TableName": str,
         "StreamArn": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+KinesisStreamingDestinationOutputTypeDef = TypedDict(
+    "KinesisStreamingDestinationOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TableName": str,
+        "StreamArn": str,
+        "DestinationStatus": DestinationStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
+    "ListBackupsInputListBackupsPaginateTypeDef",
+    {
+        "TableName": str,
+        "TimeRangeLowerBound": Union[datetime, str],
+        "TimeRangeUpperBound": Union[datetime, str],
+        "BackupType": BackupTypeFilterType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBackupsInputRequestTypeDef = TypedDict(
     "ListBackupsInputRequestTypeDef",
     {
@@ -1423,23 +1452,69 @@
         "TableArn": str,
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListTablesInputListTablesPaginateTypeDef = TypedDict(
+    "ListTablesInputListTablesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListTablesInputRequestTypeDef = TypedDict(
     "ListTablesInputRequestTypeDef",
     {
         "ExclusiveStartTableName": str,
         "Limit": int,
     },
     total=False,
 )
 
+ListTablesOutputTableTypeDef = TypedDict(
+    "ListTablesOutputTableTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTablesOutputTypeDef = TypedDict(
+    "ListTablesOutputTypeDef",
+    {
+        "TableNames": List[str],
+        "LastEvaluatedTableName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
+    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
+):
+    pass
+
 _RequiredListTagsOfResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsOfResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsOfResourceInputRequestTypeDef = TypedDict(
@@ -1459,21 +1534,43 @@
     "TagTableTypeDef",
     {
         "Key": str,
         "Value": str,
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
 PointInTimeRecoverySpecificationTypeDef = TypedDict(
     "PointInTimeRecoverySpecificationTypeDef",
     {
         "PointInTimeRecoveryEnabled": bool,
     },
 )
 
+ProvisionedThroughputDescriptionResponseMetadataTypeDef = TypedDict(
+    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
+    {
+        "LastIncreaseDateTime": datetime,
+        "LastDecreaseDateTime": datetime,
+        "NumberOfDecreasesToday": int,
+        "ReadCapacityUnits": int,
+        "WriteCapacityUnits": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutRequestServiceResourceTypeDef = TypedDict(
     "PutRequestServiceResourceTypeDef",
     {
         "Item": Mapping[
             str,
             Union[
                 bytes,
@@ -1509,14 +1606,36 @@
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
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
+RestoreSummaryResponseMetadataTypeDef = TypedDict(
+    "RestoreSummaryResponseMetadataTypeDef",
+    {
+        "SourceBackupArn": str,
+        "SourceTableArn": str,
+        "RestoreDateTime": datetime,
+        "RestoreInProgress": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRestoreSummaryTableTypeDef = TypedDict(
     "_RequiredRestoreSummaryTableTypeDef",
     {
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
     },
 )
@@ -1549,14 +1668,25 @@
     },
     total=False,
 )
 
 class RestoreSummaryTypeDef(_RequiredRestoreSummaryTypeDef, _OptionalRestoreSummaryTypeDef):
     pass
 
+SSEDescriptionResponseMetadataTypeDef = TypedDict(
+    "SSEDescriptionResponseMetadataTypeDef",
+    {
+        "Status": SSEStatusType,
+        "SSEType": SSETypeType,
+        "KMSMasterKeyArn": str,
+        "InaccessibleEncryptionDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SSEDescriptionTableTypeDef = TypedDict(
     "SSEDescriptionTableTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
@@ -1581,14 +1711,23 @@
         "Enabled": bool,
         "SSEType": SSETypeType,
         "KMSMasterKeyId": str,
     },
     total=False,
 )
 
+StreamSpecificationResponseMetadataTypeDef = TypedDict(
+    "StreamSpecificationResponseMetadataTypeDef",
+    {
+        "StreamEnabled": bool,
+        "StreamViewType": StreamViewTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStreamSpecificationTableTypeDef = TypedDict(
     "_RequiredStreamSpecificationTableTypeDef",
     {
         "StreamEnabled": bool,
     },
 )
 _OptionalStreamSpecificationTableTypeDef = TypedDict(
@@ -1608,14 +1747,23 @@
     "TableBatchWriterRequestTypeDef",
     {
         "overwrite_by_pkeys": List[str],
     },
     total=False,
 )
 
+TableClassSummaryResponseMetadataTypeDef = TypedDict(
+    "TableClassSummaryResponseMetadataTypeDef",
+    {
+        "TableClass": TableClassType,
+        "LastUpdateDateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TimeToLiveSpecificationTypeDef = TypedDict(
     "TimeToLiveSpecificationTypeDef",
     {
         "Enabled": bool,
         "AttributeName": str,
     },
 )
@@ -1645,138 +1793,21 @@
 
 class UpdateContributorInsightsInputRequestTypeDef(
     _RequiredUpdateContributorInsightsInputRequestTypeDef,
     _OptionalUpdateContributorInsightsInputRequestTypeDef,
 ):
     pass
 
-ArchivalSummaryResponseMetadataTypeDef = TypedDict(
-    "ArchivalSummaryResponseMetadataTypeDef",
-    {
-        "ArchivalDateTime": datetime,
-        "ArchivalReason": str,
-        "ArchivalBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BillingModeSummaryResponseMetadataTypeDef = TypedDict(
-    "BillingModeSummaryResponseMetadataTypeDef",
-    {
-        "BillingMode": BillingModeType,
-        "LastUpdateToPayPerRequestDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeLimitsOutputTypeDef = TypedDict(
-    "DescribeLimitsOutputTypeDef",
-    {
-        "AccountMaxReadCapacityUnits": int,
-        "AccountMaxWriteCapacityUnits": int,
-        "TableMaxReadCapacityUnits": int,
-        "TableMaxWriteCapacityUnits": int,
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
-KinesisStreamingDestinationOutputTypeDef = TypedDict(
-    "KinesisStreamingDestinationOutputTypeDef",
-    {
-        "TableName": str,
-        "StreamArn": str,
-        "DestinationStatus": DestinationStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTablesOutputTableTypeDef = TypedDict(
-    "ListTablesOutputTableTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTablesOutputTypeDef = TypedDict(
-    "ListTablesOutputTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ProvisionedThroughputDescriptionResponseMetadataTypeDef = TypedDict(
-    "ProvisionedThroughputDescriptionResponseMetadataTypeDef",
-    {
-        "LastIncreaseDateTime": datetime,
-        "LastDecreaseDateTime": datetime,
-        "NumberOfDecreasesToday": int,
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RestoreSummaryResponseMetadataTypeDef = TypedDict(
-    "RestoreSummaryResponseMetadataTypeDef",
-    {
-        "SourceBackupArn": str,
-        "SourceTableArn": str,
-        "RestoreDateTime": datetime,
-        "RestoreInProgress": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SSEDescriptionResponseMetadataTypeDef = TypedDict(
-    "SSEDescriptionResponseMetadataTypeDef",
-    {
-        "Status": SSEStatusType,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyArn": str,
-        "InaccessibleEncryptionDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StreamSpecificationResponseMetadataTypeDef = TypedDict(
-    "StreamSpecificationResponseMetadataTypeDef",
-    {
-        "StreamEnabled": bool,
-        "StreamViewType": StreamViewTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-TableClassSummaryResponseMetadataTypeDef = TypedDict(
-    "TableClassSummaryResponseMetadataTypeDef",
-    {
-        "TableClass": TableClassType,
-        "LastUpdateDateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateContributorInsightsOutputTypeDef = TypedDict(
     "UpdateContributorInsightsOutputTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttributeValueUpdateTypeDef = TypedDict(
     "AttributeValueUpdateTypeDef",
     {
         "Value": Union[
@@ -1799,14 +1830,24 @@
             ],
         ],
         "Action": AttributeActionType,
     },
     total=False,
 )
 
+BatchStatementErrorTypeDef = TypedDict(
+    "BatchStatementErrorTypeDef",
+    {
+        "Code": BatchStatementErrorCodeEnumType,
+        "Message": str,
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+    total=False,
+)
+
 _RequiredBatchStatementRequestTypeDef = TypedDict(
     "_RequiredBatchStatementRequestTypeDef",
     {
         "Statement": str,
     },
 )
 _OptionalBatchStatementRequestTypeDef = TypedDict(
@@ -1830,14 +1871,15 @@
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ]
         ],
         "ConsistentRead": bool,
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class BatchStatementRequestTypeDef(
     _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
 ):
@@ -2064,14 +2106,15 @@
                 ],
             ]
         ],
         "ConsistentRead": bool,
         "NextToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "Limit": int,
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class ExecuteStatementInputRequestTypeDef(
     _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
 ):
@@ -2299,14 +2342,15 @@
                     Set[bytearray],
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ]
         ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class ParameterizedStatementTypeDef(
     _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
 ):
@@ -2499,33 +2543,33 @@
 ):
     pass
 
 CreateBackupOutputTypeDef = TypedDict(
     "CreateBackupOutputTypeDef",
     {
         "BackupDetails": BackupDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBackupsOutputTableTypeDef = TypedDict(
     "ListBackupsOutputTableTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTableTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBackupsOutputTypeDef = TypedDict(
     "ListBackupsOutputTypeDef",
     {
         "BackupSummaries": List[BackupSummaryTypeDef],
         "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
     "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
     {
         "RequestItems": Mapping[str, KeysAndAttributesServiceResourceTypeDef],
@@ -2541,24 +2585,14 @@
 
 class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
     _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
     _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
 ):
     pass
 
-BatchStatementResponseTypeDef = TypedDict(
-    "BatchStatementResponseTypeDef",
-    {
-        "Error": BatchStatementErrorTypeDef,
-        "TableName": str,
-        "Item": Dict[str, AttributeValueTypeDef],
-    },
-    total=False,
-)
-
 ConsumedCapacityServiceResourceTypeDef = TypedDict(
     "ConsumedCapacityServiceResourceTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
@@ -2593,14 +2627,65 @@
         "Table": CapacityTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTypeDef],
     },
     total=False,
 )
 
+_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryInputQueryPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryInputQueryPaginateTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTableTypeDef],
+        "QueryFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class QueryInputQueryPaginateTypeDef(
+    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
+):
+    pass
+
 QueryInputTableQueryTypeDef = TypedDict(
     "QueryInputTableQueryTypeDef",
     {
         "IndexName": str,
         "Select": SelectType,
         "AttributesToGet": Sequence[str],
         "Limit": int,
@@ -2652,14 +2737,64 @@
                 None,
             ],
         ],
     },
     total=False,
 )
 
+_RequiredScanInputScanPaginateTypeDef = TypedDict(
+    "_RequiredScanInputScanPaginateTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalScanInputScanPaginateTypeDef = TypedDict(
+    "_OptionalScanInputScanPaginateTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTableTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[
+            str,
+            Union[
+                bytes,
+                bytearray,
+                str,
+                int,
+                Decimal,
+                bool,
+                Set[int],
+                Set[Decimal],
+                Set[str],
+                Set[bytes],
+                Set[bytearray],
+                Sequence[Any],
+                Mapping[str, Any],
+                None,
+            ],
+        ],
+        "ConsistentRead": bool,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ScanInputScanPaginateTypeDef(
+    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
+):
+    pass
+
 ScanInputTableScanTypeDef = TypedDict(
     "ScanInputTableScanTypeDef",
     {
         "IndexName": str,
         "AttributesToGet": Sequence[str],
         "Limit": int,
         "Select": SelectType,
@@ -2734,15 +2869,15 @@
     pass
 
 ListContributorInsightsOutputTypeDef = TypedDict(
     "ListContributorInsightsOutputTypeDef",
     {
         "ContributorInsightsSummaries": List[ContributorInsightsSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
     "LocalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
@@ -2980,15 +3115,15 @@
     pass
 
 ListTagsOfResourceOutputTypeDef = TypedDict(
     "ListTagsOfResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
@@ -3053,14 +3188,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class DeleteItemInputTableDeleteItemTypeDef(
     _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
 ):
@@ -3115,14 +3251,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class PutItemInputTablePutItemTypeDef(
     _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
 ):
@@ -3179,14 +3316,15 @@
                 Set[bytes],
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class UpdateItemInputTableUpdateItemTypeDef(
     _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
 ):
@@ -3206,48 +3344,48 @@
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsRuleList": List[str],
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "LastUpdateDateTime": datetime,
         "FailureException": FailureExceptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeExportOutputTypeDef = TypedDict(
     "DescribeExportOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportTableToPointInTimeOutputTypeDef = TypedDict(
     "ExportTableToPointInTimeOutputTypeDef",
     {
         "ExportDescription": ExportDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeKinesisStreamingDestinationOutputTypeDef = TypedDict(
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     {
         "TableName": str,
         "KinesisDataStreamDestinations": List[KinesisDataStreamDestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeTableInputTableExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeTableInputTableExistsWaitTypeDef",
     {
         "TableName": str,
@@ -3287,24 +3425,24 @@
 ):
     pass
 
 DescribeTimeToLiveOutputTypeDef = TypedDict(
     "DescribeTimeToLiveOutputTypeDef",
     {
         "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "ExportSummaries": List[ExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
     "GlobalSecondaryIndexDescriptionTableTypeDef",
     {
         "IndexName": str,
@@ -3378,161 +3516,20 @@
         "InputFormat": InputFormatType,
         "StartTime": datetime,
         "EndTime": datetime,
     },
     total=False,
 )
 
-ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
-    "ListBackupsInputListBackupsPaginateTypeDef",
-    {
-        "TableName": str,
-        "TimeRangeLowerBound": Union[datetime, str],
-        "TimeRangeUpperBound": Union[datetime, str],
-        "BackupType": BackupTypeFilterType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListTablesInputListTablesPaginateTypeDef = TypedDict(
-    "ListTablesInputListTablesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
-    _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-):
-    pass
-
-_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryInputQueryPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryInputQueryPaginateTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTableTypeDef],
-        "QueryFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class QueryInputQueryPaginateTypeDef(
-    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
-):
-    pass
-
-_RequiredScanInputScanPaginateTypeDef = TypedDict(
-    "_RequiredScanInputScanPaginateTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalScanInputScanPaginateTypeDef = TypedDict(
-    "_OptionalScanInputScanPaginateTypeDef",
-    {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ConsistentRead": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ScanInputScanPaginateTypeDef(
-    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
-):
-    pass
-
 ListTagsOfResourceOutputTableTypeDef = TypedDict(
     "ListTagsOfResourceOutputTableTypeDef",
     {
         "Tags": List[TagTableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContinuousBackupsInputRequestTypeDef = TypedDict(
     "UpdateContinuousBackupsInputRequestTypeDef",
     {
         "TableName": str,
@@ -3557,18 +3554,28 @@
     },
 )
 
 UpdateTimeToLiveOutputTypeDef = TypedDict(
     "UpdateTimeToLiveOutputTypeDef",
     {
         "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+BatchStatementResponseTypeDef = TypedDict(
+    "BatchStatementResponseTypeDef",
+    {
+        "Error": BatchStatementErrorTypeDef,
+        "TableName": str,
+        "Item": Dict[str, AttributeValueTypeDef],
+    },
+    total=False,
+)
+
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
     {
         "Statements": Sequence[BatchStatementRequestTypeDef],
     },
 )
 _OptionalBatchExecuteStatementInputRequestTypeDef = TypedDict(
@@ -3790,14 +3797,15 @@
                     Set[bytearray],
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ],
         ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class DeleteItemInputRequestTypeDef(
     _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
 ):
@@ -3859,14 +3867,15 @@
                     Set[bytearray],
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ],
         ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class PutItemInputRequestTypeDef(
     _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
 ):
@@ -3930,14 +3939,15 @@
                     Set[bytearray],
                     Sequence[Any],
                     Mapping[str, Any],
                     None,
                 ],
             ],
         ],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 class UpdateItemInputRequestTypeDef(
     _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
 ):
@@ -4058,15 +4068,15 @@
                         None,
                     ],
                 ]
             ],
         ],
         "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteItemOutputTableTypeDef = TypedDict(
     "DeleteItemOutputTableTypeDef",
     {
         "Attributes": Dict[
@@ -4086,15 +4096,15 @@
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetItemOutputTableTypeDef = TypedDict(
     "GetItemOutputTableTypeDef",
     {
         "Item": Dict[
@@ -4113,15 +4123,15 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutItemOutputTableTypeDef = TypedDict(
     "PutItemOutputTableTypeDef",
     {
         "Attributes": Dict[
@@ -4141,15 +4151,15 @@
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryOutputTableTypeDef = TypedDict(
     "QueryOutputTableTypeDef",
     {
         "Items": List[
@@ -4191,15 +4201,15 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScanOutputTableTypeDef = TypedDict(
     "ScanOutputTableTypeDef",
     {
         "Items": List[
@@ -4241,15 +4251,15 @@
                 Set[bytearray],
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateItemOutputTableTypeDef = TypedDict(
     "UpdateItemOutputTableTypeDef",
     {
         "Attributes": Dict[
@@ -4269,151 +4279,142 @@
                 Sequence[Any],
                 Mapping[str, Any],
                 None,
             ],
         ],
         "ConsumedCapacity": ConsumedCapacityTableTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchExecuteStatementOutputTypeDef = TypedDict(
-    "BatchExecuteStatementOutputTypeDef",
-    {
-        "Responses": List[BatchStatementResponseTypeDef],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetItemOutputTypeDef = TypedDict(
     "BatchGetItemOutputTypeDef",
     {
         "Responses": Dict[str, List[Dict[str, AttributeValueTypeDef]]],
         "UnprocessedKeys": Dict[str, KeysAndAttributesTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteItemOutputTypeDef = TypedDict(
     "DeleteItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExecuteStatementOutputTypeDef = TypedDict(
     "ExecuteStatementOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "NextToken": str,
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExecuteTransactionOutputTypeDef = TypedDict(
     "ExecuteTransactionOutputTypeDef",
     {
         "Responses": List[ItemResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetItemOutputTypeDef = TypedDict(
     "GetItemOutputTypeDef",
     {
         "Item": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutItemOutputTypeDef = TypedDict(
     "PutItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 QueryOutputTypeDef = TypedDict(
     "QueryOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ScanOutputTypeDef = TypedDict(
     "ScanOutputTypeDef",
     {
         "Items": List[Dict[str, AttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
         "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TransactGetItemsOutputTypeDef = TypedDict(
     "TransactGetItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "Responses": List[ItemResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TransactWriteItemsOutputTypeDef = TypedDict(
     "TransactWriteItemsOutputTypeDef",
     {
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateItemOutputTypeDef = TypedDict(
     "UpdateItemOutputTypeDef",
     {
         "Attributes": Dict[str, AttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeContinuousBackupsOutputTypeDef = TypedDict(
     "DescribeContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateContinuousBackupsOutputTypeDef = TypedDict(
     "UpdateContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GlobalSecondaryIndexUpdateTableTypeDef = TypedDict(
     "GlobalSecondaryIndexUpdateTableTypeDef",
     {
         "Update": UpdateGlobalSecondaryIndexActionTableTypeDef,
@@ -4552,15 +4553,15 @@
 )
 
 ListGlobalTablesOutputTypeDef = TypedDict(
     "ListGlobalTablesOutputTypeDef",
     {
         "GlobalTables": List[GlobalTableTypeDef],
         "LastEvaluatedGlobalTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReplicaDescriptionTableTypeDef = TypedDict(
     "ReplicaDescriptionTableTypeDef",
     {
         "RegionName": str,
@@ -4723,15 +4724,15 @@
     pass
 
 ListImportsOutputTypeDef = TypedDict(
     "ListImportsOutputTypeDef",
     {
         "ImportSummaryList": List[ImportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
     "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     {
         "RequestItems": Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
@@ -4754,15 +4755,24 @@
 
 BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
     "BatchWriteItemOutputServiceResourceTypeDef",
     {
         "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceTypeDef]],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
         "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchExecuteStatementOutputTypeDef = TypedDict(
+    "BatchExecuteStatementOutputTypeDef",
+    {
+        "Responses": List[BatchStatementResponseTypeDef],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactGetItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactGetItemTypeDef],
@@ -4803,15 +4813,15 @@
 
 BatchWriteItemOutputTypeDef = TypedDict(
     "BatchWriteItemOutputTypeDef",
     {
         "UnprocessedItems": Dict[str, List[WriteRequestTypeDef]],
         "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTransactWriteItemsInputRequestTypeDef = TypedDict(
     "_RequiredTransactWriteItemsInputRequestTypeDef",
     {
         "TransactItems": Sequence[TransactWriteItemTypeDef],
@@ -5164,47 +5174,47 @@
 ):
     pass
 
 DeleteBackupOutputTypeDef = TypedDict(
     "DeleteBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeBackupOutputTypeDef = TypedDict(
     "DescribeBackupOutputTypeDef",
     {
         "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeImportOutputTypeDef = TypedDict(
     "DescribeImportOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImportTableOutputTypeDef = TypedDict(
     "ImportTableOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteTableOutputTableTypeDef = TypedDict(
     "DeleteTableOutputTableTypeDef",
     {
         "TableDescription": TableDescriptionTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTableInputTableUpdateTypeDef = TypedDict(
     "UpdateTableInputTableUpdateTypeDef",
     {
         "AttributeDefinitions": Sequence[AttributeDefinitionTableTypeDef],
@@ -5220,79 +5230,79 @@
     total=False,
 )
 
 CreateGlobalTableOutputTypeDef = TypedDict(
     "CreateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeGlobalTableOutputTypeDef = TypedDict(
     "DescribeGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGlobalTableOutputTypeDef = TypedDict(
     "UpdateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateTableOutputTypeDef = TypedDict(
     "CreateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteTableOutputTypeDef = TypedDict(
     "DeleteTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeTableOutputTypeDef = TypedDict(
     "DescribeTableOutputTypeDef",
     {
         "Table": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreTableFromBackupOutputTypeDef = TypedDict(
     "RestoreTableFromBackupOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RestoreTableToPointInTimeOutputTypeDef = TypedDict(
     "RestoreTableToPointInTimeOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTableOutputTypeDef = TypedDict(
     "UpdateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateTableInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTableInputRequestTypeDef",
     {
         "TableName": str,
@@ -5330,24 +5340,24 @@
 )
 
 DescribeGlobalTableSettingsOutputTypeDef = TypedDict(
     "DescribeGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateGlobalTableSettingsOutputTypeDef = TypedDict(
     "UpdateGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTableReplicaAutoScalingInputRequestTypeDef",
     {
         "TableName": str,
@@ -5397,18 +5407,18 @@
 ):
     pass
 
 DescribeTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTableReplicaAutoScalingOutputTypeDef = TypedDict(
     "UpdateTableReplicaAutoScalingOutputTypeDef",
     {
         "TableAutoScalingDescription": TableAutoScalingDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/waiter.py` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb/waiter.pyi` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/PKG-INFO` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.26.97.post1
-Summary: Type annotations for boto3.DynamoDB 1.26.97 service generated with mypy-boto3-builder 7.14.1
+Version: 1.27.0
+Summary: Type annotations for boto3.DynamoDB 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-dynamodb"></a>
 
 # mypy-boto3-dynamodb
 
 [![PyPI - mypy-boto3-dynamodb](https://img.shields.io/pypi/v/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dynamodb?color=blue)](https://pypistats.org/packages/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -481,30 +481,30 @@
 ### Typed dictionaries
 
 `mypy_boto3_dynamodb.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodb.type_defs import (
-    ResponseMetadataTypeDef,
+    ArchivalSummaryResponseMetadataTypeDef,
     ArchivalSummaryTableTypeDef,
     ArchivalSummaryTypeDef,
     AttributeDefinitionServiceResourceTypeDef,
     AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
     AttributeValueTypeDef,
     AttributeValueUpdateTableTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
     BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
     KeysAndAttributesServiceResourceTypeDef,
-    BatchStatementErrorTypeDef,
     ItemCollectionMetricsServiceResourceTypeDef,
+    BillingModeSummaryResponseMetadataTypeDef,
     BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
     CapacityServiceResourceTypeDef,
     CapacityTableTypeDef,
     CapacityTypeDef,
     ConditionTableTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
@@ -547,64 +547,67 @@
     DescribeExportInputRequestTypeDef,
     ExportDescriptionTypeDef,
     DescribeGlobalTableInputRequestTypeDef,
     DescribeGlobalTableSettingsInputRequestTypeDef,
     DescribeImportInputRequestTypeDef,
     DescribeKinesisStreamingDestinationInputRequestTypeDef,
     KinesisDataStreamDestinationTypeDef,
+    DescribeLimitsOutputTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
+    EmptyResponseMetadataTypeDef,
     ExportSummaryTypeDef,
     ExportTableToPointInTimeInputRequestTypeDef,
     GetItemInputTableGetItemTypeDef,
     ProvisionedThroughputDescriptionTableTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
     ProjectionServiceResourceTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
-    PaginatorConfigTypeDef,
+    KinesisStreamingDestinationOutputTypeDef,
+    ListBackupsInputListBackupsPaginateTypeDef,
     ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
+    ListTablesInputListTablesPaginateTypeDef,
     ListTablesInputRequestTypeDef,
+    ListTablesOutputTableTypeDef,
+    ListTablesOutputTypeDef,
+    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
     TagTableTypeDef,
+    PaginatorConfigTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
+    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
     PutRequestServiceResourceTypeDef,
     TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
+    ResponseMetadataTypeDef,
+    RestoreSummaryResponseMetadataTypeDef,
     RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
+    SSEDescriptionResponseMetadataTypeDef,
     SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
     SSESpecificationTableTypeDef,
+    StreamSpecificationResponseMetadataTypeDef,
     StreamSpecificationTableTypeDef,
     TableBatchWriterRequestTypeDef,
+    TableClassSummaryResponseMetadataTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
-    ArchivalSummaryResponseMetadataTypeDef,
-    BillingModeSummaryResponseMetadataTypeDef,
-    DescribeLimitsOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    KinesisStreamingDestinationOutputTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTablesOutputTypeDef,
-    ProvisionedThroughputDescriptionResponseMetadataTypeDef,
-    RestoreSummaryResponseMetadataTypeDef,
-    SSEDescriptionResponseMetadataTypeDef,
-    StreamSpecificationResponseMetadataTypeDef,
-    TableClassSummaryResponseMetadataTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     AttributeValueUpdateTypeDef,
+    BatchStatementErrorTypeDef,
     BatchStatementRequestTypeDef,
     ConditionCheckTypeDef,
     ConditionTypeDef,
     DeleteRequestTypeDef,
     DeleteTypeDef,
     ExecuteStatementInputRequestTypeDef,
     ExpectedAttributeValueTypeDef,
@@ -619,19 +622,20 @@
     UpdateTypeDef,
     AutoScalingPolicyDescriptionTypeDef,
     AutoScalingPolicyUpdateTypeDef,
     CreateBackupOutputTypeDef,
     ListBackupsOutputTableTypeDef,
     ListBackupsOutputTypeDef,
     BatchGetItemInputServiceResourceBatchGetItemTypeDef,
-    BatchStatementResponseTypeDef,
     ConsumedCapacityServiceResourceTypeDef,
     ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
+    QueryInputQueryPaginateTypeDef,
     QueryInputTableQueryTypeDef,
+    ScanInputScanPaginateTypeDef,
     ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
     LocalSecondaryIndexDescriptionTableTypeDef,
     CreateGlobalSecondaryIndexActionTableTypeDef,
     UpdateGlobalSecondaryIndexActionTableTypeDef,
     LocalSecondaryIndexDescriptionTypeDef,
@@ -665,24 +669,20 @@
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
     GlobalSecondaryIndexDescriptionTableTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
     GlobalSecondaryIndexServiceResourceTypeDef,
     LocalSecondaryIndexServiceResourceTypeDef,
     ImportSummaryTypeDef,
-    ListBackupsInputListBackupsPaginateTypeDef,
-    ListTablesInputListTablesPaginateTypeDef,
-    ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    QueryInputQueryPaginateTypeDef,
-    ScanInputScanPaginateTypeDef,
     ListTagsOfResourceOutputTableTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
     WriteRequestServiceResourceTypeDef,
     UpdateTimeToLiveInputRequestTypeDef,
     UpdateTimeToLiveOutputTypeDef,
+    BatchStatementResponseTypeDef,
     BatchExecuteStatementInputRequestTypeDef,
     QueryInputRequestTypeDef,
     ScanInputRequestTypeDef,
     DeleteItemInputRequestTypeDef,
     PutItemInputRequestTypeDef,
     UpdateItemInputRequestTypeDef,
     TransactGetItemTypeDef,
@@ -695,15 +695,14 @@
     BatchGetItemOutputServiceResourceTypeDef,
     DeleteItemOutputTableTypeDef,
     GetItemOutputTableTypeDef,
     PutItemOutputTableTypeDef,
     QueryOutputTableTypeDef,
     ScanOutputTableTypeDef,
     UpdateItemOutputTableTypeDef,
-    BatchExecuteStatementOutputTypeDef,
     BatchGetItemOutputTypeDef,
     DeleteItemOutputTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     GetItemOutputTypeDef,
     PutItemOutputTypeDef,
     QueryOutputTypeDef,
@@ -728,14 +727,15 @@
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
     CreateTableInputServiceResourceCreateTableTypeDef,
     ListImportsOutputTypeDef,
     BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     BatchWriteItemOutputServiceResourceTypeDef,
+    BatchExecuteStatementOutputTypeDef,
     TransactGetItemsInputRequestTypeDef,
     BatchWriteItemInputRequestTypeDef,
     BatchWriteItemOutputTypeDef,
     TransactWriteItemsInputRequestTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
@@ -776,15 +776,15 @@
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_structure() -> ArchivalSummaryResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/mypy_boto3_dynamodb.egg-info/SOURCES.txt` & `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.26.97.post1/setup.py` & `mypy-boto3-dynamodb-1.27.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dynamodb",
-    version="1.26.97.post1",
+    version="1.27.0",
     packages=["mypy_boto3_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DynamoDB 1.26.97 service generated with mypy-boto3-builder"
-        " 7.14.1"
+        "Type annotations for boto3.DynamoDB 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```


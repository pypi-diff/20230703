# Comparing `tmp/mypy-boto3-glue-1.26.8.tar.gz` & `tmp/mypy-boto3-glue-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-glue-1.26.8.tar", last modified: Fri Nov 11 21:07:54 2022, max compression
+gzip compressed data, was "mypy-boto3-glue-1.27.0.tar", last modified: Mon Jul  3 19:50:49 2023, max compression
```

## Comparing `mypy-boto3-glue-1.26.8.tar` & `mypy-boto3-glue-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.082122 mypy-boto3-glue-1.26.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    38830 2022-11-11 21:07:54.074122 mypy-boto3-glue-1.26.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    37407 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.070122 mypy-boto3-glue-1.26.8/mypy_boto3_glue/
--rw-r--r--   0 runner    (1001) docker     (121)     4090 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4089 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)   126110 2022-11-11 21:07:12.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/client.py
--rw-r--r--   0 runner    (1001) docker     (121)   125898 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    19003 2022-11-11 21:07:13.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    19001 2022-11-11 21:07:12.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    21235 2022-11-11 21:07:12.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    21214 2022-11-11 21:07:12.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)   222337 2022-11-11 21:07:17.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)   222006 2022-11-11 21:07:15.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.074122 mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    38830 2022-11-11 21:07:53.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-11-11 21:07:53.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-11 21:07:53.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-11 21:07:53.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 21:07:54.082122 mypy-boto3-glue-1.26.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1930 2022-11-11 21:07:10.000000 mypy-boto3-glue-1.26.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:49.247319 mypy-boto3-glue-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:38:24.000000 mypy-boto3-glue-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42047 2023-07-03 19:50:49.243319 mypy-boto3-glue-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40574 2023-07-03 19:38:24.000000 mypy-boto3-glue-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:49.239319 mypy-boto3-glue-1.27.0/mypy_boto3_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-03 19:38:24.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-03 19:38:24.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-03 19:38:24.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137161 2023-07-03 19:38:25.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136933 2023-07-03 19:38:25.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-07-03 19:38:27.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20766 2023-07-03 19:38:26.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-07-03 19:38:26.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-07-03 19:38:26.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:38:24.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   253738 2023-07-03 19:38:33.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   253363 2023-07-03 19:38:30.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:38:24.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:49.243319 mypy-boto3-glue-1.27.0/mypy_boto3_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42047 2023-07-03 19:50:49.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-03 19:50:49.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:49.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:49.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:49.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 19:50:49.000000 mypy-boto3-glue-1.27.0/mypy_boto3_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:49.247319 mypy-boto3-glue-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-03 19:38:24.000000 mypy-boto3-glue-1.27.0/setup.py
```

### Comparing `mypy-boto3-glue-1.26.8/LICENSE` & `mypy-boto3-glue-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-glue-1.26.8/PKG-INFO` & `mypy-boto3-glue-1.27.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-glue
-Version: 1.26.8
-Summary: Type annotations for boto3.Glue 1.26.8 service generated with mypy-boto3-builder 7.11.10
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 glue type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-glue"></a>
 
 # mypy-boto3-glue
 
 [![PyPI - mypy-boto3-glue](https://img.shields.io/pypi/v/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glue?color=blue)](https://pypistats.org/packages/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
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
 [mypy-boto3-glue docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,14 +314,15 @@
 ### Literals
 
 `mypy_boto3_glue.literals` module contains literals extracted from shapes that
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_glue.literals import (
+    AdditionalOptionKeysType,
     AggFunctionType,
     BackfillErrorCodeType,
     BlueprintRunStateType,
     BlueprintStatusType,
     CatalogEncryptionModeType,
     CloudWatchEncryptionModeType,
     ColumnStatisticsTypeType,
@@ -362,16 +332,20 @@
     ConnectionPropertyKeyType,
     ConnectionTypeType,
     CrawlStateType,
     CrawlerHistoryStateType,
     CrawlerLineageSettingsType,
     CrawlerStateType,
     CsvHeaderOptionType,
+    DQStopJobOnFailureTimingType,
+    DQTransformOutputType,
     DataFormatType,
+    DataQualityRuleResultStatusType,
     DeleteBehaviorType,
+    DeltaTargetCompressionTypeType,
     EnableHybridValuesType,
     ExecutionClassType,
     ExistConditionType,
     FieldNameType,
     FilterLogicalOperatorType,
     FilterOperationType,
     FilterOperatorType,
@@ -389,27 +363,31 @@
     GetResourcePoliciesPaginatorName,
     GetSecurityConfigurationsPaginatorName,
     GetTableVersionsPaginatorName,
     GetTablesPaginatorName,
     GetTriggersPaginatorName,
     GetUserDefinedFunctionsPaginatorName,
     GlueRecordTypeType,
+    HudiTargetCompressionTypeType,
+    JDBCConnectionTypeType,
     JDBCDataTypeType,
+    JdbcMetadataEntryType,
     JobBookmarksEncryptionModeType,
     JobRunStateType,
     JoinTypeType,
     LanguageType,
     LastCrawlStatusType,
     ListRegistriesPaginatorName,
     ListSchemaVersionsPaginatorName,
     ListSchemasPaginatorName,
     LogicalOperatorType,
     LogicalType,
     MLUserDataEncryptionModeStringType,
     NodeTypeType,
+    ParamTypeType,
     ParquetCompressionTypeType,
     PartitionIndexStatusType,
     PermissionType,
     PermissionTypeType,
     PiiTypeType,
     PrincipalTypeType,
     QuoteCharType,
@@ -448,70 +426,77 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: AggFunctionType) -> bool:
+def check_value(value: AdditionalOptionKeysType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_glue.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_glue.type_defs import (
     NotificationPropertyTypeDef,
     AggregateOperationTypeDef,
+    AmazonRedshiftAdvancedOptionTypeDef,
+    OptionTypeDef,
     ApplyMappingTypeDef,
     AuditContextTypeDef,
     PartitionValueListTypeDef,
     BasicCatalogTargetTypeDef,
-    ResponseMetadataTypeDef,
     BatchDeleteConnectionRequestRequestTypeDef,
     ErrorDetailTypeDef,
     BatchDeleteTableRequestRequestTypeDef,
     BatchDeleteTableVersionRequestRequestTypeDef,
     BatchGetBlueprintsRequestRequestTypeDef,
     BatchGetCrawlersRequestRequestTypeDef,
     BatchGetCustomEntityTypesRequestRequestTypeDef,
     CustomEntityTypeTypeDef,
+    BatchGetDataQualityResultRequestRequestTypeDef,
     BatchGetDevEndpointsRequestRequestTypeDef,
     DevEndpointTypeDef,
     BatchGetJobsRequestRequestTypeDef,
     BatchGetTriggersRequestRequestTypeDef,
     BatchGetWorkflowsRequestRequestTypeDef,
     BatchStopJobRunRequestRequestTypeDef,
     BatchStopJobRunSuccessfulSubmissionTypeDef,
     BinaryColumnStatisticsDataTypeDef,
     BlueprintDetailsTypeDef,
     BlueprintRunTypeDef,
     LastActiveDefinitionTypeDef,
     BooleanColumnStatisticsDataTypeDef,
+    CancelDataQualityRuleRecommendationRunRequestRequestTypeDef,
+    CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     CancelMLTaskRunRequestRequestTypeDef,
+    CancelMLTaskRunResponseTypeDef,
     CancelStatementRequestRequestTypeDef,
     CatalogEntryTypeDef,
     CatalogImportStatusTypeDef,
     KafkaStreamingSourceOptionsTypeDef,
     StreamingDataPreviewOptionsTypeDef,
     KinesisStreamingSourceOptionsTypeDef,
     CatalogSchemaChangePolicyTypeDef,
     CatalogSourceTypeDef,
     CatalogTargetTypeDef,
     CheckSchemaVersionValidityInputRequestTypeDef,
+    CheckSchemaVersionValidityResponseTypeDef,
     CsvClassifierTypeDef,
     GrokClassifierTypeDef,
     JsonClassifierTypeDef,
     XMLClassifierTypeDef,
     CloudWatchEncryptionTypeDef,
+    DirectJDBCSourceTypeDef,
     DropDuplicatesTypeDef,
     DropFieldsTypeDef,
     DynamoDBCatalogSourceTypeDef,
     FillMissingValuesTypeDef,
     MergeTypeDef,
     MicrosoftSQLServerCatalogSourceTypeDef,
     MicrosoftSQLServerCatalogTargetTypeDef,
@@ -545,277 +530,311 @@
     ConnectionPasswordEncryptionTypeDef,
     ConnectionsListTypeDef,
     CrawlTypeDef,
     CrawlerHistoryTypeDef,
     CrawlerMetricsTypeDef,
     DeltaTargetTypeDef,
     DynamoDBTargetTypeDef,
+    IcebergTargetTypeDef,
     JdbcTargetTypeDef,
     MongoDBTargetTypeDef,
     S3TargetTypeDef,
     LakeFormationConfigurationTypeDef,
     LastCrawlInfoTypeDef,
     LineageConfigurationTypeDef,
     RecrawlPolicyTypeDef,
     ScheduleTypeDef,
     SchemaChangePolicyTypeDef,
     CrawlsFilterTypeDef,
     CreateBlueprintRequestRequestTypeDef,
+    CreateBlueprintResponseTypeDef,
     CreateCsvClassifierRequestTypeDef,
     CreateGrokClassifierRequestTypeDef,
     CreateJsonClassifierRequestTypeDef,
     CreateXMLClassifierRequestTypeDef,
     CreateCustomEntityTypeRequestRequestTypeDef,
+    CreateCustomEntityTypeResponseTypeDef,
+    DataQualityTargetTableTypeDef,
+    CreateDataQualityRulesetResponseTypeDef,
     CreateDevEndpointRequestRequestTypeDef,
+    CreateDevEndpointResponseTypeDef,
     ExecutionPropertyTypeDef,
     JobCommandTypeDef,
     SourceControlDetailsTypeDef,
+    CreateJobResponseTypeDef,
     GlueTableTypeDef,
+    CreateMLTransformResponseTypeDef,
     PartitionIndexTypeDef,
     CreateRegistryInputRequestTypeDef,
+    CreateRegistryResponseTypeDef,
     RegistryIdTypeDef,
+    CreateSchemaResponseTypeDef,
+    CreateScriptResponseTypeDef,
+    CreateSecurityConfigurationResponseTypeDef,
     SessionCommandTypeDef,
     EventBatchingConditionTypeDef,
+    CreateTriggerResponseTypeDef,
     CreateWorkflowRequestRequestTypeDef,
+    CreateWorkflowResponseTypeDef,
+    DQResultsPublishingOptionsTypeDef,
+    DQStopJobOnFailureOptionsTypeDef,
     EncryptionAtRestTypeDef,
     DataLakePrincipalTypeDef,
+    DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
+    DataQualityRuleResultTypeDef,
     DatabaseIdentifierTypeDef,
+    FederatedDatabaseTypeDef,
     DatatypeTypeDef,
     DecimalNumberTypeDef,
     DeleteBlueprintRequestRequestTypeDef,
+    DeleteBlueprintResponseTypeDef,
     DeleteClassifierRequestRequestTypeDef,
     DeleteColumnStatisticsForPartitionRequestRequestTypeDef,
     DeleteColumnStatisticsForTableRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteCrawlerRequestRequestTypeDef,
     DeleteCustomEntityTypeRequestRequestTypeDef,
+    DeleteCustomEntityTypeResponseTypeDef,
+    DeleteDataQualityRulesetRequestRequestTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteDevEndpointRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
+    DeleteJobResponseTypeDef,
     DeleteMLTransformRequestRequestTypeDef,
+    DeleteMLTransformResponseTypeDef,
     DeletePartitionIndexRequestRequestTypeDef,
     DeletePartitionRequestRequestTypeDef,
+    DeleteRegistryResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     SchemaIdTypeDef,
+    DeleteSchemaResponseTypeDef,
     DeleteSecurityConfigurationRequestRequestTypeDef,
     DeleteSessionRequestRequestTypeDef,
+    DeleteSessionResponseTypeDef,
     DeleteTableRequestRequestTypeDef,
     DeleteTableVersionRequestRequestTypeDef,
     DeleteTriggerRequestRequestTypeDef,
+    DeleteTriggerResponseTypeDef,
     DeleteUserDefinedFunctionRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
+    DeleteWorkflowResponseTypeDef,
     DevEndpointCustomLibrariesTypeDef,
     DirectSchemaChangePolicyTypeDef,
     NullCheckBoxListTypeDef,
+    TransformConfigParameterTypeDef,
     EdgeTypeDef,
     JobBookmarksEncryptionTypeDef,
     S3EncryptionTypeDef,
     ErrorDetailsTypeDef,
     ExportLabelsTaskRunPropertiesTypeDef,
+    FederatedTableTypeDef,
     FilterValueTypeDef,
     FindMatchesParametersTypeDef,
     FindMatchesTaskRunPropertiesTypeDef,
     GetBlueprintRequestRequestTypeDef,
     GetBlueprintRunRequestRequestTypeDef,
     GetBlueprintRunsRequestRequestTypeDef,
     GetCatalogImportStatusRequestRequestTypeDef,
     GetClassifierRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetClassifiersRequestGetClassifiersPaginateTypeDef,
     GetClassifiersRequestRequestTypeDef,
     GetColumnStatisticsForPartitionRequestRequestTypeDef,
     GetColumnStatisticsForTableRequestRequestTypeDef,
     GetConnectionRequestRequestTypeDef,
     GetConnectionsFilterTypeDef,
+    GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef,
     GetCrawlerMetricsRequestRequestTypeDef,
     GetCrawlerRequestRequestTypeDef,
+    GetCrawlersRequestGetCrawlersPaginateTypeDef,
     GetCrawlersRequestRequestTypeDef,
     GetCustomEntityTypeRequestRequestTypeDef,
+    GetCustomEntityTypeResponseTypeDef,
     GetDataCatalogEncryptionSettingsRequestRequestTypeDef,
+    GetDataQualityResultRequestRequestTypeDef,
+    GetDataQualityRuleRecommendationRunRequestRequestTypeDef,
+    GetDataQualityRulesetEvaluationRunRequestRequestTypeDef,
+    GetDataQualityRulesetRequestRequestTypeDef,
     GetDatabaseRequestRequestTypeDef,
+    GetDatabasesRequestGetDatabasesPaginateTypeDef,
     GetDatabasesRequestRequestTypeDef,
     GetDataflowGraphRequestRequestTypeDef,
     GetDevEndpointRequestRequestTypeDef,
+    GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef,
     GetDevEndpointsRequestRequestTypeDef,
     GetJobBookmarkRequestRequestTypeDef,
     JobBookmarkEntryTypeDef,
     GetJobRequestRequestTypeDef,
     GetJobRunRequestRequestTypeDef,
+    GetJobRunsRequestGetJobRunsPaginateTypeDef,
     GetJobRunsRequestRequestTypeDef,
+    GetJobsRequestGetJobsPaginateTypeDef,
     GetJobsRequestRequestTypeDef,
     GetMLTaskRunRequestRequestTypeDef,
     TaskRunFilterCriteriaTypeDef,
     TaskRunSortCriteriaTypeDef,
     GetMLTransformRequestRequestTypeDef,
     SchemaColumnTypeDef,
     TransformSortCriteriaTypeDef,
     MappingEntryTypeDef,
+    GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
     GetPartitionIndexesRequestRequestTypeDef,
     GetPartitionRequestRequestTypeDef,
     SegmentTypeDef,
+    GetPlanResponseTypeDef,
+    GetRegistryResponseTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GluePolicyTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetSchemaByDefinitionResponseTypeDef,
+    GetSchemaResponseTypeDef,
     SchemaVersionNumberTypeDef,
+    GetSchemaVersionResponseTypeDef,
+    GetSchemaVersionsDiffResponseTypeDef,
     GetSecurityConfigurationRequestRequestTypeDef,
+    GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef,
     GetSecurityConfigurationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
     GetStatementRequestRequestTypeDef,
     GetTableRequestRequestTypeDef,
     GetTableVersionRequestRequestTypeDef,
+    GetTableVersionsRequestGetTableVersionsPaginateTypeDef,
     GetTableVersionsRequestRequestTypeDef,
+    GetTablesRequestGetTablesPaginateTypeDef,
     GetTablesRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
+    GetTagsResponseTypeDef,
     GetTriggerRequestRequestTypeDef,
+    GetTriggersRequestGetTriggersPaginateTypeDef,
     GetTriggersRequestRequestTypeDef,
     GetUserDefinedFunctionRequestRequestTypeDef,
+    GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
     GetUserDefinedFunctionsRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowRunPropertiesRequestRequestTypeDef,
+    GetWorkflowRunPropertiesResponseTypeDef,
     GetWorkflowRunRequestRequestTypeDef,
     GetWorkflowRunsRequestRequestTypeDef,
     GlueStudioSchemaColumnTypeDef,
     S3SourceAdditionalOptionsTypeDef,
     ImportCatalogToGlueRequestRequestTypeDef,
     ImportLabelsTaskRunPropertiesTypeDef,
     JDBCConnectorOptionsTypeDef,
     PredecessorTypeDef,
     JoinColumnTypeDef,
     KeySchemaElementTypeDef,
     LabelingSetGenerationTaskRunPropertiesTypeDef,
     ListBlueprintsRequestRequestTypeDef,
+    ListBlueprintsResponseTypeDef,
     ListCrawlersRequestRequestTypeDef,
+    ListCrawlersResponseTypeDef,
     ListCustomEntityTypesRequestRequestTypeDef,
     ListDevEndpointsRequestRequestTypeDef,
+    ListDevEndpointsResponseTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListJobsResponseTypeDef,
+    ListMLTransformsResponseTypeDef,
+    ListRegistriesInputListRegistriesPaginateTypeDef,
     ListRegistriesInputRequestTypeDef,
     RegistryListItemTypeDef,
     SchemaVersionListItemTypeDef,
     SchemaListItemTypeDef,
     ListSessionsRequestRequestTypeDef,
     ListStatementsRequestRequestTypeDef,
     ListTriggersRequestRequestTypeDef,
+    ListTriggersResponseTypeDef,
     ListWorkflowsRequestRequestTypeDef,
+    ListWorkflowsResponseTypeDef,
     MLUserDataEncryptionTypeDef,
     MappingTypeDef,
     OtherMetadataValueListItemTypeDef,
     MetadataKeyValuePairTypeDef,
     OrderTypeDef,
+    PaginatorConfigTypeDef,
     PropertyPredicateTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    PutSchemaVersionMetadataResponseTypeDef,
     PutWorkflowRunPropertiesRequestRequestTypeDef,
     UpsertRedshiftTargetOptionsTypeDef,
+    RegisterSchemaVersionResponseTypeDef,
+    RemoveSchemaVersionMetadataResponseTypeDef,
     ResetJobBookmarkRequestRequestTypeDef,
     ResourceUriTypeDef,
+    ResponseMetadataTypeDef,
     ResumeWorkflowRunRequestRequestTypeDef,
+    ResumeWorkflowRunResponseTypeDef,
     RunStatementRequestRequestTypeDef,
+    RunStatementResponseTypeDef,
     S3DirectSourceAdditionalOptionsTypeDef,
     SortCriterionTypeDef,
     SerDeInfoTypeDef,
     SkewedInfoTypeDef,
     SqlAliasTypeDef,
     StartBlueprintRunRequestRequestTypeDef,
+    StartBlueprintRunResponseTypeDef,
     StartCrawlerRequestRequestTypeDef,
     StartCrawlerScheduleRequestRequestTypeDef,
+    StartDataQualityRuleRecommendationRunResponseTypeDef,
+    StartDataQualityRulesetEvaluationRunResponseTypeDef,
     StartExportLabelsTaskRunRequestRequestTypeDef,
+    StartExportLabelsTaskRunResponseTypeDef,
     StartImportLabelsTaskRunRequestRequestTypeDef,
+    StartImportLabelsTaskRunResponseTypeDef,
+    StartJobRunResponseTypeDef,
     StartMLEvaluationTaskRunRequestRequestTypeDef,
+    StartMLEvaluationTaskRunResponseTypeDef,
     StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef,
+    StartMLLabelingSetGenerationTaskRunResponseTypeDef,
     StartTriggerRequestRequestTypeDef,
+    StartTriggerResponseTypeDef,
     StartWorkflowRunRequestRequestTypeDef,
+    StartWorkflowRunResponseTypeDef,
     StartingEventBatchConditionTypeDef,
     StatementOutputDataTypeDef,
     StopCrawlerRequestRequestTypeDef,
     StopCrawlerScheduleRequestRequestTypeDef,
     StopSessionRequestRequestTypeDef,
+    StopSessionResponseTypeDef,
     StopTriggerRequestRequestTypeDef,
+    StopTriggerResponseTypeDef,
     StopWorkflowRunRequestRequestTypeDef,
     TableIdentifierTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBlueprintRequestRequestTypeDef,
+    UpdateBlueprintResponseTypeDef,
     UpdateCsvClassifierRequestTypeDef,
     UpdateGrokClassifierRequestTypeDef,
     UpdateJsonClassifierRequestTypeDef,
     UpdateXMLClassifierRequestTypeDef,
     UpdateCrawlerScheduleRequestRequestTypeDef,
+    UpdateDataQualityRulesetRequestRequestTypeDef,
+    UpdateDataQualityRulesetResponseTypeDef,
     UpdateJobFromSourceControlRequestRequestTypeDef,
+    UpdateJobFromSourceControlResponseTypeDef,
+    UpdateJobResponseTypeDef,
+    UpdateMLTransformResponseTypeDef,
+    UpdateRegistryResponseTypeDef,
+    UpdateSchemaResponseTypeDef,
     UpdateSourceControlFromJobRequestRequestTypeDef,
+    UpdateSourceControlFromJobResponseTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
+    UpdateWorkflowResponseTypeDef,
     WorkflowRunStatisticsTypeDef,
     ActionTypeDef,
     StartJobRunRequestRequestTypeDef,
     AggregateTypeDef,
+    AmazonRedshiftNodeDataTypeDef,
     GetUnfilteredPartitionMetadataRequestRequestTypeDef,
     GetUnfilteredTableMetadataRequestRequestTypeDef,
     BackfillErrorTypeDef,
     BatchDeletePartitionRequestRequestTypeDef,
     BatchGetPartitionRequestRequestTypeDef,
-    CancelMLTaskRunResponseTypeDef,
-    CheckSchemaVersionValidityResponseTypeDef,
-    CreateBlueprintResponseTypeDef,
-    CreateCustomEntityTypeResponseTypeDef,
-    CreateDevEndpointResponseTypeDef,
-    CreateJobResponseTypeDef,
-    CreateMLTransformResponseTypeDef,
-    CreateRegistryResponseTypeDef,
-    CreateSchemaResponseTypeDef,
-    CreateScriptResponseTypeDef,
-    CreateSecurityConfigurationResponseTypeDef,
-    CreateTriggerResponseTypeDef,
-    CreateWorkflowResponseTypeDef,
-    DeleteBlueprintResponseTypeDef,
-    DeleteCustomEntityTypeResponseTypeDef,
-    DeleteJobResponseTypeDef,
-    DeleteMLTransformResponseTypeDef,
-    DeleteRegistryResponseTypeDef,
-    DeleteSchemaResponseTypeDef,
-    DeleteSessionResponseTypeDef,
-    DeleteTriggerResponseTypeDef,
-    DeleteWorkflowResponseTypeDef,
-    GetCustomEntityTypeResponseTypeDef,
-    GetPlanResponseTypeDef,
-    GetRegistryResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetSchemaByDefinitionResponseTypeDef,
-    GetSchemaResponseTypeDef,
-    GetSchemaVersionResponseTypeDef,
-    GetSchemaVersionsDiffResponseTypeDef,
-    GetTagsResponseTypeDef,
-    GetWorkflowRunPropertiesResponseTypeDef,
-    ListBlueprintsResponseTypeDef,
-    ListCrawlersResponseTypeDef,
-    ListDevEndpointsResponseTypeDef,
-    ListJobsResponseTypeDef,
-    ListMLTransformsResponseTypeDef,
-    ListTriggersResponseTypeDef,
-    ListWorkflowsResponseTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    PutSchemaVersionMetadataResponseTypeDef,
-    RegisterSchemaVersionResponseTypeDef,
-    RemoveSchemaVersionMetadataResponseTypeDef,
-    ResumeWorkflowRunResponseTypeDef,
-    RunStatementResponseTypeDef,
-    StartBlueprintRunResponseTypeDef,
-    StartExportLabelsTaskRunResponseTypeDef,
-    StartImportLabelsTaskRunResponseTypeDef,
-    StartJobRunResponseTypeDef,
-    StartMLEvaluationTaskRunResponseTypeDef,
-    StartMLLabelingSetGenerationTaskRunResponseTypeDef,
-    StartTriggerResponseTypeDef,
-    StartWorkflowRunResponseTypeDef,
-    StopSessionResponseTypeDef,
-    StopTriggerResponseTypeDef,
-    UpdateBlueprintResponseTypeDef,
-    UpdateJobFromSourceControlResponseTypeDef,
-    UpdateJobResponseTypeDef,
-    UpdateMLTransformResponseTypeDef,
-    UpdateRegistryResponseTypeDef,
-    UpdateSchemaResponseTypeDef,
-    UpdateSourceControlFromJobResponseTypeDef,
-    UpdateWorkflowResponseTypeDef,
     BatchDeleteConnectionResponseTypeDef,
     BatchStopJobRunErrorTypeDef,
     BatchUpdatePartitionFailureEntryTypeDef,
     ColumnErrorTypeDef,
     PartitionErrorTypeDef,
     TableErrorTypeDef,
     TableVersionErrorTypeDef,
@@ -830,70 +849,66 @@
     GetCatalogImportStatusResponseTypeDef,
     CatalogKafkaSourceTypeDef,
     DirectKafkaSourceTypeDef,
     CatalogKinesisSourceTypeDef,
     DirectKinesisSourceTypeDef,
     GovernedCatalogTargetTypeDef,
     S3CatalogTargetTypeDef,
+    S3DeltaCatalogTargetTypeDef,
+    S3HudiCatalogTargetTypeDef,
     ClassifierTypeDef,
     CodeGenNodeTypeDef,
     LocationTypeDef,
     PredicateTypeDef,
     FindMatchesMetricsTypeDef,
     ConnectionInputTypeDef,
     ConnectionTypeDef,
     CrawlerNodeDetailsTypeDef,
     ListCrawlsResponseTypeDef,
     GetCrawlerMetricsResponseTypeDef,
     CrawlerTargetsTypeDef,
     ListCrawlsRequestRequestTypeDef,
     CreateClassifierRequestRequestTypeDef,
+    CreateDataQualityRulesetRequestRequestTypeDef,
+    DataQualityRulesetFilterCriteriaTypeDef,
+    DataQualityRulesetListDetailsTypeDef,
+    GetDataQualityRulesetResponseTypeDef,
+    DataSourceTypeDef,
     CreatePartitionIndexRequestRequestTypeDef,
     CreateSchemaInputRequestTypeDef,
     DeleteRegistryInputRequestTypeDef,
     GetRegistryInputRequestTypeDef,
+    ListSchemasInputListSchemasPaginateTypeDef,
     ListSchemasInputRequestTypeDef,
     UpdateRegistryInputRequestTypeDef,
     CreateSessionRequestRequestTypeDef,
     SessionTypeDef,
+    EvaluateDataQualityMultiFrameTypeDef,
+    EvaluateDataQualityTypeDef,
     DataCatalogEncryptionSettingsTypeDef,
     PrincipalPermissionsTypeDef,
     NullValueFieldTypeDef,
     DecimalColumnStatisticsDataTypeDef,
     DeleteSchemaInputRequestTypeDef,
     DeleteSchemaVersionsInputRequestTypeDef,
     GetSchemaByDefinitionInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
+    ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
     ListSchemaVersionsInputRequestTypeDef,
     RegisterSchemaVersionInputRequestTypeDef,
     SchemaReferenceTypeDef,
     UpdateDevEndpointRequestRequestTypeDef,
+    S3DeltaDirectTargetTypeDef,
     S3DirectTargetTypeDef,
     S3GlueParquetTargetTypeDef,
+    S3HudiDirectTargetTypeDef,
     EncryptionConfigurationTypeDef,
     SchemaVersionErrorItemTypeDef,
     FilterExpressionTypeDef,
     TransformParametersTypeDef,
-    GetClassifiersRequestGetClassifiersPaginateTypeDef,
-    GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef,
-    GetCrawlersRequestGetCrawlersPaginateTypeDef,
-    GetDatabasesRequestGetDatabasesPaginateTypeDef,
-    GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef,
-    GetJobRunsRequestGetJobRunsPaginateTypeDef,
-    GetJobsRequestGetJobsPaginateTypeDef,
-    GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef,
-    GetTableVersionsRequestGetTableVersionsPaginateTypeDef,
-    GetTablesRequestGetTablesPaginateTypeDef,
-    GetTriggersRequestGetTriggersPaginateTypeDef,
-    GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
-    ListRegistriesInputListRegistriesPaginateTypeDef,
-    ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
-    ListSchemasInputListSchemasPaginateTypeDef,
     GetConnectionsRequestGetConnectionsPaginateTypeDef,
     GetConnectionsRequestRequestTypeDef,
     GetJobBookmarkResponseTypeDef,
     ResetJobBookmarkResponseTypeDef,
     GetMLTaskRunsRequestRequestTypeDef,
     TransformFilterCriteriaTypeDef,
     GetMappingResponseTypeDef,
@@ -920,14 +935,16 @@
     RemoveSchemaVersionMetadataInputRequestTypeDef,
     RedshiftTargetTypeDef,
     UserDefinedFunctionInputTypeDef,
     UserDefinedFunctionTypeDef,
     SearchTablesRequestRequestTypeDef,
     StatementOutputTypeDef,
     UpdateClassifierRequestRequestTypeDef,
+    AmazonRedshiftSourceTypeDef,
+    AmazonRedshiftTargetTypeDef,
     PartitionIndexDescriptorTypeDef,
     BatchStopJobRunResponseTypeDef,
     BatchUpdatePartitionResponseTypeDef,
     BatchCreatePartitionResponseTypeDef,
     BatchDeletePartitionResponseTypeDef,
     BatchDeleteTableResponseTypeDef,
     BatchDeleteTableVersionResponseTypeDef,
@@ -946,14 +963,28 @@
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     GetConnectionResponseTypeDef,
     GetConnectionsResponseTypeDef,
     CrawlerTypeDef,
     CreateCrawlerRequestRequestTypeDef,
     UpdateCrawlerRequestRequestTypeDef,
+    ListDataQualityRulesetsRequestRequestTypeDef,
+    ListDataQualityRulesetsResponseTypeDef,
+    DataQualityResultDescriptionTypeDef,
+    DataQualityResultFilterCriteriaTypeDef,
+    DataQualityResultTypeDef,
+    DataQualityRuleRecommendationRunDescriptionTypeDef,
+    DataQualityRuleRecommendationRunFilterTypeDef,
+    DataQualityRulesetEvaluationRunDescriptionTypeDef,
+    DataQualityRulesetEvaluationRunFilterTypeDef,
+    GetDataQualityResultResponseTypeDef,
+    GetDataQualityRuleRecommendationRunResponseTypeDef,
+    GetDataQualityRulesetEvaluationRunResponseTypeDef,
+    StartDataQualityRuleRecommendationRunRequestRequestTypeDef,
+    StartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     CreateSessionResponseTypeDef,
     GetSessionResponseTypeDef,
     ListSessionsResponseTypeDef,
     GetDataCatalogEncryptionSettingsResponseTypeDef,
     PutDataCatalogEncryptionSettingsRequestRequestTypeDef,
     DatabaseInputTypeDef,
     DatabaseTypeDef,
@@ -964,18 +995,25 @@
     SecurityConfigurationTypeDef,
     DeleteSchemaVersionsResponseTypeDef,
     FilterTypeDef,
     UpdateMLTransformRequestRequestTypeDef,
     GetMLTransformsRequestRequestTypeDef,
     ListMLTransformsRequestRequestTypeDef,
     AthenaConnectorSourceTypeDef,
+    CatalogDeltaSourceTypeDef,
+    CatalogHudiSourceTypeDef,
     CustomCodeTypeDef,
+    DynamicTransformTypeDef,
     JDBCConnectorSourceTypeDef,
     JDBCConnectorTargetTypeDef,
+    S3CatalogDeltaSourceTypeDef,
+    S3CatalogHudiSourceTypeDef,
     S3CsvSourceTypeDef,
+    S3DeltaSourceTypeDef,
+    S3HudiSourceTypeDef,
     S3JsonSourceTypeDef,
     S3ParquetSourceTypeDef,
     SparkConnectorSourceTypeDef,
     SparkConnectorTargetTypeDef,
     SparkSQLTypeDef,
     GetJobRunResponseTypeDef,
     GetJobRunsResponseTypeDef,
@@ -997,14 +1035,21 @@
     UpdateTriggerResponseTypeDef,
     UpdateTriggerRequestRequestTypeDef,
     GetMLTransformResponseTypeDef,
     MLTransformTypeDef,
     BatchGetCrawlersResponseTypeDef,
     GetCrawlerResponseTypeDef,
     GetCrawlersResponseTypeDef,
+    ListDataQualityResultsResponseTypeDef,
+    ListDataQualityResultsRequestRequestTypeDef,
+    BatchGetDataQualityResultResponseTypeDef,
+    ListDataQualityRuleRecommendationRunsResponseTypeDef,
+    ListDataQualityRuleRecommendationRunsRequestRequestTypeDef,
+    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
+    ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef,
     CreateDatabaseRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
     GetDatabaseResponseTypeDef,
     GetDatabasesResponseTypeDef,
     ColumnStatisticsTypeDef,
     PartitionInputTypeDef,
     PartitionTypeDef,
@@ -1069,42 +1114,42 @@
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

### Comparing `mypy-boto3-glue-1.26.8/README.md` & `mypy-boto3-glue-1.27.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-glue
+Version: 1.27.0
+Summary: Type annotations for boto3.Glue 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 glue type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-glue"></a>
 
 # mypy-boto3-glue
 
 [![PyPI - mypy-boto3-glue](https://img.shields.io/pypi/v/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glue?color=blue)](https://pypistats.org/packages/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
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
 [mypy-boto3-glue docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,14 +346,15 @@
 ### Literals
 
 `mypy_boto3_glue.literals` module contains literals extracted from shapes that
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_glue.literals import (
+    AdditionalOptionKeysType,
     AggFunctionType,
     BackfillErrorCodeType,
     BlueprintRunStateType,
     BlueprintStatusType,
     CatalogEncryptionModeType,
     CloudWatchEncryptionModeType,
     ColumnStatisticsTypeType,
@@ -331,16 +364,20 @@
     ConnectionPropertyKeyType,
     ConnectionTypeType,
     CrawlStateType,
     CrawlerHistoryStateType,
     CrawlerLineageSettingsType,
     CrawlerStateType,
     CsvHeaderOptionType,
+    DQStopJobOnFailureTimingType,
+    DQTransformOutputType,
     DataFormatType,
+    DataQualityRuleResultStatusType,
     DeleteBehaviorType,
+    DeltaTargetCompressionTypeType,
     EnableHybridValuesType,
     ExecutionClassType,
     ExistConditionType,
     FieldNameType,
     FilterLogicalOperatorType,
     FilterOperationType,
     FilterOperatorType,
@@ -358,27 +395,31 @@
     GetResourcePoliciesPaginatorName,
     GetSecurityConfigurationsPaginatorName,
     GetTableVersionsPaginatorName,
     GetTablesPaginatorName,
     GetTriggersPaginatorName,
     GetUserDefinedFunctionsPaginatorName,
     GlueRecordTypeType,
+    HudiTargetCompressionTypeType,
+    JDBCConnectionTypeType,
     JDBCDataTypeType,
+    JdbcMetadataEntryType,
     JobBookmarksEncryptionModeType,
     JobRunStateType,
     JoinTypeType,
     LanguageType,
     LastCrawlStatusType,
     ListRegistriesPaginatorName,
     ListSchemaVersionsPaginatorName,
     ListSchemasPaginatorName,
     LogicalOperatorType,
     LogicalType,
     MLUserDataEncryptionModeStringType,
     NodeTypeType,
+    ParamTypeType,
     ParquetCompressionTypeType,
     PartitionIndexStatusType,
     PermissionType,
     PermissionTypeType,
     PiiTypeType,
     PrincipalTypeType,
     QuoteCharType,
@@ -417,70 +458,77 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: AggFunctionType) -> bool:
+def check_value(value: AdditionalOptionKeysType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_glue.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_glue.type_defs import (
     NotificationPropertyTypeDef,
     AggregateOperationTypeDef,
+    AmazonRedshiftAdvancedOptionTypeDef,
+    OptionTypeDef,
     ApplyMappingTypeDef,
     AuditContextTypeDef,
     PartitionValueListTypeDef,
     BasicCatalogTargetTypeDef,
-    ResponseMetadataTypeDef,
     BatchDeleteConnectionRequestRequestTypeDef,
     ErrorDetailTypeDef,
     BatchDeleteTableRequestRequestTypeDef,
     BatchDeleteTableVersionRequestRequestTypeDef,
     BatchGetBlueprintsRequestRequestTypeDef,
     BatchGetCrawlersRequestRequestTypeDef,
     BatchGetCustomEntityTypesRequestRequestTypeDef,
     CustomEntityTypeTypeDef,
+    BatchGetDataQualityResultRequestRequestTypeDef,
     BatchGetDevEndpointsRequestRequestTypeDef,
     DevEndpointTypeDef,
     BatchGetJobsRequestRequestTypeDef,
     BatchGetTriggersRequestRequestTypeDef,
     BatchGetWorkflowsRequestRequestTypeDef,
     BatchStopJobRunRequestRequestTypeDef,
     BatchStopJobRunSuccessfulSubmissionTypeDef,
     BinaryColumnStatisticsDataTypeDef,
     BlueprintDetailsTypeDef,
     BlueprintRunTypeDef,
     LastActiveDefinitionTypeDef,
     BooleanColumnStatisticsDataTypeDef,
+    CancelDataQualityRuleRecommendationRunRequestRequestTypeDef,
+    CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     CancelMLTaskRunRequestRequestTypeDef,
+    CancelMLTaskRunResponseTypeDef,
     CancelStatementRequestRequestTypeDef,
     CatalogEntryTypeDef,
     CatalogImportStatusTypeDef,
     KafkaStreamingSourceOptionsTypeDef,
     StreamingDataPreviewOptionsTypeDef,
     KinesisStreamingSourceOptionsTypeDef,
     CatalogSchemaChangePolicyTypeDef,
     CatalogSourceTypeDef,
     CatalogTargetTypeDef,
     CheckSchemaVersionValidityInputRequestTypeDef,
+    CheckSchemaVersionValidityResponseTypeDef,
     CsvClassifierTypeDef,
     GrokClassifierTypeDef,
     JsonClassifierTypeDef,
     XMLClassifierTypeDef,
     CloudWatchEncryptionTypeDef,
+    DirectJDBCSourceTypeDef,
     DropDuplicatesTypeDef,
     DropFieldsTypeDef,
     DynamoDBCatalogSourceTypeDef,
     FillMissingValuesTypeDef,
     MergeTypeDef,
     MicrosoftSQLServerCatalogSourceTypeDef,
     MicrosoftSQLServerCatalogTargetTypeDef,
@@ -514,277 +562,311 @@
     ConnectionPasswordEncryptionTypeDef,
     ConnectionsListTypeDef,
     CrawlTypeDef,
     CrawlerHistoryTypeDef,
     CrawlerMetricsTypeDef,
     DeltaTargetTypeDef,
     DynamoDBTargetTypeDef,
+    IcebergTargetTypeDef,
     JdbcTargetTypeDef,
     MongoDBTargetTypeDef,
     S3TargetTypeDef,
     LakeFormationConfigurationTypeDef,
     LastCrawlInfoTypeDef,
     LineageConfigurationTypeDef,
     RecrawlPolicyTypeDef,
     ScheduleTypeDef,
     SchemaChangePolicyTypeDef,
     CrawlsFilterTypeDef,
     CreateBlueprintRequestRequestTypeDef,
+    CreateBlueprintResponseTypeDef,
     CreateCsvClassifierRequestTypeDef,
     CreateGrokClassifierRequestTypeDef,
     CreateJsonClassifierRequestTypeDef,
     CreateXMLClassifierRequestTypeDef,
     CreateCustomEntityTypeRequestRequestTypeDef,
+    CreateCustomEntityTypeResponseTypeDef,
+    DataQualityTargetTableTypeDef,
+    CreateDataQualityRulesetResponseTypeDef,
     CreateDevEndpointRequestRequestTypeDef,
+    CreateDevEndpointResponseTypeDef,
     ExecutionPropertyTypeDef,
     JobCommandTypeDef,
     SourceControlDetailsTypeDef,
+    CreateJobResponseTypeDef,
     GlueTableTypeDef,
+    CreateMLTransformResponseTypeDef,
     PartitionIndexTypeDef,
     CreateRegistryInputRequestTypeDef,
+    CreateRegistryResponseTypeDef,
     RegistryIdTypeDef,
+    CreateSchemaResponseTypeDef,
+    CreateScriptResponseTypeDef,
+    CreateSecurityConfigurationResponseTypeDef,
     SessionCommandTypeDef,
     EventBatchingConditionTypeDef,
+    CreateTriggerResponseTypeDef,
     CreateWorkflowRequestRequestTypeDef,
+    CreateWorkflowResponseTypeDef,
+    DQResultsPublishingOptionsTypeDef,
+    DQStopJobOnFailureOptionsTypeDef,
     EncryptionAtRestTypeDef,
     DataLakePrincipalTypeDef,
+    DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
+    DataQualityRuleResultTypeDef,
     DatabaseIdentifierTypeDef,
+    FederatedDatabaseTypeDef,
     DatatypeTypeDef,
     DecimalNumberTypeDef,
     DeleteBlueprintRequestRequestTypeDef,
+    DeleteBlueprintResponseTypeDef,
     DeleteClassifierRequestRequestTypeDef,
     DeleteColumnStatisticsForPartitionRequestRequestTypeDef,
     DeleteColumnStatisticsForTableRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteCrawlerRequestRequestTypeDef,
     DeleteCustomEntityTypeRequestRequestTypeDef,
+    DeleteCustomEntityTypeResponseTypeDef,
+    DeleteDataQualityRulesetRequestRequestTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteDevEndpointRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
+    DeleteJobResponseTypeDef,
     DeleteMLTransformRequestRequestTypeDef,
+    DeleteMLTransformResponseTypeDef,
     DeletePartitionIndexRequestRequestTypeDef,
     DeletePartitionRequestRequestTypeDef,
+    DeleteRegistryResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     SchemaIdTypeDef,
+    DeleteSchemaResponseTypeDef,
     DeleteSecurityConfigurationRequestRequestTypeDef,
     DeleteSessionRequestRequestTypeDef,
+    DeleteSessionResponseTypeDef,
     DeleteTableRequestRequestTypeDef,
     DeleteTableVersionRequestRequestTypeDef,
     DeleteTriggerRequestRequestTypeDef,
+    DeleteTriggerResponseTypeDef,
     DeleteUserDefinedFunctionRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
+    DeleteWorkflowResponseTypeDef,
     DevEndpointCustomLibrariesTypeDef,
     DirectSchemaChangePolicyTypeDef,
     NullCheckBoxListTypeDef,
+    TransformConfigParameterTypeDef,
     EdgeTypeDef,
     JobBookmarksEncryptionTypeDef,
     S3EncryptionTypeDef,
     ErrorDetailsTypeDef,
     ExportLabelsTaskRunPropertiesTypeDef,
+    FederatedTableTypeDef,
     FilterValueTypeDef,
     FindMatchesParametersTypeDef,
     FindMatchesTaskRunPropertiesTypeDef,
     GetBlueprintRequestRequestTypeDef,
     GetBlueprintRunRequestRequestTypeDef,
     GetBlueprintRunsRequestRequestTypeDef,
     GetCatalogImportStatusRequestRequestTypeDef,
     GetClassifierRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetClassifiersRequestGetClassifiersPaginateTypeDef,
     GetClassifiersRequestRequestTypeDef,
     GetColumnStatisticsForPartitionRequestRequestTypeDef,
     GetColumnStatisticsForTableRequestRequestTypeDef,
     GetConnectionRequestRequestTypeDef,
     GetConnectionsFilterTypeDef,
+    GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef,
     GetCrawlerMetricsRequestRequestTypeDef,
     GetCrawlerRequestRequestTypeDef,
+    GetCrawlersRequestGetCrawlersPaginateTypeDef,
     GetCrawlersRequestRequestTypeDef,
     GetCustomEntityTypeRequestRequestTypeDef,
+    GetCustomEntityTypeResponseTypeDef,
     GetDataCatalogEncryptionSettingsRequestRequestTypeDef,
+    GetDataQualityResultRequestRequestTypeDef,
+    GetDataQualityRuleRecommendationRunRequestRequestTypeDef,
+    GetDataQualityRulesetEvaluationRunRequestRequestTypeDef,
+    GetDataQualityRulesetRequestRequestTypeDef,
     GetDatabaseRequestRequestTypeDef,
+    GetDatabasesRequestGetDatabasesPaginateTypeDef,
     GetDatabasesRequestRequestTypeDef,
     GetDataflowGraphRequestRequestTypeDef,
     GetDevEndpointRequestRequestTypeDef,
+    GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef,
     GetDevEndpointsRequestRequestTypeDef,
     GetJobBookmarkRequestRequestTypeDef,
     JobBookmarkEntryTypeDef,
     GetJobRequestRequestTypeDef,
     GetJobRunRequestRequestTypeDef,
+    GetJobRunsRequestGetJobRunsPaginateTypeDef,
     GetJobRunsRequestRequestTypeDef,
+    GetJobsRequestGetJobsPaginateTypeDef,
     GetJobsRequestRequestTypeDef,
     GetMLTaskRunRequestRequestTypeDef,
     TaskRunFilterCriteriaTypeDef,
     TaskRunSortCriteriaTypeDef,
     GetMLTransformRequestRequestTypeDef,
     SchemaColumnTypeDef,
     TransformSortCriteriaTypeDef,
     MappingEntryTypeDef,
+    GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
     GetPartitionIndexesRequestRequestTypeDef,
     GetPartitionRequestRequestTypeDef,
     SegmentTypeDef,
+    GetPlanResponseTypeDef,
+    GetRegistryResponseTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GluePolicyTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetSchemaByDefinitionResponseTypeDef,
+    GetSchemaResponseTypeDef,
     SchemaVersionNumberTypeDef,
+    GetSchemaVersionResponseTypeDef,
+    GetSchemaVersionsDiffResponseTypeDef,
     GetSecurityConfigurationRequestRequestTypeDef,
+    GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef,
     GetSecurityConfigurationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
     GetStatementRequestRequestTypeDef,
     GetTableRequestRequestTypeDef,
     GetTableVersionRequestRequestTypeDef,
+    GetTableVersionsRequestGetTableVersionsPaginateTypeDef,
     GetTableVersionsRequestRequestTypeDef,
+    GetTablesRequestGetTablesPaginateTypeDef,
     GetTablesRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
+    GetTagsResponseTypeDef,
     GetTriggerRequestRequestTypeDef,
+    GetTriggersRequestGetTriggersPaginateTypeDef,
     GetTriggersRequestRequestTypeDef,
     GetUserDefinedFunctionRequestRequestTypeDef,
+    GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
     GetUserDefinedFunctionsRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowRunPropertiesRequestRequestTypeDef,
+    GetWorkflowRunPropertiesResponseTypeDef,
     GetWorkflowRunRequestRequestTypeDef,
     GetWorkflowRunsRequestRequestTypeDef,
     GlueStudioSchemaColumnTypeDef,
     S3SourceAdditionalOptionsTypeDef,
     ImportCatalogToGlueRequestRequestTypeDef,
     ImportLabelsTaskRunPropertiesTypeDef,
     JDBCConnectorOptionsTypeDef,
     PredecessorTypeDef,
     JoinColumnTypeDef,
     KeySchemaElementTypeDef,
     LabelingSetGenerationTaskRunPropertiesTypeDef,
     ListBlueprintsRequestRequestTypeDef,
+    ListBlueprintsResponseTypeDef,
     ListCrawlersRequestRequestTypeDef,
+    ListCrawlersResponseTypeDef,
     ListCustomEntityTypesRequestRequestTypeDef,
     ListDevEndpointsRequestRequestTypeDef,
+    ListDevEndpointsResponseTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListJobsResponseTypeDef,
+    ListMLTransformsResponseTypeDef,
+    ListRegistriesInputListRegistriesPaginateTypeDef,
     ListRegistriesInputRequestTypeDef,
     RegistryListItemTypeDef,
     SchemaVersionListItemTypeDef,
     SchemaListItemTypeDef,
     ListSessionsRequestRequestTypeDef,
     ListStatementsRequestRequestTypeDef,
     ListTriggersRequestRequestTypeDef,
+    ListTriggersResponseTypeDef,
     ListWorkflowsRequestRequestTypeDef,
+    ListWorkflowsResponseTypeDef,
     MLUserDataEncryptionTypeDef,
     MappingTypeDef,
     OtherMetadataValueListItemTypeDef,
     MetadataKeyValuePairTypeDef,
     OrderTypeDef,
+    PaginatorConfigTypeDef,
     PropertyPredicateTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    PutSchemaVersionMetadataResponseTypeDef,
     PutWorkflowRunPropertiesRequestRequestTypeDef,
     UpsertRedshiftTargetOptionsTypeDef,
+    RegisterSchemaVersionResponseTypeDef,
+    RemoveSchemaVersionMetadataResponseTypeDef,
     ResetJobBookmarkRequestRequestTypeDef,
     ResourceUriTypeDef,
+    ResponseMetadataTypeDef,
     ResumeWorkflowRunRequestRequestTypeDef,
+    ResumeWorkflowRunResponseTypeDef,
     RunStatementRequestRequestTypeDef,
+    RunStatementResponseTypeDef,
     S3DirectSourceAdditionalOptionsTypeDef,
     SortCriterionTypeDef,
     SerDeInfoTypeDef,
     SkewedInfoTypeDef,
     SqlAliasTypeDef,
     StartBlueprintRunRequestRequestTypeDef,
+    StartBlueprintRunResponseTypeDef,
     StartCrawlerRequestRequestTypeDef,
     StartCrawlerScheduleRequestRequestTypeDef,
+    StartDataQualityRuleRecommendationRunResponseTypeDef,
+    StartDataQualityRulesetEvaluationRunResponseTypeDef,
     StartExportLabelsTaskRunRequestRequestTypeDef,
+    StartExportLabelsTaskRunResponseTypeDef,
     StartImportLabelsTaskRunRequestRequestTypeDef,
+    StartImportLabelsTaskRunResponseTypeDef,
+    StartJobRunResponseTypeDef,
     StartMLEvaluationTaskRunRequestRequestTypeDef,
+    StartMLEvaluationTaskRunResponseTypeDef,
     StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef,
+    StartMLLabelingSetGenerationTaskRunResponseTypeDef,
     StartTriggerRequestRequestTypeDef,
+    StartTriggerResponseTypeDef,
     StartWorkflowRunRequestRequestTypeDef,
+    StartWorkflowRunResponseTypeDef,
     StartingEventBatchConditionTypeDef,
     StatementOutputDataTypeDef,
     StopCrawlerRequestRequestTypeDef,
     StopCrawlerScheduleRequestRequestTypeDef,
     StopSessionRequestRequestTypeDef,
+    StopSessionResponseTypeDef,
     StopTriggerRequestRequestTypeDef,
+    StopTriggerResponseTypeDef,
     StopWorkflowRunRequestRequestTypeDef,
     TableIdentifierTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBlueprintRequestRequestTypeDef,
+    UpdateBlueprintResponseTypeDef,
     UpdateCsvClassifierRequestTypeDef,
     UpdateGrokClassifierRequestTypeDef,
     UpdateJsonClassifierRequestTypeDef,
     UpdateXMLClassifierRequestTypeDef,
     UpdateCrawlerScheduleRequestRequestTypeDef,
+    UpdateDataQualityRulesetRequestRequestTypeDef,
+    UpdateDataQualityRulesetResponseTypeDef,
     UpdateJobFromSourceControlRequestRequestTypeDef,
+    UpdateJobFromSourceControlResponseTypeDef,
+    UpdateJobResponseTypeDef,
+    UpdateMLTransformResponseTypeDef,
+    UpdateRegistryResponseTypeDef,
+    UpdateSchemaResponseTypeDef,
     UpdateSourceControlFromJobRequestRequestTypeDef,
+    UpdateSourceControlFromJobResponseTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
+    UpdateWorkflowResponseTypeDef,
     WorkflowRunStatisticsTypeDef,
     ActionTypeDef,
     StartJobRunRequestRequestTypeDef,
     AggregateTypeDef,
+    AmazonRedshiftNodeDataTypeDef,
     GetUnfilteredPartitionMetadataRequestRequestTypeDef,
     GetUnfilteredTableMetadataRequestRequestTypeDef,
     BackfillErrorTypeDef,
     BatchDeletePartitionRequestRequestTypeDef,
     BatchGetPartitionRequestRequestTypeDef,
-    CancelMLTaskRunResponseTypeDef,
-    CheckSchemaVersionValidityResponseTypeDef,
-    CreateBlueprintResponseTypeDef,
-    CreateCustomEntityTypeResponseTypeDef,
-    CreateDevEndpointResponseTypeDef,
-    CreateJobResponseTypeDef,
-    CreateMLTransformResponseTypeDef,
-    CreateRegistryResponseTypeDef,
-    CreateSchemaResponseTypeDef,
-    CreateScriptResponseTypeDef,
-    CreateSecurityConfigurationResponseTypeDef,
-    CreateTriggerResponseTypeDef,
-    CreateWorkflowResponseTypeDef,
-    DeleteBlueprintResponseTypeDef,
-    DeleteCustomEntityTypeResponseTypeDef,
-    DeleteJobResponseTypeDef,
-    DeleteMLTransformResponseTypeDef,
-    DeleteRegistryResponseTypeDef,
-    DeleteSchemaResponseTypeDef,
-    DeleteSessionResponseTypeDef,
-    DeleteTriggerResponseTypeDef,
-    DeleteWorkflowResponseTypeDef,
-    GetCustomEntityTypeResponseTypeDef,
-    GetPlanResponseTypeDef,
-    GetRegistryResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetSchemaByDefinitionResponseTypeDef,
-    GetSchemaResponseTypeDef,
-    GetSchemaVersionResponseTypeDef,
-    GetSchemaVersionsDiffResponseTypeDef,
-    GetTagsResponseTypeDef,
-    GetWorkflowRunPropertiesResponseTypeDef,
-    ListBlueprintsResponseTypeDef,
-    ListCrawlersResponseTypeDef,
-    ListDevEndpointsResponseTypeDef,
-    ListJobsResponseTypeDef,
-    ListMLTransformsResponseTypeDef,
-    ListTriggersResponseTypeDef,
-    ListWorkflowsResponseTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    PutSchemaVersionMetadataResponseTypeDef,
-    RegisterSchemaVersionResponseTypeDef,
-    RemoveSchemaVersionMetadataResponseTypeDef,
-    ResumeWorkflowRunResponseTypeDef,
-    RunStatementResponseTypeDef,
-    StartBlueprintRunResponseTypeDef,
-    StartExportLabelsTaskRunResponseTypeDef,
-    StartImportLabelsTaskRunResponseTypeDef,
-    StartJobRunResponseTypeDef,
-    StartMLEvaluationTaskRunResponseTypeDef,
-    StartMLLabelingSetGenerationTaskRunResponseTypeDef,
-    StartTriggerResponseTypeDef,
-    StartWorkflowRunResponseTypeDef,
-    StopSessionResponseTypeDef,
-    StopTriggerResponseTypeDef,
-    UpdateBlueprintResponseTypeDef,
-    UpdateJobFromSourceControlResponseTypeDef,
-    UpdateJobResponseTypeDef,
-    UpdateMLTransformResponseTypeDef,
-    UpdateRegistryResponseTypeDef,
-    UpdateSchemaResponseTypeDef,
-    UpdateSourceControlFromJobResponseTypeDef,
-    UpdateWorkflowResponseTypeDef,
     BatchDeleteConnectionResponseTypeDef,
     BatchStopJobRunErrorTypeDef,
     BatchUpdatePartitionFailureEntryTypeDef,
     ColumnErrorTypeDef,
     PartitionErrorTypeDef,
     TableErrorTypeDef,
     TableVersionErrorTypeDef,
@@ -799,70 +881,66 @@
     GetCatalogImportStatusResponseTypeDef,
     CatalogKafkaSourceTypeDef,
     DirectKafkaSourceTypeDef,
     CatalogKinesisSourceTypeDef,
     DirectKinesisSourceTypeDef,
     GovernedCatalogTargetTypeDef,
     S3CatalogTargetTypeDef,
+    S3DeltaCatalogTargetTypeDef,
+    S3HudiCatalogTargetTypeDef,
     ClassifierTypeDef,
     CodeGenNodeTypeDef,
     LocationTypeDef,
     PredicateTypeDef,
     FindMatchesMetricsTypeDef,
     ConnectionInputTypeDef,
     ConnectionTypeDef,
     CrawlerNodeDetailsTypeDef,
     ListCrawlsResponseTypeDef,
     GetCrawlerMetricsResponseTypeDef,
     CrawlerTargetsTypeDef,
     ListCrawlsRequestRequestTypeDef,
     CreateClassifierRequestRequestTypeDef,
+    CreateDataQualityRulesetRequestRequestTypeDef,
+    DataQualityRulesetFilterCriteriaTypeDef,
+    DataQualityRulesetListDetailsTypeDef,
+    GetDataQualityRulesetResponseTypeDef,
+    DataSourceTypeDef,
     CreatePartitionIndexRequestRequestTypeDef,
     CreateSchemaInputRequestTypeDef,
     DeleteRegistryInputRequestTypeDef,
     GetRegistryInputRequestTypeDef,
+    ListSchemasInputListSchemasPaginateTypeDef,
     ListSchemasInputRequestTypeDef,
     UpdateRegistryInputRequestTypeDef,
     CreateSessionRequestRequestTypeDef,
     SessionTypeDef,
+    EvaluateDataQualityMultiFrameTypeDef,
+    EvaluateDataQualityTypeDef,
     DataCatalogEncryptionSettingsTypeDef,
     PrincipalPermissionsTypeDef,
     NullValueFieldTypeDef,
     DecimalColumnStatisticsDataTypeDef,
     DeleteSchemaInputRequestTypeDef,
     DeleteSchemaVersionsInputRequestTypeDef,
     GetSchemaByDefinitionInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
+    ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
     ListSchemaVersionsInputRequestTypeDef,
     RegisterSchemaVersionInputRequestTypeDef,
     SchemaReferenceTypeDef,
     UpdateDevEndpointRequestRequestTypeDef,
+    S3DeltaDirectTargetTypeDef,
     S3DirectTargetTypeDef,
     S3GlueParquetTargetTypeDef,
+    S3HudiDirectTargetTypeDef,
     EncryptionConfigurationTypeDef,
     SchemaVersionErrorItemTypeDef,
     FilterExpressionTypeDef,
     TransformParametersTypeDef,
-    GetClassifiersRequestGetClassifiersPaginateTypeDef,
-    GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef,
-    GetCrawlersRequestGetCrawlersPaginateTypeDef,
-    GetDatabasesRequestGetDatabasesPaginateTypeDef,
-    GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef,
-    GetJobRunsRequestGetJobRunsPaginateTypeDef,
-    GetJobsRequestGetJobsPaginateTypeDef,
-    GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef,
-    GetTableVersionsRequestGetTableVersionsPaginateTypeDef,
-    GetTablesRequestGetTablesPaginateTypeDef,
-    GetTriggersRequestGetTriggersPaginateTypeDef,
-    GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
-    ListRegistriesInputListRegistriesPaginateTypeDef,
-    ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
-    ListSchemasInputListSchemasPaginateTypeDef,
     GetConnectionsRequestGetConnectionsPaginateTypeDef,
     GetConnectionsRequestRequestTypeDef,
     GetJobBookmarkResponseTypeDef,
     ResetJobBookmarkResponseTypeDef,
     GetMLTaskRunsRequestRequestTypeDef,
     TransformFilterCriteriaTypeDef,
     GetMappingResponseTypeDef,
@@ -889,14 +967,16 @@
     RemoveSchemaVersionMetadataInputRequestTypeDef,
     RedshiftTargetTypeDef,
     UserDefinedFunctionInputTypeDef,
     UserDefinedFunctionTypeDef,
     SearchTablesRequestRequestTypeDef,
     StatementOutputTypeDef,
     UpdateClassifierRequestRequestTypeDef,
+    AmazonRedshiftSourceTypeDef,
+    AmazonRedshiftTargetTypeDef,
     PartitionIndexDescriptorTypeDef,
     BatchStopJobRunResponseTypeDef,
     BatchUpdatePartitionResponseTypeDef,
     BatchCreatePartitionResponseTypeDef,
     BatchDeletePartitionResponseTypeDef,
     BatchDeleteTableResponseTypeDef,
     BatchDeleteTableVersionResponseTypeDef,
@@ -915,14 +995,28 @@
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     GetConnectionResponseTypeDef,
     GetConnectionsResponseTypeDef,
     CrawlerTypeDef,
     CreateCrawlerRequestRequestTypeDef,
     UpdateCrawlerRequestRequestTypeDef,
+    ListDataQualityRulesetsRequestRequestTypeDef,
+    ListDataQualityRulesetsResponseTypeDef,
+    DataQualityResultDescriptionTypeDef,
+    DataQualityResultFilterCriteriaTypeDef,
+    DataQualityResultTypeDef,
+    DataQualityRuleRecommendationRunDescriptionTypeDef,
+    DataQualityRuleRecommendationRunFilterTypeDef,
+    DataQualityRulesetEvaluationRunDescriptionTypeDef,
+    DataQualityRulesetEvaluationRunFilterTypeDef,
+    GetDataQualityResultResponseTypeDef,
+    GetDataQualityRuleRecommendationRunResponseTypeDef,
+    GetDataQualityRulesetEvaluationRunResponseTypeDef,
+    StartDataQualityRuleRecommendationRunRequestRequestTypeDef,
+    StartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     CreateSessionResponseTypeDef,
     GetSessionResponseTypeDef,
     ListSessionsResponseTypeDef,
     GetDataCatalogEncryptionSettingsResponseTypeDef,
     PutDataCatalogEncryptionSettingsRequestRequestTypeDef,
     DatabaseInputTypeDef,
     DatabaseTypeDef,
@@ -933,18 +1027,25 @@
     SecurityConfigurationTypeDef,
     DeleteSchemaVersionsResponseTypeDef,
     FilterTypeDef,
     UpdateMLTransformRequestRequestTypeDef,
     GetMLTransformsRequestRequestTypeDef,
     ListMLTransformsRequestRequestTypeDef,
     AthenaConnectorSourceTypeDef,
+    CatalogDeltaSourceTypeDef,
+    CatalogHudiSourceTypeDef,
     CustomCodeTypeDef,
+    DynamicTransformTypeDef,
     JDBCConnectorSourceTypeDef,
     JDBCConnectorTargetTypeDef,
+    S3CatalogDeltaSourceTypeDef,
+    S3CatalogHudiSourceTypeDef,
     S3CsvSourceTypeDef,
+    S3DeltaSourceTypeDef,
+    S3HudiSourceTypeDef,
     S3JsonSourceTypeDef,
     S3ParquetSourceTypeDef,
     SparkConnectorSourceTypeDef,
     SparkConnectorTargetTypeDef,
     SparkSQLTypeDef,
     GetJobRunResponseTypeDef,
     GetJobRunsResponseTypeDef,
@@ -966,14 +1067,21 @@
     UpdateTriggerResponseTypeDef,
     UpdateTriggerRequestRequestTypeDef,
     GetMLTransformResponseTypeDef,
     MLTransformTypeDef,
     BatchGetCrawlersResponseTypeDef,
     GetCrawlerResponseTypeDef,
     GetCrawlersResponseTypeDef,
+    ListDataQualityResultsResponseTypeDef,
+    ListDataQualityResultsRequestRequestTypeDef,
+    BatchGetDataQualityResultResponseTypeDef,
+    ListDataQualityRuleRecommendationRunsResponseTypeDef,
+    ListDataQualityRuleRecommendationRunsRequestRequestTypeDef,
+    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
+    ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef,
     CreateDatabaseRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
     GetDatabaseResponseTypeDef,
     GetDatabasesResponseTypeDef,
     ColumnStatisticsTypeDef,
     PartitionInputTypeDef,
     PartitionTypeDef,
@@ -1038,42 +1146,42 @@
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

### Comparing `mypy-boto3-glue-1.26.8/mypy_boto3_glue/__init__.py` & `mypy-boto3-glue-1.27.0/mypy_boto3_glue/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.26.8/mypy_boto3_glue/__init__.pyi` & `mypy-boto3-glue-1.27.0/mypy_boto3_glue/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.26.8/mypy_boto3_glue/__main__.py` & `mypy-boto3-glue-1.27.0/mypy_boto3_glue/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Glue 1.26.8\nVersion:         1.26.8\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.Glue 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue\nOther"
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

### Comparing `mypy-boto3-glue-1.26.8/mypy_boto3_glue/client.py` & `mypy-boto3-glue-1.27.0/mypy_boto3_glue/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     BatchDeleteConnectionResponseTypeDef,
     BatchDeletePartitionResponseTypeDef,
     BatchDeleteTableResponseTypeDef,
     BatchDeleteTableVersionResponseTypeDef,
     BatchGetBlueprintsResponseTypeDef,
     BatchGetCrawlersResponseTypeDef,
     BatchGetCustomEntityTypesResponseTypeDef,
+    BatchGetDataQualityResultResponseTypeDef,
     BatchGetDevEndpointsResponseTypeDef,
     BatchGetJobsResponseTypeDef,
     BatchGetPartitionResponseTypeDef,
     BatchGetTriggersResponseTypeDef,
     BatchGetWorkflowsResponseTypeDef,
     BatchStopJobRunResponseTypeDef,
     BatchUpdatePartitionRequestEntryTypeDef,
@@ -83,14 +84,15 @@
     ConnectionInputTypeDef,
     ConnectionsListTypeDef,
     CrawlerTargetsTypeDef,
     CrawlsFilterTypeDef,
     CreateBlueprintResponseTypeDef,
     CreateCsvClassifierRequestTypeDef,
     CreateCustomEntityTypeResponseTypeDef,
+    CreateDataQualityRulesetResponseTypeDef,
     CreateDevEndpointResponseTypeDef,
     CreateGrokClassifierRequestTypeDef,
     CreateJobResponseTypeDef,
     CreateJsonClassifierRequestTypeDef,
     CreateMLTransformResponseTypeDef,
     CreateRegistryResponseTypeDef,
     CreateSchemaResponseTypeDef,
@@ -98,14 +100,21 @@
     CreateSecurityConfigurationResponseTypeDef,
     CreateSessionResponseTypeDef,
     CreateTriggerResponseTypeDef,
     CreateWorkflowResponseTypeDef,
     CreateXMLClassifierRequestTypeDef,
     DatabaseInputTypeDef,
     DataCatalogEncryptionSettingsTypeDef,
+    DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
+    DataQualityResultFilterCriteriaTypeDef,
+    DataQualityRuleRecommendationRunFilterTypeDef,
+    DataQualityRulesetEvaluationRunFilterTypeDef,
+    DataQualityRulesetFilterCriteriaTypeDef,
+    DataQualityTargetTableTypeDef,
+    DataSourceTypeDef,
     DeleteBlueprintResponseTypeDef,
     DeleteCustomEntityTypeResponseTypeDef,
     DeleteJobResponseTypeDef,
     DeleteMLTransformResponseTypeDef,
     DeleteRegistryResponseTypeDef,
     DeleteSchemaResponseTypeDef,
     DeleteSchemaVersionsResponseTypeDef,
@@ -131,14 +140,18 @@
     GetCrawlerResponseTypeDef,
     GetCrawlersResponseTypeDef,
     GetCustomEntityTypeResponseTypeDef,
     GetDatabaseResponseTypeDef,
     GetDatabasesResponseTypeDef,
     GetDataCatalogEncryptionSettingsResponseTypeDef,
     GetDataflowGraphResponseTypeDef,
+    GetDataQualityResultResponseTypeDef,
+    GetDataQualityRuleRecommendationRunResponseTypeDef,
+    GetDataQualityRulesetEvaluationRunResponseTypeDef,
+    GetDataQualityRulesetResponseTypeDef,
     GetDevEndpointResponseTypeDef,
     GetDevEndpointsResponseTypeDef,
     GetJobBookmarkResponseTypeDef,
     GetJobResponseTypeDef,
     GetJobRunResponseTypeDef,
     GetJobRunsResponseTypeDef,
     GetJobsResponseTypeDef,
@@ -183,14 +196,18 @@
     JobUpdateTypeDef,
     LakeFormationConfigurationTypeDef,
     LineageConfigurationTypeDef,
     ListBlueprintsResponseTypeDef,
     ListCrawlersResponseTypeDef,
     ListCrawlsResponseTypeDef,
     ListCustomEntityTypesResponseTypeDef,
+    ListDataQualityResultsResponseTypeDef,
+    ListDataQualityRuleRecommendationRunsResponseTypeDef,
+    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
+    ListDataQualityRulesetsResponseTypeDef,
     ListDevEndpointsResponseTypeDef,
     ListJobsResponseTypeDef,
     ListMLTransformsResponseTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemasResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSessionsResponseTypeDef,
@@ -221,14 +238,16 @@
     SchemaVersionNumberTypeDef,
     SearchTablesResponseTypeDef,
     SegmentTypeDef,
     SessionCommandTypeDef,
     SortCriterionTypeDef,
     SourceControlDetailsTypeDef,
     StartBlueprintRunResponseTypeDef,
+    StartDataQualityRuleRecommendationRunResponseTypeDef,
+    StartDataQualityRulesetEvaluationRunResponseTypeDef,
     StartExportLabelsTaskRunResponseTypeDef,
     StartImportLabelsTaskRunResponseTypeDef,
     StartJobRunResponseTypeDef,
     StartMLEvaluationTaskRunResponseTypeDef,
     StartMLLabelingSetGenerationTaskRunResponseTypeDef,
     StartTriggerResponseTypeDef,
     StartWorkflowRunResponseTypeDef,
@@ -242,14 +261,15 @@
     TransformParametersTypeDef,
     TransformSortCriteriaTypeDef,
     TriggerUpdateTypeDef,
     UpdateBlueprintResponseTypeDef,
     UpdateColumnStatisticsForPartitionResponseTypeDef,
     UpdateColumnStatisticsForTableResponseTypeDef,
     UpdateCsvClassifierRequestTypeDef,
+    UpdateDataQualityRulesetResponseTypeDef,
     UpdateGrokClassifierRequestTypeDef,
     UpdateJobFromSourceControlResponseTypeDef,
     UpdateJobResponseTypeDef,
     UpdateJsonClassifierRequestTypeDef,
     UpdateMLTransformResponseTypeDef,
     UpdateRegistryResponseTypeDef,
     UpdateSchemaResponseTypeDef,
@@ -285,14 +305,17 @@
     ConcurrentRunsExceededException: Type[BotocoreClientError]
     ConditionCheckFailureException: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     CrawlerNotRunningException: Type[BotocoreClientError]
     CrawlerRunningException: Type[BotocoreClientError]
     CrawlerStoppingException: Type[BotocoreClientError]
     EntityNotFoundException: Type[BotocoreClientError]
+    FederatedResourceAlreadyExistsException: Type[BotocoreClientError]
+    FederationSourceException: Type[BotocoreClientError]
+    FederationSourceRetryableException: Type[BotocoreClientError]
     GlueEncryptionException: Type[BotocoreClientError]
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     IllegalBlueprintStateException: Type[BotocoreClientError]
     IllegalSessionStateException: Type[BotocoreClientError]
     IllegalWorkflowStateException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     InvalidInputException: Type[BotocoreClientError]
@@ -420,14 +443,24 @@
         """
         Retrieves the details for the custom patterns specified by a list of names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_get_custom_entity_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#batch_get_custom_entity_types)
         """
 
+    def batch_get_data_quality_result(
+        self, *, ResultIds: Sequence[str]
+    ) -> BatchGetDataQualityResultResponseTypeDef:
+        """
+        Retrieves a list of data quality results for the specified result IDs.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_get_data_quality_result)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#batch_get_data_quality_result)
+        """
+
     def batch_get_dev_endpoints(
         self, *, DevEndpointNames: Sequence[str]
     ) -> BatchGetDevEndpointsResponseTypeDef:
         """
         Returns a list of resource metadata for a given list of development endpoint
         names.
 
@@ -505,14 +538,30 @@
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#can_paginate)
         """
 
+    def cancel_data_quality_rule_recommendation_run(self, *, RunId: str) -> Dict[str, Any]:
+        """
+        Cancels the specified recommendation run that was being used to generate rules.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.cancel_data_quality_rule_recommendation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#cancel_data_quality_rule_recommendation_run)
+        """
+
+    def cancel_data_quality_ruleset_evaluation_run(self, *, RunId: str) -> Dict[str, Any]:
+        """
+        Cancels a run where a ruleset is being evaluated against a data source.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.cancel_data_quality_ruleset_evaluation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#cancel_data_quality_ruleset_evaluation_run)
+        """
+
     def cancel_ml_task_run(
         self, *, TransformId: str, TaskRunId: str
     ) -> CancelMLTaskRunResponseTypeDef:
         """
         Cancels (stops) a task run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.cancel_ml_task_run)
@@ -615,24 +664,47 @@
         schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_crawler)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#create_crawler)
         """
 
     def create_custom_entity_type(
-        self, *, Name: str, RegexString: str, ContextWords: Sequence[str] = ...
+        self,
+        *,
+        Name: str,
+        RegexString: str,
+        ContextWords: Sequence[str] = ...,
+        Tags: Mapping[str, str] = ...
     ) -> CreateCustomEntityTypeResponseTypeDef:
         """
         Creates a custom pattern that is used to detect sensitive data across the
         columns and rows of your structured data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_custom_entity_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#create_custom_entity_type)
         """
 
+    def create_data_quality_ruleset(
+        self,
+        *,
+        Name: str,
+        Ruleset: str,
+        Description: str = ...,
+        Tags: Mapping[str, str] = ...,
+        TargetTable: DataQualityTargetTableTypeDef = ...,
+        ClientToken: str = ...
+    ) -> CreateDataQualityRulesetResponseTypeDef:
+        """
+        Creates a data quality ruleset with DQDL rules applied to a specified Glue
+        table.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_data_quality_ruleset)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#create_data_quality_ruleset)
+        """
+
     def create_database(
         self,
         *,
         DatabaseInput: DatabaseInputTypeDef,
         CatalogId: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> Dict[str, Any]:
@@ -950,28 +1022,36 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_connection)
         """
 
     def delete_crawler(self, *, Name: str) -> Dict[str, Any]:
         """
         Removes a specified crawler from the Glue Data Catalog, unless the crawler state
-        is `RUNNING` .
+        is `RUNNING`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_crawler)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_crawler)
         """
 
     def delete_custom_entity_type(self, *, Name: str) -> DeleteCustomEntityTypeResponseTypeDef:
         """
         Deletes a custom pattern by specifying its name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_custom_entity_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_custom_entity_type)
         """
 
+    def delete_data_quality_ruleset(self, *, Name: str) -> Dict[str, Any]:
+        """
+        Deletes a data quality ruleset.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_data_quality_ruleset)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_data_quality_ruleset)
+        """
+
     def delete_database(self, *, Name: str, CatalogId: str = ...) -> Dict[str, Any]:
         """
         Removes a specified database from a Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_database)
         """
@@ -1289,14 +1369,50 @@
         """
         Retrieves the security configuration for a specified catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_catalog_encryption_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_catalog_encryption_settings)
         """
 
+    def get_data_quality_result(self, *, ResultId: str) -> GetDataQualityResultResponseTypeDef:
+        """
+        Retrieves the result of a data quality rule evaluation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_result)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_result)
+        """
+
+    def get_data_quality_rule_recommendation_run(
+        self, *, RunId: str
+    ) -> GetDataQualityRuleRecommendationRunResponseTypeDef:
+        """
+        Gets the specified recommendation run that was used to generate rules.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_rule_recommendation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_rule_recommendation_run)
+        """
+
+    def get_data_quality_ruleset(self, *, Name: str) -> GetDataQualityRulesetResponseTypeDef:
+        """
+        Returns an existing ruleset by identifier or name.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_ruleset)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_ruleset)
+        """
+
+    def get_data_quality_ruleset_evaluation_run(
+        self, *, RunId: str
+    ) -> GetDataQualityRulesetEvaluationRunResponseTypeDef:
+        """
+        Retrieves a specific run where a ruleset is evaluated against a data source.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_ruleset_evaluation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_ruleset_evaluation_run)
+        """
+
     def get_database(self, *, Name: str, CatalogId: str = ...) -> GetDatabaseResponseTypeDef:
         """
         Retrieves the definition of a specified database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_database)
         """
@@ -1674,15 +1790,15 @@
         Expression: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         TransactionId: str = ...,
         QueryAsOfTime: Union[datetime, str] = ...
     ) -> GetTablesResponseTypeDef:
         """
-        Retrieves the definitions of some or all of the tables in a given `Database` .
+        Retrieves the definitions of some or all of the tables in a given `Database`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_tables)
         """
 
     def get_tags(self, *, ResourceArn: str) -> GetTagsResponseTypeDef:
         """
@@ -1717,16 +1833,16 @@
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
         SupportedPermissionTypes: Sequence[PermissionTypeType],
         AuditContext: AuditContextTypeDef = ...
     ) -> GetUnfilteredPartitionMetadataResponseTypeDef:
         """
-        See also: [AWS API
-        Documentation](https://docs.aws.amazon.com/goto/WebAPI/glue-2017-03-31/GetUnfilteredPartitionMetadata).
+        Retrieves partition metadata from the Data Catalog that contains unfiltered
+        metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_partition_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_unfiltered_partition_metadata)
         """
 
     def get_unfiltered_partitions_metadata(
         self,
@@ -1738,16 +1854,16 @@
         Expression: str = ...,
         AuditContext: AuditContextTypeDef = ...,
         NextToken: str = ...,
         Segment: SegmentTypeDef = ...,
         MaxResults: int = ...
     ) -> GetUnfilteredPartitionsMetadataResponseTypeDef:
         """
-        See also: [AWS API
-        Documentation](https://docs.aws.amazon.com/goto/WebAPI/glue-2017-03-31/GetUnfilteredPartitionsMetadata).
+        Retrieves partition metadata from the Data Catalog that contains unfiltered
+        metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_partitions_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_unfiltered_partitions_metadata)
         """
 
     def get_unfiltered_table_metadata(
         self,
@@ -1755,16 +1871,16 @@
         CatalogId: str,
         DatabaseName: str,
         Name: str,
         SupportedPermissionTypes: Sequence[PermissionTypeType],
         AuditContext: AuditContextTypeDef = ...
     ) -> GetUnfilteredTableMetadataResponseTypeDef:
         """
-        See also: [AWS API
-        Documentation](https://docs.aws.amazon.com/goto/WebAPI/glue-2017-03-31/GetUnfilteredTableMetadata).
+        Retrieves table metadata from the Data Catalog that contains unfiltered
+        metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_table_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_unfiltered_table_metadata)
         """
 
     def get_user_defined_function(
         self, *, DatabaseName: str, FunctionName: str, CatalogId: str = ...
@@ -1871,23 +1987,81 @@
         Returns all the crawls of a specified crawler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_crawls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_crawls)
         """
 
     def list_custom_entity_types(
-        self, *, NextToken: str = ..., MaxResults: int = ...
+        self, *, NextToken: str = ..., MaxResults: int = ..., Tags: Mapping[str, str] = ...
     ) -> ListCustomEntityTypesResponseTypeDef:
         """
         Lists all the custom patterns that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_custom_entity_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_custom_entity_types)
         """
 
+    def list_data_quality_results(
+        self,
+        *,
+        Filter: DataQualityResultFilterCriteriaTypeDef = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> ListDataQualityResultsResponseTypeDef:
+        """
+        Returns all data quality execution results for your account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_results)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_results)
+        """
+
+    def list_data_quality_rule_recommendation_runs(
+        self,
+        *,
+        Filter: DataQualityRuleRecommendationRunFilterTypeDef = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> ListDataQualityRuleRecommendationRunsResponseTypeDef:
+        """
+        Lists the recommendation runs meeting the filter criteria.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_rule_recommendation_runs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_rule_recommendation_runs)
+        """
+
+    def list_data_quality_ruleset_evaluation_runs(
+        self,
+        *,
+        Filter: DataQualityRulesetEvaluationRunFilterTypeDef = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> ListDataQualityRulesetEvaluationRunsResponseTypeDef:
+        """
+        Lists all the runs meeting the filter criteria, where a ruleset is evaluated
+        against a data source.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_ruleset_evaluation_runs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_ruleset_evaluation_runs)
+        """
+
+    def list_data_quality_rulesets(
+        self,
+        *,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        Filter: DataQualityRulesetFilterCriteriaTypeDef = ...,
+        Tags: Mapping[str, str] = ...
+    ) -> ListDataQualityRulesetsResponseTypeDef:
+        """
+        Returns a paginated list of rulesets for the specified list of Glue tables.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_rulesets)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_rulesets)
+        """
+
     def list_dev_endpoints(
         self, *, NextToken: str = ..., MaxResults: int = ..., Tags: Mapping[str, str] = ...
     ) -> ListDevEndpointsResponseTypeDef:
         """
         Retrieves the names of all `DevEndpoint` resources in this Amazon Web Services
         account, or the resources with the specified tag.
 
@@ -2170,21 +2344,59 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_crawler)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#start_crawler)
         """
 
     def start_crawler_schedule(self, *, CrawlerName: str) -> Dict[str, Any]:
         """
-        Changes the schedule state of the specified crawler to `SCHEDULED` , unless the
-        crawler is already running or the schedule state is already `SCHEDULED` .
+        Changes the schedule state of the specified crawler to `SCHEDULED`, unless the
+        crawler is already running or the schedule state is already `SCHEDULED`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_crawler_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#start_crawler_schedule)
         """
 
+    def start_data_quality_rule_recommendation_run(
+        self,
+        *,
+        DataSource: DataSourceTypeDef,
+        Role: str,
+        NumberOfWorkers: int = ...,
+        Timeout: int = ...,
+        CreatedRulesetName: str = ...,
+        ClientToken: str = ...
+    ) -> StartDataQualityRuleRecommendationRunResponseTypeDef:
+        """
+        Starts a recommendation run that is used to generate rules when you don't know
+        what rules to write.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_rule_recommendation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#start_data_quality_rule_recommendation_run)
+        """
+
+    def start_data_quality_ruleset_evaluation_run(
+        self,
+        *,
+        DataSource: DataSourceTypeDef,
+        Role: str,
+        RulesetNames: Sequence[str],
+        NumberOfWorkers: int = ...,
+        Timeout: int = ...,
+        ClientToken: str = ...,
+        AdditionalRunOptions: DataQualityEvaluationRunAdditionalRunOptionsTypeDef = ...,
+        AdditionalDataSources: Mapping[str, DataSourceTypeDef] = ...
+    ) -> StartDataQualityRulesetEvaluationRunResponseTypeDef:
+        """
+        Once you have a ruleset definition (either recommended or your own), you call
+        this operation to evaluate the ruleset against a data source (Glue table).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_ruleset_evaluation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#start_data_quality_ruleset_evaluation_run)
+        """
+
     def start_export_labels_task_run(
         self, *, TransformId: str, OutputS3Path: str
     ) -> StartExportLabelsTaskRunResponseTypeDef:
         """
         Begins an asynchronous task to export all labeled data for a particular
         transform.
 
@@ -2270,15 +2482,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.stop_crawler)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#stop_crawler)
         """
 
     def stop_crawler_schedule(self, *, CrawlerName: str) -> Dict[str, Any]:
         """
-        Sets the schedule state of the specified crawler to `NOT_SCHEDULED` , but does
+        Sets the schedule state of the specified crawler to `NOT_SCHEDULED`, but does
         not stop the crawler if it is already running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.stop_crawler_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#stop_crawler_schedule)
         """
 
     def stop_session(self, *, Id: str, RequestOrigin: str = ...) -> StopSessionResponseTypeDef:
@@ -2336,16 +2548,16 @@
         *,
         GrokClassifier: UpdateGrokClassifierRequestTypeDef = ...,
         XMLClassifier: UpdateXMLClassifierRequestTypeDef = ...,
         JsonClassifier: UpdateJsonClassifierRequestTypeDef = ...,
         CsvClassifier: UpdateCsvClassifierRequestTypeDef = ...
     ) -> Dict[str, Any]:
         """
-        Modifies an existing classifier (a `GrokClassifier` , an `XMLClassifier` , a
-        `JsonClassifier` , or a `CsvClassifier` , depending on which field is present).
+        Modifies an existing classifier (a `GrokClassifier`, an `XMLClassifier`, a
+        `JsonClassifier`, or a `CsvClassifier`, depending on which field is present).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_classifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#update_classifier)
         """
 
     def update_column_statistics_for_partition(
         self,
@@ -2417,14 +2629,24 @@
         """
         Updates the schedule of a crawler using a `cron` expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_crawler_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#update_crawler_schedule)
         """
 
+    def update_data_quality_ruleset(
+        self, *, Name: str, Description: str = ..., Ruleset: str = ...
+    ) -> UpdateDataQualityRulesetResponseTypeDef:
+        """
+        Updates the specified data quality ruleset.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_data_quality_ruleset)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#update_data_quality_ruleset)
+        """
+
     def update_database(
         self, *, Name: str, DatabaseInput: DatabaseInputTypeDef, CatalogId: str = ...
     ) -> Dict[str, Any]:
         """
         Updates an existing database definition in a Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_database)
```

### Comparing `mypy-boto3-glue-1.26.8/mypy_boto3_glue/client.pyi` & `mypy-boto3-glue-1.27.0/mypy_boto3_glue/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     BatchDeleteConnectionResponseTypeDef,
     BatchDeletePartitionResponseTypeDef,
     BatchDeleteTableResponseTypeDef,
     BatchDeleteTableVersionResponseTypeDef,
     BatchGetBlueprintsResponseTypeDef,
     BatchGetCrawlersResponseTypeDef,
     BatchGetCustomEntityTypesResponseTypeDef,
+    BatchGetDataQualityResultResponseTypeDef,
     BatchGetDevEndpointsResponseTypeDef,
     BatchGetJobsResponseTypeDef,
     BatchGetPartitionResponseTypeDef,
     BatchGetTriggersResponseTypeDef,
     BatchGetWorkflowsResponseTypeDef,
     BatchStopJobRunResponseTypeDef,
     BatchUpdatePartitionRequestEntryTypeDef,
@@ -83,14 +84,15 @@
     ConnectionInputTypeDef,
     ConnectionsListTypeDef,
     CrawlerTargetsTypeDef,
     CrawlsFilterTypeDef,
     CreateBlueprintResponseTypeDef,
     CreateCsvClassifierRequestTypeDef,
     CreateCustomEntityTypeResponseTypeDef,
+    CreateDataQualityRulesetResponseTypeDef,
     CreateDevEndpointResponseTypeDef,
     CreateGrokClassifierRequestTypeDef,
     CreateJobResponseTypeDef,
     CreateJsonClassifierRequestTypeDef,
     CreateMLTransformResponseTypeDef,
     CreateRegistryResponseTypeDef,
     CreateSchemaResponseTypeDef,
@@ -98,14 +100,21 @@
     CreateSecurityConfigurationResponseTypeDef,
     CreateSessionResponseTypeDef,
     CreateTriggerResponseTypeDef,
     CreateWorkflowResponseTypeDef,
     CreateXMLClassifierRequestTypeDef,
     DatabaseInputTypeDef,
     DataCatalogEncryptionSettingsTypeDef,
+    DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
+    DataQualityResultFilterCriteriaTypeDef,
+    DataQualityRuleRecommendationRunFilterTypeDef,
+    DataQualityRulesetEvaluationRunFilterTypeDef,
+    DataQualityRulesetFilterCriteriaTypeDef,
+    DataQualityTargetTableTypeDef,
+    DataSourceTypeDef,
     DeleteBlueprintResponseTypeDef,
     DeleteCustomEntityTypeResponseTypeDef,
     DeleteJobResponseTypeDef,
     DeleteMLTransformResponseTypeDef,
     DeleteRegistryResponseTypeDef,
     DeleteSchemaResponseTypeDef,
     DeleteSchemaVersionsResponseTypeDef,
@@ -131,14 +140,18 @@
     GetCrawlerResponseTypeDef,
     GetCrawlersResponseTypeDef,
     GetCustomEntityTypeResponseTypeDef,
     GetDatabaseResponseTypeDef,
     GetDatabasesResponseTypeDef,
     GetDataCatalogEncryptionSettingsResponseTypeDef,
     GetDataflowGraphResponseTypeDef,
+    GetDataQualityResultResponseTypeDef,
+    GetDataQualityRuleRecommendationRunResponseTypeDef,
+    GetDataQualityRulesetEvaluationRunResponseTypeDef,
+    GetDataQualityRulesetResponseTypeDef,
     GetDevEndpointResponseTypeDef,
     GetDevEndpointsResponseTypeDef,
     GetJobBookmarkResponseTypeDef,
     GetJobResponseTypeDef,
     GetJobRunResponseTypeDef,
     GetJobRunsResponseTypeDef,
     GetJobsResponseTypeDef,
@@ -183,14 +196,18 @@
     JobUpdateTypeDef,
     LakeFormationConfigurationTypeDef,
     LineageConfigurationTypeDef,
     ListBlueprintsResponseTypeDef,
     ListCrawlersResponseTypeDef,
     ListCrawlsResponseTypeDef,
     ListCustomEntityTypesResponseTypeDef,
+    ListDataQualityResultsResponseTypeDef,
+    ListDataQualityRuleRecommendationRunsResponseTypeDef,
+    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
+    ListDataQualityRulesetsResponseTypeDef,
     ListDevEndpointsResponseTypeDef,
     ListJobsResponseTypeDef,
     ListMLTransformsResponseTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemasResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSessionsResponseTypeDef,
@@ -221,14 +238,16 @@
     SchemaVersionNumberTypeDef,
     SearchTablesResponseTypeDef,
     SegmentTypeDef,
     SessionCommandTypeDef,
     SortCriterionTypeDef,
     SourceControlDetailsTypeDef,
     StartBlueprintRunResponseTypeDef,
+    StartDataQualityRuleRecommendationRunResponseTypeDef,
+    StartDataQualityRulesetEvaluationRunResponseTypeDef,
     StartExportLabelsTaskRunResponseTypeDef,
     StartImportLabelsTaskRunResponseTypeDef,
     StartJobRunResponseTypeDef,
     StartMLEvaluationTaskRunResponseTypeDef,
     StartMLLabelingSetGenerationTaskRunResponseTypeDef,
     StartTriggerResponseTypeDef,
     StartWorkflowRunResponseTypeDef,
@@ -242,14 +261,15 @@
     TransformParametersTypeDef,
     TransformSortCriteriaTypeDef,
     TriggerUpdateTypeDef,
     UpdateBlueprintResponseTypeDef,
     UpdateColumnStatisticsForPartitionResponseTypeDef,
     UpdateColumnStatisticsForTableResponseTypeDef,
     UpdateCsvClassifierRequestTypeDef,
+    UpdateDataQualityRulesetResponseTypeDef,
     UpdateGrokClassifierRequestTypeDef,
     UpdateJobFromSourceControlResponseTypeDef,
     UpdateJobResponseTypeDef,
     UpdateJsonClassifierRequestTypeDef,
     UpdateMLTransformResponseTypeDef,
     UpdateRegistryResponseTypeDef,
     UpdateSchemaResponseTypeDef,
@@ -282,14 +302,17 @@
     ConcurrentRunsExceededException: Type[BotocoreClientError]
     ConditionCheckFailureException: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     CrawlerNotRunningException: Type[BotocoreClientError]
     CrawlerRunningException: Type[BotocoreClientError]
     CrawlerStoppingException: Type[BotocoreClientError]
     EntityNotFoundException: Type[BotocoreClientError]
+    FederatedResourceAlreadyExistsException: Type[BotocoreClientError]
+    FederationSourceException: Type[BotocoreClientError]
+    FederationSourceRetryableException: Type[BotocoreClientError]
     GlueEncryptionException: Type[BotocoreClientError]
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     IllegalBlueprintStateException: Type[BotocoreClientError]
     IllegalSessionStateException: Type[BotocoreClientError]
     IllegalWorkflowStateException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     InvalidInputException: Type[BotocoreClientError]
@@ -407,14 +430,23 @@
     ) -> BatchGetCustomEntityTypesResponseTypeDef:
         """
         Retrieves the details for the custom patterns specified by a list of names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_get_custom_entity_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#batch_get_custom_entity_types)
         """
+    def batch_get_data_quality_result(
+        self, *, ResultIds: Sequence[str]
+    ) -> BatchGetDataQualityResultResponseTypeDef:
+        """
+        Retrieves a list of data quality results for the specified result IDs.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_get_data_quality_result)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#batch_get_data_quality_result)
+        """
     def batch_get_dev_endpoints(
         self, *, DevEndpointNames: Sequence[str]
     ) -> BatchGetDevEndpointsResponseTypeDef:
         """
         Returns a list of resource metadata for a given list of development endpoint
         names.
 
@@ -484,14 +516,28 @@
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#can_paginate)
         """
+    def cancel_data_quality_rule_recommendation_run(self, *, RunId: str) -> Dict[str, Any]:
+        """
+        Cancels the specified recommendation run that was being used to generate rules.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.cancel_data_quality_rule_recommendation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#cancel_data_quality_rule_recommendation_run)
+        """
+    def cancel_data_quality_ruleset_evaluation_run(self, *, RunId: str) -> Dict[str, Any]:
+        """
+        Cancels a run where a ruleset is being evaluated against a data source.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.cancel_data_quality_ruleset_evaluation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#cancel_data_quality_ruleset_evaluation_run)
+        """
     def cancel_ml_task_run(
         self, *, TransformId: str, TaskRunId: str
     ) -> CancelMLTaskRunResponseTypeDef:
         """
         Cancels (stops) a task run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.cancel_ml_task_run)
@@ -586,23 +632,45 @@
         Creates a new crawler with specified targets, role, configuration, and optional
         schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_crawler)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#create_crawler)
         """
     def create_custom_entity_type(
-        self, *, Name: str, RegexString: str, ContextWords: Sequence[str] = ...
+        self,
+        *,
+        Name: str,
+        RegexString: str,
+        ContextWords: Sequence[str] = ...,
+        Tags: Mapping[str, str] = ...
     ) -> CreateCustomEntityTypeResponseTypeDef:
         """
         Creates a custom pattern that is used to detect sensitive data across the
         columns and rows of your structured data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_custom_entity_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#create_custom_entity_type)
         """
+    def create_data_quality_ruleset(
+        self,
+        *,
+        Name: str,
+        Ruleset: str,
+        Description: str = ...,
+        Tags: Mapping[str, str] = ...,
+        TargetTable: DataQualityTargetTableTypeDef = ...,
+        ClientToken: str = ...
+    ) -> CreateDataQualityRulesetResponseTypeDef:
+        """
+        Creates a data quality ruleset with DQDL rules applied to a specified Glue
+        table.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_data_quality_ruleset)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#create_data_quality_ruleset)
+        """
     def create_database(
         self,
         *,
         DatabaseInput: DatabaseInputTypeDef,
         CatalogId: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> Dict[str, Any]:
@@ -900,26 +968,33 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_connection)
         """
     def delete_crawler(self, *, Name: str) -> Dict[str, Any]:
         """
         Removes a specified crawler from the Glue Data Catalog, unless the crawler state
-        is `RUNNING` .
+        is `RUNNING`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_crawler)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_crawler)
         """
     def delete_custom_entity_type(self, *, Name: str) -> DeleteCustomEntityTypeResponseTypeDef:
         """
         Deletes a custom pattern by specifying its name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_custom_entity_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_custom_entity_type)
         """
+    def delete_data_quality_ruleset(self, *, Name: str) -> Dict[str, Any]:
+        """
+        Deletes a data quality ruleset.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_data_quality_ruleset)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_data_quality_ruleset)
+        """
     def delete_database(self, *, Name: str, CatalogId: str = ...) -> Dict[str, Any]:
         """
         Removes a specified database from a Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_database)
         """
@@ -1204,14 +1279,46 @@
     ) -> GetDataCatalogEncryptionSettingsResponseTypeDef:
         """
         Retrieves the security configuration for a specified catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_catalog_encryption_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_catalog_encryption_settings)
         """
+    def get_data_quality_result(self, *, ResultId: str) -> GetDataQualityResultResponseTypeDef:
+        """
+        Retrieves the result of a data quality rule evaluation.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_result)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_result)
+        """
+    def get_data_quality_rule_recommendation_run(
+        self, *, RunId: str
+    ) -> GetDataQualityRuleRecommendationRunResponseTypeDef:
+        """
+        Gets the specified recommendation run that was used to generate rules.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_rule_recommendation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_rule_recommendation_run)
+        """
+    def get_data_quality_ruleset(self, *, Name: str) -> GetDataQualityRulesetResponseTypeDef:
+        """
+        Returns an existing ruleset by identifier or name.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_ruleset)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_ruleset)
+        """
+    def get_data_quality_ruleset_evaluation_run(
+        self, *, RunId: str
+    ) -> GetDataQualityRulesetEvaluationRunResponseTypeDef:
+        """
+        Retrieves a specific run where a ruleset is evaluated against a data source.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_ruleset_evaluation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_ruleset_evaluation_run)
+        """
     def get_database(self, *, Name: str, CatalogId: str = ...) -> GetDatabaseResponseTypeDef:
         """
         Retrieves the definition of a specified database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_database)
         """
@@ -1556,15 +1663,15 @@
         Expression: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         TransactionId: str = ...,
         QueryAsOfTime: Union[datetime, str] = ...
     ) -> GetTablesResponseTypeDef:
         """
-        Retrieves the definitions of some or all of the tables in a given `Database` .
+        Retrieves the definitions of some or all of the tables in a given `Database`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_tables)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_tables)
         """
     def get_tags(self, *, ResourceArn: str) -> GetTagsResponseTypeDef:
         """
         Retrieves a list of tags associated with a resource.
@@ -1595,16 +1702,16 @@
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
         SupportedPermissionTypes: Sequence[PermissionTypeType],
         AuditContext: AuditContextTypeDef = ...
     ) -> GetUnfilteredPartitionMetadataResponseTypeDef:
         """
-        See also: [AWS API
-        Documentation](https://docs.aws.amazon.com/goto/WebAPI/glue-2017-03-31/GetUnfilteredPartitionMetadata).
+        Retrieves partition metadata from the Data Catalog that contains unfiltered
+        metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_partition_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_unfiltered_partition_metadata)
         """
     def get_unfiltered_partitions_metadata(
         self,
         *,
@@ -1615,32 +1722,32 @@
         Expression: str = ...,
         AuditContext: AuditContextTypeDef = ...,
         NextToken: str = ...,
         Segment: SegmentTypeDef = ...,
         MaxResults: int = ...
     ) -> GetUnfilteredPartitionsMetadataResponseTypeDef:
         """
-        See also: [AWS API
-        Documentation](https://docs.aws.amazon.com/goto/WebAPI/glue-2017-03-31/GetUnfilteredPartitionsMetadata).
+        Retrieves partition metadata from the Data Catalog that contains unfiltered
+        metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_partitions_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_unfiltered_partitions_metadata)
         """
     def get_unfiltered_table_metadata(
         self,
         *,
         CatalogId: str,
         DatabaseName: str,
         Name: str,
         SupportedPermissionTypes: Sequence[PermissionTypeType],
         AuditContext: AuditContextTypeDef = ...
     ) -> GetUnfilteredTableMetadataResponseTypeDef:
         """
-        See also: [AWS API
-        Documentation](https://docs.aws.amazon.com/goto/WebAPI/glue-2017-03-31/GetUnfilteredTableMetadata).
+        Retrieves table metadata from the Data Catalog that contains unfiltered
+        metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_table_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_unfiltered_table_metadata)
         """
     def get_user_defined_function(
         self, *, DatabaseName: str, FunctionName: str, CatalogId: str = ...
     ) -> GetUserDefinedFunctionResponseTypeDef:
@@ -1736,22 +1843,76 @@
         """
         Returns all the crawls of a specified crawler.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_crawls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_crawls)
         """
     def list_custom_entity_types(
-        self, *, NextToken: str = ..., MaxResults: int = ...
+        self, *, NextToken: str = ..., MaxResults: int = ..., Tags: Mapping[str, str] = ...
     ) -> ListCustomEntityTypesResponseTypeDef:
         """
         Lists all the custom patterns that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_custom_entity_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_custom_entity_types)
         """
+    def list_data_quality_results(
+        self,
+        *,
+        Filter: DataQualityResultFilterCriteriaTypeDef = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> ListDataQualityResultsResponseTypeDef:
+        """
+        Returns all data quality execution results for your account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_results)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_results)
+        """
+    def list_data_quality_rule_recommendation_runs(
+        self,
+        *,
+        Filter: DataQualityRuleRecommendationRunFilterTypeDef = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> ListDataQualityRuleRecommendationRunsResponseTypeDef:
+        """
+        Lists the recommendation runs meeting the filter criteria.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_rule_recommendation_runs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_rule_recommendation_runs)
+        """
+    def list_data_quality_ruleset_evaluation_runs(
+        self,
+        *,
+        Filter: DataQualityRulesetEvaluationRunFilterTypeDef = ...,
+        NextToken: str = ...,
+        MaxResults: int = ...
+    ) -> ListDataQualityRulesetEvaluationRunsResponseTypeDef:
+        """
+        Lists all the runs meeting the filter criteria, where a ruleset is evaluated
+        against a data source.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_ruleset_evaluation_runs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_ruleset_evaluation_runs)
+        """
+    def list_data_quality_rulesets(
+        self,
+        *,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        Filter: DataQualityRulesetFilterCriteriaTypeDef = ...,
+        Tags: Mapping[str, str] = ...
+    ) -> ListDataQualityRulesetsResponseTypeDef:
+        """
+        Returns a paginated list of rulesets for the specified list of Glue tables.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_rulesets)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_rulesets)
+        """
     def list_dev_endpoints(
         self, *, NextToken: str = ..., MaxResults: int = ..., Tags: Mapping[str, str] = ...
     ) -> ListDevEndpointsResponseTypeDef:
         """
         Retrieves the names of all `DevEndpoint` resources in this Amazon Web Services
         account, or the resources with the specified tag.
 
@@ -2011,20 +2172,56 @@
         Starts a crawl using the specified crawler, regardless of what is scheduled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_crawler)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#start_crawler)
         """
     def start_crawler_schedule(self, *, CrawlerName: str) -> Dict[str, Any]:
         """
-        Changes the schedule state of the specified crawler to `SCHEDULED` , unless the
-        crawler is already running or the schedule state is already `SCHEDULED` .
+        Changes the schedule state of the specified crawler to `SCHEDULED`, unless the
+        crawler is already running or the schedule state is already `SCHEDULED`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_crawler_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#start_crawler_schedule)
         """
+    def start_data_quality_rule_recommendation_run(
+        self,
+        *,
+        DataSource: DataSourceTypeDef,
+        Role: str,
+        NumberOfWorkers: int = ...,
+        Timeout: int = ...,
+        CreatedRulesetName: str = ...,
+        ClientToken: str = ...
+    ) -> StartDataQualityRuleRecommendationRunResponseTypeDef:
+        """
+        Starts a recommendation run that is used to generate rules when you don't know
+        what rules to write.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_rule_recommendation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#start_data_quality_rule_recommendation_run)
+        """
+    def start_data_quality_ruleset_evaluation_run(
+        self,
+        *,
+        DataSource: DataSourceTypeDef,
+        Role: str,
+        RulesetNames: Sequence[str],
+        NumberOfWorkers: int = ...,
+        Timeout: int = ...,
+        ClientToken: str = ...,
+        AdditionalRunOptions: DataQualityEvaluationRunAdditionalRunOptionsTypeDef = ...,
+        AdditionalDataSources: Mapping[str, DataSourceTypeDef] = ...
+    ) -> StartDataQualityRulesetEvaluationRunResponseTypeDef:
+        """
+        Once you have a ruleset definition (either recommended or your own), you call
+        this operation to evaluate the ruleset against a data source (Glue table).
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_ruleset_evaluation_run)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#start_data_quality_ruleset_evaluation_run)
+        """
     def start_export_labels_task_run(
         self, *, TransformId: str, OutputS3Path: str
     ) -> StartExportLabelsTaskRunResponseTypeDef:
         """
         Begins an asynchronous task to export all labeled data for a particular
         transform.
 
@@ -2102,15 +2299,15 @@
         If the specified crawler is running, stops the crawl.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.stop_crawler)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#stop_crawler)
         """
     def stop_crawler_schedule(self, *, CrawlerName: str) -> Dict[str, Any]:
         """
-        Sets the schedule state of the specified crawler to `NOT_SCHEDULED` , but does
+        Sets the schedule state of the specified crawler to `NOT_SCHEDULED`, but does
         not stop the crawler if it is already running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.stop_crawler_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#stop_crawler_schedule)
         """
     def stop_session(self, *, Id: str, RequestOrigin: str = ...) -> StopSessionResponseTypeDef:
         """
@@ -2161,16 +2358,16 @@
         *,
         GrokClassifier: UpdateGrokClassifierRequestTypeDef = ...,
         XMLClassifier: UpdateXMLClassifierRequestTypeDef = ...,
         JsonClassifier: UpdateJsonClassifierRequestTypeDef = ...,
         CsvClassifier: UpdateCsvClassifierRequestTypeDef = ...
     ) -> Dict[str, Any]:
         """
-        Modifies an existing classifier (a `GrokClassifier` , an `XMLClassifier` , a
-        `JsonClassifier` , or a `CsvClassifier` , depending on which field is present).
+        Modifies an existing classifier (a `GrokClassifier`, an `XMLClassifier`, a
+        `JsonClassifier`, or a `CsvClassifier`, depending on which field is present).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_classifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#update_classifier)
         """
     def update_column_statistics_for_partition(
         self,
         *,
@@ -2236,14 +2433,23 @@
     def update_crawler_schedule(self, *, CrawlerName: str, Schedule: str = ...) -> Dict[str, Any]:
         """
         Updates the schedule of a crawler using a `cron` expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_crawler_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#update_crawler_schedule)
         """
+    def update_data_quality_ruleset(
+        self, *, Name: str, Description: str = ..., Ruleset: str = ...
+    ) -> UpdateDataQualityRulesetResponseTypeDef:
+        """
+        Updates the specified data quality ruleset.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_data_quality_ruleset)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#update_data_quality_ruleset)
+        """
     def update_database(
         self, *, Name: str, DatabaseInput: DatabaseInputTypeDef, CatalogId: str = ...
     ) -> Dict[str, Any]:
         """
         Updates an existing database definition in a Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_database)
```

### Comparing `mypy-boto3-glue-1.26.8/mypy_boto3_glue/literals.py` & `mypy-boto3-glue-1.27.0/mypy_boto3_glue/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 Type annotations for glue service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_glue.literals import AggFunctionType
+    from mypy_boto3_glue.literals import AdditionalOptionKeysType
 
-    data: AggFunctionType = "avg"
+    data: AdditionalOptionKeysType = "performanceTuning.caching"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
+    "AdditionalOptionKeysType",
     "AggFunctionType",
     "BackfillErrorCodeType",
     "BlueprintRunStateType",
     "BlueprintStatusType",
     "CatalogEncryptionModeType",
     "CloudWatchEncryptionModeType",
     "ColumnStatisticsTypeType",
@@ -33,16 +33,20 @@
     "ConnectionPropertyKeyType",
     "ConnectionTypeType",
     "CrawlStateType",
     "CrawlerHistoryStateType",
     "CrawlerLineageSettingsType",
     "CrawlerStateType",
     "CsvHeaderOptionType",
+    "DQStopJobOnFailureTimingType",
+    "DQTransformOutputType",
     "DataFormatType",
+    "DataQualityRuleResultStatusType",
     "DeleteBehaviorType",
+    "DeltaTargetCompressionTypeType",
     "EnableHybridValuesType",
     "ExecutionClassType",
     "ExistConditionType",
     "FieldNameType",
     "FilterLogicalOperatorType",
     "FilterOperationType",
     "FilterOperatorType",
@@ -60,27 +64,31 @@
     "GetResourcePoliciesPaginatorName",
     "GetSecurityConfigurationsPaginatorName",
     "GetTableVersionsPaginatorName",
     "GetTablesPaginatorName",
     "GetTriggersPaginatorName",
     "GetUserDefinedFunctionsPaginatorName",
     "GlueRecordTypeType",
+    "HudiTargetCompressionTypeType",
+    "JDBCConnectionTypeType",
     "JDBCDataTypeType",
+    "JdbcMetadataEntryType",
     "JobBookmarksEncryptionModeType",
     "JobRunStateType",
     "JoinTypeType",
     "LanguageType",
     "LastCrawlStatusType",
     "ListRegistriesPaginatorName",
     "ListSchemaVersionsPaginatorName",
     "ListSchemasPaginatorName",
     "LogicalOperatorType",
     "LogicalType",
     "MLUserDataEncryptionModeStringType",
     "NodeTypeType",
+    "ParamTypeType",
     "ParquetCompressionTypeType",
     "PartitionIndexStatusType",
     "PermissionType",
     "PermissionTypeType",
     "PiiTypeType",
     "PrincipalTypeType",
     "QuoteCharType",
@@ -118,15 +126,15 @@
     "GlueServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
+AdditionalOptionKeysType = Literal["performanceTuning.caching"]
 AggFunctionType = Literal[
     "avg",
     "count",
     "countDistinct",
     "first",
     "kurtosis",
     "last",
@@ -195,16 +203,20 @@
 ]
 ConnectionTypeType = Literal["CUSTOM", "JDBC", "KAFKA", "MARKETPLACE", "MONGODB", "NETWORK", "SFTP"]
 CrawlStateType = Literal["CANCELLED", "CANCELLING", "ERROR", "FAILED", "RUNNING", "SUCCEEDED"]
 CrawlerHistoryStateType = Literal["COMPLETED", "FAILED", "RUNNING", "STOPPED"]
 CrawlerLineageSettingsType = Literal["DISABLE", "ENABLE"]
 CrawlerStateType = Literal["READY", "RUNNING", "STOPPING"]
 CsvHeaderOptionType = Literal["ABSENT", "PRESENT", "UNKNOWN"]
+DQStopJobOnFailureTimingType = Literal["AfterDataLoad", "Immediate"]
+DQTransformOutputType = Literal["EvaluationResults", "PrimaryInput"]
 DataFormatType = Literal["AVRO", "JSON", "PROTOBUF"]
+DataQualityRuleResultStatusType = Literal["ERROR", "FAIL", "PASS"]
 DeleteBehaviorType = Literal["DELETE_FROM_DATABASE", "DEPRECATE_IN_DATABASE", "LOG"]
+DeltaTargetCompressionTypeType = Literal["snappy", "uncompressed"]
 EnableHybridValuesType = Literal["FALSE", "TRUE"]
 ExecutionClassType = Literal["FLEX", "STANDARD"]
 ExistConditionType = Literal["MUST_EXIST", "NONE", "NOT_EXIST"]
 FieldNameType = Literal["CRAWL_ID", "DPU_HOUR", "END_TIME", "START_TIME", "STATE"]
 FilterLogicalOperatorType = Literal["AND", "OR"]
 FilterOperationType = Literal["EQ", "GT", "GTE", "ISNULL", "LT", "LTE", "REGEX"]
 FilterOperatorType = Literal["EQ", "GE", "GT", "LE", "LT", "NE"]
@@ -224,14 +236,16 @@
 GetTableVersionsPaginatorName = Literal["get_table_versions"]
 GetTablesPaginatorName = Literal["get_tables"]
 GetTriggersPaginatorName = Literal["get_triggers"]
 GetUserDefinedFunctionsPaginatorName = Literal["get_user_defined_functions"]
 GlueRecordTypeType = Literal[
     "BIGDECIMAL", "BYTE", "DATE", "DOUBLE", "FLOAT", "INT", "LONG", "SHORT", "STRING", "TIMESTAMP"
 ]
+HudiTargetCompressionTypeType = Literal["gzip", "lzo", "snappy", "uncompressed"]
+JDBCConnectionTypeType = Literal["mysql", "oracle", "postgresql", "redshift", "sqlserver"]
 JDBCDataTypeType = Literal[
     "ARRAY",
     "BIGINT",
     "BINARY",
     "BIT",
     "BLOB",
     "BOOLEAN",
@@ -265,14 +279,15 @@
     "TIMESTAMP",
     "TIMESTAMP_WITH_TIMEZONE",
     "TIME_WITH_TIMEZONE",
     "TINYINT",
     "VARBINARY",
     "VARCHAR",
 ]
+JdbcMetadataEntryType = Literal["COMMENTS", "RAWTYPES"]
 JobBookmarksEncryptionModeType = Literal["CSE-KMS", "DISABLED"]
 JobRunStateType = Literal[
     "ERROR",
     "FAILED",
     "RUNNING",
     "STARTING",
     "STOPPED",
@@ -287,14 +302,15 @@
 ListRegistriesPaginatorName = Literal["list_registries"]
 ListSchemaVersionsPaginatorName = Literal["list_schema_versions"]
 ListSchemasPaginatorName = Literal["list_schemas"]
 LogicalOperatorType = Literal["EQUALS"]
 LogicalType = Literal["AND", "ANY"]
 MLUserDataEncryptionModeStringType = Literal["DISABLED", "SSE-KMS"]
 NodeTypeType = Literal["CRAWLER", "JOB", "TRIGGER"]
+ParamTypeType = Literal["bool", "complex", "float", "int", "list", "null", "str"]
 ParquetCompressionTypeType = Literal["gzip", "lzo", "none", "snappy", "uncompressed"]
 PartitionIndexStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 PermissionType = Literal[
     "ALL",
     "ALTER",
     "CREATE_DATABASE",
     "CREATE_TABLE",
@@ -306,30 +322,30 @@
 ]
 PermissionTypeType = Literal["CELL_FILTER_PERMISSION", "COLUMN_PERMISSION"]
 PiiTypeType = Literal["ColumnAudit", "ColumnMasking", "RowAudit", "RowMasking"]
 PrincipalTypeType = Literal["GROUP", "ROLE", "USER"]
 QuoteCharType = Literal["disabled", "quillemet", "quote", "single_quote"]
 RecrawlBehaviorType = Literal["CRAWL_EVENT_MODE", "CRAWL_EVERYTHING", "CRAWL_NEW_FOLDERS_ONLY"]
 RegistryStatusType = Literal["AVAILABLE", "DELETING"]
-ResourceShareTypeType = Literal["ALL", "FOREIGN"]
+ResourceShareTypeType = Literal["ALL", "FEDERATED", "FOREIGN"]
 ResourceTypeType = Literal["ARCHIVE", "FILE", "JAR"]
 S3EncryptionModeType = Literal["DISABLED", "SSE-KMS", "SSE-S3"]
 ScheduleStateType = Literal["NOT_SCHEDULED", "SCHEDULED", "TRANSITIONING"]
 SchemaDiffTypeType = Literal["SYNTAX_DIFF"]
 SchemaStatusType = Literal["AVAILABLE", "DELETING", "PENDING"]
 SchemaVersionStatusType = Literal["AVAILABLE", "DELETING", "FAILURE", "PENDING"]
 SeparatorType = Literal["comma", "ctrla", "pipe", "semicolon", "tab"]
 SessionStatusType = Literal["FAILED", "PROVISIONING", "READY", "STOPPED", "STOPPING", "TIMEOUT"]
 SortDirectionTypeType = Literal["ASCENDING", "DESCENDING"]
 SortType = Literal["ASC", "DESC"]
 SourceControlAuthStrategyType = Literal["AWS_SECRETS_MANAGER", "PERSONAL_ACCESS_TOKEN"]
 SourceControlProviderType = Literal["AWS_CODE_COMMIT", "GITHUB"]
-StartingPositionType = Literal["earliest", "latest", "trim_horizon"]
+StartingPositionType = Literal["earliest", "latest", "timestamp", "trim_horizon"]
 StatementStateType = Literal["AVAILABLE", "CANCELLED", "CANCELLING", "ERROR", "RUNNING", "WAITING"]
-TargetFormatType = Literal["avro", "csv", "json", "orc", "parquet"]
+TargetFormatType = Literal["avro", "csv", "delta", "hudi", "json", "orc", "parquet"]
 TaskRunSortColumnTypeType = Literal["STARTED", "STATUS", "TASK_RUN_TYPE"]
 TaskStatusTypeType = Literal[
     "FAILED", "RUNNING", "STARTING", "STOPPED", "STOPPING", "SUCCEEDED", "TIMEOUT"
 ]
 TaskTypeType = Literal[
     "EVALUATION", "EXPORT_LABELS", "FIND_MATCHES", "IMPORT_LABELS", "LABELING_SET_GENERATION"
 ]
@@ -348,15 +364,15 @@
     "DELETING",
     "UPDATING",
 ]
 TriggerTypeType = Literal["CONDITIONAL", "EVENT", "ON_DEMAND", "SCHEDULED"]
 UnionTypeType = Literal["ALL", "DISTINCT"]
 UpdateBehaviorType = Literal["LOG", "UPDATE_IN_DATABASE"]
 UpdateCatalogBehaviorType = Literal["LOG", "UPDATE_IN_DATABASE"]
-WorkerTypeType = Literal["G.025X", "G.1X", "G.2X", "Standard"]
+WorkerTypeType = Literal["G.025X", "G.1X", "G.2X", "G.4X", "G.8X", "Standard", "Z.2X"]
 WorkflowRunStatusType = Literal["COMPLETED", "ERROR", "RUNNING", "STOPPED", "STOPPING"]
 GlueServiceName = Literal["glue"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -366,23 +382,25 @@
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
@@ -392,30 +410,35 @@
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
@@ -441,14 +464,15 @@
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
@@ -493,51 +517,57 @@
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
@@ -550,14 +580,15 @@
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
@@ -569,28 +600,35 @@
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
@@ -618,56 +656,64 @@
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
@@ -718,19 +764,22 @@
     "ap-northeast-3",
     "ap-south-1",
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

### Comparing `mypy-boto3-glue-1.26.8/mypy_boto3_glue/literals.pyi` & `mypy-boto3-glue-1.27.0/mypy_boto3_glue/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 Type annotations for glue service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_glue.literals import AggFunctionType
+    from mypy_boto3_glue.literals import AdditionalOptionKeysType
 
-    data: AggFunctionType = "avg"
+    data: AdditionalOptionKeysType = "performanceTuning.caching"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
+    "AdditionalOptionKeysType",
     "AggFunctionType",
     "BackfillErrorCodeType",
     "BlueprintRunStateType",
     "BlueprintStatusType",
     "CatalogEncryptionModeType",
     "CloudWatchEncryptionModeType",
     "ColumnStatisticsTypeType",
@@ -32,16 +34,20 @@
     "ConnectionPropertyKeyType",
     "ConnectionTypeType",
     "CrawlStateType",
     "CrawlerHistoryStateType",
     "CrawlerLineageSettingsType",
     "CrawlerStateType",
     "CsvHeaderOptionType",
+    "DQStopJobOnFailureTimingType",
+    "DQTransformOutputType",
     "DataFormatType",
+    "DataQualityRuleResultStatusType",
     "DeleteBehaviorType",
+    "DeltaTargetCompressionTypeType",
     "EnableHybridValuesType",
     "ExecutionClassType",
     "ExistConditionType",
     "FieldNameType",
     "FilterLogicalOperatorType",
     "FilterOperationType",
     "FilterOperatorType",
@@ -59,27 +65,31 @@
     "GetResourcePoliciesPaginatorName",
     "GetSecurityConfigurationsPaginatorName",
     "GetTableVersionsPaginatorName",
     "GetTablesPaginatorName",
     "GetTriggersPaginatorName",
     "GetUserDefinedFunctionsPaginatorName",
     "GlueRecordTypeType",
+    "HudiTargetCompressionTypeType",
+    "JDBCConnectionTypeType",
     "JDBCDataTypeType",
+    "JdbcMetadataEntryType",
     "JobBookmarksEncryptionModeType",
     "JobRunStateType",
     "JoinTypeType",
     "LanguageType",
     "LastCrawlStatusType",
     "ListRegistriesPaginatorName",
     "ListSchemaVersionsPaginatorName",
     "ListSchemasPaginatorName",
     "LogicalOperatorType",
     "LogicalType",
     "MLUserDataEncryptionModeStringType",
     "NodeTypeType",
+    "ParamTypeType",
     "ParquetCompressionTypeType",
     "PartitionIndexStatusType",
     "PermissionType",
     "PermissionTypeType",
     "PiiTypeType",
     "PrincipalTypeType",
     "QuoteCharType",
@@ -117,14 +127,16 @@
     "GlueServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
+AdditionalOptionKeysType = Literal["performanceTuning.caching"]
 AggFunctionType = Literal[
     "avg",
     "count",
     "countDistinct",
     "first",
     "kurtosis",
     "last",
@@ -193,16 +205,20 @@
 ]
 ConnectionTypeType = Literal["CUSTOM", "JDBC", "KAFKA", "MARKETPLACE", "MONGODB", "NETWORK", "SFTP"]
 CrawlStateType = Literal["CANCELLED", "CANCELLING", "ERROR", "FAILED", "RUNNING", "SUCCEEDED"]
 CrawlerHistoryStateType = Literal["COMPLETED", "FAILED", "RUNNING", "STOPPED"]
 CrawlerLineageSettingsType = Literal["DISABLE", "ENABLE"]
 CrawlerStateType = Literal["READY", "RUNNING", "STOPPING"]
 CsvHeaderOptionType = Literal["ABSENT", "PRESENT", "UNKNOWN"]
+DQStopJobOnFailureTimingType = Literal["AfterDataLoad", "Immediate"]
+DQTransformOutputType = Literal["EvaluationResults", "PrimaryInput"]
 DataFormatType = Literal["AVRO", "JSON", "PROTOBUF"]
+DataQualityRuleResultStatusType = Literal["ERROR", "FAIL", "PASS"]
 DeleteBehaviorType = Literal["DELETE_FROM_DATABASE", "DEPRECATE_IN_DATABASE", "LOG"]
+DeltaTargetCompressionTypeType = Literal["snappy", "uncompressed"]
 EnableHybridValuesType = Literal["FALSE", "TRUE"]
 ExecutionClassType = Literal["FLEX", "STANDARD"]
 ExistConditionType = Literal["MUST_EXIST", "NONE", "NOT_EXIST"]
 FieldNameType = Literal["CRAWL_ID", "DPU_HOUR", "END_TIME", "START_TIME", "STATE"]
 FilterLogicalOperatorType = Literal["AND", "OR"]
 FilterOperationType = Literal["EQ", "GT", "GTE", "ISNULL", "LT", "LTE", "REGEX"]
 FilterOperatorType = Literal["EQ", "GE", "GT", "LE", "LT", "NE"]
@@ -222,14 +238,16 @@
 GetTableVersionsPaginatorName = Literal["get_table_versions"]
 GetTablesPaginatorName = Literal["get_tables"]
 GetTriggersPaginatorName = Literal["get_triggers"]
 GetUserDefinedFunctionsPaginatorName = Literal["get_user_defined_functions"]
 GlueRecordTypeType = Literal[
     "BIGDECIMAL", "BYTE", "DATE", "DOUBLE", "FLOAT", "INT", "LONG", "SHORT", "STRING", "TIMESTAMP"
 ]
+HudiTargetCompressionTypeType = Literal["gzip", "lzo", "snappy", "uncompressed"]
+JDBCConnectionTypeType = Literal["mysql", "oracle", "postgresql", "redshift", "sqlserver"]
 JDBCDataTypeType = Literal[
     "ARRAY",
     "BIGINT",
     "BINARY",
     "BIT",
     "BLOB",
     "BOOLEAN",
@@ -263,14 +281,15 @@
     "TIMESTAMP",
     "TIMESTAMP_WITH_TIMEZONE",
     "TIME_WITH_TIMEZONE",
     "TINYINT",
     "VARBINARY",
     "VARCHAR",
 ]
+JdbcMetadataEntryType = Literal["COMMENTS", "RAWTYPES"]
 JobBookmarksEncryptionModeType = Literal["CSE-KMS", "DISABLED"]
 JobRunStateType = Literal[
     "ERROR",
     "FAILED",
     "RUNNING",
     "STARTING",
     "STOPPED",
@@ -285,14 +304,15 @@
 ListRegistriesPaginatorName = Literal["list_registries"]
 ListSchemaVersionsPaginatorName = Literal["list_schema_versions"]
 ListSchemasPaginatorName = Literal["list_schemas"]
 LogicalOperatorType = Literal["EQUALS"]
 LogicalType = Literal["AND", "ANY"]
 MLUserDataEncryptionModeStringType = Literal["DISABLED", "SSE-KMS"]
 NodeTypeType = Literal["CRAWLER", "JOB", "TRIGGER"]
+ParamTypeType = Literal["bool", "complex", "float", "int", "list", "null", "str"]
 ParquetCompressionTypeType = Literal["gzip", "lzo", "none", "snappy", "uncompressed"]
 PartitionIndexStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 PermissionType = Literal[
     "ALL",
     "ALTER",
     "CREATE_DATABASE",
     "CREATE_TABLE",
@@ -304,30 +324,30 @@
 ]
 PermissionTypeType = Literal["CELL_FILTER_PERMISSION", "COLUMN_PERMISSION"]
 PiiTypeType = Literal["ColumnAudit", "ColumnMasking", "RowAudit", "RowMasking"]
 PrincipalTypeType = Literal["GROUP", "ROLE", "USER"]
 QuoteCharType = Literal["disabled", "quillemet", "quote", "single_quote"]
 RecrawlBehaviorType = Literal["CRAWL_EVENT_MODE", "CRAWL_EVERYTHING", "CRAWL_NEW_FOLDERS_ONLY"]
 RegistryStatusType = Literal["AVAILABLE", "DELETING"]
-ResourceShareTypeType = Literal["ALL", "FOREIGN"]
+ResourceShareTypeType = Literal["ALL", "FEDERATED", "FOREIGN"]
 ResourceTypeType = Literal["ARCHIVE", "FILE", "JAR"]
 S3EncryptionModeType = Literal["DISABLED", "SSE-KMS", "SSE-S3"]
 ScheduleStateType = Literal["NOT_SCHEDULED", "SCHEDULED", "TRANSITIONING"]
 SchemaDiffTypeType = Literal["SYNTAX_DIFF"]
 SchemaStatusType = Literal["AVAILABLE", "DELETING", "PENDING"]
 SchemaVersionStatusType = Literal["AVAILABLE", "DELETING", "FAILURE", "PENDING"]
 SeparatorType = Literal["comma", "ctrla", "pipe", "semicolon", "tab"]
 SessionStatusType = Literal["FAILED", "PROVISIONING", "READY", "STOPPED", "STOPPING", "TIMEOUT"]
 SortDirectionTypeType = Literal["ASCENDING", "DESCENDING"]
 SortType = Literal["ASC", "DESC"]
 SourceControlAuthStrategyType = Literal["AWS_SECRETS_MANAGER", "PERSONAL_ACCESS_TOKEN"]
 SourceControlProviderType = Literal["AWS_CODE_COMMIT", "GITHUB"]
-StartingPositionType = Literal["earliest", "latest", "trim_horizon"]
+StartingPositionType = Literal["earliest", "latest", "timestamp", "trim_horizon"]
 StatementStateType = Literal["AVAILABLE", "CANCELLED", "CANCELLING", "ERROR", "RUNNING", "WAITING"]
-TargetFormatType = Literal["avro", "csv", "json", "orc", "parquet"]
+TargetFormatType = Literal["avro", "csv", "delta", "hudi", "json", "orc", "parquet"]
 TaskRunSortColumnTypeType = Literal["STARTED", "STATUS", "TASK_RUN_TYPE"]
 TaskStatusTypeType = Literal[
     "FAILED", "RUNNING", "STARTING", "STOPPED", "STOPPING", "SUCCEEDED", "TIMEOUT"
 ]
 TaskTypeType = Literal[
     "EVALUATION", "EXPORT_LABELS", "FIND_MATCHES", "IMPORT_LABELS", "LABELING_SET_GENERATION"
 ]
@@ -346,15 +366,15 @@
     "DELETING",
     "UPDATING",
 ]
 TriggerTypeType = Literal["CONDITIONAL", "EVENT", "ON_DEMAND", "SCHEDULED"]
 UnionTypeType = Literal["ALL", "DISTINCT"]
 UpdateBehaviorType = Literal["LOG", "UPDATE_IN_DATABASE"]
 UpdateCatalogBehaviorType = Literal["LOG", "UPDATE_IN_DATABASE"]
-WorkerTypeType = Literal["G.025X", "G.1X", "G.2X", "Standard"]
+WorkerTypeType = Literal["G.025X", "G.1X", "G.2X", "G.4X", "G.8X", "Standard", "Z.2X"]
 WorkflowRunStatusType = Literal["COMPLETED", "ERROR", "RUNNING", "STOPPED", "STOPPING"]
 GlueServiceName = Literal["glue"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -364,23 +384,25 @@
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
@@ -390,30 +412,35 @@
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
@@ -439,14 +466,15 @@
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
@@ -491,51 +519,57 @@
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
@@ -548,14 +582,15 @@
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
@@ -567,28 +602,35 @@
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
@@ -616,56 +658,64 @@
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
@@ -716,19 +766,22 @@
     "ap-northeast-3",
     "ap-south-1",
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

### Comparing `mypy-boto3-glue-1.26.8/mypy_boto3_glue/paginator.py` & `mypy-boto3-glue-1.27.0/mypy_boto3_glue/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 class GetClassifiersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetClassifiers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getclassifierspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetClassifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetClassifiers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getclassifierspaginator)
         """
 
 
@@ -144,15 +144,15 @@
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         Filter: GetConnectionsFilterTypeDef = ...,
         HidePassword: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getconnectionspaginator)
         """
 
 
@@ -162,30 +162,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getcrawlermetricspaginator)
     """
 
     def paginate(
         self,
         *,
         CrawlerNameList: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetCrawlerMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetCrawlerMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getcrawlermetricspaginator)
         """
 
 
 class GetCrawlersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetCrawlers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getcrawlerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetCrawlersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetCrawlers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getcrawlerspaginator)
         """
 
 
@@ -196,60 +196,60 @@
     """
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDatabasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getdatabasespaginator)
         """
 
 
 class GetDevEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetDevEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getdevendpointspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDevEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetDevEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getdevendpointspaginator)
         """
 
 
 class GetJobRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetJobRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getjobrunspaginator)
     """
 
     def paginate(
-        self, *, JobName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, JobName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getjobrunspaginator)
         """
 
 
 class GetJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getjobspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getjobspaginator)
         """
 
 
@@ -261,15 +261,15 @@
 
     def paginate(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetPartitionIndexesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetPartitionIndexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getpartitionindexespaginator)
         """
 
 
@@ -286,45 +286,45 @@
         TableName: str,
         CatalogId: str = ...,
         Expression: str = ...,
         Segment: SegmentTypeDef = ...,
         ExcludeColumnSchema: bool = ...,
         TransactionId: str = ...,
         QueryAsOfTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetPartitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetPartitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getpartitionspaginator)
         """
 
 
 class GetResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getresourcepoliciespaginator)
         """
 
 
 class GetSecurityConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetSecurityConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getsecurityconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetSecurityConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetSecurityConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getsecurityconfigurationspaginator)
         """
 
 
@@ -336,15 +336,15 @@
 
     def paginate(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTableVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTableVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#gettableversionspaginator)
         """
 
 
@@ -358,30 +358,30 @@
         self,
         *,
         DatabaseName: str,
         CatalogId: str = ...,
         Expression: str = ...,
         TransactionId: str = ...,
         QueryAsOfTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTablesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#gettablespaginator)
         """
 
 
 class GetTriggersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTriggers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#gettriggerspaginator)
     """
 
     def paginate(
-        self, *, DependentJobName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DependentJobName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTriggersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTriggers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#gettriggerspaginator)
         """
 
 
@@ -393,58 +393,61 @@
 
     def paginate(
         self,
         *,
         Pattern: str,
         CatalogId: str = ...,
         DatabaseName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetUserDefinedFunctionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetUserDefinedFunctions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getuserdefinedfunctionspaginator)
         """
 
 
 class ListRegistriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListRegistries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#listregistriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListRegistries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#listregistriespaginator)
         """
 
 
 class ListSchemaVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListSchemaVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#listschemaversionspaginator)
     """
 
     def paginate(
-        self, *, SchemaId: SchemaIdTypeDef, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SchemaId: SchemaIdTypeDef, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchemaVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListSchemaVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#listschemaversionspaginator)
         """
 
 
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#listschemaspaginator)
     """
 
     def paginate(
-        self, *, RegistryId: RegistryIdTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        RegistryId: RegistryIdTypeDef = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#listschemaspaginator)
         """
```

### Comparing `mypy-boto3-glue-1.26.8/mypy_boto3_glue/paginator.pyi` & `mypy-boto3-glue-1.27.0/mypy_boto3_glue/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 class GetClassifiersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetClassifiers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getclassifierspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetClassifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetClassifiers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getclassifierspaginator)
         """
 
 class GetConnectionsPaginator(Paginator):
@@ -140,15 +140,15 @@
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         Filter: GetConnectionsFilterTypeDef = ...,
         HidePassword: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetConnections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getconnectionspaginator)
         """
 
 class GetCrawlerMetricsPaginator(Paginator):
@@ -157,29 +157,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getcrawlermetricspaginator)
     """
 
     def paginate(
         self,
         *,
         CrawlerNameList: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetCrawlerMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetCrawlerMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getcrawlermetricspaginator)
         """
 
 class GetCrawlersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetCrawlers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getcrawlerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetCrawlersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetCrawlers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getcrawlerspaginator)
         """
 
 class GetDatabasesPaginator(Paginator):
@@ -189,57 +189,57 @@
     """
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDatabasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getdatabasespaginator)
         """
 
 class GetDevEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetDevEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getdevendpointspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetDevEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetDevEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getdevendpointspaginator)
         """
 
 class GetJobRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetJobRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getjobrunspaginator)
     """
 
     def paginate(
-        self, *, JobName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, JobName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getjobrunspaginator)
         """
 
 class GetJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getjobspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getjobspaginator)
         """
 
 class GetPartitionIndexesPaginator(Paginator):
@@ -250,15 +250,15 @@
 
     def paginate(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetPartitionIndexesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetPartitionIndexes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getpartitionindexespaginator)
         """
 
 class GetPartitionsPaginator(Paginator):
@@ -274,43 +274,43 @@
         TableName: str,
         CatalogId: str = ...,
         Expression: str = ...,
         Segment: SegmentTypeDef = ...,
         ExcludeColumnSchema: bool = ...,
         TransactionId: str = ...,
         QueryAsOfTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetPartitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetPartitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getpartitionspaginator)
         """
 
 class GetResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getresourcepoliciespaginator)
         """
 
 class GetSecurityConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetSecurityConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getsecurityconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetSecurityConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetSecurityConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getsecurityconfigurationspaginator)
         """
 
 class GetTableVersionsPaginator(Paginator):
@@ -321,15 +321,15 @@
 
     def paginate(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTableVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTableVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#gettableversionspaginator)
         """
 
 class GetTablesPaginator(Paginator):
@@ -342,29 +342,29 @@
         self,
         *,
         DatabaseName: str,
         CatalogId: str = ...,
         Expression: str = ...,
         TransactionId: str = ...,
         QueryAsOfTime: Union[datetime, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTablesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#gettablespaginator)
         """
 
 class GetTriggersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTriggers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#gettriggerspaginator)
     """
 
     def paginate(
-        self, *, DependentJobName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DependentJobName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetTriggersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetTriggers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#gettriggerspaginator)
         """
 
 class GetUserDefinedFunctionsPaginator(Paginator):
@@ -375,55 +375,58 @@
 
     def paginate(
         self,
         *,
         Pattern: str,
         CatalogId: str = ...,
         DatabaseName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[GetUserDefinedFunctionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.GetUserDefinedFunctions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#getuserdefinedfunctionspaginator)
         """
 
 class ListRegistriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListRegistries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#listregistriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListRegistries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#listregistriespaginator)
         """
 
 class ListSchemaVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListSchemaVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#listschemaversionspaginator)
     """
 
     def paginate(
-        self, *, SchemaId: SchemaIdTypeDef, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, SchemaId: SchemaIdTypeDef, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchemaVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListSchemaVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#listschemaversionspaginator)
         """
 
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#listschemaspaginator)
     """
 
     def paginate(
-        self, *, RegistryId: RegistryIdTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        RegistryId: RegistryIdTypeDef = ...,
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/paginators/#listschemaspaginator)
         """
```

### Comparing `mypy-boto3-glue-1.26.8/mypy_boto3_glue/type_defs.py` & `mypy-boto3-glue-1.27.0/mypy_boto3_glue/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,33 +30,41 @@
     ConnectionTypeType,
     CrawlerHistoryStateType,
     CrawlerLineageSettingsType,
     CrawlerStateType,
     CrawlStateType,
     CsvHeaderOptionType,
     DataFormatType,
+    DataQualityRuleResultStatusType,
     DeleteBehaviorType,
+    DeltaTargetCompressionTypeType,
+    DQStopJobOnFailureTimingType,
+    DQTransformOutputType,
     EnableHybridValuesType,
     ExecutionClassType,
     ExistConditionType,
     FieldNameType,
     FilterLogicalOperatorType,
     FilterOperationType,
     FilterOperatorType,
     FilterValueTypeType,
     GlueRecordTypeType,
+    HudiTargetCompressionTypeType,
+    JDBCConnectionTypeType,
     JDBCDataTypeType,
+    JdbcMetadataEntryType,
     JobBookmarksEncryptionModeType,
     JobRunStateType,
     JoinTypeType,
     LanguageType,
     LastCrawlStatusType,
     LogicalType,
     MLUserDataEncryptionModeStringType,
     NodeTypeType,
+    ParamTypeType,
     ParquetCompressionTypeType,
     PartitionIndexStatusType,
     PermissionType,
     PermissionTypeType,
     PiiTypeType,
     PrincipalTypeType,
     QuoteCharType,
@@ -100,55 +108,62 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "NotificationPropertyTypeDef",
     "AggregateOperationTypeDef",
+    "AmazonRedshiftAdvancedOptionTypeDef",
+    "OptionTypeDef",
     "ApplyMappingTypeDef",
     "AuditContextTypeDef",
     "PartitionValueListTypeDef",
     "BasicCatalogTargetTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchDeleteConnectionRequestRequestTypeDef",
     "ErrorDetailTypeDef",
     "BatchDeleteTableRequestRequestTypeDef",
     "BatchDeleteTableVersionRequestRequestTypeDef",
     "BatchGetBlueprintsRequestRequestTypeDef",
     "BatchGetCrawlersRequestRequestTypeDef",
     "BatchGetCustomEntityTypesRequestRequestTypeDef",
     "CustomEntityTypeTypeDef",
+    "BatchGetDataQualityResultRequestRequestTypeDef",
     "BatchGetDevEndpointsRequestRequestTypeDef",
     "DevEndpointTypeDef",
     "BatchGetJobsRequestRequestTypeDef",
     "BatchGetTriggersRequestRequestTypeDef",
     "BatchGetWorkflowsRequestRequestTypeDef",
     "BatchStopJobRunRequestRequestTypeDef",
     "BatchStopJobRunSuccessfulSubmissionTypeDef",
     "BinaryColumnStatisticsDataTypeDef",
     "BlueprintDetailsTypeDef",
     "BlueprintRunTypeDef",
     "LastActiveDefinitionTypeDef",
     "BooleanColumnStatisticsDataTypeDef",
+    "CancelDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    "CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     "CancelMLTaskRunRequestRequestTypeDef",
+    "CancelMLTaskRunResponseTypeDef",
     "CancelStatementRequestRequestTypeDef",
     "CatalogEntryTypeDef",
     "CatalogImportStatusTypeDef",
     "KafkaStreamingSourceOptionsTypeDef",
     "StreamingDataPreviewOptionsTypeDef",
     "KinesisStreamingSourceOptionsTypeDef",
     "CatalogSchemaChangePolicyTypeDef",
     "CatalogSourceTypeDef",
     "CatalogTargetTypeDef",
     "CheckSchemaVersionValidityInputRequestTypeDef",
+    "CheckSchemaVersionValidityResponseTypeDef",
     "CsvClassifierTypeDef",
     "GrokClassifierTypeDef",
     "JsonClassifierTypeDef",
     "XMLClassifierTypeDef",
     "CloudWatchEncryptionTypeDef",
+    "DirectJDBCSourceTypeDef",
     "DropDuplicatesTypeDef",
     "DropFieldsTypeDef",
     "DynamoDBCatalogSourceTypeDef",
     "FillMissingValuesTypeDef",
     "MergeTypeDef",
     "MicrosoftSQLServerCatalogSourceTypeDef",
     "MicrosoftSQLServerCatalogTargetTypeDef",
@@ -182,277 +197,311 @@
     "ConnectionPasswordEncryptionTypeDef",
     "ConnectionsListTypeDef",
     "CrawlTypeDef",
     "CrawlerHistoryTypeDef",
     "CrawlerMetricsTypeDef",
     "DeltaTargetTypeDef",
     "DynamoDBTargetTypeDef",
+    "IcebergTargetTypeDef",
     "JdbcTargetTypeDef",
     "MongoDBTargetTypeDef",
     "S3TargetTypeDef",
     "LakeFormationConfigurationTypeDef",
     "LastCrawlInfoTypeDef",
     "LineageConfigurationTypeDef",
     "RecrawlPolicyTypeDef",
     "ScheduleTypeDef",
     "SchemaChangePolicyTypeDef",
     "CrawlsFilterTypeDef",
     "CreateBlueprintRequestRequestTypeDef",
+    "CreateBlueprintResponseTypeDef",
     "CreateCsvClassifierRequestTypeDef",
     "CreateGrokClassifierRequestTypeDef",
     "CreateJsonClassifierRequestTypeDef",
     "CreateXMLClassifierRequestTypeDef",
     "CreateCustomEntityTypeRequestRequestTypeDef",
+    "CreateCustomEntityTypeResponseTypeDef",
+    "DataQualityTargetTableTypeDef",
+    "CreateDataQualityRulesetResponseTypeDef",
     "CreateDevEndpointRequestRequestTypeDef",
+    "CreateDevEndpointResponseTypeDef",
     "ExecutionPropertyTypeDef",
     "JobCommandTypeDef",
     "SourceControlDetailsTypeDef",
+    "CreateJobResponseTypeDef",
     "GlueTableTypeDef",
+    "CreateMLTransformResponseTypeDef",
     "PartitionIndexTypeDef",
     "CreateRegistryInputRequestTypeDef",
+    "CreateRegistryResponseTypeDef",
     "RegistryIdTypeDef",
+    "CreateSchemaResponseTypeDef",
+    "CreateScriptResponseTypeDef",
+    "CreateSecurityConfigurationResponseTypeDef",
     "SessionCommandTypeDef",
     "EventBatchingConditionTypeDef",
+    "CreateTriggerResponseTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
+    "CreateWorkflowResponseTypeDef",
+    "DQResultsPublishingOptionsTypeDef",
+    "DQStopJobOnFailureOptionsTypeDef",
     "EncryptionAtRestTypeDef",
     "DataLakePrincipalTypeDef",
+    "DataQualityEvaluationRunAdditionalRunOptionsTypeDef",
+    "DataQualityRuleResultTypeDef",
     "DatabaseIdentifierTypeDef",
+    "FederatedDatabaseTypeDef",
     "DatatypeTypeDef",
     "DecimalNumberTypeDef",
     "DeleteBlueprintRequestRequestTypeDef",
+    "DeleteBlueprintResponseTypeDef",
     "DeleteClassifierRequestRequestTypeDef",
     "DeleteColumnStatisticsForPartitionRequestRequestTypeDef",
     "DeleteColumnStatisticsForTableRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteCrawlerRequestRequestTypeDef",
     "DeleteCustomEntityTypeRequestRequestTypeDef",
+    "DeleteCustomEntityTypeResponseTypeDef",
+    "DeleteDataQualityRulesetRequestRequestTypeDef",
     "DeleteDatabaseRequestRequestTypeDef",
     "DeleteDevEndpointRequestRequestTypeDef",
     "DeleteJobRequestRequestTypeDef",
+    "DeleteJobResponseTypeDef",
     "DeleteMLTransformRequestRequestTypeDef",
+    "DeleteMLTransformResponseTypeDef",
     "DeletePartitionIndexRequestRequestTypeDef",
     "DeletePartitionRequestRequestTypeDef",
+    "DeleteRegistryResponseTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "SchemaIdTypeDef",
+    "DeleteSchemaResponseTypeDef",
     "DeleteSecurityConfigurationRequestRequestTypeDef",
     "DeleteSessionRequestRequestTypeDef",
+    "DeleteSessionResponseTypeDef",
     "DeleteTableRequestRequestTypeDef",
     "DeleteTableVersionRequestRequestTypeDef",
     "DeleteTriggerRequestRequestTypeDef",
+    "DeleteTriggerResponseTypeDef",
     "DeleteUserDefinedFunctionRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
+    "DeleteWorkflowResponseTypeDef",
     "DevEndpointCustomLibrariesTypeDef",
     "DirectSchemaChangePolicyTypeDef",
     "NullCheckBoxListTypeDef",
+    "TransformConfigParameterTypeDef",
     "EdgeTypeDef",
     "JobBookmarksEncryptionTypeDef",
     "S3EncryptionTypeDef",
     "ErrorDetailsTypeDef",
     "ExportLabelsTaskRunPropertiesTypeDef",
+    "FederatedTableTypeDef",
     "FilterValueTypeDef",
     "FindMatchesParametersTypeDef",
     "FindMatchesTaskRunPropertiesTypeDef",
     "GetBlueprintRequestRequestTypeDef",
     "GetBlueprintRunRequestRequestTypeDef",
     "GetBlueprintRunsRequestRequestTypeDef",
     "GetCatalogImportStatusRequestRequestTypeDef",
     "GetClassifierRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     "GetClassifiersRequestRequestTypeDef",
     "GetColumnStatisticsForPartitionRequestRequestTypeDef",
     "GetColumnStatisticsForTableRequestRequestTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "GetConnectionsFilterTypeDef",
+    "GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef",
     "GetCrawlerMetricsRequestRequestTypeDef",
     "GetCrawlerRequestRequestTypeDef",
+    "GetCrawlersRequestGetCrawlersPaginateTypeDef",
     "GetCrawlersRequestRequestTypeDef",
     "GetCustomEntityTypeRequestRequestTypeDef",
+    "GetCustomEntityTypeResponseTypeDef",
     "GetDataCatalogEncryptionSettingsRequestRequestTypeDef",
+    "GetDataQualityResultRequestRequestTypeDef",
+    "GetDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    "GetDataQualityRulesetEvaluationRunRequestRequestTypeDef",
+    "GetDataQualityRulesetRequestRequestTypeDef",
     "GetDatabaseRequestRequestTypeDef",
+    "GetDatabasesRequestGetDatabasesPaginateTypeDef",
     "GetDatabasesRequestRequestTypeDef",
     "GetDataflowGraphRequestRequestTypeDef",
     "GetDevEndpointRequestRequestTypeDef",
+    "GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef",
     "GetDevEndpointsRequestRequestTypeDef",
     "GetJobBookmarkRequestRequestTypeDef",
     "JobBookmarkEntryTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetJobRunRequestRequestTypeDef",
+    "GetJobRunsRequestGetJobRunsPaginateTypeDef",
     "GetJobRunsRequestRequestTypeDef",
+    "GetJobsRequestGetJobsPaginateTypeDef",
     "GetJobsRequestRequestTypeDef",
     "GetMLTaskRunRequestRequestTypeDef",
     "TaskRunFilterCriteriaTypeDef",
     "TaskRunSortCriteriaTypeDef",
     "GetMLTransformRequestRequestTypeDef",
     "SchemaColumnTypeDef",
     "TransformSortCriteriaTypeDef",
     "MappingEntryTypeDef",
+    "GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef",
     "GetPartitionIndexesRequestRequestTypeDef",
     "GetPartitionRequestRequestTypeDef",
     "SegmentTypeDef",
+    "GetPlanResponseTypeDef",
+    "GetRegistryResponseTypeDef",
+    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GluePolicyTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "GetSchemaByDefinitionResponseTypeDef",
+    "GetSchemaResponseTypeDef",
     "SchemaVersionNumberTypeDef",
+    "GetSchemaVersionResponseTypeDef",
+    "GetSchemaVersionsDiffResponseTypeDef",
     "GetSecurityConfigurationRequestRequestTypeDef",
+    "GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef",
     "GetSecurityConfigurationsRequestRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
     "GetStatementRequestRequestTypeDef",
     "GetTableRequestRequestTypeDef",
     "GetTableVersionRequestRequestTypeDef",
+    "GetTableVersionsRequestGetTableVersionsPaginateTypeDef",
     "GetTableVersionsRequestRequestTypeDef",
+    "GetTablesRequestGetTablesPaginateTypeDef",
     "GetTablesRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
+    "GetTagsResponseTypeDef",
     "GetTriggerRequestRequestTypeDef",
+    "GetTriggersRequestGetTriggersPaginateTypeDef",
     "GetTriggersRequestRequestTypeDef",
     "GetUserDefinedFunctionRequestRequestTypeDef",
+    "GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef",
     "GetUserDefinedFunctionsRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
+    "GetWorkflowRunPropertiesResponseTypeDef",
     "GetWorkflowRunRequestRequestTypeDef",
     "GetWorkflowRunsRequestRequestTypeDef",
     "GlueStudioSchemaColumnTypeDef",
     "S3SourceAdditionalOptionsTypeDef",
     "ImportCatalogToGlueRequestRequestTypeDef",
     "ImportLabelsTaskRunPropertiesTypeDef",
     "JDBCConnectorOptionsTypeDef",
     "PredecessorTypeDef",
     "JoinColumnTypeDef",
     "KeySchemaElementTypeDef",
     "LabelingSetGenerationTaskRunPropertiesTypeDef",
     "ListBlueprintsRequestRequestTypeDef",
+    "ListBlueprintsResponseTypeDef",
     "ListCrawlersRequestRequestTypeDef",
+    "ListCrawlersResponseTypeDef",
     "ListCustomEntityTypesRequestRequestTypeDef",
     "ListDevEndpointsRequestRequestTypeDef",
+    "ListDevEndpointsResponseTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListJobsResponseTypeDef",
+    "ListMLTransformsResponseTypeDef",
+    "ListRegistriesInputListRegistriesPaginateTypeDef",
     "ListRegistriesInputRequestTypeDef",
     "RegistryListItemTypeDef",
     "SchemaVersionListItemTypeDef",
     "SchemaListItemTypeDef",
     "ListSessionsRequestRequestTypeDef",
     "ListStatementsRequestRequestTypeDef",
     "ListTriggersRequestRequestTypeDef",
+    "ListTriggersResponseTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
+    "ListWorkflowsResponseTypeDef",
     "MLUserDataEncryptionTypeDef",
     "MappingTypeDef",
     "OtherMetadataValueListItemTypeDef",
     "MetadataKeyValuePairTypeDef",
     "OrderTypeDef",
+    "PaginatorConfigTypeDef",
     "PropertyPredicateTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "PutSchemaVersionMetadataResponseTypeDef",
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
     "UpsertRedshiftTargetOptionsTypeDef",
+    "RegisterSchemaVersionResponseTypeDef",
+    "RemoveSchemaVersionMetadataResponseTypeDef",
     "ResetJobBookmarkRequestRequestTypeDef",
     "ResourceUriTypeDef",
+    "ResponseMetadataTypeDef",
     "ResumeWorkflowRunRequestRequestTypeDef",
+    "ResumeWorkflowRunResponseTypeDef",
     "RunStatementRequestRequestTypeDef",
+    "RunStatementResponseTypeDef",
     "S3DirectSourceAdditionalOptionsTypeDef",
     "SortCriterionTypeDef",
     "SerDeInfoTypeDef",
     "SkewedInfoTypeDef",
     "SqlAliasTypeDef",
     "StartBlueprintRunRequestRequestTypeDef",
+    "StartBlueprintRunResponseTypeDef",
     "StartCrawlerRequestRequestTypeDef",
     "StartCrawlerScheduleRequestRequestTypeDef",
+    "StartDataQualityRuleRecommendationRunResponseTypeDef",
+    "StartDataQualityRulesetEvaluationRunResponseTypeDef",
     "StartExportLabelsTaskRunRequestRequestTypeDef",
+    "StartExportLabelsTaskRunResponseTypeDef",
     "StartImportLabelsTaskRunRequestRequestTypeDef",
+    "StartImportLabelsTaskRunResponseTypeDef",
+    "StartJobRunResponseTypeDef",
     "StartMLEvaluationTaskRunRequestRequestTypeDef",
+    "StartMLEvaluationTaskRunResponseTypeDef",
     "StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef",
+    "StartMLLabelingSetGenerationTaskRunResponseTypeDef",
     "StartTriggerRequestRequestTypeDef",
+    "StartTriggerResponseTypeDef",
     "StartWorkflowRunRequestRequestTypeDef",
+    "StartWorkflowRunResponseTypeDef",
     "StartingEventBatchConditionTypeDef",
     "StatementOutputDataTypeDef",
     "StopCrawlerRequestRequestTypeDef",
     "StopCrawlerScheduleRequestRequestTypeDef",
     "StopSessionRequestRequestTypeDef",
+    "StopSessionResponseTypeDef",
     "StopTriggerRequestRequestTypeDef",
+    "StopTriggerResponseTypeDef",
     "StopWorkflowRunRequestRequestTypeDef",
     "TableIdentifierTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBlueprintRequestRequestTypeDef",
+    "UpdateBlueprintResponseTypeDef",
     "UpdateCsvClassifierRequestTypeDef",
     "UpdateGrokClassifierRequestTypeDef",
     "UpdateJsonClassifierRequestTypeDef",
     "UpdateXMLClassifierRequestTypeDef",
     "UpdateCrawlerScheduleRequestRequestTypeDef",
+    "UpdateDataQualityRulesetRequestRequestTypeDef",
+    "UpdateDataQualityRulesetResponseTypeDef",
     "UpdateJobFromSourceControlRequestRequestTypeDef",
+    "UpdateJobFromSourceControlResponseTypeDef",
+    "UpdateJobResponseTypeDef",
+    "UpdateMLTransformResponseTypeDef",
+    "UpdateRegistryResponseTypeDef",
+    "UpdateSchemaResponseTypeDef",
     "UpdateSourceControlFromJobRequestRequestTypeDef",
+    "UpdateSourceControlFromJobResponseTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
+    "UpdateWorkflowResponseTypeDef",
     "WorkflowRunStatisticsTypeDef",
     "ActionTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "AggregateTypeDef",
+    "AmazonRedshiftNodeDataTypeDef",
     "GetUnfilteredPartitionMetadataRequestRequestTypeDef",
     "GetUnfilteredTableMetadataRequestRequestTypeDef",
     "BackfillErrorTypeDef",
     "BatchDeletePartitionRequestRequestTypeDef",
     "BatchGetPartitionRequestRequestTypeDef",
-    "CancelMLTaskRunResponseTypeDef",
-    "CheckSchemaVersionValidityResponseTypeDef",
-    "CreateBlueprintResponseTypeDef",
-    "CreateCustomEntityTypeResponseTypeDef",
-    "CreateDevEndpointResponseTypeDef",
-    "CreateJobResponseTypeDef",
-    "CreateMLTransformResponseTypeDef",
-    "CreateRegistryResponseTypeDef",
-    "CreateSchemaResponseTypeDef",
-    "CreateScriptResponseTypeDef",
-    "CreateSecurityConfigurationResponseTypeDef",
-    "CreateTriggerResponseTypeDef",
-    "CreateWorkflowResponseTypeDef",
-    "DeleteBlueprintResponseTypeDef",
-    "DeleteCustomEntityTypeResponseTypeDef",
-    "DeleteJobResponseTypeDef",
-    "DeleteMLTransformResponseTypeDef",
-    "DeleteRegistryResponseTypeDef",
-    "DeleteSchemaResponseTypeDef",
-    "DeleteSessionResponseTypeDef",
-    "DeleteTriggerResponseTypeDef",
-    "DeleteWorkflowResponseTypeDef",
-    "GetCustomEntityTypeResponseTypeDef",
-    "GetPlanResponseTypeDef",
-    "GetRegistryResponseTypeDef",
-    "GetResourcePolicyResponseTypeDef",
-    "GetSchemaByDefinitionResponseTypeDef",
-    "GetSchemaResponseTypeDef",
-    "GetSchemaVersionResponseTypeDef",
-    "GetSchemaVersionsDiffResponseTypeDef",
-    "GetTagsResponseTypeDef",
-    "GetWorkflowRunPropertiesResponseTypeDef",
-    "ListBlueprintsResponseTypeDef",
-    "ListCrawlersResponseTypeDef",
-    "ListDevEndpointsResponseTypeDef",
-    "ListJobsResponseTypeDef",
-    "ListMLTransformsResponseTypeDef",
-    "ListTriggersResponseTypeDef",
-    "ListWorkflowsResponseTypeDef",
-    "PutResourcePolicyResponseTypeDef",
-    "PutSchemaVersionMetadataResponseTypeDef",
-    "RegisterSchemaVersionResponseTypeDef",
-    "RemoveSchemaVersionMetadataResponseTypeDef",
-    "ResumeWorkflowRunResponseTypeDef",
-    "RunStatementResponseTypeDef",
-    "StartBlueprintRunResponseTypeDef",
-    "StartExportLabelsTaskRunResponseTypeDef",
-    "StartImportLabelsTaskRunResponseTypeDef",
-    "StartJobRunResponseTypeDef",
-    "StartMLEvaluationTaskRunResponseTypeDef",
-    "StartMLLabelingSetGenerationTaskRunResponseTypeDef",
-    "StartTriggerResponseTypeDef",
-    "StartWorkflowRunResponseTypeDef",
-    "StopSessionResponseTypeDef",
-    "StopTriggerResponseTypeDef",
-    "UpdateBlueprintResponseTypeDef",
-    "UpdateJobFromSourceControlResponseTypeDef",
-    "UpdateJobResponseTypeDef",
-    "UpdateMLTransformResponseTypeDef",
-    "UpdateRegistryResponseTypeDef",
-    "UpdateSchemaResponseTypeDef",
-    "UpdateSourceControlFromJobResponseTypeDef",
-    "UpdateWorkflowResponseTypeDef",
     "BatchDeleteConnectionResponseTypeDef",
     "BatchStopJobRunErrorTypeDef",
     "BatchUpdatePartitionFailureEntryTypeDef",
     "ColumnErrorTypeDef",
     "PartitionErrorTypeDef",
     "TableErrorTypeDef",
     "TableVersionErrorTypeDef",
@@ -467,70 +516,66 @@
     "GetCatalogImportStatusResponseTypeDef",
     "CatalogKafkaSourceTypeDef",
     "DirectKafkaSourceTypeDef",
     "CatalogKinesisSourceTypeDef",
     "DirectKinesisSourceTypeDef",
     "GovernedCatalogTargetTypeDef",
     "S3CatalogTargetTypeDef",
+    "S3DeltaCatalogTargetTypeDef",
+    "S3HudiCatalogTargetTypeDef",
     "ClassifierTypeDef",
     "CodeGenNodeTypeDef",
     "LocationTypeDef",
     "PredicateTypeDef",
     "FindMatchesMetricsTypeDef",
     "ConnectionInputTypeDef",
     "ConnectionTypeDef",
     "CrawlerNodeDetailsTypeDef",
     "ListCrawlsResponseTypeDef",
     "GetCrawlerMetricsResponseTypeDef",
     "CrawlerTargetsTypeDef",
     "ListCrawlsRequestRequestTypeDef",
     "CreateClassifierRequestRequestTypeDef",
+    "CreateDataQualityRulesetRequestRequestTypeDef",
+    "DataQualityRulesetFilterCriteriaTypeDef",
+    "DataQualityRulesetListDetailsTypeDef",
+    "GetDataQualityRulesetResponseTypeDef",
+    "DataSourceTypeDef",
     "CreatePartitionIndexRequestRequestTypeDef",
     "CreateSchemaInputRequestTypeDef",
     "DeleteRegistryInputRequestTypeDef",
     "GetRegistryInputRequestTypeDef",
+    "ListSchemasInputListSchemasPaginateTypeDef",
     "ListSchemasInputRequestTypeDef",
     "UpdateRegistryInputRequestTypeDef",
     "CreateSessionRequestRequestTypeDef",
     "SessionTypeDef",
+    "EvaluateDataQualityMultiFrameTypeDef",
+    "EvaluateDataQualityTypeDef",
     "DataCatalogEncryptionSettingsTypeDef",
     "PrincipalPermissionsTypeDef",
     "NullValueFieldTypeDef",
     "DecimalColumnStatisticsDataTypeDef",
     "DeleteSchemaInputRequestTypeDef",
     "DeleteSchemaVersionsInputRequestTypeDef",
     "GetSchemaByDefinitionInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
+    "ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
     "ListSchemaVersionsInputRequestTypeDef",
     "RegisterSchemaVersionInputRequestTypeDef",
     "SchemaReferenceTypeDef",
     "UpdateDevEndpointRequestRequestTypeDef",
+    "S3DeltaDirectTargetTypeDef",
     "S3DirectTargetTypeDef",
     "S3GlueParquetTargetTypeDef",
+    "S3HudiDirectTargetTypeDef",
     "EncryptionConfigurationTypeDef",
     "SchemaVersionErrorItemTypeDef",
     "FilterExpressionTypeDef",
     "TransformParametersTypeDef",
-    "GetClassifiersRequestGetClassifiersPaginateTypeDef",
-    "GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef",
-    "GetCrawlersRequestGetCrawlersPaginateTypeDef",
-    "GetDatabasesRequestGetDatabasesPaginateTypeDef",
-    "GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef",
-    "GetJobRunsRequestGetJobRunsPaginateTypeDef",
-    "GetJobsRequestGetJobsPaginateTypeDef",
-    "GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef",
-    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    "GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef",
-    "GetTableVersionsRequestGetTableVersionsPaginateTypeDef",
-    "GetTablesRequestGetTablesPaginateTypeDef",
-    "GetTriggersRequestGetTriggersPaginateTypeDef",
-    "GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef",
-    "ListRegistriesInputListRegistriesPaginateTypeDef",
-    "ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
-    "ListSchemasInputListSchemasPaginateTypeDef",
     "GetConnectionsRequestGetConnectionsPaginateTypeDef",
     "GetConnectionsRequestRequestTypeDef",
     "GetJobBookmarkResponseTypeDef",
     "ResetJobBookmarkResponseTypeDef",
     "GetMLTaskRunsRequestRequestTypeDef",
     "TransformFilterCriteriaTypeDef",
     "GetMappingResponseTypeDef",
@@ -557,14 +602,16 @@
     "RemoveSchemaVersionMetadataInputRequestTypeDef",
     "RedshiftTargetTypeDef",
     "UserDefinedFunctionInputTypeDef",
     "UserDefinedFunctionTypeDef",
     "SearchTablesRequestRequestTypeDef",
     "StatementOutputTypeDef",
     "UpdateClassifierRequestRequestTypeDef",
+    "AmazonRedshiftSourceTypeDef",
+    "AmazonRedshiftTargetTypeDef",
     "PartitionIndexDescriptorTypeDef",
     "BatchStopJobRunResponseTypeDef",
     "BatchUpdatePartitionResponseTypeDef",
     "BatchCreatePartitionResponseTypeDef",
     "BatchDeletePartitionResponseTypeDef",
     "BatchDeleteTableResponseTypeDef",
     "BatchDeleteTableVersionResponseTypeDef",
@@ -583,14 +630,28 @@
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "GetConnectionResponseTypeDef",
     "GetConnectionsResponseTypeDef",
     "CrawlerTypeDef",
     "CreateCrawlerRequestRequestTypeDef",
     "UpdateCrawlerRequestRequestTypeDef",
+    "ListDataQualityRulesetsRequestRequestTypeDef",
+    "ListDataQualityRulesetsResponseTypeDef",
+    "DataQualityResultDescriptionTypeDef",
+    "DataQualityResultFilterCriteriaTypeDef",
+    "DataQualityResultTypeDef",
+    "DataQualityRuleRecommendationRunDescriptionTypeDef",
+    "DataQualityRuleRecommendationRunFilterTypeDef",
+    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
+    "DataQualityRulesetEvaluationRunFilterTypeDef",
+    "GetDataQualityResultResponseTypeDef",
+    "GetDataQualityRuleRecommendationRunResponseTypeDef",
+    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
+    "StartDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    "StartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     "CreateSessionResponseTypeDef",
     "GetSessionResponseTypeDef",
     "ListSessionsResponseTypeDef",
     "GetDataCatalogEncryptionSettingsResponseTypeDef",
     "PutDataCatalogEncryptionSettingsRequestRequestTypeDef",
     "DatabaseInputTypeDef",
     "DatabaseTypeDef",
@@ -601,18 +662,25 @@
     "SecurityConfigurationTypeDef",
     "DeleteSchemaVersionsResponseTypeDef",
     "FilterTypeDef",
     "UpdateMLTransformRequestRequestTypeDef",
     "GetMLTransformsRequestRequestTypeDef",
     "ListMLTransformsRequestRequestTypeDef",
     "AthenaConnectorSourceTypeDef",
+    "CatalogDeltaSourceTypeDef",
+    "CatalogHudiSourceTypeDef",
     "CustomCodeTypeDef",
+    "DynamicTransformTypeDef",
     "JDBCConnectorSourceTypeDef",
     "JDBCConnectorTargetTypeDef",
+    "S3CatalogDeltaSourceTypeDef",
+    "S3CatalogHudiSourceTypeDef",
     "S3CsvSourceTypeDef",
+    "S3DeltaSourceTypeDef",
+    "S3HudiSourceTypeDef",
     "S3JsonSourceTypeDef",
     "S3ParquetSourceTypeDef",
     "SparkConnectorSourceTypeDef",
     "SparkConnectorTargetTypeDef",
     "SparkSQLTypeDef",
     "GetJobRunResponseTypeDef",
     "GetJobRunsResponseTypeDef",
@@ -634,14 +702,21 @@
     "UpdateTriggerResponseTypeDef",
     "UpdateTriggerRequestRequestTypeDef",
     "GetMLTransformResponseTypeDef",
     "MLTransformTypeDef",
     "BatchGetCrawlersResponseTypeDef",
     "GetCrawlerResponseTypeDef",
     "GetCrawlersResponseTypeDef",
+    "ListDataQualityResultsResponseTypeDef",
+    "ListDataQualityResultsRequestRequestTypeDef",
+    "BatchGetDataQualityResultResponseTypeDef",
+    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
+    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
+    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
+    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
     "CreateDatabaseRequestRequestTypeDef",
     "UpdateDatabaseRequestRequestTypeDef",
     "GetDatabaseResponseTypeDef",
     "GetDatabasesResponseTypeDef",
     "ColumnStatisticsTypeDef",
     "PartitionInputTypeDef",
     "PartitionTypeDef",
@@ -710,14 +785,33 @@
     "AggregateOperationTypeDef",
     {
         "Column": List[str],
         "AggFunc": AggFunctionType,
     },
 )
 
+AmazonRedshiftAdvancedOptionTypeDef = TypedDict(
+    "AmazonRedshiftAdvancedOptionTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
+OptionTypeDef = TypedDict(
+    "OptionTypeDef",
+    {
+        "Value": str,
+        "Label": str,
+        "Description": str,
+    },
+    total=False,
+)
+
 ApplyMappingTypeDef = TypedDict(
     "ApplyMappingTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Mapping": List["MappingTypeDef"],
     },
@@ -746,25 +840,14 @@
         "Name": str,
         "Inputs": List[str],
         "Database": str,
         "Table": str,
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
 _RequiredBatchDeleteConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionNameList": Sequence[str],
     },
 )
 _OptionalBatchDeleteConnectionRequestRequestTypeDef = TypedDict(
@@ -892,14 +975,21 @@
 )
 
 
 class CustomEntityTypeTypeDef(_RequiredCustomEntityTypeTypeDef, _OptionalCustomEntityTypeTypeDef):
     pass
 
 
+BatchGetDataQualityResultRequestRequestTypeDef = TypedDict(
+    "BatchGetDataQualityResultRequestRequestTypeDef",
+    {
+        "ResultIds": Sequence[str],
+    },
+)
+
 BatchGetDevEndpointsRequestRequestTypeDef = TypedDict(
     "BatchGetDevEndpointsRequestRequestTypeDef",
     {
         "DevEndpointNames": Sequence[str],
     },
 )
 
@@ -1039,22 +1129,46 @@
     {
         "NumberOfTrues": int,
         "NumberOfFalses": int,
         "NumberOfNulls": int,
     },
 )
 
+CancelDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
+    "CancelDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    {
+        "RunId": str,
+    },
+)
+
+CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
+    "CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef",
+    {
+        "RunId": str,
+    },
+)
+
 CancelMLTaskRunRequestRequestTypeDef = TypedDict(
     "CancelMLTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
         "TaskRunId": str,
     },
 )
 
+CancelMLTaskRunResponseTypeDef = TypedDict(
+    "CancelMLTaskRunResponseTypeDef",
+    {
+        "TransformId": str,
+        "TaskRunId": str,
+        "Status": TaskStatusTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCancelStatementRequestRequestTypeDef = TypedDict(
     "_RequiredCancelStatementRequestRequestTypeDef",
     {
         "SessionId": str,
         "Id": int,
     },
 )
@@ -1105,14 +1219,18 @@
         "StartingOffsets": str,
         "EndingOffsets": str,
         "PollTimeoutMs": int,
         "NumRetries": int,
         "RetryIntervalMs": int,
         "MaxOffsetsPerTrigger": int,
         "MinPartitions": int,
+        "IncludeHeaders": bool,
+        "AddRecordTimestamp": str,
+        "EmitConsumerLagMetrics": str,
+        "StartingTimestamp": datetime,
     },
     total=False,
 )
 
 StreamingDataPreviewOptionsTypeDef = TypedDict(
     "StreamingDataPreviewOptionsTypeDef",
     {
@@ -1139,14 +1257,17 @@
         "NumRetries": int,
         "RetryIntervalMs": int,
         "MaxRetryIntervalMs": int,
         "AvoidEmptyBatches": bool,
         "StreamArn": str,
         "RoleArn": str,
         "RoleSessionName": str,
+        "AddRecordTimestamp": str,
+        "EmitConsumerLagMetrics": str,
+        "StartingTimestamp": datetime,
     },
     total=False,
 )
 
 CatalogSchemaChangePolicyTypeDef = TypedDict(
     "CatalogSchemaChangePolicyTypeDef",
     {
@@ -1191,14 +1312,23 @@
     "CheckSchemaVersionValidityInputRequestTypeDef",
     {
         "DataFormat": DataFormatType,
         "SchemaDefinition": str,
     },
 )
 
+CheckSchemaVersionValidityResponseTypeDef = TypedDict(
+    "CheckSchemaVersionValidityResponseTypeDef",
+    {
+        "Valid": bool,
+        "Error": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCsvClassifierTypeDef = TypedDict(
     "_RequiredCsvClassifierTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCsvClassifierTypeDef = TypedDict(
@@ -1298,14 +1428,37 @@
     {
         "CloudWatchEncryptionMode": CloudWatchEncryptionModeType,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
+_RequiredDirectJDBCSourceTypeDef = TypedDict(
+    "_RequiredDirectJDBCSourceTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "ConnectionName": str,
+        "ConnectionType": JDBCConnectionTypeType,
+    },
+)
+_OptionalDirectJDBCSourceTypeDef = TypedDict(
+    "_OptionalDirectJDBCSourceTypeDef",
+    {
+        "RedshiftTmpDir": str,
+    },
+    total=False,
+)
+
+
+class DirectJDBCSourceTypeDef(_RequiredDirectJDBCSourceTypeDef, _OptionalDirectJDBCSourceTypeDef):
+    pass
+
+
 _RequiredDropDuplicatesTypeDef = TypedDict(
     "_RequiredDropDuplicatesTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
     },
 )
@@ -1840,34 +1993,47 @@
 
 DeltaTargetTypeDef = TypedDict(
     "DeltaTargetTypeDef",
     {
         "DeltaTables": List[str],
         "ConnectionName": str,
         "WriteManifest": bool,
+        "CreateNativeDeltaTable": bool,
     },
     total=False,
 )
 
 DynamoDBTargetTypeDef = TypedDict(
     "DynamoDBTargetTypeDef",
     {
         "Path": str,
         "scanAll": bool,
         "scanRate": float,
     },
     total=False,
 )
 
+IcebergTargetTypeDef = TypedDict(
+    "IcebergTargetTypeDef",
+    {
+        "Paths": List[str],
+        "ConnectionName": str,
+        "Exclusions": List[str],
+        "MaximumTraversalDepth": int,
+    },
+    total=False,
+)
+
 JdbcTargetTypeDef = TypedDict(
     "JdbcTargetTypeDef",
     {
         "ConnectionName": str,
         "Path": str,
         "Exclusions": List[str],
+        "EnableAdditionalMetadata": List[JdbcMetadataEntryType],
     },
     total=False,
 )
 
 MongoDBTargetTypeDef = TypedDict(
     "MongoDBTargetTypeDef",
     {
@@ -1976,14 +2142,22 @@
 
 class CreateBlueprintRequestRequestTypeDef(
     _RequiredCreateBlueprintRequestRequestTypeDef, _OptionalCreateBlueprintRequestRequestTypeDef
 ):
     pass
 
 
+CreateBlueprintResponseTypeDef = TypedDict(
+    "CreateBlueprintResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredCreateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateCsvClassifierRequestTypeDef = TypedDict(
@@ -2068,26 +2242,65 @@
         "RegexString": str,
     },
 )
 _OptionalCreateCustomEntityTypeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCustomEntityTypeRequestRequestTypeDef",
     {
         "ContextWords": Sequence[str],
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
 class CreateCustomEntityTypeRequestRequestTypeDef(
     _RequiredCreateCustomEntityTypeRequestRequestTypeDef,
     _OptionalCreateCustomEntityTypeRequestRequestTypeDef,
 ):
     pass
 
 
+CreateCustomEntityTypeResponseTypeDef = TypedDict(
+    "CreateCustomEntityTypeResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredDataQualityTargetTableTypeDef = TypedDict(
+    "_RequiredDataQualityTargetTableTypeDef",
+    {
+        "TableName": str,
+        "DatabaseName": str,
+    },
+)
+_OptionalDataQualityTargetTableTypeDef = TypedDict(
+    "_OptionalDataQualityTargetTableTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+
+class DataQualityTargetTableTypeDef(
+    _RequiredDataQualityTargetTableTypeDef, _OptionalDataQualityTargetTableTypeDef
+):
+    pass
+
+
+CreateDataQualityRulesetResponseTypeDef = TypedDict(
+    "CreateDataQualityRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateDevEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
         "RoleArn": str,
     },
 )
@@ -2114,28 +2327,55 @@
 
 class CreateDevEndpointRequestRequestTypeDef(
     _RequiredCreateDevEndpointRequestRequestTypeDef, _OptionalCreateDevEndpointRequestRequestTypeDef
 ):
     pass
 
 
+CreateDevEndpointResponseTypeDef = TypedDict(
+    "CreateDevEndpointResponseTypeDef",
+    {
+        "EndpointName": str,
+        "Status": str,
+        "SecurityGroupIds": List[str],
+        "SubnetId": str,
+        "RoleArn": str,
+        "YarnEndpointAddress": str,
+        "ZeppelinRemoteSparkInterpreterPort": int,
+        "NumberOfNodes": int,
+        "WorkerType": WorkerTypeType,
+        "GlueVersion": str,
+        "NumberOfWorkers": int,
+        "AvailabilityZone": str,
+        "VpcId": str,
+        "ExtraPythonLibsS3Path": str,
+        "ExtraJarsS3Path": str,
+        "FailureReason": str,
+        "SecurityConfiguration": str,
+        "CreatedTimestamp": datetime,
+        "Arguments": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExecutionPropertyTypeDef = TypedDict(
     "ExecutionPropertyTypeDef",
     {
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
 
 JobCommandTypeDef = TypedDict(
     "JobCommandTypeDef",
     {
         "Name": str,
         "ScriptLocation": str,
         "PythonVersion": str,
+        "Runtime": str,
     },
     total=False,
 )
 
 SourceControlDetailsTypeDef = TypedDict(
     "SourceControlDetailsTypeDef",
     {
@@ -2147,35 +2387,52 @@
         "LastCommitId": str,
         "AuthStrategy": SourceControlAuthStrategyType,
         "AuthToken": str,
     },
     total=False,
 )
 
+CreateJobResponseTypeDef = TypedDict(
+    "CreateJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGlueTableTypeDef = TypedDict(
     "_RequiredGlueTableTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
 _OptionalGlueTableTypeDef = TypedDict(
     "_OptionalGlueTableTypeDef",
     {
         "CatalogId": str,
         "ConnectionName": str,
+        "AdditionalOptions": Dict[str, str],
     },
     total=False,
 )
 
 
 class GlueTableTypeDef(_RequiredGlueTableTypeDef, _OptionalGlueTableTypeDef):
     pass
 
 
+CreateMLTransformResponseTypeDef = TypedDict(
+    "CreateMLTransformResponseTypeDef",
+    {
+        "TransformId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PartitionIndexTypeDef = TypedDict(
     "PartitionIndexTypeDef",
     {
         "Keys": Sequence[str],
         "IndexName": str,
     },
 )
@@ -2198,23 +2455,73 @@
 
 class CreateRegistryInputRequestTypeDef(
     _RequiredCreateRegistryInputRequestTypeDef, _OptionalCreateRegistryInputRequestTypeDef
 ):
     pass
 
 
+CreateRegistryResponseTypeDef = TypedDict(
+    "CreateRegistryResponseTypeDef",
+    {
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegistryIdTypeDef = TypedDict(
     "RegistryIdTypeDef",
     {
         "RegistryName": str,
         "RegistryArn": str,
     },
     total=False,
 )
 
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "RegistryName": str,
+        "RegistryArn": str,
+        "SchemaName": str,
+        "SchemaArn": str,
+        "Description": str,
+        "DataFormat": DataFormatType,
+        "Compatibility": CompatibilityType,
+        "SchemaCheckpoint": int,
+        "LatestSchemaVersion": int,
+        "NextSchemaVersion": int,
+        "SchemaStatus": SchemaStatusType,
+        "Tags": Dict[str, str],
+        "SchemaVersionId": str,
+        "SchemaVersionStatus": SchemaVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateScriptResponseTypeDef = TypedDict(
+    "CreateScriptResponseTypeDef",
+    {
+        "PythonScript": str,
+        "ScalaCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSecurityConfigurationResponseTypeDef = TypedDict(
+    "CreateSecurityConfigurationResponseTypeDef",
+    {
+        "Name": str,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SessionCommandTypeDef = TypedDict(
     "SessionCommandTypeDef",
     {
         "Name": str,
         "PythonVersion": str,
     },
     total=False,
@@ -2237,14 +2544,22 @@
 
 class EventBatchingConditionTypeDef(
     _RequiredEventBatchingConditionTypeDef, _OptionalEventBatchingConditionTypeDef
 ):
     pass
 
 
+CreateTriggerResponseTypeDef = TypedDict(
+    "CreateTriggerResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
@@ -2261,14 +2576,41 @@
 
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
 
 
+CreateWorkflowResponseTypeDef = TypedDict(
+    "CreateWorkflowResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DQResultsPublishingOptionsTypeDef = TypedDict(
+    "DQResultsPublishingOptionsTypeDef",
+    {
+        "EvaluationContext": str,
+        "ResultsS3Prefix": str,
+        "CloudWatchMetricsEnabled": bool,
+        "ResultsPublishingEnabled": bool,
+    },
+    total=False,
+)
+
+DQStopJobOnFailureOptionsTypeDef = TypedDict(
+    "DQStopJobOnFailureOptionsTypeDef",
+    {
+        "StopJobOnFailureTiming": DQStopJobOnFailureTimingType,
+    },
+    total=False,
+)
+
 _RequiredEncryptionAtRestTypeDef = TypedDict(
     "_RequiredEncryptionAtRestTypeDef",
     {
         "CatalogEncryptionMode": CatalogEncryptionModeType,
     },
 )
 _OptionalEncryptionAtRestTypeDef = TypedDict(
@@ -2288,19 +2630,50 @@
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
     total=False,
 )
 
+DataQualityEvaluationRunAdditionalRunOptionsTypeDef = TypedDict(
+    "DataQualityEvaluationRunAdditionalRunOptionsTypeDef",
+    {
+        "CloudWatchMetricsEnabled": bool,
+        "ResultsS3Prefix": str,
+    },
+    total=False,
+)
+
+DataQualityRuleResultTypeDef = TypedDict(
+    "DataQualityRuleResultTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "EvaluationMessage": str,
+        "Result": DataQualityRuleResultStatusType,
+        "EvaluatedMetrics": Dict[str, float],
+    },
+    total=False,
+)
+
 DatabaseIdentifierTypeDef = TypedDict(
     "DatabaseIdentifierTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
+        "Region": str,
+    },
+    total=False,
+)
+
+FederatedDatabaseTypeDef = TypedDict(
+    "FederatedDatabaseTypeDef",
+    {
+        "Identifier": str,
+        "ConnectionName": str,
     },
     total=False,
 )
 
 DatatypeTypeDef = TypedDict(
     "DatatypeTypeDef",
     {
@@ -2320,14 +2693,22 @@
 DeleteBlueprintRequestRequestTypeDef = TypedDict(
     "DeleteBlueprintRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteBlueprintResponseTypeDef = TypedDict(
+    "DeleteBlueprintResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteClassifierRequestRequestTypeDef = TypedDict(
     "DeleteClassifierRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2411,14 +2792,29 @@
 DeleteCustomEntityTypeRequestRequestTypeDef = TypedDict(
     "DeleteCustomEntityTypeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteCustomEntityTypeResponseTypeDef = TypedDict(
+    "DeleteCustomEntityTypeResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteDataQualityRulesetRequestRequestTypeDef = TypedDict(
+    "DeleteDataQualityRulesetRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 _RequiredDeleteDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDatabaseRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDeleteDatabaseRequestRequestTypeDef = TypedDict(
@@ -2446,21 +2842,37 @@
 DeleteJobRequestRequestTypeDef = TypedDict(
     "DeleteJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 
+DeleteJobResponseTypeDef = TypedDict(
+    "DeleteJobResponseTypeDef",
+    {
+        "JobName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteMLTransformRequestRequestTypeDef = TypedDict(
     "DeleteMLTransformRequestRequestTypeDef",
     {
         "TransformId": str,
     },
 )
 
+DeleteMLTransformResponseTypeDef = TypedDict(
+    "DeleteMLTransformResponseTypeDef",
+    {
+        "TransformId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeletePartitionIndexRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePartitionIndexRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "IndexName": str,
     },
@@ -2500,14 +2912,24 @@
 
 class DeletePartitionRequestRequestTypeDef(
     _RequiredDeletePartitionRequestRequestTypeDef, _OptionalDeletePartitionRequestRequestTypeDef
 ):
     pass
 
 
+DeleteRegistryResponseTypeDef = TypedDict(
+    "DeleteRegistryResponseTypeDef",
+    {
+        "RegistryName": str,
+        "RegistryArn": str,
+        "Status": RegistryStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyHashCondition": str,
         "ResourceArn": str,
     },
     total=False,
@@ -2519,14 +2941,24 @@
         "SchemaArn": str,
         "SchemaName": str,
         "RegistryName": str,
     },
     total=False,
 )
 
+DeleteSchemaResponseTypeDef = TypedDict(
+    "DeleteSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "SchemaName": str,
+        "Status": SchemaStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSecurityConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteSecurityConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2547,14 +2979,22 @@
 
 class DeleteSessionRequestRequestTypeDef(
     _RequiredDeleteSessionRequestRequestTypeDef, _OptionalDeleteSessionRequestRequestTypeDef
 ):
     pass
 
 
+DeleteSessionResponseTypeDef = TypedDict(
+    "DeleteSessionResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteTableRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -2601,14 +3041,22 @@
 DeleteTriggerRequestRequestTypeDef = TypedDict(
     "DeleteTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteTriggerResponseTypeDef = TypedDict(
+    "DeleteTriggerResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteUserDefinedFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteUserDefinedFunctionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "FunctionName": str,
     },
 )
@@ -2631,14 +3079,22 @@
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteWorkflowResponseTypeDef = TypedDict(
+    "DeleteWorkflowResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DevEndpointCustomLibrariesTypeDef = TypedDict(
     "DevEndpointCustomLibrariesTypeDef",
     {
         "ExtraPythonLibsS3Path": str,
         "ExtraJarsS3Path": str,
     },
     total=False,
@@ -2661,14 +3117,40 @@
         "IsEmpty": bool,
         "IsNullString": bool,
         "IsNegOne": bool,
     },
     total=False,
 )
 
+_RequiredTransformConfigParameterTypeDef = TypedDict(
+    "_RequiredTransformConfigParameterTypeDef",
+    {
+        "Name": str,
+        "Type": ParamTypeType,
+    },
+)
+_OptionalTransformConfigParameterTypeDef = TypedDict(
+    "_OptionalTransformConfigParameterTypeDef",
+    {
+        "ValidationRule": str,
+        "ValidationMessage": str,
+        "Value": List[str],
+        "ListType": ParamTypeType,
+        "IsOptional": bool,
+    },
+    total=False,
+)
+
+
+class TransformConfigParameterTypeDef(
+    _RequiredTransformConfigParameterTypeDef, _OptionalTransformConfigParameterTypeDef
+):
+    pass
+
+
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "SourceId": str,
         "DestinationId": str,
     },
     total=False,
@@ -2705,14 +3187,24 @@
     "ExportLabelsTaskRunPropertiesTypeDef",
     {
         "OutputS3Path": str,
     },
     total=False,
 )
 
+FederatedTableTypeDef = TypedDict(
+    "FederatedTableTypeDef",
+    {
+        "Identifier": str,
+        "DatabaseIdentifier": str,
+        "ConnectionName": str,
+    },
+    total=False,
+)
+
 FilterValueTypeDef = TypedDict(
     "FilterValueTypeDef",
     {
         "Type": FilterValueTypeType,
         "Value": List[str],
     },
 )
@@ -2801,20 +3293,18 @@
 GetClassifierRequestRequestTypeDef = TypedDict(
     "GetClassifierRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetClassifiersRequestGetClassifiersPaginateTypeDef = TypedDict(
+    "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetClassifiersRequestRequestTypeDef = TypedDict(
     "GetClassifiersRequestRequestTypeDef",
     {
@@ -2900,14 +3390,23 @@
     {
         "MatchCriteria": Sequence[str],
         "ConnectionType": ConnectionTypeType,
     },
     total=False,
 )
 
+GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef = TypedDict(
+    "GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef",
+    {
+        "CrawlerNameList": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetCrawlerMetricsRequestRequestTypeDef = TypedDict(
     "GetCrawlerMetricsRequestRequestTypeDef",
     {
         "CrawlerNameList": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -2917,14 +3416,22 @@
 GetCrawlerRequestRequestTypeDef = TypedDict(
     "GetCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+GetCrawlersRequestGetCrawlersPaginateTypeDef = TypedDict(
+    "GetCrawlersRequestGetCrawlersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetCrawlersRequestRequestTypeDef = TypedDict(
     "GetCrawlersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -2933,22 +3440,60 @@
 GetCustomEntityTypeRequestRequestTypeDef = TypedDict(
     "GetCustomEntityTypeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+GetCustomEntityTypeResponseTypeDef = TypedDict(
+    "GetCustomEntityTypeResponseTypeDef",
+    {
+        "Name": str,
+        "RegexString": str,
+        "ContextWords": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDataCatalogEncryptionSettingsRequestRequestTypeDef = TypedDict(
     "GetDataCatalogEncryptionSettingsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+GetDataQualityResultRequestRequestTypeDef = TypedDict(
+    "GetDataQualityResultRequestRequestTypeDef",
+    {
+        "ResultId": str,
+    },
+)
+
+GetDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
+    "GetDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    {
+        "RunId": str,
+    },
+)
+
+GetDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
+    "GetDataQualityRulesetEvaluationRunRequestRequestTypeDef",
+    {
+        "RunId": str,
+    },
+)
+
+GetDataQualityRulesetRequestRequestTypeDef = TypedDict(
+    "GetDataQualityRulesetRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 _RequiredGetDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredGetDatabaseRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetDatabaseRequestRequestTypeDef = TypedDict(
@@ -2962,14 +3507,24 @@
 
 class GetDatabaseRequestRequestTypeDef(
     _RequiredGetDatabaseRequestRequestTypeDef, _OptionalGetDatabaseRequestRequestTypeDef
 ):
     pass
 
 
+GetDatabasesRequestGetDatabasesPaginateTypeDef = TypedDict(
+    "GetDatabasesRequestGetDatabasesPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceShareType": ResourceShareTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetDatabasesRequestRequestTypeDef = TypedDict(
     "GetDatabasesRequestRequestTypeDef",
     {
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
         "ResourceShareType": ResourceShareTypeType,
@@ -2988,14 +3543,22 @@
 GetDevEndpointRequestRequestTypeDef = TypedDict(
     "GetDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
 
+GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef = TypedDict(
+    "GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetDevEndpointsRequestRequestTypeDef = TypedDict(
     "GetDevEndpointsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -3061,14 +3624,36 @@
 
 class GetJobRunRequestRequestTypeDef(
     _RequiredGetJobRunRequestRequestTypeDef, _OptionalGetJobRunRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef",
+    {
+        "JobName": str,
+    },
+)
+_OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetJobRunsRequestGetJobRunsPaginateTypeDef(
+    _RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef,
+    _OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJobRunsRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 _OptionalGetJobRunsRequestRequestTypeDef = TypedDict(
@@ -3083,14 +3668,22 @@
 
 class GetJobRunsRequestRequestTypeDef(
     _RequiredGetJobRunsRequestRequestTypeDef, _OptionalGetJobRunsRequestRequestTypeDef
 ):
     pass
 
 
+GetJobsRequestGetJobsPaginateTypeDef = TypedDict(
+    "GetJobsRequestGetJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetJobsRequestRequestTypeDef = TypedDict(
     "GetJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -3156,14 +3749,38 @@
         "TargetTable": str,
         "TargetPath": str,
         "TargetType": str,
     },
     total=False,
 )
 
+_RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef = TypedDict(
+    "_RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+    },
+)
+_OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef = TypedDict(
+    "_OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef(
+    _RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
+    _OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetPartitionIndexesRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionIndexesRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3211,14 +3828,44 @@
     "SegmentTypeDef",
     {
         "SegmentNumber": int,
         "TotalSegments": int,
     },
 )
 
+GetPlanResponseTypeDef = TypedDict(
+    "GetPlanResponseTypeDef",
+    {
+        "PythonScript": str,
+        "ScalaCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetRegistryResponseTypeDef = TypedDict(
+    "GetRegistryResponseTypeDef",
+    {
+        "RegistryName": str,
+        "RegistryArn": str,
+        "Description": str,
+        "Status": RegistryStatusType,
+        "CreatedTime": str,
+        "UpdatedTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "GetResourcePoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -3239,30 +3886,103 @@
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
     total=False,
 )
 
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "PolicyInJson": str,
+        "PolicyHash": str,
+        "CreateTime": datetime,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSchemaByDefinitionResponseTypeDef = TypedDict(
+    "GetSchemaByDefinitionResponseTypeDef",
+    {
+        "SchemaVersionId": str,
+        "SchemaArn": str,
+        "DataFormat": DataFormatType,
+        "Status": SchemaVersionStatusType,
+        "CreatedTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSchemaResponseTypeDef = TypedDict(
+    "GetSchemaResponseTypeDef",
+    {
+        "RegistryName": str,
+        "RegistryArn": str,
+        "SchemaName": str,
+        "SchemaArn": str,
+        "Description": str,
+        "DataFormat": DataFormatType,
+        "Compatibility": CompatibilityType,
+        "SchemaCheckpoint": int,
+        "LatestSchemaVersion": int,
+        "NextSchemaVersion": int,
+        "SchemaStatus": SchemaStatusType,
+        "CreatedTime": str,
+        "UpdatedTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SchemaVersionNumberTypeDef = TypedDict(
     "SchemaVersionNumberTypeDef",
     {
         "LatestVersion": bool,
         "VersionNumber": int,
     },
     total=False,
 )
 
+GetSchemaVersionResponseTypeDef = TypedDict(
+    "GetSchemaVersionResponseTypeDef",
+    {
+        "SchemaVersionId": str,
+        "SchemaDefinition": str,
+        "DataFormat": DataFormatType,
+        "SchemaArn": str,
+        "VersionNumber": int,
+        "Status": SchemaVersionStatusType,
+        "CreatedTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSchemaVersionsDiffResponseTypeDef = TypedDict(
+    "GetSchemaVersionsDiffResponseTypeDef",
+    {
+        "Diff": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSecurityConfigurationRequestRequestTypeDef = TypedDict(
     "GetSecurityConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef = TypedDict(
+    "GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetSecurityConfigurationsRequestRequestTypeDef = TypedDict(
     "GetSecurityConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -3354,14 +4074,38 @@
 
 class GetTableVersionRequestRequestTypeDef(
     _RequiredGetTableVersionRequestRequestTypeDef, _OptionalGetTableVersionRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+    },
+)
+_OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetTableVersionsRequestGetTableVersionsPaginateTypeDef(
+    _RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
+    _OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetTableVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableVersionsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3378,14 +4122,40 @@
 
 class GetTableVersionsRequestRequestTypeDef(
     _RequiredGetTableVersionsRequestRequestTypeDef, _OptionalGetTableVersionsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
+    "_RequiredGetTablesRequestGetTablesPaginateTypeDef",
+    {
+        "DatabaseName": str,
+    },
+)
+_OptionalGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
+    "_OptionalGetTablesRequestGetTablesPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "Expression": str,
+        "TransactionId": str,
+        "QueryAsOfTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetTablesRequestGetTablesPaginateTypeDef(
+    _RequiredGetTablesRequestGetTablesPaginateTypeDef,
+    _OptionalGetTablesRequestGetTablesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetTablesRequestRequestTypeDef = TypedDict(
     "_RequiredGetTablesRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalGetTablesRequestRequestTypeDef = TypedDict(
@@ -3411,21 +4181,38 @@
 GetTagsRequestRequestTypeDef = TypedDict(
     "GetTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTriggerRequestRequestTypeDef = TypedDict(
     "GetTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+GetTriggersRequestGetTriggersPaginateTypeDef = TypedDict(
+    "GetTriggersRequestGetTriggersPaginateTypeDef",
+    {
+        "DependentJobName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetTriggersRequestRequestTypeDef = TypedDict(
     "GetTriggersRequestRequestTypeDef",
     {
         "NextToken": str,
         "DependentJobName": str,
         "MaxResults": int,
     },
@@ -3451,14 +4238,38 @@
 class GetUserDefinedFunctionRequestRequestTypeDef(
     _RequiredGetUserDefinedFunctionRequestRequestTypeDef,
     _OptionalGetUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef = TypedDict(
+    "_RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef",
+    {
+        "Pattern": str,
+    },
+)
+_OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef = TypedDict(
+    "_OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "DatabaseName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef(
+    _RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
+    _OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetUserDefinedFunctionsRequestRequestTypeDef",
     {
         "Pattern": str,
     },
 )
 _OptionalGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
@@ -3505,14 +4316,22 @@
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
 
+GetWorkflowRunPropertiesResponseTypeDef = TypedDict(
+    "GetWorkflowRunPropertiesResponseTypeDef",
+    {
+        "RunProperties": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetWorkflowRunRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
@@ -3655,53 +4474,107 @@
         "NextToken": str,
         "MaxResults": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+ListBlueprintsResponseTypeDef = TypedDict(
+    "ListBlueprintsResponseTypeDef",
+    {
+        "Blueprints": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListCrawlersRequestRequestTypeDef = TypedDict(
     "ListCrawlersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+ListCrawlersResponseTypeDef = TypedDict(
+    "ListCrawlersResponseTypeDef",
+    {
+        "CrawlerNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListCustomEntityTypesRequestRequestTypeDef = TypedDict(
     "ListCustomEntityTypesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 ListDevEndpointsRequestRequestTypeDef = TypedDict(
     "ListDevEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+ListDevEndpointsResponseTypeDef = TypedDict(
+    "ListDevEndpointsResponseTypeDef",
+    {
+        "DevEndpointNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+ListJobsResponseTypeDef = TypedDict(
+    "ListJobsResponseTypeDef",
+    {
+        "JobNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListMLTransformsResponseTypeDef = TypedDict(
+    "ListMLTransformsResponseTypeDef",
+    {
+        "TransformIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListRegistriesInputListRegistriesPaginateTypeDef = TypedDict(
+    "ListRegistriesInputListRegistriesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRegistriesInputRequestTypeDef = TypedDict(
     "ListRegistriesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -3786,23 +4659,41 @@
         "DependentJobName": str,
         "MaxResults": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+ListTriggersResponseTypeDef = TypedDict(
+    "ListTriggersResponseTypeDef",
+    {
+        "TriggerNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListWorkflowsRequestRequestTypeDef = TypedDict(
     "ListWorkflowsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListWorkflowsResponseTypeDef = TypedDict(
+    "ListWorkflowsResponseTypeDef",
+    {
+        "Workflows": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredMLUserDataEncryptionTypeDef = TypedDict(
     "_RequiredMLUserDataEncryptionTypeDef",
     {
         "MlUserDataEncryptionMode": MLUserDataEncryptionModeStringType,
     },
 )
 _OptionalMLUserDataEncryptionTypeDef = TypedDict(
@@ -3855,14 +4746,24 @@
     "OrderTypeDef",
     {
         "Column": str,
         "SortOrder": int,
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
 PropertyPredicateTypeDef = TypedDict(
     "PropertyPredicateTypeDef",
     {
         "Key": str,
         "Value": str,
         "Comparator": ComparatorType,
     },
@@ -3889,14 +4790,37 @@
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
 
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "PolicyHash": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutSchemaVersionMetadataResponseTypeDef = TypedDict(
+    "PutSchemaVersionMetadataResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "SchemaName": str,
+        "RegistryName": str,
+        "LatestVersion": bool,
+        "VersionNumber": int,
+        "SchemaVersionId": str,
+        "MetadataKey": str,
+        "MetadataValue": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutWorkflowRunPropertiesRequestRequestTypeDef = TypedDict(
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
         "RunProperties": Mapping[str, str],
     },
@@ -3908,14 +4832,39 @@
         "TableLocation": str,
         "ConnectionName": str,
         "UpsertKeys": List[str],
     },
     total=False,
 )
 
+RegisterSchemaVersionResponseTypeDef = TypedDict(
+    "RegisterSchemaVersionResponseTypeDef",
+    {
+        "SchemaVersionId": str,
+        "VersionNumber": int,
+        "Status": SchemaVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RemoveSchemaVersionMetadataResponseTypeDef = TypedDict(
+    "RemoveSchemaVersionMetadataResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "SchemaName": str,
+        "RegistryName": str,
+        "LatestVersion": bool,
+        "VersionNumber": int,
+        "SchemaVersionId": str,
+        "MetadataKey": str,
+        "MetadataValue": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredResetJobBookmarkRequestRequestTypeDef = TypedDict(
     "_RequiredResetJobBookmarkRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 _OptionalResetJobBookmarkRequestRequestTypeDef = TypedDict(
@@ -3938,23 +4887,43 @@
     {
         "ResourceType": ResourceTypeType,
         "Uri": str,
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
 ResumeWorkflowRunRequestRequestTypeDef = TypedDict(
     "ResumeWorkflowRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
         "NodeIds": Sequence[str],
     },
 )
 
+ResumeWorkflowRunResponseTypeDef = TypedDict(
+    "ResumeWorkflowRunResponseTypeDef",
+    {
+        "RunId": str,
+        "NodeIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRunStatementRequestRequestTypeDef = TypedDict(
     "_RequiredRunStatementRequestRequestTypeDef",
     {
         "SessionId": str,
         "Code": str,
     },
 )
@@ -3969,14 +4938,22 @@
 
 class RunStatementRequestRequestTypeDef(
     _RequiredRunStatementRequestRequestTypeDef, _OptionalRunStatementRequestRequestTypeDef
 ):
     pass
 
 
+RunStatementResponseTypeDef = TypedDict(
+    "RunStatementResponseTypeDef",
+    {
+        "Id": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 S3DirectSourceAdditionalOptionsTypeDef = TypedDict(
     "S3DirectSourceAdditionalOptionsTypeDef",
     {
         "BoundedSize": int,
         "BoundedFiles": int,
         "EnableSamplePath": bool,
         "SamplePath": str,
@@ -4039,36 +5016,68 @@
 
 class StartBlueprintRunRequestRequestTypeDef(
     _RequiredStartBlueprintRunRequestRequestTypeDef, _OptionalStartBlueprintRunRequestRequestTypeDef
 ):
     pass
 
 
+StartBlueprintRunResponseTypeDef = TypedDict(
+    "StartBlueprintRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartCrawlerRequestRequestTypeDef = TypedDict(
     "StartCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 StartCrawlerScheduleRequestRequestTypeDef = TypedDict(
     "StartCrawlerScheduleRequestRequestTypeDef",
     {
         "CrawlerName": str,
     },
 )
 
+StartDataQualityRuleRecommendationRunResponseTypeDef = TypedDict(
+    "StartDataQualityRuleRecommendationRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartDataQualityRulesetEvaluationRunResponseTypeDef = TypedDict(
+    "StartDataQualityRulesetEvaluationRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartExportLabelsTaskRunRequestRequestTypeDef = TypedDict(
     "StartExportLabelsTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
         "OutputS3Path": str,
     },
 )
 
+StartExportLabelsTaskRunResponseTypeDef = TypedDict(
+    "StartExportLabelsTaskRunResponseTypeDef",
+    {
+        "TaskRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartImportLabelsTaskRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportLabelsTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
         "InputS3Path": str,
     },
 )
@@ -4084,36 +5093,76 @@
 class StartImportLabelsTaskRunRequestRequestTypeDef(
     _RequiredStartImportLabelsTaskRunRequestRequestTypeDef,
     _OptionalStartImportLabelsTaskRunRequestRequestTypeDef,
 ):
     pass
 
 
+StartImportLabelsTaskRunResponseTypeDef = TypedDict(
+    "StartImportLabelsTaskRunResponseTypeDef",
+    {
+        "TaskRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
+    {
+        "JobRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartMLEvaluationTaskRunRequestRequestTypeDef = TypedDict(
     "StartMLEvaluationTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
     },
 )
 
+StartMLEvaluationTaskRunResponseTypeDef = TypedDict(
+    "StartMLEvaluationTaskRunResponseTypeDef",
+    {
+        "TaskRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef = TypedDict(
     "StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
         "OutputS3Path": str,
     },
 )
 
+StartMLLabelingSetGenerationTaskRunResponseTypeDef = TypedDict(
+    "StartMLLabelingSetGenerationTaskRunResponseTypeDef",
+    {
+        "TaskRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartTriggerRequestRequestTypeDef = TypedDict(
     "StartTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+StartTriggerResponseTypeDef = TypedDict(
+    "StartTriggerResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartWorkflowRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartWorkflowRunRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalStartWorkflowRunRequestRequestTypeDef = TypedDict(
@@ -4127,14 +5176,22 @@
 
 class StartWorkflowRunRequestRequestTypeDef(
     _RequiredStartWorkflowRunRequestRequestTypeDef, _OptionalStartWorkflowRunRequestRequestTypeDef
 ):
     pass
 
 
+StartWorkflowRunResponseTypeDef = TypedDict(
+    "StartWorkflowRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartingEventBatchConditionTypeDef = TypedDict(
     "StartingEventBatchConditionTypeDef",
     {
         "BatchSize": int,
         "BatchWindow": int,
     },
     total=False,
@@ -4179,35 +5236,52 @@
 
 class StopSessionRequestRequestTypeDef(
     _RequiredStopSessionRequestRequestTypeDef, _OptionalStopSessionRequestRequestTypeDef
 ):
     pass
 
 
+StopSessionResponseTypeDef = TypedDict(
+    "StopSessionResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopTriggerRequestRequestTypeDef = TypedDict(
     "StopTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+StopTriggerResponseTypeDef = TypedDict(
+    "StopTriggerResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopWorkflowRunRequestRequestTypeDef = TypedDict(
     "StopWorkflowRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
 
 TableIdentifierTypeDef = TypedDict(
     "TableIdentifierTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
+        "Region": str,
     },
     total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
@@ -4242,14 +5316,22 @@
 
 class UpdateBlueprintRequestRequestTypeDef(
     _RequiredUpdateBlueprintRequestRequestTypeDef, _OptionalUpdateBlueprintRequestRequestTypeDef
 ):
     pass
 
 
+UpdateBlueprintResponseTypeDef = TypedDict(
+    "UpdateBlueprintResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCsvClassifierRequestTypeDef = TypedDict(
@@ -4358,14 +5440,47 @@
 class UpdateCrawlerScheduleRequestRequestTypeDef(
     _RequiredUpdateCrawlerScheduleRequestRequestTypeDef,
     _OptionalUpdateCrawlerScheduleRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDataQualityRulesetRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDataQualityRulesetRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Ruleset": str,
+    },
+    total=False,
+)
+
+
+class UpdateDataQualityRulesetRequestRequestTypeDef(
+    _RequiredUpdateDataQualityRulesetRequestRequestTypeDef,
+    _OptionalUpdateDataQualityRulesetRequestRequestTypeDef,
+):
+    pass
+
+
+UpdateDataQualityRulesetResponseTypeDef = TypedDict(
+    "UpdateDataQualityRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Ruleset": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateJobFromSourceControlRequestRequestTypeDef = TypedDict(
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     {
         "JobName": str,
         "Provider": SourceControlProviderType,
         "RepositoryName": str,
         "RepositoryOwner": str,
@@ -4374,14 +5489,57 @@
         "CommitId": str,
         "AuthStrategy": SourceControlAuthStrategyType,
         "AuthToken": str,
     },
     total=False,
 )
 
+UpdateJobFromSourceControlResponseTypeDef = TypedDict(
+    "UpdateJobFromSourceControlResponseTypeDef",
+    {
+        "JobName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateJobResponseTypeDef = TypedDict(
+    "UpdateJobResponseTypeDef",
+    {
+        "JobName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateMLTransformResponseTypeDef = TypedDict(
+    "UpdateMLTransformResponseTypeDef",
+    {
+        "TransformId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateRegistryResponseTypeDef = TypedDict(
+    "UpdateRegistryResponseTypeDef",
+    {
+        "RegistryName": str,
+        "RegistryArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSchemaResponseTypeDef = TypedDict(
+    "UpdateSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "SchemaName": str,
+        "RegistryName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateSourceControlFromJobRequestRequestTypeDef = TypedDict(
     "UpdateSourceControlFromJobRequestRequestTypeDef",
     {
         "JobName": str,
         "Provider": SourceControlProviderType,
         "RepositoryName": str,
         "RepositoryOwner": str,
@@ -4390,14 +5548,22 @@
         "CommitId": str,
         "AuthStrategy": SourceControlAuthStrategyType,
         "AuthToken": str,
     },
     total=False,
 )
 
+UpdateSourceControlFromJobResponseTypeDef = TypedDict(
+    "UpdateSourceControlFromJobResponseTypeDef",
+    {
+        "JobName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateWorkflowRequestRequestTypeDef = TypedDict(
@@ -4413,14 +5579,22 @@
 
 class UpdateWorkflowRequestRequestTypeDef(
     _RequiredUpdateWorkflowRequestRequestTypeDef, _OptionalUpdateWorkflowRequestRequestTypeDef
 ):
     pass
 
 
+UpdateWorkflowResponseTypeDef = TypedDict(
+    "UpdateWorkflowResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WorkflowRunStatisticsTypeDef = TypedDict(
     "WorkflowRunStatisticsTypeDef",
     {
         "TotalActions": int,
         "TimeoutActions": int,
         "FailedActions": int,
         "StoppedActions": int,
@@ -4481,14 +5655,47 @@
         "Name": str,
         "Inputs": List[str],
         "Groups": List[List[str]],
         "Aggs": List[AggregateOperationTypeDef],
     },
 )
 
+AmazonRedshiftNodeDataTypeDef = TypedDict(
+    "AmazonRedshiftNodeDataTypeDef",
+    {
+        "AccessType": str,
+        "SourceType": str,
+        "Connection": OptionTypeDef,
+        "Schema": OptionTypeDef,
+        "Table": OptionTypeDef,
+        "CatalogDatabase": OptionTypeDef,
+        "CatalogTable": OptionTypeDef,
+        "CatalogRedshiftSchema": str,
+        "CatalogRedshiftTable": str,
+        "TempDir": str,
+        "IamRole": OptionTypeDef,
+        "AdvancedOptions": List[AmazonRedshiftAdvancedOptionTypeDef],
+        "SampleQuery": str,
+        "PreAction": str,
+        "PostAction": str,
+        "Action": str,
+        "TablePrefix": str,
+        "Upsert": bool,
+        "MergeAction": str,
+        "MergeWhenMatched": str,
+        "MergeWhenNotMatched": str,
+        "MergeClause": str,
+        "CrawlerConnection": str,
+        "TableSchema": List[OptionTypeDef],
+        "StagingTable": str,
+        "SelectedColumns": List[OptionTypeDef],
+    },
+    total=False,
+)
+
 _RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
@@ -4588,627 +5795,20 @@
 
 class BatchGetPartitionRequestRequestTypeDef(
     _RequiredBatchGetPartitionRequestRequestTypeDef, _OptionalBatchGetPartitionRequestRequestTypeDef
 ):
     pass
 
 
-CancelMLTaskRunResponseTypeDef = TypedDict(
-    "CancelMLTaskRunResponseTypeDef",
-    {
-        "TransformId": str,
-        "TaskRunId": str,
-        "Status": TaskStatusTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CheckSchemaVersionValidityResponseTypeDef = TypedDict(
-    "CheckSchemaVersionValidityResponseTypeDef",
-    {
-        "Valid": bool,
-        "Error": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBlueprintResponseTypeDef = TypedDict(
-    "CreateBlueprintResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCustomEntityTypeResponseTypeDef = TypedDict(
-    "CreateCustomEntityTypeResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDevEndpointResponseTypeDef = TypedDict(
-    "CreateDevEndpointResponseTypeDef",
-    {
-        "EndpointName": str,
-        "Status": str,
-        "SecurityGroupIds": List[str],
-        "SubnetId": str,
-        "RoleArn": str,
-        "YarnEndpointAddress": str,
-        "ZeppelinRemoteSparkInterpreterPort": int,
-        "NumberOfNodes": int,
-        "WorkerType": WorkerTypeType,
-        "GlueVersion": str,
-        "NumberOfWorkers": int,
-        "AvailabilityZone": str,
-        "VpcId": str,
-        "ExtraPythonLibsS3Path": str,
-        "ExtraJarsS3Path": str,
-        "FailureReason": str,
-        "SecurityConfiguration": str,
-        "CreatedTimestamp": datetime,
-        "Arguments": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobResponseTypeDef = TypedDict(
-    "CreateJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMLTransformResponseTypeDef = TypedDict(
-    "CreateMLTransformResponseTypeDef",
-    {
-        "TransformId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRegistryResponseTypeDef = TypedDict(
-    "CreateRegistryResponseTypeDef",
-    {
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "RegistryName": str,
-        "RegistryArn": str,
-        "SchemaName": str,
-        "SchemaArn": str,
-        "Description": str,
-        "DataFormat": DataFormatType,
-        "Compatibility": CompatibilityType,
-        "SchemaCheckpoint": int,
-        "LatestSchemaVersion": int,
-        "NextSchemaVersion": int,
-        "SchemaStatus": SchemaStatusType,
-        "Tags": Dict[str, str],
-        "SchemaVersionId": str,
-        "SchemaVersionStatus": SchemaVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateScriptResponseTypeDef = TypedDict(
-    "CreateScriptResponseTypeDef",
-    {
-        "PythonScript": str,
-        "ScalaCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSecurityConfigurationResponseTypeDef = TypedDict(
-    "CreateSecurityConfigurationResponseTypeDef",
-    {
-        "Name": str,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTriggerResponseTypeDef = TypedDict(
-    "CreateTriggerResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkflowResponseTypeDef = TypedDict(
-    "CreateWorkflowResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBlueprintResponseTypeDef = TypedDict(
-    "DeleteBlueprintResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteCustomEntityTypeResponseTypeDef = TypedDict(
-    "DeleteCustomEntityTypeResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteJobResponseTypeDef = TypedDict(
-    "DeleteJobResponseTypeDef",
-    {
-        "JobName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteMLTransformResponseTypeDef = TypedDict(
-    "DeleteMLTransformResponseTypeDef",
-    {
-        "TransformId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteRegistryResponseTypeDef = TypedDict(
-    "DeleteRegistryResponseTypeDef",
-    {
-        "RegistryName": str,
-        "RegistryArn": str,
-        "Status": RegistryStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSchemaResponseTypeDef = TypedDict(
-    "DeleteSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "SchemaName": str,
-        "Status": SchemaStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSessionResponseTypeDef = TypedDict(
-    "DeleteSessionResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteTriggerResponseTypeDef = TypedDict(
-    "DeleteTriggerResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteWorkflowResponseTypeDef = TypedDict(
-    "DeleteWorkflowResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCustomEntityTypeResponseTypeDef = TypedDict(
-    "GetCustomEntityTypeResponseTypeDef",
-    {
-        "Name": str,
-        "RegexString": str,
-        "ContextWords": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPlanResponseTypeDef = TypedDict(
-    "GetPlanResponseTypeDef",
-    {
-        "PythonScript": str,
-        "ScalaCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRegistryResponseTypeDef = TypedDict(
-    "GetRegistryResponseTypeDef",
-    {
-        "RegistryName": str,
-        "RegistryArn": str,
-        "Description": str,
-        "Status": RegistryStatusType,
-        "CreatedTime": str,
-        "UpdatedTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "PolicyInJson": str,
-        "PolicyHash": str,
-        "CreateTime": datetime,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSchemaByDefinitionResponseTypeDef = TypedDict(
-    "GetSchemaByDefinitionResponseTypeDef",
-    {
-        "SchemaVersionId": str,
-        "SchemaArn": str,
-        "DataFormat": DataFormatType,
-        "Status": SchemaVersionStatusType,
-        "CreatedTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSchemaResponseTypeDef = TypedDict(
-    "GetSchemaResponseTypeDef",
-    {
-        "RegistryName": str,
-        "RegistryArn": str,
-        "SchemaName": str,
-        "SchemaArn": str,
-        "Description": str,
-        "DataFormat": DataFormatType,
-        "Compatibility": CompatibilityType,
-        "SchemaCheckpoint": int,
-        "LatestSchemaVersion": int,
-        "NextSchemaVersion": int,
-        "SchemaStatus": SchemaStatusType,
-        "CreatedTime": str,
-        "UpdatedTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSchemaVersionResponseTypeDef = TypedDict(
-    "GetSchemaVersionResponseTypeDef",
-    {
-        "SchemaVersionId": str,
-        "SchemaDefinition": str,
-        "DataFormat": DataFormatType,
-        "SchemaArn": str,
-        "VersionNumber": int,
-        "Status": SchemaVersionStatusType,
-        "CreatedTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSchemaVersionsDiffResponseTypeDef = TypedDict(
-    "GetSchemaVersionsDiffResponseTypeDef",
-    {
-        "Diff": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetWorkflowRunPropertiesResponseTypeDef = TypedDict(
-    "GetWorkflowRunPropertiesResponseTypeDef",
-    {
-        "RunProperties": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBlueprintsResponseTypeDef = TypedDict(
-    "ListBlueprintsResponseTypeDef",
-    {
-        "Blueprints": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCrawlersResponseTypeDef = TypedDict(
-    "ListCrawlersResponseTypeDef",
-    {
-        "CrawlerNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDevEndpointsResponseTypeDef = TypedDict(
-    "ListDevEndpointsResponseTypeDef",
-    {
-        "DevEndpointNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListJobsResponseTypeDef = TypedDict(
-    "ListJobsResponseTypeDef",
-    {
-        "JobNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListMLTransformsResponseTypeDef = TypedDict(
-    "ListMLTransformsResponseTypeDef",
-    {
-        "TransformIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTriggersResponseTypeDef = TypedDict(
-    "ListTriggersResponseTypeDef",
-    {
-        "TriggerNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListWorkflowsResponseTypeDef = TypedDict(
-    "ListWorkflowsResponseTypeDef",
-    {
-        "Workflows": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "PolicyHash": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutSchemaVersionMetadataResponseTypeDef = TypedDict(
-    "PutSchemaVersionMetadataResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "SchemaName": str,
-        "RegistryName": str,
-        "LatestVersion": bool,
-        "VersionNumber": int,
-        "SchemaVersionId": str,
-        "MetadataKey": str,
-        "MetadataValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterSchemaVersionResponseTypeDef = TypedDict(
-    "RegisterSchemaVersionResponseTypeDef",
-    {
-        "SchemaVersionId": str,
-        "VersionNumber": int,
-        "Status": SchemaVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveSchemaVersionMetadataResponseTypeDef = TypedDict(
-    "RemoveSchemaVersionMetadataResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "SchemaName": str,
-        "RegistryName": str,
-        "LatestVersion": bool,
-        "VersionNumber": int,
-        "SchemaVersionId": str,
-        "MetadataKey": str,
-        "MetadataValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ResumeWorkflowRunResponseTypeDef = TypedDict(
-    "ResumeWorkflowRunResponseTypeDef",
-    {
-        "RunId": str,
-        "NodeIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RunStatementResponseTypeDef = TypedDict(
-    "RunStatementResponseTypeDef",
-    {
-        "Id": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartBlueprintRunResponseTypeDef = TypedDict(
-    "StartBlueprintRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartExportLabelsTaskRunResponseTypeDef = TypedDict(
-    "StartExportLabelsTaskRunResponseTypeDef",
-    {
-        "TaskRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartImportLabelsTaskRunResponseTypeDef = TypedDict(
-    "StartImportLabelsTaskRunResponseTypeDef",
-    {
-        "TaskRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
-    {
-        "JobRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartMLEvaluationTaskRunResponseTypeDef = TypedDict(
-    "StartMLEvaluationTaskRunResponseTypeDef",
-    {
-        "TaskRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartMLLabelingSetGenerationTaskRunResponseTypeDef = TypedDict(
-    "StartMLLabelingSetGenerationTaskRunResponseTypeDef",
-    {
-        "TaskRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartTriggerResponseTypeDef = TypedDict(
-    "StartTriggerResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartWorkflowRunResponseTypeDef = TypedDict(
-    "StartWorkflowRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopSessionResponseTypeDef = TypedDict(
-    "StopSessionResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopTriggerResponseTypeDef = TypedDict(
-    "StopTriggerResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateBlueprintResponseTypeDef = TypedDict(
-    "UpdateBlueprintResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateJobFromSourceControlResponseTypeDef = TypedDict(
-    "UpdateJobFromSourceControlResponseTypeDef",
-    {
-        "JobName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateJobResponseTypeDef = TypedDict(
-    "UpdateJobResponseTypeDef",
-    {
-        "JobName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMLTransformResponseTypeDef = TypedDict(
-    "UpdateMLTransformResponseTypeDef",
-    {
-        "TransformId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateRegistryResponseTypeDef = TypedDict(
-    "UpdateRegistryResponseTypeDef",
-    {
-        "RegistryName": str,
-        "RegistryArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSchemaResponseTypeDef = TypedDict(
-    "UpdateSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "SchemaName": str,
-        "RegistryName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSourceControlFromJobResponseTypeDef = TypedDict(
-    "UpdateSourceControlFromJobResponseTypeDef",
-    {
-        "JobName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateWorkflowResponseTypeDef = TypedDict(
-    "UpdateWorkflowResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchDeleteConnectionResponseTypeDef = TypedDict(
     "BatchDeleteConnectionResponseTypeDef",
     {
         "Succeeded": List[str],
         "Errors": Dict[str, ErrorDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchStopJobRunErrorTypeDef = TypedDict(
     "BatchStopJobRunErrorTypeDef",
     {
         "JobName": str,
@@ -5265,67 +5865,67 @@
 )
 
 BatchGetCustomEntityTypesResponseTypeDef = TypedDict(
     "BatchGetCustomEntityTypesResponseTypeDef",
     {
         "CustomEntityTypes": List[CustomEntityTypeTypeDef],
         "CustomEntityTypesNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomEntityTypesResponseTypeDef = TypedDict(
     "ListCustomEntityTypesResponseTypeDef",
     {
         "CustomEntityTypes": List[CustomEntityTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetDevEndpointsResponseTypeDef = TypedDict(
     "BatchGetDevEndpointsResponseTypeDef",
     {
         "DevEndpoints": List[DevEndpointTypeDef],
         "DevEndpointsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDevEndpointResponseTypeDef = TypedDict(
     "GetDevEndpointResponseTypeDef",
     {
         "DevEndpoint": DevEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDevEndpointsResponseTypeDef = TypedDict(
     "GetDevEndpointsResponseTypeDef",
     {
         "DevEndpoints": List[DevEndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBlueprintRunResponseTypeDef = TypedDict(
     "GetBlueprintRunResponseTypeDef",
     {
         "BlueprintRun": BlueprintRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBlueprintRunsResponseTypeDef = TypedDict(
     "GetBlueprintRunsResponseTypeDef",
     {
         "BlueprintRuns": List[BlueprintRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BlueprintTypeDef = TypedDict(
     "BlueprintTypeDef",
     {
         "Name": str,
@@ -5342,15 +5942,15 @@
     total=False,
 )
 
 GetCatalogImportStatusResponseTypeDef = TypedDict(
     "GetCatalogImportStatusResponseTypeDef",
     {
         "ImportStatus": CatalogImportStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCatalogKafkaSourceTypeDef = TypedDict(
     "_RequiredCatalogKafkaSourceTypeDef",
     {
         "Name": str,
@@ -5494,14 +6094,66 @@
 )
 
 
 class S3CatalogTargetTypeDef(_RequiredS3CatalogTargetTypeDef, _OptionalS3CatalogTargetTypeDef):
     pass
 
 
+_RequiredS3DeltaCatalogTargetTypeDef = TypedDict(
+    "_RequiredS3DeltaCatalogTargetTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Table": str,
+        "Database": str,
+    },
+)
+_OptionalS3DeltaCatalogTargetTypeDef = TypedDict(
+    "_OptionalS3DeltaCatalogTargetTypeDef",
+    {
+        "PartitionKeys": List[List[str]],
+        "AdditionalOptions": Dict[str, str],
+        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
+    },
+    total=False,
+)
+
+
+class S3DeltaCatalogTargetTypeDef(
+    _RequiredS3DeltaCatalogTargetTypeDef, _OptionalS3DeltaCatalogTargetTypeDef
+):
+    pass
+
+
+_RequiredS3HudiCatalogTargetTypeDef = TypedDict(
+    "_RequiredS3HudiCatalogTargetTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Table": str,
+        "Database": str,
+        "AdditionalOptions": Dict[str, str],
+    },
+)
+_OptionalS3HudiCatalogTargetTypeDef = TypedDict(
+    "_OptionalS3HudiCatalogTargetTypeDef",
+    {
+        "PartitionKeys": List[List[str]],
+        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
+    },
+    total=False,
+)
+
+
+class S3HudiCatalogTargetTypeDef(
+    _RequiredS3HudiCatalogTargetTypeDef, _OptionalS3HudiCatalogTargetTypeDef
+):
+    pass
+
+
 ClassifierTypeDef = TypedDict(
     "ClassifierTypeDef",
     {
         "GrokClassifier": GrokClassifierTypeDef,
         "XMLClassifier": XMLClassifierTypeDef,
         "JsonClassifier": JsonClassifierTypeDef,
         "CsvClassifier": CsvClassifierTypeDef,
@@ -5610,36 +6262,37 @@
 )
 
 ListCrawlsResponseTypeDef = TypedDict(
     "ListCrawlsResponseTypeDef",
     {
         "Crawls": List[CrawlerHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCrawlerMetricsResponseTypeDef = TypedDict(
     "GetCrawlerMetricsResponseTypeDef",
     {
         "CrawlerMetricsList": List[CrawlerMetricsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CrawlerTargetsTypeDef = TypedDict(
     "CrawlerTargetsTypeDef",
     {
         "S3Targets": List[S3TargetTypeDef],
         "JdbcTargets": List[JdbcTargetTypeDef],
         "MongoDBTargets": List[MongoDBTargetTypeDef],
         "DynamoDBTargets": List[DynamoDBTargetTypeDef],
         "CatalogTargets": List[CatalogTargetTypeDef],
         "DeltaTargets": List[DeltaTargetTypeDef],
+        "IcebergTargets": List[IcebergTargetTypeDef],
     },
     total=False,
 )
 
 _RequiredListCrawlsRequestRequestTypeDef = TypedDict(
     "_RequiredListCrawlsRequestRequestTypeDef",
     {
@@ -5670,14 +6323,89 @@
         "XMLClassifier": CreateXMLClassifierRequestTypeDef,
         "JsonClassifier": CreateJsonClassifierRequestTypeDef,
         "CsvClassifier": CreateCsvClassifierRequestTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateDataQualityRulesetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataQualityRulesetRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Ruleset": str,
+    },
+)
+_OptionalCreateDataQualityRulesetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataQualityRulesetRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Mapping[str, str],
+        "TargetTable": DataQualityTargetTableTypeDef,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateDataQualityRulesetRequestRequestTypeDef(
+    _RequiredCreateDataQualityRulesetRequestRequestTypeDef,
+    _OptionalCreateDataQualityRulesetRequestRequestTypeDef,
+):
+    pass
+
+
+DataQualityRulesetFilterCriteriaTypeDef = TypedDict(
+    "DataQualityRulesetFilterCriteriaTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "CreatedBefore": Union[datetime, str],
+        "CreatedAfter": Union[datetime, str],
+        "LastModifiedBefore": Union[datetime, str],
+        "LastModifiedAfter": Union[datetime, str],
+        "TargetTable": DataQualityTargetTableTypeDef,
+    },
+    total=False,
+)
+
+DataQualityRulesetListDetailsTypeDef = TypedDict(
+    "DataQualityRulesetListDetailsTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "CreatedOn": datetime,
+        "LastModifiedOn": datetime,
+        "TargetTable": DataQualityTargetTableTypeDef,
+        "RecommendationRunId": str,
+        "RuleCount": int,
+    },
+    total=False,
+)
+
+GetDataQualityRulesetResponseTypeDef = TypedDict(
+    "GetDataQualityRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Ruleset": str,
+        "TargetTable": DataQualityTargetTableTypeDef,
+        "CreatedOn": datetime,
+        "LastModifiedOn": datetime,
+        "RecommendationRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DataSourceTypeDef = TypedDict(
+    "DataSourceTypeDef",
+    {
+        "GlueTable": GlueTableTypeDef,
+    },
+)
+
 _RequiredCreatePartitionIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePartitionIndexRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionIndex": PartitionIndexTypeDef,
     },
@@ -5734,14 +6462,23 @@
 GetRegistryInputRequestTypeDef = TypedDict(
     "GetRegistryInputRequestTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
     },
 )
 
+ListSchemasInputListSchemasPaginateTypeDef = TypedDict(
+    "ListSchemasInputListSchemasPaginateTypeDef",
+    {
+        "RegistryId": RegistryIdTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSchemasInputRequestTypeDef = TypedDict(
     "ListSchemasInputRequestTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -5806,14 +6543,65 @@
         "MaxCapacity": float,
         "SecurityConfiguration": str,
         "GlueVersion": str,
     },
     total=False,
 )
 
+_RequiredEvaluateDataQualityMultiFrameTypeDef = TypedDict(
+    "_RequiredEvaluateDataQualityMultiFrameTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Ruleset": str,
+    },
+)
+_OptionalEvaluateDataQualityMultiFrameTypeDef = TypedDict(
+    "_OptionalEvaluateDataQualityMultiFrameTypeDef",
+    {
+        "AdditionalDataSources": Dict[str, str],
+        "PublishingOptions": DQResultsPublishingOptionsTypeDef,
+        "AdditionalOptions": Dict[Literal["performanceTuning.caching"], str],
+        "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
+    },
+    total=False,
+)
+
+
+class EvaluateDataQualityMultiFrameTypeDef(
+    _RequiredEvaluateDataQualityMultiFrameTypeDef, _OptionalEvaluateDataQualityMultiFrameTypeDef
+):
+    pass
+
+
+_RequiredEvaluateDataQualityTypeDef = TypedDict(
+    "_RequiredEvaluateDataQualityTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Ruleset": str,
+    },
+)
+_OptionalEvaluateDataQualityTypeDef = TypedDict(
+    "_OptionalEvaluateDataQualityTypeDef",
+    {
+        "Output": DQTransformOutputType,
+        "PublishingOptions": DQResultsPublishingOptionsTypeDef,
+        "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
+    },
+    total=False,
+)
+
+
+class EvaluateDataQualityTypeDef(
+    _RequiredEvaluateDataQualityTypeDef, _OptionalEvaluateDataQualityTypeDef
+):
+    pass
+
+
 DataCatalogEncryptionSettingsTypeDef = TypedDict(
     "DataCatalogEncryptionSettingsTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "ConnectionPasswordEncryption": ConnectionPasswordEncryptionTypeDef,
     },
     total=False,
@@ -5885,14 +6673,36 @@
 GetSchemaInputRequestTypeDef = TypedDict(
     "GetSchemaInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
     },
 )
 
+_RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
+    {
+        "SchemaId": SchemaIdTypeDef,
+    },
+)
+_OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef(
+    _RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
+    _OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListSchemaVersionsInputRequestTypeDef = TypedDict(
     "_RequiredListSchemaVersionsInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
     },
 )
 _OptionalListSchemaVersionsInputRequestTypeDef = TypedDict(
@@ -5952,14 +6762,41 @@
 
 class UpdateDevEndpointRequestRequestTypeDef(
     _RequiredUpdateDevEndpointRequestRequestTypeDef, _OptionalUpdateDevEndpointRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredS3DeltaDirectTargetTypeDef = TypedDict(
+    "_RequiredS3DeltaDirectTargetTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Path": str,
+        "Compression": DeltaTargetCompressionTypeType,
+        "Format": TargetFormatType,
+    },
+)
+_OptionalS3DeltaDirectTargetTypeDef = TypedDict(
+    "_OptionalS3DeltaDirectTargetTypeDef",
+    {
+        "PartitionKeys": List[List[str]],
+        "AdditionalOptions": Dict[str, str],
+        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
+    },
+    total=False,
+)
+
+
+class S3DeltaDirectTargetTypeDef(
+    _RequiredS3DeltaDirectTargetTypeDef, _OptionalS3DeltaDirectTargetTypeDef
+):
+    pass
+
+
 _RequiredS3DirectTargetTypeDef = TypedDict(
     "_RequiredS3DirectTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Path": str,
         "Format": TargetFormatType,
@@ -6001,14 +6838,41 @@
 
 class S3GlueParquetTargetTypeDef(
     _RequiredS3GlueParquetTargetTypeDef, _OptionalS3GlueParquetTargetTypeDef
 ):
     pass
 
 
+_RequiredS3HudiDirectTargetTypeDef = TypedDict(
+    "_RequiredS3HudiDirectTargetTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Path": str,
+        "Compression": HudiTargetCompressionTypeType,
+        "Format": TargetFormatType,
+        "AdditionalOptions": Dict[str, str],
+    },
+)
+_OptionalS3HudiDirectTargetTypeDef = TypedDict(
+    "_OptionalS3HudiDirectTargetTypeDef",
+    {
+        "PartitionKeys": List[List[str]],
+        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
+    },
+    total=False,
+)
+
+
+class S3HudiDirectTargetTypeDef(
+    _RequiredS3HudiDirectTargetTypeDef, _OptionalS3HudiDirectTargetTypeDef
+):
+    pass
+
+
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "S3Encryption": Sequence[S3EncryptionTypeDef],
         "CloudWatchEncryption": CloudWatchEncryptionTypeDef,
         "JobBookmarksEncryption": JobBookmarksEncryptionTypeDef,
     },
@@ -6061,256 +6925,21 @@
 
 class TransformParametersTypeDef(
     _RequiredTransformParametersTypeDef, _OptionalTransformParametersTypeDef
 ):
     pass
 
 
-GetClassifiersRequestGetClassifiersPaginateTypeDef = TypedDict(
-    "GetClassifiersRequestGetClassifiersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef = TypedDict(
-    "GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef",
-    {
-        "CrawlerNameList": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetCrawlersRequestGetCrawlersPaginateTypeDef = TypedDict(
-    "GetCrawlersRequestGetCrawlersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetDatabasesRequestGetDatabasesPaginateTypeDef = TypedDict(
-    "GetDatabasesRequestGetDatabasesPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "ResourceShareType": ResourceShareTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef = TypedDict(
-    "GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef",
-    {
-        "JobName": str,
-    },
-)
-_OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetJobRunsRequestGetJobRunsPaginateTypeDef(
-    _RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef,
-    _OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef,
-):
-    pass
-
-
-GetJobsRequestGetJobsPaginateTypeDef = TypedDict(
-    "GetJobsRequestGetJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef = TypedDict(
-    "_RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-    },
-)
-_OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef = TypedDict(
-    "_OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef(
-    _RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
-    _OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
-):
-    pass
-
-
-GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef = TypedDict(
-    "GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-    },
-)
-_OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetTableVersionsRequestGetTableVersionsPaginateTypeDef(
-    _RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
-    _OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
-    "_RequiredGetTablesRequestGetTablesPaginateTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
-    "_OptionalGetTablesRequestGetTablesPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "Expression": str,
-        "TransactionId": str,
-        "QueryAsOfTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetTablesRequestGetTablesPaginateTypeDef(
-    _RequiredGetTablesRequestGetTablesPaginateTypeDef,
-    _OptionalGetTablesRequestGetTablesPaginateTypeDef,
-):
-    pass
-
-
-GetTriggersRequestGetTriggersPaginateTypeDef = TypedDict(
-    "GetTriggersRequestGetTriggersPaginateTypeDef",
-    {
-        "DependentJobName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef = TypedDict(
-    "_RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef",
-    {
-        "Pattern": str,
-    },
-)
-_OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef = TypedDict(
-    "_OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "DatabaseName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef(
-    _RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
-    _OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
-):
-    pass
-
-
-ListRegistriesInputListRegistriesPaginateTypeDef = TypedDict(
-    "ListRegistriesInputListRegistriesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
-    {
-        "SchemaId": SchemaIdTypeDef,
-    },
-)
-_OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef(
-    _RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
-    _OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListSchemasInputListSchemasPaginateTypeDef = TypedDict(
-    "ListSchemasInputListSchemasPaginateTypeDef",
-    {
-        "RegistryId": RegistryIdTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 GetConnectionsRequestGetConnectionsPaginateTypeDef = TypedDict(
     "GetConnectionsRequestGetConnectionsPaginateTypeDef",
     {
         "CatalogId": str,
         "Filter": GetConnectionsFilterTypeDef,
         "HidePassword": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetConnectionsRequestRequestTypeDef = TypedDict(
     "GetConnectionsRequestRequestTypeDef",
     {
@@ -6323,23 +6952,23 @@
     total=False,
 )
 
 GetJobBookmarkResponseTypeDef = TypedDict(
     "GetJobBookmarkResponseTypeDef",
     {
         "JobBookmarkEntry": JobBookmarkEntryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResetJobBookmarkResponseTypeDef = TypedDict(
     "ResetJobBookmarkResponseTypeDef",
     {
         "JobBookmarkEntry": JobBookmarkEntryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetMLTaskRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetMLTaskRunsRequestRequestTypeDef",
     {
         "TransformId": str,
@@ -6379,15 +7008,15 @@
     total=False,
 )
 
 GetMappingResponseTypeDef = TypedDict(
     "GetMappingResponseTypeDef",
     {
         "Mapping": List[MappingEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef = TypedDict(
     "_RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef",
     {
         "DatabaseName": str,
@@ -6399,15 +7028,15 @@
     {
         "CatalogId": str,
         "Expression": str,
         "Segment": SegmentTypeDef,
         "ExcludeColumnSchema": bool,
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class GetPartitionsRequestGetPartitionsPaginateTypeDef(
     _RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef,
@@ -6475,15 +7104,15 @@
 
 
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "GetResourcePoliciesResponseList": List[GluePolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSchemaVersionInputRequestTypeDef = TypedDict(
     "GetSchemaVersionInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
@@ -6634,33 +7263,33 @@
 )
 
 ListRegistriesResponseTypeDef = TypedDict(
     "ListRegistriesResponseTypeDef",
     {
         "Registries": List[RegistryListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSchemaVersionsResponseTypeDef = TypedDict(
     "ListSchemaVersionsResponseTypeDef",
     {
         "Schemas": List[SchemaVersionListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSchemasResponseTypeDef = TypedDict(
     "ListSchemasResponseTypeDef",
     {
         "Schemas": List[SchemaListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TransformEncryptionTypeDef = TypedDict(
     "TransformEncryptionTypeDef",
     {
         "MlUserDataEncryption": MLUserDataEncryptionTypeDef,
@@ -6825,14 +7454,33 @@
         "XMLClassifier": UpdateXMLClassifierRequestTypeDef,
         "JsonClassifier": UpdateJsonClassifierRequestTypeDef,
         "CsvClassifier": UpdateCsvClassifierRequestTypeDef,
     },
     total=False,
 )
 
+AmazonRedshiftSourceTypeDef = TypedDict(
+    "AmazonRedshiftSourceTypeDef",
+    {
+        "Name": str,
+        "Data": AmazonRedshiftNodeDataTypeDef,
+    },
+    total=False,
+)
+
+AmazonRedshiftTargetTypeDef = TypedDict(
+    "AmazonRedshiftTargetTypeDef",
+    {
+        "Name": str,
+        "Data": AmazonRedshiftNodeDataTypeDef,
+        "Inputs": List[str],
+    },
+    total=False,
+)
+
 _RequiredPartitionIndexDescriptorTypeDef = TypedDict(
     "_RequiredPartitionIndexDescriptorTypeDef",
     {
         "IndexName": str,
         "Keys": List[KeySchemaElementTypeDef],
         "IndexStatus": PartitionIndexStatusType,
     },
@@ -6853,89 +7501,89 @@
 
 
 BatchStopJobRunResponseTypeDef = TypedDict(
     "BatchStopJobRunResponseTypeDef",
     {
         "SuccessfulSubmissions": List[BatchStopJobRunSuccessfulSubmissionTypeDef],
         "Errors": List[BatchStopJobRunErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdatePartitionResponseTypeDef = TypedDict(
     "BatchUpdatePartitionResponseTypeDef",
     {
         "Errors": List[BatchUpdatePartitionFailureEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchCreatePartitionResponseTypeDef = TypedDict(
     "BatchCreatePartitionResponseTypeDef",
     {
         "Errors": List[PartitionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeletePartitionResponseTypeDef = TypedDict(
     "BatchDeletePartitionResponseTypeDef",
     {
         "Errors": List[PartitionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteTableResponseTypeDef = TypedDict(
     "BatchDeleteTableResponseTypeDef",
     {
         "Errors": List[TableErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteTableVersionResponseTypeDef = TypedDict(
     "BatchDeleteTableVersionResponseTypeDef",
     {
         "Errors": List[TableVersionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetBlueprintsResponseTypeDef = TypedDict(
     "BatchGetBlueprintsResponseTypeDef",
     {
         "Blueprints": List[BlueprintTypeDef],
         "MissingBlueprints": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBlueprintResponseTypeDef = TypedDict(
     "GetBlueprintResponseTypeDef",
     {
         "Blueprint": BlueprintTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetClassifierResponseTypeDef = TypedDict(
     "GetClassifierResponseTypeDef",
     {
         "Classifier": ClassifierTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetClassifiersResponseTypeDef = TypedDict(
     "GetClassifiersResponseTypeDef",
     {
         "Classifiers": List[ClassifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateScriptRequestRequestTypeDef = TypedDict(
     "CreateScriptRequestRequestTypeDef",
     {
         "DagNodes": Sequence[CodeGenNodeTypeDef],
@@ -6946,15 +7594,15 @@
 )
 
 GetDataflowGraphResponseTypeDef = TypedDict(
     "GetDataflowGraphResponseTypeDef",
     {
         "DagNodes": List[CodeGenNodeTypeDef],
         "DagEdges": List[CodeGenEdgeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetMappingRequestRequestTypeDef = TypedDict(
     "_RequiredGetMappingRequestRequestTypeDef",
     {
         "Source": CatalogEntryTypeDef,
@@ -7125,24 +7773,24 @@
     pass
 
 
 GetConnectionResponseTypeDef = TypedDict(
     "GetConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConnectionsResponseTypeDef = TypedDict(
     "GetConnectionsResponseTypeDef",
     {
         "ConnectionList": List[ConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CrawlerTypeDef = TypedDict(
     "CrawlerTypeDef",
     {
         "Name": str,
@@ -7232,45 +7880,289 @@
 
 class UpdateCrawlerRequestRequestTypeDef(
     _RequiredUpdateCrawlerRequestRequestTypeDef, _OptionalUpdateCrawlerRequestRequestTypeDef
 ):
     pass
 
 
+ListDataQualityRulesetsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRulesetsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "Filter": DataQualityRulesetFilterCriteriaTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+ListDataQualityRulesetsResponseTypeDef = TypedDict(
+    "ListDataQualityRulesetsResponseTypeDef",
+    {
+        "Rulesets": List[DataQualityRulesetListDetailsTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DataQualityResultDescriptionTypeDef = TypedDict(
+    "DataQualityResultDescriptionTypeDef",
+    {
+        "ResultId": str,
+        "DataSource": DataSourceTypeDef,
+        "JobName": str,
+        "JobRunId": str,
+        "StartedOn": datetime,
+    },
+    total=False,
+)
+
+DataQualityResultFilterCriteriaTypeDef = TypedDict(
+    "DataQualityResultFilterCriteriaTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+        "JobName": str,
+        "JobRunId": str,
+        "StartedAfter": Union[datetime, str],
+        "StartedBefore": Union[datetime, str],
+    },
+    total=False,
+)
+
+DataQualityResultTypeDef = TypedDict(
+    "DataQualityResultTypeDef",
+    {
+        "ResultId": str,
+        "Score": float,
+        "DataSource": DataSourceTypeDef,
+        "RulesetName": str,
+        "EvaluationContext": str,
+        "StartedOn": datetime,
+        "CompletedOn": datetime,
+        "JobName": str,
+        "JobRunId": str,
+        "RulesetEvaluationRunId": str,
+        "RuleResults": List[DataQualityRuleResultTypeDef],
+    },
+    total=False,
+)
+
+DataQualityRuleRecommendationRunDescriptionTypeDef = TypedDict(
+    "DataQualityRuleRecommendationRunDescriptionTypeDef",
+    {
+        "RunId": str,
+        "Status": TaskStatusTypeType,
+        "StartedOn": datetime,
+        "DataSource": DataSourceTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
+    "_RequiredDataQualityRuleRecommendationRunFilterTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+    },
+)
+_OptionalDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
+    "_OptionalDataQualityRuleRecommendationRunFilterTypeDef",
+    {
+        "StartedBefore": Union[datetime, str],
+        "StartedAfter": Union[datetime, str],
+    },
+    total=False,
+)
+
+
+class DataQualityRuleRecommendationRunFilterTypeDef(
+    _RequiredDataQualityRuleRecommendationRunFilterTypeDef,
+    _OptionalDataQualityRuleRecommendationRunFilterTypeDef,
+):
+    pass
+
+
+DataQualityRulesetEvaluationRunDescriptionTypeDef = TypedDict(
+    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
+    {
+        "RunId": str,
+        "Status": TaskStatusTypeType,
+        "StartedOn": datetime,
+        "DataSource": DataSourceTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
+    "_RequiredDataQualityRulesetEvaluationRunFilterTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+    },
+)
+_OptionalDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
+    "_OptionalDataQualityRulesetEvaluationRunFilterTypeDef",
+    {
+        "StartedBefore": Union[datetime, str],
+        "StartedAfter": Union[datetime, str],
+    },
+    total=False,
+)
+
+
+class DataQualityRulesetEvaluationRunFilterTypeDef(
+    _RequiredDataQualityRulesetEvaluationRunFilterTypeDef,
+    _OptionalDataQualityRulesetEvaluationRunFilterTypeDef,
+):
+    pass
+
+
+GetDataQualityResultResponseTypeDef = TypedDict(
+    "GetDataQualityResultResponseTypeDef",
+    {
+        "ResultId": str,
+        "Score": float,
+        "DataSource": DataSourceTypeDef,
+        "RulesetName": str,
+        "EvaluationContext": str,
+        "StartedOn": datetime,
+        "CompletedOn": datetime,
+        "JobName": str,
+        "JobRunId": str,
+        "RulesetEvaluationRunId": str,
+        "RuleResults": List[DataQualityRuleResultTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDataQualityRuleRecommendationRunResponseTypeDef = TypedDict(
+    "GetDataQualityRuleRecommendationRunResponseTypeDef",
+    {
+        "RunId": str,
+        "DataSource": DataSourceTypeDef,
+        "Role": str,
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "Status": TaskStatusTypeType,
+        "ErrorString": str,
+        "StartedOn": datetime,
+        "LastModifiedOn": datetime,
+        "CompletedOn": datetime,
+        "ExecutionTime": int,
+        "RecommendedRuleset": str,
+        "CreatedRulesetName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDataQualityRulesetEvaluationRunResponseTypeDef = TypedDict(
+    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
+    {
+        "RunId": str,
+        "DataSource": DataSourceTypeDef,
+        "Role": str,
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
+        "Status": TaskStatusTypeType,
+        "ErrorString": str,
+        "StartedOn": datetime,
+        "LastModifiedOn": datetime,
+        "CompletedOn": datetime,
+        "ExecutionTime": int,
+        "RulesetNames": List[str],
+        "ResultIds": List[str],
+        "AdditionalDataSources": Dict[str, DataSourceTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+        "Role": str,
+    },
+)
+_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    {
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "CreatedRulesetName": str,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class StartDataQualityRuleRecommendationRunRequestRequestTypeDef(
+    _RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
+    _OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+        "Role": str,
+        "RulesetNames": Sequence[str],
+    },
+)
+_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
+    {
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "ClientToken": str,
+        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
+        "AdditionalDataSources": Mapping[str, DataSourceTypeDef],
+    },
+    total=False,
+)
+
+
+class StartDataQualityRulesetEvaluationRunRequestRequestTypeDef(
+    _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
+    _OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
+):
+    pass
+
+
 CreateSessionResponseTypeDef = TypedDict(
     "CreateSessionResponseTypeDef",
     {
         "Session": SessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "Session": SessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSessionsResponseTypeDef = TypedDict(
     "ListSessionsResponseTypeDef",
     {
         "Ids": List[str],
         "Sessions": List[SessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDataCatalogEncryptionSettingsResponseTypeDef = TypedDict(
     "GetDataCatalogEncryptionSettingsResponseTypeDef",
     {
         "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
     {
         "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsTypeDef,
@@ -7302,14 +8194,15 @@
     "_OptionalDatabaseInputTypeDef",
     {
         "Description": str,
         "LocationUri": str,
         "Parameters": Mapping[str, str],
         "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
         "TargetDatabase": DatabaseIdentifierTypeDef,
+        "FederatedDatabase": FederatedDatabaseTypeDef,
     },
     total=False,
 )
 
 
 class DatabaseInputTypeDef(_RequiredDatabaseInputTypeDef, _OptionalDatabaseInputTypeDef):
     pass
@@ -7327,14 +8220,15 @@
         "Description": str,
         "LocationUri": str,
         "Parameters": Dict[str, str],
         "CreateTime": datetime,
         "CreateTableDefaultPermissions": List[PrincipalPermissionsTypeDef],
         "TargetDatabase": DatabaseIdentifierTypeDef,
         "CatalogId": str,
+        "FederatedDatabase": FederatedDatabaseTypeDef,
     },
     total=False,
 )
 
 
 class DatabaseTypeDef(_RequiredDatabaseTypeDef, _OptionalDatabaseTypeDef):
     pass
@@ -7427,15 +8321,15 @@
     total=False,
 )
 
 DeleteSchemaVersionsResponseTypeDef = TypedDict(
     "DeleteSchemaVersionsResponseTypeDef",
     {
         "SchemaVersionErrors": List[SchemaVersionErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
@@ -7520,14 +8414,62 @@
 
 class AthenaConnectorSourceTypeDef(
     _RequiredAthenaConnectorSourceTypeDef, _OptionalAthenaConnectorSourceTypeDef
 ):
     pass
 
 
+_RequiredCatalogDeltaSourceTypeDef = TypedDict(
+    "_RequiredCatalogDeltaSourceTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+_OptionalCatalogDeltaSourceTypeDef = TypedDict(
+    "_OptionalCatalogDeltaSourceTypeDef",
+    {
+        "AdditionalDeltaOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+
+class CatalogDeltaSourceTypeDef(
+    _RequiredCatalogDeltaSourceTypeDef, _OptionalCatalogDeltaSourceTypeDef
+):
+    pass
+
+
+_RequiredCatalogHudiSourceTypeDef = TypedDict(
+    "_RequiredCatalogHudiSourceTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+_OptionalCatalogHudiSourceTypeDef = TypedDict(
+    "_OptionalCatalogHudiSourceTypeDef",
+    {
+        "AdditionalHudiOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+
+class CatalogHudiSourceTypeDef(
+    _RequiredCatalogHudiSourceTypeDef, _OptionalCatalogHudiSourceTypeDef
+):
+    pass
+
+
 _RequiredCustomCodeTypeDef = TypedDict(
     "_RequiredCustomCodeTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Code": str,
         "ClassName": str,
@@ -7542,14 +8484,39 @@
 )
 
 
 class CustomCodeTypeDef(_RequiredCustomCodeTypeDef, _OptionalCustomCodeTypeDef):
     pass
 
 
+_RequiredDynamicTransformTypeDef = TypedDict(
+    "_RequiredDynamicTransformTypeDef",
+    {
+        "Name": str,
+        "TransformName": str,
+        "Inputs": List[str],
+        "FunctionName": str,
+        "Path": str,
+    },
+)
+_OptionalDynamicTransformTypeDef = TypedDict(
+    "_OptionalDynamicTransformTypeDef",
+    {
+        "Parameters": List[TransformConfigParameterTypeDef],
+        "Version": str,
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+
+class DynamicTransformTypeDef(_RequiredDynamicTransformTypeDef, _OptionalDynamicTransformTypeDef):
+    pass
+
+
 _RequiredJDBCConnectorSourceTypeDef = TypedDict(
     "_RequiredJDBCConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
@@ -7596,14 +8563,62 @@
 
 class JDBCConnectorTargetTypeDef(
     _RequiredJDBCConnectorTargetTypeDef, _OptionalJDBCConnectorTargetTypeDef
 ):
     pass
 
 
+_RequiredS3CatalogDeltaSourceTypeDef = TypedDict(
+    "_RequiredS3CatalogDeltaSourceTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+_OptionalS3CatalogDeltaSourceTypeDef = TypedDict(
+    "_OptionalS3CatalogDeltaSourceTypeDef",
+    {
+        "AdditionalDeltaOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+
+class S3CatalogDeltaSourceTypeDef(
+    _RequiredS3CatalogDeltaSourceTypeDef, _OptionalS3CatalogDeltaSourceTypeDef
+):
+    pass
+
+
+_RequiredS3CatalogHudiSourceTypeDef = TypedDict(
+    "_RequiredS3CatalogHudiSourceTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+_OptionalS3CatalogHudiSourceTypeDef = TypedDict(
+    "_OptionalS3CatalogHudiSourceTypeDef",
+    {
+        "AdditionalHudiOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+
+class S3CatalogHudiSourceTypeDef(
+    _RequiredS3CatalogHudiSourceTypeDef, _OptionalS3CatalogHudiSourceTypeDef
+):
+    pass
+
+
 _RequiredS3CsvSourceTypeDef = TypedDict(
     "_RequiredS3CsvSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
         "Separator": SeparatorType,
         "QuoteChar": QuoteCharType,
@@ -7632,14 +8647,58 @@
 )
 
 
 class S3CsvSourceTypeDef(_RequiredS3CsvSourceTypeDef, _OptionalS3CsvSourceTypeDef):
     pass
 
 
+_RequiredS3DeltaSourceTypeDef = TypedDict(
+    "_RequiredS3DeltaSourceTypeDef",
+    {
+        "Name": str,
+        "Paths": List[str],
+    },
+)
+_OptionalS3DeltaSourceTypeDef = TypedDict(
+    "_OptionalS3DeltaSourceTypeDef",
+    {
+        "AdditionalDeltaOptions": Dict[str, str],
+        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+
+class S3DeltaSourceTypeDef(_RequiredS3DeltaSourceTypeDef, _OptionalS3DeltaSourceTypeDef):
+    pass
+
+
+_RequiredS3HudiSourceTypeDef = TypedDict(
+    "_RequiredS3HudiSourceTypeDef",
+    {
+        "Name": str,
+        "Paths": List[str],
+    },
+)
+_OptionalS3HudiSourceTypeDef = TypedDict(
+    "_OptionalS3HudiSourceTypeDef",
+    {
+        "AdditionalHudiOptions": Dict[str, str],
+        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+
+class S3HudiSourceTypeDef(_RequiredS3HudiSourceTypeDef, _OptionalS3HudiSourceTypeDef):
+    pass
+
+
 _RequiredS3JsonSourceTypeDef = TypedDict(
     "_RequiredS3JsonSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
     },
 )
@@ -7767,24 +8826,24 @@
     pass
 
 
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "JobRun": JobRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobRunsResponseTypeDef = TypedDict(
     "GetJobRunsResponseTypeDef",
     {
         "JobRuns": List[JobRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JobNodeDetailsTypeDef = TypedDict(
     "JobNodeDetailsTypeDef",
     {
         "JobRuns": List[JobRunTypeDef],
@@ -7801,15 +8860,15 @@
         "LogGroupName": str,
         "Properties": TaskRunPropertiesTypeDef,
         "ErrorString": str,
         "StartedOn": datetime,
         "LastModifiedOn": datetime,
         "CompletedOn": datetime,
         "ExecutionTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TaskRunTypeDef = TypedDict(
     "TaskRunTypeDef",
     {
         "TransformId": str,
@@ -7860,15 +8919,15 @@
 
 QuerySchemaVersionMetadataResponseTypeDef = TypedDict(
     "QuerySchemaVersionMetadataResponseTypeDef",
     {
         "MetadataInfoMap": Dict[str, MetadataInfoTypeDef],
         "SchemaVersionId": str,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateUserDefinedFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserDefinedFunctionRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -7915,24 +8974,24 @@
     pass
 
 
 GetUserDefinedFunctionResponseTypeDef = TypedDict(
     "GetUserDefinedFunctionResponseTypeDef",
     {
         "UserDefinedFunction": UserDefinedFunctionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserDefinedFunctionsResponseTypeDef = TypedDict(
     "GetUserDefinedFunctionsResponseTypeDef",
     {
         "UserDefinedFunctions": List[UserDefinedFunctionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StatementTypeDef = TypedDict(
     "StatementTypeDef",
     {
         "Id": int,
@@ -7947,41 +9006,41 @@
 )
 
 GetPartitionIndexesResponseTypeDef = TypedDict(
     "GetPartitionIndexesResponseTypeDef",
     {
         "PartitionIndexDescriptorList": List[PartitionIndexDescriptorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetTriggersResponseTypeDef = TypedDict(
     "BatchGetTriggersResponseTypeDef",
     {
         "Triggers": List[TriggerTypeDef],
         "TriggersNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTriggerResponseTypeDef = TypedDict(
     "GetTriggerResponseTypeDef",
     {
         "Trigger": TriggerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTriggersResponseTypeDef = TypedDict(
     "GetTriggersResponseTypeDef",
     {
         "Triggers": List[TriggerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TriggerNodeDetailsTypeDef = TypedDict(
     "TriggerNodeDetailsTypeDef",
     {
         "Trigger": TriggerTypeDef,
@@ -7989,15 +9048,15 @@
     total=False,
 )
 
 UpdateTriggerResponseTypeDef = TypedDict(
     "UpdateTriggerResponseTypeDef",
     {
         "Trigger": TriggerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTriggerRequestRequestTypeDef = TypedDict(
     "UpdateTriggerRequestRequestTypeDef",
     {
         "Name": str,
@@ -8023,15 +9082,15 @@
         "GlueVersion": str,
         "MaxCapacity": float,
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "Timeout": int,
         "MaxRetries": int,
         "TransformEncryption": TransformEncryptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MLTransformTypeDef = TypedDict(
     "MLTransformTypeDef",
     {
         "TransformId": str,
@@ -8058,33 +9117,99 @@
 )
 
 BatchGetCrawlersResponseTypeDef = TypedDict(
     "BatchGetCrawlersResponseTypeDef",
     {
         "Crawlers": List[CrawlerTypeDef],
         "CrawlersNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCrawlerResponseTypeDef = TypedDict(
     "GetCrawlerResponseTypeDef",
     {
         "Crawler": CrawlerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCrawlersResponseTypeDef = TypedDict(
     "GetCrawlersResponseTypeDef",
     {
         "Crawlers": List[CrawlerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDataQualityResultsResponseTypeDef = TypedDict(
+    "ListDataQualityResultsResponseTypeDef",
+    {
+        "Results": List[DataQualityResultDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDataQualityResultsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityResultsRequestRequestTypeDef",
+    {
+        "Filter": DataQualityResultFilterCriteriaTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
     },
+    total=False,
+)
+
+BatchGetDataQualityResultResponseTypeDef = TypedDict(
+    "BatchGetDataQualityResultResponseTypeDef",
+    {
+        "Results": List[DataQualityResultTypeDef],
+        "ResultsNotFound": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDataQualityRuleRecommendationRunsResponseTypeDef = TypedDict(
+    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
+    {
+        "Runs": List[DataQualityRuleRecommendationRunDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDataQualityRuleRecommendationRunsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
+    {
+        "Filter": DataQualityRuleRecommendationRunFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDataQualityRulesetEvaluationRunsResponseTypeDef = TypedDict(
+    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
+    {
+        "Runs": List[DataQualityRulesetEvaluationRunDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
+    {
+        "Filter": DataQualityRulesetEvaluationRunFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
 )
 
 _RequiredCreateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatabaseRequestRequestTypeDef",
     {
         "DatabaseInput": DatabaseInputTypeDef,
     },
@@ -8127,24 +9252,24 @@
     pass
 
 
 GetDatabaseResponseTypeDef = TypedDict(
     "GetDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDatabasesResponseTypeDef = TypedDict(
     "GetDatabasesResponseTypeDef",
     {
         "DatabaseList": List[DatabaseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ColumnStatisticsTypeDef = TypedDict(
     "ColumnStatisticsTypeDef",
     {
         "ColumnName": str,
@@ -8236,37 +9361,38 @@
         "TableType": str,
         "Parameters": Dict[str, str],
         "CreatedBy": str,
         "IsRegisteredWithLakeFormation": bool,
         "TargetTable": TableIdentifierTypeDef,
         "CatalogId": str,
         "VersionId": str,
+        "FederatedTable": FederatedTableTypeDef,
     },
     total=False,
 )
 
 
 class TableTypeDef(_RequiredTableTypeDef, _OptionalTableTypeDef):
     pass
 
 
 GetSecurityConfigurationResponseTypeDef = TypedDict(
     "GetSecurityConfigurationResponseTypeDef",
     {
         "SecurityConfiguration": SecurityConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSecurityConfigurationsResponseTypeDef = TypedDict(
     "GetSecurityConfigurationsResponseTypeDef",
     {
         "SecurityConfigurations": List[SecurityConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CodeGenConfigurationNodeTypeDef = TypedDict(
     "CodeGenConfigurationNodeTypeDef",
     {
         "AthenaConnectorSource": AthenaConnectorSourceTypeDef,
@@ -8315,41 +9441,57 @@
         "MySQLCatalogSource": MySQLCatalogSourceTypeDef,
         "OracleSQLCatalogSource": OracleSQLCatalogSourceTypeDef,
         "PostgreSQLCatalogSource": PostgreSQLCatalogSourceTypeDef,
         "MicrosoftSQLServerCatalogTarget": MicrosoftSQLServerCatalogTargetTypeDef,
         "MySQLCatalogTarget": MySQLCatalogTargetTypeDef,
         "OracleSQLCatalogTarget": OracleSQLCatalogTargetTypeDef,
         "PostgreSQLCatalogTarget": PostgreSQLCatalogTargetTypeDef,
+        "DynamicTransform": DynamicTransformTypeDef,
+        "EvaluateDataQuality": EvaluateDataQualityTypeDef,
+        "S3CatalogHudiSource": S3CatalogHudiSourceTypeDef,
+        "CatalogHudiSource": CatalogHudiSourceTypeDef,
+        "S3HudiSource": S3HudiSourceTypeDef,
+        "S3HudiCatalogTarget": S3HudiCatalogTargetTypeDef,
+        "S3HudiDirectTarget": S3HudiDirectTargetTypeDef,
+        "DirectJDBCSource": DirectJDBCSourceTypeDef,
+        "S3CatalogDeltaSource": S3CatalogDeltaSourceTypeDef,
+        "CatalogDeltaSource": CatalogDeltaSourceTypeDef,
+        "S3DeltaSource": S3DeltaSourceTypeDef,
+        "S3DeltaCatalogTarget": S3DeltaCatalogTargetTypeDef,
+        "S3DeltaDirectTarget": S3DeltaDirectTargetTypeDef,
+        "AmazonRedshiftSource": AmazonRedshiftSourceTypeDef,
+        "AmazonRedshiftTarget": AmazonRedshiftTargetTypeDef,
+        "EvaluateDataQualityMultiFrame": EvaluateDataQualityMultiFrameTypeDef,
     },
     total=False,
 )
 
 GetMLTaskRunsResponseTypeDef = TypedDict(
     "GetMLTaskRunsResponseTypeDef",
     {
         "TaskRuns": List[TaskRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStatementResponseTypeDef = TypedDict(
     "GetStatementResponseTypeDef",
     {
         "Statement": StatementTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStatementsResponseTypeDef = TypedDict(
     "ListStatementsResponseTypeDef",
     {
         "Statements": List[StatementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "Type": NodeTypeType,
@@ -8363,15 +9505,15 @@
 )
 
 GetMLTransformsResponseTypeDef = TypedDict(
     "GetMLTransformsResponseTypeDef",
     {
         "Transforms": List[MLTransformTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ColumnStatisticsErrorTypeDef = TypedDict(
     "ColumnStatisticsErrorTypeDef",
     {
         "ColumnStatistics": ColumnStatisticsTypeDef,
@@ -8381,24 +9523,24 @@
 )
 
 GetColumnStatisticsForPartitionResponseTypeDef = TypedDict(
     "GetColumnStatisticsForPartitionResponseTypeDef",
     {
         "ColumnStatisticsList": List[ColumnStatisticsTypeDef],
         "Errors": List[ColumnErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetColumnStatisticsForTableResponseTypeDef = TypedDict(
     "GetColumnStatisticsForTableResponseTypeDef",
     {
         "ColumnStatisticsList": List[ColumnStatisticsTypeDef],
         "Errors": List[ColumnErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -8527,42 +9669,42 @@
 
 
 BatchGetPartitionResponseTypeDef = TypedDict(
     "BatchGetPartitionResponseTypeDef",
     {
         "Partitions": List[PartitionTypeDef],
         "UnprocessedKeys": List[PartitionValueListTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPartitionResponseTypeDef = TypedDict(
     "GetPartitionResponseTypeDef",
     {
         "Partition": PartitionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPartitionsResponseTypeDef = TypedDict(
     "GetPartitionsResponseTypeDef",
     {
         "Partitions": List[PartitionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUnfilteredPartitionMetadataResponseTypeDef = TypedDict(
     "GetUnfilteredPartitionMetadataResponseTypeDef",
     {
         "Partition": PartitionTypeDef,
         "AuthorizedColumns": List[str],
         "IsRegisteredWithLakeFormation": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UnfilteredPartitionTypeDef = TypedDict(
     "UnfilteredPartitionTypeDef",
     {
         "Partition": PartitionTypeDef,
@@ -8621,44 +9763,44 @@
     pass
 
 
 GetTableResponseTypeDef = TypedDict(
     "GetTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTablesResponseTypeDef = TypedDict(
     "GetTablesResponseTypeDef",
     {
         "TableList": List[TableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUnfilteredTableMetadataResponseTypeDef = TypedDict(
     "GetUnfilteredTableMetadataResponseTypeDef",
     {
         "Table": TableTypeDef,
         "AuthorizedColumns": List[str],
         "IsRegisteredWithLakeFormation": bool,
         "CellFilters": List[ColumnRowFilterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchTablesResponseTypeDef = TypedDict(
     "SearchTablesResponseTypeDef",
     {
         "NextToken": str,
         "TableList": List[TableTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TableVersionTypeDef = TypedDict(
     "TableVersionTypeDef",
     {
         "Table": TableTypeDef,
@@ -8774,23 +9916,23 @@
     total=False,
 )
 
 UpdateColumnStatisticsForPartitionResponseTypeDef = TypedDict(
     "UpdateColumnStatisticsForPartitionResponseTypeDef",
     {
         "Errors": List[ColumnStatisticsErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateColumnStatisticsForTableResponseTypeDef = TypedDict(
     "UpdateColumnStatisticsForTableResponseTypeDef",
     {
         "Errors": List[ColumnStatisticsErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchUpdatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchUpdatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -8815,58 +9957,58 @@
 
 
 GetUnfilteredPartitionsMetadataResponseTypeDef = TypedDict(
     "GetUnfilteredPartitionsMetadataResponseTypeDef",
     {
         "UnfilteredPartitions": List[UnfilteredPartitionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTableVersionResponseTypeDef = TypedDict(
     "GetTableVersionResponseTypeDef",
     {
         "TableVersion": TableVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTableVersionsResponseTypeDef = TypedDict(
     "GetTableVersionsResponseTypeDef",
     {
         "TableVersions": List[TableVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetJobsResponseTypeDef = TypedDict(
     "BatchGetJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "JobsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobsResponseTypeDef = TypedDict(
     "GetJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateJobRequestRequestTypeDef = TypedDict(
     "UpdateJobRequestRequestTypeDef",
     {
         "JobName": str,
@@ -8892,24 +10034,24 @@
     total=False,
 )
 
 GetWorkflowRunResponseTypeDef = TypedDict(
     "GetWorkflowRunResponseTypeDef",
     {
         "Run": WorkflowRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWorkflowRunsResponseTypeDef = TypedDict(
     "GetWorkflowRunsResponseTypeDef",
     {
         "Runs": List[WorkflowRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorkflowTypeDef = TypedDict(
     "WorkflowTypeDef",
     {
         "Name": str,
@@ -8926,18 +10068,18 @@
 )
 
 BatchGetWorkflowsResponseTypeDef = TypedDict(
     "BatchGetWorkflowsResponseTypeDef",
     {
         "Workflows": List[WorkflowTypeDef],
         "MissingWorkflows": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWorkflowResponseTypeDef = TypedDict(
     "GetWorkflowResponseTypeDef",
     {
         "Workflow": WorkflowTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-glue-1.26.8/mypy_boto3_glue/type_defs.pyi` & `mypy-boto3-glue-1.27.0/mypy_boto3_glue/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -30,33 +30,41 @@
     ConnectionTypeType,
     CrawlerHistoryStateType,
     CrawlerLineageSettingsType,
     CrawlerStateType,
     CrawlStateType,
     CsvHeaderOptionType,
     DataFormatType,
+    DataQualityRuleResultStatusType,
     DeleteBehaviorType,
+    DeltaTargetCompressionTypeType,
+    DQStopJobOnFailureTimingType,
+    DQTransformOutputType,
     EnableHybridValuesType,
     ExecutionClassType,
     ExistConditionType,
     FieldNameType,
     FilterLogicalOperatorType,
     FilterOperationType,
     FilterOperatorType,
     FilterValueTypeType,
     GlueRecordTypeType,
+    HudiTargetCompressionTypeType,
+    JDBCConnectionTypeType,
     JDBCDataTypeType,
+    JdbcMetadataEntryType,
     JobBookmarksEncryptionModeType,
     JobRunStateType,
     JoinTypeType,
     LanguageType,
     LastCrawlStatusType,
     LogicalType,
     MLUserDataEncryptionModeStringType,
     NodeTypeType,
+    ParamTypeType,
     ParquetCompressionTypeType,
     PartitionIndexStatusType,
     PermissionType,
     PermissionTypeType,
     PiiTypeType,
     PrincipalTypeType,
     QuoteCharType,
@@ -99,55 +107,62 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "NotificationPropertyTypeDef",
     "AggregateOperationTypeDef",
+    "AmazonRedshiftAdvancedOptionTypeDef",
+    "OptionTypeDef",
     "ApplyMappingTypeDef",
     "AuditContextTypeDef",
     "PartitionValueListTypeDef",
     "BasicCatalogTargetTypeDef",
-    "ResponseMetadataTypeDef",
     "BatchDeleteConnectionRequestRequestTypeDef",
     "ErrorDetailTypeDef",
     "BatchDeleteTableRequestRequestTypeDef",
     "BatchDeleteTableVersionRequestRequestTypeDef",
     "BatchGetBlueprintsRequestRequestTypeDef",
     "BatchGetCrawlersRequestRequestTypeDef",
     "BatchGetCustomEntityTypesRequestRequestTypeDef",
     "CustomEntityTypeTypeDef",
+    "BatchGetDataQualityResultRequestRequestTypeDef",
     "BatchGetDevEndpointsRequestRequestTypeDef",
     "DevEndpointTypeDef",
     "BatchGetJobsRequestRequestTypeDef",
     "BatchGetTriggersRequestRequestTypeDef",
     "BatchGetWorkflowsRequestRequestTypeDef",
     "BatchStopJobRunRequestRequestTypeDef",
     "BatchStopJobRunSuccessfulSubmissionTypeDef",
     "BinaryColumnStatisticsDataTypeDef",
     "BlueprintDetailsTypeDef",
     "BlueprintRunTypeDef",
     "LastActiveDefinitionTypeDef",
     "BooleanColumnStatisticsDataTypeDef",
+    "CancelDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    "CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     "CancelMLTaskRunRequestRequestTypeDef",
+    "CancelMLTaskRunResponseTypeDef",
     "CancelStatementRequestRequestTypeDef",
     "CatalogEntryTypeDef",
     "CatalogImportStatusTypeDef",
     "KafkaStreamingSourceOptionsTypeDef",
     "StreamingDataPreviewOptionsTypeDef",
     "KinesisStreamingSourceOptionsTypeDef",
     "CatalogSchemaChangePolicyTypeDef",
     "CatalogSourceTypeDef",
     "CatalogTargetTypeDef",
     "CheckSchemaVersionValidityInputRequestTypeDef",
+    "CheckSchemaVersionValidityResponseTypeDef",
     "CsvClassifierTypeDef",
     "GrokClassifierTypeDef",
     "JsonClassifierTypeDef",
     "XMLClassifierTypeDef",
     "CloudWatchEncryptionTypeDef",
+    "DirectJDBCSourceTypeDef",
     "DropDuplicatesTypeDef",
     "DropFieldsTypeDef",
     "DynamoDBCatalogSourceTypeDef",
     "FillMissingValuesTypeDef",
     "MergeTypeDef",
     "MicrosoftSQLServerCatalogSourceTypeDef",
     "MicrosoftSQLServerCatalogTargetTypeDef",
@@ -181,277 +196,311 @@
     "ConnectionPasswordEncryptionTypeDef",
     "ConnectionsListTypeDef",
     "CrawlTypeDef",
     "CrawlerHistoryTypeDef",
     "CrawlerMetricsTypeDef",
     "DeltaTargetTypeDef",
     "DynamoDBTargetTypeDef",
+    "IcebergTargetTypeDef",
     "JdbcTargetTypeDef",
     "MongoDBTargetTypeDef",
     "S3TargetTypeDef",
     "LakeFormationConfigurationTypeDef",
     "LastCrawlInfoTypeDef",
     "LineageConfigurationTypeDef",
     "RecrawlPolicyTypeDef",
     "ScheduleTypeDef",
     "SchemaChangePolicyTypeDef",
     "CrawlsFilterTypeDef",
     "CreateBlueprintRequestRequestTypeDef",
+    "CreateBlueprintResponseTypeDef",
     "CreateCsvClassifierRequestTypeDef",
     "CreateGrokClassifierRequestTypeDef",
     "CreateJsonClassifierRequestTypeDef",
     "CreateXMLClassifierRequestTypeDef",
     "CreateCustomEntityTypeRequestRequestTypeDef",
+    "CreateCustomEntityTypeResponseTypeDef",
+    "DataQualityTargetTableTypeDef",
+    "CreateDataQualityRulesetResponseTypeDef",
     "CreateDevEndpointRequestRequestTypeDef",
+    "CreateDevEndpointResponseTypeDef",
     "ExecutionPropertyTypeDef",
     "JobCommandTypeDef",
     "SourceControlDetailsTypeDef",
+    "CreateJobResponseTypeDef",
     "GlueTableTypeDef",
+    "CreateMLTransformResponseTypeDef",
     "PartitionIndexTypeDef",
     "CreateRegistryInputRequestTypeDef",
+    "CreateRegistryResponseTypeDef",
     "RegistryIdTypeDef",
+    "CreateSchemaResponseTypeDef",
+    "CreateScriptResponseTypeDef",
+    "CreateSecurityConfigurationResponseTypeDef",
     "SessionCommandTypeDef",
     "EventBatchingConditionTypeDef",
+    "CreateTriggerResponseTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
+    "CreateWorkflowResponseTypeDef",
+    "DQResultsPublishingOptionsTypeDef",
+    "DQStopJobOnFailureOptionsTypeDef",
     "EncryptionAtRestTypeDef",
     "DataLakePrincipalTypeDef",
+    "DataQualityEvaluationRunAdditionalRunOptionsTypeDef",
+    "DataQualityRuleResultTypeDef",
     "DatabaseIdentifierTypeDef",
+    "FederatedDatabaseTypeDef",
     "DatatypeTypeDef",
     "DecimalNumberTypeDef",
     "DeleteBlueprintRequestRequestTypeDef",
+    "DeleteBlueprintResponseTypeDef",
     "DeleteClassifierRequestRequestTypeDef",
     "DeleteColumnStatisticsForPartitionRequestRequestTypeDef",
     "DeleteColumnStatisticsForTableRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteCrawlerRequestRequestTypeDef",
     "DeleteCustomEntityTypeRequestRequestTypeDef",
+    "DeleteCustomEntityTypeResponseTypeDef",
+    "DeleteDataQualityRulesetRequestRequestTypeDef",
     "DeleteDatabaseRequestRequestTypeDef",
     "DeleteDevEndpointRequestRequestTypeDef",
     "DeleteJobRequestRequestTypeDef",
+    "DeleteJobResponseTypeDef",
     "DeleteMLTransformRequestRequestTypeDef",
+    "DeleteMLTransformResponseTypeDef",
     "DeletePartitionIndexRequestRequestTypeDef",
     "DeletePartitionRequestRequestTypeDef",
+    "DeleteRegistryResponseTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "SchemaIdTypeDef",
+    "DeleteSchemaResponseTypeDef",
     "DeleteSecurityConfigurationRequestRequestTypeDef",
     "DeleteSessionRequestRequestTypeDef",
+    "DeleteSessionResponseTypeDef",
     "DeleteTableRequestRequestTypeDef",
     "DeleteTableVersionRequestRequestTypeDef",
     "DeleteTriggerRequestRequestTypeDef",
+    "DeleteTriggerResponseTypeDef",
     "DeleteUserDefinedFunctionRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
+    "DeleteWorkflowResponseTypeDef",
     "DevEndpointCustomLibrariesTypeDef",
     "DirectSchemaChangePolicyTypeDef",
     "NullCheckBoxListTypeDef",
+    "TransformConfigParameterTypeDef",
     "EdgeTypeDef",
     "JobBookmarksEncryptionTypeDef",
     "S3EncryptionTypeDef",
     "ErrorDetailsTypeDef",
     "ExportLabelsTaskRunPropertiesTypeDef",
+    "FederatedTableTypeDef",
     "FilterValueTypeDef",
     "FindMatchesParametersTypeDef",
     "FindMatchesTaskRunPropertiesTypeDef",
     "GetBlueprintRequestRequestTypeDef",
     "GetBlueprintRunRequestRequestTypeDef",
     "GetBlueprintRunsRequestRequestTypeDef",
     "GetCatalogImportStatusRequestRequestTypeDef",
     "GetClassifierRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     "GetClassifiersRequestRequestTypeDef",
     "GetColumnStatisticsForPartitionRequestRequestTypeDef",
     "GetColumnStatisticsForTableRequestRequestTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "GetConnectionsFilterTypeDef",
+    "GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef",
     "GetCrawlerMetricsRequestRequestTypeDef",
     "GetCrawlerRequestRequestTypeDef",
+    "GetCrawlersRequestGetCrawlersPaginateTypeDef",
     "GetCrawlersRequestRequestTypeDef",
     "GetCustomEntityTypeRequestRequestTypeDef",
+    "GetCustomEntityTypeResponseTypeDef",
     "GetDataCatalogEncryptionSettingsRequestRequestTypeDef",
+    "GetDataQualityResultRequestRequestTypeDef",
+    "GetDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    "GetDataQualityRulesetEvaluationRunRequestRequestTypeDef",
+    "GetDataQualityRulesetRequestRequestTypeDef",
     "GetDatabaseRequestRequestTypeDef",
+    "GetDatabasesRequestGetDatabasesPaginateTypeDef",
     "GetDatabasesRequestRequestTypeDef",
     "GetDataflowGraphRequestRequestTypeDef",
     "GetDevEndpointRequestRequestTypeDef",
+    "GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef",
     "GetDevEndpointsRequestRequestTypeDef",
     "GetJobBookmarkRequestRequestTypeDef",
     "JobBookmarkEntryTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetJobRunRequestRequestTypeDef",
+    "GetJobRunsRequestGetJobRunsPaginateTypeDef",
     "GetJobRunsRequestRequestTypeDef",
+    "GetJobsRequestGetJobsPaginateTypeDef",
     "GetJobsRequestRequestTypeDef",
     "GetMLTaskRunRequestRequestTypeDef",
     "TaskRunFilterCriteriaTypeDef",
     "TaskRunSortCriteriaTypeDef",
     "GetMLTransformRequestRequestTypeDef",
     "SchemaColumnTypeDef",
     "TransformSortCriteriaTypeDef",
     "MappingEntryTypeDef",
+    "GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef",
     "GetPartitionIndexesRequestRequestTypeDef",
     "GetPartitionRequestRequestTypeDef",
     "SegmentTypeDef",
+    "GetPlanResponseTypeDef",
+    "GetRegistryResponseTypeDef",
+    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GluePolicyTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "GetSchemaByDefinitionResponseTypeDef",
+    "GetSchemaResponseTypeDef",
     "SchemaVersionNumberTypeDef",
+    "GetSchemaVersionResponseTypeDef",
+    "GetSchemaVersionsDiffResponseTypeDef",
     "GetSecurityConfigurationRequestRequestTypeDef",
+    "GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef",
     "GetSecurityConfigurationsRequestRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
     "GetStatementRequestRequestTypeDef",
     "GetTableRequestRequestTypeDef",
     "GetTableVersionRequestRequestTypeDef",
+    "GetTableVersionsRequestGetTableVersionsPaginateTypeDef",
     "GetTableVersionsRequestRequestTypeDef",
+    "GetTablesRequestGetTablesPaginateTypeDef",
     "GetTablesRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
+    "GetTagsResponseTypeDef",
     "GetTriggerRequestRequestTypeDef",
+    "GetTriggersRequestGetTriggersPaginateTypeDef",
     "GetTriggersRequestRequestTypeDef",
     "GetUserDefinedFunctionRequestRequestTypeDef",
+    "GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef",
     "GetUserDefinedFunctionsRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
+    "GetWorkflowRunPropertiesResponseTypeDef",
     "GetWorkflowRunRequestRequestTypeDef",
     "GetWorkflowRunsRequestRequestTypeDef",
     "GlueStudioSchemaColumnTypeDef",
     "S3SourceAdditionalOptionsTypeDef",
     "ImportCatalogToGlueRequestRequestTypeDef",
     "ImportLabelsTaskRunPropertiesTypeDef",
     "JDBCConnectorOptionsTypeDef",
     "PredecessorTypeDef",
     "JoinColumnTypeDef",
     "KeySchemaElementTypeDef",
     "LabelingSetGenerationTaskRunPropertiesTypeDef",
     "ListBlueprintsRequestRequestTypeDef",
+    "ListBlueprintsResponseTypeDef",
     "ListCrawlersRequestRequestTypeDef",
+    "ListCrawlersResponseTypeDef",
     "ListCustomEntityTypesRequestRequestTypeDef",
     "ListDevEndpointsRequestRequestTypeDef",
+    "ListDevEndpointsResponseTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListJobsResponseTypeDef",
+    "ListMLTransformsResponseTypeDef",
+    "ListRegistriesInputListRegistriesPaginateTypeDef",
     "ListRegistriesInputRequestTypeDef",
     "RegistryListItemTypeDef",
     "SchemaVersionListItemTypeDef",
     "SchemaListItemTypeDef",
     "ListSessionsRequestRequestTypeDef",
     "ListStatementsRequestRequestTypeDef",
     "ListTriggersRequestRequestTypeDef",
+    "ListTriggersResponseTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
+    "ListWorkflowsResponseTypeDef",
     "MLUserDataEncryptionTypeDef",
     "MappingTypeDef",
     "OtherMetadataValueListItemTypeDef",
     "MetadataKeyValuePairTypeDef",
     "OrderTypeDef",
+    "PaginatorConfigTypeDef",
     "PropertyPredicateTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "PutSchemaVersionMetadataResponseTypeDef",
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
     "UpsertRedshiftTargetOptionsTypeDef",
+    "RegisterSchemaVersionResponseTypeDef",
+    "RemoveSchemaVersionMetadataResponseTypeDef",
     "ResetJobBookmarkRequestRequestTypeDef",
     "ResourceUriTypeDef",
+    "ResponseMetadataTypeDef",
     "ResumeWorkflowRunRequestRequestTypeDef",
+    "ResumeWorkflowRunResponseTypeDef",
     "RunStatementRequestRequestTypeDef",
+    "RunStatementResponseTypeDef",
     "S3DirectSourceAdditionalOptionsTypeDef",
     "SortCriterionTypeDef",
     "SerDeInfoTypeDef",
     "SkewedInfoTypeDef",
     "SqlAliasTypeDef",
     "StartBlueprintRunRequestRequestTypeDef",
+    "StartBlueprintRunResponseTypeDef",
     "StartCrawlerRequestRequestTypeDef",
     "StartCrawlerScheduleRequestRequestTypeDef",
+    "StartDataQualityRuleRecommendationRunResponseTypeDef",
+    "StartDataQualityRulesetEvaluationRunResponseTypeDef",
     "StartExportLabelsTaskRunRequestRequestTypeDef",
+    "StartExportLabelsTaskRunResponseTypeDef",
     "StartImportLabelsTaskRunRequestRequestTypeDef",
+    "StartImportLabelsTaskRunResponseTypeDef",
+    "StartJobRunResponseTypeDef",
     "StartMLEvaluationTaskRunRequestRequestTypeDef",
+    "StartMLEvaluationTaskRunResponseTypeDef",
     "StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef",
+    "StartMLLabelingSetGenerationTaskRunResponseTypeDef",
     "StartTriggerRequestRequestTypeDef",
+    "StartTriggerResponseTypeDef",
     "StartWorkflowRunRequestRequestTypeDef",
+    "StartWorkflowRunResponseTypeDef",
     "StartingEventBatchConditionTypeDef",
     "StatementOutputDataTypeDef",
     "StopCrawlerRequestRequestTypeDef",
     "StopCrawlerScheduleRequestRequestTypeDef",
     "StopSessionRequestRequestTypeDef",
+    "StopSessionResponseTypeDef",
     "StopTriggerRequestRequestTypeDef",
+    "StopTriggerResponseTypeDef",
     "StopWorkflowRunRequestRequestTypeDef",
     "TableIdentifierTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBlueprintRequestRequestTypeDef",
+    "UpdateBlueprintResponseTypeDef",
     "UpdateCsvClassifierRequestTypeDef",
     "UpdateGrokClassifierRequestTypeDef",
     "UpdateJsonClassifierRequestTypeDef",
     "UpdateXMLClassifierRequestTypeDef",
     "UpdateCrawlerScheduleRequestRequestTypeDef",
+    "UpdateDataQualityRulesetRequestRequestTypeDef",
+    "UpdateDataQualityRulesetResponseTypeDef",
     "UpdateJobFromSourceControlRequestRequestTypeDef",
+    "UpdateJobFromSourceControlResponseTypeDef",
+    "UpdateJobResponseTypeDef",
+    "UpdateMLTransformResponseTypeDef",
+    "UpdateRegistryResponseTypeDef",
+    "UpdateSchemaResponseTypeDef",
     "UpdateSourceControlFromJobRequestRequestTypeDef",
+    "UpdateSourceControlFromJobResponseTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
+    "UpdateWorkflowResponseTypeDef",
     "WorkflowRunStatisticsTypeDef",
     "ActionTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "AggregateTypeDef",
+    "AmazonRedshiftNodeDataTypeDef",
     "GetUnfilteredPartitionMetadataRequestRequestTypeDef",
     "GetUnfilteredTableMetadataRequestRequestTypeDef",
     "BackfillErrorTypeDef",
     "BatchDeletePartitionRequestRequestTypeDef",
     "BatchGetPartitionRequestRequestTypeDef",
-    "CancelMLTaskRunResponseTypeDef",
-    "CheckSchemaVersionValidityResponseTypeDef",
-    "CreateBlueprintResponseTypeDef",
-    "CreateCustomEntityTypeResponseTypeDef",
-    "CreateDevEndpointResponseTypeDef",
-    "CreateJobResponseTypeDef",
-    "CreateMLTransformResponseTypeDef",
-    "CreateRegistryResponseTypeDef",
-    "CreateSchemaResponseTypeDef",
-    "CreateScriptResponseTypeDef",
-    "CreateSecurityConfigurationResponseTypeDef",
-    "CreateTriggerResponseTypeDef",
-    "CreateWorkflowResponseTypeDef",
-    "DeleteBlueprintResponseTypeDef",
-    "DeleteCustomEntityTypeResponseTypeDef",
-    "DeleteJobResponseTypeDef",
-    "DeleteMLTransformResponseTypeDef",
-    "DeleteRegistryResponseTypeDef",
-    "DeleteSchemaResponseTypeDef",
-    "DeleteSessionResponseTypeDef",
-    "DeleteTriggerResponseTypeDef",
-    "DeleteWorkflowResponseTypeDef",
-    "GetCustomEntityTypeResponseTypeDef",
-    "GetPlanResponseTypeDef",
-    "GetRegistryResponseTypeDef",
-    "GetResourcePolicyResponseTypeDef",
-    "GetSchemaByDefinitionResponseTypeDef",
-    "GetSchemaResponseTypeDef",
-    "GetSchemaVersionResponseTypeDef",
-    "GetSchemaVersionsDiffResponseTypeDef",
-    "GetTagsResponseTypeDef",
-    "GetWorkflowRunPropertiesResponseTypeDef",
-    "ListBlueprintsResponseTypeDef",
-    "ListCrawlersResponseTypeDef",
-    "ListDevEndpointsResponseTypeDef",
-    "ListJobsResponseTypeDef",
-    "ListMLTransformsResponseTypeDef",
-    "ListTriggersResponseTypeDef",
-    "ListWorkflowsResponseTypeDef",
-    "PutResourcePolicyResponseTypeDef",
-    "PutSchemaVersionMetadataResponseTypeDef",
-    "RegisterSchemaVersionResponseTypeDef",
-    "RemoveSchemaVersionMetadataResponseTypeDef",
-    "ResumeWorkflowRunResponseTypeDef",
-    "RunStatementResponseTypeDef",
-    "StartBlueprintRunResponseTypeDef",
-    "StartExportLabelsTaskRunResponseTypeDef",
-    "StartImportLabelsTaskRunResponseTypeDef",
-    "StartJobRunResponseTypeDef",
-    "StartMLEvaluationTaskRunResponseTypeDef",
-    "StartMLLabelingSetGenerationTaskRunResponseTypeDef",
-    "StartTriggerResponseTypeDef",
-    "StartWorkflowRunResponseTypeDef",
-    "StopSessionResponseTypeDef",
-    "StopTriggerResponseTypeDef",
-    "UpdateBlueprintResponseTypeDef",
-    "UpdateJobFromSourceControlResponseTypeDef",
-    "UpdateJobResponseTypeDef",
-    "UpdateMLTransformResponseTypeDef",
-    "UpdateRegistryResponseTypeDef",
-    "UpdateSchemaResponseTypeDef",
-    "UpdateSourceControlFromJobResponseTypeDef",
-    "UpdateWorkflowResponseTypeDef",
     "BatchDeleteConnectionResponseTypeDef",
     "BatchStopJobRunErrorTypeDef",
     "BatchUpdatePartitionFailureEntryTypeDef",
     "ColumnErrorTypeDef",
     "PartitionErrorTypeDef",
     "TableErrorTypeDef",
     "TableVersionErrorTypeDef",
@@ -466,70 +515,66 @@
     "GetCatalogImportStatusResponseTypeDef",
     "CatalogKafkaSourceTypeDef",
     "DirectKafkaSourceTypeDef",
     "CatalogKinesisSourceTypeDef",
     "DirectKinesisSourceTypeDef",
     "GovernedCatalogTargetTypeDef",
     "S3CatalogTargetTypeDef",
+    "S3DeltaCatalogTargetTypeDef",
+    "S3HudiCatalogTargetTypeDef",
     "ClassifierTypeDef",
     "CodeGenNodeTypeDef",
     "LocationTypeDef",
     "PredicateTypeDef",
     "FindMatchesMetricsTypeDef",
     "ConnectionInputTypeDef",
     "ConnectionTypeDef",
     "CrawlerNodeDetailsTypeDef",
     "ListCrawlsResponseTypeDef",
     "GetCrawlerMetricsResponseTypeDef",
     "CrawlerTargetsTypeDef",
     "ListCrawlsRequestRequestTypeDef",
     "CreateClassifierRequestRequestTypeDef",
+    "CreateDataQualityRulesetRequestRequestTypeDef",
+    "DataQualityRulesetFilterCriteriaTypeDef",
+    "DataQualityRulesetListDetailsTypeDef",
+    "GetDataQualityRulesetResponseTypeDef",
+    "DataSourceTypeDef",
     "CreatePartitionIndexRequestRequestTypeDef",
     "CreateSchemaInputRequestTypeDef",
     "DeleteRegistryInputRequestTypeDef",
     "GetRegistryInputRequestTypeDef",
+    "ListSchemasInputListSchemasPaginateTypeDef",
     "ListSchemasInputRequestTypeDef",
     "UpdateRegistryInputRequestTypeDef",
     "CreateSessionRequestRequestTypeDef",
     "SessionTypeDef",
+    "EvaluateDataQualityMultiFrameTypeDef",
+    "EvaluateDataQualityTypeDef",
     "DataCatalogEncryptionSettingsTypeDef",
     "PrincipalPermissionsTypeDef",
     "NullValueFieldTypeDef",
     "DecimalColumnStatisticsDataTypeDef",
     "DeleteSchemaInputRequestTypeDef",
     "DeleteSchemaVersionsInputRequestTypeDef",
     "GetSchemaByDefinitionInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
+    "ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
     "ListSchemaVersionsInputRequestTypeDef",
     "RegisterSchemaVersionInputRequestTypeDef",
     "SchemaReferenceTypeDef",
     "UpdateDevEndpointRequestRequestTypeDef",
+    "S3DeltaDirectTargetTypeDef",
     "S3DirectTargetTypeDef",
     "S3GlueParquetTargetTypeDef",
+    "S3HudiDirectTargetTypeDef",
     "EncryptionConfigurationTypeDef",
     "SchemaVersionErrorItemTypeDef",
     "FilterExpressionTypeDef",
     "TransformParametersTypeDef",
-    "GetClassifiersRequestGetClassifiersPaginateTypeDef",
-    "GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef",
-    "GetCrawlersRequestGetCrawlersPaginateTypeDef",
-    "GetDatabasesRequestGetDatabasesPaginateTypeDef",
-    "GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef",
-    "GetJobRunsRequestGetJobRunsPaginateTypeDef",
-    "GetJobsRequestGetJobsPaginateTypeDef",
-    "GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef",
-    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    "GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef",
-    "GetTableVersionsRequestGetTableVersionsPaginateTypeDef",
-    "GetTablesRequestGetTablesPaginateTypeDef",
-    "GetTriggersRequestGetTriggersPaginateTypeDef",
-    "GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef",
-    "ListRegistriesInputListRegistriesPaginateTypeDef",
-    "ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
-    "ListSchemasInputListSchemasPaginateTypeDef",
     "GetConnectionsRequestGetConnectionsPaginateTypeDef",
     "GetConnectionsRequestRequestTypeDef",
     "GetJobBookmarkResponseTypeDef",
     "ResetJobBookmarkResponseTypeDef",
     "GetMLTaskRunsRequestRequestTypeDef",
     "TransformFilterCriteriaTypeDef",
     "GetMappingResponseTypeDef",
@@ -556,14 +601,16 @@
     "RemoveSchemaVersionMetadataInputRequestTypeDef",
     "RedshiftTargetTypeDef",
     "UserDefinedFunctionInputTypeDef",
     "UserDefinedFunctionTypeDef",
     "SearchTablesRequestRequestTypeDef",
     "StatementOutputTypeDef",
     "UpdateClassifierRequestRequestTypeDef",
+    "AmazonRedshiftSourceTypeDef",
+    "AmazonRedshiftTargetTypeDef",
     "PartitionIndexDescriptorTypeDef",
     "BatchStopJobRunResponseTypeDef",
     "BatchUpdatePartitionResponseTypeDef",
     "BatchCreatePartitionResponseTypeDef",
     "BatchDeletePartitionResponseTypeDef",
     "BatchDeleteTableResponseTypeDef",
     "BatchDeleteTableVersionResponseTypeDef",
@@ -582,14 +629,28 @@
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "GetConnectionResponseTypeDef",
     "GetConnectionsResponseTypeDef",
     "CrawlerTypeDef",
     "CreateCrawlerRequestRequestTypeDef",
     "UpdateCrawlerRequestRequestTypeDef",
+    "ListDataQualityRulesetsRequestRequestTypeDef",
+    "ListDataQualityRulesetsResponseTypeDef",
+    "DataQualityResultDescriptionTypeDef",
+    "DataQualityResultFilterCriteriaTypeDef",
+    "DataQualityResultTypeDef",
+    "DataQualityRuleRecommendationRunDescriptionTypeDef",
+    "DataQualityRuleRecommendationRunFilterTypeDef",
+    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
+    "DataQualityRulesetEvaluationRunFilterTypeDef",
+    "GetDataQualityResultResponseTypeDef",
+    "GetDataQualityRuleRecommendationRunResponseTypeDef",
+    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
+    "StartDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    "StartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     "CreateSessionResponseTypeDef",
     "GetSessionResponseTypeDef",
     "ListSessionsResponseTypeDef",
     "GetDataCatalogEncryptionSettingsResponseTypeDef",
     "PutDataCatalogEncryptionSettingsRequestRequestTypeDef",
     "DatabaseInputTypeDef",
     "DatabaseTypeDef",
@@ -600,18 +661,25 @@
     "SecurityConfigurationTypeDef",
     "DeleteSchemaVersionsResponseTypeDef",
     "FilterTypeDef",
     "UpdateMLTransformRequestRequestTypeDef",
     "GetMLTransformsRequestRequestTypeDef",
     "ListMLTransformsRequestRequestTypeDef",
     "AthenaConnectorSourceTypeDef",
+    "CatalogDeltaSourceTypeDef",
+    "CatalogHudiSourceTypeDef",
     "CustomCodeTypeDef",
+    "DynamicTransformTypeDef",
     "JDBCConnectorSourceTypeDef",
     "JDBCConnectorTargetTypeDef",
+    "S3CatalogDeltaSourceTypeDef",
+    "S3CatalogHudiSourceTypeDef",
     "S3CsvSourceTypeDef",
+    "S3DeltaSourceTypeDef",
+    "S3HudiSourceTypeDef",
     "S3JsonSourceTypeDef",
     "S3ParquetSourceTypeDef",
     "SparkConnectorSourceTypeDef",
     "SparkConnectorTargetTypeDef",
     "SparkSQLTypeDef",
     "GetJobRunResponseTypeDef",
     "GetJobRunsResponseTypeDef",
@@ -633,14 +701,21 @@
     "UpdateTriggerResponseTypeDef",
     "UpdateTriggerRequestRequestTypeDef",
     "GetMLTransformResponseTypeDef",
     "MLTransformTypeDef",
     "BatchGetCrawlersResponseTypeDef",
     "GetCrawlerResponseTypeDef",
     "GetCrawlersResponseTypeDef",
+    "ListDataQualityResultsResponseTypeDef",
+    "ListDataQualityResultsRequestRequestTypeDef",
+    "BatchGetDataQualityResultResponseTypeDef",
+    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
+    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
+    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
+    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
     "CreateDatabaseRequestRequestTypeDef",
     "UpdateDatabaseRequestRequestTypeDef",
     "GetDatabaseResponseTypeDef",
     "GetDatabasesResponseTypeDef",
     "ColumnStatisticsTypeDef",
     "PartitionInputTypeDef",
     "PartitionTypeDef",
@@ -709,14 +784,33 @@
     "AggregateOperationTypeDef",
     {
         "Column": List[str],
         "AggFunc": AggFunctionType,
     },
 )
 
+AmazonRedshiftAdvancedOptionTypeDef = TypedDict(
+    "AmazonRedshiftAdvancedOptionTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
+OptionTypeDef = TypedDict(
+    "OptionTypeDef",
+    {
+        "Value": str,
+        "Label": str,
+        "Description": str,
+    },
+    total=False,
+)
+
 ApplyMappingTypeDef = TypedDict(
     "ApplyMappingTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Mapping": List["MappingTypeDef"],
     },
@@ -745,25 +839,14 @@
         "Name": str,
         "Inputs": List[str],
         "Database": str,
         "Table": str,
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
 _RequiredBatchDeleteConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionNameList": Sequence[str],
     },
 )
 _OptionalBatchDeleteConnectionRequestRequestTypeDef = TypedDict(
@@ -881,14 +964,21 @@
     },
     total=False,
 )
 
 class CustomEntityTypeTypeDef(_RequiredCustomEntityTypeTypeDef, _OptionalCustomEntityTypeTypeDef):
     pass
 
+BatchGetDataQualityResultRequestRequestTypeDef = TypedDict(
+    "BatchGetDataQualityResultRequestRequestTypeDef",
+    {
+        "ResultIds": Sequence[str],
+    },
+)
+
 BatchGetDevEndpointsRequestRequestTypeDef = TypedDict(
     "BatchGetDevEndpointsRequestRequestTypeDef",
     {
         "DevEndpointNames": Sequence[str],
     },
 )
 
@@ -1026,22 +1116,46 @@
     {
         "NumberOfTrues": int,
         "NumberOfFalses": int,
         "NumberOfNulls": int,
     },
 )
 
+CancelDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
+    "CancelDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    {
+        "RunId": str,
+    },
+)
+
+CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
+    "CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef",
+    {
+        "RunId": str,
+    },
+)
+
 CancelMLTaskRunRequestRequestTypeDef = TypedDict(
     "CancelMLTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
         "TaskRunId": str,
     },
 )
 
+CancelMLTaskRunResponseTypeDef = TypedDict(
+    "CancelMLTaskRunResponseTypeDef",
+    {
+        "TransformId": str,
+        "TaskRunId": str,
+        "Status": TaskStatusTypeType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCancelStatementRequestRequestTypeDef = TypedDict(
     "_RequiredCancelStatementRequestRequestTypeDef",
     {
         "SessionId": str,
         "Id": int,
     },
 )
@@ -1090,14 +1204,18 @@
         "StartingOffsets": str,
         "EndingOffsets": str,
         "PollTimeoutMs": int,
         "NumRetries": int,
         "RetryIntervalMs": int,
         "MaxOffsetsPerTrigger": int,
         "MinPartitions": int,
+        "IncludeHeaders": bool,
+        "AddRecordTimestamp": str,
+        "EmitConsumerLagMetrics": str,
+        "StartingTimestamp": datetime,
     },
     total=False,
 )
 
 StreamingDataPreviewOptionsTypeDef = TypedDict(
     "StreamingDataPreviewOptionsTypeDef",
     {
@@ -1124,14 +1242,17 @@
         "NumRetries": int,
         "RetryIntervalMs": int,
         "MaxRetryIntervalMs": int,
         "AvoidEmptyBatches": bool,
         "StreamArn": str,
         "RoleArn": str,
         "RoleSessionName": str,
+        "AddRecordTimestamp": str,
+        "EmitConsumerLagMetrics": str,
+        "StartingTimestamp": datetime,
     },
     total=False,
 )
 
 CatalogSchemaChangePolicyTypeDef = TypedDict(
     "CatalogSchemaChangePolicyTypeDef",
     {
@@ -1174,14 +1295,23 @@
     "CheckSchemaVersionValidityInputRequestTypeDef",
     {
         "DataFormat": DataFormatType,
         "SchemaDefinition": str,
     },
 )
 
+CheckSchemaVersionValidityResponseTypeDef = TypedDict(
+    "CheckSchemaVersionValidityResponseTypeDef",
+    {
+        "Valid": bool,
+        "Error": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCsvClassifierTypeDef = TypedDict(
     "_RequiredCsvClassifierTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCsvClassifierTypeDef = TypedDict(
@@ -1273,14 +1403,35 @@
     {
         "CloudWatchEncryptionMode": CloudWatchEncryptionModeType,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
+_RequiredDirectJDBCSourceTypeDef = TypedDict(
+    "_RequiredDirectJDBCSourceTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+        "ConnectionName": str,
+        "ConnectionType": JDBCConnectionTypeType,
+    },
+)
+_OptionalDirectJDBCSourceTypeDef = TypedDict(
+    "_OptionalDirectJDBCSourceTypeDef",
+    {
+        "RedshiftTmpDir": str,
+    },
+    total=False,
+)
+
+class DirectJDBCSourceTypeDef(_RequiredDirectJDBCSourceTypeDef, _OptionalDirectJDBCSourceTypeDef):
+    pass
+
 _RequiredDropDuplicatesTypeDef = TypedDict(
     "_RequiredDropDuplicatesTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
     },
 )
@@ -1791,34 +1942,47 @@
 
 DeltaTargetTypeDef = TypedDict(
     "DeltaTargetTypeDef",
     {
         "DeltaTables": List[str],
         "ConnectionName": str,
         "WriteManifest": bool,
+        "CreateNativeDeltaTable": bool,
     },
     total=False,
 )
 
 DynamoDBTargetTypeDef = TypedDict(
     "DynamoDBTargetTypeDef",
     {
         "Path": str,
         "scanAll": bool,
         "scanRate": float,
     },
     total=False,
 )
 
+IcebergTargetTypeDef = TypedDict(
+    "IcebergTargetTypeDef",
+    {
+        "Paths": List[str],
+        "ConnectionName": str,
+        "Exclusions": List[str],
+        "MaximumTraversalDepth": int,
+    },
+    total=False,
+)
+
 JdbcTargetTypeDef = TypedDict(
     "JdbcTargetTypeDef",
     {
         "ConnectionName": str,
         "Path": str,
         "Exclusions": List[str],
+        "EnableAdditionalMetadata": List[JdbcMetadataEntryType],
     },
     total=False,
 )
 
 MongoDBTargetTypeDef = TypedDict(
     "MongoDBTargetTypeDef",
     {
@@ -1925,14 +2089,22 @@
 )
 
 class CreateBlueprintRequestRequestTypeDef(
     _RequiredCreateBlueprintRequestRequestTypeDef, _OptionalCreateBlueprintRequestRequestTypeDef
 ):
     pass
 
+CreateBlueprintResponseTypeDef = TypedDict(
+    "CreateBlueprintResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredCreateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateCsvClassifierRequestTypeDef = TypedDict(
@@ -2011,24 +2183,61 @@
         "RegexString": str,
     },
 )
 _OptionalCreateCustomEntityTypeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCustomEntityTypeRequestRequestTypeDef",
     {
         "ContextWords": Sequence[str],
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateCustomEntityTypeRequestRequestTypeDef(
     _RequiredCreateCustomEntityTypeRequestRequestTypeDef,
     _OptionalCreateCustomEntityTypeRequestRequestTypeDef,
 ):
     pass
 
+CreateCustomEntityTypeResponseTypeDef = TypedDict(
+    "CreateCustomEntityTypeResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredDataQualityTargetTableTypeDef = TypedDict(
+    "_RequiredDataQualityTargetTableTypeDef",
+    {
+        "TableName": str,
+        "DatabaseName": str,
+    },
+)
+_OptionalDataQualityTargetTableTypeDef = TypedDict(
+    "_OptionalDataQualityTargetTableTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class DataQualityTargetTableTypeDef(
+    _RequiredDataQualityTargetTableTypeDef, _OptionalDataQualityTargetTableTypeDef
+):
+    pass
+
+CreateDataQualityRulesetResponseTypeDef = TypedDict(
+    "CreateDataQualityRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateDevEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
         "RoleArn": str,
     },
 )
@@ -2053,28 +2262,55 @@
 )
 
 class CreateDevEndpointRequestRequestTypeDef(
     _RequiredCreateDevEndpointRequestRequestTypeDef, _OptionalCreateDevEndpointRequestRequestTypeDef
 ):
     pass
 
+CreateDevEndpointResponseTypeDef = TypedDict(
+    "CreateDevEndpointResponseTypeDef",
+    {
+        "EndpointName": str,
+        "Status": str,
+        "SecurityGroupIds": List[str],
+        "SubnetId": str,
+        "RoleArn": str,
+        "YarnEndpointAddress": str,
+        "ZeppelinRemoteSparkInterpreterPort": int,
+        "NumberOfNodes": int,
+        "WorkerType": WorkerTypeType,
+        "GlueVersion": str,
+        "NumberOfWorkers": int,
+        "AvailabilityZone": str,
+        "VpcId": str,
+        "ExtraPythonLibsS3Path": str,
+        "ExtraJarsS3Path": str,
+        "FailureReason": str,
+        "SecurityConfiguration": str,
+        "CreatedTimestamp": datetime,
+        "Arguments": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExecutionPropertyTypeDef = TypedDict(
     "ExecutionPropertyTypeDef",
     {
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
 
 JobCommandTypeDef = TypedDict(
     "JobCommandTypeDef",
     {
         "Name": str,
         "ScriptLocation": str,
         "PythonVersion": str,
+        "Runtime": str,
     },
     total=False,
 )
 
 SourceControlDetailsTypeDef = TypedDict(
     "SourceControlDetailsTypeDef",
     {
@@ -2086,33 +2322,50 @@
         "LastCommitId": str,
         "AuthStrategy": SourceControlAuthStrategyType,
         "AuthToken": str,
     },
     total=False,
 )
 
+CreateJobResponseTypeDef = TypedDict(
+    "CreateJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGlueTableTypeDef = TypedDict(
     "_RequiredGlueTableTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
 _OptionalGlueTableTypeDef = TypedDict(
     "_OptionalGlueTableTypeDef",
     {
         "CatalogId": str,
         "ConnectionName": str,
+        "AdditionalOptions": Dict[str, str],
     },
     total=False,
 )
 
 class GlueTableTypeDef(_RequiredGlueTableTypeDef, _OptionalGlueTableTypeDef):
     pass
 
+CreateMLTransformResponseTypeDef = TypedDict(
+    "CreateMLTransformResponseTypeDef",
+    {
+        "TransformId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PartitionIndexTypeDef = TypedDict(
     "PartitionIndexTypeDef",
     {
         "Keys": Sequence[str],
         "IndexName": str,
     },
 )
@@ -2133,23 +2386,73 @@
 )
 
 class CreateRegistryInputRequestTypeDef(
     _RequiredCreateRegistryInputRequestTypeDef, _OptionalCreateRegistryInputRequestTypeDef
 ):
     pass
 
+CreateRegistryResponseTypeDef = TypedDict(
+    "CreateRegistryResponseTypeDef",
+    {
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RegistryIdTypeDef = TypedDict(
     "RegistryIdTypeDef",
     {
         "RegistryName": str,
         "RegistryArn": str,
     },
     total=False,
 )
 
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "RegistryName": str,
+        "RegistryArn": str,
+        "SchemaName": str,
+        "SchemaArn": str,
+        "Description": str,
+        "DataFormat": DataFormatType,
+        "Compatibility": CompatibilityType,
+        "SchemaCheckpoint": int,
+        "LatestSchemaVersion": int,
+        "NextSchemaVersion": int,
+        "SchemaStatus": SchemaStatusType,
+        "Tags": Dict[str, str],
+        "SchemaVersionId": str,
+        "SchemaVersionStatus": SchemaVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateScriptResponseTypeDef = TypedDict(
+    "CreateScriptResponseTypeDef",
+    {
+        "PythonScript": str,
+        "ScalaCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSecurityConfigurationResponseTypeDef = TypedDict(
+    "CreateSecurityConfigurationResponseTypeDef",
+    {
+        "Name": str,
+        "CreatedTimestamp": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SessionCommandTypeDef = TypedDict(
     "SessionCommandTypeDef",
     {
         "Name": str,
         "PythonVersion": str,
     },
     total=False,
@@ -2170,14 +2473,22 @@
 )
 
 class EventBatchingConditionTypeDef(
     _RequiredEventBatchingConditionTypeDef, _OptionalEventBatchingConditionTypeDef
 ):
     pass
 
+CreateTriggerResponseTypeDef = TypedDict(
+    "CreateTriggerResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
@@ -2192,14 +2503,41 @@
 )
 
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
 
+CreateWorkflowResponseTypeDef = TypedDict(
+    "CreateWorkflowResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DQResultsPublishingOptionsTypeDef = TypedDict(
+    "DQResultsPublishingOptionsTypeDef",
+    {
+        "EvaluationContext": str,
+        "ResultsS3Prefix": str,
+        "CloudWatchMetricsEnabled": bool,
+        "ResultsPublishingEnabled": bool,
+    },
+    total=False,
+)
+
+DQStopJobOnFailureOptionsTypeDef = TypedDict(
+    "DQStopJobOnFailureOptionsTypeDef",
+    {
+        "StopJobOnFailureTiming": DQStopJobOnFailureTimingType,
+    },
+    total=False,
+)
+
 _RequiredEncryptionAtRestTypeDef = TypedDict(
     "_RequiredEncryptionAtRestTypeDef",
     {
         "CatalogEncryptionMode": CatalogEncryptionModeType,
     },
 )
 _OptionalEncryptionAtRestTypeDef = TypedDict(
@@ -2217,19 +2555,50 @@
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
     total=False,
 )
 
+DataQualityEvaluationRunAdditionalRunOptionsTypeDef = TypedDict(
+    "DataQualityEvaluationRunAdditionalRunOptionsTypeDef",
+    {
+        "CloudWatchMetricsEnabled": bool,
+        "ResultsS3Prefix": str,
+    },
+    total=False,
+)
+
+DataQualityRuleResultTypeDef = TypedDict(
+    "DataQualityRuleResultTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "EvaluationMessage": str,
+        "Result": DataQualityRuleResultStatusType,
+        "EvaluatedMetrics": Dict[str, float],
+    },
+    total=False,
+)
+
 DatabaseIdentifierTypeDef = TypedDict(
     "DatabaseIdentifierTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
+        "Region": str,
+    },
+    total=False,
+)
+
+FederatedDatabaseTypeDef = TypedDict(
+    "FederatedDatabaseTypeDef",
+    {
+        "Identifier": str,
+        "ConnectionName": str,
     },
     total=False,
 )
 
 DatatypeTypeDef = TypedDict(
     "DatatypeTypeDef",
     {
@@ -2249,14 +2618,22 @@
 DeleteBlueprintRequestRequestTypeDef = TypedDict(
     "DeleteBlueprintRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteBlueprintResponseTypeDef = TypedDict(
+    "DeleteBlueprintResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteClassifierRequestRequestTypeDef = TypedDict(
     "DeleteClassifierRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2334,14 +2711,29 @@
 DeleteCustomEntityTypeRequestRequestTypeDef = TypedDict(
     "DeleteCustomEntityTypeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteCustomEntityTypeResponseTypeDef = TypedDict(
+    "DeleteCustomEntityTypeResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteDataQualityRulesetRequestRequestTypeDef = TypedDict(
+    "DeleteDataQualityRulesetRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 _RequiredDeleteDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDatabaseRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDeleteDatabaseRequestRequestTypeDef = TypedDict(
@@ -2367,21 +2759,37 @@
 DeleteJobRequestRequestTypeDef = TypedDict(
     "DeleteJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 
+DeleteJobResponseTypeDef = TypedDict(
+    "DeleteJobResponseTypeDef",
+    {
+        "JobName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteMLTransformRequestRequestTypeDef = TypedDict(
     "DeleteMLTransformRequestRequestTypeDef",
     {
         "TransformId": str,
     },
 )
 
+DeleteMLTransformResponseTypeDef = TypedDict(
+    "DeleteMLTransformResponseTypeDef",
+    {
+        "TransformId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeletePartitionIndexRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePartitionIndexRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "IndexName": str,
     },
@@ -2417,14 +2825,24 @@
 )
 
 class DeletePartitionRequestRequestTypeDef(
     _RequiredDeletePartitionRequestRequestTypeDef, _OptionalDeletePartitionRequestRequestTypeDef
 ):
     pass
 
+DeleteRegistryResponseTypeDef = TypedDict(
+    "DeleteRegistryResponseTypeDef",
+    {
+        "RegistryName": str,
+        "RegistryArn": str,
+        "Status": RegistryStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyHashCondition": str,
         "ResourceArn": str,
     },
     total=False,
@@ -2436,14 +2854,24 @@
         "SchemaArn": str,
         "SchemaName": str,
         "RegistryName": str,
     },
     total=False,
 )
 
+DeleteSchemaResponseTypeDef = TypedDict(
+    "DeleteSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "SchemaName": str,
+        "Status": SchemaStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteSecurityConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteSecurityConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2462,14 +2890,22 @@
 )
 
 class DeleteSessionRequestRequestTypeDef(
     _RequiredDeleteSessionRequestRequestTypeDef, _OptionalDeleteSessionRequestRequestTypeDef
 ):
     pass
 
+DeleteSessionResponseTypeDef = TypedDict(
+    "DeleteSessionResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteTableRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -2512,14 +2948,22 @@
 DeleteTriggerRequestRequestTypeDef = TypedDict(
     "DeleteTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteTriggerResponseTypeDef = TypedDict(
+    "DeleteTriggerResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteUserDefinedFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteUserDefinedFunctionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "FunctionName": str,
     },
 )
@@ -2540,14 +2984,22 @@
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeleteWorkflowResponseTypeDef = TypedDict(
+    "DeleteWorkflowResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DevEndpointCustomLibrariesTypeDef = TypedDict(
     "DevEndpointCustomLibrariesTypeDef",
     {
         "ExtraPythonLibsS3Path": str,
         "ExtraJarsS3Path": str,
     },
     total=False,
@@ -2570,14 +3022,38 @@
         "IsEmpty": bool,
         "IsNullString": bool,
         "IsNegOne": bool,
     },
     total=False,
 )
 
+_RequiredTransformConfigParameterTypeDef = TypedDict(
+    "_RequiredTransformConfigParameterTypeDef",
+    {
+        "Name": str,
+        "Type": ParamTypeType,
+    },
+)
+_OptionalTransformConfigParameterTypeDef = TypedDict(
+    "_OptionalTransformConfigParameterTypeDef",
+    {
+        "ValidationRule": str,
+        "ValidationMessage": str,
+        "Value": List[str],
+        "ListType": ParamTypeType,
+        "IsOptional": bool,
+    },
+    total=False,
+)
+
+class TransformConfigParameterTypeDef(
+    _RequiredTransformConfigParameterTypeDef, _OptionalTransformConfigParameterTypeDef
+):
+    pass
+
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "SourceId": str,
         "DestinationId": str,
     },
     total=False,
@@ -2614,14 +3090,24 @@
     "ExportLabelsTaskRunPropertiesTypeDef",
     {
         "OutputS3Path": str,
     },
     total=False,
 )
 
+FederatedTableTypeDef = TypedDict(
+    "FederatedTableTypeDef",
+    {
+        "Identifier": str,
+        "DatabaseIdentifier": str,
+        "ConnectionName": str,
+    },
+    total=False,
+)
+
 FilterValueTypeDef = TypedDict(
     "FilterValueTypeDef",
     {
         "Type": FilterValueTypeType,
         "Value": List[str],
     },
 )
@@ -2706,20 +3192,18 @@
 GetClassifierRequestRequestTypeDef = TypedDict(
     "GetClassifierRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetClassifiersRequestGetClassifiersPaginateTypeDef = TypedDict(
+    "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetClassifiersRequestRequestTypeDef = TypedDict(
     "GetClassifiersRequestRequestTypeDef",
     {
@@ -2799,14 +3283,23 @@
     {
         "MatchCriteria": Sequence[str],
         "ConnectionType": ConnectionTypeType,
     },
     total=False,
 )
 
+GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef = TypedDict(
+    "GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef",
+    {
+        "CrawlerNameList": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetCrawlerMetricsRequestRequestTypeDef = TypedDict(
     "GetCrawlerMetricsRequestRequestTypeDef",
     {
         "CrawlerNameList": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -2816,14 +3309,22 @@
 GetCrawlerRequestRequestTypeDef = TypedDict(
     "GetCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+GetCrawlersRequestGetCrawlersPaginateTypeDef = TypedDict(
+    "GetCrawlersRequestGetCrawlersPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetCrawlersRequestRequestTypeDef = TypedDict(
     "GetCrawlersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -2832,22 +3333,60 @@
 GetCustomEntityTypeRequestRequestTypeDef = TypedDict(
     "GetCustomEntityTypeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+GetCustomEntityTypeResponseTypeDef = TypedDict(
+    "GetCustomEntityTypeResponseTypeDef",
+    {
+        "Name": str,
+        "RegexString": str,
+        "ContextWords": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDataCatalogEncryptionSettingsRequestRequestTypeDef = TypedDict(
     "GetDataCatalogEncryptionSettingsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+GetDataQualityResultRequestRequestTypeDef = TypedDict(
+    "GetDataQualityResultRequestRequestTypeDef",
+    {
+        "ResultId": str,
+    },
+)
+
+GetDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
+    "GetDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    {
+        "RunId": str,
+    },
+)
+
+GetDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
+    "GetDataQualityRulesetEvaluationRunRequestRequestTypeDef",
+    {
+        "RunId": str,
+    },
+)
+
+GetDataQualityRulesetRequestRequestTypeDef = TypedDict(
+    "GetDataQualityRulesetRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 _RequiredGetDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredGetDatabaseRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetDatabaseRequestRequestTypeDef = TypedDict(
@@ -2859,14 +3398,24 @@
 )
 
 class GetDatabaseRequestRequestTypeDef(
     _RequiredGetDatabaseRequestRequestTypeDef, _OptionalGetDatabaseRequestRequestTypeDef
 ):
     pass
 
+GetDatabasesRequestGetDatabasesPaginateTypeDef = TypedDict(
+    "GetDatabasesRequestGetDatabasesPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceShareType": ResourceShareTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetDatabasesRequestRequestTypeDef = TypedDict(
     "GetDatabasesRequestRequestTypeDef",
     {
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
         "ResourceShareType": ResourceShareTypeType,
@@ -2885,14 +3434,22 @@
 GetDevEndpointRequestRequestTypeDef = TypedDict(
     "GetDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
 
+GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef = TypedDict(
+    "GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetDevEndpointsRequestRequestTypeDef = TypedDict(
     "GetDevEndpointsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -2954,14 +3511,34 @@
 )
 
 class GetJobRunRequestRequestTypeDef(
     _RequiredGetJobRunRequestRequestTypeDef, _OptionalGetJobRunRequestRequestTypeDef
 ):
     pass
 
+_RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef",
+    {
+        "JobName": str,
+    },
+)
+_OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetJobRunsRequestGetJobRunsPaginateTypeDef(
+    _RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef,
+    _OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJobRunsRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 _OptionalGetJobRunsRequestRequestTypeDef = TypedDict(
@@ -2974,14 +3551,22 @@
 )
 
 class GetJobRunsRequestRequestTypeDef(
     _RequiredGetJobRunsRequestRequestTypeDef, _OptionalGetJobRunsRequestRequestTypeDef
 ):
     pass
 
+GetJobsRequestGetJobsPaginateTypeDef = TypedDict(
+    "GetJobsRequestGetJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetJobsRequestRequestTypeDef = TypedDict(
     "GetJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -3047,14 +3632,36 @@
         "TargetTable": str,
         "TargetPath": str,
         "TargetType": str,
     },
     total=False,
 )
 
+_RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef = TypedDict(
+    "_RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+    },
+)
+_OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef = TypedDict(
+    "_OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef(
+    _RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
+    _OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
+):
+    pass
+
 _RequiredGetPartitionIndexesRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionIndexesRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3098,14 +3705,44 @@
     "SegmentTypeDef",
     {
         "SegmentNumber": int,
         "TotalSegments": int,
     },
 )
 
+GetPlanResponseTypeDef = TypedDict(
+    "GetPlanResponseTypeDef",
+    {
+        "PythonScript": str,
+        "ScalaCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetRegistryResponseTypeDef = TypedDict(
+    "GetRegistryResponseTypeDef",
+    {
+        "RegistryName": str,
+        "RegistryArn": str,
+        "Description": str,
+        "Status": RegistryStatusType,
+        "CreatedTime": str,
+        "UpdatedTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "GetResourcePoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -3126,30 +3763,103 @@
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
     total=False,
 )
 
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "PolicyInJson": str,
+        "PolicyHash": str,
+        "CreateTime": datetime,
+        "UpdateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSchemaByDefinitionResponseTypeDef = TypedDict(
+    "GetSchemaByDefinitionResponseTypeDef",
+    {
+        "SchemaVersionId": str,
+        "SchemaArn": str,
+        "DataFormat": DataFormatType,
+        "Status": SchemaVersionStatusType,
+        "CreatedTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSchemaResponseTypeDef = TypedDict(
+    "GetSchemaResponseTypeDef",
+    {
+        "RegistryName": str,
+        "RegistryArn": str,
+        "SchemaName": str,
+        "SchemaArn": str,
+        "Description": str,
+        "DataFormat": DataFormatType,
+        "Compatibility": CompatibilityType,
+        "SchemaCheckpoint": int,
+        "LatestSchemaVersion": int,
+        "NextSchemaVersion": int,
+        "SchemaStatus": SchemaStatusType,
+        "CreatedTime": str,
+        "UpdatedTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SchemaVersionNumberTypeDef = TypedDict(
     "SchemaVersionNumberTypeDef",
     {
         "LatestVersion": bool,
         "VersionNumber": int,
     },
     total=False,
 )
 
+GetSchemaVersionResponseTypeDef = TypedDict(
+    "GetSchemaVersionResponseTypeDef",
+    {
+        "SchemaVersionId": str,
+        "SchemaDefinition": str,
+        "DataFormat": DataFormatType,
+        "SchemaArn": str,
+        "VersionNumber": int,
+        "Status": SchemaVersionStatusType,
+        "CreatedTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetSchemaVersionsDiffResponseTypeDef = TypedDict(
+    "GetSchemaVersionsDiffResponseTypeDef",
+    {
+        "Diff": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSecurityConfigurationRequestRequestTypeDef = TypedDict(
     "GetSecurityConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef = TypedDict(
+    "GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetSecurityConfigurationsRequestRequestTypeDef = TypedDict(
     "GetSecurityConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -3233,14 +3943,36 @@
 )
 
 class GetTableVersionRequestRequestTypeDef(
     _RequiredGetTableVersionRequestRequestTypeDef, _OptionalGetTableVersionRequestRequestTypeDef
 ):
     pass
 
+_RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+    },
+)
+_OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetTableVersionsRequestGetTableVersionsPaginateTypeDef(
+    _RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
+    _OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetTableVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableVersionsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3255,14 +3987,38 @@
 )
 
 class GetTableVersionsRequestRequestTypeDef(
     _RequiredGetTableVersionsRequestRequestTypeDef, _OptionalGetTableVersionsRequestRequestTypeDef
 ):
     pass
 
+_RequiredGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
+    "_RequiredGetTablesRequestGetTablesPaginateTypeDef",
+    {
+        "DatabaseName": str,
+    },
+)
+_OptionalGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
+    "_OptionalGetTablesRequestGetTablesPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "Expression": str,
+        "TransactionId": str,
+        "QueryAsOfTime": Union[datetime, str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetTablesRequestGetTablesPaginateTypeDef(
+    _RequiredGetTablesRequestGetTablesPaginateTypeDef,
+    _OptionalGetTablesRequestGetTablesPaginateTypeDef,
+):
+    pass
+
 _RequiredGetTablesRequestRequestTypeDef = TypedDict(
     "_RequiredGetTablesRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalGetTablesRequestRequestTypeDef = TypedDict(
@@ -3286,21 +4042,38 @@
 GetTagsRequestRequestTypeDef = TypedDict(
     "GetTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetTriggerRequestRequestTypeDef = TypedDict(
     "GetTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+GetTriggersRequestGetTriggersPaginateTypeDef = TypedDict(
+    "GetTriggersRequestGetTriggersPaginateTypeDef",
+    {
+        "DependentJobName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 GetTriggersRequestRequestTypeDef = TypedDict(
     "GetTriggersRequestRequestTypeDef",
     {
         "NextToken": str,
         "DependentJobName": str,
         "MaxResults": int,
     },
@@ -3324,14 +4097,36 @@
 
 class GetUserDefinedFunctionRequestRequestTypeDef(
     _RequiredGetUserDefinedFunctionRequestRequestTypeDef,
     _OptionalGetUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
+_RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef = TypedDict(
+    "_RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef",
+    {
+        "Pattern": str,
+    },
+)
+_OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef = TypedDict(
+    "_OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "DatabaseName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef(
+    _RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
+    _OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetUserDefinedFunctionsRequestRequestTypeDef",
     {
         "Pattern": str,
     },
 )
 _OptionalGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
@@ -3374,14 +4169,22 @@
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
 
+GetWorkflowRunPropertiesResponseTypeDef = TypedDict(
+    "GetWorkflowRunPropertiesResponseTypeDef",
+    {
+        "RunProperties": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetWorkflowRunRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
@@ -3518,53 +4321,107 @@
         "NextToken": str,
         "MaxResults": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+ListBlueprintsResponseTypeDef = TypedDict(
+    "ListBlueprintsResponseTypeDef",
+    {
+        "Blueprints": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListCrawlersRequestRequestTypeDef = TypedDict(
     "ListCrawlersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+ListCrawlersResponseTypeDef = TypedDict(
+    "ListCrawlersResponseTypeDef",
+    {
+        "CrawlerNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListCustomEntityTypesRequestRequestTypeDef = TypedDict(
     "ListCustomEntityTypesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 ListDevEndpointsRequestRequestTypeDef = TypedDict(
     "ListDevEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+ListDevEndpointsResponseTypeDef = TypedDict(
+    "ListDevEndpointsResponseTypeDef",
+    {
+        "DevEndpointNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+ListJobsResponseTypeDef = TypedDict(
+    "ListJobsResponseTypeDef",
+    {
+        "JobNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListMLTransformsResponseTypeDef = TypedDict(
+    "ListMLTransformsResponseTypeDef",
+    {
+        "TransformIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListRegistriesInputListRegistriesPaginateTypeDef = TypedDict(
+    "ListRegistriesInputListRegistriesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListRegistriesInputRequestTypeDef = TypedDict(
     "ListRegistriesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -3647,23 +4504,41 @@
         "DependentJobName": str,
         "MaxResults": int,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+ListTriggersResponseTypeDef = TypedDict(
+    "ListTriggersResponseTypeDef",
+    {
+        "TriggerNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListWorkflowsRequestRequestTypeDef = TypedDict(
     "ListWorkflowsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListWorkflowsResponseTypeDef = TypedDict(
+    "ListWorkflowsResponseTypeDef",
+    {
+        "Workflows": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredMLUserDataEncryptionTypeDef = TypedDict(
     "_RequiredMLUserDataEncryptionTypeDef",
     {
         "MlUserDataEncryptionMode": MLUserDataEncryptionModeStringType,
     },
 )
 _OptionalMLUserDataEncryptionTypeDef = TypedDict(
@@ -3714,14 +4589,24 @@
     "OrderTypeDef",
     {
         "Column": str,
         "SortOrder": int,
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
 PropertyPredicateTypeDef = TypedDict(
     "PropertyPredicateTypeDef",
     {
         "Key": str,
         "Value": str,
         "Comparator": ComparatorType,
     },
@@ -3746,14 +4631,37 @@
 )
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "PolicyHash": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutSchemaVersionMetadataResponseTypeDef = TypedDict(
+    "PutSchemaVersionMetadataResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "SchemaName": str,
+        "RegistryName": str,
+        "LatestVersion": bool,
+        "VersionNumber": int,
+        "SchemaVersionId": str,
+        "MetadataKey": str,
+        "MetadataValue": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutWorkflowRunPropertiesRequestRequestTypeDef = TypedDict(
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
         "RunProperties": Mapping[str, str],
     },
@@ -3765,14 +4673,39 @@
         "TableLocation": str,
         "ConnectionName": str,
         "UpsertKeys": List[str],
     },
     total=False,
 )
 
+RegisterSchemaVersionResponseTypeDef = TypedDict(
+    "RegisterSchemaVersionResponseTypeDef",
+    {
+        "SchemaVersionId": str,
+        "VersionNumber": int,
+        "Status": SchemaVersionStatusType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RemoveSchemaVersionMetadataResponseTypeDef = TypedDict(
+    "RemoveSchemaVersionMetadataResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "SchemaName": str,
+        "RegistryName": str,
+        "LatestVersion": bool,
+        "VersionNumber": int,
+        "SchemaVersionId": str,
+        "MetadataKey": str,
+        "MetadataValue": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredResetJobBookmarkRequestRequestTypeDef = TypedDict(
     "_RequiredResetJobBookmarkRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 _OptionalResetJobBookmarkRequestRequestTypeDef = TypedDict(
@@ -3793,23 +4726,43 @@
     {
         "ResourceType": ResourceTypeType,
         "Uri": str,
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
 ResumeWorkflowRunRequestRequestTypeDef = TypedDict(
     "ResumeWorkflowRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
         "NodeIds": Sequence[str],
     },
 )
 
+ResumeWorkflowRunResponseTypeDef = TypedDict(
+    "ResumeWorkflowRunResponseTypeDef",
+    {
+        "RunId": str,
+        "NodeIds": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRunStatementRequestRequestTypeDef = TypedDict(
     "_RequiredRunStatementRequestRequestTypeDef",
     {
         "SessionId": str,
         "Code": str,
     },
 )
@@ -3822,14 +4775,22 @@
 )
 
 class RunStatementRequestRequestTypeDef(
     _RequiredRunStatementRequestRequestTypeDef, _OptionalRunStatementRequestRequestTypeDef
 ):
     pass
 
+RunStatementResponseTypeDef = TypedDict(
+    "RunStatementResponseTypeDef",
+    {
+        "Id": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 S3DirectSourceAdditionalOptionsTypeDef = TypedDict(
     "S3DirectSourceAdditionalOptionsTypeDef",
     {
         "BoundedSize": int,
         "BoundedFiles": int,
         "EnableSamplePath": bool,
         "SamplePath": str,
@@ -3890,36 +4851,68 @@
 )
 
 class StartBlueprintRunRequestRequestTypeDef(
     _RequiredStartBlueprintRunRequestRequestTypeDef, _OptionalStartBlueprintRunRequestRequestTypeDef
 ):
     pass
 
+StartBlueprintRunResponseTypeDef = TypedDict(
+    "StartBlueprintRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartCrawlerRequestRequestTypeDef = TypedDict(
     "StartCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 StartCrawlerScheduleRequestRequestTypeDef = TypedDict(
     "StartCrawlerScheduleRequestRequestTypeDef",
     {
         "CrawlerName": str,
     },
 )
 
+StartDataQualityRuleRecommendationRunResponseTypeDef = TypedDict(
+    "StartDataQualityRuleRecommendationRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartDataQualityRulesetEvaluationRunResponseTypeDef = TypedDict(
+    "StartDataQualityRulesetEvaluationRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartExportLabelsTaskRunRequestRequestTypeDef = TypedDict(
     "StartExportLabelsTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
         "OutputS3Path": str,
     },
 )
 
+StartExportLabelsTaskRunResponseTypeDef = TypedDict(
+    "StartExportLabelsTaskRunResponseTypeDef",
+    {
+        "TaskRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartImportLabelsTaskRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportLabelsTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
         "InputS3Path": str,
     },
 )
@@ -3933,36 +4926,76 @@
 
 class StartImportLabelsTaskRunRequestRequestTypeDef(
     _RequiredStartImportLabelsTaskRunRequestRequestTypeDef,
     _OptionalStartImportLabelsTaskRunRequestRequestTypeDef,
 ):
     pass
 
+StartImportLabelsTaskRunResponseTypeDef = TypedDict(
+    "StartImportLabelsTaskRunResponseTypeDef",
+    {
+        "TaskRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
+    {
+        "JobRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartMLEvaluationTaskRunRequestRequestTypeDef = TypedDict(
     "StartMLEvaluationTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
     },
 )
 
+StartMLEvaluationTaskRunResponseTypeDef = TypedDict(
+    "StartMLEvaluationTaskRunResponseTypeDef",
+    {
+        "TaskRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef = TypedDict(
     "StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
         "OutputS3Path": str,
     },
 )
 
+StartMLLabelingSetGenerationTaskRunResponseTypeDef = TypedDict(
+    "StartMLLabelingSetGenerationTaskRunResponseTypeDef",
+    {
+        "TaskRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartTriggerRequestRequestTypeDef = TypedDict(
     "StartTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+StartTriggerResponseTypeDef = TypedDict(
+    "StartTriggerResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartWorkflowRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartWorkflowRunRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalStartWorkflowRunRequestRequestTypeDef = TypedDict(
@@ -3974,14 +5007,22 @@
 )
 
 class StartWorkflowRunRequestRequestTypeDef(
     _RequiredStartWorkflowRunRequestRequestTypeDef, _OptionalStartWorkflowRunRequestRequestTypeDef
 ):
     pass
 
+StartWorkflowRunResponseTypeDef = TypedDict(
+    "StartWorkflowRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StartingEventBatchConditionTypeDef = TypedDict(
     "StartingEventBatchConditionTypeDef",
     {
         "BatchSize": int,
         "BatchWindow": int,
     },
     total=False,
@@ -4024,35 +5065,52 @@
 )
 
 class StopSessionRequestRequestTypeDef(
     _RequiredStopSessionRequestRequestTypeDef, _OptionalStopSessionRequestRequestTypeDef
 ):
     pass
 
+StopSessionResponseTypeDef = TypedDict(
+    "StopSessionResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopTriggerRequestRequestTypeDef = TypedDict(
     "StopTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+StopTriggerResponseTypeDef = TypedDict(
+    "StopTriggerResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopWorkflowRunRequestRequestTypeDef = TypedDict(
     "StopWorkflowRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
 
 TableIdentifierTypeDef = TypedDict(
     "TableIdentifierTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
+        "Region": str,
     },
     total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
@@ -4085,14 +5143,22 @@
 )
 
 class UpdateBlueprintRequestRequestTypeDef(
     _RequiredUpdateBlueprintRequestRequestTypeDef, _OptionalUpdateBlueprintRequestRequestTypeDef
 ):
     pass
 
+UpdateBlueprintResponseTypeDef = TypedDict(
+    "UpdateBlueprintResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCsvClassifierRequestTypeDef = TypedDict(
@@ -4191,14 +5257,45 @@
 
 class UpdateCrawlerScheduleRequestRequestTypeDef(
     _RequiredUpdateCrawlerScheduleRequestRequestTypeDef,
     _OptionalUpdateCrawlerScheduleRequestRequestTypeDef,
 ):
     pass
 
+_RequiredUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDataQualityRulesetRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDataQualityRulesetRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Ruleset": str,
+    },
+    total=False,
+)
+
+class UpdateDataQualityRulesetRequestRequestTypeDef(
+    _RequiredUpdateDataQualityRulesetRequestRequestTypeDef,
+    _OptionalUpdateDataQualityRulesetRequestRequestTypeDef,
+):
+    pass
+
+UpdateDataQualityRulesetResponseTypeDef = TypedDict(
+    "UpdateDataQualityRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Ruleset": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateJobFromSourceControlRequestRequestTypeDef = TypedDict(
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     {
         "JobName": str,
         "Provider": SourceControlProviderType,
         "RepositoryName": str,
         "RepositoryOwner": str,
@@ -4207,14 +5304,57 @@
         "CommitId": str,
         "AuthStrategy": SourceControlAuthStrategyType,
         "AuthToken": str,
     },
     total=False,
 )
 
+UpdateJobFromSourceControlResponseTypeDef = TypedDict(
+    "UpdateJobFromSourceControlResponseTypeDef",
+    {
+        "JobName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateJobResponseTypeDef = TypedDict(
+    "UpdateJobResponseTypeDef",
+    {
+        "JobName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateMLTransformResponseTypeDef = TypedDict(
+    "UpdateMLTransformResponseTypeDef",
+    {
+        "TransformId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateRegistryResponseTypeDef = TypedDict(
+    "UpdateRegistryResponseTypeDef",
+    {
+        "RegistryName": str,
+        "RegistryArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateSchemaResponseTypeDef = TypedDict(
+    "UpdateSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "SchemaName": str,
+        "RegistryName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateSourceControlFromJobRequestRequestTypeDef = TypedDict(
     "UpdateSourceControlFromJobRequestRequestTypeDef",
     {
         "JobName": str,
         "Provider": SourceControlProviderType,
         "RepositoryName": str,
         "RepositoryOwner": str,
@@ -4223,14 +5363,22 @@
         "CommitId": str,
         "AuthStrategy": SourceControlAuthStrategyType,
         "AuthToken": str,
     },
     total=False,
 )
 
+UpdateSourceControlFromJobResponseTypeDef = TypedDict(
+    "UpdateSourceControlFromJobResponseTypeDef",
+    {
+        "JobName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateWorkflowRequestRequestTypeDef = TypedDict(
@@ -4244,14 +5392,22 @@
 )
 
 class UpdateWorkflowRequestRequestTypeDef(
     _RequiredUpdateWorkflowRequestRequestTypeDef, _OptionalUpdateWorkflowRequestRequestTypeDef
 ):
     pass
 
+UpdateWorkflowResponseTypeDef = TypedDict(
+    "UpdateWorkflowResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WorkflowRunStatisticsTypeDef = TypedDict(
     "WorkflowRunStatisticsTypeDef",
     {
         "TotalActions": int,
         "TimeoutActions": int,
         "FailedActions": int,
         "StoppedActions": int,
@@ -4310,14 +5466,47 @@
         "Name": str,
         "Inputs": List[str],
         "Groups": List[List[str]],
         "Aggs": List[AggregateOperationTypeDef],
     },
 )
 
+AmazonRedshiftNodeDataTypeDef = TypedDict(
+    "AmazonRedshiftNodeDataTypeDef",
+    {
+        "AccessType": str,
+        "SourceType": str,
+        "Connection": OptionTypeDef,
+        "Schema": OptionTypeDef,
+        "Table": OptionTypeDef,
+        "CatalogDatabase": OptionTypeDef,
+        "CatalogTable": OptionTypeDef,
+        "CatalogRedshiftSchema": str,
+        "CatalogRedshiftTable": str,
+        "TempDir": str,
+        "IamRole": OptionTypeDef,
+        "AdvancedOptions": List[AmazonRedshiftAdvancedOptionTypeDef],
+        "SampleQuery": str,
+        "PreAction": str,
+        "PostAction": str,
+        "Action": str,
+        "TablePrefix": str,
+        "Upsert": bool,
+        "MergeAction": str,
+        "MergeWhenMatched": str,
+        "MergeWhenNotMatched": str,
+        "MergeClause": str,
+        "CrawlerConnection": str,
+        "TableSchema": List[OptionTypeDef],
+        "StagingTable": str,
+        "SelectedColumns": List[OptionTypeDef],
+    },
+    total=False,
+)
+
 _RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
@@ -4409,627 +5598,20 @@
 )
 
 class BatchGetPartitionRequestRequestTypeDef(
     _RequiredBatchGetPartitionRequestRequestTypeDef, _OptionalBatchGetPartitionRequestRequestTypeDef
 ):
     pass
 
-CancelMLTaskRunResponseTypeDef = TypedDict(
-    "CancelMLTaskRunResponseTypeDef",
-    {
-        "TransformId": str,
-        "TaskRunId": str,
-        "Status": TaskStatusTypeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CheckSchemaVersionValidityResponseTypeDef = TypedDict(
-    "CheckSchemaVersionValidityResponseTypeDef",
-    {
-        "Valid": bool,
-        "Error": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBlueprintResponseTypeDef = TypedDict(
-    "CreateBlueprintResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCustomEntityTypeResponseTypeDef = TypedDict(
-    "CreateCustomEntityTypeResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDevEndpointResponseTypeDef = TypedDict(
-    "CreateDevEndpointResponseTypeDef",
-    {
-        "EndpointName": str,
-        "Status": str,
-        "SecurityGroupIds": List[str],
-        "SubnetId": str,
-        "RoleArn": str,
-        "YarnEndpointAddress": str,
-        "ZeppelinRemoteSparkInterpreterPort": int,
-        "NumberOfNodes": int,
-        "WorkerType": WorkerTypeType,
-        "GlueVersion": str,
-        "NumberOfWorkers": int,
-        "AvailabilityZone": str,
-        "VpcId": str,
-        "ExtraPythonLibsS3Path": str,
-        "ExtraJarsS3Path": str,
-        "FailureReason": str,
-        "SecurityConfiguration": str,
-        "CreatedTimestamp": datetime,
-        "Arguments": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobResponseTypeDef = TypedDict(
-    "CreateJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMLTransformResponseTypeDef = TypedDict(
-    "CreateMLTransformResponseTypeDef",
-    {
-        "TransformId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateRegistryResponseTypeDef = TypedDict(
-    "CreateRegistryResponseTypeDef",
-    {
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "RegistryName": str,
-        "RegistryArn": str,
-        "SchemaName": str,
-        "SchemaArn": str,
-        "Description": str,
-        "DataFormat": DataFormatType,
-        "Compatibility": CompatibilityType,
-        "SchemaCheckpoint": int,
-        "LatestSchemaVersion": int,
-        "NextSchemaVersion": int,
-        "SchemaStatus": SchemaStatusType,
-        "Tags": Dict[str, str],
-        "SchemaVersionId": str,
-        "SchemaVersionStatus": SchemaVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateScriptResponseTypeDef = TypedDict(
-    "CreateScriptResponseTypeDef",
-    {
-        "PythonScript": str,
-        "ScalaCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSecurityConfigurationResponseTypeDef = TypedDict(
-    "CreateSecurityConfigurationResponseTypeDef",
-    {
-        "Name": str,
-        "CreatedTimestamp": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateTriggerResponseTypeDef = TypedDict(
-    "CreateTriggerResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateWorkflowResponseTypeDef = TypedDict(
-    "CreateWorkflowResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBlueprintResponseTypeDef = TypedDict(
-    "DeleteBlueprintResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteCustomEntityTypeResponseTypeDef = TypedDict(
-    "DeleteCustomEntityTypeResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteJobResponseTypeDef = TypedDict(
-    "DeleteJobResponseTypeDef",
-    {
-        "JobName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteMLTransformResponseTypeDef = TypedDict(
-    "DeleteMLTransformResponseTypeDef",
-    {
-        "TransformId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteRegistryResponseTypeDef = TypedDict(
-    "DeleteRegistryResponseTypeDef",
-    {
-        "RegistryName": str,
-        "RegistryArn": str,
-        "Status": RegistryStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSchemaResponseTypeDef = TypedDict(
-    "DeleteSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "SchemaName": str,
-        "Status": SchemaStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteSessionResponseTypeDef = TypedDict(
-    "DeleteSessionResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteTriggerResponseTypeDef = TypedDict(
-    "DeleteTriggerResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteWorkflowResponseTypeDef = TypedDict(
-    "DeleteWorkflowResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCustomEntityTypeResponseTypeDef = TypedDict(
-    "GetCustomEntityTypeResponseTypeDef",
-    {
-        "Name": str,
-        "RegexString": str,
-        "ContextWords": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPlanResponseTypeDef = TypedDict(
-    "GetPlanResponseTypeDef",
-    {
-        "PythonScript": str,
-        "ScalaCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRegistryResponseTypeDef = TypedDict(
-    "GetRegistryResponseTypeDef",
-    {
-        "RegistryName": str,
-        "RegistryArn": str,
-        "Description": str,
-        "Status": RegistryStatusType,
-        "CreatedTime": str,
-        "UpdatedTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "PolicyInJson": str,
-        "PolicyHash": str,
-        "CreateTime": datetime,
-        "UpdateTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSchemaByDefinitionResponseTypeDef = TypedDict(
-    "GetSchemaByDefinitionResponseTypeDef",
-    {
-        "SchemaVersionId": str,
-        "SchemaArn": str,
-        "DataFormat": DataFormatType,
-        "Status": SchemaVersionStatusType,
-        "CreatedTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSchemaResponseTypeDef = TypedDict(
-    "GetSchemaResponseTypeDef",
-    {
-        "RegistryName": str,
-        "RegistryArn": str,
-        "SchemaName": str,
-        "SchemaArn": str,
-        "Description": str,
-        "DataFormat": DataFormatType,
-        "Compatibility": CompatibilityType,
-        "SchemaCheckpoint": int,
-        "LatestSchemaVersion": int,
-        "NextSchemaVersion": int,
-        "SchemaStatus": SchemaStatusType,
-        "CreatedTime": str,
-        "UpdatedTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSchemaVersionResponseTypeDef = TypedDict(
-    "GetSchemaVersionResponseTypeDef",
-    {
-        "SchemaVersionId": str,
-        "SchemaDefinition": str,
-        "DataFormat": DataFormatType,
-        "SchemaArn": str,
-        "VersionNumber": int,
-        "Status": SchemaVersionStatusType,
-        "CreatedTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSchemaVersionsDiffResponseTypeDef = TypedDict(
-    "GetSchemaVersionsDiffResponseTypeDef",
-    {
-        "Diff": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetWorkflowRunPropertiesResponseTypeDef = TypedDict(
-    "GetWorkflowRunPropertiesResponseTypeDef",
-    {
-        "RunProperties": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBlueprintsResponseTypeDef = TypedDict(
-    "ListBlueprintsResponseTypeDef",
-    {
-        "Blueprints": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCrawlersResponseTypeDef = TypedDict(
-    "ListCrawlersResponseTypeDef",
-    {
-        "CrawlerNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDevEndpointsResponseTypeDef = TypedDict(
-    "ListDevEndpointsResponseTypeDef",
-    {
-        "DevEndpointNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListJobsResponseTypeDef = TypedDict(
-    "ListJobsResponseTypeDef",
-    {
-        "JobNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListMLTransformsResponseTypeDef = TypedDict(
-    "ListMLTransformsResponseTypeDef",
-    {
-        "TransformIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTriggersResponseTypeDef = TypedDict(
-    "ListTriggersResponseTypeDef",
-    {
-        "TriggerNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListWorkflowsResponseTypeDef = TypedDict(
-    "ListWorkflowsResponseTypeDef",
-    {
-        "Workflows": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "PolicyHash": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutSchemaVersionMetadataResponseTypeDef = TypedDict(
-    "PutSchemaVersionMetadataResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "SchemaName": str,
-        "RegistryName": str,
-        "LatestVersion": bool,
-        "VersionNumber": int,
-        "SchemaVersionId": str,
-        "MetadataKey": str,
-        "MetadataValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterSchemaVersionResponseTypeDef = TypedDict(
-    "RegisterSchemaVersionResponseTypeDef",
-    {
-        "SchemaVersionId": str,
-        "VersionNumber": int,
-        "Status": SchemaVersionStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveSchemaVersionMetadataResponseTypeDef = TypedDict(
-    "RemoveSchemaVersionMetadataResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "SchemaName": str,
-        "RegistryName": str,
-        "LatestVersion": bool,
-        "VersionNumber": int,
-        "SchemaVersionId": str,
-        "MetadataKey": str,
-        "MetadataValue": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ResumeWorkflowRunResponseTypeDef = TypedDict(
-    "ResumeWorkflowRunResponseTypeDef",
-    {
-        "RunId": str,
-        "NodeIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RunStatementResponseTypeDef = TypedDict(
-    "RunStatementResponseTypeDef",
-    {
-        "Id": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartBlueprintRunResponseTypeDef = TypedDict(
-    "StartBlueprintRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartExportLabelsTaskRunResponseTypeDef = TypedDict(
-    "StartExportLabelsTaskRunResponseTypeDef",
-    {
-        "TaskRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartImportLabelsTaskRunResponseTypeDef = TypedDict(
-    "StartImportLabelsTaskRunResponseTypeDef",
-    {
-        "TaskRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
-    {
-        "JobRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartMLEvaluationTaskRunResponseTypeDef = TypedDict(
-    "StartMLEvaluationTaskRunResponseTypeDef",
-    {
-        "TaskRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartMLLabelingSetGenerationTaskRunResponseTypeDef = TypedDict(
-    "StartMLLabelingSetGenerationTaskRunResponseTypeDef",
-    {
-        "TaskRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartTriggerResponseTypeDef = TypedDict(
-    "StartTriggerResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartWorkflowRunResponseTypeDef = TypedDict(
-    "StartWorkflowRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopSessionResponseTypeDef = TypedDict(
-    "StopSessionResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopTriggerResponseTypeDef = TypedDict(
-    "StopTriggerResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateBlueprintResponseTypeDef = TypedDict(
-    "UpdateBlueprintResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateJobFromSourceControlResponseTypeDef = TypedDict(
-    "UpdateJobFromSourceControlResponseTypeDef",
-    {
-        "JobName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateJobResponseTypeDef = TypedDict(
-    "UpdateJobResponseTypeDef",
-    {
-        "JobName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateMLTransformResponseTypeDef = TypedDict(
-    "UpdateMLTransformResponseTypeDef",
-    {
-        "TransformId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateRegistryResponseTypeDef = TypedDict(
-    "UpdateRegistryResponseTypeDef",
-    {
-        "RegistryName": str,
-        "RegistryArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSchemaResponseTypeDef = TypedDict(
-    "UpdateSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "SchemaName": str,
-        "RegistryName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateSourceControlFromJobResponseTypeDef = TypedDict(
-    "UpdateSourceControlFromJobResponseTypeDef",
-    {
-        "JobName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateWorkflowResponseTypeDef = TypedDict(
-    "UpdateWorkflowResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchDeleteConnectionResponseTypeDef = TypedDict(
     "BatchDeleteConnectionResponseTypeDef",
     {
         "Succeeded": List[str],
         "Errors": Dict[str, ErrorDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchStopJobRunErrorTypeDef = TypedDict(
     "BatchStopJobRunErrorTypeDef",
     {
         "JobName": str,
@@ -5086,67 +5668,67 @@
 )
 
 BatchGetCustomEntityTypesResponseTypeDef = TypedDict(
     "BatchGetCustomEntityTypesResponseTypeDef",
     {
         "CustomEntityTypes": List[CustomEntityTypeTypeDef],
         "CustomEntityTypesNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomEntityTypesResponseTypeDef = TypedDict(
     "ListCustomEntityTypesResponseTypeDef",
     {
         "CustomEntityTypes": List[CustomEntityTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetDevEndpointsResponseTypeDef = TypedDict(
     "BatchGetDevEndpointsResponseTypeDef",
     {
         "DevEndpoints": List[DevEndpointTypeDef],
         "DevEndpointsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDevEndpointResponseTypeDef = TypedDict(
     "GetDevEndpointResponseTypeDef",
     {
         "DevEndpoint": DevEndpointTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDevEndpointsResponseTypeDef = TypedDict(
     "GetDevEndpointsResponseTypeDef",
     {
         "DevEndpoints": List[DevEndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBlueprintRunResponseTypeDef = TypedDict(
     "GetBlueprintRunResponseTypeDef",
     {
         "BlueprintRun": BlueprintRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBlueprintRunsResponseTypeDef = TypedDict(
     "GetBlueprintRunsResponseTypeDef",
     {
         "BlueprintRuns": List[BlueprintRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BlueprintTypeDef = TypedDict(
     "BlueprintTypeDef",
     {
         "Name": str,
@@ -5163,15 +5745,15 @@
     total=False,
 )
 
 GetCatalogImportStatusResponseTypeDef = TypedDict(
     "GetCatalogImportStatusResponseTypeDef",
     {
         "ImportStatus": CatalogImportStatusTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCatalogKafkaSourceTypeDef = TypedDict(
     "_RequiredCatalogKafkaSourceTypeDef",
     {
         "Name": str,
@@ -5303,14 +5885,62 @@
     },
     total=False,
 )
 
 class S3CatalogTargetTypeDef(_RequiredS3CatalogTargetTypeDef, _OptionalS3CatalogTargetTypeDef):
     pass
 
+_RequiredS3DeltaCatalogTargetTypeDef = TypedDict(
+    "_RequiredS3DeltaCatalogTargetTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Table": str,
+        "Database": str,
+    },
+)
+_OptionalS3DeltaCatalogTargetTypeDef = TypedDict(
+    "_OptionalS3DeltaCatalogTargetTypeDef",
+    {
+        "PartitionKeys": List[List[str]],
+        "AdditionalOptions": Dict[str, str],
+        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
+    },
+    total=False,
+)
+
+class S3DeltaCatalogTargetTypeDef(
+    _RequiredS3DeltaCatalogTargetTypeDef, _OptionalS3DeltaCatalogTargetTypeDef
+):
+    pass
+
+_RequiredS3HudiCatalogTargetTypeDef = TypedDict(
+    "_RequiredS3HudiCatalogTargetTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Table": str,
+        "Database": str,
+        "AdditionalOptions": Dict[str, str],
+    },
+)
+_OptionalS3HudiCatalogTargetTypeDef = TypedDict(
+    "_OptionalS3HudiCatalogTargetTypeDef",
+    {
+        "PartitionKeys": List[List[str]],
+        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
+    },
+    total=False,
+)
+
+class S3HudiCatalogTargetTypeDef(
+    _RequiredS3HudiCatalogTargetTypeDef, _OptionalS3HudiCatalogTargetTypeDef
+):
+    pass
+
 ClassifierTypeDef = TypedDict(
     "ClassifierTypeDef",
     {
         "GrokClassifier": GrokClassifierTypeDef,
         "XMLClassifier": XMLClassifierTypeDef,
         "JsonClassifier": JsonClassifierTypeDef,
         "CsvClassifier": CsvClassifierTypeDef,
@@ -5415,36 +6045,37 @@
 )
 
 ListCrawlsResponseTypeDef = TypedDict(
     "ListCrawlsResponseTypeDef",
     {
         "Crawls": List[CrawlerHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCrawlerMetricsResponseTypeDef = TypedDict(
     "GetCrawlerMetricsResponseTypeDef",
     {
         "CrawlerMetricsList": List[CrawlerMetricsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CrawlerTargetsTypeDef = TypedDict(
     "CrawlerTargetsTypeDef",
     {
         "S3Targets": List[S3TargetTypeDef],
         "JdbcTargets": List[JdbcTargetTypeDef],
         "MongoDBTargets": List[MongoDBTargetTypeDef],
         "DynamoDBTargets": List[DynamoDBTargetTypeDef],
         "CatalogTargets": List[CatalogTargetTypeDef],
         "DeltaTargets": List[DeltaTargetTypeDef],
+        "IcebergTargets": List[IcebergTargetTypeDef],
     },
     total=False,
 )
 
 _RequiredListCrawlsRequestRequestTypeDef = TypedDict(
     "_RequiredListCrawlsRequestRequestTypeDef",
     {
@@ -5473,14 +6104,87 @@
         "XMLClassifier": CreateXMLClassifierRequestTypeDef,
         "JsonClassifier": CreateJsonClassifierRequestTypeDef,
         "CsvClassifier": CreateCsvClassifierRequestTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateDataQualityRulesetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataQualityRulesetRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Ruleset": str,
+    },
+)
+_OptionalCreateDataQualityRulesetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataQualityRulesetRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Mapping[str, str],
+        "TargetTable": DataQualityTargetTableTypeDef,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class CreateDataQualityRulesetRequestRequestTypeDef(
+    _RequiredCreateDataQualityRulesetRequestRequestTypeDef,
+    _OptionalCreateDataQualityRulesetRequestRequestTypeDef,
+):
+    pass
+
+DataQualityRulesetFilterCriteriaTypeDef = TypedDict(
+    "DataQualityRulesetFilterCriteriaTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "CreatedBefore": Union[datetime, str],
+        "CreatedAfter": Union[datetime, str],
+        "LastModifiedBefore": Union[datetime, str],
+        "LastModifiedAfter": Union[datetime, str],
+        "TargetTable": DataQualityTargetTableTypeDef,
+    },
+    total=False,
+)
+
+DataQualityRulesetListDetailsTypeDef = TypedDict(
+    "DataQualityRulesetListDetailsTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "CreatedOn": datetime,
+        "LastModifiedOn": datetime,
+        "TargetTable": DataQualityTargetTableTypeDef,
+        "RecommendationRunId": str,
+        "RuleCount": int,
+    },
+    total=False,
+)
+
+GetDataQualityRulesetResponseTypeDef = TypedDict(
+    "GetDataQualityRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Ruleset": str,
+        "TargetTable": DataQualityTargetTableTypeDef,
+        "CreatedOn": datetime,
+        "LastModifiedOn": datetime,
+        "RecommendationRunId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DataSourceTypeDef = TypedDict(
+    "DataSourceTypeDef",
+    {
+        "GlueTable": GlueTableTypeDef,
+    },
+)
+
 _RequiredCreatePartitionIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePartitionIndexRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionIndex": PartitionIndexTypeDef,
     },
@@ -5533,14 +6237,23 @@
 GetRegistryInputRequestTypeDef = TypedDict(
     "GetRegistryInputRequestTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
     },
 )
 
+ListSchemasInputListSchemasPaginateTypeDef = TypedDict(
+    "ListSchemasInputListSchemasPaginateTypeDef",
+    {
+        "RegistryId": RegistryIdTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSchemasInputRequestTypeDef = TypedDict(
     "ListSchemasInputRequestTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -5603,14 +6316,61 @@
         "MaxCapacity": float,
         "SecurityConfiguration": str,
         "GlueVersion": str,
     },
     total=False,
 )
 
+_RequiredEvaluateDataQualityMultiFrameTypeDef = TypedDict(
+    "_RequiredEvaluateDataQualityMultiFrameTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Ruleset": str,
+    },
+)
+_OptionalEvaluateDataQualityMultiFrameTypeDef = TypedDict(
+    "_OptionalEvaluateDataQualityMultiFrameTypeDef",
+    {
+        "AdditionalDataSources": Dict[str, str],
+        "PublishingOptions": DQResultsPublishingOptionsTypeDef,
+        "AdditionalOptions": Dict[Literal["performanceTuning.caching"], str],
+        "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
+    },
+    total=False,
+)
+
+class EvaluateDataQualityMultiFrameTypeDef(
+    _RequiredEvaluateDataQualityMultiFrameTypeDef, _OptionalEvaluateDataQualityMultiFrameTypeDef
+):
+    pass
+
+_RequiredEvaluateDataQualityTypeDef = TypedDict(
+    "_RequiredEvaluateDataQualityTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Ruleset": str,
+    },
+)
+_OptionalEvaluateDataQualityTypeDef = TypedDict(
+    "_OptionalEvaluateDataQualityTypeDef",
+    {
+        "Output": DQTransformOutputType,
+        "PublishingOptions": DQResultsPublishingOptionsTypeDef,
+        "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
+    },
+    total=False,
+)
+
+class EvaluateDataQualityTypeDef(
+    _RequiredEvaluateDataQualityTypeDef, _OptionalEvaluateDataQualityTypeDef
+):
+    pass
+
 DataCatalogEncryptionSettingsTypeDef = TypedDict(
     "DataCatalogEncryptionSettingsTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "ConnectionPasswordEncryption": ConnectionPasswordEncryptionTypeDef,
     },
     total=False,
@@ -5680,14 +6440,34 @@
 GetSchemaInputRequestTypeDef = TypedDict(
     "GetSchemaInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
     },
 )
 
+_RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
+    {
+        "SchemaId": SchemaIdTypeDef,
+    },
+)
+_OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef(
+    _RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
+    _OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListSchemaVersionsInputRequestTypeDef = TypedDict(
     "_RequiredListSchemaVersionsInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
     },
 )
 _OptionalListSchemaVersionsInputRequestTypeDef = TypedDict(
@@ -5743,14 +6523,39 @@
 )
 
 class UpdateDevEndpointRequestRequestTypeDef(
     _RequiredUpdateDevEndpointRequestRequestTypeDef, _OptionalUpdateDevEndpointRequestRequestTypeDef
 ):
     pass
 
+_RequiredS3DeltaDirectTargetTypeDef = TypedDict(
+    "_RequiredS3DeltaDirectTargetTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Path": str,
+        "Compression": DeltaTargetCompressionTypeType,
+        "Format": TargetFormatType,
+    },
+)
+_OptionalS3DeltaDirectTargetTypeDef = TypedDict(
+    "_OptionalS3DeltaDirectTargetTypeDef",
+    {
+        "PartitionKeys": List[List[str]],
+        "AdditionalOptions": Dict[str, str],
+        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
+    },
+    total=False,
+)
+
+class S3DeltaDirectTargetTypeDef(
+    _RequiredS3DeltaDirectTargetTypeDef, _OptionalS3DeltaDirectTargetTypeDef
+):
+    pass
+
 _RequiredS3DirectTargetTypeDef = TypedDict(
     "_RequiredS3DirectTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Path": str,
         "Format": TargetFormatType,
@@ -5788,14 +6593,39 @@
 )
 
 class S3GlueParquetTargetTypeDef(
     _RequiredS3GlueParquetTargetTypeDef, _OptionalS3GlueParquetTargetTypeDef
 ):
     pass
 
+_RequiredS3HudiDirectTargetTypeDef = TypedDict(
+    "_RequiredS3HudiDirectTargetTypeDef",
+    {
+        "Name": str,
+        "Inputs": List[str],
+        "Path": str,
+        "Compression": HudiTargetCompressionTypeType,
+        "Format": TargetFormatType,
+        "AdditionalOptions": Dict[str, str],
+    },
+)
+_OptionalS3HudiDirectTargetTypeDef = TypedDict(
+    "_OptionalS3HudiDirectTargetTypeDef",
+    {
+        "PartitionKeys": List[List[str]],
+        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
+    },
+    total=False,
+)
+
+class S3HudiDirectTargetTypeDef(
+    _RequiredS3HudiDirectTargetTypeDef, _OptionalS3HudiDirectTargetTypeDef
+):
+    pass
+
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "S3Encryption": Sequence[S3EncryptionTypeDef],
         "CloudWatchEncryption": CloudWatchEncryptionTypeDef,
         "JobBookmarksEncryption": JobBookmarksEncryptionTypeDef,
     },
@@ -5844,244 +6674,21 @@
 )
 
 class TransformParametersTypeDef(
     _RequiredTransformParametersTypeDef, _OptionalTransformParametersTypeDef
 ):
     pass
 
-GetClassifiersRequestGetClassifiersPaginateTypeDef = TypedDict(
-    "GetClassifiersRequestGetClassifiersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef = TypedDict(
-    "GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef",
-    {
-        "CrawlerNameList": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetCrawlersRequestGetCrawlersPaginateTypeDef = TypedDict(
-    "GetCrawlersRequestGetCrawlersPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetDatabasesRequestGetDatabasesPaginateTypeDef = TypedDict(
-    "GetDatabasesRequestGetDatabasesPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "ResourceShareType": ResourceShareTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef = TypedDict(
-    "GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef",
-    {
-        "JobName": str,
-    },
-)
-_OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetJobRunsRequestGetJobRunsPaginateTypeDef(
-    _RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef,
-    _OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef,
-):
-    pass
-
-GetJobsRequestGetJobsPaginateTypeDef = TypedDict(
-    "GetJobsRequestGetJobsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef = TypedDict(
-    "_RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-    },
-)
-_OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef = TypedDict(
-    "_OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef(
-    _RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
-    _OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
-):
-    pass
-
-GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef = TypedDict(
-    "GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-    },
-)
-_OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetTableVersionsRequestGetTableVersionsPaginateTypeDef(
-    _RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
-    _OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
-):
-    pass
-
-_RequiredGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
-    "_RequiredGetTablesRequestGetTablesPaginateTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
-    "_OptionalGetTablesRequestGetTablesPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "Expression": str,
-        "TransactionId": str,
-        "QueryAsOfTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetTablesRequestGetTablesPaginateTypeDef(
-    _RequiredGetTablesRequestGetTablesPaginateTypeDef,
-    _OptionalGetTablesRequestGetTablesPaginateTypeDef,
-):
-    pass
-
-GetTriggersRequestGetTriggersPaginateTypeDef = TypedDict(
-    "GetTriggersRequestGetTriggersPaginateTypeDef",
-    {
-        "DependentJobName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef = TypedDict(
-    "_RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef",
-    {
-        "Pattern": str,
-    },
-)
-_OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef = TypedDict(
-    "_OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "DatabaseName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef(
-    _RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
-    _OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
-):
-    pass
-
-ListRegistriesInputListRegistriesPaginateTypeDef = TypedDict(
-    "ListRegistriesInputListRegistriesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
-    {
-        "SchemaId": SchemaIdTypeDef,
-    },
-)
-_OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef(
-    _RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
-    _OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
-):
-    pass
-
-ListSchemasInputListSchemasPaginateTypeDef = TypedDict(
-    "ListSchemasInputListSchemasPaginateTypeDef",
-    {
-        "RegistryId": RegistryIdTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 GetConnectionsRequestGetConnectionsPaginateTypeDef = TypedDict(
     "GetConnectionsRequestGetConnectionsPaginateTypeDef",
     {
         "CatalogId": str,
         "Filter": GetConnectionsFilterTypeDef,
         "HidePassword": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 GetConnectionsRequestRequestTypeDef = TypedDict(
     "GetConnectionsRequestRequestTypeDef",
     {
@@ -6094,23 +6701,23 @@
     total=False,
 )
 
 GetJobBookmarkResponseTypeDef = TypedDict(
     "GetJobBookmarkResponseTypeDef",
     {
         "JobBookmarkEntry": JobBookmarkEntryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResetJobBookmarkResponseTypeDef = TypedDict(
     "ResetJobBookmarkResponseTypeDef",
     {
         "JobBookmarkEntry": JobBookmarkEntryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetMLTaskRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetMLTaskRunsRequestRequestTypeDef",
     {
         "TransformId": str,
@@ -6148,15 +6755,15 @@
     total=False,
 )
 
 GetMappingResponseTypeDef = TypedDict(
     "GetMappingResponseTypeDef",
     {
         "Mapping": List[MappingEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef = TypedDict(
     "_RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef",
     {
         "DatabaseName": str,
@@ -6168,15 +6775,15 @@
     {
         "CatalogId": str,
         "Expression": str,
         "Segment": SegmentTypeDef,
         "ExcludeColumnSchema": bool,
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class GetPartitionsRequestGetPartitionsPaginateTypeDef(
     _RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef,
     _OptionalGetPartitionsRequestGetPartitionsPaginateTypeDef,
@@ -6238,15 +6845,15 @@
     pass
 
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "GetResourcePoliciesResponseList": List[GluePolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSchemaVersionInputRequestTypeDef = TypedDict(
     "GetSchemaVersionInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
@@ -6391,33 +6998,33 @@
 )
 
 ListRegistriesResponseTypeDef = TypedDict(
     "ListRegistriesResponseTypeDef",
     {
         "Registries": List[RegistryListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSchemaVersionsResponseTypeDef = TypedDict(
     "ListSchemaVersionsResponseTypeDef",
     {
         "Schemas": List[SchemaVersionListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSchemasResponseTypeDef = TypedDict(
     "ListSchemasResponseTypeDef",
     {
         "Schemas": List[SchemaListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TransformEncryptionTypeDef = TypedDict(
     "TransformEncryptionTypeDef",
     {
         "MlUserDataEncryption": MLUserDataEncryptionTypeDef,
@@ -6576,14 +7183,33 @@
         "XMLClassifier": UpdateXMLClassifierRequestTypeDef,
         "JsonClassifier": UpdateJsonClassifierRequestTypeDef,
         "CsvClassifier": UpdateCsvClassifierRequestTypeDef,
     },
     total=False,
 )
 
+AmazonRedshiftSourceTypeDef = TypedDict(
+    "AmazonRedshiftSourceTypeDef",
+    {
+        "Name": str,
+        "Data": AmazonRedshiftNodeDataTypeDef,
+    },
+    total=False,
+)
+
+AmazonRedshiftTargetTypeDef = TypedDict(
+    "AmazonRedshiftTargetTypeDef",
+    {
+        "Name": str,
+        "Data": AmazonRedshiftNodeDataTypeDef,
+        "Inputs": List[str],
+    },
+    total=False,
+)
+
 _RequiredPartitionIndexDescriptorTypeDef = TypedDict(
     "_RequiredPartitionIndexDescriptorTypeDef",
     {
         "IndexName": str,
         "Keys": List[KeySchemaElementTypeDef],
         "IndexStatus": PartitionIndexStatusType,
     },
@@ -6602,89 +7228,89 @@
     pass
 
 BatchStopJobRunResponseTypeDef = TypedDict(
     "BatchStopJobRunResponseTypeDef",
     {
         "SuccessfulSubmissions": List[BatchStopJobRunSuccessfulSubmissionTypeDef],
         "Errors": List[BatchStopJobRunErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchUpdatePartitionResponseTypeDef = TypedDict(
     "BatchUpdatePartitionResponseTypeDef",
     {
         "Errors": List[BatchUpdatePartitionFailureEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchCreatePartitionResponseTypeDef = TypedDict(
     "BatchCreatePartitionResponseTypeDef",
     {
         "Errors": List[PartitionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeletePartitionResponseTypeDef = TypedDict(
     "BatchDeletePartitionResponseTypeDef",
     {
         "Errors": List[PartitionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteTableResponseTypeDef = TypedDict(
     "BatchDeleteTableResponseTypeDef",
     {
         "Errors": List[TableErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDeleteTableVersionResponseTypeDef = TypedDict(
     "BatchDeleteTableVersionResponseTypeDef",
     {
         "Errors": List[TableVersionErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetBlueprintsResponseTypeDef = TypedDict(
     "BatchGetBlueprintsResponseTypeDef",
     {
         "Blueprints": List[BlueprintTypeDef],
         "MissingBlueprints": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetBlueprintResponseTypeDef = TypedDict(
     "GetBlueprintResponseTypeDef",
     {
         "Blueprint": BlueprintTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetClassifierResponseTypeDef = TypedDict(
     "GetClassifierResponseTypeDef",
     {
         "Classifier": ClassifierTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetClassifiersResponseTypeDef = TypedDict(
     "GetClassifiersResponseTypeDef",
     {
         "Classifiers": List[ClassifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateScriptRequestRequestTypeDef = TypedDict(
     "CreateScriptRequestRequestTypeDef",
     {
         "DagNodes": Sequence[CodeGenNodeTypeDef],
@@ -6695,15 +7321,15 @@
 )
 
 GetDataflowGraphResponseTypeDef = TypedDict(
     "GetDataflowGraphResponseTypeDef",
     {
         "DagNodes": List[CodeGenNodeTypeDef],
         "DagEdges": List[CodeGenEdgeTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetMappingRequestRequestTypeDef = TypedDict(
     "_RequiredGetMappingRequestRequestTypeDef",
     {
         "Source": CatalogEntryTypeDef,
@@ -6862,24 +7488,24 @@
 ):
     pass
 
 GetConnectionResponseTypeDef = TypedDict(
     "GetConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetConnectionsResponseTypeDef = TypedDict(
     "GetConnectionsResponseTypeDef",
     {
         "ConnectionList": List[ConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CrawlerTypeDef = TypedDict(
     "CrawlerTypeDef",
     {
         "Name": str,
@@ -6965,45 +7591,281 @@
 )
 
 class UpdateCrawlerRequestRequestTypeDef(
     _RequiredUpdateCrawlerRequestRequestTypeDef, _OptionalUpdateCrawlerRequestRequestTypeDef
 ):
     pass
 
+ListDataQualityRulesetsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRulesetsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "Filter": DataQualityRulesetFilterCriteriaTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+ListDataQualityRulesetsResponseTypeDef = TypedDict(
+    "ListDataQualityRulesetsResponseTypeDef",
+    {
+        "Rulesets": List[DataQualityRulesetListDetailsTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DataQualityResultDescriptionTypeDef = TypedDict(
+    "DataQualityResultDescriptionTypeDef",
+    {
+        "ResultId": str,
+        "DataSource": DataSourceTypeDef,
+        "JobName": str,
+        "JobRunId": str,
+        "StartedOn": datetime,
+    },
+    total=False,
+)
+
+DataQualityResultFilterCriteriaTypeDef = TypedDict(
+    "DataQualityResultFilterCriteriaTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+        "JobName": str,
+        "JobRunId": str,
+        "StartedAfter": Union[datetime, str],
+        "StartedBefore": Union[datetime, str],
+    },
+    total=False,
+)
+
+DataQualityResultTypeDef = TypedDict(
+    "DataQualityResultTypeDef",
+    {
+        "ResultId": str,
+        "Score": float,
+        "DataSource": DataSourceTypeDef,
+        "RulesetName": str,
+        "EvaluationContext": str,
+        "StartedOn": datetime,
+        "CompletedOn": datetime,
+        "JobName": str,
+        "JobRunId": str,
+        "RulesetEvaluationRunId": str,
+        "RuleResults": List[DataQualityRuleResultTypeDef],
+    },
+    total=False,
+)
+
+DataQualityRuleRecommendationRunDescriptionTypeDef = TypedDict(
+    "DataQualityRuleRecommendationRunDescriptionTypeDef",
+    {
+        "RunId": str,
+        "Status": TaskStatusTypeType,
+        "StartedOn": datetime,
+        "DataSource": DataSourceTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
+    "_RequiredDataQualityRuleRecommendationRunFilterTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+    },
+)
+_OptionalDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
+    "_OptionalDataQualityRuleRecommendationRunFilterTypeDef",
+    {
+        "StartedBefore": Union[datetime, str],
+        "StartedAfter": Union[datetime, str],
+    },
+    total=False,
+)
+
+class DataQualityRuleRecommendationRunFilterTypeDef(
+    _RequiredDataQualityRuleRecommendationRunFilterTypeDef,
+    _OptionalDataQualityRuleRecommendationRunFilterTypeDef,
+):
+    pass
+
+DataQualityRulesetEvaluationRunDescriptionTypeDef = TypedDict(
+    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
+    {
+        "RunId": str,
+        "Status": TaskStatusTypeType,
+        "StartedOn": datetime,
+        "DataSource": DataSourceTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
+    "_RequiredDataQualityRulesetEvaluationRunFilterTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+    },
+)
+_OptionalDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
+    "_OptionalDataQualityRulesetEvaluationRunFilterTypeDef",
+    {
+        "StartedBefore": Union[datetime, str],
+        "StartedAfter": Union[datetime, str],
+    },
+    total=False,
+)
+
+class DataQualityRulesetEvaluationRunFilterTypeDef(
+    _RequiredDataQualityRulesetEvaluationRunFilterTypeDef,
+    _OptionalDataQualityRulesetEvaluationRunFilterTypeDef,
+):
+    pass
+
+GetDataQualityResultResponseTypeDef = TypedDict(
+    "GetDataQualityResultResponseTypeDef",
+    {
+        "ResultId": str,
+        "Score": float,
+        "DataSource": DataSourceTypeDef,
+        "RulesetName": str,
+        "EvaluationContext": str,
+        "StartedOn": datetime,
+        "CompletedOn": datetime,
+        "JobName": str,
+        "JobRunId": str,
+        "RulesetEvaluationRunId": str,
+        "RuleResults": List[DataQualityRuleResultTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDataQualityRuleRecommendationRunResponseTypeDef = TypedDict(
+    "GetDataQualityRuleRecommendationRunResponseTypeDef",
+    {
+        "RunId": str,
+        "DataSource": DataSourceTypeDef,
+        "Role": str,
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "Status": TaskStatusTypeType,
+        "ErrorString": str,
+        "StartedOn": datetime,
+        "LastModifiedOn": datetime,
+        "CompletedOn": datetime,
+        "ExecutionTime": int,
+        "RecommendedRuleset": str,
+        "CreatedRulesetName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDataQualityRulesetEvaluationRunResponseTypeDef = TypedDict(
+    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
+    {
+        "RunId": str,
+        "DataSource": DataSourceTypeDef,
+        "Role": str,
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
+        "Status": TaskStatusTypeType,
+        "ErrorString": str,
+        "StartedOn": datetime,
+        "LastModifiedOn": datetime,
+        "CompletedOn": datetime,
+        "ExecutionTime": int,
+        "RulesetNames": List[str],
+        "ResultIds": List[str],
+        "AdditionalDataSources": Dict[str, DataSourceTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+        "Role": str,
+    },
+)
+_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
+    {
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "CreatedRulesetName": str,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class StartDataQualityRuleRecommendationRunRequestRequestTypeDef(
+    _RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
+    _OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+        "Role": str,
+        "RulesetNames": Sequence[str],
+    },
+)
+_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
+    {
+        "NumberOfWorkers": int,
+        "Timeout": int,
+        "ClientToken": str,
+        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
+        "AdditionalDataSources": Mapping[str, DataSourceTypeDef],
+    },
+    total=False,
+)
+
+class StartDataQualityRulesetEvaluationRunRequestRequestTypeDef(
+    _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
+    _OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
+):
+    pass
+
 CreateSessionResponseTypeDef = TypedDict(
     "CreateSessionResponseTypeDef",
     {
         "Session": SessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "Session": SessionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSessionsResponseTypeDef = TypedDict(
     "ListSessionsResponseTypeDef",
     {
         "Ids": List[str],
         "Sessions": List[SessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDataCatalogEncryptionSettingsResponseTypeDef = TypedDict(
     "GetDataCatalogEncryptionSettingsResponseTypeDef",
     {
         "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
     {
         "DataCatalogEncryptionSettings": DataCatalogEncryptionSettingsTypeDef,
@@ -7033,14 +7895,15 @@
     "_OptionalDatabaseInputTypeDef",
     {
         "Description": str,
         "LocationUri": str,
         "Parameters": Mapping[str, str],
         "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
         "TargetDatabase": DatabaseIdentifierTypeDef,
+        "FederatedDatabase": FederatedDatabaseTypeDef,
     },
     total=False,
 )
 
 class DatabaseInputTypeDef(_RequiredDatabaseInputTypeDef, _OptionalDatabaseInputTypeDef):
     pass
 
@@ -7056,14 +7919,15 @@
         "Description": str,
         "LocationUri": str,
         "Parameters": Dict[str, str],
         "CreateTime": datetime,
         "CreateTableDefaultPermissions": List[PrincipalPermissionsTypeDef],
         "TargetDatabase": DatabaseIdentifierTypeDef,
         "CatalogId": str,
+        "FederatedDatabase": FederatedDatabaseTypeDef,
     },
     total=False,
 )
 
 class DatabaseTypeDef(_RequiredDatabaseTypeDef, _OptionalDatabaseTypeDef):
     pass
 
@@ -7150,15 +8014,15 @@
     total=False,
 )
 
 DeleteSchemaVersionsResponseTypeDef = TypedDict(
     "DeleteSchemaVersionsResponseTypeDef",
     {
         "SchemaVersionErrors": List[SchemaVersionErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
@@ -7239,14 +8103,58 @@
 )
 
 class AthenaConnectorSourceTypeDef(
     _RequiredAthenaConnectorSourceTypeDef, _OptionalAthenaConnectorSourceTypeDef
 ):
     pass
 
+_RequiredCatalogDeltaSourceTypeDef = TypedDict(
+    "_RequiredCatalogDeltaSourceTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+_OptionalCatalogDeltaSourceTypeDef = TypedDict(
+    "_OptionalCatalogDeltaSourceTypeDef",
+    {
+        "AdditionalDeltaOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+class CatalogDeltaSourceTypeDef(
+    _RequiredCatalogDeltaSourceTypeDef, _OptionalCatalogDeltaSourceTypeDef
+):
+    pass
+
+_RequiredCatalogHudiSourceTypeDef = TypedDict(
+    "_RequiredCatalogHudiSourceTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+_OptionalCatalogHudiSourceTypeDef = TypedDict(
+    "_OptionalCatalogHudiSourceTypeDef",
+    {
+        "AdditionalHudiOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+class CatalogHudiSourceTypeDef(
+    _RequiredCatalogHudiSourceTypeDef, _OptionalCatalogHudiSourceTypeDef
+):
+    pass
+
 _RequiredCustomCodeTypeDef = TypedDict(
     "_RequiredCustomCodeTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Code": str,
         "ClassName": str,
@@ -7259,14 +8167,37 @@
     },
     total=False,
 )
 
 class CustomCodeTypeDef(_RequiredCustomCodeTypeDef, _OptionalCustomCodeTypeDef):
     pass
 
+_RequiredDynamicTransformTypeDef = TypedDict(
+    "_RequiredDynamicTransformTypeDef",
+    {
+        "Name": str,
+        "TransformName": str,
+        "Inputs": List[str],
+        "FunctionName": str,
+        "Path": str,
+    },
+)
+_OptionalDynamicTransformTypeDef = TypedDict(
+    "_OptionalDynamicTransformTypeDef",
+    {
+        "Parameters": List[TransformConfigParameterTypeDef],
+        "Version": str,
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+class DynamicTransformTypeDef(_RequiredDynamicTransformTypeDef, _OptionalDynamicTransformTypeDef):
+    pass
+
 _RequiredJDBCConnectorSourceTypeDef = TypedDict(
     "_RequiredJDBCConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
@@ -7309,14 +8240,58 @@
 )
 
 class JDBCConnectorTargetTypeDef(
     _RequiredJDBCConnectorTargetTypeDef, _OptionalJDBCConnectorTargetTypeDef
 ):
     pass
 
+_RequiredS3CatalogDeltaSourceTypeDef = TypedDict(
+    "_RequiredS3CatalogDeltaSourceTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+_OptionalS3CatalogDeltaSourceTypeDef = TypedDict(
+    "_OptionalS3CatalogDeltaSourceTypeDef",
+    {
+        "AdditionalDeltaOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+class S3CatalogDeltaSourceTypeDef(
+    _RequiredS3CatalogDeltaSourceTypeDef, _OptionalS3CatalogDeltaSourceTypeDef
+):
+    pass
+
+_RequiredS3CatalogHudiSourceTypeDef = TypedDict(
+    "_RequiredS3CatalogHudiSourceTypeDef",
+    {
+        "Name": str,
+        "Database": str,
+        "Table": str,
+    },
+)
+_OptionalS3CatalogHudiSourceTypeDef = TypedDict(
+    "_OptionalS3CatalogHudiSourceTypeDef",
+    {
+        "AdditionalHudiOptions": Dict[str, str],
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+class S3CatalogHudiSourceTypeDef(
+    _RequiredS3CatalogHudiSourceTypeDef, _OptionalS3CatalogHudiSourceTypeDef
+):
+    pass
+
 _RequiredS3CsvSourceTypeDef = TypedDict(
     "_RequiredS3CsvSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
         "Separator": SeparatorType,
         "QuoteChar": QuoteCharType,
@@ -7343,14 +8318,54 @@
     },
     total=False,
 )
 
 class S3CsvSourceTypeDef(_RequiredS3CsvSourceTypeDef, _OptionalS3CsvSourceTypeDef):
     pass
 
+_RequiredS3DeltaSourceTypeDef = TypedDict(
+    "_RequiredS3DeltaSourceTypeDef",
+    {
+        "Name": str,
+        "Paths": List[str],
+    },
+)
+_OptionalS3DeltaSourceTypeDef = TypedDict(
+    "_OptionalS3DeltaSourceTypeDef",
+    {
+        "AdditionalDeltaOptions": Dict[str, str],
+        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+class S3DeltaSourceTypeDef(_RequiredS3DeltaSourceTypeDef, _OptionalS3DeltaSourceTypeDef):
+    pass
+
+_RequiredS3HudiSourceTypeDef = TypedDict(
+    "_RequiredS3HudiSourceTypeDef",
+    {
+        "Name": str,
+        "Paths": List[str],
+    },
+)
+_OptionalS3HudiSourceTypeDef = TypedDict(
+    "_OptionalS3HudiSourceTypeDef",
+    {
+        "AdditionalHudiOptions": Dict[str, str],
+        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
+        "OutputSchemas": List[GlueSchemaTypeDef],
+    },
+    total=False,
+)
+
+class S3HudiSourceTypeDef(_RequiredS3HudiSourceTypeDef, _OptionalS3HudiSourceTypeDef):
+    pass
+
 _RequiredS3JsonSourceTypeDef = TypedDict(
     "_RequiredS3JsonSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
     },
 )
@@ -7468,24 +8483,24 @@
 class SparkSQLTypeDef(_RequiredSparkSQLTypeDef, _OptionalSparkSQLTypeDef):
     pass
 
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "JobRun": JobRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobRunsResponseTypeDef = TypedDict(
     "GetJobRunsResponseTypeDef",
     {
         "JobRuns": List[JobRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JobNodeDetailsTypeDef = TypedDict(
     "JobNodeDetailsTypeDef",
     {
         "JobRuns": List[JobRunTypeDef],
@@ -7502,15 +8517,15 @@
         "LogGroupName": str,
         "Properties": TaskRunPropertiesTypeDef,
         "ErrorString": str,
         "StartedOn": datetime,
         "LastModifiedOn": datetime,
         "CompletedOn": datetime,
         "ExecutionTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TaskRunTypeDef = TypedDict(
     "TaskRunTypeDef",
     {
         "TransformId": str,
@@ -7559,15 +8574,15 @@
 
 QuerySchemaVersionMetadataResponseTypeDef = TypedDict(
     "QuerySchemaVersionMetadataResponseTypeDef",
     {
         "MetadataInfoMap": Dict[str, MetadataInfoTypeDef],
         "SchemaVersionId": str,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateUserDefinedFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserDefinedFunctionRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -7610,24 +8625,24 @@
 ):
     pass
 
 GetUserDefinedFunctionResponseTypeDef = TypedDict(
     "GetUserDefinedFunctionResponseTypeDef",
     {
         "UserDefinedFunction": UserDefinedFunctionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUserDefinedFunctionsResponseTypeDef = TypedDict(
     "GetUserDefinedFunctionsResponseTypeDef",
     {
         "UserDefinedFunctions": List[UserDefinedFunctionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StatementTypeDef = TypedDict(
     "StatementTypeDef",
     {
         "Id": int,
@@ -7642,41 +8657,41 @@
 )
 
 GetPartitionIndexesResponseTypeDef = TypedDict(
     "GetPartitionIndexesResponseTypeDef",
     {
         "PartitionIndexDescriptorList": List[PartitionIndexDescriptorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetTriggersResponseTypeDef = TypedDict(
     "BatchGetTriggersResponseTypeDef",
     {
         "Triggers": List[TriggerTypeDef],
         "TriggersNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTriggerResponseTypeDef = TypedDict(
     "GetTriggerResponseTypeDef",
     {
         "Trigger": TriggerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTriggersResponseTypeDef = TypedDict(
     "GetTriggersResponseTypeDef",
     {
         "Triggers": List[TriggerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TriggerNodeDetailsTypeDef = TypedDict(
     "TriggerNodeDetailsTypeDef",
     {
         "Trigger": TriggerTypeDef,
@@ -7684,15 +8699,15 @@
     total=False,
 )
 
 UpdateTriggerResponseTypeDef = TypedDict(
     "UpdateTriggerResponseTypeDef",
     {
         "Trigger": TriggerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateTriggerRequestRequestTypeDef = TypedDict(
     "UpdateTriggerRequestRequestTypeDef",
     {
         "Name": str,
@@ -7718,15 +8733,15 @@
         "GlueVersion": str,
         "MaxCapacity": float,
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "Timeout": int,
         "MaxRetries": int,
         "TransformEncryption": TransformEncryptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MLTransformTypeDef = TypedDict(
     "MLTransformTypeDef",
     {
         "TransformId": str,
@@ -7753,35 +8768,101 @@
 )
 
 BatchGetCrawlersResponseTypeDef = TypedDict(
     "BatchGetCrawlersResponseTypeDef",
     {
         "Crawlers": List[CrawlerTypeDef],
         "CrawlersNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCrawlerResponseTypeDef = TypedDict(
     "GetCrawlerResponseTypeDef",
     {
         "Crawler": CrawlerTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCrawlersResponseTypeDef = TypedDict(
     "GetCrawlersResponseTypeDef",
     {
         "Crawlers": List[CrawlerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDataQualityResultsResponseTypeDef = TypedDict(
+    "ListDataQualityResultsResponseTypeDef",
+    {
+        "Results": List[DataQualityResultDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDataQualityResultsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityResultsRequestRequestTypeDef",
+    {
+        "Filter": DataQualityResultFilterCriteriaTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+BatchGetDataQualityResultResponseTypeDef = TypedDict(
+    "BatchGetDataQualityResultResponseTypeDef",
+    {
+        "Results": List[DataQualityResultTypeDef],
+        "ResultsNotFound": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDataQualityRuleRecommendationRunsResponseTypeDef = TypedDict(
+    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
+    {
+        "Runs": List[DataQualityRuleRecommendationRunDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDataQualityRuleRecommendationRunsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
+    {
+        "Filter": DataQualityRuleRecommendationRunFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListDataQualityRulesetEvaluationRunsResponseTypeDef = TypedDict(
+    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
+    {
+        "Runs": List[DataQualityRulesetEvaluationRunDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef = TypedDict(
+    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
+    {
+        "Filter": DataQualityRulesetEvaluationRunFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 _RequiredCreateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatabaseRequestRequestTypeDef",
     {
         "DatabaseInput": DatabaseInputTypeDef,
     },
 )
 _OptionalCreateDatabaseRequestRequestTypeDef = TypedDict(
@@ -7818,24 +8899,24 @@
 ):
     pass
 
 GetDatabaseResponseTypeDef = TypedDict(
     "GetDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDatabasesResponseTypeDef = TypedDict(
     "GetDatabasesResponseTypeDef",
     {
         "DatabaseList": List[DatabaseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ColumnStatisticsTypeDef = TypedDict(
     "ColumnStatisticsTypeDef",
     {
         "ColumnName": str,
@@ -7925,35 +9006,36 @@
         "TableType": str,
         "Parameters": Dict[str, str],
         "CreatedBy": str,
         "IsRegisteredWithLakeFormation": bool,
         "TargetTable": TableIdentifierTypeDef,
         "CatalogId": str,
         "VersionId": str,
+        "FederatedTable": FederatedTableTypeDef,
     },
     total=False,
 )
 
 class TableTypeDef(_RequiredTableTypeDef, _OptionalTableTypeDef):
     pass
 
 GetSecurityConfigurationResponseTypeDef = TypedDict(
     "GetSecurityConfigurationResponseTypeDef",
     {
         "SecurityConfiguration": SecurityConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSecurityConfigurationsResponseTypeDef = TypedDict(
     "GetSecurityConfigurationsResponseTypeDef",
     {
         "SecurityConfigurations": List[SecurityConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CodeGenConfigurationNodeTypeDef = TypedDict(
     "CodeGenConfigurationNodeTypeDef",
     {
         "AthenaConnectorSource": AthenaConnectorSourceTypeDef,
@@ -8002,41 +9084,57 @@
         "MySQLCatalogSource": MySQLCatalogSourceTypeDef,
         "OracleSQLCatalogSource": OracleSQLCatalogSourceTypeDef,
         "PostgreSQLCatalogSource": PostgreSQLCatalogSourceTypeDef,
         "MicrosoftSQLServerCatalogTarget": MicrosoftSQLServerCatalogTargetTypeDef,
         "MySQLCatalogTarget": MySQLCatalogTargetTypeDef,
         "OracleSQLCatalogTarget": OracleSQLCatalogTargetTypeDef,
         "PostgreSQLCatalogTarget": PostgreSQLCatalogTargetTypeDef,
+        "DynamicTransform": DynamicTransformTypeDef,
+        "EvaluateDataQuality": EvaluateDataQualityTypeDef,
+        "S3CatalogHudiSource": S3CatalogHudiSourceTypeDef,
+        "CatalogHudiSource": CatalogHudiSourceTypeDef,
+        "S3HudiSource": S3HudiSourceTypeDef,
+        "S3HudiCatalogTarget": S3HudiCatalogTargetTypeDef,
+        "S3HudiDirectTarget": S3HudiDirectTargetTypeDef,
+        "DirectJDBCSource": DirectJDBCSourceTypeDef,
+        "S3CatalogDeltaSource": S3CatalogDeltaSourceTypeDef,
+        "CatalogDeltaSource": CatalogDeltaSourceTypeDef,
+        "S3DeltaSource": S3DeltaSourceTypeDef,
+        "S3DeltaCatalogTarget": S3DeltaCatalogTargetTypeDef,
+        "S3DeltaDirectTarget": S3DeltaDirectTargetTypeDef,
+        "AmazonRedshiftSource": AmazonRedshiftSourceTypeDef,
+        "AmazonRedshiftTarget": AmazonRedshiftTargetTypeDef,
+        "EvaluateDataQualityMultiFrame": EvaluateDataQualityMultiFrameTypeDef,
     },
     total=False,
 )
 
 GetMLTaskRunsResponseTypeDef = TypedDict(
     "GetMLTaskRunsResponseTypeDef",
     {
         "TaskRuns": List[TaskRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetStatementResponseTypeDef = TypedDict(
     "GetStatementResponseTypeDef",
     {
         "Statement": StatementTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListStatementsResponseTypeDef = TypedDict(
     "ListStatementsResponseTypeDef",
     {
         "Statements": List[StatementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "Type": NodeTypeType,
@@ -8050,15 +9148,15 @@
 )
 
 GetMLTransformsResponseTypeDef = TypedDict(
     "GetMLTransformsResponseTypeDef",
     {
         "Transforms": List[MLTransformTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ColumnStatisticsErrorTypeDef = TypedDict(
     "ColumnStatisticsErrorTypeDef",
     {
         "ColumnStatistics": ColumnStatisticsTypeDef,
@@ -8068,24 +9166,24 @@
 )
 
 GetColumnStatisticsForPartitionResponseTypeDef = TypedDict(
     "GetColumnStatisticsForPartitionResponseTypeDef",
     {
         "ColumnStatisticsList": List[ColumnStatisticsTypeDef],
         "Errors": List[ColumnErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetColumnStatisticsForTableResponseTypeDef = TypedDict(
     "GetColumnStatisticsForTableResponseTypeDef",
     {
         "ColumnStatisticsList": List[ColumnStatisticsTypeDef],
         "Errors": List[ColumnErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -8204,42 +9302,42 @@
     pass
 
 BatchGetPartitionResponseTypeDef = TypedDict(
     "BatchGetPartitionResponseTypeDef",
     {
         "Partitions": List[PartitionTypeDef],
         "UnprocessedKeys": List[PartitionValueListTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPartitionResponseTypeDef = TypedDict(
     "GetPartitionResponseTypeDef",
     {
         "Partition": PartitionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPartitionsResponseTypeDef = TypedDict(
     "GetPartitionsResponseTypeDef",
     {
         "Partitions": List[PartitionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUnfilteredPartitionMetadataResponseTypeDef = TypedDict(
     "GetUnfilteredPartitionMetadataResponseTypeDef",
     {
         "Partition": PartitionTypeDef,
         "AuthorizedColumns": List[str],
         "IsRegisteredWithLakeFormation": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UnfilteredPartitionTypeDef = TypedDict(
     "UnfilteredPartitionTypeDef",
     {
         "Partition": PartitionTypeDef,
@@ -8294,44 +9392,44 @@
 ):
     pass
 
 GetTableResponseTypeDef = TypedDict(
     "GetTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTablesResponseTypeDef = TypedDict(
     "GetTablesResponseTypeDef",
     {
         "TableList": List[TableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUnfilteredTableMetadataResponseTypeDef = TypedDict(
     "GetUnfilteredTableMetadataResponseTypeDef",
     {
         "Table": TableTypeDef,
         "AuthorizedColumns": List[str],
         "IsRegisteredWithLakeFormation": bool,
         "CellFilters": List[ColumnRowFilterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SearchTablesResponseTypeDef = TypedDict(
     "SearchTablesResponseTypeDef",
     {
         "NextToken": str,
         "TableList": List[TableTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TableVersionTypeDef = TypedDict(
     "TableVersionTypeDef",
     {
         "Table": TableTypeDef,
@@ -8445,23 +9543,23 @@
     total=False,
 )
 
 UpdateColumnStatisticsForPartitionResponseTypeDef = TypedDict(
     "UpdateColumnStatisticsForPartitionResponseTypeDef",
     {
         "Errors": List[ColumnStatisticsErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateColumnStatisticsForTableResponseTypeDef = TypedDict(
     "UpdateColumnStatisticsForTableResponseTypeDef",
     {
         "Errors": List[ColumnStatisticsErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBatchUpdatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchUpdatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -8484,58 +9582,58 @@
     pass
 
 GetUnfilteredPartitionsMetadataResponseTypeDef = TypedDict(
     "GetUnfilteredPartitionsMetadataResponseTypeDef",
     {
         "UnfilteredPartitions": List[UnfilteredPartitionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTableVersionResponseTypeDef = TypedDict(
     "GetTableVersionResponseTypeDef",
     {
         "TableVersion": TableVersionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetTableVersionsResponseTypeDef = TypedDict(
     "GetTableVersionsResponseTypeDef",
     {
         "TableVersions": List[TableVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetJobsResponseTypeDef = TypedDict(
     "BatchGetJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "JobsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobsResponseTypeDef = TypedDict(
     "GetJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateJobRequestRequestTypeDef = TypedDict(
     "UpdateJobRequestRequestTypeDef",
     {
         "JobName": str,
@@ -8561,24 +9659,24 @@
     total=False,
 )
 
 GetWorkflowRunResponseTypeDef = TypedDict(
     "GetWorkflowRunResponseTypeDef",
     {
         "Run": WorkflowRunTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWorkflowRunsResponseTypeDef = TypedDict(
     "GetWorkflowRunsResponseTypeDef",
     {
         "Runs": List[WorkflowRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WorkflowTypeDef = TypedDict(
     "WorkflowTypeDef",
     {
         "Name": str,
@@ -8595,18 +9693,18 @@
 )
 
 BatchGetWorkflowsResponseTypeDef = TypedDict(
     "BatchGetWorkflowsResponseTypeDef",
     {
         "Workflows": List[WorkflowTypeDef],
         "MissingWorkflows": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWorkflowResponseTypeDef = TypedDict(
     "GetWorkflowResponseTypeDef",
     {
         "Workflow": WorkflowTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/PKG-INFO` & `mypy-boto3-glue-1.27.0/mypy_boto3_glue.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glue
-Version: 1.26.8
-Summary: Type annotations for boto3.Glue 1.26.8 service generated with mypy-boto3-builder 7.11.10
+Version: 1.27.0
+Summary: Type annotations for boto3.Glue 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
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
 
 <a id="mypy-boto3-glue"></a>
 
 # mypy-boto3-glue
 
 [![PyPI - mypy-boto3-glue](https://img.shields.io/pypi/v/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glue?color=blue)](https://pypistats.org/packages/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
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
 [mypy-boto3-glue docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,14 +346,15 @@
 ### Literals
 
 `mypy_boto3_glue.literals` module contains literals extracted from shapes that
 can be used in user code for type checking.
 
 ```python
 from mypy_boto3_glue.literals import (
+    AdditionalOptionKeysType,
     AggFunctionType,
     BackfillErrorCodeType,
     BlueprintRunStateType,
     BlueprintStatusType,
     CatalogEncryptionModeType,
     CloudWatchEncryptionModeType,
     ColumnStatisticsTypeType,
@@ -362,16 +364,20 @@
     ConnectionPropertyKeyType,
     ConnectionTypeType,
     CrawlStateType,
     CrawlerHistoryStateType,
     CrawlerLineageSettingsType,
     CrawlerStateType,
     CsvHeaderOptionType,
+    DQStopJobOnFailureTimingType,
+    DQTransformOutputType,
     DataFormatType,
+    DataQualityRuleResultStatusType,
     DeleteBehaviorType,
+    DeltaTargetCompressionTypeType,
     EnableHybridValuesType,
     ExecutionClassType,
     ExistConditionType,
     FieldNameType,
     FilterLogicalOperatorType,
     FilterOperationType,
     FilterOperatorType,
@@ -389,27 +395,31 @@
     GetResourcePoliciesPaginatorName,
     GetSecurityConfigurationsPaginatorName,
     GetTableVersionsPaginatorName,
     GetTablesPaginatorName,
     GetTriggersPaginatorName,
     GetUserDefinedFunctionsPaginatorName,
     GlueRecordTypeType,
+    HudiTargetCompressionTypeType,
+    JDBCConnectionTypeType,
     JDBCDataTypeType,
+    JdbcMetadataEntryType,
     JobBookmarksEncryptionModeType,
     JobRunStateType,
     JoinTypeType,
     LanguageType,
     LastCrawlStatusType,
     ListRegistriesPaginatorName,
     ListSchemaVersionsPaginatorName,
     ListSchemasPaginatorName,
     LogicalOperatorType,
     LogicalType,
     MLUserDataEncryptionModeStringType,
     NodeTypeType,
+    ParamTypeType,
     ParquetCompressionTypeType,
     PartitionIndexStatusType,
     PermissionType,
     PermissionTypeType,
     PiiTypeType,
     PrincipalTypeType,
     QuoteCharType,
@@ -448,70 +458,77 @@
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: AggFunctionType) -> bool:
+def check_value(value: AdditionalOptionKeysType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_glue.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_glue.type_defs import (
     NotificationPropertyTypeDef,
     AggregateOperationTypeDef,
+    AmazonRedshiftAdvancedOptionTypeDef,
+    OptionTypeDef,
     ApplyMappingTypeDef,
     AuditContextTypeDef,
     PartitionValueListTypeDef,
     BasicCatalogTargetTypeDef,
-    ResponseMetadataTypeDef,
     BatchDeleteConnectionRequestRequestTypeDef,
     ErrorDetailTypeDef,
     BatchDeleteTableRequestRequestTypeDef,
     BatchDeleteTableVersionRequestRequestTypeDef,
     BatchGetBlueprintsRequestRequestTypeDef,
     BatchGetCrawlersRequestRequestTypeDef,
     BatchGetCustomEntityTypesRequestRequestTypeDef,
     CustomEntityTypeTypeDef,
+    BatchGetDataQualityResultRequestRequestTypeDef,
     BatchGetDevEndpointsRequestRequestTypeDef,
     DevEndpointTypeDef,
     BatchGetJobsRequestRequestTypeDef,
     BatchGetTriggersRequestRequestTypeDef,
     BatchGetWorkflowsRequestRequestTypeDef,
     BatchStopJobRunRequestRequestTypeDef,
     BatchStopJobRunSuccessfulSubmissionTypeDef,
     BinaryColumnStatisticsDataTypeDef,
     BlueprintDetailsTypeDef,
     BlueprintRunTypeDef,
     LastActiveDefinitionTypeDef,
     BooleanColumnStatisticsDataTypeDef,
+    CancelDataQualityRuleRecommendationRunRequestRequestTypeDef,
+    CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     CancelMLTaskRunRequestRequestTypeDef,
+    CancelMLTaskRunResponseTypeDef,
     CancelStatementRequestRequestTypeDef,
     CatalogEntryTypeDef,
     CatalogImportStatusTypeDef,
     KafkaStreamingSourceOptionsTypeDef,
     StreamingDataPreviewOptionsTypeDef,
     KinesisStreamingSourceOptionsTypeDef,
     CatalogSchemaChangePolicyTypeDef,
     CatalogSourceTypeDef,
     CatalogTargetTypeDef,
     CheckSchemaVersionValidityInputRequestTypeDef,
+    CheckSchemaVersionValidityResponseTypeDef,
     CsvClassifierTypeDef,
     GrokClassifierTypeDef,
     JsonClassifierTypeDef,
     XMLClassifierTypeDef,
     CloudWatchEncryptionTypeDef,
+    DirectJDBCSourceTypeDef,
     DropDuplicatesTypeDef,
     DropFieldsTypeDef,
     DynamoDBCatalogSourceTypeDef,
     FillMissingValuesTypeDef,
     MergeTypeDef,
     MicrosoftSQLServerCatalogSourceTypeDef,
     MicrosoftSQLServerCatalogTargetTypeDef,
@@ -545,277 +562,311 @@
     ConnectionPasswordEncryptionTypeDef,
     ConnectionsListTypeDef,
     CrawlTypeDef,
     CrawlerHistoryTypeDef,
     CrawlerMetricsTypeDef,
     DeltaTargetTypeDef,
     DynamoDBTargetTypeDef,
+    IcebergTargetTypeDef,
     JdbcTargetTypeDef,
     MongoDBTargetTypeDef,
     S3TargetTypeDef,
     LakeFormationConfigurationTypeDef,
     LastCrawlInfoTypeDef,
     LineageConfigurationTypeDef,
     RecrawlPolicyTypeDef,
     ScheduleTypeDef,
     SchemaChangePolicyTypeDef,
     CrawlsFilterTypeDef,
     CreateBlueprintRequestRequestTypeDef,
+    CreateBlueprintResponseTypeDef,
     CreateCsvClassifierRequestTypeDef,
     CreateGrokClassifierRequestTypeDef,
     CreateJsonClassifierRequestTypeDef,
     CreateXMLClassifierRequestTypeDef,
     CreateCustomEntityTypeRequestRequestTypeDef,
+    CreateCustomEntityTypeResponseTypeDef,
+    DataQualityTargetTableTypeDef,
+    CreateDataQualityRulesetResponseTypeDef,
     CreateDevEndpointRequestRequestTypeDef,
+    CreateDevEndpointResponseTypeDef,
     ExecutionPropertyTypeDef,
     JobCommandTypeDef,
     SourceControlDetailsTypeDef,
+    CreateJobResponseTypeDef,
     GlueTableTypeDef,
+    CreateMLTransformResponseTypeDef,
     PartitionIndexTypeDef,
     CreateRegistryInputRequestTypeDef,
+    CreateRegistryResponseTypeDef,
     RegistryIdTypeDef,
+    CreateSchemaResponseTypeDef,
+    CreateScriptResponseTypeDef,
+    CreateSecurityConfigurationResponseTypeDef,
     SessionCommandTypeDef,
     EventBatchingConditionTypeDef,
+    CreateTriggerResponseTypeDef,
     CreateWorkflowRequestRequestTypeDef,
+    CreateWorkflowResponseTypeDef,
+    DQResultsPublishingOptionsTypeDef,
+    DQStopJobOnFailureOptionsTypeDef,
     EncryptionAtRestTypeDef,
     DataLakePrincipalTypeDef,
+    DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
+    DataQualityRuleResultTypeDef,
     DatabaseIdentifierTypeDef,
+    FederatedDatabaseTypeDef,
     DatatypeTypeDef,
     DecimalNumberTypeDef,
     DeleteBlueprintRequestRequestTypeDef,
+    DeleteBlueprintResponseTypeDef,
     DeleteClassifierRequestRequestTypeDef,
     DeleteColumnStatisticsForPartitionRequestRequestTypeDef,
     DeleteColumnStatisticsForTableRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteCrawlerRequestRequestTypeDef,
     DeleteCustomEntityTypeRequestRequestTypeDef,
+    DeleteCustomEntityTypeResponseTypeDef,
+    DeleteDataQualityRulesetRequestRequestTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteDevEndpointRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
+    DeleteJobResponseTypeDef,
     DeleteMLTransformRequestRequestTypeDef,
+    DeleteMLTransformResponseTypeDef,
     DeletePartitionIndexRequestRequestTypeDef,
     DeletePartitionRequestRequestTypeDef,
+    DeleteRegistryResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     SchemaIdTypeDef,
+    DeleteSchemaResponseTypeDef,
     DeleteSecurityConfigurationRequestRequestTypeDef,
     DeleteSessionRequestRequestTypeDef,
+    DeleteSessionResponseTypeDef,
     DeleteTableRequestRequestTypeDef,
     DeleteTableVersionRequestRequestTypeDef,
     DeleteTriggerRequestRequestTypeDef,
+    DeleteTriggerResponseTypeDef,
     DeleteUserDefinedFunctionRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
+    DeleteWorkflowResponseTypeDef,
     DevEndpointCustomLibrariesTypeDef,
     DirectSchemaChangePolicyTypeDef,
     NullCheckBoxListTypeDef,
+    TransformConfigParameterTypeDef,
     EdgeTypeDef,
     JobBookmarksEncryptionTypeDef,
     S3EncryptionTypeDef,
     ErrorDetailsTypeDef,
     ExportLabelsTaskRunPropertiesTypeDef,
+    FederatedTableTypeDef,
     FilterValueTypeDef,
     FindMatchesParametersTypeDef,
     FindMatchesTaskRunPropertiesTypeDef,
     GetBlueprintRequestRequestTypeDef,
     GetBlueprintRunRequestRequestTypeDef,
     GetBlueprintRunsRequestRequestTypeDef,
     GetCatalogImportStatusRequestRequestTypeDef,
     GetClassifierRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    GetClassifiersRequestGetClassifiersPaginateTypeDef,
     GetClassifiersRequestRequestTypeDef,
     GetColumnStatisticsForPartitionRequestRequestTypeDef,
     GetColumnStatisticsForTableRequestRequestTypeDef,
     GetConnectionRequestRequestTypeDef,
     GetConnectionsFilterTypeDef,
+    GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef,
     GetCrawlerMetricsRequestRequestTypeDef,
     GetCrawlerRequestRequestTypeDef,
+    GetCrawlersRequestGetCrawlersPaginateTypeDef,
     GetCrawlersRequestRequestTypeDef,
     GetCustomEntityTypeRequestRequestTypeDef,
+    GetCustomEntityTypeResponseTypeDef,
     GetDataCatalogEncryptionSettingsRequestRequestTypeDef,
+    GetDataQualityResultRequestRequestTypeDef,
+    GetDataQualityRuleRecommendationRunRequestRequestTypeDef,
+    GetDataQualityRulesetEvaluationRunRequestRequestTypeDef,
+    GetDataQualityRulesetRequestRequestTypeDef,
     GetDatabaseRequestRequestTypeDef,
+    GetDatabasesRequestGetDatabasesPaginateTypeDef,
     GetDatabasesRequestRequestTypeDef,
     GetDataflowGraphRequestRequestTypeDef,
     GetDevEndpointRequestRequestTypeDef,
+    GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef,
     GetDevEndpointsRequestRequestTypeDef,
     GetJobBookmarkRequestRequestTypeDef,
     JobBookmarkEntryTypeDef,
     GetJobRequestRequestTypeDef,
     GetJobRunRequestRequestTypeDef,
+    GetJobRunsRequestGetJobRunsPaginateTypeDef,
     GetJobRunsRequestRequestTypeDef,
+    GetJobsRequestGetJobsPaginateTypeDef,
     GetJobsRequestRequestTypeDef,
     GetMLTaskRunRequestRequestTypeDef,
     TaskRunFilterCriteriaTypeDef,
     TaskRunSortCriteriaTypeDef,
     GetMLTransformRequestRequestTypeDef,
     SchemaColumnTypeDef,
     TransformSortCriteriaTypeDef,
     MappingEntryTypeDef,
+    GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
     GetPartitionIndexesRequestRequestTypeDef,
     GetPartitionRequestRequestTypeDef,
     SegmentTypeDef,
+    GetPlanResponseTypeDef,
+    GetRegistryResponseTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GluePolicyTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetSchemaByDefinitionResponseTypeDef,
+    GetSchemaResponseTypeDef,
     SchemaVersionNumberTypeDef,
+    GetSchemaVersionResponseTypeDef,
+    GetSchemaVersionsDiffResponseTypeDef,
     GetSecurityConfigurationRequestRequestTypeDef,
+    GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef,
     GetSecurityConfigurationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
     GetStatementRequestRequestTypeDef,
     GetTableRequestRequestTypeDef,
     GetTableVersionRequestRequestTypeDef,
+    GetTableVersionsRequestGetTableVersionsPaginateTypeDef,
     GetTableVersionsRequestRequestTypeDef,
+    GetTablesRequestGetTablesPaginateTypeDef,
     GetTablesRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
+    GetTagsResponseTypeDef,
     GetTriggerRequestRequestTypeDef,
+    GetTriggersRequestGetTriggersPaginateTypeDef,
     GetTriggersRequestRequestTypeDef,
     GetUserDefinedFunctionRequestRequestTypeDef,
+    GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
     GetUserDefinedFunctionsRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowRunPropertiesRequestRequestTypeDef,
+    GetWorkflowRunPropertiesResponseTypeDef,
     GetWorkflowRunRequestRequestTypeDef,
     GetWorkflowRunsRequestRequestTypeDef,
     GlueStudioSchemaColumnTypeDef,
     S3SourceAdditionalOptionsTypeDef,
     ImportCatalogToGlueRequestRequestTypeDef,
     ImportLabelsTaskRunPropertiesTypeDef,
     JDBCConnectorOptionsTypeDef,
     PredecessorTypeDef,
     JoinColumnTypeDef,
     KeySchemaElementTypeDef,
     LabelingSetGenerationTaskRunPropertiesTypeDef,
     ListBlueprintsRequestRequestTypeDef,
+    ListBlueprintsResponseTypeDef,
     ListCrawlersRequestRequestTypeDef,
+    ListCrawlersResponseTypeDef,
     ListCustomEntityTypesRequestRequestTypeDef,
     ListDevEndpointsRequestRequestTypeDef,
+    ListDevEndpointsResponseTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListJobsResponseTypeDef,
+    ListMLTransformsResponseTypeDef,
+    ListRegistriesInputListRegistriesPaginateTypeDef,
     ListRegistriesInputRequestTypeDef,
     RegistryListItemTypeDef,
     SchemaVersionListItemTypeDef,
     SchemaListItemTypeDef,
     ListSessionsRequestRequestTypeDef,
     ListStatementsRequestRequestTypeDef,
     ListTriggersRequestRequestTypeDef,
+    ListTriggersResponseTypeDef,
     ListWorkflowsRequestRequestTypeDef,
+    ListWorkflowsResponseTypeDef,
     MLUserDataEncryptionTypeDef,
     MappingTypeDef,
     OtherMetadataValueListItemTypeDef,
     MetadataKeyValuePairTypeDef,
     OrderTypeDef,
+    PaginatorConfigTypeDef,
     PropertyPredicateTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    PutSchemaVersionMetadataResponseTypeDef,
     PutWorkflowRunPropertiesRequestRequestTypeDef,
     UpsertRedshiftTargetOptionsTypeDef,
+    RegisterSchemaVersionResponseTypeDef,
+    RemoveSchemaVersionMetadataResponseTypeDef,
     ResetJobBookmarkRequestRequestTypeDef,
     ResourceUriTypeDef,
+    ResponseMetadataTypeDef,
     ResumeWorkflowRunRequestRequestTypeDef,
+    ResumeWorkflowRunResponseTypeDef,
     RunStatementRequestRequestTypeDef,
+    RunStatementResponseTypeDef,
     S3DirectSourceAdditionalOptionsTypeDef,
     SortCriterionTypeDef,
     SerDeInfoTypeDef,
     SkewedInfoTypeDef,
     SqlAliasTypeDef,
     StartBlueprintRunRequestRequestTypeDef,
+    StartBlueprintRunResponseTypeDef,
     StartCrawlerRequestRequestTypeDef,
     StartCrawlerScheduleRequestRequestTypeDef,
+    StartDataQualityRuleRecommendationRunResponseTypeDef,
+    StartDataQualityRulesetEvaluationRunResponseTypeDef,
     StartExportLabelsTaskRunRequestRequestTypeDef,
+    StartExportLabelsTaskRunResponseTypeDef,
     StartImportLabelsTaskRunRequestRequestTypeDef,
+    StartImportLabelsTaskRunResponseTypeDef,
+    StartJobRunResponseTypeDef,
     StartMLEvaluationTaskRunRequestRequestTypeDef,
+    StartMLEvaluationTaskRunResponseTypeDef,
     StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef,
+    StartMLLabelingSetGenerationTaskRunResponseTypeDef,
     StartTriggerRequestRequestTypeDef,
+    StartTriggerResponseTypeDef,
     StartWorkflowRunRequestRequestTypeDef,
+    StartWorkflowRunResponseTypeDef,
     StartingEventBatchConditionTypeDef,
     StatementOutputDataTypeDef,
     StopCrawlerRequestRequestTypeDef,
     StopCrawlerScheduleRequestRequestTypeDef,
     StopSessionRequestRequestTypeDef,
+    StopSessionResponseTypeDef,
     StopTriggerRequestRequestTypeDef,
+    StopTriggerResponseTypeDef,
     StopWorkflowRunRequestRequestTypeDef,
     TableIdentifierTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBlueprintRequestRequestTypeDef,
+    UpdateBlueprintResponseTypeDef,
     UpdateCsvClassifierRequestTypeDef,
     UpdateGrokClassifierRequestTypeDef,
     UpdateJsonClassifierRequestTypeDef,
     UpdateXMLClassifierRequestTypeDef,
     UpdateCrawlerScheduleRequestRequestTypeDef,
+    UpdateDataQualityRulesetRequestRequestTypeDef,
+    UpdateDataQualityRulesetResponseTypeDef,
     UpdateJobFromSourceControlRequestRequestTypeDef,
+    UpdateJobFromSourceControlResponseTypeDef,
+    UpdateJobResponseTypeDef,
+    UpdateMLTransformResponseTypeDef,
+    UpdateRegistryResponseTypeDef,
+    UpdateSchemaResponseTypeDef,
     UpdateSourceControlFromJobRequestRequestTypeDef,
+    UpdateSourceControlFromJobResponseTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
+    UpdateWorkflowResponseTypeDef,
     WorkflowRunStatisticsTypeDef,
     ActionTypeDef,
     StartJobRunRequestRequestTypeDef,
     AggregateTypeDef,
+    AmazonRedshiftNodeDataTypeDef,
     GetUnfilteredPartitionMetadataRequestRequestTypeDef,
     GetUnfilteredTableMetadataRequestRequestTypeDef,
     BackfillErrorTypeDef,
     BatchDeletePartitionRequestRequestTypeDef,
     BatchGetPartitionRequestRequestTypeDef,
-    CancelMLTaskRunResponseTypeDef,
-    CheckSchemaVersionValidityResponseTypeDef,
-    CreateBlueprintResponseTypeDef,
-    CreateCustomEntityTypeResponseTypeDef,
-    CreateDevEndpointResponseTypeDef,
-    CreateJobResponseTypeDef,
-    CreateMLTransformResponseTypeDef,
-    CreateRegistryResponseTypeDef,
-    CreateSchemaResponseTypeDef,
-    CreateScriptResponseTypeDef,
-    CreateSecurityConfigurationResponseTypeDef,
-    CreateTriggerResponseTypeDef,
-    CreateWorkflowResponseTypeDef,
-    DeleteBlueprintResponseTypeDef,
-    DeleteCustomEntityTypeResponseTypeDef,
-    DeleteJobResponseTypeDef,
-    DeleteMLTransformResponseTypeDef,
-    DeleteRegistryResponseTypeDef,
-    DeleteSchemaResponseTypeDef,
-    DeleteSessionResponseTypeDef,
-    DeleteTriggerResponseTypeDef,
-    DeleteWorkflowResponseTypeDef,
-    GetCustomEntityTypeResponseTypeDef,
-    GetPlanResponseTypeDef,
-    GetRegistryResponseTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    GetSchemaByDefinitionResponseTypeDef,
-    GetSchemaResponseTypeDef,
-    GetSchemaVersionResponseTypeDef,
-    GetSchemaVersionsDiffResponseTypeDef,
-    GetTagsResponseTypeDef,
-    GetWorkflowRunPropertiesResponseTypeDef,
-    ListBlueprintsResponseTypeDef,
-    ListCrawlersResponseTypeDef,
-    ListDevEndpointsResponseTypeDef,
-    ListJobsResponseTypeDef,
-    ListMLTransformsResponseTypeDef,
-    ListTriggersResponseTypeDef,
-    ListWorkflowsResponseTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    PutSchemaVersionMetadataResponseTypeDef,
-    RegisterSchemaVersionResponseTypeDef,
-    RemoveSchemaVersionMetadataResponseTypeDef,
-    ResumeWorkflowRunResponseTypeDef,
-    RunStatementResponseTypeDef,
-    StartBlueprintRunResponseTypeDef,
-    StartExportLabelsTaskRunResponseTypeDef,
-    StartImportLabelsTaskRunResponseTypeDef,
-    StartJobRunResponseTypeDef,
-    StartMLEvaluationTaskRunResponseTypeDef,
-    StartMLLabelingSetGenerationTaskRunResponseTypeDef,
-    StartTriggerResponseTypeDef,
-    StartWorkflowRunResponseTypeDef,
-    StopSessionResponseTypeDef,
-    StopTriggerResponseTypeDef,
-    UpdateBlueprintResponseTypeDef,
-    UpdateJobFromSourceControlResponseTypeDef,
-    UpdateJobResponseTypeDef,
-    UpdateMLTransformResponseTypeDef,
-    UpdateRegistryResponseTypeDef,
-    UpdateSchemaResponseTypeDef,
-    UpdateSourceControlFromJobResponseTypeDef,
-    UpdateWorkflowResponseTypeDef,
     BatchDeleteConnectionResponseTypeDef,
     BatchStopJobRunErrorTypeDef,
     BatchUpdatePartitionFailureEntryTypeDef,
     ColumnErrorTypeDef,
     PartitionErrorTypeDef,
     TableErrorTypeDef,
     TableVersionErrorTypeDef,
@@ -830,70 +881,66 @@
     GetCatalogImportStatusResponseTypeDef,
     CatalogKafkaSourceTypeDef,
     DirectKafkaSourceTypeDef,
     CatalogKinesisSourceTypeDef,
     DirectKinesisSourceTypeDef,
     GovernedCatalogTargetTypeDef,
     S3CatalogTargetTypeDef,
+    S3DeltaCatalogTargetTypeDef,
+    S3HudiCatalogTargetTypeDef,
     ClassifierTypeDef,
     CodeGenNodeTypeDef,
     LocationTypeDef,
     PredicateTypeDef,
     FindMatchesMetricsTypeDef,
     ConnectionInputTypeDef,
     ConnectionTypeDef,
     CrawlerNodeDetailsTypeDef,
     ListCrawlsResponseTypeDef,
     GetCrawlerMetricsResponseTypeDef,
     CrawlerTargetsTypeDef,
     ListCrawlsRequestRequestTypeDef,
     CreateClassifierRequestRequestTypeDef,
+    CreateDataQualityRulesetRequestRequestTypeDef,
+    DataQualityRulesetFilterCriteriaTypeDef,
+    DataQualityRulesetListDetailsTypeDef,
+    GetDataQualityRulesetResponseTypeDef,
+    DataSourceTypeDef,
     CreatePartitionIndexRequestRequestTypeDef,
     CreateSchemaInputRequestTypeDef,
     DeleteRegistryInputRequestTypeDef,
     GetRegistryInputRequestTypeDef,
+    ListSchemasInputListSchemasPaginateTypeDef,
     ListSchemasInputRequestTypeDef,
     UpdateRegistryInputRequestTypeDef,
     CreateSessionRequestRequestTypeDef,
     SessionTypeDef,
+    EvaluateDataQualityMultiFrameTypeDef,
+    EvaluateDataQualityTypeDef,
     DataCatalogEncryptionSettingsTypeDef,
     PrincipalPermissionsTypeDef,
     NullValueFieldTypeDef,
     DecimalColumnStatisticsDataTypeDef,
     DeleteSchemaInputRequestTypeDef,
     DeleteSchemaVersionsInputRequestTypeDef,
     GetSchemaByDefinitionInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
+    ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
     ListSchemaVersionsInputRequestTypeDef,
     RegisterSchemaVersionInputRequestTypeDef,
     SchemaReferenceTypeDef,
     UpdateDevEndpointRequestRequestTypeDef,
+    S3DeltaDirectTargetTypeDef,
     S3DirectTargetTypeDef,
     S3GlueParquetTargetTypeDef,
+    S3HudiDirectTargetTypeDef,
     EncryptionConfigurationTypeDef,
     SchemaVersionErrorItemTypeDef,
     FilterExpressionTypeDef,
     TransformParametersTypeDef,
-    GetClassifiersRequestGetClassifiersPaginateTypeDef,
-    GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef,
-    GetCrawlersRequestGetCrawlersPaginateTypeDef,
-    GetDatabasesRequestGetDatabasesPaginateTypeDef,
-    GetDevEndpointsRequestGetDevEndpointsPaginateTypeDef,
-    GetJobRunsRequestGetJobRunsPaginateTypeDef,
-    GetJobsRequestGetJobsPaginateTypeDef,
-    GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    GetSecurityConfigurationsRequestGetSecurityConfigurationsPaginateTypeDef,
-    GetTableVersionsRequestGetTableVersionsPaginateTypeDef,
-    GetTablesRequestGetTablesPaginateTypeDef,
-    GetTriggersRequestGetTriggersPaginateTypeDef,
-    GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
-    ListRegistriesInputListRegistriesPaginateTypeDef,
-    ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
-    ListSchemasInputListSchemasPaginateTypeDef,
     GetConnectionsRequestGetConnectionsPaginateTypeDef,
     GetConnectionsRequestRequestTypeDef,
     GetJobBookmarkResponseTypeDef,
     ResetJobBookmarkResponseTypeDef,
     GetMLTaskRunsRequestRequestTypeDef,
     TransformFilterCriteriaTypeDef,
     GetMappingResponseTypeDef,
@@ -920,14 +967,16 @@
     RemoveSchemaVersionMetadataInputRequestTypeDef,
     RedshiftTargetTypeDef,
     UserDefinedFunctionInputTypeDef,
     UserDefinedFunctionTypeDef,
     SearchTablesRequestRequestTypeDef,
     StatementOutputTypeDef,
     UpdateClassifierRequestRequestTypeDef,
+    AmazonRedshiftSourceTypeDef,
+    AmazonRedshiftTargetTypeDef,
     PartitionIndexDescriptorTypeDef,
     BatchStopJobRunResponseTypeDef,
     BatchUpdatePartitionResponseTypeDef,
     BatchCreatePartitionResponseTypeDef,
     BatchDeletePartitionResponseTypeDef,
     BatchDeleteTableResponseTypeDef,
     BatchDeleteTableVersionResponseTypeDef,
@@ -946,14 +995,28 @@
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     GetConnectionResponseTypeDef,
     GetConnectionsResponseTypeDef,
     CrawlerTypeDef,
     CreateCrawlerRequestRequestTypeDef,
     UpdateCrawlerRequestRequestTypeDef,
+    ListDataQualityRulesetsRequestRequestTypeDef,
+    ListDataQualityRulesetsResponseTypeDef,
+    DataQualityResultDescriptionTypeDef,
+    DataQualityResultFilterCriteriaTypeDef,
+    DataQualityResultTypeDef,
+    DataQualityRuleRecommendationRunDescriptionTypeDef,
+    DataQualityRuleRecommendationRunFilterTypeDef,
+    DataQualityRulesetEvaluationRunDescriptionTypeDef,
+    DataQualityRulesetEvaluationRunFilterTypeDef,
+    GetDataQualityResultResponseTypeDef,
+    GetDataQualityRuleRecommendationRunResponseTypeDef,
+    GetDataQualityRulesetEvaluationRunResponseTypeDef,
+    StartDataQualityRuleRecommendationRunRequestRequestTypeDef,
+    StartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     CreateSessionResponseTypeDef,
     GetSessionResponseTypeDef,
     ListSessionsResponseTypeDef,
     GetDataCatalogEncryptionSettingsResponseTypeDef,
     PutDataCatalogEncryptionSettingsRequestRequestTypeDef,
     DatabaseInputTypeDef,
     DatabaseTypeDef,
@@ -964,18 +1027,25 @@
     SecurityConfigurationTypeDef,
     DeleteSchemaVersionsResponseTypeDef,
     FilterTypeDef,
     UpdateMLTransformRequestRequestTypeDef,
     GetMLTransformsRequestRequestTypeDef,
     ListMLTransformsRequestRequestTypeDef,
     AthenaConnectorSourceTypeDef,
+    CatalogDeltaSourceTypeDef,
+    CatalogHudiSourceTypeDef,
     CustomCodeTypeDef,
+    DynamicTransformTypeDef,
     JDBCConnectorSourceTypeDef,
     JDBCConnectorTargetTypeDef,
+    S3CatalogDeltaSourceTypeDef,
+    S3CatalogHudiSourceTypeDef,
     S3CsvSourceTypeDef,
+    S3DeltaSourceTypeDef,
+    S3HudiSourceTypeDef,
     S3JsonSourceTypeDef,
     S3ParquetSourceTypeDef,
     SparkConnectorSourceTypeDef,
     SparkConnectorTargetTypeDef,
     SparkSQLTypeDef,
     GetJobRunResponseTypeDef,
     GetJobRunsResponseTypeDef,
@@ -997,14 +1067,21 @@
     UpdateTriggerResponseTypeDef,
     UpdateTriggerRequestRequestTypeDef,
     GetMLTransformResponseTypeDef,
     MLTransformTypeDef,
     BatchGetCrawlersResponseTypeDef,
     GetCrawlerResponseTypeDef,
     GetCrawlersResponseTypeDef,
+    ListDataQualityResultsResponseTypeDef,
+    ListDataQualityResultsRequestRequestTypeDef,
+    BatchGetDataQualityResultResponseTypeDef,
+    ListDataQualityRuleRecommendationRunsResponseTypeDef,
+    ListDataQualityRuleRecommendationRunsRequestRequestTypeDef,
+    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
+    ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef,
     CreateDatabaseRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
     GetDatabaseResponseTypeDef,
     GetDatabasesResponseTypeDef,
     ColumnStatisticsTypeDef,
     PartitionInputTypeDef,
     PartitionTypeDef,
@@ -1069,42 +1146,42 @@
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

### Comparing `mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/SOURCES.txt` & `mypy-boto3-glue-1.27.0/mypy_boto3_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.26.8/setup.py` & `mypy-boto3-glue-1.27.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-glue.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-glue",
-    version="1.26.8",
+    version="1.27.0",
     packages=["mypy_boto3_glue"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Glue 1.26.8 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.Glue 1.27.0 service generated with mypy-boto3-builder 7.14.5"
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
     keywords="boto3 glue type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_glue": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_glue": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/",
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


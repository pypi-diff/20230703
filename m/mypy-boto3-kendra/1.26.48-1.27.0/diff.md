# Comparing `tmp/mypy-boto3-kendra-1.26.48.tar.gz` & `tmp/mypy-boto3-kendra-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kendra-1.26.48.tar", last modified: Wed Jan 11 20:26:39 2023, max compression
+gzip compressed data, was "mypy-boto3-kendra-1.27.0.tar", last modified: Mon Jul  3 19:50:57 2023, max compression
```

## Comparing `mypy-boto3-kendra-1.26.48.tar` & `mypy-boto3-kendra-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 20:26:39.945933 mypy-boto3-kendra-1.26.48/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-01-11 20:26:39.945933 mypy-boto3-kendra-1.26.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21105 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 20:26:39.945933 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43005 2023-01-11 20:26:28.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42939 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14745 2023-01-11 20:26:28.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14743 2023-01-11 20:26:28.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   100671 2023-01-11 20:26:31.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   100526 2023-01-11 20:26:29.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 20:26:39.945933 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-01-11 20:26:39.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-01-11 20:26:39.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 20:26:39.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 20:26:39.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-11 20:26:39.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-11 20:26:39.000000 mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 20:26:39.945933 mypy-boto3-kendra-1.26.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-01-11 20:26:27.000000 mypy-boto3-kendra-1.26.48/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.415484 mypy-boto3-kendra-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23685 2023-07-03 19:50:57.411484 mypy-boto3-kendra-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.407483 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47945 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47873 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-07-03 19:40:13.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   110862 2023-07-03 19:40:15.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110709 2023-07-03 19:40:14.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.411484 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23685 2023-07-03 19:50:57.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-03 19:50:57.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:57.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:57.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:57.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 19:50:57.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:57.415484 mypy-boto3-kendra-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/setup.py
```

### Comparing `mypy-boto3-kendra-1.26.48/LICENSE` & `mypy-boto3-kendra-1.27.0/LICENSE`

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

### Comparing `mypy-boto3-kendra-1.26.48/PKG-INFO` & `mypy-boto3-kendra-1.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kendra
-Version: 1.26.48
-Summary: Type annotations for boto3.kendra 1.26.48 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.kendra 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-kendra"></a>
 
 # mypy-boto3-kendra
 
 [![PyPI - mypy-boto3-kendra](https://img.shields.io/pypi/v/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kendra?color=blue)](https://pypistats.org/packages/mypy-boto3-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.kendra 1.26.48](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[boto3.kendra 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
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
 [mypy-boto3-kendra docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,14 +277,15 @@
 `mypy_boto3_kendra.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_kendra.literals import (
     AdditionalResultAttributeValueTypeType,
     AlfrescoEntityType,
+    AttributeSuggestionsModeType,
     ConditionOperatorType,
     ConfluenceAttachmentFieldNameType,
     ConfluenceAuthenticationTypeType,
     ConfluenceBlogFieldNameType,
     ConfluencePageFieldNameType,
     ConfluenceSpaceFieldNameType,
     ConfluenceVersionType,
@@ -297,14 +298,15 @@
     DocumentStatusType,
     EndpointTypeType,
     EntityTypeType,
     ErrorCodeType,
     ExperienceStatusType,
     FaqFileFormatType,
     FaqStatusType,
+    FeaturedResultsSetStatusType,
     FsxFileSystemTypeType,
     HighlightTypeType,
     IndexEditionType,
     IndexStatusType,
     IntervalType,
     IssueSubEntityType,
     KeyLocationType,
@@ -327,14 +329,15 @@
     ScoreConfidenceType,
     ServiceNowAuthenticationTypeType,
     ServiceNowBuildVersionTypeType,
     SharePointOnlineAuthenticationTypeType,
     SharePointVersionType,
     SlackEntityType,
     SortOrderType,
+    SuggestionTypeType,
     ThesaurusStatusType,
     TypeType,
     UserContextPolicyType,
     UserGroupResolutionModeType,
     WarningCodeType,
     WebCrawlerModeType,
     kendraServiceName,
@@ -361,19 +364,21 @@
     AccessControlListConfigurationTypeDef,
     AclConfigurationTypeDef,
     DataSourceToIndexFieldMappingTypeDef,
     DataSourceVpcConfigurationTypeDef,
     S3PathTypeDef,
     EntityConfigurationTypeDef,
     FailedEntityTypeDef,
-    ResponseMetadataTypeDef,
     EntityPersonaConfigurationTypeDef,
+    SuggestableConfigTypeDef,
     BasicAuthenticationConfigurationTypeDef,
     DataSourceSyncJobMetricTargetTypeDef,
     BatchDeleteDocumentResponseFailedDocumentTypeDef,
+    BatchDeleteFeaturedResultsSetErrorTypeDef,
+    BatchDeleteFeaturedResultsSetRequestRequestTypeDef,
     BatchGetDocumentStatusResponseErrorTypeDef,
     StatusTypeDef,
     BatchPutDocumentResponseFailedDocumentTypeDef,
     CapacityUnitsConfigurationTypeDef,
     ClearQuerySuggestionsRequestRequestTypeDef,
     ClickFeedbackTypeDef,
     ConfluenceAttachmentToIndexFieldMappingTypeDef,
@@ -381,17 +386,25 @@
     ProxyConfigurationTypeDef,
     ConfluencePageToIndexFieldMappingTypeDef,
     ConfluenceSpaceToIndexFieldMappingTypeDef,
     ConnectionConfigurationTypeDef,
     ContentSourceConfigurationTypeDef,
     CorrectionTypeDef,
     PrincipalTypeDef,
+    CreateAccessControlConfigurationResponseTypeDef,
     TagTypeDef,
+    CreateDataSourceResponseTypeDef,
+    CreateExperienceResponseTypeDef,
+    CreateFaqResponseTypeDef,
+    FeaturedDocumentTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     UserGroupResolutionConfigurationTypeDef,
+    CreateIndexResponseTypeDef,
+    CreateQuerySuggestionsBlockListResponseTypeDef,
+    CreateThesaurusResponseTypeDef,
     TemplateConfigurationTypeDef,
     DataSourceGroupTypeDef,
     DataSourceSummaryTypeDef,
     DataSourceSyncJobMetricsTypeDef,
     SqlConfigurationTypeDef,
     DeleteAccessControlConfigurationRequestRequestTypeDef,
     DeleteDataSourceRequestRequestTypeDef,
@@ -402,32 +415,36 @@
     DeleteQuerySuggestionsBlockListRequestRequestTypeDef,
     DeleteThesaurusRequestRequestTypeDef,
     DescribeAccessControlConfigurationRequestRequestTypeDef,
     DescribeDataSourceRequestRequestTypeDef,
     DescribeExperienceRequestRequestTypeDef,
     ExperienceEndpointTypeDef,
     DescribeFaqRequestRequestTypeDef,
+    DescribeFeaturedResultsSetRequestRequestTypeDef,
+    FeaturedDocumentMissingTypeDef,
+    FeaturedDocumentWithMetadataTypeDef,
     DescribeIndexRequestRequestTypeDef,
     DescribePrincipalMappingRequestRequestTypeDef,
     GroupOrderingIdSummaryTypeDef,
     DescribeQuerySuggestionsBlockListRequestRequestTypeDef,
     DescribeQuerySuggestionsConfigRequestRequestTypeDef,
     DescribeThesaurusRequestRequestTypeDef,
     DisassociatePersonasFromEntitiesRequestRequestTypeDef,
     DocumentAttributeValueTypeDef,
     RelevanceTypeDef,
     SearchTypeDef,
     DocumentsMetadataConfigurationTypeDef,
+    EmptyResponseMetadataTypeDef,
     EntityDisplayDataTypeDef,
     UserIdentityConfigurationTypeDef,
     FacetResultTypeDef,
     FacetTypeDef,
     FaqStatisticsTypeDef,
     FaqSummaryTypeDef,
-    GetQuerySuggestionsRequestRequestTypeDef,
+    FeaturedResultsSetSummaryTypeDef,
     GetSnapshotsRequestRequestTypeDef,
     TimeRangeTypeDef,
     GitHubDocumentCrawlPropertiesTypeDef,
     SaaSConfigurationTypeDef,
     MemberGroupTypeDef,
     MemberUserTypeDef,
     GroupSummaryTypeDef,
@@ -439,34 +456,37 @@
     ListAccessControlConfigurationsRequestRequestTypeDef,
     ListDataSourcesRequestRequestTypeDef,
     ListEntityPersonasRequestRequestTypeDef,
     PersonasSummaryTypeDef,
     ListExperienceEntitiesRequestRequestTypeDef,
     ListExperiencesRequestRequestTypeDef,
     ListFaqsRequestRequestTypeDef,
+    ListFeaturedResultsSetsRequestRequestTypeDef,
     ListGroupsOlderThanOrderingIdRequestRequestTypeDef,
     ListIndicesRequestRequestTypeDef,
     ListQuerySuggestionsBlockListsRequestRequestTypeDef,
     QuerySuggestionsBlockListSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListThesauriRequestRequestTypeDef,
     ThesaurusSummaryTypeDef,
     SortingConfigurationTypeDef,
     SpellCorrectionConfigurationTypeDef,
     ScoreAttributesTypeDef,
     WarningTypeDef,
     RelevanceFeedbackTypeDef,
+    ResponseMetadataTypeDef,
     SeedUrlConfigurationTypeDef,
     SiteMapsConfigurationTypeDef,
     StartDataSourceSyncJobRequestRequestTypeDef,
+    StartDataSourceSyncJobResponseTypeDef,
     StopDataSourceSyncJobRequestRequestTypeDef,
     SuggestionHighlightTypeDef,
     TableCellTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateQuerySuggestionsConfigRequestRequestTypeDef,
+    ListAccessControlConfigurationsResponseTypeDef,
     ColumnConfigurationTypeDef,
     GoogleDriveConfigurationTypeDef,
     SalesforceChatterFeedConfigurationTypeDef,
     SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
     SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
     SalesforceStandardObjectAttachmentConfigurationTypeDef,
     SalesforceStandardObjectConfigurationTypeDef,
@@ -475,71 +495,68 @@
     WorkDocsConfigurationTypeDef,
     BoxConfigurationTypeDef,
     FsxConfigurationTypeDef,
     JiraConfigurationTypeDef,
     QuipConfigurationTypeDef,
     SlackConfigurationTypeDef,
     AlfrescoConfigurationTypeDef,
+    DescribeFaqResponseTypeDef,
+    DescribeQuerySuggestionsBlockListResponseTypeDef,
+    DescribeThesaurusResponseTypeDef,
     OnPremiseConfigurationTypeDef,
     OneDriveUsersTypeDef,
     UpdateQuerySuggestionsBlockListRequestRequestTypeDef,
     UpdateThesaurusRequestRequestTypeDef,
     AssociateEntitiesToExperienceRequestRequestTypeDef,
     DisassociateEntitiesFromExperienceRequestRequestTypeDef,
     AssociateEntitiesToExperienceResponseTypeDef,
     AssociatePersonasToEntitiesResponseTypeDef,
-    CreateAccessControlConfigurationResponseTypeDef,
-    CreateDataSourceResponseTypeDef,
-    CreateExperienceResponseTypeDef,
-    CreateFaqResponseTypeDef,
-    CreateIndexResponseTypeDef,
-    CreateQuerySuggestionsBlockListResponseTypeDef,
-    CreateThesaurusResponseTypeDef,
-    DescribeFaqResponseTypeDef,
-    DescribeQuerySuggestionsBlockListResponseTypeDef,
-    DescribeQuerySuggestionsConfigResponseTypeDef,
-    DescribeThesaurusResponseTypeDef,
     DisassociateEntitiesFromExperienceResponseTypeDef,
     DisassociatePersonasFromEntitiesResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAccessControlConfigurationsResponseTypeDef,
-    StartDataSourceSyncJobResponseTypeDef,
     AssociatePersonasToEntitiesRequestRequestTypeDef,
+    AttributeSuggestionsDescribeConfigTypeDef,
+    AttributeSuggestionsUpdateConfigTypeDef,
     AuthenticationConfigurationTypeDef,
     BatchDeleteDocumentRequestRequestTypeDef,
     BatchDeleteDocumentResponseTypeDef,
+    BatchDeleteFeaturedResultsSetResponseTypeDef,
     BatchGetDocumentStatusResponseTypeDef,
     BatchPutDocumentResponseTypeDef,
     ConfluenceAttachmentConfigurationTypeDef,
     ConfluenceBlogConfigurationTypeDef,
     SharePointConfigurationTypeDef,
     ConfluencePageConfigurationTypeDef,
     ConfluenceSpaceConfigurationTypeDef,
     SpellCorrectedQueryTypeDef,
     HierarchicalPrincipalTypeDef,
     CreateFaqRequestRequestTypeDef,
     CreateQuerySuggestionsBlockListRequestRequestTypeDef,
     CreateThesaurusRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateFeaturedResultsSetRequestRequestTypeDef,
+    FeaturedResultsSetTypeDef,
+    UpdateFeaturedResultsSetRequestRequestTypeDef,
     UserContextTypeDef,
     ListDataSourcesResponseTypeDef,
     DataSourceSyncJobTypeDef,
     ExperiencesSummaryTypeDef,
+    DescribeFeaturedResultsSetResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DocumentAttributeConditionTypeDef,
     DocumentAttributeTargetTypeDef,
     DocumentAttributeTypeDef,
     DocumentAttributeValueCountPairTypeDef,
     DocumentRelevanceConfigurationTypeDef,
     DocumentMetadataConfigurationTypeDef,
     S3DataSourceConfigurationTypeDef,
     ExperienceEntitiesSummaryTypeDef,
     ExperienceConfigurationTypeDef,
     ListFaqsResponseTypeDef,
+    ListFeaturedResultsSetsResponseTypeDef,
     GetSnapshotsResponseTypeDef,
     ListDataSourceSyncJobsRequestRequestTypeDef,
     GroupMembersTypeDef,
     ListGroupsOlderThanOrderingIdResponseTypeDef,
     TextWithHighlightsTypeDef,
     ListIndicesResponseTypeDef,
     IndexStatisticsTypeDef,
@@ -552,45 +569,56 @@
     SuggestionTextWithHighlightsTypeDef,
     TableRowTypeDef,
     DatabaseConfigurationTypeDef,
     SalesforceKnowledgeArticleConfigurationTypeDef,
     ServiceNowConfigurationTypeDef,
     GitHubConfigurationTypeDef,
     OneDriveConfigurationTypeDef,
+    DescribeQuerySuggestionsConfigResponseTypeDef,
+    UpdateQuerySuggestionsConfigRequestRequestTypeDef,
     ConfluenceConfigurationTypeDef,
     CreateAccessControlConfigurationRequestRequestTypeDef,
     DescribeAccessControlConfigurationResponseTypeDef,
     UpdateAccessControlConfigurationRequestRequestTypeDef,
+    CreateFeaturedResultsSetResponseTypeDef,
+    UpdateFeaturedResultsSetResponseTypeDef,
+    AttributeSuggestionsGetConfigTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListExperiencesResponseTypeDef,
     HookConfigurationTypeDef,
     InlineCustomDocumentEnrichmentConfigurationTypeDef,
     AttributeFilterTypeDef,
     DocumentInfoTypeDef,
     DocumentTypeDef,
+    RetrieveResultItemTypeDef,
+    SourceDocumentTypeDef,
     QueryRequestRequestTypeDef,
+    RetrieveRequestRequestTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     CreateExperienceRequestRequestTypeDef,
     DescribeExperienceResponseTypeDef,
     UpdateExperienceRequestRequestTypeDef,
     PutPrincipalMappingRequestRequestTypeDef,
     AdditionalResultAttributeValueTypeDef,
     CreateIndexRequestRequestTypeDef,
     DescribeIndexResponseTypeDef,
     UpdateIndexRequestRequestTypeDef,
     WebCrawlerConfigurationTypeDef,
     SuggestionValueTypeDef,
     TableExcerptTypeDef,
     SalesforceConfigurationTypeDef,
+    GetQuerySuggestionsRequestRequestTypeDef,
     CustomDocumentEnrichmentConfigurationTypeDef,
     BatchGetDocumentStatusRequestRequestTypeDef,
+    RetrieveResultTypeDef,
     AdditionalResultAttributeTypeDef,
     SuggestionTypeDef,
     DataSourceConfigurationTypeDef,
     BatchPutDocumentRequestRequestTypeDef,
+    FeaturedResultsItemTypeDef,
     QueryResultItemTypeDef,
     GetQuerySuggestionsResponseTypeDef,
     CreateDataSourceRequestRequestTypeDef,
     DescribeDataSourceResponseTypeDef,
     UpdateDataSourceRequestRequestTypeDef,
     QueryResultTypeDef,
 )
@@ -603,42 +631,42 @@
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

### Comparing `mypy-boto3-kendra-1.26.48/README.md` & `mypy-boto3-kendra-1.27.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-kendra"></a>
 
 # mypy-boto3-kendra
 
 [![PyPI - mypy-boto3-kendra](https://img.shields.io/pypi/v/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kendra?color=blue)](https://pypistats.org/packages/mypy-boto3-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.kendra 1.26.48](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[boto3.kendra 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
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
 [mypy-boto3-kendra docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/).
 
 See how it helps to find and fix potential bugs:
 
@@ -245,14 +245,15 @@
 `mypy_boto3_kendra.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_kendra.literals import (
     AdditionalResultAttributeValueTypeType,
     AlfrescoEntityType,
+    AttributeSuggestionsModeType,
     ConditionOperatorType,
     ConfluenceAttachmentFieldNameType,
     ConfluenceAuthenticationTypeType,
     ConfluenceBlogFieldNameType,
     ConfluencePageFieldNameType,
     ConfluenceSpaceFieldNameType,
     ConfluenceVersionType,
@@ -265,14 +266,15 @@
     DocumentStatusType,
     EndpointTypeType,
     EntityTypeType,
     ErrorCodeType,
     ExperienceStatusType,
     FaqFileFormatType,
     FaqStatusType,
+    FeaturedResultsSetStatusType,
     FsxFileSystemTypeType,
     HighlightTypeType,
     IndexEditionType,
     IndexStatusType,
     IntervalType,
     IssueSubEntityType,
     KeyLocationType,
@@ -295,14 +297,15 @@
     ScoreConfidenceType,
     ServiceNowAuthenticationTypeType,
     ServiceNowBuildVersionTypeType,
     SharePointOnlineAuthenticationTypeType,
     SharePointVersionType,
     SlackEntityType,
     SortOrderType,
+    SuggestionTypeType,
     ThesaurusStatusType,
     TypeType,
     UserContextPolicyType,
     UserGroupResolutionModeType,
     WarningCodeType,
     WebCrawlerModeType,
     kendraServiceName,
@@ -329,19 +332,21 @@
     AccessControlListConfigurationTypeDef,
     AclConfigurationTypeDef,
     DataSourceToIndexFieldMappingTypeDef,
     DataSourceVpcConfigurationTypeDef,
     S3PathTypeDef,
     EntityConfigurationTypeDef,
     FailedEntityTypeDef,
-    ResponseMetadataTypeDef,
     EntityPersonaConfigurationTypeDef,
+    SuggestableConfigTypeDef,
     BasicAuthenticationConfigurationTypeDef,
     DataSourceSyncJobMetricTargetTypeDef,
     BatchDeleteDocumentResponseFailedDocumentTypeDef,
+    BatchDeleteFeaturedResultsSetErrorTypeDef,
+    BatchDeleteFeaturedResultsSetRequestRequestTypeDef,
     BatchGetDocumentStatusResponseErrorTypeDef,
     StatusTypeDef,
     BatchPutDocumentResponseFailedDocumentTypeDef,
     CapacityUnitsConfigurationTypeDef,
     ClearQuerySuggestionsRequestRequestTypeDef,
     ClickFeedbackTypeDef,
     ConfluenceAttachmentToIndexFieldMappingTypeDef,
@@ -349,17 +354,25 @@
     ProxyConfigurationTypeDef,
     ConfluencePageToIndexFieldMappingTypeDef,
     ConfluenceSpaceToIndexFieldMappingTypeDef,
     ConnectionConfigurationTypeDef,
     ContentSourceConfigurationTypeDef,
     CorrectionTypeDef,
     PrincipalTypeDef,
+    CreateAccessControlConfigurationResponseTypeDef,
     TagTypeDef,
+    CreateDataSourceResponseTypeDef,
+    CreateExperienceResponseTypeDef,
+    CreateFaqResponseTypeDef,
+    FeaturedDocumentTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     UserGroupResolutionConfigurationTypeDef,
+    CreateIndexResponseTypeDef,
+    CreateQuerySuggestionsBlockListResponseTypeDef,
+    CreateThesaurusResponseTypeDef,
     TemplateConfigurationTypeDef,
     DataSourceGroupTypeDef,
     DataSourceSummaryTypeDef,
     DataSourceSyncJobMetricsTypeDef,
     SqlConfigurationTypeDef,
     DeleteAccessControlConfigurationRequestRequestTypeDef,
     DeleteDataSourceRequestRequestTypeDef,
@@ -370,32 +383,36 @@
     DeleteQuerySuggestionsBlockListRequestRequestTypeDef,
     DeleteThesaurusRequestRequestTypeDef,
     DescribeAccessControlConfigurationRequestRequestTypeDef,
     DescribeDataSourceRequestRequestTypeDef,
     DescribeExperienceRequestRequestTypeDef,
     ExperienceEndpointTypeDef,
     DescribeFaqRequestRequestTypeDef,
+    DescribeFeaturedResultsSetRequestRequestTypeDef,
+    FeaturedDocumentMissingTypeDef,
+    FeaturedDocumentWithMetadataTypeDef,
     DescribeIndexRequestRequestTypeDef,
     DescribePrincipalMappingRequestRequestTypeDef,
     GroupOrderingIdSummaryTypeDef,
     DescribeQuerySuggestionsBlockListRequestRequestTypeDef,
     DescribeQuerySuggestionsConfigRequestRequestTypeDef,
     DescribeThesaurusRequestRequestTypeDef,
     DisassociatePersonasFromEntitiesRequestRequestTypeDef,
     DocumentAttributeValueTypeDef,
     RelevanceTypeDef,
     SearchTypeDef,
     DocumentsMetadataConfigurationTypeDef,
+    EmptyResponseMetadataTypeDef,
     EntityDisplayDataTypeDef,
     UserIdentityConfigurationTypeDef,
     FacetResultTypeDef,
     FacetTypeDef,
     FaqStatisticsTypeDef,
     FaqSummaryTypeDef,
-    GetQuerySuggestionsRequestRequestTypeDef,
+    FeaturedResultsSetSummaryTypeDef,
     GetSnapshotsRequestRequestTypeDef,
     TimeRangeTypeDef,
     GitHubDocumentCrawlPropertiesTypeDef,
     SaaSConfigurationTypeDef,
     MemberGroupTypeDef,
     MemberUserTypeDef,
     GroupSummaryTypeDef,
@@ -407,34 +424,37 @@
     ListAccessControlConfigurationsRequestRequestTypeDef,
     ListDataSourcesRequestRequestTypeDef,
     ListEntityPersonasRequestRequestTypeDef,
     PersonasSummaryTypeDef,
     ListExperienceEntitiesRequestRequestTypeDef,
     ListExperiencesRequestRequestTypeDef,
     ListFaqsRequestRequestTypeDef,
+    ListFeaturedResultsSetsRequestRequestTypeDef,
     ListGroupsOlderThanOrderingIdRequestRequestTypeDef,
     ListIndicesRequestRequestTypeDef,
     ListQuerySuggestionsBlockListsRequestRequestTypeDef,
     QuerySuggestionsBlockListSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListThesauriRequestRequestTypeDef,
     ThesaurusSummaryTypeDef,
     SortingConfigurationTypeDef,
     SpellCorrectionConfigurationTypeDef,
     ScoreAttributesTypeDef,
     WarningTypeDef,
     RelevanceFeedbackTypeDef,
+    ResponseMetadataTypeDef,
     SeedUrlConfigurationTypeDef,
     SiteMapsConfigurationTypeDef,
     StartDataSourceSyncJobRequestRequestTypeDef,
+    StartDataSourceSyncJobResponseTypeDef,
     StopDataSourceSyncJobRequestRequestTypeDef,
     SuggestionHighlightTypeDef,
     TableCellTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateQuerySuggestionsConfigRequestRequestTypeDef,
+    ListAccessControlConfigurationsResponseTypeDef,
     ColumnConfigurationTypeDef,
     GoogleDriveConfigurationTypeDef,
     SalesforceChatterFeedConfigurationTypeDef,
     SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
     SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
     SalesforceStandardObjectAttachmentConfigurationTypeDef,
     SalesforceStandardObjectConfigurationTypeDef,
@@ -443,71 +463,68 @@
     WorkDocsConfigurationTypeDef,
     BoxConfigurationTypeDef,
     FsxConfigurationTypeDef,
     JiraConfigurationTypeDef,
     QuipConfigurationTypeDef,
     SlackConfigurationTypeDef,
     AlfrescoConfigurationTypeDef,
+    DescribeFaqResponseTypeDef,
+    DescribeQuerySuggestionsBlockListResponseTypeDef,
+    DescribeThesaurusResponseTypeDef,
     OnPremiseConfigurationTypeDef,
     OneDriveUsersTypeDef,
     UpdateQuerySuggestionsBlockListRequestRequestTypeDef,
     UpdateThesaurusRequestRequestTypeDef,
     AssociateEntitiesToExperienceRequestRequestTypeDef,
     DisassociateEntitiesFromExperienceRequestRequestTypeDef,
     AssociateEntitiesToExperienceResponseTypeDef,
     AssociatePersonasToEntitiesResponseTypeDef,
-    CreateAccessControlConfigurationResponseTypeDef,
-    CreateDataSourceResponseTypeDef,
-    CreateExperienceResponseTypeDef,
-    CreateFaqResponseTypeDef,
-    CreateIndexResponseTypeDef,
-    CreateQuerySuggestionsBlockListResponseTypeDef,
-    CreateThesaurusResponseTypeDef,
-    DescribeFaqResponseTypeDef,
-    DescribeQuerySuggestionsBlockListResponseTypeDef,
-    DescribeQuerySuggestionsConfigResponseTypeDef,
-    DescribeThesaurusResponseTypeDef,
     DisassociateEntitiesFromExperienceResponseTypeDef,
     DisassociatePersonasFromEntitiesResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAccessControlConfigurationsResponseTypeDef,
-    StartDataSourceSyncJobResponseTypeDef,
     AssociatePersonasToEntitiesRequestRequestTypeDef,
+    AttributeSuggestionsDescribeConfigTypeDef,
+    AttributeSuggestionsUpdateConfigTypeDef,
     AuthenticationConfigurationTypeDef,
     BatchDeleteDocumentRequestRequestTypeDef,
     BatchDeleteDocumentResponseTypeDef,
+    BatchDeleteFeaturedResultsSetResponseTypeDef,
     BatchGetDocumentStatusResponseTypeDef,
     BatchPutDocumentResponseTypeDef,
     ConfluenceAttachmentConfigurationTypeDef,
     ConfluenceBlogConfigurationTypeDef,
     SharePointConfigurationTypeDef,
     ConfluencePageConfigurationTypeDef,
     ConfluenceSpaceConfigurationTypeDef,
     SpellCorrectedQueryTypeDef,
     HierarchicalPrincipalTypeDef,
     CreateFaqRequestRequestTypeDef,
     CreateQuerySuggestionsBlockListRequestRequestTypeDef,
     CreateThesaurusRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateFeaturedResultsSetRequestRequestTypeDef,
+    FeaturedResultsSetTypeDef,
+    UpdateFeaturedResultsSetRequestRequestTypeDef,
     UserContextTypeDef,
     ListDataSourcesResponseTypeDef,
     DataSourceSyncJobTypeDef,
     ExperiencesSummaryTypeDef,
+    DescribeFeaturedResultsSetResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DocumentAttributeConditionTypeDef,
     DocumentAttributeTargetTypeDef,
     DocumentAttributeTypeDef,
     DocumentAttributeValueCountPairTypeDef,
     DocumentRelevanceConfigurationTypeDef,
     DocumentMetadataConfigurationTypeDef,
     S3DataSourceConfigurationTypeDef,
     ExperienceEntitiesSummaryTypeDef,
     ExperienceConfigurationTypeDef,
     ListFaqsResponseTypeDef,
+    ListFeaturedResultsSetsResponseTypeDef,
     GetSnapshotsResponseTypeDef,
     ListDataSourceSyncJobsRequestRequestTypeDef,
     GroupMembersTypeDef,
     ListGroupsOlderThanOrderingIdResponseTypeDef,
     TextWithHighlightsTypeDef,
     ListIndicesResponseTypeDef,
     IndexStatisticsTypeDef,
@@ -520,45 +537,56 @@
     SuggestionTextWithHighlightsTypeDef,
     TableRowTypeDef,
     DatabaseConfigurationTypeDef,
     SalesforceKnowledgeArticleConfigurationTypeDef,
     ServiceNowConfigurationTypeDef,
     GitHubConfigurationTypeDef,
     OneDriveConfigurationTypeDef,
+    DescribeQuerySuggestionsConfigResponseTypeDef,
+    UpdateQuerySuggestionsConfigRequestRequestTypeDef,
     ConfluenceConfigurationTypeDef,
     CreateAccessControlConfigurationRequestRequestTypeDef,
     DescribeAccessControlConfigurationResponseTypeDef,
     UpdateAccessControlConfigurationRequestRequestTypeDef,
+    CreateFeaturedResultsSetResponseTypeDef,
+    UpdateFeaturedResultsSetResponseTypeDef,
+    AttributeSuggestionsGetConfigTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListExperiencesResponseTypeDef,
     HookConfigurationTypeDef,
     InlineCustomDocumentEnrichmentConfigurationTypeDef,
     AttributeFilterTypeDef,
     DocumentInfoTypeDef,
     DocumentTypeDef,
+    RetrieveResultItemTypeDef,
+    SourceDocumentTypeDef,
     QueryRequestRequestTypeDef,
+    RetrieveRequestRequestTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     CreateExperienceRequestRequestTypeDef,
     DescribeExperienceResponseTypeDef,
     UpdateExperienceRequestRequestTypeDef,
     PutPrincipalMappingRequestRequestTypeDef,
     AdditionalResultAttributeValueTypeDef,
     CreateIndexRequestRequestTypeDef,
     DescribeIndexResponseTypeDef,
     UpdateIndexRequestRequestTypeDef,
     WebCrawlerConfigurationTypeDef,
     SuggestionValueTypeDef,
     TableExcerptTypeDef,
     SalesforceConfigurationTypeDef,
+    GetQuerySuggestionsRequestRequestTypeDef,
     CustomDocumentEnrichmentConfigurationTypeDef,
     BatchGetDocumentStatusRequestRequestTypeDef,
+    RetrieveResultTypeDef,
     AdditionalResultAttributeTypeDef,
     SuggestionTypeDef,
     DataSourceConfigurationTypeDef,
     BatchPutDocumentRequestRequestTypeDef,
+    FeaturedResultsItemTypeDef,
     QueryResultItemTypeDef,
     GetQuerySuggestionsResponseTypeDef,
     CreateDataSourceRequestRequestTypeDef,
     DescribeDataSourceResponseTypeDef,
     UpdateDataSourceRequestRequestTypeDef,
     QueryResultTypeDef,
 )
@@ -571,42 +599,42 @@
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

### Comparing `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/__main__.py` & `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.kendra 1.26.48\nVersion:         1.26.48\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.kendra 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.48")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/client.py` & `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -17,45 +17,52 @@
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DataSourceSyncJobStatusType,
     DataSourceTypeType,
     FaqFileFormatType,
+    FeaturedResultsSetStatusType,
     IndexEditionType,
     IntervalType,
     MetricTypeType,
     ModeType,
     QueryResultTypeType,
+    SuggestionTypeType,
     UserContextPolicyType,
 )
 from .type_defs import (
     AssociateEntitiesToExperienceResponseTypeDef,
     AssociatePersonasToEntitiesResponseTypeDef,
     AttributeFilterTypeDef,
+    AttributeSuggestionsGetConfigTypeDef,
+    AttributeSuggestionsUpdateConfigTypeDef,
     BatchDeleteDocumentResponseTypeDef,
+    BatchDeleteFeaturedResultsSetResponseTypeDef,
     BatchGetDocumentStatusResponseTypeDef,
     BatchPutDocumentResponseTypeDef,
     CapacityUnitsConfigurationTypeDef,
     ClickFeedbackTypeDef,
     CreateAccessControlConfigurationResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateExperienceResponseTypeDef,
     CreateFaqResponseTypeDef,
+    CreateFeaturedResultsSetResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreateQuerySuggestionsBlockListResponseTypeDef,
     CreateThesaurusResponseTypeDef,
     CustomDocumentEnrichmentConfigurationTypeDef,
     DataSourceConfigurationTypeDef,
     DataSourceSyncJobMetricTargetTypeDef,
     DataSourceVpcConfigurationTypeDef,
     DescribeAccessControlConfigurationResponseTypeDef,
     DescribeDataSourceResponseTypeDef,
     DescribeExperienceResponseTypeDef,
     DescribeFaqResponseTypeDef,
+    DescribeFeaturedResultsSetResponseTypeDef,
     DescribeIndexResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DescribeQuerySuggestionsBlockListResponseTypeDef,
     DescribeQuerySuggestionsConfigResponseTypeDef,
     DescribeThesaurusResponseTypeDef,
     DisassociateEntitiesFromExperienceResponseTypeDef,
     DisassociatePersonasFromEntitiesResponseTypeDef,
@@ -64,71 +71,73 @@
     DocumentRelevanceConfigurationTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EntityConfigurationTypeDef,
     EntityPersonaConfigurationTypeDef,
     ExperienceConfigurationTypeDef,
     FacetTypeDef,
+    FeaturedDocumentTypeDef,
     GetQuerySuggestionsResponseTypeDef,
     GetSnapshotsResponseTypeDef,
     GroupMembersTypeDef,
     HierarchicalPrincipalTypeDef,
     ListAccessControlConfigurationsResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListEntityPersonasResponseTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     ListExperiencesResponseTypeDef,
     ListFaqsResponseTypeDef,
+    ListFeaturedResultsSetsResponseTypeDef,
     ListGroupsOlderThanOrderingIdResponseTypeDef,
     ListIndicesResponseTypeDef,
     ListQuerySuggestionsBlockListsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThesauriResponseTypeDef,
     PrincipalTypeDef,
     QueryResultTypeDef,
     RelevanceFeedbackTypeDef,
+    RetrieveResultTypeDef,
     S3PathTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     SortingConfigurationTypeDef,
     SpellCorrectionConfigurationTypeDef,
     StartDataSourceSyncJobResponseTypeDef,
     TagTypeDef,
     TimeRangeTypeDef,
+    UpdateFeaturedResultsSetResponseTypeDef,
     UserContextTypeDef,
     UserGroupResolutionConfigurationTypeDef,
     UserTokenConfigurationTypeDef,
 )
 
 __all__ = ("kendraClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
+    FeaturedResultsConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     ResourceAlreadyExistException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceUnavailableException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class kendraClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/)
     """
 
     meta: ClientMeta
@@ -137,102 +146,102 @@
     def exceptions(self) -> Exceptions:
         """
         kendraClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#exceptions)
         """
-
     def associate_entities_to_experience(
         self, *, Id: str, IndexId: str, EntityList: Sequence[EntityConfigurationTypeDef]
     ) -> AssociateEntitiesToExperienceResponseTypeDef:
         """
         Grants users or groups in your IAM Identity Center identity source access to
         your Amazon Kendra experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.associate_entities_to_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#associate_entities_to_experience)
         """
-
     def associate_personas_to_entities(
         self, *, Id: str, IndexId: str, Personas: Sequence[EntityPersonaConfigurationTypeDef]
     ) -> AssociatePersonasToEntitiesResponseTypeDef:
         """
         Defines the specific permissions of users or groups in your IAM Identity Center
         identity source with access to your Amazon Kendra experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.associate_personas_to_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#associate_personas_to_entities)
         """
-
     def batch_delete_document(
         self,
         *,
         IndexId: str,
         DocumentIdList: Sequence[str],
         DataSourceSyncJobMetricTarget: DataSourceSyncJobMetricTargetTypeDef = ...
     ) -> BatchDeleteDocumentResponseTypeDef:
         """
         Removes one or more documents from an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_delete_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#batch_delete_document)
         """
+    def batch_delete_featured_results_set(
+        self, *, IndexId: str, FeaturedResultsSetIds: Sequence[str]
+    ) -> BatchDeleteFeaturedResultsSetResponseTypeDef:
+        """
+        Removes one or more sets of featured results.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_delete_featured_results_set)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#batch_delete_featured_results_set)
+        """
     def batch_get_document_status(
         self, *, IndexId: str, DocumentInfoList: Sequence[DocumentInfoTypeDef]
     ) -> BatchGetDocumentStatusResponseTypeDef:
         """
         Returns the indexing status for one or more documents submitted with the
         [BatchPutDocument](https://docs.aws.amazon.com/kendra/latest/dg/API_BatchPutDocument.html)_
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_get_document_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#batch_get_document_status)
         """
-
     def batch_put_document(
         self,
         *,
         IndexId: str,
         Documents: Sequence[DocumentTypeDef],
         RoleArn: str = ...,
         CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
     ) -> BatchPutDocumentResponseTypeDef:
         """
         Adds one or more documents to an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_put_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#batch_put_document)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#can_paginate)
         """
-
     def clear_query_suggestions(self, *, IndexId: str) -> EmptyResponseMetadataTypeDef:
         """
         Clears existing query suggestions from an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.clear_query_suggestions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#clear_query_suggestions)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#close)
         """
-
     def create_access_control_configuration(
         self,
         *,
         IndexId: str,
         Name: str,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
@@ -241,15 +250,14 @@
     ) -> CreateAccessControlConfigurationResponseTypeDef:
         """
         Creates an access configuration for your documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_access_control_configuration)
         """
-
     def create_data_source(
         self,
         *,
         Name: str,
         IndexId: str,
         Type: DataSourceTypeType,
         Configuration: DataSourceConfigurationTypeDef = ...,
@@ -265,15 +273,14 @@
         """
         Creates a data source connector that you want to use with an Amazon Kendra
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_data_source)
         """
-
     def create_experience(
         self,
         *,
         Name: str,
         IndexId: str,
         RoleArn: str = ...,
         Configuration: ExperienceConfigurationTypeDef = ...,
@@ -282,35 +289,53 @@
     ) -> CreateExperienceResponseTypeDef:
         """
         Creates an Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_experience)
         """
-
     def create_faq(
         self,
         *,
         IndexId: str,
         Name: str,
         S3Path: S3PathTypeDef,
         RoleArn: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FileFormat: FaqFileFormatType = ...,
         ClientToken: str = ...,
         LanguageCode: str = ...
     ) -> CreateFaqResponseTypeDef:
         """
-        Creates an new set of frequently asked question (FAQ) questions and answers.
+        Creates a set of frequently ask questions (FAQs) using a specified FAQ file
+        stored in an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_faq)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_faq)
         """
+    def create_featured_results_set(
+        self,
+        *,
+        IndexId: str,
+        FeaturedResultsSetName: str,
+        Description: str = ...,
+        ClientToken: str = ...,
+        Status: FeaturedResultsSetStatusType = ...,
+        QueryTexts: Sequence[str] = ...,
+        FeaturedDocuments: Sequence[FeaturedDocumentTypeDef] = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> CreateFeaturedResultsSetResponseTypeDef:
+        """
+        Creates a set of featured results to display at the top of the search results
+        page.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_featured_results_set)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_featured_results_set)
+        """
     def create_index(
         self,
         *,
         Name: str,
         RoleArn: str,
         Edition: IndexEditionType = ...,
         ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
@@ -323,15 +348,14 @@
     ) -> CreateIndexResponseTypeDef:
         """
         Creates an Amazon Kendra index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_index)
         """
-
     def create_query_suggestions_block_list(
         self,
         *,
         IndexId: str,
         Name: str,
         SourceS3Path: S3PathTypeDef,
         RoleArn: str,
@@ -341,15 +365,14 @@
     ) -> CreateQuerySuggestionsBlockListResponseTypeDef:
         """
         Creates a block list to exlcude certain queries from suggestions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_query_suggestions_block_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_query_suggestions_block_list)
         """
-
     def create_thesaurus(
         self,
         *,
         IndexId: str,
         Name: str,
         RoleArn: str,
         SourceS3Path: S3PathTypeDef,
@@ -359,214 +382,207 @@
     ) -> CreateThesaurusResponseTypeDef:
         """
         Creates a thesaurus for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_thesaurus)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_thesaurus)
         """
-
     def delete_access_control_configuration(self, *, IndexId: str, Id: str) -> Dict[str, Any]:
         """
         Deletes an access control configuration that you created for your documents in
         an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_access_control_configuration)
         """
-
     def delete_data_source(self, *, Id: str, IndexId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an Amazon Kendra data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_data_source)
         """
-
     def delete_experience(self, *, Id: str, IndexId: str) -> Dict[str, Any]:
         """
         Deletes your Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_experience)
         """
-
     def delete_faq(self, *, Id: str, IndexId: str) -> EmptyResponseMetadataTypeDef:
         """
         Removes an FAQ from an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_faq)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_faq)
         """
-
     def delete_index(self, *, Id: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an existing Amazon Kendra index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_index)
         """
-
     def delete_principal_mapping(
         self, *, IndexId: str, GroupId: str, DataSourceId: str = ..., OrderingId: int = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a group so that all users and sub groups that belong to the group can no
         longer access documents only available to that group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_principal_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_principal_mapping)
         """
-
     def delete_query_suggestions_block_list(
         self, *, IndexId: str, Id: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a block list used for query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_query_suggestions_block_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_query_suggestions_block_list)
         """
-
     def delete_thesaurus(self, *, Id: str, IndexId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an existing Amazon Kendra thesaurus.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_thesaurus)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_thesaurus)
         """
-
     def describe_access_control_configuration(
         self, *, IndexId: str, Id: str
     ) -> DescribeAccessControlConfigurationResponseTypeDef:
         """
         Gets information about an access control configuration that you created for your
         documents in an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_access_control_configuration)
         """
-
     def describe_data_source(self, *, Id: str, IndexId: str) -> DescribeDataSourceResponseTypeDef:
         """
         Gets information about an Amazon Kendra data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_data_source)
         """
-
     def describe_experience(self, *, Id: str, IndexId: str) -> DescribeExperienceResponseTypeDef:
         """
         Gets information about your Amazon Kendra experience such as a search
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_experience)
         """
-
     def describe_faq(self, *, Id: str, IndexId: str) -> DescribeFaqResponseTypeDef:
         """
         Gets information about an FAQ list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_faq)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_faq)
         """
+    def describe_featured_results_set(
+        self, *, IndexId: str, FeaturedResultsSetId: str
+    ) -> DescribeFeaturedResultsSetResponseTypeDef:
+        """
+        Gets information about a set of featured results.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_featured_results_set)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_featured_results_set)
+        """
     def describe_index(self, *, Id: str) -> DescribeIndexResponseTypeDef:
         """
         Gets information about an existing Amazon Kendra index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_index)
         """
-
     def describe_principal_mapping(
         self, *, IndexId: str, GroupId: str, DataSourceId: str = ...
     ) -> DescribePrincipalMappingResponseTypeDef:
         """
         Describes the processing of `PUT` and `DELETE` actions for mapping users to
         their groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_principal_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_principal_mapping)
         """
-
     def describe_query_suggestions_block_list(
         self, *, IndexId: str, Id: str
     ) -> DescribeQuerySuggestionsBlockListResponseTypeDef:
         """
         Gets information about a block list used for query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_query_suggestions_block_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_query_suggestions_block_list)
         """
-
     def describe_query_suggestions_config(
         self, *, IndexId: str
     ) -> DescribeQuerySuggestionsConfigResponseTypeDef:
         """
         Gets information on the settings of query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_query_suggestions_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_query_suggestions_config)
         """
-
     def describe_thesaurus(self, *, Id: str, IndexId: str) -> DescribeThesaurusResponseTypeDef:
         """
         Gets information about an existing Amazon Kendra thesaurus.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_thesaurus)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_thesaurus)
         """
-
     def disassociate_entities_from_experience(
         self, *, Id: str, IndexId: str, EntityList: Sequence[EntityConfigurationTypeDef]
     ) -> DisassociateEntitiesFromExperienceResponseTypeDef:
         """
         Prevents users or groups in your IAM Identity Center identity source from
         accessing your Amazon Kendra experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.disassociate_entities_from_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#disassociate_entities_from_experience)
         """
-
     def disassociate_personas_from_entities(
         self, *, Id: str, IndexId: str, EntityIds: Sequence[str]
     ) -> DisassociatePersonasFromEntitiesResponseTypeDef:
         """
         Removes the specific permissions of users or groups in your IAM Identity Center
         identity source with access to your Amazon Kendra experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.disassociate_personas_from_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#disassociate_personas_from_entities)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#generate_presigned_url)
         """
-
     def get_query_suggestions(
-        self, *, IndexId: str, QueryText: str, MaxSuggestionsCount: int = ...
+        self,
+        *,
+        IndexId: str,
+        QueryText: str,
+        MaxSuggestionsCount: int = ...,
+        SuggestionTypes: Sequence[SuggestionTypeType] = ...,
+        AttributeSuggestionsConfig: AttributeSuggestionsGetConfigTypeDef = ...
     ) -> GetQuerySuggestionsResponseTypeDef:
         """
         Fetches the queries that are suggested to your users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.get_query_suggestions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#get_query_suggestions)
         """
-
     def get_snapshots(
         self,
         *,
         IndexId: str,
         Interval: IntervalType,
         MetricType: MetricTypeType,
         NextToken: str = ...,
@@ -574,25 +590,23 @@
     ) -> GetSnapshotsResponseTypeDef:
         """
         Retrieves search metrics data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.get_snapshots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#get_snapshots)
         """
-
     def list_access_control_configurations(
         self, *, IndexId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListAccessControlConfigurationsResponseTypeDef:
         """
         Lists one or more access control configurations for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_access_control_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_access_control_configurations)
         """
-
     def list_data_source_sync_jobs(
         self,
         *,
         Id: str,
         IndexId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
@@ -601,67 +615,70 @@
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
         Gets statistics about synchronizing a data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_data_source_sync_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_data_source_sync_jobs)
         """
-
     def list_data_sources(
         self, *, IndexId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDataSourcesResponseTypeDef:
         """
         Lists the data source connectors that you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_data_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_data_sources)
         """
-
     def list_entity_personas(
         self, *, Id: str, IndexId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListEntityPersonasResponseTypeDef:
         """
         Lists specific permissions of users and groups with access to your Amazon Kendra
         experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_entity_personas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_entity_personas)
         """
-
     def list_experience_entities(
         self, *, Id: str, IndexId: str, NextToken: str = ...
     ) -> ListExperienceEntitiesResponseTypeDef:
         """
         Lists users or groups in your IAM Identity Center identity source that are
         granted access to your Amazon Kendra experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_experience_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_experience_entities)
         """
-
     def list_experiences(
         self, *, IndexId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListExperiencesResponseTypeDef:
         """
         Lists one or more Amazon Kendra experiences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_experiences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_experiences)
         """
-
     def list_faqs(
         self, *, IndexId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListFaqsResponseTypeDef:
         """
         Gets a list of FAQ lists associated with an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_faqs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_faqs)
         """
+    def list_featured_results_sets(
+        self, *, IndexId: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListFeaturedResultsSetsResponseTypeDef:
+        """
+        Lists all your sets of featured results for a given index.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_featured_results_sets)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_featured_results_sets)
+        """
     def list_groups_older_than_ordering_id(
         self,
         *,
         IndexId: str,
         OrderingId: int,
         DataSourceId: str = ...,
         NextToken: str = ...,
@@ -670,53 +687,48 @@
         """
         Provides a list of groups that are mapped to users before a given ordering or
         timestamp identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_groups_older_than_ordering_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_groups_older_than_ordering_id)
         """
-
     def list_indices(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListIndicesResponseTypeDef:
         """
         Lists the Amazon Kendra indexes that you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_indices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_indices)
         """
-
     def list_query_suggestions_block_lists(
         self, *, IndexId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListQuerySuggestionsBlockListsResponseTypeDef:
         """
         Lists the block lists used for query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_query_suggestions_block_lists)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_query_suggestions_block_lists)
         """
-
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
         Gets a list of tags associated with a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_tags_for_resource)
         """
-
     def list_thesauri(
         self, *, IndexId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListThesauriResponseTypeDef:
         """
         Lists the thesauri for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_thesauri)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_thesauri)
         """
-
     def put_principal_mapping(
         self,
         *,
         IndexId: str,
         GroupId: str,
         GroupMembers: GroupMembersTypeDef,
         DataSourceId: str = ...,
@@ -726,15 +738,14 @@
         """
         Maps users to their groups so that you only need to provide the user ID when you
         issue the query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.put_principal_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#put_principal_mapping)
         """
-
     def query(
         self,
         *,
         IndexId: str,
         QueryText: str = ...,
         AttributeFilter: "AttributeFilterTypeDef" = ...,
         Facets: Sequence["FacetTypeDef"] = ...,
@@ -747,38 +758,55 @@
         PageSize: int = ...,
         SortingConfiguration: SortingConfigurationTypeDef = ...,
         UserContext: UserContextTypeDef = ...,
         VisitorId: str = ...,
         SpellCorrectionConfiguration: SpellCorrectionConfigurationTypeDef = ...
     ) -> QueryResultTypeDef:
         """
-        Searches an active index.
+        Searches an index given an input query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#query)
         """
+    def retrieve(
+        self,
+        *,
+        IndexId: str,
+        QueryText: str,
+        AttributeFilter: "AttributeFilterTypeDef" = ...,
+        RequestedDocumentAttributes: Sequence[str] = ...,
+        DocumentRelevanceOverrideConfigurations: Sequence[
+            DocumentRelevanceConfigurationTypeDef
+        ] = ...,
+        PageNumber: int = ...,
+        PageSize: int = ...,
+        UserContext: UserContextTypeDef = ...
+    ) -> RetrieveResultTypeDef:
+        """
+        Retrieves relevant passages or text excerpts given an input query.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.retrieve)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#retrieve)
+        """
     def start_data_source_sync_job(
         self, *, Id: str, IndexId: str
     ) -> StartDataSourceSyncJobResponseTypeDef:
         """
         Starts a synchronization job for a data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.start_data_source_sync_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#start_data_source_sync_job)
         """
-
     def stop_data_source_sync_job(self, *, Id: str, IndexId: str) -> EmptyResponseMetadataTypeDef:
         """
         Stops a synchronization job that is currently running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.stop_data_source_sync_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#stop_data_source_sync_job)
         """
-
     def submit_feedback(
         self,
         *,
         IndexId: str,
         QueryId: str,
         ClickFeedbackItems: Sequence[ClickFeedbackTypeDef] = ...,
         RelevanceFeedbackItems: Sequence[RelevanceFeedbackTypeDef] = ...
@@ -786,31 +814,28 @@
         """
         Enables you to provide feedback to Amazon Kendra to improve the performance of
         your index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.submit_feedback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#submit_feedback)
         """
-
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds the specified tag to the specified index, FAQ, or data source resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#tag_resource)
         """
-
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag from an index, FAQ, or a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#untag_resource)
         """
-
     def update_access_control_configuration(
         self,
         *,
         IndexId: str,
         Id: str,
         Name: str = ...,
         Description: str = ...,
@@ -819,15 +844,14 @@
     ) -> Dict[str, Any]:
         """
         Updates an access control configuration for your documents in an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_access_control_configuration)
         """
-
     def update_data_source(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         Configuration: DataSourceConfigurationTypeDef = ...,
@@ -840,15 +864,14 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_data_source)
         """
-
     def update_experience(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         RoleArn: str = ...,
@@ -857,15 +880,31 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates your Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_experience)
         """
+    def update_featured_results_set(
+        self,
+        *,
+        IndexId: str,
+        FeaturedResultsSetId: str,
+        FeaturedResultsSetName: str = ...,
+        Description: str = ...,
+        Status: FeaturedResultsSetStatusType = ...,
+        QueryTexts: Sequence[str] = ...,
+        FeaturedDocuments: Sequence[FeaturedDocumentTypeDef] = ...
+    ) -> UpdateFeaturedResultsSetResponseTypeDef:
+        """
+        Updates a set of featured results.
 
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_featured_results_set)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_featured_results_set)
+        """
     def update_index(
         self,
         *,
         Id: str,
         Name: str = ...,
         RoleArn: str = ...,
         Description: str = ...,
@@ -877,15 +916,14 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_index)
         """
-
     def update_query_suggestions_block_list(
         self,
         *,
         IndexId: str,
         Id: str,
         Name: str = ...,
         Description: str = ...,
@@ -894,32 +932,31 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a block list used for query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_query_suggestions_block_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_query_suggestions_block_list)
         """
-
     def update_query_suggestions_config(
         self,
         *,
         IndexId: str,
         Mode: ModeType = ...,
         QueryLogLookBackWindowInDays: int = ...,
         IncludeQueriesWithoutUserInformation: bool = ...,
         MinimumNumberOfQueryingUsers: int = ...,
-        MinimumQueryCount: int = ...
+        MinimumQueryCount: int = ...,
+        AttributeSuggestionsConfig: AttributeSuggestionsUpdateConfigTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the settings of query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_query_suggestions_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_query_suggestions_config)
         """
-
     def update_thesaurus(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         Description: str = ...,
```

### Comparing `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/client.pyi` & `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,45 +17,52 @@
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DataSourceSyncJobStatusType,
     DataSourceTypeType,
     FaqFileFormatType,
+    FeaturedResultsSetStatusType,
     IndexEditionType,
     IntervalType,
     MetricTypeType,
     ModeType,
     QueryResultTypeType,
+    SuggestionTypeType,
     UserContextPolicyType,
 )
 from .type_defs import (
     AssociateEntitiesToExperienceResponseTypeDef,
     AssociatePersonasToEntitiesResponseTypeDef,
     AttributeFilterTypeDef,
+    AttributeSuggestionsGetConfigTypeDef,
+    AttributeSuggestionsUpdateConfigTypeDef,
     BatchDeleteDocumentResponseTypeDef,
+    BatchDeleteFeaturedResultsSetResponseTypeDef,
     BatchGetDocumentStatusResponseTypeDef,
     BatchPutDocumentResponseTypeDef,
     CapacityUnitsConfigurationTypeDef,
     ClickFeedbackTypeDef,
     CreateAccessControlConfigurationResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateExperienceResponseTypeDef,
     CreateFaqResponseTypeDef,
+    CreateFeaturedResultsSetResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreateQuerySuggestionsBlockListResponseTypeDef,
     CreateThesaurusResponseTypeDef,
     CustomDocumentEnrichmentConfigurationTypeDef,
     DataSourceConfigurationTypeDef,
     DataSourceSyncJobMetricTargetTypeDef,
     DataSourceVpcConfigurationTypeDef,
     DescribeAccessControlConfigurationResponseTypeDef,
     DescribeDataSourceResponseTypeDef,
     DescribeExperienceResponseTypeDef,
     DescribeFaqResponseTypeDef,
+    DescribeFeaturedResultsSetResponseTypeDef,
     DescribeIndexResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DescribeQuerySuggestionsBlockListResponseTypeDef,
     DescribeQuerySuggestionsConfigResponseTypeDef,
     DescribeThesaurusResponseTypeDef,
     DisassociateEntitiesFromExperienceResponseTypeDef,
     DisassociatePersonasFromEntitiesResponseTypeDef,
@@ -64,68 +71,76 @@
     DocumentRelevanceConfigurationTypeDef,
     DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EntityConfigurationTypeDef,
     EntityPersonaConfigurationTypeDef,
     ExperienceConfigurationTypeDef,
     FacetTypeDef,
+    FeaturedDocumentTypeDef,
     GetQuerySuggestionsResponseTypeDef,
     GetSnapshotsResponseTypeDef,
     GroupMembersTypeDef,
     HierarchicalPrincipalTypeDef,
     ListAccessControlConfigurationsResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListEntityPersonasResponseTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     ListExperiencesResponseTypeDef,
     ListFaqsResponseTypeDef,
+    ListFeaturedResultsSetsResponseTypeDef,
     ListGroupsOlderThanOrderingIdResponseTypeDef,
     ListIndicesResponseTypeDef,
     ListQuerySuggestionsBlockListsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThesauriResponseTypeDef,
     PrincipalTypeDef,
     QueryResultTypeDef,
     RelevanceFeedbackTypeDef,
+    RetrieveResultTypeDef,
     S3PathTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     SortingConfigurationTypeDef,
     SpellCorrectionConfigurationTypeDef,
     StartDataSourceSyncJobResponseTypeDef,
     TagTypeDef,
     TimeRangeTypeDef,
+    UpdateFeaturedResultsSetResponseTypeDef,
     UserContextTypeDef,
     UserGroupResolutionConfigurationTypeDef,
     UserTokenConfigurationTypeDef,
 )
 
 __all__ = ("kendraClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
+    FeaturedResultsConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     ResourceAlreadyExistException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceUnavailableException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class kendraClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/)
     """
 
     meta: ClientMeta
@@ -134,93 +149,112 @@
     def exceptions(self) -> Exceptions:
         """
         kendraClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#exceptions)
         """
+
     def associate_entities_to_experience(
         self, *, Id: str, IndexId: str, EntityList: Sequence[EntityConfigurationTypeDef]
     ) -> AssociateEntitiesToExperienceResponseTypeDef:
         """
         Grants users or groups in your IAM Identity Center identity source access to
         your Amazon Kendra experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.associate_entities_to_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#associate_entities_to_experience)
         """
+
     def associate_personas_to_entities(
         self, *, Id: str, IndexId: str, Personas: Sequence[EntityPersonaConfigurationTypeDef]
     ) -> AssociatePersonasToEntitiesResponseTypeDef:
         """
         Defines the specific permissions of users or groups in your IAM Identity Center
         identity source with access to your Amazon Kendra experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.associate_personas_to_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#associate_personas_to_entities)
         """
+
     def batch_delete_document(
         self,
         *,
         IndexId: str,
         DocumentIdList: Sequence[str],
         DataSourceSyncJobMetricTarget: DataSourceSyncJobMetricTargetTypeDef = ...
     ) -> BatchDeleteDocumentResponseTypeDef:
         """
         Removes one or more documents from an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_delete_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#batch_delete_document)
         """
+
+    def batch_delete_featured_results_set(
+        self, *, IndexId: str, FeaturedResultsSetIds: Sequence[str]
+    ) -> BatchDeleteFeaturedResultsSetResponseTypeDef:
+        """
+        Removes one or more sets of featured results.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_delete_featured_results_set)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#batch_delete_featured_results_set)
+        """
+
     def batch_get_document_status(
         self, *, IndexId: str, DocumentInfoList: Sequence[DocumentInfoTypeDef]
     ) -> BatchGetDocumentStatusResponseTypeDef:
         """
         Returns the indexing status for one or more documents submitted with the
         [BatchPutDocument](https://docs.aws.amazon.com/kendra/latest/dg/API_BatchPutDocument.html)_
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_get_document_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#batch_get_document_status)
         """
+
     def batch_put_document(
         self,
         *,
         IndexId: str,
         Documents: Sequence[DocumentTypeDef],
         RoleArn: str = ...,
         CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationTypeDef = ...
     ) -> BatchPutDocumentResponseTypeDef:
         """
         Adds one or more documents to an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.batch_put_document)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#batch_put_document)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#can_paginate)
         """
+
     def clear_query_suggestions(self, *, IndexId: str) -> EmptyResponseMetadataTypeDef:
         """
         Clears existing query suggestions from an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.clear_query_suggestions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#clear_query_suggestions)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#close)
         """
+
     def create_access_control_configuration(
         self,
         *,
         IndexId: str,
         Name: str,
         Description: str = ...,
         AccessControlList: Sequence[PrincipalTypeDef] = ...,
@@ -229,14 +263,15 @@
     ) -> CreateAccessControlConfigurationResponseTypeDef:
         """
         Creates an access configuration for your documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_access_control_configuration)
         """
+
     def create_data_source(
         self,
         *,
         Name: str,
         IndexId: str,
         Type: DataSourceTypeType,
         Configuration: DataSourceConfigurationTypeDef = ...,
@@ -252,14 +287,15 @@
         """
         Creates a data source connector that you want to use with an Amazon Kendra
         index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_data_source)
         """
+
     def create_experience(
         self,
         *,
         Name: str,
         IndexId: str,
         RoleArn: str = ...,
         Configuration: ExperienceConfigurationTypeDef = ...,
@@ -268,33 +304,56 @@
     ) -> CreateExperienceResponseTypeDef:
         """
         Creates an Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_experience)
         """
+
     def create_faq(
         self,
         *,
         IndexId: str,
         Name: str,
         S3Path: S3PathTypeDef,
         RoleArn: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FileFormat: FaqFileFormatType = ...,
         ClientToken: str = ...,
         LanguageCode: str = ...
     ) -> CreateFaqResponseTypeDef:
         """
-        Creates an new set of frequently asked question (FAQ) questions and answers.
+        Creates a set of frequently ask questions (FAQs) using a specified FAQ file
+        stored in an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_faq)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_faq)
         """
+
+    def create_featured_results_set(
+        self,
+        *,
+        IndexId: str,
+        FeaturedResultsSetName: str,
+        Description: str = ...,
+        ClientToken: str = ...,
+        Status: FeaturedResultsSetStatusType = ...,
+        QueryTexts: Sequence[str] = ...,
+        FeaturedDocuments: Sequence[FeaturedDocumentTypeDef] = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> CreateFeaturedResultsSetResponseTypeDef:
+        """
+        Creates a set of featured results to display at the top of the search results
+        page.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_featured_results_set)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_featured_results_set)
+        """
+
     def create_index(
         self,
         *,
         Name: str,
         RoleArn: str,
         Edition: IndexEditionType = ...,
         ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
@@ -307,14 +366,15 @@
     ) -> CreateIndexResponseTypeDef:
         """
         Creates an Amazon Kendra index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_index)
         """
+
     def create_query_suggestions_block_list(
         self,
         *,
         IndexId: str,
         Name: str,
         SourceS3Path: S3PathTypeDef,
         RoleArn: str,
@@ -324,14 +384,15 @@
     ) -> CreateQuerySuggestionsBlockListResponseTypeDef:
         """
         Creates a block list to exlcude certain queries from suggestions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_query_suggestions_block_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_query_suggestions_block_list)
         """
+
     def create_thesaurus(
         self,
         *,
         IndexId: str,
         Name: str,
         RoleArn: str,
         SourceS3Path: S3PathTypeDef,
@@ -341,192 +402,230 @@
     ) -> CreateThesaurusResponseTypeDef:
         """
         Creates a thesaurus for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.create_thesaurus)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#create_thesaurus)
         """
+
     def delete_access_control_configuration(self, *, IndexId: str, Id: str) -> Dict[str, Any]:
         """
         Deletes an access control configuration that you created for your documents in
         an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_access_control_configuration)
         """
+
     def delete_data_source(self, *, Id: str, IndexId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an Amazon Kendra data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_data_source)
         """
+
     def delete_experience(self, *, Id: str, IndexId: str) -> Dict[str, Any]:
         """
         Deletes your Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_experience)
         """
+
     def delete_faq(self, *, Id: str, IndexId: str) -> EmptyResponseMetadataTypeDef:
         """
         Removes an FAQ from an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_faq)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_faq)
         """
+
     def delete_index(self, *, Id: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an existing Amazon Kendra index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_index)
         """
+
     def delete_principal_mapping(
         self, *, IndexId: str, GroupId: str, DataSourceId: str = ..., OrderingId: int = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a group so that all users and sub groups that belong to the group can no
         longer access documents only available to that group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_principal_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_principal_mapping)
         """
+
     def delete_query_suggestions_block_list(
         self, *, IndexId: str, Id: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a block list used for query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_query_suggestions_block_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_query_suggestions_block_list)
         """
+
     def delete_thesaurus(self, *, Id: str, IndexId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an existing Amazon Kendra thesaurus.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.delete_thesaurus)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#delete_thesaurus)
         """
+
     def describe_access_control_configuration(
         self, *, IndexId: str, Id: str
     ) -> DescribeAccessControlConfigurationResponseTypeDef:
         """
         Gets information about an access control configuration that you created for your
         documents in an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_access_control_configuration)
         """
+
     def describe_data_source(self, *, Id: str, IndexId: str) -> DescribeDataSourceResponseTypeDef:
         """
         Gets information about an Amazon Kendra data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_data_source)
         """
+
     def describe_experience(self, *, Id: str, IndexId: str) -> DescribeExperienceResponseTypeDef:
         """
         Gets information about your Amazon Kendra experience such as a search
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_experience)
         """
+
     def describe_faq(self, *, Id: str, IndexId: str) -> DescribeFaqResponseTypeDef:
         """
         Gets information about an FAQ list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_faq)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_faq)
         """
+
+    def describe_featured_results_set(
+        self, *, IndexId: str, FeaturedResultsSetId: str
+    ) -> DescribeFeaturedResultsSetResponseTypeDef:
+        """
+        Gets information about a set of featured results.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_featured_results_set)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_featured_results_set)
+        """
+
     def describe_index(self, *, Id: str) -> DescribeIndexResponseTypeDef:
         """
         Gets information about an existing Amazon Kendra index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_index)
         """
+
     def describe_principal_mapping(
         self, *, IndexId: str, GroupId: str, DataSourceId: str = ...
     ) -> DescribePrincipalMappingResponseTypeDef:
         """
         Describes the processing of `PUT` and `DELETE` actions for mapping users to
         their groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_principal_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_principal_mapping)
         """
+
     def describe_query_suggestions_block_list(
         self, *, IndexId: str, Id: str
     ) -> DescribeQuerySuggestionsBlockListResponseTypeDef:
         """
         Gets information about a block list used for query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_query_suggestions_block_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_query_suggestions_block_list)
         """
+
     def describe_query_suggestions_config(
         self, *, IndexId: str
     ) -> DescribeQuerySuggestionsConfigResponseTypeDef:
         """
         Gets information on the settings of query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_query_suggestions_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_query_suggestions_config)
         """
+
     def describe_thesaurus(self, *, Id: str, IndexId: str) -> DescribeThesaurusResponseTypeDef:
         """
         Gets information about an existing Amazon Kendra thesaurus.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.describe_thesaurus)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#describe_thesaurus)
         """
+
     def disassociate_entities_from_experience(
         self, *, Id: str, IndexId: str, EntityList: Sequence[EntityConfigurationTypeDef]
     ) -> DisassociateEntitiesFromExperienceResponseTypeDef:
         """
         Prevents users or groups in your IAM Identity Center identity source from
         accessing your Amazon Kendra experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.disassociate_entities_from_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#disassociate_entities_from_experience)
         """
+
     def disassociate_personas_from_entities(
         self, *, Id: str, IndexId: str, EntityIds: Sequence[str]
     ) -> DisassociatePersonasFromEntitiesResponseTypeDef:
         """
         Removes the specific permissions of users or groups in your IAM Identity Center
         identity source with access to your Amazon Kendra experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.disassociate_personas_from_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#disassociate_personas_from_entities)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#generate_presigned_url)
         """
+
     def get_query_suggestions(
-        self, *, IndexId: str, QueryText: str, MaxSuggestionsCount: int = ...
+        self,
+        *,
+        IndexId: str,
+        QueryText: str,
+        MaxSuggestionsCount: int = ...,
+        SuggestionTypes: Sequence[SuggestionTypeType] = ...,
+        AttributeSuggestionsConfig: AttributeSuggestionsGetConfigTypeDef = ...
     ) -> GetQuerySuggestionsResponseTypeDef:
         """
         Fetches the queries that are suggested to your users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.get_query_suggestions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#get_query_suggestions)
         """
+
     def get_snapshots(
         self,
         *,
         IndexId: str,
         Interval: IntervalType,
         MetricType: MetricTypeType,
         NextToken: str = ...,
@@ -534,23 +633,25 @@
     ) -> GetSnapshotsResponseTypeDef:
         """
         Retrieves search metrics data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.get_snapshots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#get_snapshots)
         """
+
     def list_access_control_configurations(
         self, *, IndexId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListAccessControlConfigurationsResponseTypeDef:
         """
         Lists one or more access control configurations for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_access_control_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_access_control_configurations)
         """
+
     def list_data_source_sync_jobs(
         self,
         *,
         Id: str,
         IndexId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
@@ -559,61 +660,77 @@
     ) -> ListDataSourceSyncJobsResponseTypeDef:
         """
         Gets statistics about synchronizing a data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_data_source_sync_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_data_source_sync_jobs)
         """
+
     def list_data_sources(
         self, *, IndexId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListDataSourcesResponseTypeDef:
         """
         Lists the data source connectors that you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_data_sources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_data_sources)
         """
+
     def list_entity_personas(
         self, *, Id: str, IndexId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListEntityPersonasResponseTypeDef:
         """
         Lists specific permissions of users and groups with access to your Amazon Kendra
         experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_entity_personas)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_entity_personas)
         """
+
     def list_experience_entities(
         self, *, Id: str, IndexId: str, NextToken: str = ...
     ) -> ListExperienceEntitiesResponseTypeDef:
         """
         Lists users or groups in your IAM Identity Center identity source that are
         granted access to your Amazon Kendra experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_experience_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_experience_entities)
         """
+
     def list_experiences(
         self, *, IndexId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListExperiencesResponseTypeDef:
         """
         Lists one or more Amazon Kendra experiences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_experiences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_experiences)
         """
+
     def list_faqs(
         self, *, IndexId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListFaqsResponseTypeDef:
         """
         Gets a list of FAQ lists associated with an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_faqs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_faqs)
         """
+
+    def list_featured_results_sets(
+        self, *, IndexId: str, NextToken: str = ..., MaxResults: int = ...
+    ) -> ListFeaturedResultsSetsResponseTypeDef:
+        """
+        Lists all your sets of featured results for a given index.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_featured_results_sets)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_featured_results_sets)
+        """
+
     def list_groups_older_than_ordering_id(
         self,
         *,
         IndexId: str,
         OrderingId: int,
         DataSourceId: str = ...,
         NextToken: str = ...,
@@ -622,48 +739,53 @@
         """
         Provides a list of groups that are mapped to users before a given ordering or
         timestamp identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_groups_older_than_ordering_id)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_groups_older_than_ordering_id)
         """
+
     def list_indices(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListIndicesResponseTypeDef:
         """
         Lists the Amazon Kendra indexes that you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_indices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_indices)
         """
+
     def list_query_suggestions_block_lists(
         self, *, IndexId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListQuerySuggestionsBlockListsResponseTypeDef:
         """
         Lists the block lists used for query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_query_suggestions_block_lists)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_query_suggestions_block_lists)
         """
+
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
         Gets a list of tags associated with a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_tags_for_resource)
         """
+
     def list_thesauri(
         self, *, IndexId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListThesauriResponseTypeDef:
         """
         Lists the thesauri for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.list_thesauri)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#list_thesauri)
         """
+
     def put_principal_mapping(
         self,
         *,
         IndexId: str,
         GroupId: str,
         GroupMembers: GroupMembersTypeDef,
         DataSourceId: str = ...,
@@ -673,14 +795,15 @@
         """
         Maps users to their groups so that you only need to provide the user ID when you
         issue the query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.put_principal_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#put_principal_mapping)
         """
+
     def query(
         self,
         *,
         IndexId: str,
         QueryText: str = ...,
         AttributeFilter: "AttributeFilterTypeDef" = ...,
         Facets: Sequence["FacetTypeDef"] = ...,
@@ -693,35 +816,59 @@
         PageSize: int = ...,
         SortingConfiguration: SortingConfigurationTypeDef = ...,
         UserContext: UserContextTypeDef = ...,
         VisitorId: str = ...,
         SpellCorrectionConfiguration: SpellCorrectionConfigurationTypeDef = ...
     ) -> QueryResultTypeDef:
         """
-        Searches an active index.
+        Searches an index given an input query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#query)
         """
+
+    def retrieve(
+        self,
+        *,
+        IndexId: str,
+        QueryText: str,
+        AttributeFilter: "AttributeFilterTypeDef" = ...,
+        RequestedDocumentAttributes: Sequence[str] = ...,
+        DocumentRelevanceOverrideConfigurations: Sequence[
+            DocumentRelevanceConfigurationTypeDef
+        ] = ...,
+        PageNumber: int = ...,
+        PageSize: int = ...,
+        UserContext: UserContextTypeDef = ...
+    ) -> RetrieveResultTypeDef:
+        """
+        Retrieves relevant passages or text excerpts given an input query.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.retrieve)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#retrieve)
+        """
+
     def start_data_source_sync_job(
         self, *, Id: str, IndexId: str
     ) -> StartDataSourceSyncJobResponseTypeDef:
         """
         Starts a synchronization job for a data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.start_data_source_sync_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#start_data_source_sync_job)
         """
+
     def stop_data_source_sync_job(self, *, Id: str, IndexId: str) -> EmptyResponseMetadataTypeDef:
         """
         Stops a synchronization job that is currently running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.stop_data_source_sync_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#stop_data_source_sync_job)
         """
+
     def submit_feedback(
         self,
         *,
         IndexId: str,
         QueryId: str,
         ClickFeedbackItems: Sequence[ClickFeedbackTypeDef] = ...,
         RelevanceFeedbackItems: Sequence[RelevanceFeedbackTypeDef] = ...
@@ -729,28 +876,31 @@
         """
         Enables you to provide feedback to Amazon Kendra to improve the performance of
         your index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.submit_feedback)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#submit_feedback)
         """
+
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds the specified tag to the specified index, FAQ, or data source resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#tag_resource)
         """
+
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag from an index, FAQ, or a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#untag_resource)
         """
+
     def update_access_control_configuration(
         self,
         *,
         IndexId: str,
         Id: str,
         Name: str = ...,
         Description: str = ...,
@@ -759,14 +909,15 @@
     ) -> Dict[str, Any]:
         """
         Updates an access control configuration for your documents in an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_access_control_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_access_control_configuration)
         """
+
     def update_data_source(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         Configuration: DataSourceConfigurationTypeDef = ...,
@@ -779,14 +930,15 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra data source connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_data_source)
         """
+
     def update_experience(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         RoleArn: str = ...,
@@ -795,14 +947,33 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates your Amazon Kendra experience such as a search application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_experience)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_experience)
         """
+
+    def update_featured_results_set(
+        self,
+        *,
+        IndexId: str,
+        FeaturedResultsSetId: str,
+        FeaturedResultsSetName: str = ...,
+        Description: str = ...,
+        Status: FeaturedResultsSetStatusType = ...,
+        QueryTexts: Sequence[str] = ...,
+        FeaturedDocuments: Sequence[FeaturedDocumentTypeDef] = ...
+    ) -> UpdateFeaturedResultsSetResponseTypeDef:
+        """
+        Updates a set of featured results.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_featured_results_set)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_featured_results_set)
+        """
+
     def update_index(
         self,
         *,
         Id: str,
         Name: str = ...,
         RoleArn: str = ...,
         Description: str = ...,
@@ -814,14 +985,15 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing Amazon Kendra index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_index)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_index)
         """
+
     def update_query_suggestions_block_list(
         self,
         *,
         IndexId: str,
         Id: str,
         Name: str = ...,
         Description: str = ...,
@@ -830,30 +1002,33 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a block list used for query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_query_suggestions_block_list)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_query_suggestions_block_list)
         """
+
     def update_query_suggestions_config(
         self,
         *,
         IndexId: str,
         Mode: ModeType = ...,
         QueryLogLookBackWindowInDays: int = ...,
         IncludeQueriesWithoutUserInformation: bool = ...,
         MinimumNumberOfQueryingUsers: int = ...,
-        MinimumQueryCount: int = ...
+        MinimumQueryCount: int = ...,
+        AttributeSuggestionsConfig: AttributeSuggestionsUpdateConfigTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the settings of query suggestions for an index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra.Client.update_query_suggestions_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/client/#update_query_suggestions_config)
         """
+
     def update_thesaurus(
         self,
         *,
         Id: str,
         IndexId: str,
         Name: str = ...,
         Description: str = ...,
```

### Comparing `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/literals.py` & `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AdditionalResultAttributeValueTypeType",
     "AlfrescoEntityType",
+    "AttributeSuggestionsModeType",
     "ConditionOperatorType",
     "ConfluenceAttachmentFieldNameType",
     "ConfluenceAuthenticationTypeType",
     "ConfluenceBlogFieldNameType",
     "ConfluencePageFieldNameType",
     "ConfluenceSpaceFieldNameType",
     "ConfluenceVersionType",
@@ -38,14 +39,15 @@
     "DocumentStatusType",
     "EndpointTypeType",
     "EntityTypeType",
     "ErrorCodeType",
     "ExperienceStatusType",
     "FaqFileFormatType",
     "FaqStatusType",
+    "FeaturedResultsSetStatusType",
     "FsxFileSystemTypeType",
     "HighlightTypeType",
     "IndexEditionType",
     "IndexStatusType",
     "IntervalType",
     "IssueSubEntityType",
     "KeyLocationType",
@@ -68,14 +70,15 @@
     "ScoreConfidenceType",
     "ServiceNowAuthenticationTypeType",
     "ServiceNowBuildVersionTypeType",
     "SharePointOnlineAuthenticationTypeType",
     "SharePointVersionType",
     "SlackEntityType",
     "SortOrderType",
+    "SuggestionTypeType",
     "ThesaurusStatusType",
     "TypeType",
     "UserContextPolicyType",
     "UserGroupResolutionModeType",
     "WarningCodeType",
     "WebCrawlerModeType",
     "kendraServiceName",
@@ -83,14 +86,15 @@
     "ResourceServiceName",
     "RegionName",
 )
 
 
 AdditionalResultAttributeValueTypeType = Literal["TEXT_WITH_HIGHLIGHTS_VALUE"]
 AlfrescoEntityType = Literal["blog", "documentLibrary", "wiki"]
+AttributeSuggestionsModeType = Literal["ACTIVE", "INACTIVE"]
 ConditionOperatorType = Literal[
     "BeginsWith",
     "Contains",
     "Equals",
     "Exists",
     "GreaterThan",
     "GreaterThanOrEquals",
@@ -191,14 +195,15 @@
 ]
 EndpointTypeType = Literal["HOME"]
 EntityTypeType = Literal["GROUP", "USER"]
 ErrorCodeType = Literal["InternalError", "InvalidRequest"]
 ExperienceStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 FaqFileFormatType = Literal["CSV", "CSV_WITH_HEADER", "JSON"]
 FaqStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
+FeaturedResultsSetStatusType = Literal["ACTIVE", "INACTIVE"]
 FsxFileSystemTypeType = Literal["WINDOWS"]
 HighlightTypeType = Literal["STANDARD", "THESAURUS_SYNONYM"]
 IndexEditionType = Literal["DEVELOPER_EDITION", "ENTERPRISE_EDITION"]
 IndexStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "SYSTEM_UPDATING", "UPDATING"]
 IntervalType = Literal[
     "ONE_MONTH_AGO", "ONE_WEEK_AGO", "THIS_MONTH", "THIS_WEEK", "TWO_MONTHS_AGO", "TWO_WEEKS_AGO"
 ]
@@ -252,14 +257,15 @@
 ServiceNowBuildVersionTypeType = Literal["LONDON", "OTHERS"]
 SharePointOnlineAuthenticationTypeType = Literal["HTTP_BASIC", "OAUTH2"]
 SharePointVersionType = Literal[
     "SHAREPOINT_2013", "SHAREPOINT_2016", "SHAREPOINT_2019", "SHAREPOINT_ONLINE"
 ]
 SlackEntityType = Literal["DIRECT_MESSAGE", "GROUP_MESSAGE", "PRIVATE_CHANNEL", "PUBLIC_CHANNEL"]
 SortOrderType = Literal["ASC", "DESC"]
+SuggestionTypeType = Literal["DOCUMENT_ATTRIBUTES", "QUERY"]
 ThesaurusStatusType = Literal[
     "ACTIVE", "ACTIVE_BUT_UPDATE_FAILED", "CREATING", "DELETING", "FAILED", "UPDATING"
 ]
 TypeType = Literal["ON_PREMISE", "SAAS"]
 UserContextPolicyType = Literal["ATTRIBUTE_FILTER", "USER_TOKEN"]
 UserGroupResolutionModeType = Literal["AWS_SSO", "NONE"]
 WarningCodeType = Literal["QUERY_LANGUAGE_INVALID_SYNTAX"]
@@ -276,14 +282,15 @@
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
@@ -304,31 +311,34 @@
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
@@ -407,14 +417,15 @@
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
@@ -425,14 +436,15 @@
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
@@ -468,14 +480,15 @@
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
@@ -494,16 +507,19 @@
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
@@ -583,18 +599,21 @@
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
@@ -613,16 +632,18 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 RegionName = Literal[
+    "ap-northeast-1",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-west-1",
+    "eu-west-2",
     "us-east-1",
     "us-east-2",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/literals.pyi` & `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AdditionalResultAttributeValueTypeType",
     "AlfrescoEntityType",
+    "AttributeSuggestionsModeType",
     "ConditionOperatorType",
     "ConfluenceAttachmentFieldNameType",
     "ConfluenceAuthenticationTypeType",
     "ConfluenceBlogFieldNameType",
     "ConfluencePageFieldNameType",
     "ConfluenceSpaceFieldNameType",
     "ConfluenceVersionType",
@@ -37,14 +38,15 @@
     "DocumentStatusType",
     "EndpointTypeType",
     "EntityTypeType",
     "ErrorCodeType",
     "ExperienceStatusType",
     "FaqFileFormatType",
     "FaqStatusType",
+    "FeaturedResultsSetStatusType",
     "FsxFileSystemTypeType",
     "HighlightTypeType",
     "IndexEditionType",
     "IndexStatusType",
     "IntervalType",
     "IssueSubEntityType",
     "KeyLocationType",
@@ -67,28 +69,30 @@
     "ScoreConfidenceType",
     "ServiceNowAuthenticationTypeType",
     "ServiceNowBuildVersionTypeType",
     "SharePointOnlineAuthenticationTypeType",
     "SharePointVersionType",
     "SlackEntityType",
     "SortOrderType",
+    "SuggestionTypeType",
     "ThesaurusStatusType",
     "TypeType",
     "UserContextPolicyType",
     "UserGroupResolutionModeType",
     "WarningCodeType",
     "WebCrawlerModeType",
     "kendraServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 AdditionalResultAttributeValueTypeType = Literal["TEXT_WITH_HIGHLIGHTS_VALUE"]
 AlfrescoEntityType = Literal["blog", "documentLibrary", "wiki"]
+AttributeSuggestionsModeType = Literal["ACTIVE", "INACTIVE"]
 ConditionOperatorType = Literal[
     "BeginsWith",
     "Contains",
     "Equals",
     "Exists",
     "GreaterThan",
     "GreaterThanOrEquals",
@@ -189,14 +193,15 @@
 ]
 EndpointTypeType = Literal["HOME"]
 EntityTypeType = Literal["GROUP", "USER"]
 ErrorCodeType = Literal["InternalError", "InvalidRequest"]
 ExperienceStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 FaqFileFormatType = Literal["CSV", "CSV_WITH_HEADER", "JSON"]
 FaqStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
+FeaturedResultsSetStatusType = Literal["ACTIVE", "INACTIVE"]
 FsxFileSystemTypeType = Literal["WINDOWS"]
 HighlightTypeType = Literal["STANDARD", "THESAURUS_SYNONYM"]
 IndexEditionType = Literal["DEVELOPER_EDITION", "ENTERPRISE_EDITION"]
 IndexStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "SYSTEM_UPDATING", "UPDATING"]
 IntervalType = Literal[
     "ONE_MONTH_AGO", "ONE_WEEK_AGO", "THIS_MONTH", "THIS_WEEK", "TWO_MONTHS_AGO", "TWO_WEEKS_AGO"
 ]
@@ -250,14 +255,15 @@
 ServiceNowBuildVersionTypeType = Literal["LONDON", "OTHERS"]
 SharePointOnlineAuthenticationTypeType = Literal["HTTP_BASIC", "OAUTH2"]
 SharePointVersionType = Literal[
     "SHAREPOINT_2013", "SHAREPOINT_2016", "SHAREPOINT_2019", "SHAREPOINT_ONLINE"
 ]
 SlackEntityType = Literal["DIRECT_MESSAGE", "GROUP_MESSAGE", "PRIVATE_CHANNEL", "PUBLIC_CHANNEL"]
 SortOrderType = Literal["ASC", "DESC"]
+SuggestionTypeType = Literal["DOCUMENT_ATTRIBUTES", "QUERY"]
 ThesaurusStatusType = Literal[
     "ACTIVE", "ACTIVE_BUT_UPDATE_FAILED", "CREATING", "DELETING", "FAILED", "UPDATING"
 ]
 TypeType = Literal["ON_PREMISE", "SAAS"]
 UserContextPolicyType = Literal["ATTRIBUTE_FILTER", "USER_TOKEN"]
 UserGroupResolutionModeType = Literal["AWS_SSO", "NONE"]
 WarningCodeType = Literal["QUERY_LANGUAGE_INVALID_SYNTAX"]
@@ -274,14 +280,15 @@
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
@@ -302,31 +309,34 @@
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
@@ -405,14 +415,15 @@
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
@@ -423,14 +434,15 @@
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
@@ -466,14 +478,15 @@
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
@@ -492,16 +505,19 @@
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
@@ -581,18 +597,21 @@
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
@@ -611,16 +630,18 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 RegionName = Literal[
+    "ap-northeast-1",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-west-1",
+    "eu-west-2",
     "us-east-1",
     "us-east-2",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/type_defs.py` & `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AlfrescoEntityType,
+    AttributeSuggestionsModeType,
     ConditionOperatorType,
     ConfluenceAttachmentFieldNameType,
     ConfluenceAuthenticationTypeType,
     ConfluenceBlogFieldNameType,
     ConfluencePageFieldNameType,
     ConfluenceSpaceFieldNameType,
     ConfluenceVersionType,
@@ -34,14 +35,15 @@
     DocumentAttributeValueTypeType,
     DocumentStatusType,
     EntityTypeType,
     ErrorCodeType,
     ExperienceStatusType,
     FaqFileFormatType,
     FaqStatusType,
+    FeaturedResultsSetStatusType,
     HighlightTypeType,
     IndexEditionType,
     IndexStatusType,
     IntervalType,
     IssueSubEntityType,
     KeyLocationType,
     MetricTypeType,
@@ -63,14 +65,15 @@
     ScoreConfidenceType,
     ServiceNowAuthenticationTypeType,
     ServiceNowBuildVersionTypeType,
     SharePointOnlineAuthenticationTypeType,
     SharePointVersionType,
     SlackEntityType,
     SortOrderType,
+    SuggestionTypeType,
     ThesaurusStatusType,
     TypeType,
     UserContextPolicyType,
     UserGroupResolutionModeType,
     WebCrawlerModeType,
 )
 
@@ -89,19 +92,21 @@
     "AccessControlListConfigurationTypeDef",
     "AclConfigurationTypeDef",
     "DataSourceToIndexFieldMappingTypeDef",
     "DataSourceVpcConfigurationTypeDef",
     "S3PathTypeDef",
     "EntityConfigurationTypeDef",
     "FailedEntityTypeDef",
-    "ResponseMetadataTypeDef",
     "EntityPersonaConfigurationTypeDef",
+    "SuggestableConfigTypeDef",
     "BasicAuthenticationConfigurationTypeDef",
     "DataSourceSyncJobMetricTargetTypeDef",
     "BatchDeleteDocumentResponseFailedDocumentTypeDef",
+    "BatchDeleteFeaturedResultsSetErrorTypeDef",
+    "BatchDeleteFeaturedResultsSetRequestRequestTypeDef",
     "BatchGetDocumentStatusResponseErrorTypeDef",
     "StatusTypeDef",
     "BatchPutDocumentResponseFailedDocumentTypeDef",
     "CapacityUnitsConfigurationTypeDef",
     "ClearQuerySuggestionsRequestRequestTypeDef",
     "ClickFeedbackTypeDef",
     "ConfluenceAttachmentToIndexFieldMappingTypeDef",
@@ -109,17 +114,25 @@
     "ProxyConfigurationTypeDef",
     "ConfluencePageToIndexFieldMappingTypeDef",
     "ConfluenceSpaceToIndexFieldMappingTypeDef",
     "ConnectionConfigurationTypeDef",
     "ContentSourceConfigurationTypeDef",
     "CorrectionTypeDef",
     "PrincipalTypeDef",
+    "CreateAccessControlConfigurationResponseTypeDef",
     "TagTypeDef",
+    "CreateDataSourceResponseTypeDef",
+    "CreateExperienceResponseTypeDef",
+    "CreateFaqResponseTypeDef",
+    "FeaturedDocumentTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "UserGroupResolutionConfigurationTypeDef",
+    "CreateIndexResponseTypeDef",
+    "CreateQuerySuggestionsBlockListResponseTypeDef",
+    "CreateThesaurusResponseTypeDef",
     "TemplateConfigurationTypeDef",
     "DataSourceGroupTypeDef",
     "DataSourceSummaryTypeDef",
     "DataSourceSyncJobMetricsTypeDef",
     "SqlConfigurationTypeDef",
     "DeleteAccessControlConfigurationRequestRequestTypeDef",
     "DeleteDataSourceRequestRequestTypeDef",
@@ -130,32 +143,36 @@
     "DeleteQuerySuggestionsBlockListRequestRequestTypeDef",
     "DeleteThesaurusRequestRequestTypeDef",
     "DescribeAccessControlConfigurationRequestRequestTypeDef",
     "DescribeDataSourceRequestRequestTypeDef",
     "DescribeExperienceRequestRequestTypeDef",
     "ExperienceEndpointTypeDef",
     "DescribeFaqRequestRequestTypeDef",
+    "DescribeFeaturedResultsSetRequestRequestTypeDef",
+    "FeaturedDocumentMissingTypeDef",
+    "FeaturedDocumentWithMetadataTypeDef",
     "DescribeIndexRequestRequestTypeDef",
     "DescribePrincipalMappingRequestRequestTypeDef",
     "GroupOrderingIdSummaryTypeDef",
     "DescribeQuerySuggestionsBlockListRequestRequestTypeDef",
     "DescribeQuerySuggestionsConfigRequestRequestTypeDef",
     "DescribeThesaurusRequestRequestTypeDef",
     "DisassociatePersonasFromEntitiesRequestRequestTypeDef",
     "DocumentAttributeValueTypeDef",
     "RelevanceTypeDef",
     "SearchTypeDef",
     "DocumentsMetadataConfigurationTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EntityDisplayDataTypeDef",
     "UserIdentityConfigurationTypeDef",
     "FacetResultTypeDef",
     "FacetTypeDef",
     "FaqStatisticsTypeDef",
     "FaqSummaryTypeDef",
-    "GetQuerySuggestionsRequestRequestTypeDef",
+    "FeaturedResultsSetSummaryTypeDef",
     "GetSnapshotsRequestRequestTypeDef",
     "TimeRangeTypeDef",
     "GitHubDocumentCrawlPropertiesTypeDef",
     "SaaSConfigurationTypeDef",
     "MemberGroupTypeDef",
     "MemberUserTypeDef",
     "GroupSummaryTypeDef",
@@ -167,34 +184,37 @@
     "ListAccessControlConfigurationsRequestRequestTypeDef",
     "ListDataSourcesRequestRequestTypeDef",
     "ListEntityPersonasRequestRequestTypeDef",
     "PersonasSummaryTypeDef",
     "ListExperienceEntitiesRequestRequestTypeDef",
     "ListExperiencesRequestRequestTypeDef",
     "ListFaqsRequestRequestTypeDef",
+    "ListFeaturedResultsSetsRequestRequestTypeDef",
     "ListGroupsOlderThanOrderingIdRequestRequestTypeDef",
     "ListIndicesRequestRequestTypeDef",
     "ListQuerySuggestionsBlockListsRequestRequestTypeDef",
     "QuerySuggestionsBlockListSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListThesauriRequestRequestTypeDef",
     "ThesaurusSummaryTypeDef",
     "SortingConfigurationTypeDef",
     "SpellCorrectionConfigurationTypeDef",
     "ScoreAttributesTypeDef",
     "WarningTypeDef",
     "RelevanceFeedbackTypeDef",
+    "ResponseMetadataTypeDef",
     "SeedUrlConfigurationTypeDef",
     "SiteMapsConfigurationTypeDef",
     "StartDataSourceSyncJobRequestRequestTypeDef",
+    "StartDataSourceSyncJobResponseTypeDef",
     "StopDataSourceSyncJobRequestRequestTypeDef",
     "SuggestionHighlightTypeDef",
     "TableCellTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateQuerySuggestionsConfigRequestRequestTypeDef",
+    "ListAccessControlConfigurationsResponseTypeDef",
     "ColumnConfigurationTypeDef",
     "GoogleDriveConfigurationTypeDef",
     "SalesforceChatterFeedConfigurationTypeDef",
     "SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
     "SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
     "SalesforceStandardObjectAttachmentConfigurationTypeDef",
     "SalesforceStandardObjectConfigurationTypeDef",
@@ -203,71 +223,68 @@
     "WorkDocsConfigurationTypeDef",
     "BoxConfigurationTypeDef",
     "FsxConfigurationTypeDef",
     "JiraConfigurationTypeDef",
     "QuipConfigurationTypeDef",
     "SlackConfigurationTypeDef",
     "AlfrescoConfigurationTypeDef",
+    "DescribeFaqResponseTypeDef",
+    "DescribeQuerySuggestionsBlockListResponseTypeDef",
+    "DescribeThesaurusResponseTypeDef",
     "OnPremiseConfigurationTypeDef",
     "OneDriveUsersTypeDef",
     "UpdateQuerySuggestionsBlockListRequestRequestTypeDef",
     "UpdateThesaurusRequestRequestTypeDef",
     "AssociateEntitiesToExperienceRequestRequestTypeDef",
     "DisassociateEntitiesFromExperienceRequestRequestTypeDef",
     "AssociateEntitiesToExperienceResponseTypeDef",
     "AssociatePersonasToEntitiesResponseTypeDef",
-    "CreateAccessControlConfigurationResponseTypeDef",
-    "CreateDataSourceResponseTypeDef",
-    "CreateExperienceResponseTypeDef",
-    "CreateFaqResponseTypeDef",
-    "CreateIndexResponseTypeDef",
-    "CreateQuerySuggestionsBlockListResponseTypeDef",
-    "CreateThesaurusResponseTypeDef",
-    "DescribeFaqResponseTypeDef",
-    "DescribeQuerySuggestionsBlockListResponseTypeDef",
-    "DescribeQuerySuggestionsConfigResponseTypeDef",
-    "DescribeThesaurusResponseTypeDef",
     "DisassociateEntitiesFromExperienceResponseTypeDef",
     "DisassociatePersonasFromEntitiesResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListAccessControlConfigurationsResponseTypeDef",
-    "StartDataSourceSyncJobResponseTypeDef",
     "AssociatePersonasToEntitiesRequestRequestTypeDef",
+    "AttributeSuggestionsDescribeConfigTypeDef",
+    "AttributeSuggestionsUpdateConfigTypeDef",
     "AuthenticationConfigurationTypeDef",
     "BatchDeleteDocumentRequestRequestTypeDef",
     "BatchDeleteDocumentResponseTypeDef",
+    "BatchDeleteFeaturedResultsSetResponseTypeDef",
     "BatchGetDocumentStatusResponseTypeDef",
     "BatchPutDocumentResponseTypeDef",
     "ConfluenceAttachmentConfigurationTypeDef",
     "ConfluenceBlogConfigurationTypeDef",
     "SharePointConfigurationTypeDef",
     "ConfluencePageConfigurationTypeDef",
     "ConfluenceSpaceConfigurationTypeDef",
     "SpellCorrectedQueryTypeDef",
     "HierarchicalPrincipalTypeDef",
     "CreateFaqRequestRequestTypeDef",
     "CreateQuerySuggestionsBlockListRequestRequestTypeDef",
     "CreateThesaurusRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateFeaturedResultsSetRequestRequestTypeDef",
+    "FeaturedResultsSetTypeDef",
+    "UpdateFeaturedResultsSetRequestRequestTypeDef",
     "UserContextTypeDef",
     "ListDataSourcesResponseTypeDef",
     "DataSourceSyncJobTypeDef",
     "ExperiencesSummaryTypeDef",
+    "DescribeFeaturedResultsSetResponseTypeDef",
     "DescribePrincipalMappingResponseTypeDef",
     "DocumentAttributeConditionTypeDef",
     "DocumentAttributeTargetTypeDef",
     "DocumentAttributeTypeDef",
     "DocumentAttributeValueCountPairTypeDef",
     "DocumentRelevanceConfigurationTypeDef",
     "DocumentMetadataConfigurationTypeDef",
     "S3DataSourceConfigurationTypeDef",
     "ExperienceEntitiesSummaryTypeDef",
     "ExperienceConfigurationTypeDef",
     "ListFaqsResponseTypeDef",
+    "ListFeaturedResultsSetsResponseTypeDef",
     "GetSnapshotsResponseTypeDef",
     "ListDataSourceSyncJobsRequestRequestTypeDef",
     "GroupMembersTypeDef",
     "ListGroupsOlderThanOrderingIdResponseTypeDef",
     "TextWithHighlightsTypeDef",
     "ListIndicesResponseTypeDef",
     "IndexStatisticsTypeDef",
@@ -280,45 +297,56 @@
     "SuggestionTextWithHighlightsTypeDef",
     "TableRowTypeDef",
     "DatabaseConfigurationTypeDef",
     "SalesforceKnowledgeArticleConfigurationTypeDef",
     "ServiceNowConfigurationTypeDef",
     "GitHubConfigurationTypeDef",
     "OneDriveConfigurationTypeDef",
+    "DescribeQuerySuggestionsConfigResponseTypeDef",
+    "UpdateQuerySuggestionsConfigRequestRequestTypeDef",
     "ConfluenceConfigurationTypeDef",
     "CreateAccessControlConfigurationRequestRequestTypeDef",
     "DescribeAccessControlConfigurationResponseTypeDef",
     "UpdateAccessControlConfigurationRequestRequestTypeDef",
+    "CreateFeaturedResultsSetResponseTypeDef",
+    "UpdateFeaturedResultsSetResponseTypeDef",
+    "AttributeSuggestionsGetConfigTypeDef",
     "ListDataSourceSyncJobsResponseTypeDef",
     "ListExperiencesResponseTypeDef",
     "HookConfigurationTypeDef",
     "InlineCustomDocumentEnrichmentConfigurationTypeDef",
     "AttributeFilterTypeDef",
     "DocumentInfoTypeDef",
     "DocumentTypeDef",
+    "RetrieveResultItemTypeDef",
+    "SourceDocumentTypeDef",
     "QueryRequestRequestTypeDef",
+    "RetrieveRequestRequestTypeDef",
     "ListExperienceEntitiesResponseTypeDef",
     "CreateExperienceRequestRequestTypeDef",
     "DescribeExperienceResponseTypeDef",
     "UpdateExperienceRequestRequestTypeDef",
     "PutPrincipalMappingRequestRequestTypeDef",
     "AdditionalResultAttributeValueTypeDef",
     "CreateIndexRequestRequestTypeDef",
     "DescribeIndexResponseTypeDef",
     "UpdateIndexRequestRequestTypeDef",
     "WebCrawlerConfigurationTypeDef",
     "SuggestionValueTypeDef",
     "TableExcerptTypeDef",
     "SalesforceConfigurationTypeDef",
+    "GetQuerySuggestionsRequestRequestTypeDef",
     "CustomDocumentEnrichmentConfigurationTypeDef",
     "BatchGetDocumentStatusRequestRequestTypeDef",
+    "RetrieveResultTypeDef",
     "AdditionalResultAttributeTypeDef",
     "SuggestionTypeDef",
     "DataSourceConfigurationTypeDef",
     "BatchPutDocumentRequestRequestTypeDef",
+    "FeaturedResultsItemTypeDef",
     "QueryResultItemTypeDef",
     "GetQuerySuggestionsResponseTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
     "DescribeDataSourceResponseTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
     "QueryResultTypeDef",
 )
@@ -396,33 +424,31 @@
     {
         "EntityId": str,
         "ErrorMessage": str,
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
 EntityPersonaConfigurationTypeDef = TypedDict(
     "EntityPersonaConfigurationTypeDef",
     {
         "EntityId": str,
         "Persona": PersonaType,
     },
 )
 
+SuggestableConfigTypeDef = TypedDict(
+    "SuggestableConfigTypeDef",
+    {
+        "AttributeName": str,
+        "Suggestable": bool,
+    },
+    total=False,
+)
+
 BasicAuthenticationConfigurationTypeDef = TypedDict(
     "BasicAuthenticationConfigurationTypeDef",
     {
         "Host": str,
         "Port": int,
         "Credentials": str,
     },
@@ -455,14 +481,31 @@
         "Id": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+BatchDeleteFeaturedResultsSetErrorTypeDef = TypedDict(
+    "BatchDeleteFeaturedResultsSetErrorTypeDef",
+    {
+        "Id": str,
+        "ErrorCode": ErrorCodeType,
+        "ErrorMessage": str,
+    },
+)
+
+BatchDeleteFeaturedResultsSetRequestRequestTypeDef = TypedDict(
+    "BatchDeleteFeaturedResultsSetRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "FeaturedResultsSetIds": Sequence[str],
+    },
+)
+
 BatchGetDocumentStatusResponseErrorTypeDef = TypedDict(
     "BatchGetDocumentStatusResponseErrorTypeDef",
     {
         "DocumentId": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
@@ -624,22 +667,62 @@
 )
 
 
 class PrincipalTypeDef(_RequiredPrincipalTypeDef, _OptionalPrincipalTypeDef):
     pass
 
 
+CreateAccessControlConfigurationResponseTypeDef = TypedDict(
+    "CreateAccessControlConfigurationResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateDataSourceResponseTypeDef = TypedDict(
+    "CreateDataSourceResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateExperienceResponseTypeDef = TypedDict(
+    "CreateExperienceResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateFaqResponseTypeDef = TypedDict(
+    "CreateFaqResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+FeaturedDocumentTypeDef = TypedDict(
+    "FeaturedDocumentTypeDef",
+    {
+        "Id": str,
+    },
+    total=False,
+)
+
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
@@ -647,14 +730,38 @@
 UserGroupResolutionConfigurationTypeDef = TypedDict(
     "UserGroupResolutionConfigurationTypeDef",
     {
         "UserGroupResolutionMode": UserGroupResolutionModeType,
     },
 )
 
+CreateIndexResponseTypeDef = TypedDict(
+    "CreateIndexResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateQuerySuggestionsBlockListResponseTypeDef = TypedDict(
+    "CreateQuerySuggestionsBlockListResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateThesaurusResponseTypeDef = TypedDict(
+    "CreateThesaurusResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TemplateConfigurationTypeDef = TypedDict(
     "TemplateConfigurationTypeDef",
     {
         "Template": Mapping[str, Any],
     },
     total=False,
 )
@@ -817,14 +924,40 @@
     "DescribeFaqRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
 
+DescribeFeaturedResultsSetRequestRequestTypeDef = TypedDict(
+    "DescribeFeaturedResultsSetRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "FeaturedResultsSetId": str,
+    },
+)
+
+FeaturedDocumentMissingTypeDef = TypedDict(
+    "FeaturedDocumentMissingTypeDef",
+    {
+        "Id": str,
+    },
+    total=False,
+)
+
+FeaturedDocumentWithMetadataTypeDef = TypedDict(
+    "FeaturedDocumentWithMetadataTypeDef",
+    {
+        "Id": str,
+        "Title": str,
+        "URI": str,
+    },
+    total=False,
+)
+
 DescribeIndexRequestRequestTypeDef = TypedDict(
     "DescribeIndexRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -933,14 +1066,21 @@
     "DocumentsMetadataConfigurationTypeDef",
     {
         "S3Prefix": str,
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
 EntityDisplayDataTypeDef = TypedDict(
     "EntityDisplayDataTypeDef",
     {
         "UserName": str,
         "GroupName": str,
         "IdentifiedUserName": str,
         "FirstName": str,
@@ -994,37 +1134,26 @@
         "UpdatedAt": datetime,
         "FileFormat": FaqFileFormatType,
         "LanguageCode": str,
     },
     total=False,
 )
 
-_RequiredGetQuerySuggestionsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetQuerySuggestionsRequestRequestTypeDef",
+FeaturedResultsSetSummaryTypeDef = TypedDict(
+    "FeaturedResultsSetSummaryTypeDef",
     {
-        "IndexId": str,
-        "QueryText": str,
-    },
-)
-_OptionalGetQuerySuggestionsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetQuerySuggestionsRequestRequestTypeDef",
-    {
-        "MaxSuggestionsCount": int,
+        "FeaturedResultsSetId": str,
+        "FeaturedResultsSetName": str,
+        "Status": FeaturedResultsSetStatusType,
+        "LastUpdatedTimestamp": int,
+        "CreationTimestamp": int,
     },
     total=False,
 )
 
-
-class GetQuerySuggestionsRequestRequestTypeDef(
-    _RequiredGetQuerySuggestionsRequestRequestTypeDef,
-    _OptionalGetQuerySuggestionsRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredGetSnapshotsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSnapshotsRequestRequestTypeDef",
     {
         "IndexId": str,
         "Interval": IntervalType,
         "MetricType": MetricTypeType,
     },
@@ -1342,14 +1471,37 @@
 
 class ListFaqsRequestRequestTypeDef(
     _RequiredListFaqsRequestRequestTypeDef, _OptionalListFaqsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListFeaturedResultsSetsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFeaturedResultsSetsRequestRequestTypeDef",
+    {
+        "IndexId": str,
+    },
+)
+_OptionalListFeaturedResultsSetsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFeaturedResultsSetsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListFeaturedResultsSetsRequestRequestTypeDef(
+    _RequiredListFeaturedResultsSetsRequestRequestTypeDef,
+    _OptionalListFeaturedResultsSetsRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredListGroupsOlderThanOrderingIdRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsOlderThanOrderingIdRequestRequestTypeDef",
     {
         "IndexId": str,
         "OrderingId": int,
     },
 )
@@ -1493,14 +1645,25 @@
     "RelevanceFeedbackTypeDef",
     {
         "ResultId": str,
         "RelevanceValue": RelevanceTypeType,
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
 _RequiredSeedUrlConfigurationTypeDef = TypedDict(
     "_RequiredSeedUrlConfigurationTypeDef",
     {
         "SeedUrls": Sequence[str],
     },
 )
 _OptionalSeedUrlConfigurationTypeDef = TypedDict(
@@ -1529,14 +1692,22 @@
     "StartDataSourceSyncJobRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
 
+StartDataSourceSyncJobResponseTypeDef = TypedDict(
+    "StartDataSourceSyncJobResponseTypeDef",
+    {
+        "ExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopDataSourceSyncJobRequestRequestTypeDef = TypedDict(
     "StopDataSourceSyncJobRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -1565,40 +1736,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef",
-    {
-        "IndexId": str,
-    },
-)
-_OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef",
+ListAccessControlConfigurationsResponseTypeDef = TypedDict(
+    "ListAccessControlConfigurationsResponseTypeDef",
     {
-        "Mode": ModeType,
-        "QueryLogLookBackWindowInDays": int,
-        "IncludeQueriesWithoutUserInformation": bool,
-        "MinimumNumberOfQueryingUsers": int,
-        "MinimumQueryCount": int,
+        "NextToken": str,
+        "AccessControlConfigurations": List[AccessControlConfigurationSummaryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class UpdateQuerySuggestionsConfigRequestRequestTypeDef(
-    _RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef,
-    _OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredColumnConfigurationTypeDef = TypedDict(
     "_RequiredColumnConfigurationTypeDef",
     {
         "DocumentIdColumnName": str,
         "DocumentDataColumnName": str,
         "ChangeDetectingColumns": Sequence[str],
     },
@@ -2007,14 +2161,72 @@
 
 class AlfrescoConfigurationTypeDef(
     _RequiredAlfrescoConfigurationTypeDef, _OptionalAlfrescoConfigurationTypeDef
 ):
     pass
 
 
+DescribeFaqResponseTypeDef = TypedDict(
+    "DescribeFaqResponseTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+        "Name": str,
+        "Description": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "S3Path": S3PathTypeDef,
+        "Status": FaqStatusType,
+        "RoleArn": str,
+        "ErrorMessage": str,
+        "FileFormat": FaqFileFormatType,
+        "LanguageCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeQuerySuggestionsBlockListResponseTypeDef = TypedDict(
+    "DescribeQuerySuggestionsBlockListResponseTypeDef",
+    {
+        "IndexId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "Status": QuerySuggestionsBlockListStatusType,
+        "ErrorMessage": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "SourceS3Path": S3PathTypeDef,
+        "ItemCount": int,
+        "FileSizeBytes": int,
+        "RoleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeThesaurusResponseTypeDef = TypedDict(
+    "DescribeThesaurusResponseTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+        "Name": str,
+        "Description": str,
+        "Status": ThesaurusStatusType,
+        "ErrorMessage": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "RoleArn": str,
+        "SourceS3Path": S3PathTypeDef,
+        "FileSizeBytes": int,
+        "TermCount": int,
+        "SynonymRuleCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 OnPremiseConfigurationTypeDef = TypedDict(
     "OnPremiseConfigurationTypeDef",
     {
         "HostUrl": str,
         "OrganizationName": str,
         "SslCertificateS3Path": S3PathTypeDef,
     },
@@ -2098,203 +2310,67 @@
     },
 )
 
 AssociateEntitiesToExperienceResponseTypeDef = TypedDict(
     "AssociateEntitiesToExperienceResponseTypeDef",
     {
         "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociatePersonasToEntitiesResponseTypeDef = TypedDict(
     "AssociatePersonasToEntitiesResponseTypeDef",
     {
         "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAccessControlConfigurationResponseTypeDef = TypedDict(
-    "CreateAccessControlConfigurationResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDataSourceResponseTypeDef = TypedDict(
-    "CreateDataSourceResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateExperienceResponseTypeDef = TypedDict(
-    "CreateExperienceResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFaqResponseTypeDef = TypedDict(
-    "CreateFaqResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIndexResponseTypeDef = TypedDict(
-    "CreateIndexResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateQuerySuggestionsBlockListResponseTypeDef = TypedDict(
-    "CreateQuerySuggestionsBlockListResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateThesaurusResponseTypeDef = TypedDict(
-    "CreateThesaurusResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFaqResponseTypeDef = TypedDict(
-    "DescribeFaqResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Description": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "S3Path": S3PathTypeDef,
-        "Status": FaqStatusType,
-        "RoleArn": str,
-        "ErrorMessage": str,
-        "FileFormat": FaqFileFormatType,
-        "LanguageCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeQuerySuggestionsBlockListResponseTypeDef = TypedDict(
-    "DescribeQuerySuggestionsBlockListResponseTypeDef",
-    {
-        "IndexId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "Status": QuerySuggestionsBlockListStatusType,
-        "ErrorMessage": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "SourceS3Path": S3PathTypeDef,
-        "ItemCount": int,
-        "FileSizeBytes": int,
-        "RoleArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeQuerySuggestionsConfigResponseTypeDef = TypedDict(
-    "DescribeQuerySuggestionsConfigResponseTypeDef",
-    {
-        "Mode": ModeType,
-        "Status": QuerySuggestionsStatusType,
-        "QueryLogLookBackWindowInDays": int,
-        "IncludeQueriesWithoutUserInformation": bool,
-        "MinimumNumberOfQueryingUsers": int,
-        "MinimumQueryCount": int,
-        "LastSuggestionsBuildTime": datetime,
-        "LastClearTime": datetime,
-        "TotalSuggestionsCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeThesaurusResponseTypeDef = TypedDict(
-    "DescribeThesaurusResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Description": str,
-        "Status": ThesaurusStatusType,
-        "ErrorMessage": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "RoleArn": str,
-        "SourceS3Path": S3PathTypeDef,
-        "FileSizeBytes": int,
-        "TermCount": int,
-        "SynonymRuleCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateEntitiesFromExperienceResponseTypeDef = TypedDict(
     "DisassociateEntitiesFromExperienceResponseTypeDef",
     {
         "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociatePersonasFromEntitiesResponseTypeDef = TypedDict(
     "DisassociatePersonasFromEntitiesResponseTypeDef",
     {
         "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+AssociatePersonasToEntitiesRequestRequestTypeDef = TypedDict(
+    "AssociatePersonasToEntitiesRequestRequestTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Id": str,
+        "IndexId": str,
+        "Personas": Sequence[EntityPersonaConfigurationTypeDef],
     },
 )
 
-ListAccessControlConfigurationsResponseTypeDef = TypedDict(
-    "ListAccessControlConfigurationsResponseTypeDef",
+AttributeSuggestionsDescribeConfigTypeDef = TypedDict(
+    "AttributeSuggestionsDescribeConfigTypeDef",
     {
-        "NextToken": str,
-        "AccessControlConfigurations": List[AccessControlConfigurationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SuggestableConfigList": List[SuggestableConfigTypeDef],
+        "AttributeSuggestionsMode": AttributeSuggestionsModeType,
     },
+    total=False,
 )
 
-StartDataSourceSyncJobResponseTypeDef = TypedDict(
-    "StartDataSourceSyncJobResponseTypeDef",
+AttributeSuggestionsUpdateConfigTypeDef = TypedDict(
+    "AttributeSuggestionsUpdateConfigTypeDef",
     {
-        "ExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociatePersonasToEntitiesRequestRequestTypeDef = TypedDict(
-    "AssociatePersonasToEntitiesRequestRequestTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Personas": Sequence[EntityPersonaConfigurationTypeDef],
+        "SuggestableConfigList": Sequence[SuggestableConfigTypeDef],
+        "AttributeSuggestionsMode": AttributeSuggestionsModeType,
     },
+    total=False,
 )
 
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
         "BasicAuthentication": Sequence[BasicAuthenticationConfigurationTypeDef],
     },
@@ -2324,32 +2400,40 @@
     pass
 
 
 BatchDeleteDocumentResponseTypeDef = TypedDict(
     "BatchDeleteDocumentResponseTypeDef",
     {
         "FailedDocuments": List[BatchDeleteDocumentResponseFailedDocumentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchDeleteFeaturedResultsSetResponseTypeDef = TypedDict(
+    "BatchDeleteFeaturedResultsSetResponseTypeDef",
+    {
+        "Errors": List[BatchDeleteFeaturedResultsSetErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetDocumentStatusResponseTypeDef = TypedDict(
     "BatchGetDocumentStatusResponseTypeDef",
     {
         "Errors": List[BatchGetDocumentStatusResponseErrorTypeDef],
         "DocumentStatusList": List[StatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutDocumentResponseTypeDef = TypedDict(
     "BatchPutDocumentResponseTypeDef",
     {
         "FailedDocuments": List[BatchPutDocumentResponseFailedDocumentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfluenceAttachmentConfigurationTypeDef = TypedDict(
     "ConfluenceAttachmentConfigurationTypeDef",
     {
         "CrawlAttachments": bool,
@@ -2516,26 +2600,96 @@
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredCreateFeaturedResultsSetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFeaturedResultsSetRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "FeaturedResultsSetName": str,
+    },
+)
+_OptionalCreateFeaturedResultsSetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFeaturedResultsSetRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ClientToken": str,
+        "Status": FeaturedResultsSetStatusType,
+        "QueryTexts": Sequence[str],
+        "FeaturedDocuments": Sequence[FeaturedDocumentTypeDef],
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateFeaturedResultsSetRequestRequestTypeDef(
+    _RequiredCreateFeaturedResultsSetRequestRequestTypeDef,
+    _OptionalCreateFeaturedResultsSetRequestRequestTypeDef,
+):
+    pass
+
+
+FeaturedResultsSetTypeDef = TypedDict(
+    "FeaturedResultsSetTypeDef",
+    {
+        "FeaturedResultsSetId": str,
+        "FeaturedResultsSetName": str,
+        "Description": str,
+        "Status": FeaturedResultsSetStatusType,
+        "QueryTexts": List[str],
+        "FeaturedDocuments": List[FeaturedDocumentTypeDef],
+        "LastUpdatedTimestamp": int,
+        "CreationTimestamp": int,
+    },
+    total=False,
+)
+
+_RequiredUpdateFeaturedResultsSetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFeaturedResultsSetRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "FeaturedResultsSetId": str,
+    },
+)
+_OptionalUpdateFeaturedResultsSetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFeaturedResultsSetRequestRequestTypeDef",
+    {
+        "FeaturedResultsSetName": str,
+        "Description": str,
+        "Status": FeaturedResultsSetStatusType,
+        "QueryTexts": Sequence[str],
+        "FeaturedDocuments": Sequence[FeaturedDocumentTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateFeaturedResultsSetRequestRequestTypeDef(
+    _RequiredUpdateFeaturedResultsSetRequestRequestTypeDef,
+    _OptionalUpdateFeaturedResultsSetRequestRequestTypeDef,
+):
+    pass
+
+
 UserContextTypeDef = TypedDict(
     "UserContextTypeDef",
     {
         "Token": str,
         "UserId": str,
         "Groups": Sequence[str],
         "DataSourceGroups": Sequence[DataSourceGroupTypeDef],
@@ -2544,15 +2698,15 @@
 )
 
 ListDataSourcesResponseTypeDef = TypedDict(
     "ListDataSourcesResponseTypeDef",
     {
         "SummaryItems": List[DataSourceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataSourceSyncJobTypeDef = TypedDict(
     "DataSourceSyncJobTypeDef",
     {
         "ExecutionId": str,
@@ -2575,22 +2729,38 @@
         "CreatedAt": datetime,
         "Status": ExperienceStatusType,
         "Endpoints": List[ExperienceEndpointTypeDef],
     },
     total=False,
 )
 
+DescribeFeaturedResultsSetResponseTypeDef = TypedDict(
+    "DescribeFeaturedResultsSetResponseTypeDef",
+    {
+        "FeaturedResultsSetId": str,
+        "FeaturedResultsSetName": str,
+        "Description": str,
+        "Status": FeaturedResultsSetStatusType,
+        "QueryTexts": List[str],
+        "FeaturedDocumentsWithMetadata": List[FeaturedDocumentWithMetadataTypeDef],
+        "FeaturedDocumentsMissing": List[FeaturedDocumentMissingTypeDef],
+        "LastUpdatedTimestamp": int,
+        "CreationTimestamp": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribePrincipalMappingResponseTypeDef = TypedDict(
     "DescribePrincipalMappingResponseTypeDef",
     {
         "IndexId": str,
         "DataSourceId": str,
         "GroupId": str,
         "GroupOrderingIdSummaries": List[GroupOrderingIdSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDocumentAttributeConditionTypeDef = TypedDict(
     "_RequiredDocumentAttributeConditionTypeDef",
     {
         "ConditionDocumentAttributeKey": str,
@@ -2716,26 +2886,35 @@
 )
 
 ListFaqsResponseTypeDef = TypedDict(
     "ListFaqsResponseTypeDef",
     {
         "NextToken": str,
         "FaqSummaryItems": List[FaqSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListFeaturedResultsSetsResponseTypeDef = TypedDict(
+    "ListFeaturedResultsSetsResponseTypeDef",
+    {
+        "FeaturedResultsSetSummaryItems": List[FeaturedResultsSetSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSnapshotsResponseTypeDef = TypedDict(
     "GetSnapshotsResponseTypeDef",
     {
         "SnapShotTimeFilter": TimeRangeTypeDef,
         "SnapshotsDataHeader": List[str],
         "SnapshotsData": List[List[str]],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSourceSyncJobsRequestRequestTypeDef",
     {
         "Id": str,
@@ -2772,15 +2951,15 @@
 )
 
 ListGroupsOlderThanOrderingIdResponseTypeDef = TypedDict(
     "ListGroupsOlderThanOrderingIdResponseTypeDef",
     {
         "GroupsSummaries": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TextWithHighlightsTypeDef = TypedDict(
     "TextWithHighlightsTypeDef",
     {
         "Text": str,
@@ -2790,15 +2969,15 @@
 )
 
 ListIndicesResponseTypeDef = TypedDict(
     "ListIndicesResponseTypeDef",
     {
         "IndexConfigurationSummaryItems": List[IndexConfigurationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IndexStatisticsTypeDef = TypedDict(
     "IndexStatisticsTypeDef",
     {
         "FaqStatistics": FaqStatisticsTypeDef,
@@ -2816,33 +2995,33 @@
 )
 
 ListEntityPersonasResponseTypeDef = TypedDict(
     "ListEntityPersonasResponseTypeDef",
     {
         "SummaryItems": List[PersonasSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListQuerySuggestionsBlockListsResponseTypeDef = TypedDict(
     "ListQuerySuggestionsBlockListsResponseTypeDef",
     {
         "BlockListSummaryItems": List[QuerySuggestionsBlockListSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListThesauriResponseTypeDef = TypedDict(
     "ListThesauriResponseTypeDef",
     {
         "NextToken": str,
         "ThesaurusSummaryItems": List[ThesaurusSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSubmitFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitFeedbackRequestRequestTypeDef",
     {
         "IndexId": str,
@@ -2921,15 +3100,17 @@
     {
         "IncludedStates": Sequence[SalesforceKnowledgeArticleStateType],
     },
 )
 _OptionalSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
     "_OptionalSalesforceKnowledgeArticleConfigurationTypeDef",
     {
-        "StandardKnowledgeArticleTypeConfiguration": SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
+        "StandardKnowledgeArticleTypeConfiguration": (
+            SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef
+        ),
         "CustomKnowledgeArticleTypeConfigurations": Sequence[
             SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef
         ],
     },
     total=False,
 )
 
@@ -3043,14 +3224,58 @@
 
 class OneDriveConfigurationTypeDef(
     _RequiredOneDriveConfigurationTypeDef, _OptionalOneDriveConfigurationTypeDef
 ):
     pass
 
 
+DescribeQuerySuggestionsConfigResponseTypeDef = TypedDict(
+    "DescribeQuerySuggestionsConfigResponseTypeDef",
+    {
+        "Mode": ModeType,
+        "Status": QuerySuggestionsStatusType,
+        "QueryLogLookBackWindowInDays": int,
+        "IncludeQueriesWithoutUserInformation": bool,
+        "MinimumNumberOfQueryingUsers": int,
+        "MinimumQueryCount": int,
+        "LastSuggestionsBuildTime": datetime,
+        "LastClearTime": datetime,
+        "TotalSuggestionsCount": int,
+        "AttributeSuggestionsConfig": AttributeSuggestionsDescribeConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef",
+    {
+        "IndexId": str,
+    },
+)
+_OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef",
+    {
+        "Mode": ModeType,
+        "QueryLogLookBackWindowInDays": int,
+        "IncludeQueriesWithoutUserInformation": bool,
+        "MinimumNumberOfQueryingUsers": int,
+        "MinimumQueryCount": int,
+        "AttributeSuggestionsConfig": AttributeSuggestionsUpdateConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateQuerySuggestionsConfigRequestRequestTypeDef(
+    _RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef,
+    _OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredConfluenceConfigurationTypeDef = TypedDict(
     "_RequiredConfluenceConfigurationTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
         "Version": ConfluenceVersionType,
     },
@@ -3108,15 +3333,15 @@
     "DescribeAccessControlConfigurationResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "ErrorMessage": str,
         "AccessControlList": List[PrincipalTypeDef],
         "HierarchicalAccessControlList": List[HierarchicalPrincipalTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef",
     {
         "IndexId": str,
@@ -3138,29 +3363,56 @@
 class UpdateAccessControlConfigurationRequestRequestTypeDef(
     _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef,
     _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+CreateFeaturedResultsSetResponseTypeDef = TypedDict(
+    "CreateFeaturedResultsSetResponseTypeDef",
+    {
+        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateFeaturedResultsSetResponseTypeDef = TypedDict(
+    "UpdateFeaturedResultsSetResponseTypeDef",
+    {
+        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AttributeSuggestionsGetConfigTypeDef = TypedDict(
+    "AttributeSuggestionsGetConfigTypeDef",
+    {
+        "SuggestionAttributes": Sequence[str],
+        "AdditionalResponseAttributes": Sequence[str],
+        "AttributeFilter": "AttributeFilterTypeDef",
+        "UserContext": UserContextTypeDef,
+    },
+    total=False,
+)
+
 ListDataSourceSyncJobsResponseTypeDef = TypedDict(
     "ListDataSourceSyncJobsResponseTypeDef",
     {
         "History": List[DataSourceSyncJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExperiencesResponseTypeDef = TypedDict(
     "ListExperiencesResponseTypeDef",
     {
         "SummaryItems": List[ExperiencesSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredHookConfigurationTypeDef = TypedDict(
     "_RequiredHookConfigurationTypeDef",
     {
         "LambdaArn": str,
@@ -3250,14 +3502,37 @@
 )
 
 
 class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
     pass
 
 
+RetrieveResultItemTypeDef = TypedDict(
+    "RetrieveResultItemTypeDef",
+    {
+        "Id": str,
+        "DocumentId": str,
+        "DocumentTitle": str,
+        "Content": str,
+        "DocumentURI": str,
+        "DocumentAttributes": List[DocumentAttributeTypeDef],
+    },
+    total=False,
+)
+
+SourceDocumentTypeDef = TypedDict(
+    "SourceDocumentTypeDef",
+    {
+        "DocumentId": str,
+        "SuggestionAttributes": List[str],
+        "AdditionalAttributes": List[DocumentAttributeTypeDef],
+    },
+    total=False,
+)
+
 _RequiredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredQueryRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalQueryRequestRequestTypeDef = TypedDict(
@@ -3282,20 +3557,47 @@
 
 class QueryRequestRequestTypeDef(
     _RequiredQueryRequestRequestTypeDef, _OptionalQueryRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredRetrieveRequestRequestTypeDef = TypedDict(
+    "_RequiredRetrieveRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "QueryText": str,
+    },
+)
+_OptionalRetrieveRequestRequestTypeDef = TypedDict(
+    "_OptionalRetrieveRequestRequestTypeDef",
+    {
+        "AttributeFilter": "AttributeFilterTypeDef",
+        "RequestedDocumentAttributes": Sequence[str],
+        "DocumentRelevanceOverrideConfigurations": Sequence[DocumentRelevanceConfigurationTypeDef],
+        "PageNumber": int,
+        "PageSize": int,
+        "UserContext": UserContextTypeDef,
+    },
+    total=False,
+)
+
+
+class RetrieveRequestRequestTypeDef(
+    _RequiredRetrieveRequestRequestTypeDef, _OptionalRetrieveRequestRequestTypeDef
+):
+    pass
+
+
 ListExperienceEntitiesResponseTypeDef = TypedDict(
     "ListExperienceEntitiesResponseTypeDef",
     {
         "SummaryItems": List[ExperienceEntitiesSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperienceRequestRequestTypeDef",
     {
         "Name": str,
@@ -3330,15 +3632,15 @@
         "Configuration": ExperienceConfigurationTypeDef,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "Description": str,
         "Status": ExperienceStatusType,
         "RoleArn": str,
         "ErrorMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExperienceRequestRequestTypeDef",
     {
         "Id": str,
@@ -3441,15 +3743,15 @@
         "DocumentMetadataConfigurations": List[DocumentMetadataConfigurationTypeDef],
         "IndexStatistics": IndexStatisticsTypeDef,
         "ErrorMessage": str,
         "CapacityUnits": CapacityUnitsConfigurationTypeDef,
         "UserTokenConfigurations": List[UserTokenConfigurationTypeDef],
         "UserContextPolicy": UserContextPolicyType,
         "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateIndexRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIndexRequestRequestTypeDef",
     {
         "Id": str,
@@ -3532,28 +3834,55 @@
 _OptionalSalesforceConfigurationTypeDef = TypedDict(
     "_OptionalSalesforceConfigurationTypeDef",
     {
         "StandardObjectConfigurations": Sequence[SalesforceStandardObjectConfigurationTypeDef],
         "KnowledgeArticleConfiguration": SalesforceKnowledgeArticleConfigurationTypeDef,
         "ChatterFeedConfiguration": SalesforceChatterFeedConfigurationTypeDef,
         "CrawlAttachments": bool,
-        "StandardObjectAttachmentConfiguration": SalesforceStandardObjectAttachmentConfigurationTypeDef,
+        "StandardObjectAttachmentConfiguration": (
+            SalesforceStandardObjectAttachmentConfigurationTypeDef
+        ),
         "IncludeAttachmentFilePatterns": Sequence[str],
         "ExcludeAttachmentFilePatterns": Sequence[str],
     },
     total=False,
 )
 
 
 class SalesforceConfigurationTypeDef(
     _RequiredSalesforceConfigurationTypeDef, _OptionalSalesforceConfigurationTypeDef
 ):
     pass
 
 
+_RequiredGetQuerySuggestionsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetQuerySuggestionsRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "QueryText": str,
+    },
+)
+_OptionalGetQuerySuggestionsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetQuerySuggestionsRequestRequestTypeDef",
+    {
+        "MaxSuggestionsCount": int,
+        "SuggestionTypes": Sequence[SuggestionTypeType],
+        "AttributeSuggestionsConfig": AttributeSuggestionsGetConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetQuerySuggestionsRequestRequestTypeDef(
+    _RequiredGetQuerySuggestionsRequestRequestTypeDef,
+    _OptionalGetQuerySuggestionsRequestRequestTypeDef,
+):
+    pass
+
+
 CustomDocumentEnrichmentConfigurationTypeDef = TypedDict(
     "CustomDocumentEnrichmentConfigurationTypeDef",
     {
         "InlineConfigurations": Sequence[InlineCustomDocumentEnrichmentConfigurationTypeDef],
         "PreExtractionHookConfiguration": HookConfigurationTypeDef,
         "PostExtractionHookConfiguration": HookConfigurationTypeDef,
         "RoleArn": str,
@@ -3565,28 +3894,38 @@
     "BatchGetDocumentStatusRequestRequestTypeDef",
     {
         "IndexId": str,
         "DocumentInfoList": Sequence[DocumentInfoTypeDef],
     },
 )
 
+RetrieveResultTypeDef = TypedDict(
+    "RetrieveResultTypeDef",
+    {
+        "QueryId": str,
+        "ResultItems": List[RetrieveResultItemTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AdditionalResultAttributeTypeDef = TypedDict(
     "AdditionalResultAttributeTypeDef",
     {
         "Key": str,
         "ValueType": Literal["TEXT_WITH_HIGHLIGHTS_VALUE"],
         "Value": AdditionalResultAttributeValueTypeDef,
     },
 )
 
 SuggestionTypeDef = TypedDict(
     "SuggestionTypeDef",
     {
         "Id": str,
         "Value": SuggestionValueTypeDef,
+        "SourceDocuments": List[SourceDocumentTypeDef],
     },
     total=False,
 )
 
 DataSourceConfigurationTypeDef = TypedDict(
     "DataSourceConfigurationTypeDef",
     {
@@ -3631,14 +3970,30 @@
 
 class BatchPutDocumentRequestRequestTypeDef(
     _RequiredBatchPutDocumentRequestRequestTypeDef, _OptionalBatchPutDocumentRequestRequestTypeDef
 ):
     pass
 
 
+FeaturedResultsItemTypeDef = TypedDict(
+    "FeaturedResultsItemTypeDef",
+    {
+        "Id": str,
+        "Type": QueryResultTypeType,
+        "AdditionalAttributes": List[AdditionalResultAttributeTypeDef],
+        "DocumentId": str,
+        "DocumentTitle": TextWithHighlightsTypeDef,
+        "DocumentExcerpt": TextWithHighlightsTypeDef,
+        "DocumentURI": str,
+        "DocumentAttributes": List[DocumentAttributeTypeDef],
+        "FeedbackToken": str,
+    },
+    total=False,
+)
+
 QueryResultItemTypeDef = TypedDict(
     "QueryResultItemTypeDef",
     {
         "Id": str,
         "Type": QueryResultTypeType,
         "Format": QueryResultFormatType,
         "AdditionalAttributes": List[AdditionalResultAttributeTypeDef],
@@ -3655,15 +4010,15 @@
 )
 
 GetQuerySuggestionsResponseTypeDef = TypedDict(
     "GetQuerySuggestionsResponseTypeDef",
     {
         "QuerySuggestionsId": str,
         "Suggestions": List[SuggestionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceRequestRequestTypeDef",
     {
         "Name": str,
@@ -3708,15 +4063,15 @@
         "Description": str,
         "Status": DataSourceStatusType,
         "Schedule": str,
         "RoleArn": str,
         "ErrorMessage": str,
         "LanguageCode": str,
         "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataSourceRequestRequestTypeDef",
     {
         "Id": str,
@@ -3750,10 +4105,11 @@
     {
         "QueryId": str,
         "ResultItems": List[QueryResultItemTypeDef],
         "FacetResults": List["FacetResultTypeDef"],
         "TotalNumberOfResults": int,
         "Warnings": List[WarningTypeDef],
         "SpellCorrectedQueries": List[SpellCorrectedQueryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "FeaturedResultsItems": List[FeaturedResultsItemTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra/type_defs.pyi` & `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AlfrescoEntityType,
+    AttributeSuggestionsModeType,
     ConditionOperatorType,
     ConfluenceAttachmentFieldNameType,
     ConfluenceAuthenticationTypeType,
     ConfluenceBlogFieldNameType,
     ConfluencePageFieldNameType,
     ConfluenceSpaceFieldNameType,
     ConfluenceVersionType,
@@ -34,14 +35,15 @@
     DocumentAttributeValueTypeType,
     DocumentStatusType,
     EntityTypeType,
     ErrorCodeType,
     ExperienceStatusType,
     FaqFileFormatType,
     FaqStatusType,
+    FeaturedResultsSetStatusType,
     HighlightTypeType,
     IndexEditionType,
     IndexStatusType,
     IntervalType,
     IssueSubEntityType,
     KeyLocationType,
     MetricTypeType,
@@ -63,14 +65,15 @@
     ScoreConfidenceType,
     ServiceNowAuthenticationTypeType,
     ServiceNowBuildVersionTypeType,
     SharePointOnlineAuthenticationTypeType,
     SharePointVersionType,
     SlackEntityType,
     SortOrderType,
+    SuggestionTypeType,
     ThesaurusStatusType,
     TypeType,
     UserContextPolicyType,
     UserGroupResolutionModeType,
     WebCrawlerModeType,
 )
 
@@ -88,19 +91,21 @@
     "AccessControlListConfigurationTypeDef",
     "AclConfigurationTypeDef",
     "DataSourceToIndexFieldMappingTypeDef",
     "DataSourceVpcConfigurationTypeDef",
     "S3PathTypeDef",
     "EntityConfigurationTypeDef",
     "FailedEntityTypeDef",
-    "ResponseMetadataTypeDef",
     "EntityPersonaConfigurationTypeDef",
+    "SuggestableConfigTypeDef",
     "BasicAuthenticationConfigurationTypeDef",
     "DataSourceSyncJobMetricTargetTypeDef",
     "BatchDeleteDocumentResponseFailedDocumentTypeDef",
+    "BatchDeleteFeaturedResultsSetErrorTypeDef",
+    "BatchDeleteFeaturedResultsSetRequestRequestTypeDef",
     "BatchGetDocumentStatusResponseErrorTypeDef",
     "StatusTypeDef",
     "BatchPutDocumentResponseFailedDocumentTypeDef",
     "CapacityUnitsConfigurationTypeDef",
     "ClearQuerySuggestionsRequestRequestTypeDef",
     "ClickFeedbackTypeDef",
     "ConfluenceAttachmentToIndexFieldMappingTypeDef",
@@ -108,17 +113,25 @@
     "ProxyConfigurationTypeDef",
     "ConfluencePageToIndexFieldMappingTypeDef",
     "ConfluenceSpaceToIndexFieldMappingTypeDef",
     "ConnectionConfigurationTypeDef",
     "ContentSourceConfigurationTypeDef",
     "CorrectionTypeDef",
     "PrincipalTypeDef",
+    "CreateAccessControlConfigurationResponseTypeDef",
     "TagTypeDef",
+    "CreateDataSourceResponseTypeDef",
+    "CreateExperienceResponseTypeDef",
+    "CreateFaqResponseTypeDef",
+    "FeaturedDocumentTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "UserGroupResolutionConfigurationTypeDef",
+    "CreateIndexResponseTypeDef",
+    "CreateQuerySuggestionsBlockListResponseTypeDef",
+    "CreateThesaurusResponseTypeDef",
     "TemplateConfigurationTypeDef",
     "DataSourceGroupTypeDef",
     "DataSourceSummaryTypeDef",
     "DataSourceSyncJobMetricsTypeDef",
     "SqlConfigurationTypeDef",
     "DeleteAccessControlConfigurationRequestRequestTypeDef",
     "DeleteDataSourceRequestRequestTypeDef",
@@ -129,32 +142,36 @@
     "DeleteQuerySuggestionsBlockListRequestRequestTypeDef",
     "DeleteThesaurusRequestRequestTypeDef",
     "DescribeAccessControlConfigurationRequestRequestTypeDef",
     "DescribeDataSourceRequestRequestTypeDef",
     "DescribeExperienceRequestRequestTypeDef",
     "ExperienceEndpointTypeDef",
     "DescribeFaqRequestRequestTypeDef",
+    "DescribeFeaturedResultsSetRequestRequestTypeDef",
+    "FeaturedDocumentMissingTypeDef",
+    "FeaturedDocumentWithMetadataTypeDef",
     "DescribeIndexRequestRequestTypeDef",
     "DescribePrincipalMappingRequestRequestTypeDef",
     "GroupOrderingIdSummaryTypeDef",
     "DescribeQuerySuggestionsBlockListRequestRequestTypeDef",
     "DescribeQuerySuggestionsConfigRequestRequestTypeDef",
     "DescribeThesaurusRequestRequestTypeDef",
     "DisassociatePersonasFromEntitiesRequestRequestTypeDef",
     "DocumentAttributeValueTypeDef",
     "RelevanceTypeDef",
     "SearchTypeDef",
     "DocumentsMetadataConfigurationTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EntityDisplayDataTypeDef",
     "UserIdentityConfigurationTypeDef",
     "FacetResultTypeDef",
     "FacetTypeDef",
     "FaqStatisticsTypeDef",
     "FaqSummaryTypeDef",
-    "GetQuerySuggestionsRequestRequestTypeDef",
+    "FeaturedResultsSetSummaryTypeDef",
     "GetSnapshotsRequestRequestTypeDef",
     "TimeRangeTypeDef",
     "GitHubDocumentCrawlPropertiesTypeDef",
     "SaaSConfigurationTypeDef",
     "MemberGroupTypeDef",
     "MemberUserTypeDef",
     "GroupSummaryTypeDef",
@@ -166,34 +183,37 @@
     "ListAccessControlConfigurationsRequestRequestTypeDef",
     "ListDataSourcesRequestRequestTypeDef",
     "ListEntityPersonasRequestRequestTypeDef",
     "PersonasSummaryTypeDef",
     "ListExperienceEntitiesRequestRequestTypeDef",
     "ListExperiencesRequestRequestTypeDef",
     "ListFaqsRequestRequestTypeDef",
+    "ListFeaturedResultsSetsRequestRequestTypeDef",
     "ListGroupsOlderThanOrderingIdRequestRequestTypeDef",
     "ListIndicesRequestRequestTypeDef",
     "ListQuerySuggestionsBlockListsRequestRequestTypeDef",
     "QuerySuggestionsBlockListSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListThesauriRequestRequestTypeDef",
     "ThesaurusSummaryTypeDef",
     "SortingConfigurationTypeDef",
     "SpellCorrectionConfigurationTypeDef",
     "ScoreAttributesTypeDef",
     "WarningTypeDef",
     "RelevanceFeedbackTypeDef",
+    "ResponseMetadataTypeDef",
     "SeedUrlConfigurationTypeDef",
     "SiteMapsConfigurationTypeDef",
     "StartDataSourceSyncJobRequestRequestTypeDef",
+    "StartDataSourceSyncJobResponseTypeDef",
     "StopDataSourceSyncJobRequestRequestTypeDef",
     "SuggestionHighlightTypeDef",
     "TableCellTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateQuerySuggestionsConfigRequestRequestTypeDef",
+    "ListAccessControlConfigurationsResponseTypeDef",
     "ColumnConfigurationTypeDef",
     "GoogleDriveConfigurationTypeDef",
     "SalesforceChatterFeedConfigurationTypeDef",
     "SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef",
     "SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef",
     "SalesforceStandardObjectAttachmentConfigurationTypeDef",
     "SalesforceStandardObjectConfigurationTypeDef",
@@ -202,71 +222,68 @@
     "WorkDocsConfigurationTypeDef",
     "BoxConfigurationTypeDef",
     "FsxConfigurationTypeDef",
     "JiraConfigurationTypeDef",
     "QuipConfigurationTypeDef",
     "SlackConfigurationTypeDef",
     "AlfrescoConfigurationTypeDef",
+    "DescribeFaqResponseTypeDef",
+    "DescribeQuerySuggestionsBlockListResponseTypeDef",
+    "DescribeThesaurusResponseTypeDef",
     "OnPremiseConfigurationTypeDef",
     "OneDriveUsersTypeDef",
     "UpdateQuerySuggestionsBlockListRequestRequestTypeDef",
     "UpdateThesaurusRequestRequestTypeDef",
     "AssociateEntitiesToExperienceRequestRequestTypeDef",
     "DisassociateEntitiesFromExperienceRequestRequestTypeDef",
     "AssociateEntitiesToExperienceResponseTypeDef",
     "AssociatePersonasToEntitiesResponseTypeDef",
-    "CreateAccessControlConfigurationResponseTypeDef",
-    "CreateDataSourceResponseTypeDef",
-    "CreateExperienceResponseTypeDef",
-    "CreateFaqResponseTypeDef",
-    "CreateIndexResponseTypeDef",
-    "CreateQuerySuggestionsBlockListResponseTypeDef",
-    "CreateThesaurusResponseTypeDef",
-    "DescribeFaqResponseTypeDef",
-    "DescribeQuerySuggestionsBlockListResponseTypeDef",
-    "DescribeQuerySuggestionsConfigResponseTypeDef",
-    "DescribeThesaurusResponseTypeDef",
     "DisassociateEntitiesFromExperienceResponseTypeDef",
     "DisassociatePersonasFromEntitiesResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListAccessControlConfigurationsResponseTypeDef",
-    "StartDataSourceSyncJobResponseTypeDef",
     "AssociatePersonasToEntitiesRequestRequestTypeDef",
+    "AttributeSuggestionsDescribeConfigTypeDef",
+    "AttributeSuggestionsUpdateConfigTypeDef",
     "AuthenticationConfigurationTypeDef",
     "BatchDeleteDocumentRequestRequestTypeDef",
     "BatchDeleteDocumentResponseTypeDef",
+    "BatchDeleteFeaturedResultsSetResponseTypeDef",
     "BatchGetDocumentStatusResponseTypeDef",
     "BatchPutDocumentResponseTypeDef",
     "ConfluenceAttachmentConfigurationTypeDef",
     "ConfluenceBlogConfigurationTypeDef",
     "SharePointConfigurationTypeDef",
     "ConfluencePageConfigurationTypeDef",
     "ConfluenceSpaceConfigurationTypeDef",
     "SpellCorrectedQueryTypeDef",
     "HierarchicalPrincipalTypeDef",
     "CreateFaqRequestRequestTypeDef",
     "CreateQuerySuggestionsBlockListRequestRequestTypeDef",
     "CreateThesaurusRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateFeaturedResultsSetRequestRequestTypeDef",
+    "FeaturedResultsSetTypeDef",
+    "UpdateFeaturedResultsSetRequestRequestTypeDef",
     "UserContextTypeDef",
     "ListDataSourcesResponseTypeDef",
     "DataSourceSyncJobTypeDef",
     "ExperiencesSummaryTypeDef",
+    "DescribeFeaturedResultsSetResponseTypeDef",
     "DescribePrincipalMappingResponseTypeDef",
     "DocumentAttributeConditionTypeDef",
     "DocumentAttributeTargetTypeDef",
     "DocumentAttributeTypeDef",
     "DocumentAttributeValueCountPairTypeDef",
     "DocumentRelevanceConfigurationTypeDef",
     "DocumentMetadataConfigurationTypeDef",
     "S3DataSourceConfigurationTypeDef",
     "ExperienceEntitiesSummaryTypeDef",
     "ExperienceConfigurationTypeDef",
     "ListFaqsResponseTypeDef",
+    "ListFeaturedResultsSetsResponseTypeDef",
     "GetSnapshotsResponseTypeDef",
     "ListDataSourceSyncJobsRequestRequestTypeDef",
     "GroupMembersTypeDef",
     "ListGroupsOlderThanOrderingIdResponseTypeDef",
     "TextWithHighlightsTypeDef",
     "ListIndicesResponseTypeDef",
     "IndexStatisticsTypeDef",
@@ -279,45 +296,56 @@
     "SuggestionTextWithHighlightsTypeDef",
     "TableRowTypeDef",
     "DatabaseConfigurationTypeDef",
     "SalesforceKnowledgeArticleConfigurationTypeDef",
     "ServiceNowConfigurationTypeDef",
     "GitHubConfigurationTypeDef",
     "OneDriveConfigurationTypeDef",
+    "DescribeQuerySuggestionsConfigResponseTypeDef",
+    "UpdateQuerySuggestionsConfigRequestRequestTypeDef",
     "ConfluenceConfigurationTypeDef",
     "CreateAccessControlConfigurationRequestRequestTypeDef",
     "DescribeAccessControlConfigurationResponseTypeDef",
     "UpdateAccessControlConfigurationRequestRequestTypeDef",
+    "CreateFeaturedResultsSetResponseTypeDef",
+    "UpdateFeaturedResultsSetResponseTypeDef",
+    "AttributeSuggestionsGetConfigTypeDef",
     "ListDataSourceSyncJobsResponseTypeDef",
     "ListExperiencesResponseTypeDef",
     "HookConfigurationTypeDef",
     "InlineCustomDocumentEnrichmentConfigurationTypeDef",
     "AttributeFilterTypeDef",
     "DocumentInfoTypeDef",
     "DocumentTypeDef",
+    "RetrieveResultItemTypeDef",
+    "SourceDocumentTypeDef",
     "QueryRequestRequestTypeDef",
+    "RetrieveRequestRequestTypeDef",
     "ListExperienceEntitiesResponseTypeDef",
     "CreateExperienceRequestRequestTypeDef",
     "DescribeExperienceResponseTypeDef",
     "UpdateExperienceRequestRequestTypeDef",
     "PutPrincipalMappingRequestRequestTypeDef",
     "AdditionalResultAttributeValueTypeDef",
     "CreateIndexRequestRequestTypeDef",
     "DescribeIndexResponseTypeDef",
     "UpdateIndexRequestRequestTypeDef",
     "WebCrawlerConfigurationTypeDef",
     "SuggestionValueTypeDef",
     "TableExcerptTypeDef",
     "SalesforceConfigurationTypeDef",
+    "GetQuerySuggestionsRequestRequestTypeDef",
     "CustomDocumentEnrichmentConfigurationTypeDef",
     "BatchGetDocumentStatusRequestRequestTypeDef",
+    "RetrieveResultTypeDef",
     "AdditionalResultAttributeTypeDef",
     "SuggestionTypeDef",
     "DataSourceConfigurationTypeDef",
     "BatchPutDocumentRequestRequestTypeDef",
+    "FeaturedResultsItemTypeDef",
     "QueryResultItemTypeDef",
     "GetQuerySuggestionsResponseTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
     "DescribeDataSourceResponseTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
     "QueryResultTypeDef",
 )
@@ -393,33 +421,31 @@
     {
         "EntityId": str,
         "ErrorMessage": str,
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
 EntityPersonaConfigurationTypeDef = TypedDict(
     "EntityPersonaConfigurationTypeDef",
     {
         "EntityId": str,
         "Persona": PersonaType,
     },
 )
 
+SuggestableConfigTypeDef = TypedDict(
+    "SuggestableConfigTypeDef",
+    {
+        "AttributeName": str,
+        "Suggestable": bool,
+    },
+    total=False,
+)
+
 BasicAuthenticationConfigurationTypeDef = TypedDict(
     "BasicAuthenticationConfigurationTypeDef",
     {
         "Host": str,
         "Port": int,
         "Credentials": str,
     },
@@ -450,14 +476,31 @@
         "Id": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+BatchDeleteFeaturedResultsSetErrorTypeDef = TypedDict(
+    "BatchDeleteFeaturedResultsSetErrorTypeDef",
+    {
+        "Id": str,
+        "ErrorCode": ErrorCodeType,
+        "ErrorMessage": str,
+    },
+)
+
+BatchDeleteFeaturedResultsSetRequestRequestTypeDef = TypedDict(
+    "BatchDeleteFeaturedResultsSetRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "FeaturedResultsSetIds": Sequence[str],
+    },
+)
+
 BatchGetDocumentStatusResponseErrorTypeDef = TypedDict(
     "BatchGetDocumentStatusResponseErrorTypeDef",
     {
         "DocumentId": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
@@ -615,22 +658,62 @@
     },
     total=False,
 )
 
 class PrincipalTypeDef(_RequiredPrincipalTypeDef, _OptionalPrincipalTypeDef):
     pass
 
+CreateAccessControlConfigurationResponseTypeDef = TypedDict(
+    "CreateAccessControlConfigurationResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+CreateDataSourceResponseTypeDef = TypedDict(
+    "CreateDataSourceResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateExperienceResponseTypeDef = TypedDict(
+    "CreateExperienceResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateFaqResponseTypeDef = TypedDict(
+    "CreateFaqResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+FeaturedDocumentTypeDef = TypedDict(
+    "FeaturedDocumentTypeDef",
+    {
+        "Id": str,
+    },
+    total=False,
+)
+
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
@@ -638,14 +721,38 @@
 UserGroupResolutionConfigurationTypeDef = TypedDict(
     "UserGroupResolutionConfigurationTypeDef",
     {
         "UserGroupResolutionMode": UserGroupResolutionModeType,
     },
 )
 
+CreateIndexResponseTypeDef = TypedDict(
+    "CreateIndexResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateQuerySuggestionsBlockListResponseTypeDef = TypedDict(
+    "CreateQuerySuggestionsBlockListResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateThesaurusResponseTypeDef = TypedDict(
+    "CreateThesaurusResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TemplateConfigurationTypeDef = TypedDict(
     "TemplateConfigurationTypeDef",
     {
         "Template": Mapping[str, Any],
     },
     total=False,
 )
@@ -806,14 +913,40 @@
     "DescribeFaqRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
 
+DescribeFeaturedResultsSetRequestRequestTypeDef = TypedDict(
+    "DescribeFeaturedResultsSetRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "FeaturedResultsSetId": str,
+    },
+)
+
+FeaturedDocumentMissingTypeDef = TypedDict(
+    "FeaturedDocumentMissingTypeDef",
+    {
+        "Id": str,
+    },
+    total=False,
+)
+
+FeaturedDocumentWithMetadataTypeDef = TypedDict(
+    "FeaturedDocumentWithMetadataTypeDef",
+    {
+        "Id": str,
+        "Title": str,
+        "URI": str,
+    },
+    total=False,
+)
+
 DescribeIndexRequestRequestTypeDef = TypedDict(
     "DescribeIndexRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -920,14 +1053,21 @@
     "DocumentsMetadataConfigurationTypeDef",
     {
         "S3Prefix": str,
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
 EntityDisplayDataTypeDef = TypedDict(
     "EntityDisplayDataTypeDef",
     {
         "UserName": str,
         "GroupName": str,
         "IdentifiedUserName": str,
         "FirstName": str,
@@ -981,35 +1121,26 @@
         "UpdatedAt": datetime,
         "FileFormat": FaqFileFormatType,
         "LanguageCode": str,
     },
     total=False,
 )
 
-_RequiredGetQuerySuggestionsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetQuerySuggestionsRequestRequestTypeDef",
-    {
-        "IndexId": str,
-        "QueryText": str,
-    },
-)
-_OptionalGetQuerySuggestionsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetQuerySuggestionsRequestRequestTypeDef",
+FeaturedResultsSetSummaryTypeDef = TypedDict(
+    "FeaturedResultsSetSummaryTypeDef",
     {
-        "MaxSuggestionsCount": int,
+        "FeaturedResultsSetId": str,
+        "FeaturedResultsSetName": str,
+        "Status": FeaturedResultsSetStatusType,
+        "LastUpdatedTimestamp": int,
+        "CreationTimestamp": int,
     },
     total=False,
 )
 
-class GetQuerySuggestionsRequestRequestTypeDef(
-    _RequiredGetQuerySuggestionsRequestRequestTypeDef,
-    _OptionalGetQuerySuggestionsRequestRequestTypeDef,
-):
-    pass
-
 _RequiredGetSnapshotsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSnapshotsRequestRequestTypeDef",
     {
         "IndexId": str,
         "Interval": IntervalType,
         "MetricType": MetricTypeType,
     },
@@ -1305,14 +1436,35 @@
 )
 
 class ListFaqsRequestRequestTypeDef(
     _RequiredListFaqsRequestRequestTypeDef, _OptionalListFaqsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListFeaturedResultsSetsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFeaturedResultsSetsRequestRequestTypeDef",
+    {
+        "IndexId": str,
+    },
+)
+_OptionalListFeaturedResultsSetsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFeaturedResultsSetsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListFeaturedResultsSetsRequestRequestTypeDef(
+    _RequiredListFeaturedResultsSetsRequestRequestTypeDef,
+    _OptionalListFeaturedResultsSetsRequestRequestTypeDef,
+):
+    pass
+
 _RequiredListGroupsOlderThanOrderingIdRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsOlderThanOrderingIdRequestRequestTypeDef",
     {
         "IndexId": str,
         "OrderingId": int,
     },
 )
@@ -1450,14 +1602,25 @@
     "RelevanceFeedbackTypeDef",
     {
         "ResultId": str,
         "RelevanceValue": RelevanceTypeType,
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
 _RequiredSeedUrlConfigurationTypeDef = TypedDict(
     "_RequiredSeedUrlConfigurationTypeDef",
     {
         "SeedUrls": Sequence[str],
     },
 )
 _OptionalSeedUrlConfigurationTypeDef = TypedDict(
@@ -1484,14 +1647,22 @@
     "StartDataSourceSyncJobRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
 
+StartDataSourceSyncJobResponseTypeDef = TypedDict(
+    "StartDataSourceSyncJobResponseTypeDef",
+    {
+        "ExecutionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopDataSourceSyncJobRequestRequestTypeDef = TypedDict(
     "StopDataSourceSyncJobRequestRequestTypeDef",
     {
         "Id": str,
         "IndexId": str,
     },
 )
@@ -1520,38 +1691,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-_RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef",
-    {
-        "IndexId": str,
-    },
-)
-_OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef",
+ListAccessControlConfigurationsResponseTypeDef = TypedDict(
+    "ListAccessControlConfigurationsResponseTypeDef",
     {
-        "Mode": ModeType,
-        "QueryLogLookBackWindowInDays": int,
-        "IncludeQueriesWithoutUserInformation": bool,
-        "MinimumNumberOfQueryingUsers": int,
-        "MinimumQueryCount": int,
+        "NextToken": str,
+        "AccessControlConfigurations": List[AccessControlConfigurationSummaryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class UpdateQuerySuggestionsConfigRequestRequestTypeDef(
-    _RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef,
-    _OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef,
-):
-    pass
-
 _RequiredColumnConfigurationTypeDef = TypedDict(
     "_RequiredColumnConfigurationTypeDef",
     {
         "DocumentIdColumnName": str,
         "DocumentDataColumnName": str,
         "ChangeDetectingColumns": Sequence[str],
     },
@@ -1930,14 +2086,72 @@
 )
 
 class AlfrescoConfigurationTypeDef(
     _RequiredAlfrescoConfigurationTypeDef, _OptionalAlfrescoConfigurationTypeDef
 ):
     pass
 
+DescribeFaqResponseTypeDef = TypedDict(
+    "DescribeFaqResponseTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+        "Name": str,
+        "Description": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "S3Path": S3PathTypeDef,
+        "Status": FaqStatusType,
+        "RoleArn": str,
+        "ErrorMessage": str,
+        "FileFormat": FaqFileFormatType,
+        "LanguageCode": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeQuerySuggestionsBlockListResponseTypeDef = TypedDict(
+    "DescribeQuerySuggestionsBlockListResponseTypeDef",
+    {
+        "IndexId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "Status": QuerySuggestionsBlockListStatusType,
+        "ErrorMessage": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "SourceS3Path": S3PathTypeDef,
+        "ItemCount": int,
+        "FileSizeBytes": int,
+        "RoleArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeThesaurusResponseTypeDef = TypedDict(
+    "DescribeThesaurusResponseTypeDef",
+    {
+        "Id": str,
+        "IndexId": str,
+        "Name": str,
+        "Description": str,
+        "Status": ThesaurusStatusType,
+        "ErrorMessage": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "RoleArn": str,
+        "SourceS3Path": S3PathTypeDef,
+        "FileSizeBytes": int,
+        "TermCount": int,
+        "SynonymRuleCount": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 OnPremiseConfigurationTypeDef = TypedDict(
     "OnPremiseConfigurationTypeDef",
     {
         "HostUrl": str,
         "OrganizationName": str,
         "SslCertificateS3Path": S3PathTypeDef,
     },
@@ -2017,203 +2231,67 @@
     },
 )
 
 AssociateEntitiesToExperienceResponseTypeDef = TypedDict(
     "AssociateEntitiesToExperienceResponseTypeDef",
     {
         "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociatePersonasToEntitiesResponseTypeDef = TypedDict(
     "AssociatePersonasToEntitiesResponseTypeDef",
     {
         "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAccessControlConfigurationResponseTypeDef = TypedDict(
-    "CreateAccessControlConfigurationResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDataSourceResponseTypeDef = TypedDict(
-    "CreateDataSourceResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateExperienceResponseTypeDef = TypedDict(
-    "CreateExperienceResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateFaqResponseTypeDef = TypedDict(
-    "CreateFaqResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIndexResponseTypeDef = TypedDict(
-    "CreateIndexResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateQuerySuggestionsBlockListResponseTypeDef = TypedDict(
-    "CreateQuerySuggestionsBlockListResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateThesaurusResponseTypeDef = TypedDict(
-    "CreateThesaurusResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFaqResponseTypeDef = TypedDict(
-    "DescribeFaqResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Description": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "S3Path": S3PathTypeDef,
-        "Status": FaqStatusType,
-        "RoleArn": str,
-        "ErrorMessage": str,
-        "FileFormat": FaqFileFormatType,
-        "LanguageCode": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeQuerySuggestionsBlockListResponseTypeDef = TypedDict(
-    "DescribeQuerySuggestionsBlockListResponseTypeDef",
-    {
-        "IndexId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "Status": QuerySuggestionsBlockListStatusType,
-        "ErrorMessage": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "SourceS3Path": S3PathTypeDef,
-        "ItemCount": int,
-        "FileSizeBytes": int,
-        "RoleArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeQuerySuggestionsConfigResponseTypeDef = TypedDict(
-    "DescribeQuerySuggestionsConfigResponseTypeDef",
-    {
-        "Mode": ModeType,
-        "Status": QuerySuggestionsStatusType,
-        "QueryLogLookBackWindowInDays": int,
-        "IncludeQueriesWithoutUserInformation": bool,
-        "MinimumNumberOfQueryingUsers": int,
-        "MinimumQueryCount": int,
-        "LastSuggestionsBuildTime": datetime,
-        "LastClearTime": datetime,
-        "TotalSuggestionsCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeThesaurusResponseTypeDef = TypedDict(
-    "DescribeThesaurusResponseTypeDef",
-    {
-        "Id": str,
-        "IndexId": str,
-        "Name": str,
-        "Description": str,
-        "Status": ThesaurusStatusType,
-        "ErrorMessage": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "RoleArn": str,
-        "SourceS3Path": S3PathTypeDef,
-        "FileSizeBytes": int,
-        "TermCount": int,
-        "SynonymRuleCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociateEntitiesFromExperienceResponseTypeDef = TypedDict(
     "DisassociateEntitiesFromExperienceResponseTypeDef",
     {
         "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DisassociatePersonasFromEntitiesResponseTypeDef = TypedDict(
     "DisassociatePersonasFromEntitiesResponseTypeDef",
     {
         "FailedEntityList": List[FailedEntityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListAccessControlConfigurationsResponseTypeDef = TypedDict(
-    "ListAccessControlConfigurationsResponseTypeDef",
+AssociatePersonasToEntitiesRequestRequestTypeDef = TypedDict(
+    "AssociatePersonasToEntitiesRequestRequestTypeDef",
     {
-        "NextToken": str,
-        "AccessControlConfigurations": List[AccessControlConfigurationSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Id": str,
+        "IndexId": str,
+        "Personas": Sequence[EntityPersonaConfigurationTypeDef],
     },
 )
 
-StartDataSourceSyncJobResponseTypeDef = TypedDict(
-    "StartDataSourceSyncJobResponseTypeDef",
+AttributeSuggestionsDescribeConfigTypeDef = TypedDict(
+    "AttributeSuggestionsDescribeConfigTypeDef",
     {
-        "ExecutionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SuggestableConfigList": List[SuggestableConfigTypeDef],
+        "AttributeSuggestionsMode": AttributeSuggestionsModeType,
     },
+    total=False,
 )
 
-AssociatePersonasToEntitiesRequestRequestTypeDef = TypedDict(
-    "AssociatePersonasToEntitiesRequestRequestTypeDef",
+AttributeSuggestionsUpdateConfigTypeDef = TypedDict(
+    "AttributeSuggestionsUpdateConfigTypeDef",
     {
-        "Id": str,
-        "IndexId": str,
-        "Personas": Sequence[EntityPersonaConfigurationTypeDef],
+        "SuggestableConfigList": Sequence[SuggestableConfigTypeDef],
+        "AttributeSuggestionsMode": AttributeSuggestionsModeType,
     },
+    total=False,
 )
 
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
         "BasicAuthentication": Sequence[BasicAuthenticationConfigurationTypeDef],
     },
@@ -2241,32 +2319,40 @@
 ):
     pass
 
 BatchDeleteDocumentResponseTypeDef = TypedDict(
     "BatchDeleteDocumentResponseTypeDef",
     {
         "FailedDocuments": List[BatchDeleteDocumentResponseFailedDocumentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchDeleteFeaturedResultsSetResponseTypeDef = TypedDict(
+    "BatchDeleteFeaturedResultsSetResponseTypeDef",
+    {
+        "Errors": List[BatchDeleteFeaturedResultsSetErrorTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetDocumentStatusResponseTypeDef = TypedDict(
     "BatchGetDocumentStatusResponseTypeDef",
     {
         "Errors": List[BatchGetDocumentStatusResponseErrorTypeDef],
         "DocumentStatusList": List[StatusTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchPutDocumentResponseTypeDef = TypedDict(
     "BatchPutDocumentResponseTypeDef",
     {
         "FailedDocuments": List[BatchPutDocumentResponseFailedDocumentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfluenceAttachmentConfigurationTypeDef = TypedDict(
     "ConfluenceAttachmentConfigurationTypeDef",
     {
         "CrawlAttachments": bool,
@@ -2425,26 +2511,92 @@
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
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredCreateFeaturedResultsSetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFeaturedResultsSetRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "FeaturedResultsSetName": str,
+    },
+)
+_OptionalCreateFeaturedResultsSetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFeaturedResultsSetRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ClientToken": str,
+        "Status": FeaturedResultsSetStatusType,
+        "QueryTexts": Sequence[str],
+        "FeaturedDocuments": Sequence[FeaturedDocumentTypeDef],
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateFeaturedResultsSetRequestRequestTypeDef(
+    _RequiredCreateFeaturedResultsSetRequestRequestTypeDef,
+    _OptionalCreateFeaturedResultsSetRequestRequestTypeDef,
+):
+    pass
+
+FeaturedResultsSetTypeDef = TypedDict(
+    "FeaturedResultsSetTypeDef",
+    {
+        "FeaturedResultsSetId": str,
+        "FeaturedResultsSetName": str,
+        "Description": str,
+        "Status": FeaturedResultsSetStatusType,
+        "QueryTexts": List[str],
+        "FeaturedDocuments": List[FeaturedDocumentTypeDef],
+        "LastUpdatedTimestamp": int,
+        "CreationTimestamp": int,
+    },
+    total=False,
+)
+
+_RequiredUpdateFeaturedResultsSetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFeaturedResultsSetRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "FeaturedResultsSetId": str,
+    },
+)
+_OptionalUpdateFeaturedResultsSetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFeaturedResultsSetRequestRequestTypeDef",
+    {
+        "FeaturedResultsSetName": str,
+        "Description": str,
+        "Status": FeaturedResultsSetStatusType,
+        "QueryTexts": Sequence[str],
+        "FeaturedDocuments": Sequence[FeaturedDocumentTypeDef],
+    },
+    total=False,
+)
+
+class UpdateFeaturedResultsSetRequestRequestTypeDef(
+    _RequiredUpdateFeaturedResultsSetRequestRequestTypeDef,
+    _OptionalUpdateFeaturedResultsSetRequestRequestTypeDef,
+):
+    pass
+
 UserContextTypeDef = TypedDict(
     "UserContextTypeDef",
     {
         "Token": str,
         "UserId": str,
         "Groups": Sequence[str],
         "DataSourceGroups": Sequence[DataSourceGroupTypeDef],
@@ -2453,15 +2605,15 @@
 )
 
 ListDataSourcesResponseTypeDef = TypedDict(
     "ListDataSourcesResponseTypeDef",
     {
         "SummaryItems": List[DataSourceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DataSourceSyncJobTypeDef = TypedDict(
     "DataSourceSyncJobTypeDef",
     {
         "ExecutionId": str,
@@ -2484,22 +2636,38 @@
         "CreatedAt": datetime,
         "Status": ExperienceStatusType,
         "Endpoints": List[ExperienceEndpointTypeDef],
     },
     total=False,
 )
 
+DescribeFeaturedResultsSetResponseTypeDef = TypedDict(
+    "DescribeFeaturedResultsSetResponseTypeDef",
+    {
+        "FeaturedResultsSetId": str,
+        "FeaturedResultsSetName": str,
+        "Description": str,
+        "Status": FeaturedResultsSetStatusType,
+        "QueryTexts": List[str],
+        "FeaturedDocumentsWithMetadata": List[FeaturedDocumentWithMetadataTypeDef],
+        "FeaturedDocumentsMissing": List[FeaturedDocumentMissingTypeDef],
+        "LastUpdatedTimestamp": int,
+        "CreationTimestamp": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribePrincipalMappingResponseTypeDef = TypedDict(
     "DescribePrincipalMappingResponseTypeDef",
     {
         "IndexId": str,
         "DataSourceId": str,
         "GroupId": str,
         "GroupOrderingIdSummaries": List[GroupOrderingIdSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDocumentAttributeConditionTypeDef = TypedDict(
     "_RequiredDocumentAttributeConditionTypeDef",
     {
         "ConditionDocumentAttributeKey": str,
@@ -2619,26 +2787,35 @@
 )
 
 ListFaqsResponseTypeDef = TypedDict(
     "ListFaqsResponseTypeDef",
     {
         "NextToken": str,
         "FaqSummaryItems": List[FaqSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListFeaturedResultsSetsResponseTypeDef = TypedDict(
+    "ListFeaturedResultsSetsResponseTypeDef",
+    {
+        "FeaturedResultsSetSummaryItems": List[FeaturedResultsSetSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSnapshotsResponseTypeDef = TypedDict(
     "GetSnapshotsResponseTypeDef",
     {
         "SnapShotTimeFilter": TimeRangeTypeDef,
         "SnapshotsDataHeader": List[str],
         "SnapshotsData": List[List[str]],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListDataSourceSyncJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSourceSyncJobsRequestRequestTypeDef",
     {
         "Id": str,
@@ -2673,15 +2850,15 @@
 )
 
 ListGroupsOlderThanOrderingIdResponseTypeDef = TypedDict(
     "ListGroupsOlderThanOrderingIdResponseTypeDef",
     {
         "GroupsSummaries": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TextWithHighlightsTypeDef = TypedDict(
     "TextWithHighlightsTypeDef",
     {
         "Text": str,
@@ -2691,15 +2868,15 @@
 )
 
 ListIndicesResponseTypeDef = TypedDict(
     "ListIndicesResponseTypeDef",
     {
         "IndexConfigurationSummaryItems": List[IndexConfigurationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IndexStatisticsTypeDef = TypedDict(
     "IndexStatisticsTypeDef",
     {
         "FaqStatistics": FaqStatisticsTypeDef,
@@ -2717,33 +2894,33 @@
 )
 
 ListEntityPersonasResponseTypeDef = TypedDict(
     "ListEntityPersonasResponseTypeDef",
     {
         "SummaryItems": List[PersonasSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListQuerySuggestionsBlockListsResponseTypeDef = TypedDict(
     "ListQuerySuggestionsBlockListsResponseTypeDef",
     {
         "BlockListSummaryItems": List[QuerySuggestionsBlockListSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListThesauriResponseTypeDef = TypedDict(
     "ListThesauriResponseTypeDef",
     {
         "NextToken": str,
         "ThesaurusSummaryItems": List[ThesaurusSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSubmitFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitFeedbackRequestRequestTypeDef",
     {
         "IndexId": str,
@@ -2818,15 +2995,17 @@
     {
         "IncludedStates": Sequence[SalesforceKnowledgeArticleStateType],
     },
 )
 _OptionalSalesforceKnowledgeArticleConfigurationTypeDef = TypedDict(
     "_OptionalSalesforceKnowledgeArticleConfigurationTypeDef",
     {
-        "StandardKnowledgeArticleTypeConfiguration": SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
+        "StandardKnowledgeArticleTypeConfiguration": (
+            SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef
+        ),
         "CustomKnowledgeArticleTypeConfigurations": Sequence[
             SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef
         ],
     },
     total=False,
 )
 
@@ -2932,14 +3111,56 @@
 )
 
 class OneDriveConfigurationTypeDef(
     _RequiredOneDriveConfigurationTypeDef, _OptionalOneDriveConfigurationTypeDef
 ):
     pass
 
+DescribeQuerySuggestionsConfigResponseTypeDef = TypedDict(
+    "DescribeQuerySuggestionsConfigResponseTypeDef",
+    {
+        "Mode": ModeType,
+        "Status": QuerySuggestionsStatusType,
+        "QueryLogLookBackWindowInDays": int,
+        "IncludeQueriesWithoutUserInformation": bool,
+        "MinimumNumberOfQueryingUsers": int,
+        "MinimumQueryCount": int,
+        "LastSuggestionsBuildTime": datetime,
+        "LastClearTime": datetime,
+        "TotalSuggestionsCount": int,
+        "AttributeSuggestionsConfig": AttributeSuggestionsDescribeConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef",
+    {
+        "IndexId": str,
+    },
+)
+_OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef",
+    {
+        "Mode": ModeType,
+        "QueryLogLookBackWindowInDays": int,
+        "IncludeQueriesWithoutUserInformation": bool,
+        "MinimumNumberOfQueryingUsers": int,
+        "MinimumQueryCount": int,
+        "AttributeSuggestionsConfig": AttributeSuggestionsUpdateConfigTypeDef,
+    },
+    total=False,
+)
+
+class UpdateQuerySuggestionsConfigRequestRequestTypeDef(
+    _RequiredUpdateQuerySuggestionsConfigRequestRequestTypeDef,
+    _OptionalUpdateQuerySuggestionsConfigRequestRequestTypeDef,
+):
+    pass
+
 _RequiredConfluenceConfigurationTypeDef = TypedDict(
     "_RequiredConfluenceConfigurationTypeDef",
     {
         "ServerUrl": str,
         "SecretArn": str,
         "Version": ConfluenceVersionType,
     },
@@ -2993,15 +3214,15 @@
     "DescribeAccessControlConfigurationResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "ErrorMessage": str,
         "AccessControlList": List[PrincipalTypeDef],
         "HierarchicalAccessControlList": List[HierarchicalPrincipalTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAccessControlConfigurationRequestRequestTypeDef",
     {
         "IndexId": str,
@@ -3021,29 +3242,56 @@
 
 class UpdateAccessControlConfigurationRequestRequestTypeDef(
     _RequiredUpdateAccessControlConfigurationRequestRequestTypeDef,
     _OptionalUpdateAccessControlConfigurationRequestRequestTypeDef,
 ):
     pass
 
+CreateFeaturedResultsSetResponseTypeDef = TypedDict(
+    "CreateFeaturedResultsSetResponseTypeDef",
+    {
+        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateFeaturedResultsSetResponseTypeDef = TypedDict(
+    "UpdateFeaturedResultsSetResponseTypeDef",
+    {
+        "FeaturedResultsSet": FeaturedResultsSetTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+AttributeSuggestionsGetConfigTypeDef = TypedDict(
+    "AttributeSuggestionsGetConfigTypeDef",
+    {
+        "SuggestionAttributes": Sequence[str],
+        "AdditionalResponseAttributes": Sequence[str],
+        "AttributeFilter": "AttributeFilterTypeDef",
+        "UserContext": UserContextTypeDef,
+    },
+    total=False,
+)
+
 ListDataSourceSyncJobsResponseTypeDef = TypedDict(
     "ListDataSourceSyncJobsResponseTypeDef",
     {
         "History": List[DataSourceSyncJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListExperiencesResponseTypeDef = TypedDict(
     "ListExperiencesResponseTypeDef",
     {
         "SummaryItems": List[ExperiencesSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredHookConfigurationTypeDef = TypedDict(
     "_RequiredHookConfigurationTypeDef",
     {
         "LambdaArn": str,
@@ -3127,14 +3375,37 @@
     },
     total=False,
 )
 
 class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
     pass
 
+RetrieveResultItemTypeDef = TypedDict(
+    "RetrieveResultItemTypeDef",
+    {
+        "Id": str,
+        "DocumentId": str,
+        "DocumentTitle": str,
+        "Content": str,
+        "DocumentURI": str,
+        "DocumentAttributes": List[DocumentAttributeTypeDef],
+    },
+    total=False,
+)
+
+SourceDocumentTypeDef = TypedDict(
+    "SourceDocumentTypeDef",
+    {
+        "DocumentId": str,
+        "SuggestionAttributes": List[str],
+        "AdditionalAttributes": List[DocumentAttributeTypeDef],
+    },
+    total=False,
+)
+
 _RequiredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredQueryRequestRequestTypeDef",
     {
         "IndexId": str,
     },
 )
 _OptionalQueryRequestRequestTypeDef = TypedDict(
@@ -3157,20 +3428,45 @@
 )
 
 class QueryRequestRequestTypeDef(
     _RequiredQueryRequestRequestTypeDef, _OptionalQueryRequestRequestTypeDef
 ):
     pass
 
+_RequiredRetrieveRequestRequestTypeDef = TypedDict(
+    "_RequiredRetrieveRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "QueryText": str,
+    },
+)
+_OptionalRetrieveRequestRequestTypeDef = TypedDict(
+    "_OptionalRetrieveRequestRequestTypeDef",
+    {
+        "AttributeFilter": "AttributeFilterTypeDef",
+        "RequestedDocumentAttributes": Sequence[str],
+        "DocumentRelevanceOverrideConfigurations": Sequence[DocumentRelevanceConfigurationTypeDef],
+        "PageNumber": int,
+        "PageSize": int,
+        "UserContext": UserContextTypeDef,
+    },
+    total=False,
+)
+
+class RetrieveRequestRequestTypeDef(
+    _RequiredRetrieveRequestRequestTypeDef, _OptionalRetrieveRequestRequestTypeDef
+):
+    pass
+
 ListExperienceEntitiesResponseTypeDef = TypedDict(
     "ListExperienceEntitiesResponseTypeDef",
     {
         "SummaryItems": List[ExperienceEntitiesSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperienceRequestRequestTypeDef",
     {
         "Name": str,
@@ -3203,15 +3499,15 @@
         "Configuration": ExperienceConfigurationTypeDef,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "Description": str,
         "Status": ExperienceStatusType,
         "RoleArn": str,
         "ErrorMessage": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateExperienceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExperienceRequestRequestTypeDef",
     {
         "Id": str,
@@ -3308,15 +3604,15 @@
         "DocumentMetadataConfigurations": List[DocumentMetadataConfigurationTypeDef],
         "IndexStatistics": IndexStatisticsTypeDef,
         "ErrorMessage": str,
         "CapacityUnits": CapacityUnitsConfigurationTypeDef,
         "UserTokenConfigurations": List[UserTokenConfigurationTypeDef],
         "UserContextPolicy": UserContextPolicyType,
         "UserGroupResolutionConfiguration": UserGroupResolutionConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateIndexRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIndexRequestRequestTypeDef",
     {
         "Id": str,
@@ -3395,26 +3691,51 @@
 _OptionalSalesforceConfigurationTypeDef = TypedDict(
     "_OptionalSalesforceConfigurationTypeDef",
     {
         "StandardObjectConfigurations": Sequence[SalesforceStandardObjectConfigurationTypeDef],
         "KnowledgeArticleConfiguration": SalesforceKnowledgeArticleConfigurationTypeDef,
         "ChatterFeedConfiguration": SalesforceChatterFeedConfigurationTypeDef,
         "CrawlAttachments": bool,
-        "StandardObjectAttachmentConfiguration": SalesforceStandardObjectAttachmentConfigurationTypeDef,
+        "StandardObjectAttachmentConfiguration": (
+            SalesforceStandardObjectAttachmentConfigurationTypeDef
+        ),
         "IncludeAttachmentFilePatterns": Sequence[str],
         "ExcludeAttachmentFilePatterns": Sequence[str],
     },
     total=False,
 )
 
 class SalesforceConfigurationTypeDef(
     _RequiredSalesforceConfigurationTypeDef, _OptionalSalesforceConfigurationTypeDef
 ):
     pass
 
+_RequiredGetQuerySuggestionsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetQuerySuggestionsRequestRequestTypeDef",
+    {
+        "IndexId": str,
+        "QueryText": str,
+    },
+)
+_OptionalGetQuerySuggestionsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetQuerySuggestionsRequestRequestTypeDef",
+    {
+        "MaxSuggestionsCount": int,
+        "SuggestionTypes": Sequence[SuggestionTypeType],
+        "AttributeSuggestionsConfig": AttributeSuggestionsGetConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetQuerySuggestionsRequestRequestTypeDef(
+    _RequiredGetQuerySuggestionsRequestRequestTypeDef,
+    _OptionalGetQuerySuggestionsRequestRequestTypeDef,
+):
+    pass
+
 CustomDocumentEnrichmentConfigurationTypeDef = TypedDict(
     "CustomDocumentEnrichmentConfigurationTypeDef",
     {
         "InlineConfigurations": Sequence[InlineCustomDocumentEnrichmentConfigurationTypeDef],
         "PreExtractionHookConfiguration": HookConfigurationTypeDef,
         "PostExtractionHookConfiguration": HookConfigurationTypeDef,
         "RoleArn": str,
@@ -3426,28 +3747,38 @@
     "BatchGetDocumentStatusRequestRequestTypeDef",
     {
         "IndexId": str,
         "DocumentInfoList": Sequence[DocumentInfoTypeDef],
     },
 )
 
+RetrieveResultTypeDef = TypedDict(
+    "RetrieveResultTypeDef",
+    {
+        "QueryId": str,
+        "ResultItems": List[RetrieveResultItemTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AdditionalResultAttributeTypeDef = TypedDict(
     "AdditionalResultAttributeTypeDef",
     {
         "Key": str,
         "ValueType": Literal["TEXT_WITH_HIGHLIGHTS_VALUE"],
         "Value": AdditionalResultAttributeValueTypeDef,
     },
 )
 
 SuggestionTypeDef = TypedDict(
     "SuggestionTypeDef",
     {
         "Id": str,
         "Value": SuggestionValueTypeDef,
+        "SourceDocuments": List[SourceDocumentTypeDef],
     },
     total=False,
 )
 
 DataSourceConfigurationTypeDef = TypedDict(
     "DataSourceConfigurationTypeDef",
     {
@@ -3490,14 +3821,30 @@
 )
 
 class BatchPutDocumentRequestRequestTypeDef(
     _RequiredBatchPutDocumentRequestRequestTypeDef, _OptionalBatchPutDocumentRequestRequestTypeDef
 ):
     pass
 
+FeaturedResultsItemTypeDef = TypedDict(
+    "FeaturedResultsItemTypeDef",
+    {
+        "Id": str,
+        "Type": QueryResultTypeType,
+        "AdditionalAttributes": List[AdditionalResultAttributeTypeDef],
+        "DocumentId": str,
+        "DocumentTitle": TextWithHighlightsTypeDef,
+        "DocumentExcerpt": TextWithHighlightsTypeDef,
+        "DocumentURI": str,
+        "DocumentAttributes": List[DocumentAttributeTypeDef],
+        "FeedbackToken": str,
+    },
+    total=False,
+)
+
 QueryResultItemTypeDef = TypedDict(
     "QueryResultItemTypeDef",
     {
         "Id": str,
         "Type": QueryResultTypeType,
         "Format": QueryResultFormatType,
         "AdditionalAttributes": List[AdditionalResultAttributeTypeDef],
@@ -3514,15 +3861,15 @@
 )
 
 GetQuerySuggestionsResponseTypeDef = TypedDict(
     "GetQuerySuggestionsResponseTypeDef",
     {
         "QuerySuggestionsId": str,
         "Suggestions": List[SuggestionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceRequestRequestTypeDef",
     {
         "Name": str,
@@ -3565,15 +3912,15 @@
         "Description": str,
         "Status": DataSourceStatusType,
         "Schedule": str,
         "RoleArn": str,
         "ErrorMessage": str,
         "LanguageCode": str,
         "CustomDocumentEnrichmentConfiguration": CustomDocumentEnrichmentConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataSourceRequestRequestTypeDef",
     {
         "Id": str,
@@ -3605,10 +3952,11 @@
     {
         "QueryId": str,
         "ResultItems": List[QueryResultItemTypeDef],
         "FacetResults": List["FacetResultTypeDef"],
         "TotalNumberOfResults": int,
         "Warnings": List[WarningTypeDef],
         "SpellCorrectedQueries": List[SpellCorrectedQueryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "FeaturedResultsItems": List[FeaturedResultsItemTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/PKG-INFO` & `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kendra
-Version: 1.26.48
-Summary: Type annotations for boto3.kendra 1.26.48 service generated with mypy-boto3-builder 7.12.3
+Version: 1.27.0
+Summary: Type annotations for boto3.kendra 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-kendra"></a>
 
 # mypy-boto3-kendra
 
 [![PyPI - mypy-boto3-kendra](https://img.shields.io/pypi/v/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kendra?color=blue)](https://pypistats.org/packages/mypy-boto3-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.kendra 1.26.48](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[boto3.kendra 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
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
 [mypy-boto3-kendra docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/).
 
 See how it helps to find and fix potential bugs:
 
@@ -277,14 +277,15 @@
 `mypy_boto3_kendra.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_kendra.literals import (
     AdditionalResultAttributeValueTypeType,
     AlfrescoEntityType,
+    AttributeSuggestionsModeType,
     ConditionOperatorType,
     ConfluenceAttachmentFieldNameType,
     ConfluenceAuthenticationTypeType,
     ConfluenceBlogFieldNameType,
     ConfluencePageFieldNameType,
     ConfluenceSpaceFieldNameType,
     ConfluenceVersionType,
@@ -297,14 +298,15 @@
     DocumentStatusType,
     EndpointTypeType,
     EntityTypeType,
     ErrorCodeType,
     ExperienceStatusType,
     FaqFileFormatType,
     FaqStatusType,
+    FeaturedResultsSetStatusType,
     FsxFileSystemTypeType,
     HighlightTypeType,
     IndexEditionType,
     IndexStatusType,
     IntervalType,
     IssueSubEntityType,
     KeyLocationType,
@@ -327,14 +329,15 @@
     ScoreConfidenceType,
     ServiceNowAuthenticationTypeType,
     ServiceNowBuildVersionTypeType,
     SharePointOnlineAuthenticationTypeType,
     SharePointVersionType,
     SlackEntityType,
     SortOrderType,
+    SuggestionTypeType,
     ThesaurusStatusType,
     TypeType,
     UserContextPolicyType,
     UserGroupResolutionModeType,
     WarningCodeType,
     WebCrawlerModeType,
     kendraServiceName,
@@ -361,19 +364,21 @@
     AccessControlListConfigurationTypeDef,
     AclConfigurationTypeDef,
     DataSourceToIndexFieldMappingTypeDef,
     DataSourceVpcConfigurationTypeDef,
     S3PathTypeDef,
     EntityConfigurationTypeDef,
     FailedEntityTypeDef,
-    ResponseMetadataTypeDef,
     EntityPersonaConfigurationTypeDef,
+    SuggestableConfigTypeDef,
     BasicAuthenticationConfigurationTypeDef,
     DataSourceSyncJobMetricTargetTypeDef,
     BatchDeleteDocumentResponseFailedDocumentTypeDef,
+    BatchDeleteFeaturedResultsSetErrorTypeDef,
+    BatchDeleteFeaturedResultsSetRequestRequestTypeDef,
     BatchGetDocumentStatusResponseErrorTypeDef,
     StatusTypeDef,
     BatchPutDocumentResponseFailedDocumentTypeDef,
     CapacityUnitsConfigurationTypeDef,
     ClearQuerySuggestionsRequestRequestTypeDef,
     ClickFeedbackTypeDef,
     ConfluenceAttachmentToIndexFieldMappingTypeDef,
@@ -381,17 +386,25 @@
     ProxyConfigurationTypeDef,
     ConfluencePageToIndexFieldMappingTypeDef,
     ConfluenceSpaceToIndexFieldMappingTypeDef,
     ConnectionConfigurationTypeDef,
     ContentSourceConfigurationTypeDef,
     CorrectionTypeDef,
     PrincipalTypeDef,
+    CreateAccessControlConfigurationResponseTypeDef,
     TagTypeDef,
+    CreateDataSourceResponseTypeDef,
+    CreateExperienceResponseTypeDef,
+    CreateFaqResponseTypeDef,
+    FeaturedDocumentTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     UserGroupResolutionConfigurationTypeDef,
+    CreateIndexResponseTypeDef,
+    CreateQuerySuggestionsBlockListResponseTypeDef,
+    CreateThesaurusResponseTypeDef,
     TemplateConfigurationTypeDef,
     DataSourceGroupTypeDef,
     DataSourceSummaryTypeDef,
     DataSourceSyncJobMetricsTypeDef,
     SqlConfigurationTypeDef,
     DeleteAccessControlConfigurationRequestRequestTypeDef,
     DeleteDataSourceRequestRequestTypeDef,
@@ -402,32 +415,36 @@
     DeleteQuerySuggestionsBlockListRequestRequestTypeDef,
     DeleteThesaurusRequestRequestTypeDef,
     DescribeAccessControlConfigurationRequestRequestTypeDef,
     DescribeDataSourceRequestRequestTypeDef,
     DescribeExperienceRequestRequestTypeDef,
     ExperienceEndpointTypeDef,
     DescribeFaqRequestRequestTypeDef,
+    DescribeFeaturedResultsSetRequestRequestTypeDef,
+    FeaturedDocumentMissingTypeDef,
+    FeaturedDocumentWithMetadataTypeDef,
     DescribeIndexRequestRequestTypeDef,
     DescribePrincipalMappingRequestRequestTypeDef,
     GroupOrderingIdSummaryTypeDef,
     DescribeQuerySuggestionsBlockListRequestRequestTypeDef,
     DescribeQuerySuggestionsConfigRequestRequestTypeDef,
     DescribeThesaurusRequestRequestTypeDef,
     DisassociatePersonasFromEntitiesRequestRequestTypeDef,
     DocumentAttributeValueTypeDef,
     RelevanceTypeDef,
     SearchTypeDef,
     DocumentsMetadataConfigurationTypeDef,
+    EmptyResponseMetadataTypeDef,
     EntityDisplayDataTypeDef,
     UserIdentityConfigurationTypeDef,
     FacetResultTypeDef,
     FacetTypeDef,
     FaqStatisticsTypeDef,
     FaqSummaryTypeDef,
-    GetQuerySuggestionsRequestRequestTypeDef,
+    FeaturedResultsSetSummaryTypeDef,
     GetSnapshotsRequestRequestTypeDef,
     TimeRangeTypeDef,
     GitHubDocumentCrawlPropertiesTypeDef,
     SaaSConfigurationTypeDef,
     MemberGroupTypeDef,
     MemberUserTypeDef,
     GroupSummaryTypeDef,
@@ -439,34 +456,37 @@
     ListAccessControlConfigurationsRequestRequestTypeDef,
     ListDataSourcesRequestRequestTypeDef,
     ListEntityPersonasRequestRequestTypeDef,
     PersonasSummaryTypeDef,
     ListExperienceEntitiesRequestRequestTypeDef,
     ListExperiencesRequestRequestTypeDef,
     ListFaqsRequestRequestTypeDef,
+    ListFeaturedResultsSetsRequestRequestTypeDef,
     ListGroupsOlderThanOrderingIdRequestRequestTypeDef,
     ListIndicesRequestRequestTypeDef,
     ListQuerySuggestionsBlockListsRequestRequestTypeDef,
     QuerySuggestionsBlockListSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListThesauriRequestRequestTypeDef,
     ThesaurusSummaryTypeDef,
     SortingConfigurationTypeDef,
     SpellCorrectionConfigurationTypeDef,
     ScoreAttributesTypeDef,
     WarningTypeDef,
     RelevanceFeedbackTypeDef,
+    ResponseMetadataTypeDef,
     SeedUrlConfigurationTypeDef,
     SiteMapsConfigurationTypeDef,
     StartDataSourceSyncJobRequestRequestTypeDef,
+    StartDataSourceSyncJobResponseTypeDef,
     StopDataSourceSyncJobRequestRequestTypeDef,
     SuggestionHighlightTypeDef,
     TableCellTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateQuerySuggestionsConfigRequestRequestTypeDef,
+    ListAccessControlConfigurationsResponseTypeDef,
     ColumnConfigurationTypeDef,
     GoogleDriveConfigurationTypeDef,
     SalesforceChatterFeedConfigurationTypeDef,
     SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,
     SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,
     SalesforceStandardObjectAttachmentConfigurationTypeDef,
     SalesforceStandardObjectConfigurationTypeDef,
@@ -475,71 +495,68 @@
     WorkDocsConfigurationTypeDef,
     BoxConfigurationTypeDef,
     FsxConfigurationTypeDef,
     JiraConfigurationTypeDef,
     QuipConfigurationTypeDef,
     SlackConfigurationTypeDef,
     AlfrescoConfigurationTypeDef,
+    DescribeFaqResponseTypeDef,
+    DescribeQuerySuggestionsBlockListResponseTypeDef,
+    DescribeThesaurusResponseTypeDef,
     OnPremiseConfigurationTypeDef,
     OneDriveUsersTypeDef,
     UpdateQuerySuggestionsBlockListRequestRequestTypeDef,
     UpdateThesaurusRequestRequestTypeDef,
     AssociateEntitiesToExperienceRequestRequestTypeDef,
     DisassociateEntitiesFromExperienceRequestRequestTypeDef,
     AssociateEntitiesToExperienceResponseTypeDef,
     AssociatePersonasToEntitiesResponseTypeDef,
-    CreateAccessControlConfigurationResponseTypeDef,
-    CreateDataSourceResponseTypeDef,
-    CreateExperienceResponseTypeDef,
-    CreateFaqResponseTypeDef,
-    CreateIndexResponseTypeDef,
-    CreateQuerySuggestionsBlockListResponseTypeDef,
-    CreateThesaurusResponseTypeDef,
-    DescribeFaqResponseTypeDef,
-    DescribeQuerySuggestionsBlockListResponseTypeDef,
-    DescribeQuerySuggestionsConfigResponseTypeDef,
-    DescribeThesaurusResponseTypeDef,
     DisassociateEntitiesFromExperienceResponseTypeDef,
     DisassociatePersonasFromEntitiesResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAccessControlConfigurationsResponseTypeDef,
-    StartDataSourceSyncJobResponseTypeDef,
     AssociatePersonasToEntitiesRequestRequestTypeDef,
+    AttributeSuggestionsDescribeConfigTypeDef,
+    AttributeSuggestionsUpdateConfigTypeDef,
     AuthenticationConfigurationTypeDef,
     BatchDeleteDocumentRequestRequestTypeDef,
     BatchDeleteDocumentResponseTypeDef,
+    BatchDeleteFeaturedResultsSetResponseTypeDef,
     BatchGetDocumentStatusResponseTypeDef,
     BatchPutDocumentResponseTypeDef,
     ConfluenceAttachmentConfigurationTypeDef,
     ConfluenceBlogConfigurationTypeDef,
     SharePointConfigurationTypeDef,
     ConfluencePageConfigurationTypeDef,
     ConfluenceSpaceConfigurationTypeDef,
     SpellCorrectedQueryTypeDef,
     HierarchicalPrincipalTypeDef,
     CreateFaqRequestRequestTypeDef,
     CreateQuerySuggestionsBlockListRequestRequestTypeDef,
     CreateThesaurusRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateFeaturedResultsSetRequestRequestTypeDef,
+    FeaturedResultsSetTypeDef,
+    UpdateFeaturedResultsSetRequestRequestTypeDef,
     UserContextTypeDef,
     ListDataSourcesResponseTypeDef,
     DataSourceSyncJobTypeDef,
     ExperiencesSummaryTypeDef,
+    DescribeFeaturedResultsSetResponseTypeDef,
     DescribePrincipalMappingResponseTypeDef,
     DocumentAttributeConditionTypeDef,
     DocumentAttributeTargetTypeDef,
     DocumentAttributeTypeDef,
     DocumentAttributeValueCountPairTypeDef,
     DocumentRelevanceConfigurationTypeDef,
     DocumentMetadataConfigurationTypeDef,
     S3DataSourceConfigurationTypeDef,
     ExperienceEntitiesSummaryTypeDef,
     ExperienceConfigurationTypeDef,
     ListFaqsResponseTypeDef,
+    ListFeaturedResultsSetsResponseTypeDef,
     GetSnapshotsResponseTypeDef,
     ListDataSourceSyncJobsRequestRequestTypeDef,
     GroupMembersTypeDef,
     ListGroupsOlderThanOrderingIdResponseTypeDef,
     TextWithHighlightsTypeDef,
     ListIndicesResponseTypeDef,
     IndexStatisticsTypeDef,
@@ -552,45 +569,56 @@
     SuggestionTextWithHighlightsTypeDef,
     TableRowTypeDef,
     DatabaseConfigurationTypeDef,
     SalesforceKnowledgeArticleConfigurationTypeDef,
     ServiceNowConfigurationTypeDef,
     GitHubConfigurationTypeDef,
     OneDriveConfigurationTypeDef,
+    DescribeQuerySuggestionsConfigResponseTypeDef,
+    UpdateQuerySuggestionsConfigRequestRequestTypeDef,
     ConfluenceConfigurationTypeDef,
     CreateAccessControlConfigurationRequestRequestTypeDef,
     DescribeAccessControlConfigurationResponseTypeDef,
     UpdateAccessControlConfigurationRequestRequestTypeDef,
+    CreateFeaturedResultsSetResponseTypeDef,
+    UpdateFeaturedResultsSetResponseTypeDef,
+    AttributeSuggestionsGetConfigTypeDef,
     ListDataSourceSyncJobsResponseTypeDef,
     ListExperiencesResponseTypeDef,
     HookConfigurationTypeDef,
     InlineCustomDocumentEnrichmentConfigurationTypeDef,
     AttributeFilterTypeDef,
     DocumentInfoTypeDef,
     DocumentTypeDef,
+    RetrieveResultItemTypeDef,
+    SourceDocumentTypeDef,
     QueryRequestRequestTypeDef,
+    RetrieveRequestRequestTypeDef,
     ListExperienceEntitiesResponseTypeDef,
     CreateExperienceRequestRequestTypeDef,
     DescribeExperienceResponseTypeDef,
     UpdateExperienceRequestRequestTypeDef,
     PutPrincipalMappingRequestRequestTypeDef,
     AdditionalResultAttributeValueTypeDef,
     CreateIndexRequestRequestTypeDef,
     DescribeIndexResponseTypeDef,
     UpdateIndexRequestRequestTypeDef,
     WebCrawlerConfigurationTypeDef,
     SuggestionValueTypeDef,
     TableExcerptTypeDef,
     SalesforceConfigurationTypeDef,
+    GetQuerySuggestionsRequestRequestTypeDef,
     CustomDocumentEnrichmentConfigurationTypeDef,
     BatchGetDocumentStatusRequestRequestTypeDef,
+    RetrieveResultTypeDef,
     AdditionalResultAttributeTypeDef,
     SuggestionTypeDef,
     DataSourceConfigurationTypeDef,
     BatchPutDocumentRequestRequestTypeDef,
+    FeaturedResultsItemTypeDef,
     QueryResultItemTypeDef,
     GetQuerySuggestionsResponseTypeDef,
     CreateDataSourceRequestRequestTypeDef,
     DescribeDataSourceResponseTypeDef,
     UpdateDataSourceRequestRequestTypeDef,
     QueryResultTypeDef,
 )
@@ -603,42 +631,42 @@
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

### Comparing `mypy-boto3-kendra-1.26.48/mypy_boto3_kendra.egg-info/SOURCES.txt` & `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.26.48/setup.py` & `mypy-boto3-kendra-1.27.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Setup script for mypy-boto3-kendra.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kendra",
-    version="1.26.48",
+    version="1.27.0",
     packages=["mypy_boto3_kendra"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.kendra 1.26.48 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.kendra 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -44,11 +44,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/",
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

